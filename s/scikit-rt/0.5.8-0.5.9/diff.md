# Comparing `tmp/scikit-rt-0.5.8.tar.gz` & `tmp/scikit-rt-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-rt-0.5.8.tar", last modified: Thu Jun 29 23:32:25 2023, max compression
+gzip compressed data, was "scikit-rt-0.5.9.tar", last modified: Fri Jun 30 16:50:09 2023, max compression
```

## Comparing `scikit-rt-0.5.8.tar` & `scikit-rt-0.5.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:32:25.474924 scikit-rt-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-29 23:32:25.474924 scikit-rt-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/pypi.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-29 23:32:25.478924 scikit-rt-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:32:25.450923 scikit-rt-0.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:32:25.450923 scikit-rt-0.5.8/src/scikit_rt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-29 23:32:25.000000 scikit-rt-0.5.8/src/scikit_rt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-29 23:32:25.000000 scikit-rt-0.5.8/src/scikit_rt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:32:25.000000 scikit-rt-0.5.8/src/scikit_rt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-29 23:32:25.000000 scikit-rt-0.5.8/src/scikit_rt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 23:32:25.000000 scikit-rt-0.5.8/src/scikit_rt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:32:25.458923 scikit-rt-0.5.8/src/skrt/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:32:25.462923 scikit-rt-0.5.8/src/skrt/better_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)   132535 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/better_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/better_viewer/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    76116 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:32:25.450923 scikit-rt-0.5.8/src/skrt/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:32:25.462923 scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/MI_Affine.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/MI_Translation.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:32:25.462923 scikit-rt-0.5.8/src/skrt/data/niftyreg_parameter_files/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/niftyreg_parameter_files/Affine.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/data/niftyreg_parameter_files/Rigid.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27334 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/dicom_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39944 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/dose.py
--rw-r--r--   0 runner    (1001) docker     (123)   257359 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)   118936 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/patient.py
--rw-r--r--   0 runner    (1001) docker     (123)   152018 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    61265 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)   358501 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:32:25.466923 scikit-rt-0.5.8/src/skrt/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/viewer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/src/skrt/viewer/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:32:25.474924 scikit-rt-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_01_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_dose.py
--rw-r--r--   0 runner    (1001) docker     (123)    61981 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_patient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_qv_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_qv_quickviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_qv_struct_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_qv_struct_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_qv_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34841 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_roi_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_synthetic_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-29 23:28:04.000000 scikit-rt-0.5.8/tests/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:50:09.963344 scikit-rt-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-30 16:50:09.963344 scikit-rt-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/pypi.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-30 16:50:09.963344 scikit-rt-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:50:09.935344 scikit-rt-0.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:50:09.939344 scikit-rt-0.5.9/src/scikit_rt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-30 16:50:09.000000 scikit-rt-0.5.9/src/scikit_rt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-30 16:50:09.000000 scikit-rt-0.5.9/src/scikit_rt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:50:09.000000 scikit-rt-0.5.9/src/scikit_rt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-30 16:50:09.000000 scikit-rt-0.5.9/src/scikit_rt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 16:50:09.000000 scikit-rt-0.5.9/src/scikit_rt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:50:09.947344 scikit-rt-0.5.9/src/skrt/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:50:09.951344 scikit-rt-0.5.9/src/skrt/better_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)   132535 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/better_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/better_viewer/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76116 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:50:09.935344 scikit-rt-0.5.9/src/skrt/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:50:09.951344 scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/MI_Affine.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/MI_Translation.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:50:09.951344 scikit-rt-0.5.9/src/skrt/data/niftyreg_parameter_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/niftyreg_parameter_files/Affine.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/data/niftyreg_parameter_files/Rigid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27334 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/dicom_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39944 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)   257359 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118936 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152018 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61265 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   358501 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:50:09.955344 scikit-rt-0.5.9/src/skrt/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/viewer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/src/skrt/viewer/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:50:09.963344 scikit-rt-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_01_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61981 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_qv_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_qv_quickviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_qv_struct_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_qv_struct_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_qv_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34841 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_roi_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_synthetic_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-30 16:45:58.000000 scikit-rt-0.5.9/tests/test_viewer.py
```

### Comparing `scikit-rt-0.5.8/LICENSE` & `scikit-rt-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/PKG-INFO` & `scikit-rt-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.5.8
+Version: 0.5.9
 Summary: Toolkit for analysis of radiotherapy data
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.5.8/README.md` & `scikit-rt-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/pypi.md` & `scikit-rt-0.5.9/pypi.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/setup.cfg` & `scikit-rt-0.5.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scikit-rt
-version = 0.5.8
+version = 0.5.9
 author = H. Pullen, K. Harrison
 author_email = scikit-rt@hep.phy.cam.ac.uk
 description = Toolkit for analysis of radiotherapy data
 long_description = file: pypi.md
 long_description_content_type = text/markdown
 url = https://github.com/scikit-rt/scikit-rt
 project_urls =
