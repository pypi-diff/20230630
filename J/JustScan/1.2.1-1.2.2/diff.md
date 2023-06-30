# Comparing `tmp/JustScan-1.2.1.tar.gz` & `tmp/JustScan-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JustScan-1.2.1.tar", last modified: Wed Jun 28 10:19:07 2023, max compression
+gzip compressed data, was "JustScan-1.2.2.tar", last modified: Fri Jun 30 09:29:05 2023, max compression
```

## Comparing `JustScan-1.2.1.tar` & `JustScan-1.2.2.tar`

### file list

```diff
@@ -1,185 +1,184 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.182484 JustScan-1.2.1/
--rw-r--r--   0 macbook    (501) staff       (20)     2433 2023-06-28 10:19:07.182281 JustScan-1.2.1/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     2131 2023-04-12 07:19:45.000000 JustScan-1.2.1/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.153227 JustScan-1.2.1/app/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.158446 JustScan-1.2.1/app/JustScan/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 17:20:30.000000 JustScan-1.2.1/app/JustScan/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.160199 JustScan-1.2.1/app/JustScan/api/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 09:21:37.000000 JustScan-1.2.1/app/JustScan/api/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      181 2023-06-28 10:18:54.000000 JustScan-1.2.1/app/JustScan/api/itc_cli.py
--rw-r--r--   0 macbook    (501) staff       (20)     5520 2023-06-20 17:06:38.000000 JustScan-1.2.1/app/JustScan/api/just_scan_api.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.161073 JustScan-1.2.1/app/JustScan/config/
--rw-r--r--   0 macbook    (501) staff       (20)      100 2023-06-20 07:14:31.000000 JustScan-1.2.1/app/JustScan/config/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1546 2023-06-20 10:29:43.000000 JustScan-1.2.1/app/JustScan/config/config.py
--rw-r--r--   0 macbook    (501) staff       (20)      619 2023-06-20 10:30:42.000000 JustScan-1.2.1/app/JustScan/config/config_db.py
--rw-r--r--   0 macbook    (501) staff       (20)     1872 2023-06-20 10:31:25.000000 JustScan-1.2.1/app/JustScan/config/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     4337 2023-05-09 09:10:33.000000 JustScan-1.2.1/app/JustScan/config/pydantic_models.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.161753 JustScan-1.2.1/app/JustScan/database/
--rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-20 07:14:31.000000 JustScan-1.2.1/app/JustScan/database/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     4411 2023-06-21 02:51:05.000000 JustScan-1.2.1/app/JustScan/database/crud.py
--rw-r--r--   0 macbook    (501) staff       (20)      867 2023-06-20 10:35:51.000000 JustScan-1.2.1/app/JustScan/database/data_models.py
--rw-r--r--   0 macbook    (501) staff       (20)      570 2023-06-20 17:06:38.000000 JustScan-1.2.1/app/JustScan/database/database.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.161925 JustScan-1.2.1/app/JustScan/face_id/
--rw-r--r--   0 macbook    (501) staff       (20)       66 2023-06-20 07:09:37.000000 JustScan-1.2.1/app/JustScan/face_id/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.162248 JustScan-1.2.1/app/JustScan/face_id/commons/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.163246 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/
--rw-r--r--   0 macbook    (501) staff       (20)     2206 2023-06-20 10:35:31.000000 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2037 2023-06-20 10:35:31.000000 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.163788 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/data_io/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/data_io/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    20275 2023-04-12 07:19:45.000000 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py
--rw-r--r--   0 macbook    (501) staff       (20)    11469 2023-06-21 02:49:42.000000 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py
--rw-r--r--   0 macbook    (501) staff       (20)      802 2023-06-20 10:35:31.000000 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py
--rw-r--r--   0 macbook    (501) staff       (20)     1402 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.164328 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/model_lib/
--rw-r--r--   0 macbook    (501) staff       (20)    12487 2023-04-12 07:19:45.000000 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py
--rw-r--r--   0 macbook    (501) staff       (20)     2739 2023-06-20 16:58:59.000000 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/model_lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      990 2023-06-20 10:35:31.000000 JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/utility.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.164641 JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/
--rw-r--r--   0 macbook    (501) staff       (20)     3030 2023-06-23 10:15:59.000000 JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)      983 2023-06-21 02:52:02.000000 JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.165356 JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/lib/
--rw-r--r--   0 macbook    (501) staff       (20)      213 2023-06-20 16:58:59.000000 JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3036 2023-04-12 07:19:45.000000 JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/lib/layers.py
--rw-r--r--   0 macbook    (501) staff       (20)     4293 2023-06-20 16:58:59.000000 JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/lib/models.py
--rw-r--r--   0 macbook    (501) staff       (20)     2436 2023-04-12 07:19:45.000000 JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/lib/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.165907 JustScan-1.2.1/app/JustScan/face_id/commons/CloseEyes/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.1/app/JustScan/face_id/commons/CloseEyes/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1165 2023-06-23 10:15:59.000000 JustScan-1.2.1/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py
--rw-r--r--   0 macbook    (501) staff       (20)     1315 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/face_id/commons/CloseEyes/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.166234 JustScan-1.2.1/app/JustScan/face_id/commons/FaceMask/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.1/app/JustScan/face_id/commons/FaceMask/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      873 2023-06-23 10:15:59.000000 JustScan-1.2.1/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.166693 JustScan-1.2.1/app/JustScan/face_id/commons/FaceQuality/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.1/app/JustScan/face_id/commons/FaceQuality/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-06-01 06:55:11.000000 JustScan-1.2.1/app/JustScan/face_id/commons/FaceQuality/dom.py
--rw-r--r--   0 macbook    (501) staff       (20)     1855 2023-06-20 08:14:55.000000 JustScan-1.2.1/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.166988 JustScan-1.2.1/app/JustScan/face_id/commons/ScrFd/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.1/app/JustScan/face_id/commons/ScrFd/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    12656 2023-06-23 10:15:59.000000 JustScan-1.2.1/app/JustScan/face_id/commons/ScrFd/scrfd.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.1/app/JustScan/face_id/commons/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2297 2023-06-19 18:18:48.000000 JustScan-1.2.1/app/JustScan/face_id/commons/config.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.167640 JustScan-1.2.1/app/JustScan/face_id/libraries/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.1/app/JustScan/face_id/libraries/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7235 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/face_id/libraries/face_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)     5325 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/face_id/libraries/face_id.py
--rw-r--r--   0 macbook    (501) staff       (20)      395 2023-06-20 08:01:32.000000 JustScan-1.2.1/app/JustScan/face_id/libraries/face_recognition.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.167929 JustScan-1.2.1/app/JustScan/face_id/tools/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.1/app/JustScan/face_id/tools/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3955 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/face_id/tools/modules.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.168092 JustScan-1.2.1/app/JustScan/ocr/
--rw-r--r--   0 macbook    (501) staff       (20)       19 2023-06-20 07:08:18.000000 JustScan-1.2.1/app/JustScan/ocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.168277 JustScan-1.2.1/app/JustScan/ocr/core/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:27:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.169382 JustScan-1.2.1/app/JustScan/ocr/core/commons/
--rw-r--r--   0 macbook    (501) staff       (20)      851 2023-06-22 07:17:17.000000 JustScan-1.2.1/app/JustScan/ocr/core/commons/SpoofingNID.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.1/app/JustScan/ocr/core/commons/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7951 2023-06-28 09:47:49.000000 JustScan-1.2.1/app/JustScan/ocr/core/commons/config.py
--rw-r--r--   0 macbook    (501) staff       (20)      817 2023-06-22 07:17:17.000000 JustScan-1.2.1/app/JustScan/ocr/core/commons/id_card_classification.py
--rw-r--r--   0 macbook    (501) staff       (20)     5392 2023-06-28 10:15:34.000000 JustScan-1.2.1/app/JustScan/ocr/core/commons/id_card_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)     5573 2023-06-26 05:02:01.000000 JustScan-1.2.1/app/JustScan/ocr/core/commons/id_card_trt.py
--rw-r--r--   0 macbook    (501) staff       (20)     1651 2023-06-26 06:35:58.000000 JustScan-1.2.1/app/JustScan/ocr/core/commons/merge_model.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.169672 JustScan-1.2.1/app/JustScan/ocr/core/commons/utils/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 JustScan-1.2.1/app/JustScan/ocr/core/commons/utils/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1887 2023-06-26 04:13:41.000000 JustScan-1.2.1/app/JustScan/ocr/core/commons/utils/utils_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.169856 JustScan-1.2.1/app/JustScan/ocr/core/modules/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.170342 JustScan-1.2.1/app/JustScan/ocr/core/modules/corner_detection/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/corner_detection/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1145 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py
--rw-r--r--   0 macbook    (501) staff       (20)     3973 2023-06-19 14:29:56.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/corner_detection/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.170687 JustScan-1.2.1/app/JustScan/ocr/core/modules/id_card_classification/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/id_card_classification/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      923 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/id_card_classification/classify.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.171179 JustScan-1.2.1/app/JustScan/ocr/core/modules/mrc/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/mrc/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2938 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/mrc/mrc_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)      627 2023-06-20 08:24:11.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/mrc/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.171897 JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9072 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/passport.py
--rw-r--r--   0 macbook    (501) staff       (20)      510 2023-06-20 08:24:11.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/passport_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)     2288 2023-06-20 08:30:21.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.172509 JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/utils_align_passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/utils_align_passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3248 2023-04-18 08:29:08.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py
--rw-r--r--   0 macbook    (501) staff       (20)     4344 2023-04-18 03:26:14.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.172952 JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/utils_detect_passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/utils_detect_passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9668 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.173394 JustScan-1.2.1/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-26 09:38:30.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2936 2023-06-21 02:53:49.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.173813 JustScan-1.2.1/app/JustScan/ocr/core/modules/spell_checking/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/spell_checking/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2350 2023-05-10 09:12:33.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.174218 JustScan-1.2.1/app/JustScan/ocr/core/modules/spoofing_nid/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/spoofing_nid/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      935 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.174831 JustScan-1.2.1/app/JustScan/ocr/core/modules/text_detection/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/text_detection/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7241 2023-06-28 09:47:49.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/text_detection/dictionary.py
--rw-r--r--   0 macbook    (501) staff       (20)    11602 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/text_detection/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.175597 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.176084 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-27 08:50:27.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     8899 2023-06-26 11:05:01.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/trt_loader.py
--rw-r--r--   0 macbook    (501) staff       (20)     2539 2023-06-27 09:39:17.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)     3719 2023-06-27 09:48:38.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_trt.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.176577 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.177259 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py
--rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py
--rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.178097 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.178782 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-20 08:38:07.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py
--rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py
--rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py
--rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.179461 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
--rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py
--rw-r--r--   0 macbook    (501) staff       (20)     1630 2023-06-20 08:38:07.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py
--rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.179927 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
--rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py
--rw-r--r--   0 macbook    (501) staff       (20)      538 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.180214 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.181329 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-06-20 08:39:08.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py
--rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py
--rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     1445 2023-06-20 16:58:59.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py
--rw-r--r--   0 macbook    (501) staff       (20)     8785 2023-06-27 09:40:05.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py
--rw-r--r--   0 macbook    (501) staff       (20)     2690 2023-06-27 09:25:01.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.181948 JustScan-1.2.1/app/JustScan/ocr/core/tools/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.1/app/JustScan/ocr/core/tools/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     5552 2023-04-18 03:26:14.000000 JustScan-1.2.1/app/JustScan/ocr/core/tools/api_json.py
--rw-r--r--   0 macbook    (501) staff       (20)     5533 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/ocr/core/tools/dictionaries.py
--rw-r--r--   0 macbook    (501) staff       (20)     2518 2023-06-20 17:16:54.000000 JustScan-1.2.1/app/JustScan/ocr/core/tools/functional.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-28 10:19:07.159719 JustScan-1.2.1/app/JustScan.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     2433 2023-06-28 10:19:07.000000 JustScan-1.2.1/app/JustScan.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     7463 2023-06-28 10:19:07.000000 JustScan-1.2.1/app/JustScan.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-28 10:19:07.000000 JustScan-1.2.1/app/JustScan.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       58 2023-06-28 10:19:07.000000 JustScan-1.2.1/app/JustScan.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)      865 2023-06-28 10:19:07.000000 JustScan-1.2.1/app/JustScan.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        9 2023-06-28 10:19:07.000000 JustScan-1.2.1/app/JustScan.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-28 10:19:07.182555 JustScan-1.2.1/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     1178 2023-06-28 10:19:01.000000 JustScan-1.2.1/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.735112 JustScan-1.2.2/
+-rw-r--r--   0 macbook    (501) staff       (20)     2433 2023-06-30 09:29:05.734948 JustScan-1.2.2/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     2131 2023-04-12 07:19:45.000000 JustScan-1.2.2/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.709609 JustScan-1.2.2/app/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.713949 JustScan-1.2.2/app/JustScan/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 17:20:30.000000 JustScan-1.2.2/app/JustScan/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.715303 JustScan-1.2.2/app/JustScan/api/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 09:21:37.000000 JustScan-1.2.2/app/JustScan/api/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      181 2023-06-28 10:18:54.000000 JustScan-1.2.2/app/JustScan/api/itc_cli.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5520 2023-06-20 17:06:38.000000 JustScan-1.2.2/app/JustScan/api/just_scan_api.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.716030 JustScan-1.2.2/app/JustScan/config/
+-rw-r--r--   0 macbook    (501) staff       (20)      100 2023-06-20 07:14:31.000000 JustScan-1.2.2/app/JustScan/config/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1546 2023-06-20 10:29:43.000000 JustScan-1.2.2/app/JustScan/config/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)      619 2023-06-20 10:30:42.000000 JustScan-1.2.2/app/JustScan/config/config_db.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1872 2023-06-20 10:31:25.000000 JustScan-1.2.2/app/JustScan/config/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4337 2023-05-09 09:10:33.000000 JustScan-1.2.2/app/JustScan/config/pydantic_models.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.716738 JustScan-1.2.2/app/JustScan/database/
+-rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-20 07:14:31.000000 JustScan-1.2.2/app/JustScan/database/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4411 2023-06-21 02:51:05.000000 JustScan-1.2.2/app/JustScan/database/crud.py
+-rw-r--r--   0 macbook    (501) staff       (20)      867 2023-06-20 10:35:51.000000 JustScan-1.2.2/app/JustScan/database/data_models.py
+-rw-r--r--   0 macbook    (501) staff       (20)      570 2023-06-20 17:06:38.000000 JustScan-1.2.2/app/JustScan/database/database.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.716987 JustScan-1.2.2/app/JustScan/face_id/
+-rw-r--r--   0 macbook    (501) staff       (20)       66 2023-06-20 07:09:37.000000 JustScan-1.2.2/app/JustScan/face_id/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.717276 JustScan-1.2.2/app/JustScan/face_id/commons/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.718060 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/
+-rw-r--r--   0 macbook    (501) staff       (20)     2206 2023-06-20 10:35:31.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2037 2023-06-20 10:35:31.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.718473 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/data_io/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/data_io/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    20275 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11469 2023-06-21 02:49:42.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py
+-rw-r--r--   0 macbook    (501) staff       (20)      802 2023-06-20 10:35:31.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1402 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.718847 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/
+-rw-r--r--   0 macbook    (501) staff       (20)    12487 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2739 2023-06-20 16:58:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      990 2023-06-20 10:35:31.000000 JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/utility.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.719090 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/
+-rw-r--r--   0 macbook    (501) staff       (20)     3030 2023-06-23 10:15:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)      983 2023-06-21 02:52:02.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.719669 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/
+-rw-r--r--   0 macbook    (501) staff       (20)      213 2023-06-20 16:58:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3036 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/layers.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4293 2023-06-20 16:58:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/models.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2436 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.720114 JustScan-1.2.2/app/JustScan/face_id/commons/CloseEyes/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/CloseEyes/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1165 2023-06-23 10:15:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1315 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/face_id/commons/CloseEyes/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.720388 JustScan-1.2.2/app/JustScan/face_id/commons/FaceMask/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/FaceMask/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      873 2023-06-23 10:15:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.720847 JustScan-1.2.2/app/JustScan/face_id/commons/FaceQuality/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/FaceQuality/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-06-01 06:55:11.000000 JustScan-1.2.2/app/JustScan/face_id/commons/FaceQuality/dom.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1855 2023-06-20 08:14:55.000000 JustScan-1.2.2/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.721134 JustScan-1.2.2/app/JustScan/face_id/commons/ScrFd/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ScrFd/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    12656 2023-06-23 10:15:59.000000 JustScan-1.2.2/app/JustScan/face_id/commons/ScrFd/scrfd.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/face_id/commons/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2297 2023-06-19 18:18:48.000000 JustScan-1.2.2/app/JustScan/face_id/commons/config.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.721738 JustScan-1.2.2/app/JustScan/face_id/libraries/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/face_id/libraries/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7235 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/face_id/libraries/face_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5325 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/face_id/libraries/face_id.py
+-rw-r--r--   0 macbook    (501) staff       (20)      395 2023-06-20 08:01:32.000000 JustScan-1.2.2/app/JustScan/face_id/libraries/face_recognition.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.722028 JustScan-1.2.2/app/JustScan/face_id/tools/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/face_id/tools/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3955 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/face_id/tools/modules.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.722180 JustScan-1.2.2/app/JustScan/ocr/
+-rw-r--r--   0 macbook    (501) staff       (20)       19 2023-06-20 07:08:18.000000 JustScan-1.2.2/app/JustScan/ocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.722351 JustScan-1.2.2/app/JustScan/ocr/core/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:27:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.723237 JustScan-1.2.2/app/JustScan/ocr/core/commons/
+-rw-r--r--   0 macbook    (501) staff       (20)      851 2023-06-22 07:17:17.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/SpoofingNID.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7192 2023-06-30 07:02:41.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)      817 2023-06-22 07:17:17.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/id_card_classification.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4112 2023-06-30 09:27:04.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/id_card_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1764 2023-06-30 09:27:04.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/merge_model.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.723514 JustScan-1.2.2/app/JustScan/ocr/core/commons/utils/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/utils/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1887 2023-06-26 04:13:41.000000 JustScan-1.2.2/app/JustScan/ocr/core/commons/utils/utils_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.723637 JustScan-1.2.2/app/JustScan/ocr/core/modules/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.724031 JustScan-1.2.2/app/JustScan/ocr/core/modules/corner_detection/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/corner_detection/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1145 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3973 2023-06-19 14:29:56.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/corner_detection/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.724367 JustScan-1.2.2/app/JustScan/ocr/core/modules/id_card_classification/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/id_card_classification/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      923 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/id_card_classification/classify.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.724859 JustScan-1.2.2/app/JustScan/ocr/core/modules/mrc/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/mrc/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2938 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/mrc/mrc_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)      627 2023-06-20 08:24:11.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/mrc/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.726553 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9072 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/passport.py
+-rw-r--r--   0 macbook    (501) staff       (20)      510 2023-06-20 08:24:11.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/passport_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2288 2023-06-20 08:30:21.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.727123 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3248 2023-04-18 08:29:08.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4344 2023-04-18 03:26:14.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.727538 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_detect_passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_detect_passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9668 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.727879 JustScan-1.2.2/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-26 09:38:30.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2936 2023-06-21 02:53:49.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.728394 JustScan-1.2.2/app/JustScan/ocr/core/modules/spell_checking/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/spell_checking/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2350 2023-05-10 09:12:33.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.728761 JustScan-1.2.2/app/JustScan/ocr/core/modules/spoofing_nid/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/spoofing_nid/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      935 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.729206 JustScan-1.2.2/app/JustScan/ocr/core/modules/text_detection/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/text_detection/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7241 2023-06-28 09:47:49.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/text_detection/dictionary.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11602 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/text_detection/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.729600 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.729894 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-27 08:50:27.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     8899 2023-06-26 11:05:01.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/trt_loader.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2539 2023-06-27 09:39:17.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3719 2023-06-27 09:48:38.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_trt.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.730282 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.730841 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py
+-rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.731656 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.732256 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-20 08:38:07.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.732782 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
+-rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1630 2023-06-20 08:38:07.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py
+-rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.733149 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py
+-rw-r--r--   0 macbook    (501) staff       (20)      538 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.733387 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.734261 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-06-20 08:39:08.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py
+-rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1445 2023-06-20 16:58:59.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py
+-rw-r--r--   0 macbook    (501) staff       (20)     8785 2023-06-27 09:40:05.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2690 2023-06-27 09:25:01.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.734748 JustScan-1.2.2/app/JustScan/ocr/core/tools/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.2.2/app/JustScan/ocr/core/tools/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5552 2023-04-18 03:26:14.000000 JustScan-1.2.2/app/JustScan/ocr/core/tools/api_json.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5533 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/tools/dictionaries.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2518 2023-06-20 17:16:54.000000 JustScan-1.2.2/app/JustScan/ocr/core/tools/functional.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-30 09:29:05.714885 JustScan-1.2.2/app/JustScan.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     2433 2023-06-30 09:29:05.000000 JustScan-1.2.2/app/JustScan.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     7418 2023-06-30 09:29:05.000000 JustScan-1.2.2/app/JustScan.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-30 09:29:05.000000 JustScan-1.2.2/app/JustScan.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       58 2023-06-30 09:29:05.000000 JustScan-1.2.2/app/JustScan.egg-info/entry_points.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      865 2023-06-30 09:29:05.000000 JustScan-1.2.2/app/JustScan.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        9 2023-06-30 09:29:05.000000 JustScan-1.2.2/app/JustScan.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-30 09:29:05.735161 JustScan-1.2.2/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1178 2023-06-30 09:29:04.000000 JustScan-1.2.2/setup.py
```

### Comparing `JustScan-1.2.1/PKG-INFO` & `JustScan-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustScan
-Version: 1.2.1
+Version: 1.2.2
 Summary: E-kyc for Industries application
 Home-page: https://gitlab.itcgroup.io/Theodore.vo
 Author: Theodore
 Author-email: theodore.v@itcgroup.io
 License: MIT
 Keywords: ITC,AI,E-kyc,Deep Learning,Computer Vision,Yolov5,Interface
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `JustScan-1.2.1/README.md` & `JustScan-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/api/just_scan_api.py` & `JustScan-1.2.2/app/JustScan/api/just_scan_api.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/config/config.py` & `JustScan-1.2.2/app/JustScan/config/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/config/config_db.py` & `JustScan-1.2.2/app/JustScan/config/config_db.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/config/logger.py` & `JustScan-1.2.2/app/JustScan/config/logger.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/config/pydantic_models.py` & `JustScan-1.2.2/app/JustScan/config/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/database/crud.py` & `JustScan-1.2.2/app/JustScan/database/crud.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/database/data_models.py` & `JustScan-1.2.2/app/JustScan/database/data_models.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/database/database.py` & `JustScan-1.2.2/app/JustScan/database/database.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/AntiSpoof/utility.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/AntiSpoof/utility.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/__init__.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/__init__.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/lib/layers.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/layers.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/lib/models.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/models.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/ArcFace/lib/utils.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/ArcFace/lib/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/CloseEyes/utils.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/CloseEyes/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/FaceQuality/dom.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/FaceQuality/dom.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/ScrFd/scrfd.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/ScrFd/scrfd.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/commons/config.py` & `JustScan-1.2.2/app/JustScan/face_id/commons/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/libraries/face_detection.py` & `JustScan-1.2.2/app/JustScan/face_id/libraries/face_detection.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/libraries/face_id.py` & `JustScan-1.2.2/app/JustScan/face_id/libraries/face_id.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/face_id/tools/modules.py` & `JustScan-1.2.2/app/JustScan/face_id/tools/modules.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/commons/SpoofingNID.py` & `JustScan-1.2.2/app/JustScan/ocr/core/commons/SpoofingNID.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/commons/config.py` & `JustScan-1.2.2/app/JustScan/ocr/core/commons/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,31 +67,27 @@
             output = trt_model_path
             gdown.download(url_, output, quiet=False)
         return trt_model_path
 
 
 def get_model(url, onnx_mode=True, front_side=False, back_side=False, crop_nid=False, classify=False,
               anti_spoof=False, passport_crop=False, passport_detect=False,
-              mrc_crop=False, mrc_detect=False, encoder=False, decoder=False, encoder_trt=False, decoder_trt=False,encoder_quantized=False, decoder_quantized=False):
+              mrc_crop=False, mrc_detect=False, encoder=False, decoder=False):
     model_mapping = {
         front_side: 'ScanIDcard_640x480',
         back_side: 'FasterScanNIDBackSide',
         crop_nid: 'lightweight_crop_cccd',
         classify: 'idcard_classify_simplified',
         anti_spoof: 'nid_liveness_check',
         passport_crop: 'crop_passport',
         passport_detect: 'detect_passport',
         mrc_crop: 'mrc_corner',
         mrc_detect: 'mrc_detect',
         encoder: 'transformer_encoder',
-        decoder: 'transformer_decoder',
-        encoder_trt: 'transformer_encoder_trt',
-        decoder_trt: 'transformer_decoder_trt',
-        encoder_quantized: 'transformers_encoder_quantized',
-        decoder_quantized: 'transformers_decoder_quantized'
+        decoder: 'transformer_decoder'
     }
 
     model_name = model_mapping.get(True)
     if onnx_mode:
         return save_dir(url, model_name, onnx_mode=onnx_mode)
     else:
         return save_dir(url, model_name, onnx_mode=False)
@@ -134,35 +130,20 @@
             passport_crop=True),
         'passport_detect': get_model(
             url='https://drive.google.com/u/3/uc?id=1bzVxtkZJElSRFp5oDeZi_ueYBGxzLD8B&export=download',
             passport_detect=True)
     },
     'vietnamese_nlp':
         {
-            # 'encoder': get_model(
-            #     url='https://drive.google.com/u/3/uc?id=159JfNNVcHDKrV_00eM_Ve2Elui5nonIc&export=download',
-            #     encoder=True),
-            # 'decoder': get_model(
-            #     url='https://drive.google.com/u/3/uc?id=1PUmuoD77dntBT1IWByO6TLNkVLcfH5Db&export=download',
-            #     decoder=True)
             'encoder': get_model(
-                url='https://drive.google.com/u/3/uc?id=1sonbYaFK2ebw-lQSEEnHdZfgk_M2yKX1&export=download',
-                encoder_quantized=True),
+                url='https://drive.google.com/u/3/uc?id=159JfNNVcHDKrV_00eM_Ve2Elui5nonIc&export=download',
+                encoder=True),
             'decoder': get_model(
-                url='https://drive.google.com/u/3/uc?id=1yu_ICbAhw3qBDyZFhgQVxbkh3FxG3D91&export=download',
-                decoder_quantized=True)
-        },
-    'tensorrt_nlp':
-        {
-            'encoder_trt': get_model(
-                url='https://drive.google.com/u/3/uc?id=1iDPkpKDlauRkEZ3TjOjzEGIOLEMcwJc4&export=download',
-                encoder_trt=False),
-            'decoder_trt': get_model(
-                url='https://drive.google.com/u/3/uc?id=1gCkrx-s7joOQvBi-kvhnpJuOJY4fxe9H&export=download',
-                decoder_trt=False)
+                url='https://drive.google.com/u/3/uc?id=1PUmuoD77dntBT1IWByO6TLNkVLcfH5Db&export=download',
+                decoder=True)
         }
 }
 
 
 class Config(object):
     def __init__(self,
                  crop_model=config['corner_detection']['corner_model'],
@@ -171,33 +152,41 @@
                  front_side_model=config['text_detection']['cccd_front_model']
                  ):
         self.crop_model = crop_model
         self.classify_model = classify_model
         self.back_side_model = back_side_model
         self.front_side_model = front_side_model
 
-    def load_all_models(self):
-        classify = idcardclassONNX(
-            model_file=self.classify_model
-        )
-        crop = ID_CARD(
-            path=self.crop_model,
-            class_name=['top_left', 'top_right', 'bottom_left', 'bottom_right'],
-            yolov5=True
-        )
-        front_side = ID_CARD(
-            path=self.front_side_model,
-            class_name=[
-                'qr', 'id', 'name', 'birth', 'gender', 'country',
-                'home', 'add', 'valid'
-            ],
-            yolov5=True)
-        back_side = ID_CARD(
-            path=self.back_side_model,
-            class_name=[
-                'qr', 'id', 'name', 'birth', 'gender', 'country',
-                'home', 'add', 'valid', 'personal_iden',
-                'create_date', 'police_sign', 'left_finger', 'right_finger', 'mrz'
-            ],
-            yolov5=True
-        )
-        return classify, crop, front_side, back_side
+    def load_all_models(self, crop_mode=False, classify_mode=False, back_side=False, front_side=False):
+        if classify_mode:
+            classify = idcardclassONNX(
+                model_file=self.classify_model
+            )
+            return classify
+        elif crop_mode:
+            crop = ID_CARD(
+                path=self.crop_model,
+                class_name=['top_left', 'top_right', 'bottom_left', 'bottom_right'],
+                yolov5=True
+            )
+            return crop
+        elif front_side:
+            front_side = ID_CARD(
+                path=self.front_side_model,
+                class_name=[
+                    'qr', 'id', 'name', 'birth', 'gender', 'country',
+                    'home', 'add', 'valid'
+                ],
+                yolov5=True)
+            return front_side
+        elif back_side:
+            back_side = ID_CARD(
+                path=self.back_side_model,
+                class_name=[
+                    'qr', 'id', 'name', 'birth', 'gender', 'country',
+                    'home', 'add', 'valid', 'personal_iden',
+                    'create_date', 'police_sign', 'left_finger', 'right_finger', 'mrz'
+                ],
+                yolov5=True
+            )
+            return back_side
+
```

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/commons/id_card_classification.py` & `JustScan-1.2.2/app/JustScan/ocr/core/commons/id_card_classification.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/commons/id_card_onnx.py` & `JustScan-1.2.2/app/JustScan/ocr/core/commons/id_card_onnx.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,44 +15,34 @@
 
     def __call__(self, image):
         return self.detect_objects(image)
 
     def initialize_model(self, path):
         options = onnxruntime.SessionOptions()
         options.graph_optimization_level = onnxruntime.GraphOptimizationLevel.ORT_ENABLE_ALL
