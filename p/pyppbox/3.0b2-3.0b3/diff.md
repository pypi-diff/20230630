# Comparing `tmp/pyppbox-3.0b2.tar.gz` & `tmp/pyppbox-3.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppbox-3.0b2.tar", last modified: Tue Jun 27 22:36:51 2023, max compression
+gzip compressed data, was "pyppbox-3.0b3.tar", last modified: Fri Jun 30 00:50:07 2023, max compression
```

## Comparing `pyppbox-3.0b2.tar` & `pyppbox-3.0b3.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.369015 pyppbox-3.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-27 22:36:37.000000 pyppbox-3.0b2/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-27 22:36:37.000000 pyppbox-3.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-27 22:36:37.000000 pyppbox-3.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-27 22:36:51.369015 pyppbox-3.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-27 22:36:37.000000 pyppbox-3.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-06-27 22:36:37.000000 pyppbox-3.0b2/RELEASENOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.357015 pyppbox-3.0b2/pyppbox/
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.357015 pyppbox-3.0b2/pyppbox/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.357015 pyppbox-3.0b2/pyppbox/config/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/config/cfg/cfg.7z
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/config/cfg/detectors.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/config/cfg/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/config/cfg/reiders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/config/cfg/trackers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/config/configtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    65385 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/config/myconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.357015 pyppbox-3.0b2/pyppbox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/config/unifiedstrings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.353015 pyppbox-3.0b2/pyppbox/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.361015 pyppbox-3.0b2/pyppbox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.361015 pyppbox-3.0b2/pyppbox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.361015 pyppbox-3.0b2/pyppbox/data/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/data/modules/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.361015 pyppbox-3.0b2/pyppbox/data/res/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/data/res/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/data/res/idmap.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.361015 pyppbox-3.0b2/pyppbox/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.361015 pyppbox-3.0b2/pyppbox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   833181 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/assets/TReID.png
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/assets/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/guidemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/guihub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/guitools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.361015 pyppbox-3.0b2/pyppbox/gui/tmp/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/tmp/input.tmp
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/tmp/ui.tmp
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/ui_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/ui_deepsort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/ui_facenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/ui_gt.py
--rw-r--r--   0 runner    (1001) docker     (123)    23383 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/ui_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/ui_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/ui_torchreid.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/ui_yolocls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/gui/ui_yoloult.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.361015 pyppbox-3.0b2/pyppbox/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/detectors/yolocls/
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/detectors/yolocls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/detectors/yoloult/
--rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/detectors/yoloult/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/reiders/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/reiders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/reiders/facenet/
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/reiders/facenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/reiders/facenet/origin/
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/reiders/facenet/origin/detect_face.py
--rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/reiders/facenet/origin/facenet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/reiders/torchreid/
--rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/reiders/torchreid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/reiders/torchreid/model_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/reiders/torchreid/model_dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/reiders/torchreid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/trackers/centroid/
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/centroid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/trackers/sort/
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/modules/trackers/sort/origin/
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/modules/trackers/sort/origin/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.365015 pyppbox-3.0b2/pyppbox/standalone/
--rw-r--r--   0 runner    (1001) docker     (123)    45150 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/standalone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.369015 pyppbox-3.0b2/pyppbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (123)    26550 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/utils/evatools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/utils/gttools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/utils/persontools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/utils/restools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyppbox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.357015 pyppbox-3.0b2/pyppbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-27 22:36:51.000000 pyppbox-3.0b2/pyppbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-27 22:36:51.000000 pyppbox-3.0b2/pyppbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:36:51.000000 pyppbox-3.0b2/pyppbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 22:36:51.000000 pyppbox-3.0b2/pyppbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 22:36:51.000000 pyppbox-3.0b2/pyppbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 22:36:38.000000 pyppbox-3.0b2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:36:51.369015 pyppbox-3.0b2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-27 22:36:38.000000 pyppbox-3.0b2/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-27 22:36:38.000000 pyppbox-3.0b2/requirements/pippackages_cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-27 22:36:38.000000 pyppbox-3.0b2/requirements/pippackages_cuda.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-27 22:36:38.000000 pyppbox-3.0b2/requirements/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:36:51.369015 pyppbox-3.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-27 22:36:38.000000 pyppbox-3.0b2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-27 22:36:38.000000 pyppbox-3.0b2/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.498429 pyppbox-3.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-06-30 00:49:51.000000 pyppbox-3.0b3/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-30 00:49:51.000000 pyppbox-3.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-30 00:49:51.000000 pyppbox-3.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-30 00:50:07.498429 pyppbox-3.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-30 00:49:51.000000 pyppbox-3.0b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-30 00:49:51.000000 pyppbox-3.0b3/RELEASENOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.478428 pyppbox-3.0b3/pyppbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.478428 pyppbox-3.0b3/pyppbox/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.478428 pyppbox-3.0b3/pyppbox/config/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/config/cfg/cfg.7z
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/config/cfg/detectors.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/config/cfg/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/config/cfg/reiders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/config/cfg/trackers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/config/configtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65385 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/config/myconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.482429 pyppbox-3.0b3/pyppbox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/config/unifiedstrings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.470428 pyppbox-3.0b3/pyppbox/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.482429 pyppbox-3.0b3/pyppbox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.482429 pyppbox-3.0b3/pyppbox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.482429 pyppbox-3.0b3/pyppbox/data/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/data/modules/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.482429 pyppbox-3.0b3/pyppbox/data/res/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/data/res/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/data/res/idmap.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.486429 pyppbox-3.0b3/pyppbox/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.486429 pyppbox-3.0b3/pyppbox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   833181 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/assets/TReID.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/assets/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/guidemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/guihub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/guitools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.486429 pyppbox-3.0b3/pyppbox/gui/tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/tmp/input.tmp
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/tmp/ui.tmp
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/ui_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/ui_deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/ui_facenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/ui_gt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23383 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/ui_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/ui_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/ui_torchreid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/ui_yolocls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/gui/ui_yoloult.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.486429 pyppbox-3.0b3/pyppbox/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.486429 pyppbox-3.0b3/pyppbox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.486429 pyppbox-3.0b3/pyppbox/modules/detectors/yolocls/
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/detectors/yolocls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.486429 pyppbox-3.0b3/pyppbox/modules/detectors/yoloult/
+-rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/detectors/yoloult/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.490429 pyppbox-3.0b3/pyppbox/modules/reiders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/reiders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.490429 pyppbox-3.0b3/pyppbox/modules/reiders/facenet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/reiders/facenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.490429 pyppbox-3.0b3/pyppbox/modules/reiders/facenet/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/reiders/facenet/origin/detect_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/reiders/facenet/origin/facenet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.490429 pyppbox-3.0b3/pyppbox/modules/reiders/torchreid/
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/reiders/torchreid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/reiders/torchreid/model_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/reiders/torchreid/model_dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/reiders/torchreid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.490429 pyppbox-3.0b3/pyppbox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.490429 pyppbox-3.0b3/pyppbox/modules/trackers/centroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/centroid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.490429 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.494429 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.494429 pyppbox-3.0b3/pyppbox/modules/trackers/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.494429 pyppbox-3.0b3/pyppbox/modules/trackers/sort/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/modules/trackers/sort/origin/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.494429 pyppbox-3.0b3/pyppbox/standalone/
+-rw-r--r--   0 runner    (1001) docker     (123)    45150 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/standalone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.498429 pyppbox-3.0b3/pyppbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26550 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/utils/evatools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/utils/gttools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/utils/persontools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/utils/restools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyppbox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.478428 pyppbox-3.0b3/pyppbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-30 00:50:07.000000 pyppbox-3.0b3/pyppbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-30 00:50:07.000000 pyppbox-3.0b3/pyppbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:50:07.000000 pyppbox-3.0b3/pyppbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 00:50:07.000000 pyppbox-3.0b3/pyppbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 00:50:07.000000 pyppbox-3.0b3/pyppbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-30 00:49:51.000000 pyppbox-3.0b3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:50:07.498429 pyppbox-3.0b3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-30 00:49:51.000000 pyppbox-3.0b3/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-30 00:49:51.000000 pyppbox-3.0b3/requirements/pippackages_cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-30 00:49:51.000000 pyppbox-3.0b3/requirements/pippackages_cuda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-30 00:49:51.000000 pyppbox-3.0b3/requirements/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 00:50:07.498429 pyppbox-3.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-30 00:49:51.000000 pyppbox-3.0b3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-30 00:49:51.000000 pyppbox-3.0b3/setup_extra.yaml
```

### Comparing `pyppbox-3.0b2/GETSTARTED.md` & `pyppbox-3.0b3/GETSTARTED.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 # 🚀 Getting Started
 
