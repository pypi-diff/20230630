# Comparing `tmp/cell-tracking-bc-2023.6.tar.gz` & `tmp/cell-tracking-bc-2023.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cell-tracking-bc-2023.6.tar", last modified: Wed Jun 21 15:04:36 2023, max compression
+gzip compressed data, was "cell-tracking-bc-2023.7.tar", last modified: Fri Jun 30 08:19:48 2023, max compression
```

## Comparing `cell-tracking-bc-2023.6.tar` & `cell-tracking-bc-2023.7.tar`

### file list

```diff
@@ -1,142 +1,143 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/
--rw-r--r--   0 eric      (1000) users      (984)       61 2023-06-21 15:02:20.000000 cell-tracking-bc-2023.6/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     3114 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2021-02-02 12:30:22.000000 cell-tracking-bc-2023.6/README-COPYRIGHT.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 cell-tracking-bc-2023.6/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     2286 2022-02-03 09:12:09.000000 cell-tracking-bc-2023.6/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/channel/
--rw-r--r--   0 eric      (1000) users      (984)     1969 2023-02-13 12:56:29.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/channel/ratio.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/geometrical/
--rw-r--r--   0 eric      (1000) users      (984)        0 2023-02-15 15:28:16.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/geometrical/dummy.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/radiometric/
--rw-r--r--   0 eric      (1000) users      (984)     2574 2023-02-10 13:45:02.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/radiometric/entropy.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/set/
--rw-r--r--   0 eric      (1000) users      (984)     2532 2023-02-10 15:24:31.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/set/numpy_.py
--rw-r--r--   0 eric      (1000) users      (984)     4169 2023-02-10 15:24:31.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/set/skimage_.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/temporal/
--rw-r--r--   0 eric      (1000) users      (984)     2140 2023-02-10 15:02:24.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/temporal/shift.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/matching/
--rw-r--r--   0 eric      (1000) users      (984)     1985 2021-09-08 16:51:38.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/matching/jaccard.py
--rw-r--r--   0 eric      (1000) users      (984)     3209 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/parser.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/
--rw-r--r--   0 eric      (1000) users      (984)     3866 2023-02-10 13:53:35.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/background.py
--rw-r--r--   0 eric      (1000) users      (984)     1976 2023-02-10 13:53:54.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/contrast.py
--rw-r--r--   0 eric      (1000) users      (984)     2503 2023-02-10 13:54:29.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/geometry.py
--rw-r--r--   0 eric      (1000) users      (984)     2991 2023-02-10 13:55:52.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/registration.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/segmentation/
--rw-r--r--   0 eric      (1000) users      (984)     4782 2023-06-12 11:59:41.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/segmentation/tf_network.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/tracking/
--rw-r--r--   0 eric      (1000) users      (984)     5631 2023-02-10 13:58:46.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/tracking/gmb_tracker.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/
--rw-r--r--   0 eric      (1000) users      (984)    10676 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/event.py
--rw-r--r--   0 eric      (1000) users      (984)     6728 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/feature.py
--rw-r--r--   0 eric      (1000) users      (984)     4916 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/path.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/
--rw-r--r--   0 eric      (1000) users      (984)     3076 2023-02-08 13:52:59.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/cell.py
--rw-r--r--   0 eric      (1000) users      (984)     3480 2023-02-08 13:56:27.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/chart.py
--rw-r--r--   0 eric      (1000) users      (984)     2388 2023-02-08 13:57:24.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/column.py
--rw-r--r--   0 eric      (1000) users      (984)     2208 2023-02-11 18:31:12.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/sheet.py
--rw-r--r--   0 eric      (1000) users      (984)     5734 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/track.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/
--rw-r--r--   0 eric      (1000) users      (984)     7863 2023-01-24 09:27:19.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/annotations.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/
--rw-r--r--   0 eric      (1000) users      (984)     2754 2022-02-17 13:49:51.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/context.py
--rw-r--r--   0 eric      (1000) users      (984)     9151 2023-01-18 14:25:10.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_2.py
--rw-r--r--   0 eric      (1000) users      (984)     7982 2022-07-09 12:00:34.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_3.py
--rw-r--r--   0 eric      (1000) users      (984)     8450 2023-02-17 09:42:06.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_any.py
--rw-r--r--   0 eric      (1000) users      (984)     6053 2022-05-31 12:24:19.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/event.py
--rw-r--r--   0 eric      (1000) users      (984)     2798 2021-11-10 10:18:31.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/style.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/
--rw-r--r--   0 eric      (1000) users      (984)     1891 2022-02-01 15:12:55.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/context.py
--rw-r--r--   0 eric      (1000) users      (984)     8915 2022-02-01 15:14:31.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/d_3.py
--rw-r--r--   0 eric      (1000) users      (984)     5376 2022-02-23 16:34:49.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/d_any.py
--rw-r--r--   0 eric      (1000) users      (984)     1873 2022-02-01 15:24:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/missing.py
--rw-r--r--   0 eric      (1000) users      (984)     3207 2022-02-01 15:15:32.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/style.py
--rw-r--r--   0 eric      (1000) users      (984)    14278 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/event.py
--rw-r--r--   0 eric      (1000) users      (984)     3736 2023-01-11 13:41:46.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/feature.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/
--rw-r--r--   0 eric      (1000) users      (984)     4751 2023-01-18 14:26:08.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/d_2.py
--rw-r--r--   0 eric      (1000) users      (984)     4918 2023-01-11 13:38:38.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/d_3.py
--rw-r--r--   0 eric      (1000) users      (984)     2642 2023-01-20 16:01:30.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/d_any.py
--rw-r--r--   0 eric      (1000) users      (984)     4832 2023-01-17 13:23:40.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/segmentation.py
--rw-r--r--   0 eric      (1000) users      (984)     7538 2023-01-13 14:12:23.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/sequence.py
--rw-r--r--   0 eric      (1000) users      (984)    14093 2023-01-17 15:32:43.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/tracking.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/
--rw-r--r--   0 eric      (1000) users      (984)     1693 2022-01-25 19:46:56.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/annotation.py
--rw-r--r--   0 eric      (1000) users      (984)     9774 2023-02-08 13:59:20.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/axes.py
--rw-r--r--   0 eric      (1000) users      (984)     3564 2022-01-25 18:39:23.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/color.py
--rw-r--r--   0 eric      (1000) users      (984)     3104 2022-02-17 13:51:26.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/context.py
--rw-r--r--   0 eric      (1000) users      (984)    13212 2022-06-01 07:11:21.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/e_viewer_2d_t.py
--rw-r--r--   0 eric      (1000) users      (984)     1590 2022-01-25 18:11:16.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/event.py
--rw-r--r--   0 eric      (1000) users      (984)     3100 2022-05-31 12:20:28.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/figure.py
--rw-r--r--   0 eric      (1000) users      (984)    12951 2023-01-20 16:01:59.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/s_drawer_2d.py
--rw-r--r--   0 eric      (1000) users      (984)     7915 2023-01-18 14:30:43.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/s_viewer_2d.py
--rw-r--r--   0 eric      (1000) users      (984)     3060 2022-01-26 09:00:12.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/signatures.py
--rw-r--r--   0 eric      (1000) users      (984)     5295 2023-01-18 14:24:16.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/t_explorer_2d.py
--rw-r--r--   0 eric      (1000) users      (984)    11377 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/t_viewer_2d.py
--rw-r--r--   0 eric      (1000) users      (984)     3190 2023-01-10 16:09:45.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/track.py
--rw-r--r--   0 eric      (1000) users      (984)     1645 2022-01-26 08:45:06.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/widget.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/
--rw-r--r--   0 eric      (1000) users      (984)     1675 2021-11-25 09:11:46.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/dev.py
--rw-r--r--   0 eric      (1000) users      (984)     4191 2023-02-10 15:18:51.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/plot.py
--rw-r--r--   0 eric      (1000) users      (984)     4074 2022-01-25 09:33:16.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/progress.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/standard/
--rw-r--r--   0 eric      (1000) users      (984)     2899 2023-01-13 14:44:24.000000 cell-tracking-bc-2023.6/cell_tracking_BC/standard/issue.py
--rw-r--r--   0 eric      (1000) users      (984)     1632 2021-12-16 15:05:53.000000 cell-tracking-bc-2023.6/cell_tracking_BC/standard/number.py
--rw-r--r--   0 eric      (1000) users      (984)     1791 2023-02-11 18:22:01.000000 cell-tracking-bc-2023.6/cell_tracking_BC/standard/path.py
--rw-r--r--   0 eric      (1000) users      (984)     2450 2023-02-08 13:56:27.000000 cell-tracking-bc-2023.6/cell_tracking_BC/standard/uid.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/task/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/channel/
--rw-r--r--   0 eric      (1000) users      (984)     1690 2023-02-10 14:28:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/channel/base.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/feature/
--rw-r--r--   0 eric      (1000) users      (984)     2433 2023-02-10 14:12:05.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/feature/base.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/matching/
--rw-r--r--   0 eric      (1000) users      (984)     6346 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/matching/pattern.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/processing/
--rw-r--r--   0 eric      (1000) users      (984)     1664 2023-02-10 11:25:18.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/processing/base.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/registration/
--rw-r--r--   0 eric      (1000) users      (984)     4710 2023-02-10 11:32:54.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/registration/rigid.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/segmentation/
--rw-r--r--   0 eric      (1000) users      (984)    20183 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/segmentation/frame.py
--rw-r--r--   0 eric      (1000) users      (984)     5269 2023-02-10 14:19:32.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/segmentation/sequence.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/tracking/
--rw-r--r--   0 eric      (1000) users      (984)     6615 2023-01-13 15:07:41.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/tracking/base.py
--rw-r--r--   0 eric      (1000) users      (984)     1647 2022-05-13 07:50:37.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/tracking/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     2399 2022-06-28 12:49:37.000000 cell-tracking-bc-2023.6/cell_tracking_BC/track_finder.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/type/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/type/acquisition/
--rw-r--r--   0 eric      (1000) users      (984)     2006 2023-01-20 09:44:08.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/acquisition/frame.py
--rw-r--r--   0 eric      (1000) users      (984)    12594 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/acquisition/sequence.py
--rw-r--r--   0 eric      (1000) users      (984)     2076 2023-02-13 09:18:21.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/analysis.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/
--rw-r--r--   0 eric      (1000) users      (984)     7392 2023-01-20 15:29:49.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/base.py
--rw-r--r--   0 eric      (1000) users      (984)     6955 2023-01-20 15:39:59.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/cell.py
--rw-r--r--   0 eric      (1000) users      (984)     1632 2023-01-10 16:10:01.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/cytoplasm.py
--rw-r--r--   0 eric      (1000) users      (984)     1630 2023-01-10 16:10:01.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/nucleus.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/type/segmentation/
--rw-r--r--   0 eric      (1000) users      (984)     7207 2023-01-20 15:57:41.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/segmentation/frame.py
--rw-r--r--   0 eric      (1000) users      (984)    12053 2023-02-10 14:24:32.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/segmentation/sequence.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/multiple/
--rw-r--r--   0 eric      (1000) users      (984)    14508 2023-06-21 08:59:52.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/multiple/structured.py
--rw-r--r--   0 eric      (1000) users      (984)     2777 2023-01-17 12:16:47.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/multiple/unstructured.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/
--rw-r--r--   0 eric      (1000) users      (984)    16776 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/forking.py
--rw-r--r--   0 eric      (1000) users      (984)    23416 2023-06-21 13:14:27.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/structured.py
--rw-r--r--   0 eric      (1000) users      (984)    10343 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/thread.py
--rw-r--r--   0 eric      (1000) users      (984)     5380 2023-01-17 13:16:57.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/unstructured.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     3114 2023-06-21 15:04:36.000000 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     4407 2023-06-21 15:04:36.000000 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-06-21 15:04:36.000000 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       66 2023-06-21 15:04:36.000000 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) users      (984)      149 2023-06-21 15:04:36.000000 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       17 2023-06-21 15:04:36.000000 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-01-13 17:58:27.000000 cell-tracking-bc-2023.6/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5694 2023-06-21 15:02:38.000000 cell-tracking-bc-2023.6/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.093272 cell-tracking-bc-2023.7/
+-rw-r--r--   0 eric      (1000) users      (984)       61 2023-06-21 15:02:20.000000 cell-tracking-bc-2023.7/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     3114 2023-06-30 08:19:48.093272 cell-tracking-bc-2023.7/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      636 2021-02-02 12:30:22.000000 cell-tracking-bc-2023.7/README-COPYRIGHT.txt
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 cell-tracking-bc-2023.7/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     2286 2022-02-03 09:12:09.000000 cell-tracking-bc-2023.7/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.069939 cell-tracking-bc-2023.7/cell_tracking_BC/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.069939 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.069939 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/channel/
+-rw-r--r--   0 eric      (1000) users      (984)     1969 2023-02-13 12:56:29.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/channel/ratio.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.066606 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.069939 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/geometrical/
+-rw-r--r--   0 eric      (1000) users      (984)        0 2023-02-15 15:28:16.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/geometrical/dummy.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.069939 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/radiometric/
+-rw-r--r--   0 eric      (1000) users      (984)     2574 2023-02-10 13:45:02.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/radiometric/entropy.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.069939 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/set/
+-rw-r--r--   0 eric      (1000) users      (984)     2532 2023-02-10 15:24:31.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/set/numpy_.py
+-rw-r--r--   0 eric      (1000) users      (984)     4169 2023-02-10 15:24:31.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/set/skimage_.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.069939 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/temporal/
+-rw-r--r--   0 eric      (1000) users      (984)     2140 2023-02-10 15:02:24.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/temporal/shift.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.069939 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/matching/
+-rw-r--r--   0 eric      (1000) users      (984)     1985 2021-09-08 16:51:38.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/matching/jaccard.py
+-rw-r--r--   0 eric      (1000) users      (984)     3209 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/parser.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.073272 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/processing/
+-rw-r--r--   0 eric      (1000) users      (984)     3866 2023-02-10 13:53:35.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/processing/background.py
+-rw-r--r--   0 eric      (1000) users      (984)     1976 2023-02-10 13:53:54.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/processing/contrast.py
+-rw-r--r--   0 eric      (1000) users      (984)     2503 2023-02-10 13:54:29.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/processing/geometry.py
+-rw-r--r--   0 eric      (1000) users      (984)     2991 2023-02-10 13:55:52.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/processing/registration.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.073272 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/segmentation/
+-rw-r--r--   0 eric      (1000) users      (984)     4782 2023-06-12 11:59:41.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/segmentation/tf_network.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.073272 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/tracking/
+-rw-r--r--   0 eric      (1000) users      (984)     5631 2023-02-10 13:58:46.000000 cell-tracking-bc-2023.7/cell_tracking_BC/catalog/tracking/gmb_tracker.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.066606 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.073272 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/
+-rw-r--r--   0 eric      (1000) users      (984)    10676 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/event.py
+-rw-r--r--   0 eric      (1000) users      (984)     7795 2023-06-30 08:12:49.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/feature.py
+-rw-r--r--   0 eric      (1000) users      (984)     4916 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/path.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.073272 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/table/
+-rw-r--r--   0 eric      (1000) users      (984)     3244 2023-06-29 07:23:16.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/table/cell.py
+-rw-r--r--   0 eric      (1000) users      (984)     3480 2023-02-08 13:56:27.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/table/chart.py
+-rw-r--r--   0 eric      (1000) users      (984)     2388 2023-02-08 13:57:24.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/table/column.py
+-rw-r--r--   0 eric      (1000) users      (984)     2208 2023-02-11 18:31:12.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/table/sheet.py
+-rw-r--r--   0 eric      (1000) users      (984)     5734 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/track.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.076606 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/
+-rw-r--r--   0 eric      (1000) users      (984)     7863 2023-01-24 09:27:19.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/annotations.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.066606 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.076606 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/
+-rw-r--r--   0 eric      (1000) users      (984)     2754 2022-02-17 13:49:51.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/context.py
+-rw-r--r--   0 eric      (1000) users      (984)     9151 2023-01-18 14:25:10.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_2.py
+-rw-r--r--   0 eric      (1000) users      (984)     7982 2022-07-09 12:00:34.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_3.py
+-rw-r--r--   0 eric      (1000) users      (984)     8450 2023-02-17 09:42:06.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_any.py
+-rw-r--r--   0 eric      (1000) users      (984)     6053 2022-05-31 12:24:19.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/event.py
+-rw-r--r--   0 eric      (1000) users      (984)     2798 2021-11-10 10:18:31.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/style.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.079939 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/vedo/
+-rw-r--r--   0 eric      (1000) users      (984)     1891 2022-02-01 15:12:55.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/vedo/context.py
+-rw-r--r--   0 eric      (1000) users      (984)     8915 2022-02-01 15:14:31.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/vedo/d_3.py
+-rw-r--r--   0 eric      (1000) users      (984)     5376 2022-02-23 16:34:49.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/vedo/d_any.py
+-rw-r--r--   0 eric      (1000) users      (984)     1873 2022-02-01 15:24:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/vedo/missing.py
+-rw-r--r--   0 eric      (1000) users      (984)     3207 2022-02-01 15:15:32.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/vedo/style.py
+-rw-r--r--   0 eric      (1000) users      (984)    14278 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/event.py
+-rw-r--r--   0 eric      (1000) users      (984)     3736 2023-01-11 13:41:46.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/feature.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.079939 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/generic/
+-rw-r--r--   0 eric      (1000) users      (984)     4751 2023-01-18 14:26:08.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/generic/d_2.py
+-rw-r--r--   0 eric      (1000) users      (984)     4918 2023-01-11 13:38:38.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/generic/d_3.py
+-rw-r--r--   0 eric      (1000) users      (984)     2642 2023-01-20 16:01:30.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/generic/d_any.py
+-rw-r--r--   0 eric      (1000) users      (984)     4832 2023-01-17 13:23:40.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/segmentation.py
+-rw-r--r--   0 eric      (1000) users      (984)     7538 2023-01-13 14:12:23.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/sequence.py
+-rw-r--r--   0 eric      (1000) users      (984)    14093 2023-01-17 15:32:43.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/tracking.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.083272 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/
+-rw-r--r--   0 eric      (1000) users      (984)     1693 2022-01-25 19:46:56.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/annotation.py
+-rw-r--r--   0 eric      (1000) users      (984)     9774 2023-02-08 13:59:20.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/axes.py
+-rw-r--r--   0 eric      (1000) users      (984)     3564 2022-01-25 18:39:23.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/color.py
+-rw-r--r--   0 eric      (1000) users      (984)     3104 2022-02-17 13:51:26.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/context.py
+-rw-r--r--   0 eric      (1000) users      (984)    13212 2022-06-01 07:11:21.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/e_viewer_2d_t.py
+-rw-r--r--   0 eric      (1000) users      (984)     1590 2022-01-25 18:11:16.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/event.py
+-rw-r--r--   0 eric      (1000) users      (984)     3100 2022-05-31 12:20:28.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/figure.py
+-rw-r--r--   0 eric      (1000) users      (984)    12951 2023-01-20 16:01:59.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/s_drawer_2d.py
+-rw-r--r--   0 eric      (1000) users      (984)     7915 2023-01-18 14:30:43.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/s_viewer_2d.py
+-rw-r--r--   0 eric      (1000) users      (984)     3060 2022-01-26 09:00:12.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/signatures.py
+-rw-r--r--   0 eric      (1000) users      (984)     5295 2023-01-18 14:24:16.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/t_explorer_2d.py
+-rw-r--r--   0 eric      (1000) users      (984)    11377 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/t_viewer_2d.py
+-rw-r--r--   0 eric      (1000) users      (984)     3190 2023-01-10 16:09:45.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/track.py
+-rw-r--r--   0 eric      (1000) users      (984)     1645 2022-01-26 08:45:06.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/widget.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.083272 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/text/
+-rw-r--r--   0 eric      (1000) users      (984)     1675 2021-11-25 09:11:46.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/text/dev.py
+-rw-r--r--   0 eric      (1000) users      (984)     4191 2023-02-10 15:18:51.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/text/plot.py
+-rw-r--r--   0 eric      (1000) users      (984)     4074 2022-01-25 09:33:16.000000 cell-tracking-bc-2023.7/cell_tracking_BC/in_out/text/progress.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.086606 cell-tracking-bc-2023.7/cell_tracking_BC/standard/
+-rw-r--r--   0 eric      (1000) users      (984)     2899 2023-01-13 14:44:24.000000 cell-tracking-bc-2023.7/cell_tracking_BC/standard/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)     1632 2021-12-16 15:05:53.000000 cell-tracking-bc-2023.7/cell_tracking_BC/standard/number.py
+-rw-r--r--   0 eric      (1000) users      (984)     1791 2023-02-11 18:22:01.000000 cell-tracking-bc-2023.7/cell_tracking_BC/standard/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     2450 2023-02-08 13:56:27.000000 cell-tracking-bc-2023.7/cell_tracking_BC/standard/uid.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.066606 cell-tracking-bc-2023.7/cell_tracking_BC/task/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.086606 cell-tracking-bc-2023.7/cell_tracking_BC/task/channel/
+-rw-r--r--   0 eric      (1000) users      (984)     1690 2023-02-10 14:28:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/task/channel/base.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.086606 cell-tracking-bc-2023.7/cell_tracking_BC/task/feature/
+-rw-r--r--   0 eric      (1000) users      (984)     2433 2023-02-10 14:12:05.000000 cell-tracking-bc-2023.7/cell_tracking_BC/task/feature/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     2728 2023-06-30 08:14:58.000000 cell-tracking-bc-2023.7/cell_tracking_BC/task/feature/load_from_json.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.086606 cell-tracking-bc-2023.7/cell_tracking_BC/task/matching/
+-rw-r--r--   0 eric      (1000) users      (984)     6346 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/task/matching/pattern.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.086606 cell-tracking-bc-2023.7/cell_tracking_BC/task/processing/
+-rw-r--r--   0 eric      (1000) users      (984)     1664 2023-02-10 11:25:18.000000 cell-tracking-bc-2023.7/cell_tracking_BC/task/processing/base.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.086606 cell-tracking-bc-2023.7/cell_tracking_BC/task/registration/
+-rw-r--r--   0 eric      (1000) users      (984)     4710 2023-02-10 11:32:54.000000 cell-tracking-bc-2023.7/cell_tracking_BC/task/registration/rigid.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.086606 cell-tracking-bc-2023.7/cell_tracking_BC/task/segmentation/
+-rw-r--r--   0 eric      (1000) users      (984)    20183 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/task/segmentation/frame.py
+-rw-r--r--   0 eric      (1000) users      (984)     5269 2023-02-10 14:19:32.000000 cell-tracking-bc-2023.7/cell_tracking_BC/task/segmentation/sequence.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.086606 cell-tracking-bc-2023.7/cell_tracking_BC/task/tracking/
+-rw-r--r--   0 eric      (1000) users      (984)     6615 2023-01-13 15:07:41.000000 cell-tracking-bc-2023.7/cell_tracking_BC/task/tracking/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     1647 2022-05-13 07:50:37.000000 cell-tracking-bc-2023.7/cell_tracking_BC/task/tracking/constant.py
+-rw-r--r--   0 eric      (1000) users      (984)     2399 2022-06-28 12:49:37.000000 cell-tracking-bc-2023.7/cell_tracking_BC/track_finder.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.086606 cell-tracking-bc-2023.7/cell_tracking_BC/type/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.089939 cell-tracking-bc-2023.7/cell_tracking_BC/type/acquisition/
+-rw-r--r--   0 eric      (1000) users      (984)     2006 2023-01-20 09:44:08.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/acquisition/frame.py
+-rw-r--r--   0 eric      (1000) users      (984)    12594 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/acquisition/sequence.py
+-rw-r--r--   0 eric      (1000) users      (984)     2076 2023-02-13 09:18:21.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/analysis.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.089939 cell-tracking-bc-2023.7/cell_tracking_BC/type/compartment/
+-rw-r--r--   0 eric      (1000) users      (984)     7392 2023-01-20 15:29:49.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/compartment/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     6955 2023-01-20 15:39:59.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/compartment/cell.py
+-rw-r--r--   0 eric      (1000) users      (984)     1632 2023-01-10 16:10:01.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/compartment/cytoplasm.py
+-rw-r--r--   0 eric      (1000) users      (984)     1630 2023-01-10 16:10:01.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/compartment/nucleus.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.089939 cell-tracking-bc-2023.7/cell_tracking_BC/type/segmentation/
+-rw-r--r--   0 eric      (1000) users      (984)     7207 2023-01-20 15:57:41.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/segmentation/frame.py
+-rw-r--r--   0 eric      (1000) users      (984)    12053 2023-02-10 14:24:32.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/segmentation/sequence.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.066606 cell-tracking-bc-2023.7/cell_tracking_BC/type/track/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.089939 cell-tracking-bc-2023.7/cell_tracking_BC/type/track/multiple/
+-rw-r--r--   0 eric      (1000) users      (984)    14508 2023-06-21 08:59:52.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/track/multiple/structured.py
+-rw-r--r--   0 eric      (1000) users      (984)     2777 2023-01-17 12:16:47.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/track/multiple/unstructured.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.093272 cell-tracking-bc-2023.7/cell_tracking_BC/type/track/single/
+-rw-r--r--   0 eric      (1000) users      (984)    16776 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/track/single/forking.py
+-rw-r--r--   0 eric      (1000) users      (984)    23416 2023-06-21 13:14:27.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/track/single/structured.py
+-rw-r--r--   0 eric      (1000) users      (984)    10343 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/track/single/thread.py
+-rw-r--r--   0 eric      (1000) users      (984)     5380 2023-01-17 13:16:57.000000 cell-tracking-bc-2023.7/cell_tracking_BC/type/track/single/unstructured.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-30 08:19:48.093272 cell-tracking-bc-2023.7/cell_tracking_bc.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     3114 2023-06-30 08:19:48.000000 cell-tracking-bc-2023.7/cell_tracking_bc.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     4455 2023-06-30 08:19:48.000000 cell-tracking-bc-2023.7/cell_tracking_bc.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-06-30 08:19:48.000000 cell-tracking-bc-2023.7/cell_tracking_bc.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       66 2023-06-30 08:19:48.000000 cell-tracking-bc-2023.7/cell_tracking_bc.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) users      (984)      156 2023-06-30 08:19:48.000000 cell-tracking-bc-2023.7/cell_tracking_bc.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       17 2023-06-30 08:19:48.000000 cell-tracking-bc-2023.7/cell_tracking_bc.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-01-13 17:58:27.000000 cell-tracking-bc-2023.7/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-06-30 08:19:48.093272 cell-tracking-bc-2023.7/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5716 2023-06-30 08:17:54.000000 cell-tracking-bc-2023.7/setup.py
```

### Comparing `cell-tracking-bc-2023.6/PKG-INFO` & `cell-tracking-bc-2023.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cell-tracking-bc
-Version: 2023.6
+Version: 2023.7
 Summary: Base Classes for Cell Tracking in Microscopy
 Home-page: https://gitlab.inria.fr/edebreuv/cell-tracking-bc
 Author: Eric Debreuve
 Author-email: eric.debreuve@univ-cotedazur.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://gitlab.inria.fr/edebreuv/cell-tracking-bc
 Project-URL: Source, https://gitlab.inria.fr/edebreuv/cell-tracking-bc