-        options.intra_op_num_threads = 4
+        options.intra_op_num_threads = 12
         options.execution_mode = onnxruntime.ExecutionMode.ORT_SEQUENTIAL
         self.session = onnxruntime.InferenceSession(path, options=options, providers=['CoreMLExecutionProvider'])
         self.get_input_details()
         self.get_output_details()
-        self.has_postprocess = 'score' in self.output_names or self.official_nms
 
     def detect_objects(self, image):
         input_tensor = self.prepare_input(image)
         outputs = self.inference(input_tensor)
-        if self.has_postprocess:
-            self.boxes, self.scores, self.class_ids = self.parse_processed_output(outputs)
-        else:
-            self.boxes, self.scores, self.class_ids = self.process_output(outputs)
+        self.boxes, self.scores, self.class_ids = self.process_output(outputs)
         df = get_label(self.scores, self.class_ids, self.class_name)
         return self.boxes, self.scores, self.class_ids, df
 
     def prepare_input(self, image):
         self.img_height, self.img_width = image.shape[:2]
         resized_image = cv2.resize(image, (self.input_width, self.input_height))
         normalized_image = resized_image / 255.0
         return normalized_image.transpose(2, 0, 1)[np.newaxis, :, :, :].astype(np.float32)
 
     def inference(self, input_tensor):