-Installing `pyppbox` is very easy and straightforward. You can install it from [PyPI](https://pypi.org/project/pyppbox/) directly or use the prebuilt `.whl` files on [GitHub releases](https://github.com/rathaumons/pyppbox-data/releases) or install from GitHub directly or build it from source on your own machine. However, in order to get it work, you need to install all the necessary dependcies or requirements for the modules you needs.
+Installing `pyppbox` is very easy and straightforward. You can install it from [PyPI](https://pypi.org/project/pyppbox/) directly or use the prebuilt `.whl` files on [GitHub releases](https://github.com/rathaumons/pyppbox/releases) or install from GitHub directly or build it from source on your own machine. However, in order to get it work, you need to install all the necessary dependcies or requirements for the modules you needs.
+
+🆕 `pyppbox` `v3.0b2+` supports all Windows, Linux and macOS.
 
 ## ⚙️ Requirements
 
 All requirements are not strictly limited. However, some specific modules might need some special dependencies. For example, `YOLO_Classic` (With `.weights` model) relies OpenCV DNN in order to make use of GPU power. In this case, you might need to build OpenCV from source by yourself or use our [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) instead of the official `opencv-contrib-python` which does not include GPU support.
 
 * Prerequisite: 
   - For NVIDIA GPU: [CUDA Toolkit 11.x.x](https://developer.nvidia.com/cuda-downloads) with default installation path
   - For NVIDIA GPU: [cuDNN 8.x.x](https://developer.nvidia.com/rdp/cudnn-download) with default installation path
-  - Python [[3.9-3.10]](https://www.python.org/downloads/) (3.11 is currently not supported)
+  - Python [[3.8-3.11]](https://www.python.org/downloads/)
   - Local pyppbox repo: `git clone https://github.com/rathaumons/pyppbox.git`
 
+* Before you install dependencies/requirements:
+  - For Linux/Ubuntu, recommend changing `python3` to `python`: `sudo apt install python-is-python3`
+  - If you prefer conda + Python [3.8-3.11]: `conda create --name pyppbox_env python=3.10`
+  - If you don't know whether to install only Tensorflow or PyTorch or both -> Check [Supported Modules](https://rathaumons.github.io/pyppbox/pyppbox/modules.html)
+
 * Install dependencies/requirments: 
-  - If you prefer conda + Python [3.9-3.10]: `conda create --name pyppbox_env python=3.10`
   - On Windows, run the `cmd` inside `pyppbox/requirements/`:
-    - For GPU: `install_req_p3_cuda.cmd` 
+    - For GPU: `install_req_p3_cuda.cmd` (Line 28 -> PyTorch + CUDA 11.8, change if you need to)
     - For CPU-only: `install_req_p3_cpu.cmd`
   - On Linux/macOS, under `pyppbox/requirements/`:
-    - For GPU + Linux-Only:
+    - For GPU + Linux-Only (Example for PyTorch CUDA 11.8):
       ```
-      pip uninstall -y ultralytics # Remove the official ultralytics
       python -m pip install --upgrade pip
+      pip uninstall -y ultralytics # Remove the official ultralytics
       pip install "setuptools>=67.2.0"
       pip install -r pippackages_cuda.txt
-      pip install torch==2.0.1+cu118 torchaudio==2.0.2+cu118 torchvision==0.15.2+cu118 --extra-index-url https://download.pytorch.org/whl/cu118
+      pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
       ```
     - For CPU-only:
       ```
-      pip uninstall -y ultralytics # Remove the official ultralytics
       python -m pip install --upgrade pip
+      pip uninstall -y ultralytics # Remove the official ultralytics
       pip install "setuptools>=67.2.0"
       pip install -r pippackages_cpu.txt
-      pip install torch torchvision torchaudio
+      pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
       ```
 
 * (Optional) For GPU-Only -> Verify the installed dependencies:
   - Execute the `test_gup.py`
     - On Windows -> `test_gpu.cmd`
     - On Linux/macOS -> `python test_gup.py`
   - If there is no error, then you are all good and ready to go.
-  - For `pyppbox-opencv` on Windows, if `cv2` encounters `ImportError: DLL load failed ...`, please verify the path of your CUDA & cuDNN. Our pre-built `pyppbox-opencv` uses the default path of CUDA & cuDNN (`C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v1x.x`), and if your CUDA & cuDNN were installed in a different location, simply modify the `YOUR_PYTHON\Lib\site-packages\cv2\config.py` accordingly.
+  - For OpenCV, the official `opencv-contrib-python` (No GPU support) is set in the `pippackages_cuda.txt` file. If you need GPU support, check our [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) or build one from source by yourself.
 
-* ⚠️ ***Notes for CPU-Only:***
-  - Torchreid does not work for CPU-Only -> Excluded from `pippackages_cpu.txt`
-  - YOLO Ultralytics uses GPU by default, you must set `cpu` as string for the parameter `device` in its configuration
+* ⚠️ ***Notes:***
+  - For CPU-Only, Torchreid does not work on CPU -> `pyppbox-torchreid` is excluded from `pippackages_cpu.txt`.
+  - For CPU-Only, YOLO Ultralytics uses GPU by default, you must set `cpu` as string for the parameter `device` in its configuration.
+  - For GPU on Windows, Tensorflow 2.11+ no long provides native GPU support. 
 
 
 ## 💽 Setup
 
 You need to install the main package which is `pyppbox` and the data for the modules you need `pyppbox-data-xxx`. If you want to have some fun for the demo on our [GTA_V_DATASET](https://github.com/rathaumons/PoseTReID_DATASET), you also need to install `pyppbox-data-gta5`.
 
 * Install `pyppbox`
@@ -56,16 +63,17 @@
   - Or download the latest `.whl` from [releases](https://github.com/rathaumons/pyppbox/releases)
   - Or install directly from GitHub:
     ```
     pip install git+https://github.com/rathaumons/pyppbox.git
     ```
   - Or build from source:
     ```
-    cd pyppbox
-    python -m build --wheel --skip-dependency-check
+    pip install "setuptools>=67.2.0"
+    pip install wheel build PyYAML
+    python -m build --wheel --skip-dependency-check --no-isolation
     cd dist
     pip install pyppbox-xxx.whl
     ```
 
 * Install [`pyppbox-data-xxx`](https://github.com/rathaumons/pyppbox-data/)
   - Download the latest from [releases](https://github.com/rathaumons/pyppbox-data/releases)
   - Or install the ones you need directly:
@@ -89,17 +97,25 @@
     ```
     python
     import pyppbox
     pyppbox.launchGUI()
     ```
   - Now you should see the GUI of pyppbox for easy demo.
     <details><summary><ins>Show GUI example!</ins></summary><img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/pyppbox/pyppbox_gui.jpg"></details>
+  - For Linux or Ubuntu, if the GUI does not work, you might need to install these:
+    ```
+    sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-dev
+    ```
+
+## 📢 FYI
 
+### 1️⃣ Customized OpenCV
 
-## 🪧 FYI
+OpenCV is widely used in many well-known packages, but the majority of the prebuilt WHLs on the Internet including the official one on PyPI do not include GPU support. Thus, we build our custom one which includes CUDA & cuDNN supports for the DNN modules. In order to well distinguish from the rest, we decided to build and change the package name from `opencv-contrib-python` to [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) -> [[Repo]](https://github.com/rathaumons/opencv-for-pyppbox) [[WHL]](https://github.com/rathaumons/opencv-for-pyppbox/releases)
 
-🆕 We added support for Linux and macOS from `pyppbox` `v3.0b2`, and instead of using `pyppbox-opencv`, the official `opencv-contrib-python` is used by default. You still can manually remove it and install our `pyppbox-opencv` if you need to.
+### 2️⃣ Customized Torchreid
 
-OpenCV is widely used in many well-known packages, but the majority of the prebuilt WHLs on the Internet including the official one on PyPi do not include GPU support. Thus, we build our custom one which includes CUDA & cuDNN supports for the DNN modules. In order to well distinguish from the rest, we decided to build and change the package name from `opencv-contrib-python` to [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox). [[repo]](https://github.com/rathaumons/opencv-for-pyppbox) [[WHL]](https://github.com/rathaumons/pyppbox-custpkg/tree/main/pyppbox_opencv)
+Similar to [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox), our custom `torchreid` is changed to [`pyppbox-torchreid`](https://github.com/rathaumons/torchreid-for-pyppbox). More than the normal package rename, the module name is also changed from `torchreid` to `pyppbox_torchreid` which means the `import` in the code must be also changed. Find out more why `pyppbox` needs the customized `pyppbox-torchreid` -> [[Repo]](https://github.com/rathaumons/torchreid-for-pyppbox) [[PyPI]](https://pypi.org/project/pyppbox-torchreid/)
 
-Similar to [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox), our custom `torchreid` is changed to [`pyppbox-torchreid`](https://github.com/rathaumons/torchreid-for-pyppbox). More than the normal package rename, the module name is also changed from `torchreid` to `pyppbox_torchreid` which means the `import` in the code must be also changed. [[WHL]](https://github.com/rathaumons/torchreid-for-pyppbox)
+### 3️⃣ Customized Ultralytics
 
+Also, similar to `pyppbox_torchreid`, our custom `ultralytics` is changed to [`pyppbox-ultralytics`](https://github.com/rathaumons/ultralytics-for-pyppbox), but this time, the module name is still the same `ultralytics` and it is the main reason why the official `ultralytics` must be removed. Find out more why `pyppbox` needs the customized `pyppbox-ultralytics` -> [[Repo]](https://github.com/rathaumons/torchreid-for-pyppbox) [[PyPI]](https://pypi.org/project/pyppbox-torchreid/)
```

### Comparing `pyppbox-3.0b2/LICENSE` & `pyppbox-3.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/PKG-INFO` & `pyppbox-3.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.0b2
+Version: 3.0b3
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
@@ -32,15 +32,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🐍📦 [**pyppbox**](https://github.com/rathaumons/pyppbox)
 
 <div align="center">
 
-[![Documentation](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml) [![Test Core Windows](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml) [![Test Core Linux](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml) [![Test Build](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml) [![Build PyPI](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml)
+[![Build PyPI](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml) [![Documentation](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml) [![Test Core Windows](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml) [![Test Core Linux](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml) [![Test Build](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml)
 
 <img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/pyppbox/pyppbox_gui_wide.png"><br />
 
 **[📗 Documentation](https://rathaumons.github.io/pyppbox/) > [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) > [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html)**
 
 </div>
```

### Comparing `pyppbox-3.0b2/README.md` & `pyppbox-3.0b3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 🐍📦 [**pyppbox**](https://github.com/rathaumons/pyppbox)
 
 <div align="center">
 
-[![Documentation](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml) [![Test Core Windows](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml) [![Test Core Linux](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml) [![Test Build](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml) [![Build PyPI](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml)
+[![Build PyPI](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml) [![Documentation](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml) [![Test Core Windows](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml) [![Test Core Linux](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml) [![Test Build](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml)
 
 <img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/pyppbox/pyppbox_gui_wide.png"><br />
 
 **[📗 Documentation](https://rathaumons.github.io/pyppbox/) > [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) > [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html)**
 
 </div>
```

### Comparing `pyppbox-3.0b2/RELEASENOTES.md` & `pyppbox-3.0b3/RELEASENOTES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 # Release Notes 
 
 
 ## **pyppbox V3 - Make Simpler and Faster**
 
+* `pyppbox` [v3.0b3](https://github.com/rathaumons/pyppbox/tree/v3.0b3)
+
+  - Fix GUI for GT
+  - Improve supports for Python [3.8-3.11]
+  - Update and improve dependencies/requirements
+  - Update and improve `GETSTARTED.md`
+  - Update test workflows for Python [3.8-3.11]
+  - **Known issue/limitation**: 
+    - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
+
 * `pyppbox` [v3.0b2](https://github.com/rathaumons/pyppbox/tree/v3.0b2)
 
   - Add Linux and macOS supports
   - Add workflow for Windows/Linux core stability tests
   - Add workflow for PyPI build -> `pyppbox` is now available on PyPI
   - Improve independency of the modules
   - Improve supports for CPU-Only
```

### Comparing `pyppbox-3.0b2/pyppbox/__init__.py` & `pyppbox-3.0b3/pyppbox/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,17 @@
 
 A toolbox for people detecting, tracking, and re-identifying
 
     * * * * * * * * * * * * * * * * * * * * * * * *
     *  Copyright (C) 2022 UMONS-Numediart GPLV3+  *
     * * * * * * * * * * * * * * * * * * * * * * * *
 
-# Launch GUI:
->>> pyppbox.launchGUI()
-
-# Read online documentation:
->>> pyppbox.docs()
-
-# Go to our GitHub:
->>> pyppbox.github()
+>>> pyppbox.launchGUI() # Launch GUI
+>>> pyppbox.docs() # Read online documentation
+>>> pyppbox.github() # Go to our GitHub
 
 """
 
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 #                                                                           #
 #   pyppbox: Toolbox for people detecting, tracking, and re-identifying.    #
 #   Copyright (C) 2022 UMONS-Numediart                                      #
@@ -48,13 +43,13 @@
     useInternalConfigDir, 
     useThisConfigDir,
     resetInternalConfig,
     generateConfig
 )
 
 
-__version__ = '3.0b2'
+__version__ = '3.0b3'
 __author__ = 'Ratha SIV'
 __description__ = 'Toolbox for people detecting, tracking, and re-identifying.'
 __homepage__ = 'https://rathaumons.github.io/pyppbox'
 __url__ = 'https://github.com/rathaumons/pyppbox.git'
```

### Comparing `pyppbox-3.0b2/pyppbox/config/__init__.py` & `pyppbox-3.0b3/pyppbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/config/cfg/cfg.7z` & `pyppbox-3.0b3/pyppbox/config/cfg/cfg.7z`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/config/cfg/detectors.yaml` & `pyppbox-3.0b3/pyppbox/config/cfg/detectors.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/config/cfg/reiders.yaml` & `pyppbox-3.0b3/pyppbox/config/cfg/reiders.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/config/cfg/trackers.yaml` & `pyppbox-3.0b3/pyppbox/config/cfg/trackers.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/config/configtools.py` & `pyppbox-3.0b3/pyppbox/config/configtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/config/myconfig.py` & `pyppbox-3.0b3/pyppbox/config/myconfig.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/config/unifiedstrings.py` & `pyppbox-3.0b3/pyppbox/config/unifiedstrings.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/__init__.py` & `pyppbox-3.0b3/pyppbox/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/assets/TReID.png` & `pyppbox-3.0b3/pyppbox/gui/assets/TReID.png`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/assets/icon.ico` & `pyppbox-3.0b3/pyppbox/gui/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/assets/settings.ico` & `pyppbox-3.0b3/pyppbox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/guidemo.py` & `pyppbox-3.0b3/pyppbox/gui/guidemo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/guihub.py` & `pyppbox-3.0b3/pyppbox/gui/guihub.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/guitools.py` & `pyppbox-3.0b3/pyppbox/gui/guitools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/ui_centroid.py` & `pyppbox-3.0b3/pyppbox/gui/ui_centroid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/ui_deepsort.py` & `pyppbox-3.0b3/pyppbox/gui/ui_deepsort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/ui_facenet.py` & `pyppbox-3.0b3/pyppbox/gui/ui_facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/ui_gt.py` & `pyppbox-3.0b3/pyppbox/gui/ui_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,39 +69,40 @@
         self.gt_map_lineEdit.setGeometry(QtCore.QRect(110, 40, 241, 21))
         self.gt_map_lineEdit.setObjectName("gt_map_lineEdit")
         self.gt_map_label = QtWidgets.QLabel(gi_ui)
         self.gt_map_label.setGeometry(QtCore.QRect(10, 40, 91, 16))
         self.gt_map_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|
                                        QtCore.Qt.AlignmentFlag.AlignTrailing|
                                        QtCore.Qt.AlignmentFlag.AlignVCenter)
-        self.gt_map_label.setObjectName("gt_file_label")
+        self.gt_map_label.setObjectName("gt_map_label")
         font = QtGui.QFont()
         font.setPointSize(12)
         self.save_pushButton.setFont(font)
         self.save_pushButton.setDefault(True)
         self.retranslateUi(gi_ui)
         # custom
         self.loadGT()  
         self.gt_file_browse_pushButton.clicked.connect(self.browseGTFile)
-        self.gt_map_lineEdit.clicked.connect(self.browseGTMap)
+        self.gt_map_browse_pushButton.clicked.connect(self.browseGTMap)
         self.save_pushButton.clicked.connect(lambda: self.updateCFG(gi_ui))
         QtCore.QMetaObject.connectSlotsByName(gi_ui)
 
     def retranslateUi(self, gi_ui):
         _translate = QtCore.QCoreApplication.translate
         gi_ui.setWindowTitle(_translate("gi_ui", "GT"))
         self.gt_file_label.setText(_translate("gi_ui", "gt_file"))
         self.gt_file_browse_pushButton.setText(_translate("gi_ui", "..."))
-        self.gt_file_label.setText(_translate("gi_ui", "gt_map_file"))
+        self.gt_map_label.setText(_translate("gi_ui", "gt_map_file"))
         self.gt_map_browse_pushButton.setText(_translate("gi_ui", "..."))
         self.save_pushButton.setText(_translate("gi_ui", "Save"))
 
     def loadGT(self):
         self.mycfg.setAllDCFG()
         self.gt_file_lineEdit.setText(getAbsPathFDS(self.mycfg.dcfg_gt.gt_file))
+        self.gt_map_lineEdit.setText(getAbsPathFDS(self.mycfg.dcfg_gt.gt_map_file))
 
     def browseGTFile(self):
         default_path = getAncestorDir(self.mycfg.dcfg_gt.gt_file)
         file_filter = "Text (*.txt)"
         source_file, _ = QtWidgets.QFileDialog.getOpenFileName(None, "Input GT file", 
                                                                default_path, file_filter)
         if source_file:
@@ -114,12 +115,12 @@
                                                                default_path, file_filter)
         if source_file:
             self.gt_map_lineEdit.setText(source_file)
 
     def updateCFG(self, gi_ui):
         gt_doc = {"dt_name": "GT",
                   "gt_file": normalizePathFDS(root_dir, self.gt_file_lineEdit.text()),
-                  "gt_map_file": normalizePathFDS(root_dir, self.mycfg.dcfg_gt.gt_map_file)}
+                  "gt_map_file": normalizePathFDS(root_dir, self.gt_map_lineEdit.text())}
         yolo_doc = self.mycfg.dcfg_yolocs.getDocument()
         yolo_utlt_doc = self.mycfg.dcfg_yolout.getDocument()
         self.mycfg.dumpAllDCFG([yolo_doc, yolo_utlt_doc, gt_doc])
         gi_ui.close()
```

### Comparing `pyppbox-3.0b2/pyppbox/gui/ui_launcher.py` & `pyppbox-3.0b3/pyppbox/gui/ui_launcher.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/ui_sort.py` & `pyppbox-3.0b3/pyppbox/gui/ui_sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/ui_torchreid.py` & `pyppbox-3.0b3/pyppbox/gui/ui_torchreid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/ui_yolocls.py` & `pyppbox-3.0b3/pyppbox/gui/ui_yolocls.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/gui/ui_yoloult.py` & `pyppbox-3.0b3/pyppbox/gui/ui_yoloult.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/__init__.py` & `pyppbox-3.0b3/pyppbox/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/detectors/__init__.py` & `pyppbox-3.0b3/pyppbox/modules/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/detectors/yolocls/__init__.py` & `pyppbox-3.0b3/pyppbox/modules/detectors/yolocls/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/detectors/yoloult/__init__.py` & `pyppbox-3.0b3/pyppbox/modules/detectors/yoloult/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/reiders/__init__.py` & `pyppbox-3.0b3/pyppbox/modules/reiders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/reiders/facenet/__init__.py` & `pyppbox-3.0b3/pyppbox/modules/reiders/facenet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py` & `pyppbox-3.0b3/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/reiders/facenet/origin/detect_face.py` & `pyppbox-3.0b3/pyppbox/modules/reiders/facenet/origin/detect_face.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/reiders/facenet/origin/facenet.py` & `pyppbox-3.0b3/pyppbox/modules/reiders/facenet/origin/facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/reiders/torchreid/__init__.py` & `pyppbox-3.0b3/pyppbox/modules/reiders/torchreid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/reiders/torchreid/model_dict.py` & `pyppbox-3.0b3/pyppbox/modules/reiders/torchreid/model_dict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/reiders/torchreid/model_dict.yaml` & `pyppbox-3.0b3/pyppbox/modules/reiders/torchreid/model_dict.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/reiders/torchreid/utils.py` & `pyppbox-3.0b3/pyppbox/modules/reiders/torchreid/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/__init__.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/centroid/__init__.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/centroid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/__init__.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/detection.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/detection.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/generate_detections.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/generate_detections.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/iou_matching.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/iou_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/nn_matching.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/nn_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/preprocessing.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/track.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/track.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/deepsort/origin/tracker.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/deepsort/origin/tracker.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/sort/__init__.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/modules/trackers/sort/origin/sort.py` & `pyppbox-3.0b3/pyppbox/modules/trackers/sort/origin/sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/standalone/__init__.py` & `pyppbox-3.0b3/pyppbox/standalone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/utils/__init__.py` & `pyppbox-3.0b3/pyppbox/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/utils/commontools.py` & `pyppbox-3.0b3/pyppbox/utils/commontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/utils/evatools.py` & `pyppbox-3.0b3/pyppbox/utils/evatools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/utils/gttools.py` & `pyppbox-3.0b3/pyppbox/utils/gttools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/utils/logtools.py` & `pyppbox-3.0b3/pyppbox/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/utils/persontools.py` & `pyppbox-3.0b3/pyppbox/utils/persontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/utils/restools.py` & `pyppbox-3.0b3/pyppbox/utils/restools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox/utils/visualizetools.py` & `pyppbox-3.0b3/pyppbox/utils/visualizetools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/pyppbox.egg-info/PKG-INFO` & `pyppbox-3.0b3/pyppbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.0b2
+Version: 3.0b3
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
@@ -32,15 +32,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🐍📦 [**pyppbox**](https://github.com/rathaumons/pyppbox)
 
 <div align="center">
 
-[![Documentation](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml) [![Test Core Windows](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml) [![Test Core Linux](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml) [![Test Build](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml) [![Build PyPI](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml)
+[![Build PyPI](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml) [![Documentation](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml) [![Test Core Windows](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml) [![Test Core Linux](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml) [![Test Build](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml)
 
 <img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/pyppbox/pyppbox_gui_wide.png"><br />
 
 **[📗 Documentation](https://rathaumons.github.io/pyppbox/) > [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) > [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html)**
 
 </div>
```

### Comparing `pyppbox-3.0b2/pyppbox.egg-info/SOURCES.txt` & `pyppbox-3.0b3/pyppbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/requirements/test_gpu.py` & `pyppbox-3.0b3/requirements/test_gpu.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/setup.py` & `pyppbox-3.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b2/setup_extra.yaml` & `pyppbox-3.0b3/setup_extra.yaml`

 * *Files identical despite different names*

