# Comparing `tmp/dcnum-0.11.1.tar.gz` & `tmp/dcnum-0.11.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.11.1.tar", last modified: Tue Jun 27 08:33:45 2023, max compression
+gzip compressed data, was "dcnum-0.11.2.tar", last modified: Thu Jun 29 22:42:43 2023, max compression
```

## Comparing `dcnum-0.11.1.tar` & `dcnum-0.11.2.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.502594 dcnum-0.11.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.490594 dcnum-0.11.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-27 08:33:36.000000 dcnum-0.11.1/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-27 08:33:36.000000 dcnum-0.11.1/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-27 08:33:36.000000 dcnum-0.11.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-27 08:33:36.000000 dcnum-0.11.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-27 08:33:36.000000 dcnum-0.11.1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-27 08:33:36.000000 dcnum-0.11.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-27 08:33:45.502594 dcnum-0.11.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-27 08:33:36.000000 dcnum-0.11.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-27 08:33:45.000000 dcnum-0.11.1/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/dcnum/feat/feat_moments/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/segm/segmenter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-27 08:33:45.000000 dcnum-0.11.1/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-27 08:33:45.000000 dcnum-0.11.1/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:33:45.000000 dcnum-0.11.1/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 08:33:45.000000 dcnum-0.11.1/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 08:33:45.000000 dcnum-0.11.1/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-27 08:33:36.000000 dcnum-0.11.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-27 08:33:36.000000 dcnum-0.11.1/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-27 08:33:36.000000 dcnum-0.11.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-27 08:33:36.000000 dcnum-0.11.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-27 08:33:36.000000 dcnum-0.11.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 08:33:45.502594 dcnum-0.11.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.502594 dcnum-0.11.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.502594 dcnum-0.11.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_ppid.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.257078 dcnum-0.11.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-29 22:42:34.000000 dcnum-0.11.2/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-29 22:42:34.000000 dcnum-0.11.2/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-29 22:42:34.000000 dcnum-0.11.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-29 22:42:34.000000 dcnum-0.11.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-29 22:42:34.000000 dcnum-0.11.2/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-29 22:42:34.000000 dcnum-0.11.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-29 22:42:43.257078 dcnum-0.11.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-29 22:42:34.000000 dcnum-0.11.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 22:42:43.000000 dcnum-0.11.2/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/dcnum/feat/feat_moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/segm/segmenter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-29 22:42:43.000000 dcnum-0.11.2/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-29 22:42:43.000000 dcnum-0.11.2/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:42:43.000000 dcnum-0.11.2/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-29 22:42:43.000000 dcnum-0.11.2/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 22:42:43.000000 dcnum-0.11.2/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-29 22:42:34.000000 dcnum-0.11.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-29 22:42:34.000000 dcnum-0.11.2/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-29 22:42:34.000000 dcnum-0.11.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-29 22:42:34.000000 dcnum-0.11.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-29 22:42:34.000000 dcnum-0.11.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:42:43.257078 dcnum-0.11.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.257078 dcnum-0.11.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.257078 dcnum-0.11.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_write_writer.py
```

### Comparing `dcnum-0.11.1/.github/workflows/check.yml` & `dcnum-0.11.2/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/.github/workflows/deploy_pypi.yml` & `dcnum-0.11.2/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/.gitignore` & `dcnum-0.11.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/CHANGELOG` & `dcnum-0.11.2/CHANGELOG`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+0.11.2
+ - meta: increment pipeline ID (texture feature computation)
+ - fix: HDF5Data was not pickable
+ - fix: HDF5Data did not properly handle tables
+ - enh: add context manager for CPUSegmenter
+ - enh: record and log execution time of segmentation and feature extraction
+ - enh: properly handle border case for computing contour-moments
+ - enh: properly handle empty images/masks in haralick texture features
+ - tests: do not use numba's JIT during testing (coverage)
 0.11.1
  - fix: fix GPUSegmenter labeling
 0.11.0
  - feat: introduce GPUSegmenter base class
  - fix: handle bytes-values in HDF5 attributes
  - ref: correctly introduce `requires_background_correction` for segmenters
  - setup: don't requrie cibuildwheel
```