-        # import time
-        # ti = time.time()
-        # print(self.session.run(self.output_names, {self.input_names[0]: input_tensor}))
-        # ts = time.time()
-        # tf = ts - ti
-        # print(tf)
         return self.session.run(self.output_names, {self.input_names[0]: input_tensor})
 
     def process_output(self, output):
         if self.yolov5:
             predictions = np.squeeze(output[0])
             obj_conf = predictions[:, 4]
             mask = obj_conf > self.conf_threshold
@@ -82,48 +72,19 @@
                 return [], [], []
 
             class_ids = np.argmax(predictions[:, 4:], axis=1)
             boxes = self.extract_boxes(predictions)
             indices = nms(boxes, scores, self.iou_threshold)
             return boxes[indices], scores[indices], class_ids[indices]
 
-    def parse_processed_output(self, outputs):
-        if self.official_nms:
-            scores = outputs[0][:, -1]
-            predictions = outputs[0][:, [0, 5, 1, 2, 3, 4]]
-        else:
-            scores = np.squeeze(outputs[0], axis=1)
-            predictions = outputs[1]
-
-        valid_scores = scores > self.conf_threshold
-        predictions = predictions[valid_scores, :]
-        scores = scores[valid_scores]
-
-        if len(scores) == 0:
-            return [], [], []
-
-        batch_number = predictions[:, 0]
-        class_ids = predictions[:, 1].astype(int)
-        boxes = predictions[:, 2:]
-
-        if not self.official_nms:
-            boxes = boxes[:, [1, 0, 3, 2]]
-
-        boxes = self.rescale_boxes(boxes)
-
-        return boxes, scores, class_ids
-
     def extract_boxes(self, predictions):