```

### Comparing `scikit-rt-0.5.8/src/scikit_rt.egg-info/PKG-INFO` & `scikit-rt-0.5.9/src/scikit_rt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.5.8
+Version: 0.5.9
 Summary: Toolkit for analysis of radiotherapy data
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.5.8/src/scikit_rt.egg-info/SOURCES.txt` & `scikit-rt-0.5.9/src/scikit_rt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/scikit_rt.egg-info/requires.txt` & `scikit-rt-0.5.9/src/scikit_rt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/__init__.py` & `scikit-rt-0.5.9/src/skrt/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/application.py` & `scikit-rt-0.5.9/src/skrt/application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/better_viewer/__init__.py` & `scikit-rt-0.5.9/src/skrt/better_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/better_viewer/options.py` & `scikit-rt-0.5.9/src/skrt/better_viewer/options.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/core.py` & `scikit-rt-0.5.9/src/skrt/core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt` & `scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/MI_Affine.txt` & `scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/MI_Affine.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt` & `scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt` & `scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt` & `scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/MI_Rigid.txt` & `scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/MI_Rigid.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/data/elastix_parameter_files/MI_Translation.txt` & `scikit-rt-0.5.9/src/skrt/data/elastix_parameter_files/MI_Translation.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/dicom_writer.py` & `scikit-rt-0.5.9/src/skrt/dicom_writer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/dose.py` & `scikit-rt-0.5.9/src/skrt/dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/image.py` & `scikit-rt-0.5.9/src/skrt/image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/multi.py` & `scikit-rt-0.5.9/src/skrt/multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/patient.py` & `scikit-rt-0.5.9/src/skrt/patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/registration.py` & `scikit-rt-0.5.9/src/skrt/registration.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/segmentation.py` & `scikit-rt-0.5.9/src/skrt/segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/simulation.py` & `scikit-rt-0.5.9/src/skrt/simulation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/structures.py` & `scikit-rt-0.5.9/src/skrt/structures.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/viewer/core.py` & `scikit-rt-0.5.9/src/skrt/viewer/core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/src/skrt/viewer/viewer.py` & `scikit-rt-0.5.9/src/skrt/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_01_setup.py` & `scikit-rt-0.5.9/tests/test_01_setup.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_application.py` & `scikit-rt-0.5.9/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_core.py` & `scikit-rt-0.5.9/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_dose.py` & `scikit-rt-0.5.9/tests/test_dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_image.py` & `scikit-rt-0.5.9/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_multi.py` & `scikit-rt-0.5.9/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_patient.py` & `scikit-rt-0.5.9/tests/test_patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_qv_image.py` & `scikit-rt-0.5.9/tests/test_qv_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_qv_quickviewer.py` & `scikit-rt-0.5.9/tests/test_qv_quickviewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_qv_struct_loader.py` & `scikit-rt-0.5.9/tests/test_qv_struct_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_qv_struct_metrics.py` & `scikit-rt-0.5.9/tests/test_qv_struct_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_qv_structs.py` & `scikit-rt-0.5.9/tests/test_qv_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_registration.py` & `scikit-rt-0.5.9/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_roi_metrics.py` & `scikit-rt-0.5.9/tests/test_roi_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_segmentation.py` & `scikit-rt-0.5.9/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_structs.py` & `scikit-rt-0.5.9/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_synthetic_image.py` & `scikit-rt-0.5.9/tests/test_synthetic_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.8/tests/test_viewer.py` & `scikit-rt-0.5.9/tests/test_viewer.py`

 * *Files identical despite different names*