```

### Comparing `cell-tracking-bc-2023.6/README-COPYRIGHT.txt` & `cell-tracking-bc-2023.7/README-COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/README-LICENCE-utf8.txt` & `cell-tracking-bc-2023.7/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/README.rst` & `cell-tracking-bc-2023.7/README.rst`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/channel/ratio.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/channel/ratio.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/radiometric/entropy.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/radiometric/entropy.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/set/numpy_.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/set/numpy_.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/set/skimage_.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/set/skimage_.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/temporal/shift.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/feature/temporal/shift.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/matching/jaccard.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/matching/jaccard.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/parser.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/parser.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/background.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/processing/background.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/contrast.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/processing/contrast.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/geometry.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/processing/geometry.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/registration.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/processing/registration.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/segmentation/tf_network.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/segmentation/tf_network.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/tracking/gmb_tracker.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/catalog/tracking/gmb_tracker.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/event.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/event.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/feature.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/feature.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,30 +25,32 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+import gzip
 import numbers as nmbr
 import tempfile as temp
 from pathlib import Path as path_t
-from typing import IO, Optional, Union
+from typing import IO, Any, Optional, Sequence, Union
 
+import json_any as jsny
 import xlsxwriter as xlsx
+from logger_36 import LOGGER
 from xlsxwriter.format import Format as xlsx_format_t
 from xlsxwriter.workbook import Workbook as workbook_t
 
 from cell_tracking_BC.in_out.file.table.cell import SetStateBasedCellFormat
 from cell_tracking_BC.in_out.file.table.chart import AddChart_Mainly
 from cell_tracking_BC.in_out.file.table.sheet import (
     SheetNameFromLongName,
     SortAndWriteCSVLines,
 )
-from logger_36 import LOGGER
 from cell_tracking_BC.type.analysis import analysis_t
 from cell_tracking_BC.type.compartment.base import compartment_id_t, compartment_t
 from cell_tracking_BC.type.track.multiple.structured import tracks_t
 
 
 def SaveCompartmentsFeaturesToXLSX(
     base_path: Union[str, path_t],
@@ -76,14 +78,16 @@
         pruned_format = workbook.add_format({"bg_color": "gray"})
         division_format = workbook.add_format({"bg_color": "blue"})
         death_format = workbook.add_format({"bg_color": "red"})
 
         csv_path = path.with_suffix(".csv")
         csv_accessor = open(csv_path, mode="w")
 
+        feature_book = {}
+
         tracks = analysis.tracks
         if (tracks is None) or (tracks.__len__() == 0):
             LOGGER.warning("Sequence with no valid tracks.")
         else:
             one_compartment = (
                 analysis.segmentations[0].cells[0].compartments[compartment_id]
             )
@@ -92,72 +96,89 @@
             for feature in one_compartment.available_features:
                 _SaveFeature(
                     compartment_id,
                     feature,
                     tracks,
                     workbook,
                     csv_accessor,
+                    feature_book,
                     pruned_format,
                     division_format,
                     death_format,
                 )
 
+        jsoned = jsny.JsonStringOf(feature_book)
+        compressed = gzip.compress(jsoned.encode())
+        json_path = path.with_suffix(".json")
+        with open(json_path, mode="wb") as json_accessor:
+            json_accessor.write(compressed)
+
         workbook.close()
         csv_accessor.close()
 
 
 def _SaveFeature(
     compartment_id: compartment_id_t,
     feature: str,
     tracks: tracks_t,
     workbook: workbook_t,
     csv_accessor: IO,
+    feature_book: dict[(str, str), Sequence[Any]],
     pruned_format: Optional[xlsx_format_t],
     division_format: Optional[xlsx_format_t],
     death_format: Optional[xlsx_format_t],
     /,
 ) -> None:
     """"""
     sheet_name = SheetNameFromLongName(feature)
     worksheet = workbook.add_worksheet(sheet_name)
     csv_accessor.write(f"--- Feature {feature}\n")
 
     per_row_limits = {}
     csv_lines = []
+    feature_is_number = False
     for track in tracks.all_structured_iterator:
         root_time_point = track.topologic_root_time_point
         for path, label in track.LabeledThreadIterator(topologic_mode=True):
             row = label - 1
 
             if feature not in path[0].features:
                 message = f'Feature "{feature}" missing'
                 worksheet.write_string(row, 0, message)
                 csv_lines.append(f"{label}, {message}")
                 continue
 
-            evolution = []
+            raw_evolution = []
             for cell in path:
                 compartment = cell.compartments[compartment_id]
                 if isinstance(compartment, compartment_t):
-                    evolution.append(compartment.features[feature])
+                    raw_evolution.append(compartment.features[feature])
                 else:
-                    evolution.append(
+                    raw_evolution.append(
                         tuple(_cpt.features[feature] for _cpt in compartment)
                     )
-            if not isinstance(evolution[0], nmbr.Number):
-                message = f'Feature of type "{type(evolution[0]).__name__}" unhandled'
-                worksheet.write_string(0, 0, message)
-                csv_accessor.write(message + "\n")
-                return
+            feature_is_number = isinstance(raw_evolution[0], nmbr.Number)
+            evolution_as_str_list = list(map(_AsStrWithoutNewlines, raw_evolution))
+            if isinstance(raw_evolution[0], (nmbr.Number, str)):
+                evolution = raw_evolution
+            else:
+                evolution = evolution_as_str_list
 
             if root_time_point > 0:
                 worksheet.write_row(row, 0, root_time_point * ("x",))
-            worksheet.write_row(row, root_time_point, evolution)
+            if feature_is_number:
+                worksheet.write_row(row, root_time_point, evolution)
+            else:
+                for time_point, value in enumerate(evolution, start=root_time_point):
+                    worksheet.write_string(row, time_point, value)
             csv_lines.append(
-                f"{label}, " + root_time_point * "," + ", ".join(map(str, evolution))
+                f"{label}, " + root_time_point * "," + ", ".join(evolution_as_str_list)
+            )
+            feature_book[(feature, label)] = root_time_point * ("x",) + tuple(
+                raw_evolution
             )
 
             SetStateBasedCellFormat(
                 worksheet,
                 row,
                 root_time_point,
                 path,
@@ -168,18 +189,27 @@
             )
 
             per_row_limits[row + 1] = (
                 root_time_point,
                 root_time_point + evolution.__len__() - 1,
             )
 
-    AddChart_Mainly(
-        tracks,
-        per_row_limits,
-        workbook,
-        sheet_name,
-        worksheet,
-        pruned_format,
-        division_format,
-        death_format,
-    )
+    worksheet.autofit()
+
+    if feature_is_number:
+        AddChart_Mainly(
+            tracks,
+            per_row_limits,
+            workbook,
+            sheet_name,
+            worksheet,
+            pruned_format,
+            division_format,
+            death_format,
+        )
     SortAndWriteCSVLines(csv_lines, csv_accessor)
+
+
+def _AsStrWithoutNewlines(element: Any, /) -> str:
+    """"""
+    output = str(element)
+    return output.replace("\n", " ")
```

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/path.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/path.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/cell.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/table/cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from typing import Optional, Sequence
+import numbers as nmbr
 
 from xlsxwriter.format import Format as xlsx_format_t
 from xlsxwriter.worksheet import Worksheet as worksheet_t
 
 from cell_tracking_BC.type.compartment.cell import cell_t, state_e
 
 