-        return xywh2xyxy(self.rescale_boxes(predictions[:, :4]))
-
-    def rescale_boxes(self, boxes):
-        boxes = boxes / np.array([self.input_width, self.input_height, self.input_width, self.input_height],
+        boxes = predictions[:, :4] / np.array([self.input_width, self.input_height, self.input_width, self.input_height],
                                  dtype=np.float32)
         boxes *= np.array([self.img_width, self.img_height, self.img_width, self.img_height])
-        return boxes
+        return xywh2xyxy(boxes)
 
     def get_input_details(self):
         self.input_names = [self.session.get_inputs()[i].name for i in range(len(self.session.get_inputs()))]
         self.input_shape = self.session.get_inputs()[0].shape
         self.input_height = self.input_shape[2]
         self.input_width = self.input_shape[3]
```

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/commons/merge_model.py` & `JustScan-1.2.2/app/JustScan/ocr/core/commons/merge_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-from ..modules.corner_detection.id_card_aligment import align_image
 from ..commons.config import Config
+from ..modules.corner_detection.id_card_aligment import align_image
 from ..modules.mrc.utils import mrc_crop_model, mrc_detect_model
 from ..modules.passport.passport_detection import passport_detect_model
 
-classify, crop, front_side, back_side = Config().load_all_models()
-
 
 class MergeIdCardModel(object):
     def __init__(self):
         pass
 
     @staticmethod
     def detect_corner(image, mrc=False):
         if mrc:
             detection_boxes, detection_scores, detection_classes, df = mrc_crop_model.detect_objects(image)
             return align_image(image, detection_boxes, df)
         else:
-            detection_boxes, detection_scores, detection_classes, df = crop.detect_objects(
+            detection_boxes, detection_scores, detection_classes, df = Config().load_all_models(
+                crop_mode=True).detect_objects(
                 image)
             return align_image(image, detection_boxes, df)
 
     @staticmethod
     def recognize_fe(image, mrc=False, passport=False):
         if mrc:
             detection_boxes, detection_score, detection_classes, df = mrc_detect_model.detect_objects(image)
             return df, detection_boxes
         elif passport:
             detection_boxes, detection_score, detection_classes, df = passport_detect_model.detect_objects(image)
             return df, detection_boxes
         else:
-            detection_boxes, detection_score, detection_classes, df = front_side.detect_objects(image)
+            detection_boxes, detection_score, detection_classes, df = Config().load_all_models(
+                front_side=True).detect_objects(image)
             return df, detection_boxes
 
     @staticmethod
     def recognize_be(image):
-        detection_boxes, detection_score, detection_classes, df = back_side.detect_objects(image)
+        detection_boxes, detection_score, detection_classes, df = Config().load_all_models(
+            back_side=True).detect_objects(image)
         return df, detection_boxes
 
     @staticmethod
     def classify_card(image):
-        return classify.predict(image)
+        return Config().load_all_models(classify_mode=True).predict(image)
```

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/commons/utils/utils_onnx.py` & `JustScan-1.2.2/app/JustScan/ocr/core/commons/utils/utils_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/corner_detection/utils.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/corner_detection/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/id_card_classification/classify.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/id_card_classification/classify.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/mrc/mrc_detection.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/mrc/mrc_detection.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/mrc/utils.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/mrc/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/passport.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/passport.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/utils.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/text_detection/dictionary.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/text_detection/dictionary.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/text_detection/utils.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/text_detection/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/trt_loader.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/exe_backends/trt_loader.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_trt.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_trt.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py` & `JustScan-1.2.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/tools/api_json.py` & `JustScan-1.2.2/app/JustScan/ocr/core/tools/api_json.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/tools/dictionaries.py` & `JustScan-1.2.2/app/JustScan/ocr/core/tools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan/ocr/core/tools/functional.py` & `JustScan-1.2.2/app/JustScan/ocr/core/tools/functional.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/app/JustScan.egg-info/PKG-INFO` & `JustScan-1.2.2/app/JustScan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustScan
-Version: 1.2.1
+Version: 1.2.2
 Summary: E-kyc for Industries application
 Home-page: https://gitlab.itcgroup.io/Theodore.vo
 Author: Theodore
 Author-email: theodore.v@itcgroup.io
 License: MIT
 Keywords: ITC,AI,E-kyc,Deep Learning,Computer Vision,Yolov5,Interface
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `JustScan-1.2.1/app/JustScan.egg-info/SOURCES.txt` & `JustScan-1.2.2/app/JustScan.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 app/JustScan/ocr/__init__.py
 app/JustScan/ocr/core/__init__.py
 app/JustScan/ocr/core/commons/SpoofingNID.py
 app/JustScan/ocr/core/commons/__init__.py
 app/JustScan/ocr/core/commons/config.py
 app/JustScan/ocr/core/commons/id_card_classification.py
 app/JustScan/ocr/core/commons/id_card_onnx.py
-app/JustScan/ocr/core/commons/id_card_trt.py
 app/JustScan/ocr/core/commons/merge_model.py
 app/JustScan/ocr/core/commons/utils/__init__.py
 app/JustScan/ocr/core/commons/utils/utils_onnx.py
 app/JustScan/ocr/core/modules/__init__.py
 app/JustScan/ocr/core/modules/corner_detection/__init__.py
 app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py
 app/JustScan/ocr/core/modules/corner_detection/utils.py
```

### Comparing `JustScan-1.2.1/app/JustScan.egg-info/requires.txt` & `JustScan-1.2.2/app/JustScan.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `JustScan-1.2.1/setup.py` & `JustScan-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("app/JustScan/README.md", "r") as f:
     long_description = f.read()
 with open("requirements.txt", "r") as f:
     install_requires = [line.strip() for line in f if line.strip()]
 setup(
     name="JustScan",
-    version="1.2.1",
+    version="1.2.2",
     description="E-kyc for Industries application",
     package_dir={"": "app"},
     packages=find_packages(where="./app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.itcgroup.io/Theodore.vo",
     author="Theodore",
```