### Comparing `dcnum-0.11.1/LICENSE` & `dcnum-0.11.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/PKG-INFO` & `dcnum-0.11.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.11.1
+Version: 0.11.2
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.11.1/README.rst` & `dcnum-0.11.2/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.11.2/dcnum/feat/event_extractor_manager_thread.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,16 @@
         self.raw_queue = self.fe_kwargs["raw_queue"]
         #: List of chunk labels corresponding to `slot_states`
         self.labels_list = labels_list
         #: Shared labeling array
         self.label_array = np.ctypeslib.as_array(
             self.fe_kwargs["label_array"]).reshape(
             self.data.image.chunk_shape)
-
+        #: Time counter for feature extraction
+        self.t_count = 0
         #: Whether debugging is enabled
         self.debug = debug
 
     def run(self):
         # Initialize all workers
         if self.debug:
             worker_cls = EventExtractorThread
@@ -96,14 +97,16 @@
                     unavailable_slots += 1
                     cur_slot = (cur_slot + 1) % num_slots
                 if unavailable_slots >= num_slots:
                     # There is nothing to do, try to avoid 100% CPU
                     unavailable_slots = 0
                     time.sleep(.1)
 
+            t1 = time.monotonic()
+
             # We have a chunk, process it!
             chunk = self.slot_chunks[cur_slot]
             # Populate the labeling array for the workers
             new_labels = self.labels_list[cur_slot]
             if len(new_labels) == self.label_array.shape[0]:
                 self.label_array[:] = new_labels
             elif len(new_labels) < self.label_array.shape[0]:
@@ -119,16 +122,19 @@
             while self.raw_queue.qsize():
                 time.sleep(.1)
 
             # We are done here. The segmenter may continue its deed.
             self.slot_states[cur_slot] = "w"
 
             self.logger.debug(f"Extracted one chunk: {chunk}")
+            self.t_count += time.monotonic() - t1
 
             chunks_processed += 1
+
             if chunks_processed == self.data.image.num_chunks:
                 break
 
         self.logger.debug("Requesting extraction workers to join.")
         self.fe_kwargs["finalize_extraction"].value = True
         [w.join() for w in workers]
         self.logger.debug("Finished extraction.")
+        self.logger.info(f"Extraction time: {self.t_count:.1f}s")
```

### Comparing `dcnum-0.11.1/dcnum/feat/feat_background/base.py` & `dcnum-0.11.2/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.11.2/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.11.2/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.11.2/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum/feat/feat_moments/mt_legacy.py` & `dcnum-0.11.2/dcnum/feat/feat_moments/mt_legacy.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,30 +6,33 @@
 
 
 def moments_based_features(mask, pixel_size):
     assert pixel_size is not None and pixel_size != 0
 
     size = mask.shape[0]
 
-    deform = np.zeros(size, dtype=float)
-    size_x = np.zeros(size, dtype=float)
-    size_y = np.zeros(size, dtype=float)
-    pos_x = np.zeros(size, dtype=float)
-    pos_y = np.zeros(size, dtype=float)
-    area_msd = np.zeros(size, dtype=float)
-    area_ratio = np.zeros(size, dtype=float)
-    area_um = np.zeros(size, dtype=float)
-    aspect = np.zeros(size, dtype=float)
-    tilt = np.zeros(size, dtype=float)
-    inert_ratio_cvx = np.zeros(size, dtype=float)
-    inert_ratio_raw = np.zeros(size, dtype=float)
-    inert_ratio_prnc = np.zeros(size, dtype=float)
+    empty = np.full(size, np.nan, dtype=np.float64)
+    deform = np.copy(empty)
+    size_x = np.copy(empty)
+    size_y = np.copy(empty)
+    pos_x = np.copy(empty)
+    pos_y = np.copy(empty)
+    area_msd = np.copy(empty)
+    area_ratio = np.copy(empty)
+    area_um = np.copy(empty)
+    aspect = np.copy(empty)
+    tilt = np.copy(empty)
+    inert_ratio_cvx = np.copy(empty)
+    inert_ratio_raw = np.copy(empty)
+    inert_ratio_prnc = np.copy(empty)
 
     for ii in range(size):
         cont_raw = contour_single_opencv(mask[ii])
