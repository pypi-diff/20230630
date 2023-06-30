# Comparing `tmp/funfluid-202306302136.tar.gz` & `tmp/funfluid-202306302137.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funfluid-202306302136.tar", last modified: Fri Jun 30 13:36:04 2023, max compression
+gzip compressed data, was "funfluid-202306302137.tar", last modified: Fri Jun 30 13:37:11 2023, max compression
```

## Comparing `funfluid-202306302136.tar` & `funfluid-202306302137.tar`

### file list

```diff
@@ -1,102 +1,101 @@
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:49:06.000000 funfluid-202306302136/LICENSE
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-06-30 13:36:04.404837 funfluid-202306302136/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      145 2023-06-30 08:49:06.000000 funfluid-202306302136/README.md
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.392836 funfluid-202306302136/funfluid/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        2 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.396836 funfluid-202306302136/funfluid/common/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/common/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.396836 funfluid-202306302136/funfluid/common/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/common/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2837 2023-06-30 08:49:51.000000 funfluid-202306302136/funfluid/common/base/cache.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.396836 funfluid-202306302136/funfluid/common/flow/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/common/flow/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.396836 funfluid-202306302136/funfluid/common/particle/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/common/particle/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.400837 funfluid-202306302136/funfluid/experiment/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/experiment/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.400837 funfluid-202306302136/funfluid/experiment/chlamydomonas/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.400837 funfluid-202306302136/funfluid/experiment/chlamydomonas/analyse/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/analyse/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4563 2023-06-30 08:50:16.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/analyse/analyse.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.400837 funfluid-202306302136/funfluid/experiment/chlamydomonas/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3815 2023-06-30 08:50:20.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/base/base.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/base/globalconfig.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.400837 funfluid-202306302136/funfluid/experiment/chlamydomonas/detect/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/detect/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2977 2023-06-30 08:50:23.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/detect/background.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4707 2023-06-30 08:50:30.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/detect/contain.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     9205 2023-06-30 08:50:37.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/detect/particle.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.400837 funfluid-202306302136/funfluid/experiment/chlamydomonas/plot/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/plot/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/plot/core.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      239 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/plot/property.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.400837 funfluid-202306302136/funfluid/experiment/chlamydomonas/progress/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/progress/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2909 2023-06-30 08:50:45.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/progress/video_progress.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1573 2023-06-30 08:50:10.000000 funfluid-202306302136/funfluid/experiment/chlamydomonas/run.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.400837 funfluid-202306302136/funfluid/lbm/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       64 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.400837 funfluid-202306302136/funfluid/lbm/core/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       70 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/core/__init__.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/core/buff.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    21837 2023-06-30 08:50:49.000000 funfluid-202306302136/funfluid/lbm/core/lattice.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    13442 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/core/shape.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10645 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/core/speed_nb.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/lbm/example/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/example/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1921 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/example/example_cavity1.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1994 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/example/example_cavity3.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3324 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/example/example_obstacle.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2581 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/example/example_poiseuille.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3349 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/example/example_turek.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3662 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/obs_array.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2364 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/lbm/params.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/simulate/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:53:23.000000 funfluid-202306302136/funfluid/simulate/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/simulate/ellipse/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/simulate/ellipse/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:54:13.000000 funfluid-202306302136/funfluid/simulate/ellipse/analyse.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/simulate/ellipse/example/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/simulate/ellipse/example/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3179 2023-06-30 08:49:55.000000 funfluid-202306302136/funfluid/simulate/ellipse/example/largs_plot_example.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1379 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/simulate/ellipse/plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/simulate/ellipse/project/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:31:46.000000 funfluid-202306302136/funfluid/simulate/ellipse/project/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/simulate/ellipse/project/models/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:36.000000 funfluid-202306302136/funfluid/simulate/ellipse/project/models/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:30.000000 funfluid-202306302136/funfluid/simulate/ellipse/project/models/flow.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/simulate/ellipse/project/track/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       49 2023-06-30 13:35:57.000000 funfluid-202306302136/funfluid/simulate/ellipse/project/track/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     5909 2023-06-30 13:35:34.000000 funfluid-202306302136/funfluid/simulate/ellipse/project/track/core.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      955 2023-06-30 08:50:00.000000 funfluid-202306302136/funfluid/simulate/ellipse/project/track/example.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2970 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/simulate/ellipse/project/track/track_plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/simulate/ellipse/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/simulate/ellipse/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      563 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/simulate/ellipse/utils/largs_plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/tecplot/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/tecplot/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/tecplot/templates/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/tecplot/templates/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    15193 2023-06-30 08:50:52.000000 funfluid-202306302136/funfluid/tecplot/templates/templates1.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/tecplot/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/tecplot/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/tecplot/utils/connect.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/temp/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/temp/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1405 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/temp/data_fit.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       98 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/temp/temp1.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.404837 funfluid-202306302136/funfluid/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302136/funfluid/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 08:50:57.000000 funfluid-202306302136/funfluid/utils/log.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      729 2023-06-30 08:50:55.000000 funfluid-202306302136/funfluid/utils/timer.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:04.396836 funfluid-202306302136/funfluid.egg-info/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-06-30 13:36:04.000000 funfluid-202306302136/funfluid.egg-info/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2685 2023-06-30 13:36:04.000000 funfluid-202306302136/funfluid.egg-info/SOURCES.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-06-30 13:36:04.000000 funfluid-202306302136/funfluid.egg-info/dependency_links.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       12 2023-06-30 13:36:04.000000 funfluid-202306302136/funfluid.egg-info/requires.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-06-30 13:36:04.000000 funfluid-202306302136/funfluid.egg-info/top_level.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-06-30 13:36:04.404837 funfluid-202306302136/setup.cfg
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      399 2023-06-30 08:49:30.000000 funfluid-202306302136/setup.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.450753 funfluid-202306302137/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:49:06.000000 funfluid-202306302137/LICENSE
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-06-30 13:37:11.450753 funfluid-202306302137/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      145 2023-06-30 08:49:06.000000 funfluid-202306302137/README.md
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.442753 funfluid-202306302137/funfluid/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        2 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/common/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/common/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/common/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/common/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2837 2023-06-30 08:49:51.000000 funfluid-202306302137/funfluid/common/base/cache.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/common/flow/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/common/flow/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/common/particle/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/common/particle/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/experiment/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/experiment/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/experiment/chlamydomonas/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/experiment/chlamydomonas/analyse/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/analyse/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4563 2023-06-30 08:50:16.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/analyse/analyse.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/experiment/chlamydomonas/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3815 2023-06-30 08:50:20.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/base/base.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/base/globalconfig.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/experiment/chlamydomonas/detect/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/detect/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2977 2023-06-30 08:50:23.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/detect/background.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4707 2023-06-30 08:50:30.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/detect/contain.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     9205 2023-06-30 08:50:37.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/detect/particle.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/experiment/chlamydomonas/plot/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/plot/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/plot/core.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      239 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/plot/property.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/experiment/chlamydomonas/progress/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/progress/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2909 2023-06-30 08:50:45.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/progress/video_progress.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1573 2023-06-30 08:50:10.000000 funfluid-202306302137/funfluid/experiment/chlamydomonas/run.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/lbm/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       64 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/lbm/core/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       70 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/core/__init__.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/core/buff.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    21837 2023-06-30 08:50:49.000000 funfluid-202306302137/funfluid/lbm/core/lattice.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    13442 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/core/shape.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10645 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/core/speed_nb.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/lbm/example/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/example/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1921 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/example/example_cavity1.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1994 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/example/example_cavity3.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3324 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/example/example_obstacle.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2581 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/example/example_poiseuille.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3349 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/example/example_turek.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3662 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/obs_array.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2364 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/lbm/params.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/simulate/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:53:23.000000 funfluid-202306302137/funfluid/simulate/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid/simulate/ellipse/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/simulate/ellipse/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:54:13.000000 funfluid-202306302137/funfluid/simulate/ellipse/analyse.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.450753 funfluid-202306302137/funfluid/simulate/ellipse/example/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/simulate/ellipse/example/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3179 2023-06-30 08:49:55.000000 funfluid-202306302137/funfluid/simulate/ellipse/example/largs_plot_example.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1379 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/simulate/ellipse/plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.450753 funfluid-202306302137/funfluid/simulate/ellipse/project/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:31:46.000000 funfluid-202306302137/funfluid/simulate/ellipse/project/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.450753 funfluid-202306302137/funfluid/simulate/ellipse/project/models/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:36.000000 funfluid-202306302137/funfluid/simulate/ellipse/project/models/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:30.000000 funfluid-202306302137/funfluid/simulate/ellipse/project/models/flow.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:57.000000 funfluid-202306302137/funfluid/simulate/ellipse/project/project.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.450753 funfluid-202306302137/funfluid/simulate/ellipse/project/track/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       49 2023-06-30 13:36:34.000000 funfluid-202306302137/funfluid/simulate/ellipse/project/track/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     5909 2023-06-30 13:35:34.000000 funfluid-202306302137/funfluid/simulate/ellipse/project/track/plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.450753 funfluid-202306302137/funfluid/simulate/ellipse/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/simulate/ellipse/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      563 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/simulate/ellipse/utils/largs_plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.450753 funfluid-202306302137/funfluid/tecplot/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/tecplot/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.450753 funfluid-202306302137/funfluid/tecplot/templates/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/tecplot/templates/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    15193 2023-06-30 08:50:52.000000 funfluid-202306302137/funfluid/tecplot/templates/templates1.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.450753 funfluid-202306302137/funfluid/tecplot/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/tecplot/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/tecplot/utils/connect.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.450753 funfluid-202306302137/funfluid/temp/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/temp/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1405 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/temp/data_fit.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       98 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/temp/temp1.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.450753 funfluid-202306302137/funfluid/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302137/funfluid/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 08:50:57.000000 funfluid-202306302137/funfluid/utils/log.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      729 2023-06-30 08:50:55.000000 funfluid-202306302137/funfluid/utils/timer.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:37:11.446753 funfluid-202306302137/funfluid.egg-info/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-06-30 13:37:11.000000 funfluid-202306302137/funfluid.egg-info/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2625 2023-06-30 13:37:11.000000 funfluid-202306302137/funfluid.egg-info/SOURCES.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-06-30 13:37:11.000000 funfluid-202306302137/funfluid.egg-info/dependency_links.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       12 2023-06-30 13:37:11.000000 funfluid-202306302137/funfluid.egg-info/requires.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-06-30 13:37:11.000000 funfluid-202306302137/funfluid.egg-info/top_level.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-06-30 13:37:11.450753 funfluid-202306302137/setup.cfg
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      399 2023-06-30 08:49:30.000000 funfluid-202306302137/setup.py
```

### Comparing `funfluid-202306302136/LICENSE` & `funfluid-202306302137/LICENSE`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/common/base/cache.py` & `funfluid-202306302137/funfluid/common/base/cache.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/experiment/chlamydomonas/analyse/analyse.py` & `funfluid-202306302137/funfluid/experiment/chlamydomonas/analyse/analyse.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/experiment/chlamydomonas/base/base.py` & `funfluid-202306302137/funfluid/experiment/chlamydomonas/base/base.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/experiment/chlamydomonas/base/globalconfig.py` & `funfluid-202306302137/funfluid/experiment/chlamydomonas/base/globalconfig.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/experiment/chlamydomonas/detect/background.py` & `funfluid-202306302137/funfluid/experiment/chlamydomonas/detect/background.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/experiment/chlamydomonas/detect/contain.py` & `funfluid-202306302137/funfluid/experiment/chlamydomonas/detect/contain.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/experiment/chlamydomonas/detect/particle.py` & `funfluid-202306302137/funfluid/experiment/chlamydomonas/detect/particle.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/experiment/chlamydomonas/progress/video_progress.py` & `funfluid-202306302137/funfluid/experiment/chlamydomonas/progress/video_progress.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/experiment/chlamydomonas/run.py` & `funfluid-202306302137/funfluid/experiment/chlamydomonas/run.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/lbm/core/buff.py` & `funfluid-202306302137/funfluid/lbm/core/buff.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/lbm/core/lattice.py` & `funfluid-202306302137/funfluid/lbm/core/lattice.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/lbm/core/shape.py` & `funfluid-202306302137/funfluid/lbm/core/shape.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/lbm/core/speed_nb.py` & `funfluid-202306302137/funfluid/lbm/core/speed_nb.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/lbm/example/example_cavity1.py` & `funfluid-202306302137/funfluid/lbm/example/example_cavity1.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/lbm/example/example_cavity3.py` & `funfluid-202306302137/funfluid/lbm/example/example_cavity3.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/lbm/example/example_obstacle.py` & `funfluid-202306302137/funfluid/lbm/example/example_obstacle.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/lbm/example/example_poiseuille.py` & `funfluid-202306302137/funfluid/lbm/example/example_poiseuille.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/lbm/example/example_turek.py` & `funfluid-202306302137/funfluid/lbm/example/example_turek.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/lbm/obs_array.py` & `funfluid-202306302137/funfluid/lbm/obs_array.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/lbm/params.py` & `funfluid-202306302137/funfluid/lbm/params.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/simulate/ellipse/example/largs_plot_example.py` & `funfluid-202306302137/funfluid/simulate/ellipse/example/largs_plot_example.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/simulate/ellipse/plot.py` & `funfluid-202306302137/funfluid/simulate/ellipse/plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/simulate/ellipse/project/track/core.py` & `funfluid-202306302137/funfluid/simulate/ellipse/project/track/plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/simulate/ellipse/utils/largs_plot.py` & `funfluid-202306302137/funfluid/simulate/ellipse/utils/largs_plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/tecplot/templates/templates1.py` & `funfluid-202306302137/funfluid/tecplot/templates/templates1.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/temp/data_fit.py` & `funfluid-202306302137/funfluid/temp/data_fit.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid/utils/timer.py` & `funfluid-202306302137/funfluid/utils/timer.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302136/funfluid.egg-info/SOURCES.txt` & `funfluid-202306302137/funfluid.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,20 +46,19 @@
 funfluid/simulate/__init__.py
 funfluid/simulate/ellipse/__init__.py
 funfluid/simulate/ellipse/analyse.py
 funfluid/simulate/ellipse/plot.py
 funfluid/simulate/ellipse/example/__init__.py
 funfluid/simulate/ellipse/example/largs_plot_example.py
 funfluid/simulate/ellipse/project/__init__.py
+funfluid/simulate/ellipse/project/project.py
 funfluid/simulate/ellipse/project/models/__init__.py
 funfluid/simulate/ellipse/project/models/flow.py
 funfluid/simulate/ellipse/project/track/__init__.py
-funfluid/simulate/ellipse/project/track/core.py
-funfluid/simulate/ellipse/project/track/example.py
-funfluid/simulate/ellipse/project/track/track_plot.py
+funfluid/simulate/ellipse/project/track/plot.py
 funfluid/simulate/ellipse/utils/__init__.py
 funfluid/simulate/ellipse/utils/largs_plot.py
 funfluid/tecplot/__init__.py
 funfluid/tecplot/templates/__init__.py
 funfluid/tecplot/templates/templates1.py
 funfluid/tecplot/utils/__init__.py
 funfluid/tecplot/utils/connect.py
```