@@ -57,15 +58,18 @@
         elif cell.state is state_e.dead:
             cell_format = death_format
         else:
             cell_format = None
 
         if cell_format is not None:
             value = values[time_point - root_time_point]
-            worksheet.write_number(row, time_point, value, cell_format)
+            if isinstance(value, nmbr.Number):
+                worksheet.write_number(row, time_point, value, cell_format)
+            else:
+                worksheet.write_string(row, time_point, value, cell_format)
 
 
 def AddCellStateLegend(
     worksheet: worksheet_t,
     row: int,
     pruned_format: Optional[xlsx_format_t],
     division_format: Optional[xlsx_format_t],
```

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/chart.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/table/chart.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/column.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/table/column.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/sheet.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/table/sheet.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/track.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/file/track.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/annotations.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/annotations.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/context.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/context.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_2.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_2.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_3.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_3.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_any.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_any.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/event.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/event.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/style.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/matplotlib/style.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/context.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/vedo/context.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/d_3.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/vedo/d_3.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/d_any.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/vedo/d_any.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/missing.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/vedo/missing.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/style.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/dbe/vedo/style.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/event.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/event.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/feature.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/feature.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/d_2.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/generic/d_2.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/d_3.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/generic/d_3.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/d_any.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/generic/d_any.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/segmentation.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/segmentation.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/sequence.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/sequence.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/tracking.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/tracking.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/annotation.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/annotation.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/axes.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/axes.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/color.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/color.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/context.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/context.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/e_viewer_2d_t.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/e_viewer_2d_t.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/event.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/event.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/figure.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/figure.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/s_drawer_2d.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/s_drawer_2d.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/s_viewer_2d.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/s_viewer_2d.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/signatures.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/signatures.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/t_explorer_2d.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/t_explorer_2d.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/t_viewer_2d.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/t_viewer_2d.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/track.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/track.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/widget.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/graphics/type/widget.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/dev.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/text/dev.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/plot.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/text/plot.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/progress.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/in_out/text/progress.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/standard/issue.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/standard/issue.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/standard/number.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/standard/number.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/standard/path.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/standard/path.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/standard/uid.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/standard/uid.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/task/channel/base.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/task/channel/base.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/task/feature/base.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/task/feature/base.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/task/matching/pattern.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/task/matching/pattern.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/task/processing/base.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/task/processing/base.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/task/registration/rigid.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/task/registration/rigid.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/task/segmentation/frame.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/task/segmentation/frame.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/task/segmentation/sequence.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/task/segmentation/sequence.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/task/tracking/base.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/task/tracking/base.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/task/tracking/constant.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/task/tracking/constant.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/track_finder.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/track_finder.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/acquisition/frame.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/acquisition/frame.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/acquisition/sequence.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/acquisition/sequence.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/analysis.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/analysis.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/base.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/compartment/base.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/cell.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/compartment/cell.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/cytoplasm.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/compartment/cytoplasm.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/nucleus.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/compartment/nucleus.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/segmentation/frame.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/segmentation/frame.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/segmentation/sequence.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/segmentation/sequence.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/track/multiple/structured.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/track/multiple/structured.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/track/multiple/unstructured.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/track/multiple/unstructured.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/forking.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/track/single/forking.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/structured.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/track/single/structured.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/thread.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/track/single/thread.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/unstructured.py` & `cell-tracking-bc-2023.7/cell_tracking_BC/type/track/single/unstructured.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/PKG-INFO` & `cell-tracking-bc-2023.7/cell_tracking_bc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cell-tracking-bc
-Version: 2023.6
+Version: 2023.7
 Summary: Base Classes for Cell Tracking in Microscopy
 Home-page: https://gitlab.inria.fr/edebreuv/cell-tracking-bc
 Author: Eric Debreuve
 Author-email: eric.debreuve@univ-cotedazur.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://gitlab.inria.fr/edebreuv/cell-tracking-bc
 Project-URL: Source, https://gitlab.inria.fr/edebreuv/cell-tracking-bc
```

### Comparing `cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/SOURCES.txt` & `cell-tracking-bc-2023.7/cell_tracking_bc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 cell_tracking_BC/in_out/text/progress.py
 cell_tracking_BC/standard/issue.py
 cell_tracking_BC/standard/number.py
 cell_tracking_BC/standard/path.py
 cell_tracking_BC/standard/uid.py
 cell_tracking_BC/task/channel/base.py
 cell_tracking_BC/task/feature/base.py
+cell_tracking_BC/task/feature/load_from_json.py
 cell_tracking_BC/task/matching/pattern.py
 cell_tracking_BC/task/processing/base.py
 cell_tracking_BC/task/registration/rigid.py
 cell_tracking_BC/task/segmentation/frame.py
 cell_tracking_BC/task/segmentation/sequence.py
 cell_tracking_BC/task/tracking/base.py
 cell_tracking_BC/task/tracking/constant.py
```

### Comparing `cell-tracking-bc-2023.6/setup.py` & `cell-tracking-bc-2023.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 AUTHOR = "Eric Debreuve"
 E_MAIL = "eric.debreuve@univ-cotedazur.fr"
 
 PYPI_NAME = "cell-tracking-bc"
 DESCRIPTION = "Base Classes for Cell Tracking in Microscopy"
-version = "2023.6"
+version = "2023.7"
 PY_VERSION = "3.8"
 
 REPOSITORY_NAME = "cell-tracking-bc"
 REPOSITORY_USER = "edebreuv"
 REPOSITORY_SITE = "gitlab.inria.fr"
 DOCUMENTATION_SITE = f"{REPOSITORY_USER}.gitlabpages.inria.fr"
 
@@ -150,14 +150,15 @@
             "imageio",
             "json-any",
             "logger-36",
             "matplotlib",
             "mrc",
             "networkx",
             "numpy",
+            "pandas",
             "pca-b-stream",
             "Pillow",
             "plotext",
             "rich",
             "scikit-image",
             "scipy",
             "tensorflow",
```