+        if len(cont_raw.shape) < 2:
+            continue
         mu_raw = cv2.moments(cont_raw)
 
         # convex hull
         cont_cvx = np.squeeze(cv2.convexHull(cont_raw))
         mu_cvx = cv2.moments(cont_cvx)
 
         if mu_cvx["m00"] == 0 or mu_raw["m00"] == 0:
```

### Comparing `dcnum-0.11.1/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.11.2/dcnum/feat/feat_texture/tex_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from mahotas.features import haralick as mh_haralick
 import numpy as np
 
 from .common import haralick_names
 
 
-def haralick_texture_features(image, mask, image_bg=None, image_corr=None):
+def haralick_texture_features(
+        mask, image=None, image_bg=None, image_corr=None):
     # make sure we have a boolean array
     mask = np.array(mask, dtype=bool)
     size = mask.shape[0]
 
     # compute features if necessary
-    if image_bg is not None or image_corr is not None:
+    if image_bg is not None and image is not None and image_corr is None:
         # Background-corrected brightness values
-        if image_corr is None:
-            image_corr = np.array(image, dtype=np.int16) - image_bg
+        image_corr = np.array(image, dtype=np.int16) - image_bg
 
     tex_dict = {}
     empty = np.full(size, np.nan, dtype=np.float64)
     for key in haralick_names:
         tex_dict[key] = np.copy(empty)
 
     for ii in range(size):
@@ -25,14 +25,17 @@
         # https://gitlab.gwdg.de/blood_data_analysis/dcevent/-/issues/20
         # Preprocessing:
         # - create a copy of the array (don't edit `image_corr`)
         # - add grayscale values (negative values not supported)
         #   -> maximum value should be as small as possible
         # - set pixels outside contour to zero (ignored areas, see mahotas)
         maski = mask[ii]
+        if not np.any(maski):
+            # The mask is empty (nan values)
+            continue
         if image_corr.shape[0] == 1:
             # We have several masks for one image.
             imcoi = image_corr[0]
         else:
             imcoi = image_corr[ii]
         minval = imcoi[maski].min()
         imi = np.array((imcoi - minval + 1) * maski, dtype=np.uint8)
```

### Comparing `dcnum-0.11.1/dcnum/feat/gate.py` & `dcnum-0.11.2/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum/feat/queue_event_extractor.py` & `dcnum-0.11.2/dcnum/feat/queue_event_extractor.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum/meta/ppid.py` & `dcnum-0.11.2/dcnum/meta/ppid.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import hashlib
 import inspect
 import pathlib
 
 
 #: Increment this string if there are breaking changes that make
 #: previous pipelines unreproducible.
-DCNUM_PPID_GENERATION = "2"
+DCNUM_PPID_GENERATION = "3"
 
 
 def compute_pipeline_hash(bg_id, seg_id, feat_id, gate_id,
                           gen_id=DCNUM_PPID_GENERATION):
     hasher = hashlib.md5()
     hasher.update("|".join([gen_id, bg_id, seg_id, feat_id, gate_id]).encode())
     pph = hasher.hexdigest()
```

### Comparing `dcnum-0.11.1/dcnum/read/cache.py` & `dcnum-0.11.2/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum/read/hdf5_data.py` & `dcnum-0.11.2/dcnum/read/hdf5_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,14 @@
                  image_cache_size: int = 5,
                  ):
         # Init is in __setstate__ so we can pickle this class
         # and use it for multiprocessing.
         if isinstance(path, h5py.File):
             self.h5 = path
             path = path.filename
