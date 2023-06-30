# Comparing `tmp/funfluid-202306302050.tar.gz` & `tmp/funfluid-202306302052.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funfluid-202306302050.tar", last modified: Fri Jun 30 12:50:53 2023, max compression
+gzip compressed data, was "funfluid-202306302052.tar", last modified: Fri Jun 30 12:52:12 2023, max compression
```

## Comparing `funfluid-202306302050.tar` & `funfluid-202306302052.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.504052 funfluid-202306302050/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:49:06.000000 funfluid-202306302050/LICENSE
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-06-30 12:50:53.504052 funfluid-202306302050/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      145 2023-06-30 08:49:06.000000 funfluid-202306302050/README.md
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.492052 funfluid-202306302050/funfluid/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        2 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.492052 funfluid-202306302050/funfluid/common/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/common/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.492052 funfluid-202306302050/funfluid/common/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/common/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2837 2023-06-30 08:49:51.000000 funfluid-202306302050/funfluid/common/base/cache.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.492052 funfluid-202306302050/funfluid/common/flow/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/common/flow/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.496052 funfluid-202306302050/funfluid/common/particle/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/common/particle/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.496052 funfluid-202306302050/funfluid/ellipse/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/ellipse/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.496052 funfluid-202306302050/funfluid/ellipse/example/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/ellipse/example/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3179 2023-06-30 08:49:55.000000 funfluid-202306302050/funfluid/ellipse/example/largs_plot_example.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1379 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/ellipse/plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.496052 funfluid-202306302050/funfluid/ellipse/track/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/ellipse/track/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      955 2023-06-30 08:50:00.000000 funfluid-202306302050/funfluid/ellipse/track/example.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2970 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/ellipse/track/track_plot.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     5931 2023-06-30 12:50:50.000000 funfluid-202306302050/funfluid/ellipse/track/track_plot2.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.500052 funfluid-202306302050/funfluid/ellipse/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/ellipse/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      563 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/ellipse/utils/largs_plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.500052 funfluid-202306302050/funfluid/experiment/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/experiment/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.500052 funfluid-202306302050/funfluid/experiment/chlamydomonas/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.500052 funfluid-202306302050/funfluid/experiment/chlamydomonas/analyse/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/analyse/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4563 2023-06-30 08:50:16.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/analyse/analyse.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.500052 funfluid-202306302050/funfluid/experiment/chlamydomonas/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3815 2023-06-30 08:50:20.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/base/base.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/base/globalconfig.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.500052 funfluid-202306302050/funfluid/experiment/chlamydomonas/detect/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/detect/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2977 2023-06-30 08:50:23.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/detect/background.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4707 2023-06-30 08:50:30.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/detect/contain.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     9205 2023-06-30 08:50:37.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/detect/particle.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.500052 funfluid-202306302050/funfluid/experiment/chlamydomonas/plot/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/plot/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/plot/core.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      239 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/plot/property.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.500052 funfluid-202306302050/funfluid/experiment/chlamydomonas/progress/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/progress/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2909 2023-06-30 08:50:45.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/progress/video_progress.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1573 2023-06-30 08:50:10.000000 funfluid-202306302050/funfluid/experiment/chlamydomonas/run.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.500052 funfluid-202306302050/funfluid/lbm/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       64 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.500052 funfluid-202306302050/funfluid/lbm/core/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       70 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/core/__init__.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/core/buff.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    21837 2023-06-30 08:50:49.000000 funfluid-202306302050/funfluid/lbm/core/lattice.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    13442 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/core/shape.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10645 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/core/speed_nb.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.504052 funfluid-202306302050/funfluid/lbm/example/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/example/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1921 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/example/example_cavity1.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1994 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/example/example_cavity3.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3324 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/example/example_obstacle.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2581 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/example/example_poiseuille.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3349 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/example/example_turek.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3662 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/obs_array.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2364 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/lbm/params.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.504052 funfluid-202306302050/funfluid/tecplot/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/tecplot/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.504052 funfluid-202306302050/funfluid/tecplot/templates/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/tecplot/templates/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    15193 2023-06-30 08:50:52.000000 funfluid-202306302050/funfluid/tecplot/templates/templates1.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.504052 funfluid-202306302050/funfluid/tecplot/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/tecplot/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/tecplot/utils/connect.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.504052 funfluid-202306302050/funfluid/temp/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/temp/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1405 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/temp/data_fit.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       98 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/temp/temp1.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.504052 funfluid-202306302050/funfluid/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302050/funfluid/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 08:50:57.000000 funfluid-202306302050/funfluid/utils/log.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      729 2023-06-30 08:50:55.000000 funfluid-202306302050/funfluid/utils/timer.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:50:53.492052 funfluid-202306302050/funfluid.egg-info/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-06-30 12:50:53.000000 funfluid-202306302050/funfluid.egg-info/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2355 2023-06-30 12:50:53.000000 funfluid-202306302050/funfluid.egg-info/SOURCES.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-06-30 12:50:53.000000 funfluid-202306302050/funfluid.egg-info/dependency_links.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       12 2023-06-30 12:50:53.000000 funfluid-202306302050/funfluid.egg-info/requires.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-06-30 12:50:53.000000 funfluid-202306302050/funfluid.egg-info/top_level.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-06-30 12:50:53.504052 funfluid-202306302050/setup.cfg
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      399 2023-06-30 08:49:30.000000 funfluid-202306302050/setup.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.118265 funfluid-202306302052/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:49:06.000000 funfluid-202306302052/LICENSE
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-06-30 12:52:12.118265 funfluid-202306302052/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      145 2023-06-30 08:49:06.000000 funfluid-202306302052/README.md
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.102264 funfluid-202306302052/funfluid/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        2 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.106264 funfluid-202306302052/funfluid/common/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/common/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.106264 funfluid-202306302052/funfluid/common/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/common/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2837 2023-06-30 08:49:51.000000 funfluid-202306302052/funfluid/common/base/cache.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.106264 funfluid-202306302052/funfluid/common/flow/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/common/flow/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.110264 funfluid-202306302052/funfluid/common/particle/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/common/particle/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.110264 funfluid-202306302052/funfluid/ellipse/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/ellipse/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.110264 funfluid-202306302052/funfluid/ellipse/example/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/ellipse/example/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3179 2023-06-30 08:49:55.000000 funfluid-202306302052/funfluid/ellipse/example/largs_plot_example.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1379 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/ellipse/plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.114264 funfluid-202306302052/funfluid/ellipse/track/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/ellipse/track/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      955 2023-06-30 08:50:00.000000 funfluid-202306302052/funfluid/ellipse/track/example.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2970 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/ellipse/track/track_plot.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     5906 2023-06-30 12:52:08.000000 funfluid-202306302052/funfluid/ellipse/track/track_plot2.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.114264 funfluid-202306302052/funfluid/ellipse/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/ellipse/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      563 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/ellipse/utils/largs_plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.114264 funfluid-202306302052/funfluid/experiment/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/experiment/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.114264 funfluid-202306302052/funfluid/experiment/chlamydomonas/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.114264 funfluid-202306302052/funfluid/experiment/chlamydomonas/analyse/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/analyse/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4563 2023-06-30 08:50:16.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/analyse/analyse.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.114264 funfluid-202306302052/funfluid/experiment/chlamydomonas/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3815 2023-06-30 08:50:20.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/base/base.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/base/globalconfig.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.114264 funfluid-202306302052/funfluid/experiment/chlamydomonas/detect/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/detect/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2977 2023-06-30 08:50:23.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/detect/background.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4707 2023-06-30 08:50:30.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/detect/contain.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     9205 2023-06-30 08:50:37.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/detect/particle.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.114264 funfluid-202306302052/funfluid/experiment/chlamydomonas/plot/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/plot/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/plot/core.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      239 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/plot/property.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.114264 funfluid-202306302052/funfluid/experiment/chlamydomonas/progress/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/progress/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2909 2023-06-30 08:50:45.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/progress/video_progress.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1573 2023-06-30 08:50:10.000000 funfluid-202306302052/funfluid/experiment/chlamydomonas/run.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.114264 funfluid-202306302052/funfluid/lbm/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       64 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.118265 funfluid-202306302052/funfluid/lbm/core/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       70 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/core/__init__.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/core/buff.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    21837 2023-06-30 08:50:49.000000 funfluid-202306302052/funfluid/lbm/core/lattice.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    13442 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/core/shape.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10645 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/core/speed_nb.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.118265 funfluid-202306302052/funfluid/lbm/example/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/example/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1921 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/example/example_cavity1.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1994 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/example/example_cavity3.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3324 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/example/example_obstacle.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2581 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/example/example_poiseuille.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3349 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/example/example_turek.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3662 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/obs_array.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2364 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/lbm/params.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.118265 funfluid-202306302052/funfluid/tecplot/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/tecplot/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.118265 funfluid-202306302052/funfluid/tecplot/templates/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/tecplot/templates/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    15193 2023-06-30 08:50:52.000000 funfluid-202306302052/funfluid/tecplot/templates/templates1.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.118265 funfluid-202306302052/funfluid/tecplot/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/tecplot/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/tecplot/utils/connect.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.118265 funfluid-202306302052/funfluid/temp/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/temp/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1405 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/temp/data_fit.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       98 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/temp/temp1.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.118265 funfluid-202306302052/funfluid/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202306302052/funfluid/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 08:50:57.000000 funfluid-202306302052/funfluid/utils/log.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      729 2023-06-30 08:50:55.000000 funfluid-202306302052/funfluid/utils/timer.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:52:12.106264 funfluid-202306302052/funfluid.egg-info/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-06-30 12:52:12.000000 funfluid-202306302052/funfluid.egg-info/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2355 2023-06-30 12:52:12.000000 funfluid-202306302052/funfluid.egg-info/SOURCES.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-06-30 12:52:12.000000 funfluid-202306302052/funfluid.egg-info/dependency_links.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       12 2023-06-30 12:52:12.000000 funfluid-202306302052/funfluid.egg-info/requires.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-06-30 12:52:12.000000 funfluid-202306302052/funfluid.egg-info/top_level.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-06-30 12:52:12.118265 funfluid-202306302052/setup.cfg
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      399 2023-06-30 08:49:30.000000 funfluid-202306302052/setup.py
```

### Comparing `funfluid-202306302050/LICENSE` & `funfluid-202306302052/LICENSE`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/common/base/cache.py` & `funfluid-202306302052/funfluid/common/base/cache.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/ellipse/example/largs_plot_example.py` & `funfluid-202306302052/funfluid/ellipse/example/largs_plot_example.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/ellipse/plot.py` & `funfluid-202306302052/funfluid/ellipse/plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/ellipse/track/example.py` & `funfluid-202306302052/funfluid/ellipse/track/example.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/ellipse/track/track_plot.py` & `funfluid-202306302052/funfluid/ellipse/track/track_plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/ellipse/track/track_plot2.py` & `funfluid-202306302052/funfluid/ellipse/track/track_plot2.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,19 +25,16 @@
 
 
 class EllipseTrack:
     def __init__(self, df, a=10, b=5, color=None, marker=None, *args, **kwargs):
         self.df = df
         self.a = a
         self.b = b
-
         self.color = color
         self.marker = marker
-
-        # 圆心轨迹
         self.snapshot_steps = []
         self.lns = []
 
     def transform(self):
         self.df['xx'] = self.df['x']
         self.df['x'] = self.df['y']
         self.df['y'] = self.df['xx']
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `funfluid-202306302050/funfluid/ellipse/utils/largs_plot.py` & `funfluid-202306302052/funfluid/ellipse/utils/largs_plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/experiment/chlamydomonas/analyse/analyse.py` & `funfluid-202306302052/funfluid/experiment/chlamydomonas/analyse/analyse.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/experiment/chlamydomonas/base/base.py` & `funfluid-202306302052/funfluid/experiment/chlamydomonas/base/base.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/experiment/chlamydomonas/base/globalconfig.py` & `funfluid-202306302052/funfluid/experiment/chlamydomonas/base/globalconfig.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/experiment/chlamydomonas/detect/background.py` & `funfluid-202306302052/funfluid/experiment/chlamydomonas/detect/background.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/experiment/chlamydomonas/detect/contain.py` & `funfluid-202306302052/funfluid/experiment/chlamydomonas/detect/contain.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/experiment/chlamydomonas/detect/particle.py` & `funfluid-202306302052/funfluid/experiment/chlamydomonas/detect/particle.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/experiment/chlamydomonas/progress/video_progress.py` & `funfluid-202306302052/funfluid/experiment/chlamydomonas/progress/video_progress.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/experiment/chlamydomonas/run.py` & `funfluid-202306302052/funfluid/experiment/chlamydomonas/run.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/lbm/core/buff.py` & `funfluid-202306302052/funfluid/lbm/core/buff.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/lbm/core/lattice.py` & `funfluid-202306302052/funfluid/lbm/core/lattice.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/lbm/core/shape.py` & `funfluid-202306302052/funfluid/lbm/core/shape.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/lbm/core/speed_nb.py` & `funfluid-202306302052/funfluid/lbm/core/speed_nb.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/lbm/example/example_cavity1.py` & `funfluid-202306302052/funfluid/lbm/example/example_cavity1.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/lbm/example/example_cavity3.py` & `funfluid-202306302052/funfluid/lbm/example/example_cavity3.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/lbm/example/example_obstacle.py` & `funfluid-202306302052/funfluid/lbm/example/example_obstacle.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/lbm/example/example_poiseuille.py` & `funfluid-202306302052/funfluid/lbm/example/example_poiseuille.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/lbm/example/example_turek.py` & `funfluid-202306302052/funfluid/lbm/example/example_turek.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/lbm/obs_array.py` & `funfluid-202306302052/funfluid/lbm/obs_array.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/lbm/params.py` & `funfluid-202306302052/funfluid/lbm/params.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/tecplot/templates/templates1.py` & `funfluid-202306302052/funfluid/tecplot/templates/templates1.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/temp/data_fit.py` & `funfluid-202306302052/funfluid/temp/data_fit.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid/utils/timer.py` & `funfluid-202306302052/funfluid/utils/timer.py`

 * *Files identical despite different names*

### Comparing `funfluid-202306302050/funfluid.egg-info/SOURCES.txt` & `funfluid-202306302052/funfluid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

