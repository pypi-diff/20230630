# Comparing `tmp/JustScan-1.2.2.tar.gz` & `tmp/JustScan-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JustScan-1.2.2.tar", last modified: Fri Jun 30 09:29:05 2023, max compression
+gzip compressed data, was "JustScan-1.2.3.tar", last modified: Fri Jun 30 09:51:17 2023, max compression
```

## Comparing `JustScan-1.2.2.tar` & `JustScan-1.2.3.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.735112 JustScan-1.2.2/
--rw-r--r--   0 macbook    (501) staff       (20)     2433 2023-06-30 09:29:05.734948 JustScan-1.2.2/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     2131 2023-04-12 07:19:45.000000 JustScan-1.2.2/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.709609 JustScan-1.2.2/app/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.713949 JustScan-1.2.2/app/JustScan/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 17:20:30.000000 JustScan-1.2.2/app/JustScan/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.715303 JustScan-1.2.2/app/JustScan/api/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 09:21:37.000000 JustScan-1.2.2/app/JustScan/api/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      181 2023-06-28 10:18:54.000000 JustScan-1.2.2/app/JustScan/api/itc_cli.py
--rw-r--r--   0 macbook    (501) staff       (20)     5520 2023-06-20 17:06:38.000000 JustScan-1.2.2/app/JustScan/api/just_scan_api.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.716030 JustScan-1.2.2/app/JustScan/config/
--rw-r--r--   0 macbook    (501) staff       (20)      100 2023-06-20 07:14:31.000000 JustScan-1.2.2/app/JustScan/config/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1546 2023-06-20 10:29:43.000000 JustScan-1.2.2/app/JustScan/config/config.py
--rw-r--r--   0 macbook    (501) staff       (20)      619 2023-06-20 10:30:42.000000 JustScan-1.2.2/app/JustScan/config/config_db.py
--rw-r--r--   0 macbook    (501) staff       (20)     1872 2023-06-20 10:31:25.000000 JustScan-1.2.2/app/JustScan/config/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     4337 2023-05-09 09:10:33.000000 JustScan-1.2.2/app/JustScan/config/pydantic_models.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.716738 JustScan-1.2.2/app/JustScan/database/
--rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-20 07:14:31.000000 JustScan-1.2.2/app/JustScan/database/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     4411 2023-06-21 02:51:05.000000 JustScan-1.2.2/app/JustScan/database/crud.py
--rw-r--r--   0 macbook    (501) staff       (20)      867 2023-06-20 10:35:51.000000 JustScan-1.2.2/app/JustScan/database/data_models.py
--rw-r--r--   0 macbook    (501) staff       (20)      570 2023-06-20 17:06:38.000000 JustScan-1.2.2/app/JustScan/database/database.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.716987 JustScan-1.2.2/app/JustScan/face_id/
--rw-r--r--   0 macbook    (501) staff       (20)       66 2023-06-20 07:09:37.000000 JustScan-1.2.2/app/JustScan/face_id/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.717276 JustScan-1.2.2/app/JustScan/face_id/commons/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.718060 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/
--rw-r--r--   0 macbook    (501) staff       (20)     2206 2023-06-20 10:35:31.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2037 2023-06-20 10:35:31.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.718473 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/data_io/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/data_io/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    20275 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py
--rw-r--r--   0 macbook    (501) staff       (20)    11469 2023-06-21 02:49:42.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py
--rw-r--r--   0 macbook    (501) staff       (20)      802 2023-06-20 10:35:31.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py
--rw-r--r--   0 macbook    (501) staff       (20)     1402 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.718847 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/
--rw-r--r--   0 macbook    (501) staff       (20)    12487 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py
--rw-r--r--   0 macbook    (501) staff       (20)     2739 2023-06-20 16:58:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      990 2023-06-20 10:35:31.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/utility.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.719090 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/
--rw-r--r--   0 macbook    (501) staff       (20)     3030 2023-06-23 10:15:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)      983 2023-06-21 02:52:02.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.719669 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/
--rw-r--r--   0 macbook    (501) staff       (20)      213 2023-06-20 16:58:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3036 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/layers.py
--rw-r--r--   0 macbook    (501) staff       (20)     4293 2023-06-20 16:58:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/models.py
--rw-r--r--   0 macbook    (501) staff       (20)     2436 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.720114 JustScan-1.2.2/app/JustScan/face_id/commons/CloseEyes/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/CloseEyes/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1165 2023-06-23 10:15:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py
--rw-r--r--   0 macbook    (501) staff       (20)     1315 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/face_id/commons/CloseEyes/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.720388 JustScan-1.2.2/app/JustScan/face_id/commons/FaceMask/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/FaceMask/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      873 2023-06-23 10:15:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.720847 JustScan-1.2.2/app/JustScan/face_id/commons/FaceQuality/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/FaceQuality/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-06-01 06:55:11.000000 JustScan-1.2.2/app/JustScan/face_id/commons/FaceQuality/dom.py
--rw-r--r--   0 macbook    (501) staff       (20)     1855 2023-06-20 08:14:55.000000 JustScan-1.2.2/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.721134 JustScan-1.2.2/app/JustScan/face_id/commons/ScrFd/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ScrFd/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    12656 2023-06-23 10:15:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ScrFd/scrfd.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/face_id/commons/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2297 2023-06-19 18:18:48.000000 JustScan-1.2.2/app/JustScan/face_id/commons/config.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.721738 JustScan-1.2.2/app/JustScan/face_id/libraries/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/face_id/libraries/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7235 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/face_id/libraries/face_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)     5325 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/face_id/libraries/face_id.py
--rw-r--r--   0 macbook    (501) staff       (20)      395 2023-06-20 08:01:32.000000 JustScan-1.2.2/app/JustScan/face_id/libraries/face_recognition.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.722028 JustScan-1.2.2/app/JustScan/face_id/tools/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/face_id/tools/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3955 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/face_id/tools/modules.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.722180 JustScan-1.2.2/app/JustScan/ocr/
--rw-r--r--   0 macbook    (501) staff       (20)       19 2023-06-20 07:08:18.000000 JustScan-1.2.2/app/JustScan/ocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.722351 JustScan-1.2.2/app/JustScan/ocr/core/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:27:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.723237 JustScan-1.2.2/app/JustScan/ocr/core/commons/
--rw-r--r--   0 macbook    (501) staff       (20)      851 2023-06-22 07:17:17.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/SpoofingNID.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7192 2023-06-30 07:02:41.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/config.py
--rw-r--r--   0 macbook    (501) staff       (20)      817 2023-06-22 07:17:17.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/id_card_classification.py
--rw-r--r--   0 macbook    (501) staff       (20)     4112 2023-06-30 09:27:04.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/id_card_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)     1764 2023-06-30 09:27:04.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/merge_model.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.723514 JustScan-1.2.2/app/JustScan/ocr/core/commons/utils/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/utils/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1887 2023-06-26 04:13:41.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/utils/utils_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.723637 JustScan-1.2.2/app/JustScan/ocr/core/modules/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.724031 JustScan-1.2.2/app/JustScan/ocr/core/modules/corner_detection/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/corner_detection/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1145 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py
--rw-r--r--   0 macbook    (501) staff       (20)     3973 2023-06-19 14:29:56.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/corner_detection/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.724367 JustScan-1.2.2/app/JustScan/ocr/core/modules/id_card_classification/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/id_card_classification/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      923 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/id_card_classification/classify.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.724859 JustScan-1.2.2/app/JustScan/ocr/core/modules/mrc/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/mrc/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2938 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/mrc/mrc_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)      627 2023-06-20 08:24:11.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/mrc/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.726553 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9072 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/passport.py
--rw-r--r--   0 macbook    (501) staff       (20)      510 2023-06-20 08:24:11.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/passport_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)     2288 2023-06-20 08:30:21.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.727123 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3248 2023-04-18 08:29:08.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py
--rw-r--r--   0 macbook    (501) staff       (20)     4344 2023-04-18 03:26:14.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.727538 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_detect_passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_detect_passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9668 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.727879 JustScan-1.2.2/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-26 09:38:30.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2936 2023-06-21 02:53:49.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.728394 JustScan-1.2.2/app/JustScan/ocr/core/modules/spell_checking/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/spell_checking/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2350 2023-05-10 09:12:33.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.728761 JustScan-1.2.2/app/JustScan/ocr/core/modules/spoofing_nid/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/spoofing_nid/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      935 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.729206 JustScan-1.2.2/app/JustScan/ocr/core/modules/text_detection/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/text_detection/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7241 2023-06-28 09:47:49.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/text_detection/dictionary.py
--rw-r--r--   0 macbook    (501) staff       (20)    11602 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/text_detection/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.729600 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.729894 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-27 08:50:27.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     8899 2023-06-26 11:05:01.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/trt_loader.py
--rw-r--r--   0 macbook    (501) staff       (20)     2539 2023-06-27 09:39:17.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)     3719 2023-06-27 09:48:38.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_trt.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.730282 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.730841 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py
--rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py
--rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.731656 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.732256 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-20 08:38:07.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py
--rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py
--rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py
--rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.732782 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
--rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py
--rw-r--r--   0 macbook    (501) staff       (20)     1630 2023-06-20 08:38:07.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py
--rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.733149 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
--rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py
--rw-r--r--   0 macbook    (501) staff       (20)      538 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.733387 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.734261 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-06-20 08:39:08.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py
--rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py
--rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     1445 2023-06-20 16:58:59.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py
--rw-r--r--   0 macbook    (501) staff       (20)     8785 2023-06-27 09:40:05.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py
--rw-r--r--   0 macbook    (501) staff       (20)     2690 2023-06-27 09:25:01.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.734748 JustScan-1.2.2/app/JustScan/ocr/core/tools/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/ocr/core/tools/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     5552 2023-04-18 03:26:14.000000 JustScan-1.2.2/app/JustScan/ocr/core/tools/api_json.py
--rw-r--r--   0 macbook    (501) staff       (20)     5533 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/tools/dictionaries.py
--rw-r--r--   0 macbook    (501) staff       (20)     2518 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/tools/functional.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.714885 JustScan-1.2.2/app/JustScan.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     2433 2023-06-30 09:29:05.000000 JustScan-1.2.2/app/JustScan.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     7418 2023-06-30 09:29:05.000000 JustScan-1.2.2/app/JustScan.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-30 09:29:05.000000 JustScan-1.2.2/app/JustScan.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       58 2023-06-30 09:29:05.000000 JustScan-1.2.2/app/JustScan.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)      865 2023-06-30 09:29:05.000000 JustScan-1.2.2/app/JustScan.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        9 2023-06-30 09:29:05.000000 JustScan-1.2.2/app/JustScan.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-30 09:29:05.735161 JustScan-1.2.2/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     1178 2023-06-30 09:29:04.000000 JustScan-1.2.2/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.797879 JustScan-1.2.3/
+-rw-r--r--   0 macbook    (501) staff       (20)     2433 2023-06-30 09:51:17.797721 JustScan-1.2.3/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     2131 2023-04-12 07:19:45.000000 JustScan-1.2.3/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.770457 JustScan-1.2.3/app/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.774480 JustScan-1.2.3/app/JustScan/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 17:20:30.000000 JustScan-1.2.3/app/JustScan/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.775655 JustScan-1.2.3/app/JustScan/api/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 09:21:37.000000 JustScan-1.2.3/app/JustScan/api/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      181 2023-06-28 10:18:54.000000 JustScan-1.2.3/app/JustScan/api/itc_cli.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5520 2023-06-20 17:06:38.000000 JustScan-1.2.3/app/JustScan/api/just_scan_api.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.776308 JustScan-1.2.3/app/JustScan/config/
+-rw-r--r--   0 macbook    (501) staff       (20)      100 2023-06-20 07:14:31.000000 JustScan-1.2.3/app/JustScan/config/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1546 2023-06-20 10:29:43.000000 JustScan-1.2.3/app/JustScan/config/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)      619 2023-06-20 10:30:42.000000 JustScan-1.2.3/app/JustScan/config/config_db.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1872 2023-06-20 10:31:25.000000 JustScan-1.2.3/app/JustScan/config/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4337 2023-05-09 09:10:33.000000 JustScan-1.2.3/app/JustScan/config/pydantic_models.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.776844 JustScan-1.2.3/app/JustScan/database/
+-rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-20 07:14:31.000000 JustScan-1.2.3/app/JustScan/database/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4411 2023-06-21 02:51:05.000000 JustScan-1.2.3/app/JustScan/database/crud.py
+-rw-r--r--   0 macbook    (501) staff       (20)      867 2023-06-20 10:35:51.000000 JustScan-1.2.3/app/JustScan/database/data_models.py
+-rw-r--r--   0 macbook    (501) staff       (20)      570 2023-06-20 17:06:38.000000 JustScan-1.2.3/app/JustScan/database/database.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.776980 JustScan-1.2.3/app/JustScan/face_id/
+-rw-r--r--   0 macbook    (501) staff       (20)       66 2023-06-20 07:09:37.000000 JustScan-1.2.3/app/JustScan/face_id/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.777219 JustScan-1.2.3/app/JustScan/face_id/commons/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.777989 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/
+-rw-r--r--   0 macbook    (501) staff       (20)     2206 2023-06-20 10:35:31.000000 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2037 2023-06-20 10:35:31.000000 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.778433 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/data_io/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/data_io/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    20275 2023-04-12 07:19:45.000000 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11469 2023-06-21 02:49:42.000000 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py
+-rw-r--r--   0 macbook    (501) staff       (20)      802 2023-06-20 10:35:31.000000 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1402 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.778834 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/model_lib/
+-rw-r--r--   0 macbook    (501) staff       (20)    12487 2023-04-12 07:19:45.000000 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2739 2023-06-20 16:58:59.000000 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/model_lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      990 2023-06-20 10:35:31.000000 JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/utility.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.779082 JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/
+-rw-r--r--   0 macbook    (501) staff       (20)     3030 2023-06-23 10:15:59.000000 JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)      983 2023-06-21 02:52:02.000000 JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.779600 JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/lib/
+-rw-r--r--   0 macbook    (501) staff       (20)      213 2023-06-20 16:58:59.000000 JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3036 2023-04-12 07:19:45.000000 JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/lib/layers.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4293 2023-06-20 16:58:59.000000 JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/lib/models.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2436 2023-04-12 07:19:45.000000 JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/lib/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.779980 JustScan-1.2.3/app/JustScan/face_id/commons/CloseEyes/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.3/app/JustScan/face_id/commons/CloseEyes/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1165 2023-06-23 10:15:59.000000 JustScan-1.2.3/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1315 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/face_id/commons/CloseEyes/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.780212 JustScan-1.2.3/app/JustScan/face_id/commons/FaceMask/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.3/app/JustScan/face_id/commons/FaceMask/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      873 2023-06-23 10:15:59.000000 JustScan-1.2.3/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.780635 JustScan-1.2.3/app/JustScan/face_id/commons/FaceQuality/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.3/app/JustScan/face_id/commons/FaceQuality/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-06-01 06:55:11.000000 JustScan-1.2.3/app/JustScan/face_id/commons/FaceQuality/dom.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1855 2023-06-20 08:14:55.000000 JustScan-1.2.3/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.780951 JustScan-1.2.3/app/JustScan/face_id/commons/ScrFd/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.3/app/JustScan/face_id/commons/ScrFd/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    12656 2023-06-23 10:15:59.000000 JustScan-1.2.3/app/JustScan/face_id/commons/ScrFd/scrfd.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.3/app/JustScan/face_id/commons/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2297 2023-06-19 18:18:48.000000 JustScan-1.2.3/app/JustScan/face_id/commons/config.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.781575 JustScan-1.2.3/app/JustScan/face_id/libraries/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.3/app/JustScan/face_id/libraries/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7235 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/face_id/libraries/face_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5325 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/face_id/libraries/face_id.py
+-rw-r--r--   0 macbook    (501) staff       (20)      395 2023-06-20 08:01:32.000000 JustScan-1.2.3/app/JustScan/face_id/libraries/face_recognition.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.782005 JustScan-1.2.3/app/JustScan/face_id/tools/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.3/app/JustScan/face_id/tools/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3955 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/face_id/tools/modules.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.782180 JustScan-1.2.3/app/JustScan/ocr/
+-rw-r--r--   0 macbook    (501) staff       (20)       19 2023-06-20 07:08:18.000000 JustScan-1.2.3/app/JustScan/ocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.782335 JustScan-1.2.3/app/JustScan/ocr/core/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:27:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.783306 JustScan-1.2.3/app/JustScan/ocr/core/commons/
+-rw-r--r--   0 macbook    (501) staff       (20)      851 2023-06-22 07:17:17.000000 JustScan-1.2.3/app/JustScan/ocr/core/commons/SpoofingNID.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.3/app/JustScan/ocr/core/commons/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7194 2023-06-30 09:50:45.000000 JustScan-1.2.3/app/JustScan/ocr/core/commons/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)      817 2023-06-22 07:17:17.000000 JustScan-1.2.3/app/JustScan/ocr/core/commons/id_card_classification.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4112 2023-06-30 09:27:04.000000 JustScan-1.2.3/app/JustScan/ocr/core/commons/id_card_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1764 2023-06-30 09:27:04.000000 JustScan-1.2.3/app/JustScan/ocr/core/commons/merge_model.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.783616 JustScan-1.2.3/app/JustScan/ocr/core/commons/utils/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 JustScan-1.2.3/app/JustScan/ocr/core/commons/utils/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1887 2023-06-26 04:13:41.000000 JustScan-1.2.3/app/JustScan/ocr/core/commons/utils/utils_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.783793 JustScan-1.2.3/app/JustScan/ocr/core/modules/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.788102 JustScan-1.2.3/app/JustScan/ocr/core/modules/corner_detection/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/corner_detection/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1145 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3973 2023-06-19 14:29:56.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/corner_detection/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.788555 JustScan-1.2.3/app/JustScan/ocr/core/modules/id_card_classification/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/id_card_classification/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      923 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/id_card_classification/classify.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.789065 JustScan-1.2.3/app/JustScan/ocr/core/modules/mrc/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/mrc/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2938 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/mrc/mrc_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)      627 2023-06-20 08:24:11.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/mrc/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.789739 JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9072 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/passport.py
+-rw-r--r--   0 macbook    (501) staff       (20)      510 2023-06-20 08:24:11.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/passport_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2288 2023-06-20 08:30:21.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.790219 JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/utils_align_passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/utils_align_passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3248 2023-04-18 08:29:08.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4344 2023-04-18 03:26:14.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.790485 JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/utils_detect_passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/utils_detect_passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9668 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.790785 JustScan-1.2.3/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-26 09:38:30.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2936 2023-06-21 02:53:49.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.791076 JustScan-1.2.3/app/JustScan/ocr/core/modules/spell_checking/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/spell_checking/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2350 2023-05-10 09:12:33.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.791588 JustScan-1.2.3/app/JustScan/ocr/core/modules/spoofing_nid/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/spoofing_nid/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      935 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.792031 JustScan-1.2.3/app/JustScan/ocr/core/modules/text_detection/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/text_detection/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7241 2023-06-28 09:47:49.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/text_detection/dictionary.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11602 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/text_detection/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.792448 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.792739 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-27 08:50:27.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     8899 2023-06-26 11:05:01.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/trt_loader.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2539 2023-06-27 09:39:17.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3719 2023-06-27 09:48:38.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_trt.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.793113 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.793638 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py
+-rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.794304 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.794831 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-20 08:38:07.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.795378 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
+-rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1630 2023-06-20 08:38:07.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py
+-rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.795774 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py
+-rw-r--r--   0 macbook    (501) staff       (20)      538 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.796026 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.796993 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-06-20 08:39:08.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py
+-rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1445 2023-06-20 16:58:59.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py
+-rw-r--r--   0 macbook    (501) staff       (20)     8785 2023-06-27 09:40:05.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2690 2023-06-27 09:25:01.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.797520 JustScan-1.2.3/app/JustScan/ocr/core/tools/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.3/app/JustScan/ocr/core/tools/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5552 2023-04-18 03:26:14.000000 JustScan-1.2.3/app/JustScan/ocr/core/tools/api_json.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5533 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/ocr/core/tools/dictionaries.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2518 2023-06-20 17:16:54.000000 JustScan-1.2.3/app/JustScan/ocr/core/tools/functional.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:51:17.775290 JustScan-1.2.3/app/JustScan.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     2433 2023-06-30 09:51:17.000000 JustScan-1.2.3/app/JustScan.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     7418 2023-06-30 09:51:17.000000 JustScan-1.2.3/app/JustScan.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-30 09:51:17.000000 JustScan-1.2.3/app/JustScan.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       58 2023-06-30 09:51:17.000000 JustScan-1.2.3/app/JustScan.egg-info/entry_points.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      865 2023-06-30 09:51:17.000000 JustScan-1.2.3/app/JustScan.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        9 2023-06-30 09:51:17.000000 JustScan-1.2.3/app/JustScan.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-30 09:51:17.797926 JustScan-1.2.3/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1178 2023-06-30 09:51:13.000000 JustScan-1.2.3/setup.py
```

### Comparing `JustScan-1.2.2/PKG-INFO` & `JustScan-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustScan
-Version: 1.2.2
+Version: 1.2.3
 Summary: E-kyc for Industries application
 Home-page: https://gitlab.itcgroup.io/Theodore.vo
 Author: Theodore
 Author-email: theodore.v@itcgroup.io
 License: MIT
 Keywords: ITC,AI,E-kyc,Deep Learning,Computer Vision,Yolov5,Interface
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `JustScan-1.2.2/README.md` & `JustScan-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/api/just_scan_api.py` & `JustScan-1.2.3/app/JustScan/api/just_scan_api.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/config/config.py` & `JustScan-1.2.3/app/JustScan/config/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/config/config_db.py` & `JustScan-1.2.3/app/JustScan/config/config_db.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/config/logger.py` & `JustScan-1.2.3/app/JustScan/config/logger.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/config/pydantic_models.py` & `JustScan-1.2.3/app/JustScan/config/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/database/crud.py` & `JustScan-1.2.3/app/JustScan/database/crud.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/database/data_models.py` & `JustScan-1.2.3/app/JustScan/database/data_models.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/database/database.py` & `JustScan-1.2.3/app/JustScan/database/database.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/utility.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/AntiSpoof/utility.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/__init__.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/__init__.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/layers.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/lib/layers.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/models.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/lib/models.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/utils.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/ArcFace/lib/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/CloseEyes/utils.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/CloseEyes/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/FaceQuality/dom.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/FaceQuality/dom.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/ScrFd/scrfd.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/ScrFd/scrfd.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/commons/config.py` & `JustScan-1.2.3/app/JustScan/face_id/commons/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/libraries/face_detection.py` & `JustScan-1.2.3/app/JustScan/face_id/libraries/face_detection.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/libraries/face_id.py` & `JustScan-1.2.3/app/JustScan/face_id/libraries/face_id.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/face_id/tools/modules.py` & `JustScan-1.2.3/app/JustScan/face_id/tools/modules.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/commons/SpoofingNID.py` & `JustScan-1.2.3/app/JustScan/ocr/core/commons/SpoofingNID.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/commons/config.py` & `JustScan-1.2.3/app/JustScan/ocr/core/commons/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,16 +78,16 @@
         crop_nid: 'lightweight_crop_cccd',
         classify: 'idcard_classify_simplified',
         anti_spoof: 'nid_liveness_check',
         passport_crop: 'crop_passport',
         passport_detect: 'detect_passport',
         mrc_crop: 'mrc_corner',
         mrc_detect: 'mrc_detect',
-        encoder: 'transformer_encoder',
-        decoder: 'transformer_decoder'
+        encoder: 'transformers_encoder',
+        decoder: 'transformers_decoder'
     }
 
     model_name = model_mapping.get(True)
     if onnx_mode:
         return save_dir(url, model_name, onnx_mode=onnx_mode)
     else:
         return save_dir(url, model_name, onnx_mode=False)
```

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/commons/id_card_classification.py` & `JustScan-1.2.3/app/JustScan/ocr/core/commons/id_card_classification.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/commons/id_card_onnx.py` & `JustScan-1.2.3/app/JustScan/ocr/core/commons/id_card_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/commons/merge_model.py` & `JustScan-1.2.3/app/JustScan/ocr/core/commons/merge_model.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/commons/utils/utils_onnx.py` & `JustScan-1.2.3/app/JustScan/ocr/core/commons/utils/utils_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/corner_detection/utils.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/corner_detection/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/id_card_classification/classify.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/id_card_classification/classify.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/mrc/mrc_detection.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/mrc/mrc_detection.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/mrc/utils.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/mrc/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/passport.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/passport.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/text_detection/dictionary.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/text_detection/dictionary.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/text_detection/utils.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/text_detection/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/trt_loader.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/trt_loader.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_trt.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_trt.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py` & `JustScan-1.2.3/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/tools/api_json.py` & `JustScan-1.2.3/app/JustScan/ocr/core/tools/api_json.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/tools/dictionaries.py` & `JustScan-1.2.3/app/JustScan/ocr/core/tools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan/ocr/core/tools/functional.py` & `JustScan-1.2.3/app/JustScan/ocr/core/tools/functional.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan.egg-info/PKG-INFO` & `JustScan-1.2.3/app/JustScan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustScan
-Version: 1.2.2
+Version: 1.2.3
 Summary: E-kyc for Industries application
 Home-page: https://gitlab.itcgroup.io/Theodore.vo
 Author: Theodore
 Author-email: theodore.v@itcgroup.io
 License: MIT
 Keywords: ITC,AI,E-kyc,Deep Learning,Computer Vision,Yolov5,Interface
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `JustScan-1.2.2/app/JustScan.egg-info/SOURCES.txt` & `JustScan-1.2.3/app/JustScan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/app/JustScan.egg-info/requires.txt` & `JustScan-1.2.3/app/JustScan.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.2/setup.py` & `JustScan-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("app/JustScan/README.md", "r") as f:
     long_description = f.read()
 with open("requirements.txt", "r") as f:
     install_requires = [line.strip() for line in f if line.strip()]
 setup(
     name="JustScan",
-    version="1.2.2",
+    version="1.2.3",
     description="E-kyc for Industries application",
     package_dir={"": "app"},
     packages=find_packages(where="./app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.itcgroup.io/Theodore.vo",
     author="Theodore",
```