-        else:
-            self.h5 = None  # is set in __setstate__
-        self._cache_scalar = {}
         self.__setstate__({"path": path,
                            "pixel_size": pixel_size,
                            "md5_5m": md5_5m,
                            "meta": meta,
                            "logs": logs,
                            "tables": tables,
                            "image_cache_size": image_cache_size,
@@ -65,15 +62,33 @@
             self._cache_scalar[feat] = self.h5["events"][feat][:]
             return self._cache_scalar[feat]
         else:
             # Not cached (possibly slow)
             warnings.warn(f"Feature {feat} not cached (possibly slow)")
             return self.h5["events"][feat]
 
+    def __getstate__(self):
+        return {"path": self.path,
+                "pixel_size": self.pixel_size,
+                "md5_5m": self.md5_5m,
+                "meta": self.meta,
+                "logs": self.logs,
+                "tables": self.tables,
+                "image_cache_size": self.image.cache_size
+                }
+
     def __setstate__(self, state):
+        # Make sure these properties exist (we rely on __init__, because
+        # we want this class to be pickable and __init__ is not called by
+        # `pickle.load`.
+        if not hasattr(self, "_cache_scalar"):
+            self._cache_scalar = {}
+        if not hasattr(self, "h5"):
+            self.h5 = None
+
         self.path = state["path"]
 
         self.md5_5m = state["md5_5m"]
         if self.md5_5m is None:
             if isinstance(self.path, pathlib.Path):
                 # 5MB md5sum of input file
                 self.md5_5m = md5sum(self.path, count=80)
@@ -96,15 +111,18 @@
                         self.meta[key] = self.meta[key].decode("utf-8")
                 for key in h5.get("logs", []):
                     alog = list(h5["logs"][key])
                     if isinstance(alog[0], bytes):
                         alog = [ll.decode("utf") for ll in alog]
                     self.logs[key] = alog
                 for tab in h5.get("tables", []):
-                    self.tables[tab] = h5["tables"][key][:]
+                    tabdict = {}
+                    for tkey in h5["tables"][tab].dtype.fields.keys():
+                        tabdict[tkey] = h5["tables"][tab][tkey]
+                    self.tables[tab] = tabdict
 
         if state["pixel_size"] is not None:
             self.pixel_size = state["pixel_size"]
         else:
             # Set known pixel size if possible
             did = self.meta.get("setup:identifier", "EMPTY")
             if (did.startswith("RC-")
@@ -133,23 +151,14 @@
                 cache_size=state["image_cache_size"],
                 boolean=True)
         else:
             self.mask = None
 
         self.image_corr = ImageCorrCache(self.image, self.image_bg)
 
-    def __getstate__(self):
-        return {"path": self.path,
-                "pixel_size": self.pixel_size,
-                "md5_5m": self.md5_5m,
-                "meta": self.meta,
-                "logs": self.logs,
-                "tables": self.tables,
-                }
-
     @functools.cache
     def __len__(self):
         return self.h5.attrs["experiment:event count"]
 
     @property
     def meta_nest(self):
         """Return `self.meta` as nested dicitonary
```

### Comparing `dcnum-0.11.1/dcnum/segm/segm_thresh.py` & `dcnum-0.11.2/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum/segm/segmenter.py` & `dcnum-0.11.2/dcnum/segm/segmenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
             labels_eroded = cv2.erode(labels_dilated, element)
             labels, _ = ndi.label(
                 input=labels_eroded > 0,
                 structure=ndi.generate_binary_structure(2, 2))
 
         if fill_holes:
             # Floodfill only works with uint8 (too small) or int32
-            if not labels.dtype == np.int32:
+            if labels.dtype != np.int32:
                 labels = np.array(labels, dtype=np.int32)
             #
             # from scipy import ndimage
             # mask_old = ndimage.binary_fill_holes(mask)
             #
             # Floodfill algorithm fills the background image and
             # the resulting inversion is the image with holes filled.
```

### Comparing `dcnum-0.11.1/dcnum/segm/segmenter_cpu.py` & `dcnum-0.11.2/dcnum/segm/segmenter_cpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,20 @@
         # >0: this number workers finished a batch
         self.mp_batch_index = mp.Value("i", -1)
         # The iteration of the process (increment to wake workers)
         self.mp_batch_worker = mp.Value("i", 0)
         # Tells the workers to stop
         self.mp_shutdown = mp.Value("i", 0)
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.join_workers()
+
     def __getstate__(self):
         # Copy the object's state from self.__dict__ which contains
         # all our instance attributes. Always use the dict.copy()
         # method to avoid modifying the original state.
         # This is important when using "spawn" to create new processes,
         # because then the entire object gets pickled and some things
         # cannot be pickled!
@@ -43,15 +49,15 @@
         del state["logger"]
         del state["_mp_image_np"]
         del state["_mp_labels_np"]
         del state["_mp_workers"]
         return state
 
     def __setstate__(self, state):
-        # Restore instance attributes (i.e., filename and lineno).
+        # Restore instance attributes
         self.__dict__.update(state)
 
     @staticmethod
     def _create_shared_array(image_shape, batch_size, dtype):
         """Return raw and numpy-view on shared array
 
         Parameters
```

### Comparing `dcnum-0.11.1/dcnum/segm/segmenter_gpu.py` & `dcnum-0.11.2/dcnum/segm/segmenter_gpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.11.2/dcnum/segm/segmenter_manager_thread.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         self.image_data = image_data
         #: Slot states
         self.slot_states = slot_states
         #: Current slot chunk index for the slot states
         self.slot_chunks = slot_chunks
         #: List containing the segmented labels of each slot
         self.labels_list = [None] * len(self.slot_states)
+        #: Time counter for segmentation
+        self.t_count = 0
         #: Whether running in debugging mode
         self.debug = debug
 
     def run(self):
         # We iterate over all the chunks of the image data.
         for chunk in self.image_data.iter_chunks():
             num_slots = len(self.slot_states)
@@ -92,14 +94,16 @@
                     empty_slots += 1
                     cur_slot = (cur_slot + 1) % num_slots
                 if empty_slots >= num_slots:
                     # There is nothing to do, try to avoid 100% CPU
                     empty_slots = 0
                     time.sleep(.01)
 
+            t1 = time.monotonic()
+
             # We have a free slot to compute the segmentation
             labels = self.segmenter.segment_chunk(
                 image_data=self.image_data,
                 chunk=chunk)
 
             # TODO: make this more memory efficient (pre-shared mp.Arrays?)
             # Store labels in a list accessible by the main thread
@@ -107,11 +111,15 @@
             # Remember the chunk index for this slot
             self.slot_chunks[cur_slot] = chunk
             # This must be done last: Let the extractor know that this
             # slot is ready for processing.
             self.slot_states[cur_slot] = "e"
             self.logger.debug(f"Segmented one chunk: {chunk}")
 
+            self.t_count += time.monotonic() - t1
+
         # Cleanup
         if isinstance(self.segmenter, CPUSegmenter):
             # Join the segmentation workers.
             self.segmenter.join_workers()
+
+        self.logger.info(f"Segmentation time: {self.t_count:.1f}s")
```

### Comparing `dcnum-0.11.1/dcnum/write/deque_writer_thread.py` & `dcnum-0.11.2/dcnum/write/deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum/write/queue_collector_thread.py` & `dcnum-0.11.2/dcnum/write/queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum/write/writer.py` & `dcnum-0.11.2/dcnum/write/writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/dcnum.egg-info/PKG-INFO` & `dcnum-0.11.2/dcnum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.11.1
+Version: 0.11.2
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.11.1/dcnum.egg-info/SOURCES.txt` & `dcnum-0.11.2/dcnum.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,11 +59,12 @@
 tests/test_feat_moments_based.py
 tests/test_init.py
 tests/test_ppid.py
 tests/test_ppid_segm.py
 tests/test_read_concat_hdf5.py
 tests/test_read_hdf5.py
 tests/test_segm_thresh.py
+tests/test_segmenter.py
 tests/test_write_deque_writer_thread.py
 tests/test_write_writer.py
 tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
 tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
```

### Comparing `dcnum-0.11.1/docs/conf.py` & `dcnum-0.11.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/docs/extensions/github_changelog.py` & `dcnum-0.11.2/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/pyproject.toml` & `dcnum-0.11.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.11.2/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.11.2/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/tests/helper_methods.py` & `dcnum-0.11.2/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.11.2/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/tests/test_feat_brightness.py` & `dcnum-0.11.2/tests/test_feat_brightness.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,7 +27,30 @@
                            atol=0, rtol=1e-10)
         for feat in feat_brightness.brightness_names:
             assert np.allclose(h5["events"][feat][:],
                                data[feat]), f"Feature {feat} mismatch!"
         # control test
         assert not np.allclose(h5["events"]["bright_perc_10"][:],
                                data["bright_perc_90"])
+
+
+def test_basic_brightness_single_image():
+    # This original file was generated with dcevent for reference.
+    path = retrieve_data(data_path /
+                         "fmt-hdf5_cytoshot_full-features_2023.zip")
+    # Make data available
+    with h5py.File(path) as h5:
+        data = feat_brightness.brightness_features(
+            image=h5["events/image"][1][np.newaxis],
+            image_bg=h5["events/image_bg"][1][np.newaxis],
+            mask=h5["events/mask"][1][np.newaxis],
+        )
+
+        assert np.allclose(data["bright_bc_avg"][0],
+                           -43.75497215592681,
+                           atol=0, rtol=1e-10)
+        for feat in feat_brightness.brightness_names:
+            assert np.allclose(h5["events"][feat][1],
+                               data[feat][0]), f"Feature {feat} mismatch!"
+        # control test
+        assert not np.allclose(h5["events"]["bright_perc_10"][1],
+                               data["bright_perc_90"][0])
```

### Comparing `dcnum-0.11.1/tests/test_ppid.py` & `dcnum-0.11.2/tests/test_ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/tests/test_read_concat_hdf5.py` & `dcnum-0.11.2/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/tests/test_read_hdf5.py` & `dcnum-0.11.2/tests/test_read_hdf5.py`

 * *Files 18% similar despite different names*

```diff
@@ -130,30 +130,57 @@
 
 def test_pickling_state():
     path = retrieve_data(data_path /
                          "fmt-hdf5_cytoshot_full-features_2023.zip")
 
     h5d1 = read.HDF5Data(path)
     h5d1.pixel_size = 0.124
-    state = h5d1.__getstate__()
-    pstate = pickle.dumps(state)
-
-    state2 = pickle.loads(pstate)
-    h5d2 = read.HDF5Data(**state2)
+    pstate = pickle.dumps(h5d1)
+    h5d2 = pickle.loads(pstate)
     assert h5d1.md5_5m == h5d2.md5_5m
     assert h5d1.md5_5m == h5d2.md5_5m
     assert h5d1.pixel_size == h5d2.pixel_size
     assert np.allclose(h5d2.pixel_size, 0.124)
 
 
 def test_pickling_state_logs():
     path = retrieve_data(
         data_path / "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
     h5d1 = read.HDF5Data(path)
     h5d1.pixel_size = 0.124
-    state = h5d1.__getstate__()
-    pstate = pickle.dumps(state)
-
-    state2 = pickle.loads(pstate)
-    h5d2 = read.HDF5Data(**state2)
+    pstate = pickle.dumps(h5d1)
+    h5d2 = pickle.loads(pstate)
+    assert h5d1.logs
     for lk in h5d1.logs:
         assert h5d1.logs[lk] == h5d2.logs[lk]
+
+
+def test_pickling_state_tables():
+    path = retrieve_data(
+        data_path / "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
+    # The original file does not contain any tables, so we write
+    # generate a table
+    columns = ["alot", "of", "tables"]
+    ds_dt = np.dtype({'names': columns,
+                      'formats': [float] * len(columns)})
+    tab_data = np.zeros((11, len(columns)))
+    tab_data[:, 0] = np.arange(11)
+    tab_data[:, 1] = 1000
+    tab_data[:, 2] = np.linspace(1, np.sqrt(2), 11)
+    rec_arr = np.rec.array(tab_data, dtype=ds_dt)
+
+    # add table to source file
+    with h5py.File(path, "a") as h5:
+        h5tab = h5.require_group("tables")
+        h5tab.create_dataset(name="sample_table",
+                             data=rec_arr)
+
+    h5d1 = read.HDF5Data(path)
+    h5d1.pixel_size = 0.124
+    pstate = pickle.dumps(h5d1)
+    h5d2 = pickle.loads(pstate)
+    assert h5d1.tables
+    table = h5d1.tables["sample_table"]
+    assert len(table) == 3
+    for lk in table:
+        assert np.allclose(h5d1.tables["sample_table"][lk],
+                           h5d2.tables["sample_table"][lk])
```

### Comparing `dcnum-0.11.1/tests/test_write_deque_writer_thread.py` & `dcnum-0.11.2/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.1/tests/test_write_writer.py` & `dcnum-0.11.2/tests/test_write_writer.py`

 * *Files identical despite different names*

