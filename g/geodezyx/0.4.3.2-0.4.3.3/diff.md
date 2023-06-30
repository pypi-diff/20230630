# Comparing `tmp/geodezyx-0.4.3.2.tar.gz` & `tmp/geodezyx-0.4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodezyx-0.4.3.2.tar", last modified: Wed Mar  8 14:29:58 2023, max compression
+gzip compressed data, was "geodezyx-0.4.3.3.tar", last modified: Fri Jun 30 12:25:06 2023, max compression
```

## Comparing `geodezyx-0.4.3.2.tar` & `geodezyx-0.4.3.3.tar`

### file list

```diff
@@ -1,109 +1,114 @@
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.886820 geodezyx-0.4.3.2/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    35150 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/LICENSE
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1576 2023-03-08 14:29:58.886820 geodezyx-0.4.3.2/PKG-INFO
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     4913 2023-03-08 14:26:29.000000 geodezyx-0.4.3.2/README.md
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.866820 geodezyx-0.4.3.2/geodezyx/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1963 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/__init__.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.866820 geodezyx-0.4.3.2/geodezyx/athmo/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       21 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/athmo/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30462 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/athmo/athmo.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.870820 geodezyx-0.4.3.2/geodezyx/conv/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      344 2023-01-26 12:02:06.000000 geodezyx-0.4.3.2/geodezyx/conv/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     8972 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/conv/conv_angle.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    23357 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/conv/conv_coords.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9551 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/conv/conv_geometric.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5908 2022-02-10 13:50:15.000000 geodezyx-0.4.3.2/geodezyx/conv/conv_interpolators.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3891 2023-01-25 19:44:46.000000 geodezyx-0.4.3.2/geodezyx/conv/conv_proj_lambert.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6574 2023-01-26 12:02:27.000000 geodezyx-0.4.3.2/geodezyx/conv/conv_proj_utm.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10244 2022-12-09 14:03:28.000000 geodezyx-0.4.3.2/geodezyx/conv/conv_rinex.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    12038 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/conv/conv_rotation_matrices.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79809 2023-03-07 12:22:40.000000 geodezyx-0.4.3.2/geodezyx/conv/conv_time.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.870820 geodezyx-0.4.3.2/geodezyx/externlib/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1354 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/externlib/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      763 2021-06-22 11:51:35.000000 geodezyx-0.4.3.2/geodezyx/externlib/externlib.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.874820 geodezyx-0.4.3.2/geodezyx/files_rw/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      517 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/files_rw/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    80903 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/files_rw/geo_files_converter_lib.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9417 2021-06-30 10:20:35.000000 geodezyx-0.4.3.2/geodezyx/files_rw/read_athmo.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     4812 2022-02-01 13:47:04.000000 geodezyx-0.4.3.2/geodezyx/files_rw/read_coords_misc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    71323 2023-01-27 17:32:16.000000 geodezyx-0.4.3.2/geodezyx/files_rw/read_coords_time_series.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    19068 2022-02-08 21:16:09.000000 geodezyx-0.4.3.2/geodezyx/files_rw/read_eop.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    28668 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/files_rw/read_geo_files_misc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    16650 2022-11-16 11:13:59.000000 geodezyx-0.4.3.2/geodezyx/files_rw/read_gnss_prods.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     8729 2022-02-08 21:17:46.000000 geodezyx-0.4.3.2/geodezyx/files_rw/read_igs_combi.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    18124 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/files_rw/read_logsheets.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13363 2023-02-01 11:15:49.000000 geodezyx-0.4.3.2/geodezyx/files_rw/read_rinex.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2825 2021-06-23 09:02:50.000000 geodezyx-0.4.3.2/geodezyx/files_rw/read_slr.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    37800 2022-09-12 16:41:56.000000 geodezyx-0.4.3.2/geodezyx/files_rw/write_geo_files.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.874820 geodezyx-0.4.3.2/geodezyx/geodyn/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      102 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/geodyn/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10146 2022-03-15 13:51:04.000000 geodezyx-0.4.3.2/geodezyx/geodyn/emsgfz_load_interp.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13599 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/geodyn/euler_pole_calc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    27538 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/geodyn/velo_field_map_plt.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5317 2022-03-15 10:23:38.000000 geodezyx-0.4.3.2/geodezyx/geodyn/volcano_mogi.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.874820 geodezyx-0.4.3.2/geodezyx/marine/
--rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)      109 2022-11-24 14:30:34.000000 geodezyx-0.4.3.2/geodezyx/marine/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2590 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/marine/marine.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10788 2022-11-28 10:57:15.000000 geodezyx-0.4.3.2/geodezyx/marine/oseanpres_lib.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.874820 geodezyx-0.4.3.2/geodezyx/megalib/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      153 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/megalib/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      139 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/megalib/genefun.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      295 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/megalib/geo_files_converter_lib.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      454 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/megalib/geoclass.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      334 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/megalib/geodetik.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      408 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/megalib/megalib.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      720 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/megalib/softs_runner.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.878820 geodezyx-0.4.3.2/geodezyx/operational/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      635 2023-02-22 10:37:05.000000 geodezyx-0.4.3.2/geodezyx/operational/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9477 2022-12-09 11:05:27.000000 geodezyx-0.4.3.2/geodezyx/operational/anubis_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7448 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/operational/cluster_gfz.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7021 2022-10-11 11:04:29.000000 geodezyx-0.4.3.2/geodezyx/operational/download_cddis.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6743 2023-02-02 14:41:09.000000 geodezyx-0.4.3.2/geodezyx/operational/download_dropbox.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    12833 2023-01-24 10:26:13.000000 geodezyx-0.4.3.2/geodezyx/operational/download_find_files.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    32777 2023-01-25 19:45:17.000000 geodezyx-0.4.3.2/geodezyx/operational/download_prods.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17730 2022-12-09 14:27:21.000000 geodezyx-0.4.3.2/geodezyx/operational/download_rinex.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    11251 2023-01-24 10:26:13.000000 geodezyx-0.4.3.2/geodezyx/operational/download_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79440 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/operational/gins_runner.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    21977 2023-03-06 20:12:42.000000 geodezyx-0.4.3.2/geodezyx/operational/groops_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    15766 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/operational/hector_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7930 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/operational/midas_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    26045 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/operational/rinex_lister_plotter.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    31582 2023-02-24 13:19:32.000000 geodezyx-0.4.3.2/geodezyx/operational/rinex_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7075 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/operational/rtklib_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9160 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/operational/track_frontend.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.882820 geodezyx-0.4.3.2/geodezyx/reffram/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      107 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/reffram/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    43581 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/reffram/geometry.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    56868 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/reffram/gnss_products.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7243 2022-02-08 21:09:25.000000 geodezyx-0.4.3.2/geodezyx/reffram/kepler_gzyx.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3879 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/reffram/quaternions.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.882820 geodezyx-0.4.3.2/geodezyx/stats/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       50 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/stats/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30960 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/stats/least_squares.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    43975 2023-01-19 10:55:29.000000 geodezyx-0.4.3.2/geodezyx/stats/stats.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.882820 geodezyx-0.4.3.2/geodezyx/time_series/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       97 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/time_series/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    47866 2023-02-20 16:49:42.000000 geodezyx-0.4.3.2/geodezyx/time_series/ts_class.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    44482 2023-01-30 16:49:12.000000 geodezyx-0.4.3.2/geodezyx/time_series/ts_fcts.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.882820 geodezyx-0.4.3.2/geodezyx/toolbox_meta/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       96 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/toolbox_meta/__init__.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.882820 geodezyx-0.4.3.2/geodezyx/utils/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      242 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/utils/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2026 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/utils/dict_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13518 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/utils/list_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3637 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/geodezyx/utils/pandas_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7260 2023-01-30 16:46:53.000000 geodezyx-0.4.3.2/geodezyx/utils/plot_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17839 2023-01-24 10:26:13.000000 geodezyx-0.4.3.2/geodezyx/utils/shell_like.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    24787 2023-01-30 15:02:21.000000 geodezyx-0.4.3.2/geodezyx/utils/utils_core.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.866820 geodezyx-0.4.3.2/geodezyx.egg-info/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1576 2023-03-08 14:29:58.000000 geodezyx-0.4.3.2/geodezyx.egg-info/PKG-INFO
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2878 2023-03-08 14:29:58.000000 geodezyx-0.4.3.2/geodezyx.egg-info/SOURCES.txt
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)        1 2023-03-08 14:29:58.000000 geodezyx-0.4.3.2/geodezyx.egg-info/dependency_links.txt
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      168 2023-03-08 14:29:58.000000 geodezyx-0.4.3.2/geodezyx.egg-info/requires.txt
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       14 2023-03-08 14:29:58.000000 geodezyx-0.4.3.2/geodezyx.egg-info/top_level.txt
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-03-08 14:29:58.886820 geodezyx-0.4.3.2/misc/
--rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       98 2022-12-02 23:12:26.000000 geodezyx-0.4.3.2/misc/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1225 2021-06-22 11:51:35.000000 geodezyx-0.4.3.2/misc/import_generic.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3778 2023-01-16 18:09:24.000000 geodezyx-0.4.3.2/misc/refactoring.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       38 2023-03-08 14:29:58.886820 geodezyx-0.4.3.2/setup.cfg
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10174 2023-03-08 14:29:09.000000 geodezyx-0.4.3.2/setup.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.727347 geodezyx-0.4.3.3/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    35150 2023-01-16 18:09:24.000000 geodezyx-0.4.3.3/LICENSE
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1576 2023-06-30 12:25:06.727347 geodezyx-0.4.3.3/PKG-INFO
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     4990 2023-06-30 12:19:55.000000 geodezyx-0.4.3.3/README.md
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.695347 geodezyx-0.4.3.3/geodezyx/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2152 2023-05-31 13:51:35.000000 geodezyx-0.4.3.3/geodezyx/__init__.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.695347 geodezyx-0.4.3.3/geodezyx/athmo/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       21 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/athmo/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30462 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/athmo/athmo.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.699347 geodezyx-0.4.3.3/geodezyx/conv/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      344 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/conv/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9008 2023-04-27 16:56:08.000000 geodezyx-0.4.3.3/geodezyx/conv/conv_angle.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    23357 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/conv/conv_coords.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9551 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/conv/conv_geometric.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5908 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/conv/conv_interpolators.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3891 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/conv/conv_proj_lambert.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6574 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/conv/conv_proj_utm.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10244 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/conv/conv_rinex.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    12038 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/conv/conv_rotation_matrices.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79808 2023-05-31 13:56:13.000000 geodezyx-0.4.3.3/geodezyx/conv/conv_time.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.699347 geodezyx-0.4.3.3/geodezyx/externlib/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1354 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/externlib/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      763 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/externlib/externlib.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.707347 geodezyx-0.4.3.3/geodezyx/files_rw/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      556 2023-04-23 11:48:52.000000 geodezyx-0.4.3.3/geodezyx/files_rw/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    80903 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/files_rw/geo_files_converter_lib.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9417 2023-04-07 15:57:22.000000 geodezyx-0.4.3.3/geodezyx/files_rw/read_athmo.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     4812 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/files_rw/read_coords_misc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    77264 2023-06-09 15:48:46.000000 geodezyx-0.4.3.3/geodezyx/files_rw/read_coords_time_series.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    19068 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/files_rw/read_eop.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    28668 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/files_rw/read_geo_files_misc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    16650 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/files_rw/read_gnss_prods.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     8729 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/files_rw/read_igs_combi.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    18124 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/files_rw/read_logsheets.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14535 2023-04-23 18:42:34.000000 geodezyx-0.4.3.3/geodezyx/files_rw/read_rinex.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2825 2023-04-07 15:57:22.000000 geodezyx-0.4.3.3/geodezyx/files_rw/read_slr.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    37801 2023-05-31 13:56:43.000000 geodezyx-0.4.3.3/geodezyx/files_rw/write_geo_files.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6437 2023-06-06 10:47:42.000000 geodezyx-0.4.3.3/geodezyx/files_rw/write_rinex.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.707347 geodezyx-0.4.3.3/geodezyx/geodyn/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      102 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/geodyn/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10146 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/geodyn/emsgfz_load_interp.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13599 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/geodyn/euler_pole_calc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    27578 2023-06-30 12:19:55.000000 geodezyx-0.4.3.3/geodezyx/geodyn/velo_field_map_plt.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5317 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/geodyn/volcano_mogi.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.707347 geodezyx-0.4.3.3/geodezyx/logconfig/
+-rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       80 2023-04-07 18:12:57.000000 geodezyx-0.4.3.3/geodezyx/logconfig/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2009 2023-06-11 20:05:07.000000 geodezyx-0.4.3.3/geodezyx/logconfig/loggzyx.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.711347 geodezyx-0.4.3.3/geodezyx/marine/
+-rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)      109 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/marine/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2590 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/marine/marine.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10788 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/marine/oseanpres_lib.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.711347 geodezyx-0.4.3.3/geodezyx/megalib/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      153 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/megalib/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      139 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/megalib/genefun.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      295 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/megalib/geo_files_converter_lib.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      571 2023-05-12 13:59:17.000000 geodezyx-0.4.3.3/geodezyx/megalib/geoclass.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      334 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/megalib/geodetik.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      408 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/megalib/megalib.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      720 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/megalib/softs_runner.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.715347 geodezyx-0.4.3.3/geodezyx/operational/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      635 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/operational/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9590 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/operational/anubis_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7448 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/operational/cluster_gfz.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7021 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/operational/download_cddis.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6743 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/operational/download_dropbox.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    12881 2023-06-02 09:08:37.000000 geodezyx-0.4.3.3/geodezyx/operational/download_find_files.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    32777 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/operational/download_prods.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17730 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/operational/download_rinex.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    11251 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/operational/download_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79440 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/operational/gins_runner.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    21977 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/operational/groops_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    15766 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/operational/hector_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7930 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/operational/midas_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    26040 2023-06-02 08:02:32.000000 geodezyx-0.4.3.3/geodezyx/operational/rinex_lister_plotter.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    31955 2023-05-31 13:56:13.000000 geodezyx-0.4.3.3/geodezyx/operational/rinex_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7075 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/operational/rtklib_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9160 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/operational/track_frontend.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.719347 geodezyx-0.4.3.3/geodezyx/reffram/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      107 2023-04-07 15:57:22.000000 geodezyx-0.4.3.3/geodezyx/reffram/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    43633 2023-06-30 12:09:16.000000 geodezyx-0.4.3.3/geodezyx/reffram/geometry.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    56868 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/reffram/gnss_products.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7243 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/reffram/kepler_gzyx.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3879 2023-04-07 15:57:22.000000 geodezyx-0.4.3.3/geodezyx/reffram/quaternions.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.719347 geodezyx-0.4.3.3/geodezyx/stats/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       50 2023-04-07 15:57:22.000000 geodezyx-0.4.3.3/geodezyx/stats/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30960 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/stats/least_squares.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    43987 2023-06-22 13:52:44.000000 geodezyx-0.4.3.3/geodezyx/stats/stats.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.723347 geodezyx-0.4.3.3/geodezyx/time_series/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       97 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/time_series/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    48361 2023-06-23 09:38:51.000000 geodezyx-0.4.3.3/geodezyx/time_series/ts_class.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17296 2023-06-28 15:28:03.000000 geodezyx-0.4.3.3/geodezyx/time_series/ts_export.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    35307 2023-06-22 13:50:24.000000 geodezyx-0.4.3.3/geodezyx/time_series/ts_fcts.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.723347 geodezyx-0.4.3.3/geodezyx/toolbox_meta/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       96 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/toolbox_meta/__init__.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.723347 geodezyx-0.4.3.3/geodezyx/utils/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      242 2023-04-07 15:57:22.000000 geodezyx-0.4.3.3/geodezyx/utils/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2026 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/utils/dict_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13518 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/utils/list_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3637 2023-04-07 15:57:23.000000 geodezyx-0.4.3.3/geodezyx/utils/pandas_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7260 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/utils/plot_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17975 2023-04-07 16:22:38.000000 geodezyx-0.4.3.3/geodezyx/utils/shell_like.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    24926 2023-06-28 15:58:55.000000 geodezyx-0.4.3.3/geodezyx/utils/utils_core.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.695347 geodezyx-0.4.3.3/geodezyx.egg-info/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1576 2023-06-30 12:25:06.000000 geodezyx-0.4.3.3/geodezyx.egg-info/PKG-INFO
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3006 2023-06-30 12:25:06.000000 geodezyx-0.4.3.3/geodezyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)        1 2023-06-30 12:25:06.000000 geodezyx-0.4.3.3/geodezyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      177 2023-06-30 12:25:06.000000 geodezyx-0.4.3.3/geodezyx.egg-info/requires.txt
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       14 2023-06-30 12:25:06.000000 geodezyx-0.4.3.3/geodezyx.egg-info/top_level.txt
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:25:06.723347 geodezyx-0.4.3.3/misc/
+-rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       98 2022-12-02 23:12:26.000000 geodezyx-0.4.3.3/misc/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1225 2021-06-22 11:51:35.000000 geodezyx-0.4.3.3/misc/import_generic.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3778 2023-01-16 18:09:24.000000 geodezyx-0.4.3.3/misc/refactoring.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       38 2023-06-30 12:25:06.727347 geodezyx-0.4.3.3/setup.cfg
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10208 2023-06-30 12:22:58.000000 geodezyx-0.4.3.3/setup.py
```

### Comparing `geodezyx-0.4.3.2/LICENSE` & `geodezyx-0.4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/PKG-INFO` & `geodezyx-0.4.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodezyx
-Version: 0.4.3.2
+Version: 0.4.3.3
 Summary: The GeodeZYX toolbox aims to provide simple but useful functions for Geodesy and Geophysics.
 Home-page: https://github.com/GeodeZYX/geodezyx-toolbox
 Author: Pierre Sakic & Gustavo Mansur
 Author-email: pierre.sakic@gfz-potsdam.de
 Keywords: geodesy,geophysics,reference frames,gnss
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `geodezyx-0.4.3.2/README.md` & `geodezyx-0.4.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <img src="./geodezyx_toolbox_logo.png" width="300">
 
 # GeodeZYX Toolbox
 
-**Version 0.4.3.2 / 2023-03-08**, README Revision: 2023-03-08
+**Version 0.4.3.3 / 2023-06-30**, README Revision: 2023-06-30
 
 
 **Authors:** Pierre Sakic (IPGP, Paris, France), Gustavo Mansur, and Kitpracha "Na" Chaiyaporn
 (GFZ, Potsdam, Germany), with contributions from Valérie Ballu (CNRS/La Rochelle University, France)
 
 **Documentation:** [https://geodezyx.github.io/geodezyx-toolbox](https://geodezyx.github.io/geodezyx-toolbox/)
 
-**GitHub repository:** [https://github.com/GeodeZYX/geodezyx-toolbox](https://github.com/GeodeZYX/geodezyx-toolbox)
+**GitHub repository:** [https://github.com/GeodeZYX/geodezyx-toolbox](https://github.com/GeodeZYX/geodezyx-toolbox) 
 
 **PyPi project:** [https://pypi.org/project/geodezyx](https://pypi.org/project/geodezyx/)
 
 **Contact e-mail:** sakic@ipgp.fr
 
 **Citation:** Sakic, Pierre; Mansur, Gustavo; Chaiyaporn, Kitpracha; Ballu, Valérie (2019):
 *The geodeZYX toolbox: a versatile Python 3 toolbox for geodetic-oriented purposes*. 
@@ -23,15 +23,15 @@
 **Licence:** GNU GPL v3 (see below) 
 
 ## Introduction
 
 The purpose of the GeodeZYX toolbox (pronounced *geode-**zeecks***) is to provide all the functions which
 can be useful for Geodesy and Geophysics. 
 
-It includes low level functions, file management functions,
+It includes low-level functions, file management functions,
 time and space-coordinates conversion functions, 
 data (especially GNSS observations and orbits) retrieve functions, 
 plots and visual selection functions ...
 
 It is designed for Python 3 on a LINUX Ubuntu-like system.
 Also tested with Anaconda
 
@@ -64,14 +64,17 @@
 
 and install the Toolbox you downloaded with ``python setup.py install``
 
 Alternatively, you can also add the ``geodezyx`` folder in your ``PYTHONPATH`` (for experimented users)
 
 ## Changelog
 
+### v0.4.3.3, 2023-06-30
+  * a routine version update (bug corrections...)
+
 ### v0.4.3.2, 2023-03-08
   * 1000th commit on GitHub 🥳
   * GitHub repository is renamed for simplification 
     * `GeodeZYX-Toolbox_v4` becomes `geodezyx-toolbox` (lowercase and without version)
     * It must be transparent for your clones but updating them is recommended \
       https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository  
   * beta for GROOPS automatized run functions
```

### Comparing `geodezyx-0.4.3.2/geodezyx/__init__.py` & `geodezyx-0.4.3.3/geodezyx/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
 #### IMPORT EXTERNAL MODULES
 import bisect
 from collections import defaultdict
 from collections import Counter
 import copy
 import datetime as dt
 import fnmatch
@@ -37,20 +40,24 @@
 import tempfile
 from tempfile import mkstemp
 import tabulate
 import time
 import urllib
 import uuid
 
-#### IMPORT CONFIG FOR LOGGER
-log_file_path = os.path.join(path.dirname(path.abspath(__file__)),'logconfig','loggzyx.conf.py')
 
+#### IMPORT CONFIG FOR LOGGER
+log_file_path = os.path.join(path.dirname(path.abspath(__file__)),'logconfig','loggzyx.py')
+from . import logconfig
 if os.path.isfile(log_file_path):
     ##print("INFO:",log_file_path,"found")
-    logging.config.fileConfig(fname=log_file_path, disable_existing_loggers=False)
+    ###### old config file format
+    ###logging.config.fileConfig(fname=log_file_path, disable_existing_loggers=False)
+    ###### new dict
+    logging.config.dictConfig(logconfig.loggzyx.log_config_dict)
 else:
     print("ERR:logger config file",log_file_path,"is missing")
 
 
 #### IMPORT GEODEZYX INTERNAL SUBMODULES
 from . import externlib
 from . import megalib
```

### Comparing `geodezyx-0.4.3.2/geodezyx/athmo/athmo.py` & `geodezyx-0.4.3.3/geodezyx/athmo/athmo.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/conv/conv_angle.py` & `geodezyx-0.4.3.3/geodezyx/conv/conv_angle.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,17 @@
 
     Returns
     -------
     dd_float : float
         Decimal degree Angle
         
     """
-    return deg + minn * (1./60.) +  sec * (1./3600.)
+    sig = np.sign(deg)
+    
+    return deg + sig*minn * (1./60.) +  sig*sec * (1./3600.)
 
 
 def deg_dec2dms(deg_in,only_dm=False):
     """
     Angle conversion
     
     Convert :
```

### Comparing `geodezyx-0.4.3.2/geodezyx/conv/conv_coords.py` & `geodezyx-0.4.3.3/geodezyx/conv/conv_coords.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/conv/conv_geometric.py` & `geodezyx-0.4.3.3/geodezyx/conv/conv_geometric.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/conv/conv_interpolators.py` & `geodezyx-0.4.3.3/geodezyx/conv/conv_interpolators.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/conv/conv_proj_lambert.py` & `geodezyx-0.4.3.3/geodezyx/conv/conv_proj_lambert.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/conv/conv_proj_utm.py` & `geodezyx-0.4.3.3/geodezyx/conv/conv_proj_utm.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/conv/conv_rinex.py` & `geodezyx-0.4.3.3/geodezyx/conv/conv_rinex.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/conv/conv_rotation_matrices.py` & `geodezyx-0.4.3.3/geodezyx/conv/conv_rotation_matrices.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/conv/conv_time.py` & `geodezyx-0.4.3.3/geodezyx/conv/conv_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1399,15 +1399,15 @@
         doy  = int(date_str[4:7])        
         hh   = int(date_str[7:9])        
         mm   = int(date_str[9:11])       
         dt_out = doy2dt(yyyy,doy) + dt.timedelta(seconds=hh*3600 + mm*60)
         return dt_out 
 
     ##### LONG rinex name -- GFZ's GODC internal name
-    if re.search(conv_rinex.rinex_regex_long_name_gfz_godc(),rinexname): 
+    elif re.search(conv_rinex.rinex_regex_long_name_gfz_godc(),rinexname): 
         date_str = rinexname.split("_")[5]
         time_str = rinexname.split("_")[6]
         yyyy = int(date_str[:4])
         mo   = int(date_str[4:6])     
         dd   = int(date_str[6:8])     
         
         hh   = int(time_str[0:2])        
@@ -1435,15 +1435,15 @@
         else:
             h = 0
             
         return dt.datetime(year,1,1) + dt.timedelta(days = doy - 1 , seconds = h * 3600)
 
     else:
         log.error('RINEX name is not well formated: %s',rinexname)
-        raise Exception
+        return None 
     
 
 def sp3name2dt(sp3path):
     """
     Time representation conversion
     
     Orbit SP3 Name (legacy/new naming convention)  => Python's Datetime
```

### Comparing `geodezyx-0.4.3.2/geodezyx/externlib/__init__.py` & `geodezyx-0.4.3.3/geodezyx/externlib/__init__.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/externlib/externlib.py` & `geodezyx-0.4.3.3/geodezyx/externlib/externlib.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/__init__.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,7 +9,8 @@
 from .read_geo_files_misc     import *
 from .read_gnss_prods         import *
 from .read_logsheets          import *
 from .read_igs_combi          import *
 from .read_rinex              import *
 from .read_slr                import *
 from .write_geo_files         import *
+from .write_rinex             import *
```

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/geo_files_converter_lib.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/geo_files_converter_lib.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/read_athmo.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/read_athmo.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/read_coords_misc.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/read_coords_misc.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/read_coords_time_series.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/read_coords_time_series.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
 import dateutil
 import glob
 import numpy as np
 import os 
+from io import StringIO
 import pandas as pd
 import scipy
 import re
 import gzip
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import files_rw
@@ -54,15 +55,15 @@
     elif re.compile('Kinematic Processing').search(firstline):
         tsout = read_gipsy_apps(filein)
 
     elif re.compile('tdp.llh').search(filein):
         tsout = read_gipsy_bosser(filein)
 
     elif re.compile('STA').search(firstline) or re.compile('tdp').search(filein) or re.compile('TRPAZ').search(firstline):
-        tsout = read_tdp(filein)
+        tsout = read_gipsy_tdp(filein)
 
     elif re.compile('YY  MM DD HR MIN').search(firstline):
         tsout = read_track(filein)
 
     elif re.compile('Latitude').search(firstline):
         tsout = read_sonardyne_posi(filein)
 
@@ -183,17 +184,17 @@
  #      | |  __ \| |        / / ____|_   _|  __ \ / ____\ \   / / |  ____(_) |          
  #      | | |__) | |       / / |  __  | | | |__) | (___  \ \_/ /  | |__   _| | ___  ___ 
  #  _   | |  ___/| |      / /| | |_ | | | |  ___/ \___ \  \   /   |  __| | | |/ _ \/ __|
  # | |__| | |    | |____ / / | |__| |_| |_| |     ____) |  | |    | |    | | |  __/\__ \
  #  \____/|_|    |______/_/   \_____|_____|_|    |_____/   |_|    |_|    |_|_|\___||___/
                                                                                       
 
-def read_tdp(filein):
+def read_gipsy_tdp(filein):
     """
-    Read GIPSY TDP (Time Dependent Parameter) File
+    Read legacy Gipsy TDP (Time Dependent Parameter) File
 
     Parameters
     ----------
     filein : str
         input file path.
 
     Returns
@@ -239,20 +240,14 @@
             Tz = 333
 
     tsout.meta_set(filein,stat=STAT)
 
     return tsout
 
 
-def read_gipsy_tdp(filein):
-    """
-    Wrapper of read_tdp 
-    """
-    # pour un nom plus explicite (et qui evitera de recoder la fct ...)
-    return read_tdp(filein)
 
 
 def read_gipsy_tdp_list(filelistin):
     """
     Read Several GIPSY TDP (Time Dependent Parameter) Files
     
 
@@ -269,17 +264,270 @@
 
     tslist = []
     for fil in filelistin:
         ts = read_gipsy_tdp(fil)
         tslist.append(ts)
 
     tsout = time_series.merge_ts(tslist)
+    
+    stat = list(set([ts.stat for ts in tslist]))[0]
+    
+    tsout.meta_set("",stat)
+
+    return tsout
+
+
+def read_gipsyx_tdp(filein):
+    """
+    Read GipsyX TDP (Time Dependent Parameter) File
+
+    Parameters
+    ----------
+    filein : str
+        input file path.
+
+    Returns
+    -------
+    tsout : TimeSeries Object
+        output TimeSerie.
+    """
+
+
+    X,Y,Z = np.nan,np.nan,np.nan
+    Tx , Ty , Tz, T = np.nan,np.nan,np.nan,np.nan
+    sX,sY,sZ = np.nan,np.nan,np.nan
+
+    tsout = time_series.TimeSeriePoint()
+
+    for line in open(filein):
+
+        fields = line.split()
+        attribs = fields[-1].split(".") 
+
+        if attribs[1] == 'Station' and attribs[-1] == 'Z':
+            Tz = conv.tgipsy2dt(fields[0])
+            Z  = (float(fields[2]))
+            sZ = (float(fields[3]))
+
+        if attribs[1] == 'Station' and attribs[-1] == 'Y':
+            Ty = conv.tgipsy2dt(fields[0])
+            Y  = (float(fields[2]))
+            sY = (float(fields[3]))
+
+        if attribs[1] == 'Station' and attribs[-1] == 'X':
+            Tx = conv.tgipsy2dt(fields[0])
+            X  = (float(fields[2]))
+            sX = (float(fields[3]))
+            STAT = attribs[2]
+
+        if  Tx == Ty == Tz :
+            T = Tx
+            point = time_series.Point(X,Y,Z,T,'XYZ',sX,sY,sZ)
+            tsout.add_point(point)
+
+            Tx = np.nan
+            Ty = np.nan
+            Tz = np.nan
+
+    tsout.meta_set(filein,stat=STAT)
+
+    return tsout
+
+def read_gipsyx_tdp_list(filelistin):
+    """
+    Read Several GIPSYX TDP (Time Dependent Parameter) Files
+    
+
+    Parameters
+    ----------
+    filelistin : list
+        input file paths in a list.
+
+    Returns
+    -------
+    tsout : TimeSeries Object
+        output TimeSerie.    
+    """
+
+    tslist = []
+    for fil in filelistin:
+        ts = read_gipsyx_tdp(fil)
+        tslist.append(ts)
+
+    tsout = time_series.merge_ts(tslist)
+    
+    stat = list(set([ts.stat for ts in tslist]))[0]
+    
+    tsout.meta_set("",stat)
+
+    return tsout
+
+
+def read_gipsy_gdcov(filein):
+    
+    X,Y,Z = np.nan,np.nan,np.nan
+    Tx , Ty , Tz, T = np.nan,np.nan,np.nan,np.nan
+    sX,sY,sZ = np.nan,np.nan,np.nan
+
+    tsout = time_series.TimeSeriePoint()
+
+    F = open(filein)
+    L = F.readlines()
+    
+    ### parameters search
+    param = int(L[0].split()[0])
+    
+    Lparam = L[1:param+1]
+    Lcovar = L[param+2:]
+    
+    for line in Lparam:
+        fields = line.split()
+        attribs = fields[1].split(".") 
+        
+        if attribs[1] == 'STA' and attribs[-1] == 'Z':
+            Tz = conv.tgipsy2dt(fields[2])
+            Z  = (float(fields[3]))
+            sZ = (float(fields[4]))
+
+        if attribs[1] == 'STA' and attribs[-1] == 'Y':
+            Ty = conv.tgipsy2dt(fields[2])
+            Y  = (float(fields[3]))
+            sY = (float(fields[4]))
+
+        if attribs[1] == 'STA' and attribs[-1] == 'X':
+            Tx = conv.tgipsy2dt(fields[2])
+            X  = (float(fields[3]))
+            sX = (float(fields[4]))
+            STAT = attribs[0]
+
+        if  Tx == Ty == Tz :
+            T = Tx
+            point = time_series.Point(X,Y,Z,T,'XYZ',sX,sY,sZ)
+            tsout.add_point(point)
+
+            Tx = np.nan
+            Ty = np.nan
+            Tz = np.nan
+        
+    tsout.meta_set(filein,stat=STAT)
+
+    return tsout
+
+        
+
+def read_gipsy_gdcov_list(filelistin):
+    tslist = []
+    for fil in filelistin:
+        ts = read_gipsy_gdcov(fil)
+        tslist.append(ts)
+
+    tsout = time_series.merge_ts(tslist)
+    
+    stat = list(set([ts.stat for ts in tslist]))[0]
+    
+    tsout.meta_set("",stat)
 
     return tsout
 
+    
+pp = "/home/psakicki/GFZ_WORK/IPGP_WORK/OVS/GNSS_OVS/2305_compar_gipsyx/2306_nf_orb_tests/230609b/HOUE/2001/2001-01-01.HOUE.gdcov_trans"
+ts = read_gipsy_gdcov(pp)
+
+def read_gipsyx_xfile(filein):
+    """
+    Read GIPSYX X file i.e. the transformation parameters and their 
+    residuals
+    
+
+    Parameters
+    ----------
+    filein : str
+        input file path.
+        Can handle gz compressed files
+        
+    Returns
+    -------
+    df_trans_out : DataFrame
+        Helmert transformation parameters and their sigmas.
+    df_resid_out : DataFrame
+        Coordinates residuals (not implemented yet).
+
+    """
+    
+    fname = os.path.basename(filein)
+    
+    date = conv.date_string_2_dt(fname[:11])
+    
+    if filein[-2:] in ("gz","GZ"):
+        F = gzip.open(filein, "r+")
+        lines = [e.decode('utf-8') for e in F]
+    else:
+        F = open(filein,"r+")
+        lines = F.readlines()
+    
+    df_trans_out = pd.DataFrame()
+    df_resid_out = pd.DataFrame()
+    
+    df_trans_out.loc[0,"epoch"] = date
+    
+    for l in lines:
+        #### get transform parameters
+        if re.search(' = ', l):
+            l2 = l.split()
+            label = l2[0]            
+            val = float(l2[2])
+            df_trans_out.loc[0,label] = val
+
+            if len(l2) > 3:
+                val_sigma = float(l2[4])
+                df_trans_out.loc[0,"s" + label] = val_sigma
+                
+                
+        #### get residual values
+        # l_resid = []
+        # if re.search('^ ( POS| RES)', l):
+        #     l_resid.append(l)
+            
+        # df_resid_out = pd.read_csv(StringIO("\n".join(l_resid[:-1])))
+        
+    return df_trans_out, df_resid_out
+    
+
+def read_gipsyx_xfile_list(filelistin):
+    """
+    Read several GIPSYX X files i.e. the transformation parameters and their 
+    residuals
+
+    Parameters
+    ----------
+    filelistin : list
+        input file paths in a list.
+        Can handle gz compressed files
+
+
+    Returns
+    -------
+    df_trans_out : DataFrame
+        Helmert transformation parameters and their sigmas.
+    df_resid_out : DataFrame
+        Coordinates residuals (not implemented yet).
+
+    """
+    dflist = []
+    for fil in filelistin:
+        df_trans_mono,df_resid_mono = read_gipsyx_xfile(fil)
+        dflist.append(df_trans_mono)
+    
+    df_trans_out =pd.concat(dflist)
+    df_trans_out.reset_index(drop=True,inplace=True)
+    df_resid_out = pd.DataFrame()
+    
+    return df_trans_out, df_resid_out
+
+
 def read_gipsy_bosser(filein):
     """
     Read P. Bosser (@ENSTA Brest) File (GIPSY)
 
     Parameters
     ----------
     filein : str
```

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/read_eop.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/read_eop.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/read_geo_files_misc.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/read_geo_files_misc.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/read_gnss_prods.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/read_gnss_prods.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/read_igs_combi.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/read_igs_combi.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/read_logsheets.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/read_logsheets.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/read_rinex.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/read_rinex.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 Copyright (C) 2019 Pierre Sakic et al. (GFZ, pierre.sakic@gfz-postdam.de)
 GitHub repository :
 https://github.com/GeodeZYX/GeodeZYX-Toolbox_v4
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
+import datetime as dt
 import numpy as np
 import pandas as pd
 from io import StringIO
 import re
 import os
 import pathlib
 from tqdm import tqdm
@@ -88,15 +89,15 @@
     Lines_obs = [l[:60] for l in Lines_obs]
     
     ObsAllList_raw = " ".join(Lines_obs).split()
     ObsAllList = ObsAllList_raw[1:]
     ObsAllList = sorted([e for sublist in [(e,e+"_LLI",e+"_SSI") for e in ObsAllList] for e in sublist])
     
     nobs = int(ObsAllList_raw[0])
-    nlines_for_obs = int(np.ceil(nobs/5)) ## 5 is the man num of obs in the RIENX specs
+    nlines_for_obs = int(np.ceil(nobs/5)) ## 5 is the max num of obs in the RIENX specs
     
     
     DFall_stk = []
     
     #### reading the epochs    
     for iepoc in tqdm(range(len(EPOCHS)),desc="Reading " + filename):
         epoch = EPOCHS[iepoc,0]
@@ -111,14 +112,15 @@
         Lines_epoc = LINES[iline_start:iline_end]
         
         ### get the satellites for this epoch block
         epoc,nsat,lineconcat,Sats_split,iline_sats_end = _sats_find(Lines_epoc)
         
         ### for each sat, merge the breaked lines
         Lines_obs = Lines_epoc[iline_sats_end+1:iline_end]
+        Lines_obs = [e.replace("\r","") for e in Lines_obs] # not 100% sure of this
         Lines_obs = [e.replace("\n","") for e in Lines_obs]
         Lines_obs_merg = [Lines_obs[nlines_for_obs*n:nlines_for_obs*n+nlines_for_obs] for n in range(nsat)]
         Lines_obs_merg = ["".join(e) for e in Lines_obs_merg]
         
         ## read the epoch block using pandas' fixed width reader 
         B = StringIO("\n".join(Lines_obs_merg))
         columns_width = nobs*[14,1,1]
@@ -192,15 +194,14 @@
     #LINES_obs = LINES[i_end_header:]
     
     #### get the systems and observations
     Lines_sys = [l for l in LINES_header if 'SYS / # / OBS TYPES' in l]
     ## clean SYS / # / OBS TYPES
     Lines_sys = [l[:60] for l in Lines_sys]
     
-    
     ## manage the 2 lines systems
     for il,l in enumerate(Lines_sys):
         if l[0] == " ":
             Lines_sys[il-1] = Lines_sys[il-1] + l
             Lines_sys.remove(l)
     
     #### store system and observables in a dictionnary
@@ -231,20 +232,24 @@
         iline_start = EPOCHS[iepoc,1] + 1
         if iepoc == len(EPOCHS)-1:
             iline_end = None
         else:
             iline_end = EPOCHS[iepoc+1,1]
         
         Lines_epoc = LINES[iline_start:iline_end]
-        
+        ###  Remove CR (Carriage Return) and LF (Line Feed) 
+        Lines_epoc = [l.replace('\r', '') for l in Lines_epoc]
+        Lines_epoc = [l.replace('\n', '') for l in Lines_epoc]
+                
         ## read the epoch block using pandas' fixed width reader 
-        B = StringIO("".join(Lines_epoc))
+        B = StringIO("\n".join(Lines_epoc))
+        
         columns_width = [3] + nobs_max*[14,1,1]
         DFepoch = pd.read_fwf(B,header=None,widths=columns_width)      
-        
+               
         DFepoch_ok_stk = []
         #### assign the correct observable names for each system
         for sys in dict_sys_use.keys():
             #DFepoch_sys = DFepoch[DFepoch[0].str[0] == sys]
             #                   get the sats of the system sys  ||  get the meaningful columns
             DFepoch_sys_clean = DFepoch[DFepoch[0].str[0] == sys].iloc[:,:len(dict_sys_use[sys])]
             DFepoch_sys_clean.columns = dict_sys_use[sys]
@@ -309,35 +314,64 @@
         A RINEX DataFrame.
 
     Returns
     -------
     dict_sys_obs : dict
         A dictionnary with GNSS system as key (G,R,E...).
         And the observalbes for each system as values
+        
+    Note
+    ----
+    
+    Use dict_sys_obs_clean_LLI_SSI if your want to remove the LLI & SSI values
     """
     
     dict_sys_obs = dict()
 
     for sys in DFrnx_in["sys"].unique():
         DFsys = DFrnx_in[DFrnx_in["sys"] == sys]
         DFsys_mini = DFrnx_clean_LLI_SSI(DFsys)
         
         ObsSys0 = (DFsys_mini.isna().sum() == len(DFsys)).apply(np.logical_not)
         ObsSys = ObsSys0.index[ObsSys0][3:] ### strating from 3 to clean epoch sys prn
         
         #init_tup = ("epoch","sys","prn") 
-        init_tup = []
-        ObsSys_full = [init_tup] + [(e,e+"_LLI",e+"_SSI") for e in ObsSys] 
+        #init_tup = []
+        #ObsSys_full = [init_tup] + [(e,e+"_LLI",e+"_SSI") for e in ObsSys] 
+        ObsSys_full = [(e,e+"_LLI",e+"_SSI") for e in ObsSys] 
         ObsSys_full = [e for sublist in ObsSys_full for e in sublist]
                     
         dict_sys_obs[sys] = ObsSys_full
         
     return dict_sys_obs
     
+def dict_sys_obs_clean_LLI_SSI(dict_sys_obs_in):
+    """
+    Clean a `dict_sys_obs` (generated by `observables_dict_per_sys`)
+    of its LLI and SSI values
+
+    Parameters
+    ----------
+    dict_sys_obs_in : dict
+        A dictionnary with GNSS system as key (G,R,E...).
+        And the observalbes for each system as values.
 
+    Returns
+    -------
+    dict_sys_obs_out : dict
+        Same dictionnary cleanned of its LLI and SSI values.
+
+    """
+    dict_sys_obs_out = dict()
+    
+    for sys,obs in dict_sys_obs_in.items():
+        obs_clean = [e for e in obs if not "LLI" in e and not "SSI" in e]
+        dict_sys_obs_out[sys] = obs_clean
+        
+    return dict_sys_obs_out
 
 ############ INTERNAL FUNCTIONS
 
 
 def _sats_find(Lines_inp):
     """
     For RINEX2 only
@@ -413,8 +447,8 @@
             out_stk.append(out)
         else:
             try:
                 out_stk.append(float(out))
             except:
                 out_stk.append(np.nan)
     
-    return out_stk
+    return out_stk
```

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/read_slr.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/read_slr.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/files_rw/write_geo_files.py` & `geodezyx-0.4.3.3/geodezyx/files_rw/write_geo_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import re
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 from geodezyx import files_rw
 from geodezyx import reffram
-from geodezyx.megalib.megalib import *   # Import the legacy modules names
+#from geodezyx.megalib.megalib import *   # Import the legacy modules names
 
 #### Import the logger
 import logging
 log = logging.getLogger(__name__)
 
 
 #### Import star style
```

### Comparing `geodezyx-0.4.3.2/geodezyx/geodyn/emsgfz_load_interp.py` & `geodezyx-0.4.3.3/geodezyx/geodyn/emsgfz_load_interp.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/geodyn/euler_pole_calc.py` & `geodezyx-0.4.3.3/geodezyx/geodyn/euler_pole_calc.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/geodyn/velo_field_map_plt.py` & `geodezyx-0.4.3.3/geodezyx/geodyn/velo_field_map_plt.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 #### External modules
 import math
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 
 try:
+    import netCDF4
     from mpl_toolkits.basemap import Basemap
 except:
     pass
 
 from matplotlib.patches import Ellipse
 
 #### geodeZYX modules
@@ -52,43 +53,42 @@
 
 
 # ------------------
 # Plot land mask
 # ------------------
 
 def landmask(M, color='0.8'):
-
    # Make a constant colormap, default = grey
    constmap = matplotlib.colors.ListedColormap([color])
 
    jmax, imax = M.shape
    # X and Y give the grid cell boundaries,
    # one more than number of grid cells + 1
    # half integers (grid cell centers are integers)
    X = -0.5 + np.arange(imax+1)
    Y = -0.5 + np.arange(jmax+1)
 
    # Draw the mask by pcolor
-   M = ma.masked_where(M > 0, M)
-   pl.pcolor(X, Y, M, shading='flat', cmap=constmap)
+   M = np.ma.masked_where(M > 0, M)
+   plt.pcolor(X, Y, M, shading='flat', cmap=constmap)
 
 # -------------
 # Colormap
 # -------------
 
 # Colormap, smlgn. med Rob Hetland
 
 def LevelColormap(levels, cmap=None):
     """
     Make a colormap based on an increasing sequence of levels
     """
     
     # Start with an existing colormap
     if cmap == None:
-        cmap = pl.get_cmap()
+        cmap = plt.get_cmap()
 
     # Spread the colours maximally
     nlev = len(levels)
     S = np.arange(nlev, dtype='float')/(nlev-1)
     A = cmap(S)
 
     # Normalize the levels to interval [0,1]
@@ -125,28 +125,24 @@
              shorten_oversized_arrows=True,
              exclude_points_out_of_range = True,
              adjust_text=False,
              pixels_hires_backgrnd=2000,
              draw_borders=True,
              full_return=False,
              draw_latlon_lines=True):
-    """
-    """
-    
     
     nstation = len(station_etude)
     fig,ax=plt.subplots(figsize=(7,8))  
      
     if incvn_ITRF is None:
         incvn_ITRF = np.zeros(len(station_etude))
     if incve_ITRF is None:
         incve_ITRF = np.zeros(len(station_etude))
     if incplot_vertical_ITRF is None:
         incplot_vertical_ITRF = np.zeros(len(station_etude))
-        
 
     if coarse_lines:
         resolution="l"
     else:
         resolution="h"
     m= Basemap(projection='merc', llcrnrlat=latm,urcrnrlat = latM, 
                llcrnrlon = lonm, urcrnrlon = lonM, lat_ts=-20, 
@@ -166,26 +162,26 @@
         m.fillcontinents(color='#EFEFDB', lake_color='#97B6E1',zorder=1)
         m.shadedrelief()
     
     if not plot_GEBCO:
         color1='black'
     else:
         color1='white'
-        levels = [-8000,-7000,-6000,-5500,-5000,-4500,-4000]#Niveaux pour l'echelle de couleur
-        gebconc = Dataset(path+'GEBCO\\GRIDONE_2D.nc')    
+        levels = [-8000,-7000,-6000,-5500,-5000,-4500,-4000] #Niveaux pour l'echelle de couleur
+        gebconc = netCDF4.Dataset(path+'GEBCO\\GRIDONE_2D.nc')    
         #Vecteur longitudes/latitudes
         long_ini = gebconc.variables['lon'][:]
         lats_ini = gebconc.variables['lat'][:]
         (lats_area,longs_area,gebco_area) = area(long_ini,lats_ini,gebconc,latm,latM,lonm,lonM,'0-180') #lat bas,lat haut, long
         (longs,lats,gebco) = split_grid(longs_area,lats_area,gebco_area,2)
         (longs_gr,lats_gr)=np.meshgrid(longs,lats)  
         fond = m.pcolormesh(longs_gr,lats_gr,
                             gebco,shading='flat',
                             cmap=LevelColormap(list(np.asarray(levels)*(1)),
-                                               cmap=cm.deep_r),
+                                               cmap='deep_r'), # cmap=cm.deep_r
                             latlon=True) #ice,deep
         cbar=m.colorbar(location='top',pad=0.5)
         cbar.set_label('Depth [m] ', rotation=0)
         
     if draw_latlon_lines:
         m.drawparallels(np.arange(latm,latM,1.),fontsize=10,color=color1,labels=[True,False,False,False],linewidth=0.25, dashes=[10000,1]) #de -180 a 360 par pas de 5° ;   
         m.drawmeridians(np.arange(lonm,lonM,1.),fontsize=10,color=color1,labels=[False,False,False,True],linewidth=0.25, dashes=[10000,1]) # Haut / G/D/BAS 
@@ -236,20 +232,21 @@
                 log.info("INFO : exclude point because out of range")
                 continue
         
             
             x_end_arrow_ok = all_posx_proj[i]+np.multiply(ve_ITRF[i],scale_arrow)
             y_end_arrow_ok = all_posy_proj[i]+np.multiply(vn_ITRF[i],scale_arrow)
             
-            ax.annotate(s='', 
+            ax.annotate(text='', 
                          xy=(x_end_arrow_ok,
                              y_end_arrow_ok), 
                          xytext=(all_posx_proj[i], all_posy_proj[i]) , 
                          arrowprops=arrow_prop_dict,
                          annotation_clip=True) #xy point arrivee de la fleche, xytext l'origine de la fleche
+            
             a=math.atan((all_posx_proj[i]+np.multiply(ve_ITRF[i],scale_arrow)-all_posy_proj[i])/(all_posy_proj[i]+np.multiply(ve_ITRF[i],scale_arrow)-all_posy_proj[i])) # l'angle d'orientation de l'ellipsoide, avec 0 au nord et +90 a l'ouest
                 
             e = Ellipse(xy=(x_end_arrow_ok,
                             y_end_arrow_ok), 
                             width=np.multiply(2,incve_ITRF[i])*scale_ellipse,
                             height=np.multiply(2,incvn_ITRF[i])*scale_ellipse,
                             angle=a) #multiplication par 2 pour obtenir la largeur et la hauteur de l'ellipse 
@@ -321,15 +318,15 @@
                 arrow_prop_dict_V = arrow_prop_dict_V_up_short
             elif plot_vertical_ITRF[i]<=0 and not shortened_arrow:
                 arrow_prop_dict_V = arrow_prop_dict_V_down
             elif plot_vertical_ITRF[i]<=0 and shortened_arrow:
                 arrow_prop_dict_V = arrow_prop_dict_V_down_short
                                 
             ### PLOT      
-            ax.annotate(s='',
+            ax.annotate(text='',
                       xy=(x_end_arrow_ok , y_end_arrow_ok),
                       xytext=(all_posx_proj[i], all_posy_proj[i]) , 
                       arrowprops=arrow_prop_dict_V,
                       annotation_clip=False)
             #xy point arrivee de la fleche, xytext l'origine de la fleche
                 
             ### STATION NAME
@@ -374,15 +371,15 @@
     ### origine de la fleche de legende        
     xl,yl = utils.axis_data_coords_sys_transform(ax,legend_position_x,
                                               legend_position_y + 0.02,
                                               inverse=False)
     ### fin de la fleche de legende                
     xe,ye = xl+np.multiply(legend_arrow_length_metric,scale_arrow),yl
     
-    plt.annotate(s='', xy=(xe,ye), xytext=(xl, yl) , 
+    plt.annotate(text='', xy=(xe,ye), xytext=(xl, yl) , 
                  arrowprops=arrow_prop_dict) #xy point arrivee de la fleche, xytext l'origine de la fleche
 
     props = dict(boxstyle='round', facecolor='black', alpha=0)
     ax.text(legend_position_x, legend_position_y + 0.035, 
             'Velocity : ' + legend_arrow_length_label,
             transform=ax.transAxes, fontsize=11,color='black',
         verticalalignment='bottom', bbox=props)# place a text box in upper left in axes coords
```

### Comparing `geodezyx-0.4.3.2/geodezyx/geodyn/volcano_mogi.py` & `geodezyx-0.4.3.3/geodezyx/geodyn/volcano_mogi.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/marine/marine.py` & `geodezyx-0.4.3.3/geodezyx/marine/marine.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/marine/oseanpres_lib.py` & `geodezyx-0.4.3.3/geodezyx/marine/oseanpres_lib.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/megalib/softs_runner.py` & `geodezyx-0.4.3.3/geodezyx/megalib/softs_runner.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/__init__.py` & `geodezyx-0.4.3.3/geodezyx/operational/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .anubis_frontend       import *
 from .cluster_gfz           import *
-from .gins_runner           import *
+# from .gins_runner         import *
 # from .gnss_downloader     import *
 from .download_cddis         import *
 from .download_dropbox       import *
 from .download_find_files    import *
 from .download_prods         import *
 from .download_rinex         import *
 from .download_utils         import *
```

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/anubis_frontend.py` & `geodezyx-0.4.3.3/geodezyx/operational/anubis_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,17 @@
                 sp3_path = sp3_list[0]    
             else:
                 sp3_path = ""
             
         ### start to modifiy the XML
         xmltree = et.parse(xml_config_generic)
     
+        if type(nav_path) is list: #hotfix 230406 ... must be investigated!
+            nav_path = nav_path[0]
+
         # set input files
         xmltree.find('.//rinexo').text = rnx_path
         xmltree.find('.//rinexn').text = nav_path
         xmltree.find('.//sp3').text    = sp3_path
     
         # set output files
         xmltree.find('.//xtr').text = out_xtr
@@ -246,8 +249,8 @@
             process1 = subprocess.run(command,
                                       capture_output=True,
                                       text=True,
                                       shell=True)
             
             time.sleep(2)
             
-    return XML_INP_LIST
+    return XML_INP_LIST
```

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/cluster_gfz.py` & `geodezyx-0.4.3.3/geodezyx/operational/cluster_gfz.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/download_cddis.py` & `geodezyx-0.4.3.3/geodezyx/operational/download_cddis.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/download_dropbox.py` & `geodezyx-0.4.3.3/geodezyx/operational/download_dropbox.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/download_find_files.py` & `geodezyx-0.4.3.3/geodezyx/operational/download_find_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,43 +10,44 @@
 functions for Geodesy and Geophysics under the GNU GPL v3 License
 Copyright (C) 2019 Pierre Sakic et al. (GFZ, pierre.sakic@gfz-postdam.de)
 GitHub repository :
 https://github.com/GeodeZYX/GeodeZYX-Toolbox_v4
 """
 
 ########## BEGIN IMPORT ##########
-#### External modules
+# External modules
 import datetime as dt
 # from ftplib import FTP
 import glob
 # import itertools
 # import multiprocessing as mp
 import os
-# import pandas as pd 
+# import pandas as pd
 import re
 # import shutil
 # import urllib
 # import ftplib
 
-#### geodeZYX modules
+# geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
-#### Import star style
+# Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
 
 
-#### Import the logger
+# Import the logger
 import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
+
 def rinex_finder(main_dir,
                  short_name=True,
                  long_name=True,
                  gfz_godc_name=True,
                  compressed=None,
                  specific_sites=[],
                  start_epoch=None,
@@ -75,122 +76,123 @@
         `end_epoch=dt.datetime(2021,12,31)`
         The default is None.
 
     Returns
     -------
     Files_rnx_lis : list
         Found RINEXs list.
-        
-        
+
+
     Notes
     -----
-    
+
     is very similar with geodetik.rinex_lister,  gins_runner.get_rinex_list,
     operational.multi_finder_rinex
-    
+
     But this one is the most recent and elaborated (July 2022),
     must be used in priority !!!
 
     """
-    
-    Files_raw_lis , _ = utils.walk_dir(main_dir)
-    
+
+    Files_raw_lis, _ = utils.walk_dir(main_dir)
+
     Files_rnx_lis = []
-    
+
     for f in Files_raw_lis:
         fbase = os.path.basename(f)
         regex_match = conv.rinex_regex_search_tester(fbase,
-                                       short_name=short_name,
-                                       long_name=long_name,
-                                       gfz_godc_name=gfz_godc_name,
-                                       compressed=compressed)
+                                                     short_name=short_name,
+                                                     long_name=long_name,
+                                                     gfz_godc_name=gfz_godc_name,
+                                                     compressed=compressed)
         if regex_match:
             Files_rnx_lis.append(f)
-                        
+
     # SECOND FILTERING IF specific_sites LIST IS DEFINED
     if len(specific_sites) > 0:
         Files_rnx_lis_tmp = []
         for site in specific_sites:
             for rnx in Files_rnx_lis:
                 rnx_bn = os.path.basename(rnx)
                 if site.lower() in rnx_bn or site.upper() in rnx_bn:
                     Files_rnx_lis_tmp.append(rnx)
         Files_rnx_lis = Files_rnx_lis_tmp
-        
+
     # THIRD FILTERING IF start or end epoch are defined
     if start_epoch or end_epoch:
         if not start_epoch:
-            start_epoch = dt.datetime(1980,1,1)
+            start_epoch = dt.datetime(1980, 1, 1)
         if not end_epoch:
-            end_epoch = dt.datetime(2099,1,1)
+            end_epoch = dt.datetime(2099, 1, 1)
         Files_rnx_lis_tmp = []
         Dates_rnx = [conv.rinexname2dt(rnx) for rnx in Files_rnx_lis]
-        
-        for rnx,date in zip(Files_rnx_lis,Dates_rnx):
+
+        for rnx, date in zip(Files_rnx_lis, Dates_rnx):
             if start_epoch <= date and date <= end_epoch:
                 Files_rnx_lis_tmp.append(rnx)
         Files_rnx_lis = Files_rnx_lis_tmp
 
-    log.info(str(len(Files_rnx_lis)) +  ' RINEXs found')
+    Files_rnx_lis = list(sorted(Files_rnx_lis))
+    log.info(str(len(Files_rnx_lis)) + ' RINEXs found')
 
     return Files_rnx_lis
 
 
 def multi_finder_rinex(main_dir,
-                       rinex_types=('o','d','d.Z','d.z'),
-                       specific_stats = [] ):
+                       rinex_types=('o', 'd', 'd.Z', 'd.z'),
+                       specific_stats=[]):
     """
     from a main_dir, find all the rinexs in this folder and his subfolder
     (corresponding to the rinex_types)
     and return a list of the found rinexs
-    
+
     Designed for RINEX-2 / short names only
 
     is very similar with geodetik.rinex_lister,  gins_runner.get_rinex_list,
     operational.rinex_finder
-    
+
     operational.rinex_finder must be used in priority !!! (July 2022)
     """
-    
+
     log.warning("multi_finder_rinex depreciated, use rinex_finder instead!!")
-    
-    files_raw_lis , _ = utils.walk_dir(main_dir)
 
-    yylis = [str(e).zfill(2) for e in list(range(80,100)) + list(range(0,dt.datetime.now().year - 2000 + 1))]
+    files_raw_lis, _ = utils.walk_dir(main_dir)
+
+    yylis = [str(e).zfill(2) for e in list(range(80, 100)) +
+             list(range(0, dt.datetime.now().year - 2000 + 1))]
 
     rinex_lis = []
 
     for f in files_raw_lis:
         for rnxext in rinex_types:
             for yy in yylis:
                 if f.endswith(yy + rnxext):
                     rinex_lis.append(f)
 
-
     # CASE FOR specific_stats
     if len(specific_stats) > 0:
         rinex_lis2 = []
         for stat in specific_stats:
             for rnx in rinex_lis:
                 if stat in os.path.basename(rnx):
                     rinex_lis2.append(rnx)
         rinex_lis = rinex_lis2
 
-    log.info(str(len(rinex_lis)) +  ' RINEXs found')
+    log.info(str(len(rinex_lis)) + ' RINEXs found')
 
     return rinex_lis
 
 
-def find_IGS_products_files(parent_dir,File_type,ACs,date_start,date_end=None,
-                            recursive_search=True,severe=True,
+def find_IGS_products_files(parent_dir, File_type, ACs, date_start, date_end=None,
+                            recursive_search=True, severe=True,
                             compressed="incl",
-                            regex_old_naming = True,
-                            regex_new_naming = True,
-                            regex_igs_tfcc_naming = True,
-                            add_weekly_file = False):
+                            regex_old_naming=True,
+                            regex_new_naming=True,
+                            regex_igs_tfcc_naming=True,
+                            add_weekly_file=False):
     """
     Find all product files in a parent folder which correspond to file type(s),
     AC(s) and date(s)
 
     Parameters
     ----------
     parent_dir : str or list of str
@@ -216,162 +218,168 @@
         or a 2-tuple (wwww,d) e.g. (1990,0)
 
     date_end : None or dt.datetime or 2-tuple list of int
         end of the time period researched
         can be a datetime
         or a 2-tuple (wwww,d) e.g. (1990,0)
         if None, then only date_start is researched
-    
+
     severe : bool
         If True, raises an exception if something goes wrong
 
     compressed : str
         How the compressed files are handled
         "incl": include the compressed files
         "only": only consider the compressed files
         "excl": exclude the compressed files
-        
+
     regex_old_naming : bool
         Handle old naming format
 
     regex_new_naming : bool
         Handle new naming format        
-    
+
     regex_igs_tfcc_naming : bool
         Handle TFCC specific format (for SINEX files)
-        
+
     add_weekly_file : bool
         Also handle the weekly file (day 7)
         Implemented only for the  old naming format (for the moment)
 
     Returns
     -------
     Files_select_cumul_list : list
         List of files found
 
     """
-    
+
     ###### Prelim Checks   ##############
     if not os.path.exists(parent_dir):
         log.error("parent directory doesn't exist")
         log.error(parent_dir)
         if severe:
             raise Exception
 
     ###### Time management ##############
-    ###### work internally with datetime
-    ### date_start
+    # work internally with datetime
+    # date_start
     if type(date_start) is dt.datetime:
         date_start_ok = date_start
     else:
         date_start_ok = conv.gpstime2dt(*date_start)
-    ### date_end
+    # date_end
     if not date_end:
         date_end_ok = date_start_ok
     elif type(date_end) is dt.datetime:
         date_end_ok = date_end
     else:
         date_end_ok = conv.gpstime2dt(*date_end)
-    ### generate time period with a while loop
+    # generate time period with a while loop
     Dates_list = [date_start_ok]
     while Dates_list[-1] < date_end_ok:
-        Dates_list.append(Dates_list[-1]  + dt.timedelta(days=1))
-        
-    ### manage weekly file 
-    Dates_wwwwd_list   = [utils.join_improved("",*conv.dt2gpstime(d,outputtype=str)) for d in Dates_list]
-    Dates_yyyyddd_list = [utils.join_improved("",*reversed(conv.dt2doy_year(d))) for d in Dates_list]
+        Dates_list.append(Dates_list[-1] + dt.timedelta(days=1))
+
+    # manage weekly file
+    Dates_wwwwd_list = [utils.join_improved(
+        "", *conv.dt2gpstime(d, outputtype=str)) for d in Dates_list]
+    Dates_yyyyddd_list = [utils.join_improved(
+        "", *reversed(conv.dt2doy_year(d))) for d in Dates_list]
 
     ###### File type / ACs management ##############
 
     if not utils.is_iterable(File_type):
         File_type = [File_type]
     if not utils.is_iterable(ACs):
         ACs = [ACs]
 
     ###### General file search management ##############
     if utils.is_iterable(parent_dir):
         FILE_LIST = parent_dir
     elif recursive_search:
         # All the files are listed first
-        FILE_LIST = utils.find_recursive(parent_dir,".*",case_sensitive=False)
+        FILE_LIST = utils.find_recursive(
+            parent_dir, ".*", case_sensitive=False)
     else:
         FILE_LIST = glob.glob(parent_dir + "/*")
 
-
     ###### Regex Definition ##############
-    
-    join_regex_and = lambda  L : "(" +  "|".join(L) + ")"
-    
+
+    def join_regex_and(L): return "(" + "|".join(L) + ")"
+
     Re_patt_big_stk = []
-    
-    
-    ### compression handeling
+
+    # compression handeling
     if compressed == "excl":
         re_patt_comp = "$"
     elif compressed == "incl":
         re_patt_comp = "(\.Z|\.gz|)$"
     elif compressed == "only":
         re_patt_comp = "(\.Z|\.gz)$"
     else:
         log.error("check 'compressed' keyword (excl,incl, or only)")
         raise Exception
-        
-    if regex_old_naming: 
+
+    if regex_old_naming:
         if ACs[0] == "all":
             re_patt_ac = "\w{3}"
         else:
             re_patt_ac = join_regex_and([ac.lower() for ac in ACs])
-                 
+
         if add_weekly_file:
-            Dates_wwwwd_list_4old = [ e[:-1] + "(" + e[-1] + "|" + "7)"  for e in Dates_wwwwd_list]
+            Dates_wwwwd_list_4old = [
+                e[:-1] + "(" + e[-1] + "|" + "7)" for e in Dates_wwwwd_list]
         else:
             Dates_wwwwd_list_4old = Dates_wwwwd_list
-        
-        re_patt_date   = join_regex_and(Dates_wwwwd_list_4old)
+
+        re_patt_date = join_regex_and(Dates_wwwwd_list_4old)
         re_patt_filtyp = join_regex_and(File_type)
-        re_patt_big_old_naming = re_patt_ac + re_patt_date + "\." + re_patt_filtyp + re_patt_comp
+        re_patt_big_old_naming = re_patt_ac + re_patt_date + \
+            "\." + re_patt_filtyp + re_patt_comp
         Re_patt_big_stk.append(re_patt_big_old_naming)
-        
-    if regex_new_naming: ### search for new name convention
+
+    if regex_new_naming:  # search for new name convention
         if ACs[0] == "all":
-            re_patt_ac = "\W{3}"        
+            re_patt_ac = "\W{3}"
         else:
             re_patt_ac = join_regex_and([ac.upper() for ac in ACs])
-        re_patt_date   = join_regex_and(["_"+e for e in Dates_yyyyddd_list]) #add _ because it can raise a conflit with the old format
+        # add _ because it can raise a conflit with the old format
+        re_patt_date = join_regex_and(["_"+e for e in Dates_yyyyddd_list])
         re_patt_filtyp = join_regex_and([fil.upper() for fil in File_type])
-        re_patt_big_new_naming = ".*".join((re_patt_ac,re_patt_date,re_patt_filtyp + re_patt_comp))
+        re_patt_big_new_naming = ".*".join((re_patt_ac,
+                                           re_patt_date,
+                                           re_patt_filtyp + re_patt_comp))
         Re_patt_big_stk.append(re_patt_big_new_naming)
-        
+
     if regex_igs_tfcc_naming:
-        Dates_yy_list = list(set([str(conv.gpstime2dt(int(e[0:4]),int(e[4])).year)[2:] for e in Dates_wwwwd_list]))
+        Dates_yy_list = list(set([str(conv.gpstime2dt(int(e[0:4]), int(e[4])).year)[
+                             2:] for e in Dates_wwwwd_list]))
         Dates_wwww_list = list(set([e[:-1] for e in Dates_wwwwd_list]))
         #Dates_wwww_dot_list = [e + "\." for e in Dates_wwww_list]
         re_patt_year = join_regex_and(Dates_yy_list)
         # 2x re_patt_date : because .sum doesn't the day
         re_patt_date = join_regex_and(Dates_wwwwd_list + Dates_wwww_list)
-        re_patt_filtyp = "\." +  join_regex_and(File_type)
+        re_patt_filtyp = "\." + join_regex_and(File_type)
 
-        re_patt_big_igs_tfcc_naming = "igs" + re_patt_year + "P" + re_patt_date + ".*" + re_patt_filtyp + re_patt_comp
+        re_patt_big_igs_tfcc_naming = "igs" + re_patt_year + "P" + \
+            re_patt_date + ".*" + re_patt_filtyp + re_patt_comp
         Re_patt_big_stk.append(re_patt_big_igs_tfcc_naming)
 
     re_patt_big = join_regex_and(Re_patt_big_stk)
-        
-    log.info("REGEX researched :")    
+
+    log.info("REGEX researched :")
     log.info(re_patt_big)
-    
+
     ###### Specific file search management ##############
     Files_select_list = []
     for fil in FILE_LIST:
-        if re.search(re_patt_big,os.path.basename(fil),re.IGNORECASE):
+        if re.search(re_patt_big, os.path.basename(fil), re.IGNORECASE):
             Files_select_list.append(fil)
-            
+
     if len(Files_select_list) == 0:
         log.error("no products found")
         if severe:
             raise Exception
 
-    log.info("number of files found : %s",len(Files_select_list))    
+    log.info("number of files found : %s", len(Files_select_list))
     log.info(re_patt_big)
-    
-    return Files_select_list
-
 
+    return Files_select_list
```

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/download_prods.py` & `geodezyx-0.4.3.3/geodezyx/operational/download_prods.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/download_rinex.py` & `geodezyx-0.4.3.3/geodezyx/operational/download_rinex.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/download_utils.py` & `geodezyx-0.4.3.3/geodezyx/operational/download_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/gins_runner.py` & `geodezyx-0.4.3.3/geodezyx/operational/gins_runner.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/groops_frontend.py` & `geodezyx-0.4.3.3/geodezyx/operational/groops_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/hector_frontend.py` & `geodezyx-0.4.3.3/geodezyx/operational/hector_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/midas_frontend.py` & `geodezyx-0.4.3.3/geodezyx/operational/midas_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/rinex_lister_plotter.py` & `geodezyx-0.4.3.3/geodezyx/operational/rinex_lister_plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     Returns
     -------
     rinexfilelist : list
         list of rinex files.
         
     Notes
     -----
-    
     operational.rinex_finder must be used in priority !!! (July 2022)
     """
     
     log.warning("rinex_lister depreciated, use operational.rinex_finder instead!!")
     
 
     if type(path) is str:
```

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/rinex_utils.py` & `geodezyx-0.4.3.3/geodezyx/operational/rinex_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,14 +478,15 @@
 
     Parameters
     ----------
     input_rinex_path : TYPE
         path of the rinex file.
         can be the path of a RINEX or directly
         the RINEX content as a string     
+
     interval_out : bool, optional
         output also the intervals. The default is False.
         
     add_tzinfo : bool, optional
         add timezone information in the datetime's Epoches.
         The default is False.
 
@@ -517,39 +518,48 @@
 
     Tail =  utils.tail(input_rinex_path,1500)
     epochs_list_tail = rinex_read_epoch(Tail,interval_out=interval_out,
                                         add_tzinfo=add_tzinfo,out_array=False)
 
     epochs_list = epochs_list_head + epochs_list_tail
 
-    if len(epochs_list) == 0:
-        first_epoch = conv.rinexname2dt(input_rinex_path)
-        alphabet = list(string.ascii_lowercase)
-
-        if os.path.basename(input_rinex_path)[7] in alphabet:
-            last_epoch = first_epoch + dt.timedelta(hours=1)
-        else:
-            last_epoch = first_epoch + dt.timedelta(hours=24,seconds=-1)
-    else:
+    if len(epochs_list) > 0:
         first_epoch = np.min(epochs_list)
         last_epoch = np.max(epochs_list)
+    else:
+        ## here is the save mode where everything can goes wrong ;)
+        first_epoch = conv.rinexname2dt(input_rinex_path)
+        if first_epoch:
+            last_epoch = first_epoch + dt.timedelta(seconds=85399)
+        else:
+            ### here the return is None, your file is corrupted
+            last_epoch = None
+            return first_epoch,last_epoch 
+
+        ##### this legacy block if for short name only
+        #alphabet = list(string.ascii_lowercase)
+        #if os.path.basename(input_rinex_path)[7] in alphabet:
+        #    last_epoch = first_epoch + dt.timedelta(hours=1)
+        #else:
+        #    last_epoch = first_epoch + dt.timedelta(hours=24,seconds=-1)
 
     if add_tzinfo:
         first_epoch = first_epoch.replace(tzinfo=dateutil.tz.tzutc())
         last_epoch = last_epoch.replace(tzinfo=dateutil.tz.tzutc())
 
     if verbose:
-        log.info("first & last epochs: %s %s" , first_epoch , last_epoch)
+        log.debug("first & last epochs: %s %s" , first_epoch , last_epoch)
+
     if not interval_out:
         return first_epoch , last_epoch
     else:
         interv_lis = np.diff(epochs_list)
         interv_lis = [e.seconds + e.microseconds * 10**-6 for e in interv_lis]
         interval   = utils.most_common(interv_lis)
-        log.info("interval, last epoch: %s %s" , interval , last_epoch)
+        log.debug("interval, last epoch: %s %s" , interval , last_epoch)
 
         #return interv_lis , epochs_list
         return first_epoch , last_epoch , interval
 
 def rinex_session_id(first_epoch,last_epoch,full_mode=False):
     """
     full_mode:
```

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/rtklib_frontend.py` & `geodezyx-0.4.3.3/geodezyx/operational/rtklib_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/operational/track_frontend.py` & `geodezyx-0.4.3.3/geodezyx/operational/track_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/reffram/geometry.py` & `geodezyx-0.4.3.3/geodezyx/reffram/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,14 +495,16 @@
     https://elib.uni-stuttgart.de/bitstream/11682/9661/1/BscThesis_GaoYueqing.pdf
     """
 
     l_stk = []
     A_stk = []
     Bool_stk = []
     
+    log.error("we have %s points",len(X1list))
+    
     for X1 , X2 in zip(X1list , X2list):
         
         if np.sum(np.isnan(X1)) or np.sum(np.isnan(X2)):
             log.warning("one point component is nan, skipping")
             Bool_stk.append(False)
             continue
```

### Comparing `geodezyx-0.4.3.2/geodezyx/reffram/gnss_products.py` & `geodezyx-0.4.3.3/geodezyx/reffram/gnss_products.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/reffram/kepler_gzyx.py` & `geodezyx-0.4.3.3/geodezyx/reffram/kepler_gzyx.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/reffram/quaternions.py` & `geodezyx-0.4.3.3/geodezyx/reffram/quaternions.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/stats/least_squares.py` & `geodezyx-0.4.3.3/geodezyx/stats/least_squares.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/stats/stats.py` & `geodezyx-0.4.3.3/geodezyx/stats/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1176,15 +1176,15 @@
     si un point a un sigma > threshold * moy(sigmas) on le vire
     
     really old and discontinued, and not really efficient
     """
     moy = np.median(datasigmain)
     marge = moy * threshold
 
-    log.info("moy,threshold,margin",  moy,threshold,marge)
+    log.info("moy,threshold,margin: %f, %i, %f",  moy,threshold,marge)
 
     boolbad = np.abs(datasigmain) < marge
 
     datasigmaout = datasigmain[boolbad]
 
     return datasigmaout,boolbad
```

### Comparing `geodezyx-0.4.3.2/geodezyx/time_series/ts_class.py` & `geodezyx-0.4.3.3/geodezyx/time_series/ts_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,36 +145,39 @@
         self.sH = sH
 
         self.initype = 'FLH'
         self.X,self.Y,self.Z = conv.GEO2XYZ(self.F,self.L,self.H)
         self.sX,self.sY,self.sZ = conv.sFLH2sXYZ(F,L,H,sF,sL,sH)
         
 
-    def ENUset(self,E=np.nan,N=np.nan,U=np.nan,sE=np.nan,sN=np.nan,sU=np.nan):
+    def ENUset(self,E=np.nan,N=np.nan,U=np.nan,
+               sE=np.nan,sN=np.nan,sU=np.nan):
         self.E = E
         self.N = N
         self.U = U
         self.sE = sE
         self.sN = sN
         self.sU = sU
 
         self.initype = 'ENU'
 
-    def NEDset(self,N=np.nan,E=np.nan,D=np.nan,sN=np.nan,sE=np.nan,sD=np.nan):
+    def NEDset(self,N=np.nan,E=np.nan,D=np.nan,
+               sN=np.nan,sE=np.nan,sD=np.nan):
         self.N = N
         self.E = E
         self.D = D
         self.sN = sN
         self.sE = sE
         self.sD = sD
 
         self.initype = 'NED'
 
 
-    def UTMset(self,Eutm=np.nan,Nutm=np.nan,Uutm=np.nan,sEutm=np.nan,sNutm=np.nan,sUutm=np.nan):
+    def UTMset(self,Eutm=np.nan,Nutm=np.nan,Uutm=np.nan,
+               sEutm=np.nan,sNutm=np.nan,sUutm=np.nan):
         self.Eutm = Eutm
         self.Nutm = Nutm
         self.Uutm = Uutm
         self.sEutm = sEutm
         self.sNutm = sNutm
         self.sUutm = sUutm
 
@@ -202,22 +205,25 @@
 
         self.refENU = refENU
 
         dX =  self.X - refENU.X
         dY =  self.Y - refENU.Y
         dZ =  self.Z - refENU.Z
 
-        self.E,self.N,self.U = conv.XYZ2ENU(dX,dY,dZ,refENU.F,refENU.L)
+        Etmp,Ntmp,Utmp = conv.XYZ2ENU(dX,dY,dZ,refENU.F,refENU.L)
+        self.E,self.N,self.U = Etmp[0],Ntmp[0],Utmp[0]
 
         if self.initype == 'FLH' and hasattr(self,'sF'):
             if not np.isnan(self.sF):
-                self.sE,self.sN,self.sU = conv.sFLH2sENU(self.F,self.L,self.H,self.sF,self.sL,self.sH)
+                self.sE,self.sN,self.sU = conv.sFLH2sENU(self.F,self.L,self.H,
+                                                         self.sF,self.sL,self.sH)
         elif self.initype == 'XYZ' and hasattr(self,'sX'):
             if not np.isnan(self.sX):
-                self.sE,self.sN,self.sU = conv.sXYZ2sENU(self.X,self.Y,self.Z,self.sX,self.sY,self.sZ)
+                self.sE,self.sN,self.sU = conv.sXYZ2sENU(self.X,self.Y,self.Z,
+                                                         self.sX,self.sY,self.sZ)
 
 
     def UTMcalc_pt(self,ellips="wgs84"):
         self.Eutm , self.Nutm , _ = conv.utm_geo2xy(self.F,self.L)
         self.Uutm = self.H
         
 
@@ -710,15 +716,15 @@
         symbol : str, optional
             symbol. The default is '.'.
         errbar_width : TYPE, optional
             coefficient for the error bar size. The default is 1.
 
         Returns
         -------
-        None.
+        The matplotlib Figure object.
 
         """
         
         log.setLevel(logging.INFO)
 
         if new_style:
             styleint = 310
@@ -1006,14 +1012,27 @@
         Returns
         -------
         None.
 
         """
         self.ENUcalc(self.mean_posi())
         return None
+    
+    
+    def ENUcalc_from_first_posi(self):
+        """
+        Method to determine the ENU components based directly on the mean position
+
+        Returns
+        -------
+        None.
+
+        """
+        self.ENUcalc(self.pts[0])
+        return None
 
     def from_uniq_point(self,Point,startdate,enddate,pas=1):
         self.del_data()
 
         if type(startdate) == dt.datetime:
             startdate = conv.dt2posix(startdate)
         if type(enddate) == dt.datetime:
```

### Comparing `geodezyx-0.4.3.2/geodezyx/time_series/ts_fcts.py` & `geodezyx-0.4.3.3/geodezyx/time_series/ts_fcts.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,19 +17,14 @@
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import stats
 from geodezyx import utils
 from geodezyx import time_series
 from geodezyx import reffram
 
-#### Import star style
-# from geodezyx import *                   # Import the GeodeZYX modules
-# from geodezyx.externlib import *         # Import the external modules
-# from geodezyx.megalib.megalib import *   # Import the legacy modules names
-
 #### Import the logger
 import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
@@ -263,17 +258,21 @@
                  markersize=diapt, alpha=alpha,color=color)
         axD.set_ylabel(ylbl)
         axD.legend()
         axD.set_title(Dti)
         
     return fig
 
+
+
+
+
 def compar(tstup , coortype='ENU' , seuil=3. , win=[] , mode='keep' ,
-           Dtype='2D3D', namest=0,namend=10,alpha = 5 , diapt = 5 , 
-           verbose=True, print_report=True,plot=True):
+           Dtype='2D3D', namest=0,namend=10,alpha = 0.8 , diapt = 5 , 
+           verbose=True, print_report=True,plot=True,interp=True):
     """
         si seuil == 0, pas de nettoyage
 
         On preconise compar en mode keep :
         Ainsi le Tref est strictement cantonné aux bonnes valeurs des Ti
         En mode del, les Ti sont extrapolé aux valeur de Tref => nan => pbs pour la mad
 
@@ -285,16 +284,14 @@
 
     if len(Dtype) == 4:
         D2n3 = True
         Dtype = Dtype[0:2]
     else:
         D2n3 = False
 
-    diapt=10
-    alpha=0.8
 
     if len(tstup) <= 1:
         log.error("len(tstup) <= 1 , do not compare a single element !! ;) ")
 
     if verbose:
         log.info("COMPARISON SUMMARY")
         log.info("reference : %s",  tstup[0].name)
@@ -312,21 +309,24 @@
             log.info("------------------------------")
 
 
 #        tsout = TimeSeriePoint()
 #        tsout = copy.copy(tsvar)
 #        tsout.del_data()
 
+
         if tsvar.bool_interp_uptodate == False:
             tsvar.interp_set()
 
         A, B, C, T, sA , sB , sC = tsvar.to_list(coortype=coortype)
 
         tsref = tstup[0].interp_get(T,coortype=coortype)
         Aref, Bref, Cref , Tref , sA , sB , sC = tsref.to_list(coortype=coortype)
+        
+        
 
 
         # WTF IS THOSE LINES
         # autowin = time_gap(tstup[0],marge=1.1,mode='keep')
         # win = autowin
         #
         # outbool = []
@@ -373,39 +373,39 @@
 
         # nettoyage par la MAD
         if seuil != 0:
             if verbose:
                 log.info("MAD cleaning")
                 
             dAin = dA
-            dA,bb = stats.outlier_mad(dA,seuil=seuil)
+            dA,bb = stats.outlier_mad(dA,threshold=seuil)
             dAout = dA
             TA = conv.posix2dt(np.array(Tref[bb]))
 
             dBin = dB
-            dB,bb = stats.outlier_mad(dB,seuil=seuil)
+            dB,bb = stats.outlier_mad(dB,threshold=seuil)
             dBout = dB
             TB = conv.posix2dt(np.array(Tref[bb]))
 
             dCin = dC
-            dC,bb = stats.outlier_mad(dC,seuil=seuil)
+            dC,bb = stats.outlier_mad(dC,threshold=seuil)
             dCout = dC
             TC = conv.posix2dt(np.array(Tref[bb]))
 
             dDin = dD
-            dD,bb = stats.outlier_mad(dD,seuil=seuil)
+            dD,bb = stats.outlier_mad(dD,threshold=seuil)
             TD = conv.posix2dt(np.array(Tref[bb]))
             dDout = dD
             if D2n3:
                 dD2Din = dD2D
-                dD2D,bb = stats.outlier_mad(dD2D,seuil=seuil)
+                dD2D,bb = stats.outlier_mad(dD2D,threshold=seuil)
                 TD2D = conv.posix2dt(np.array(Tref[bb]))
                 dD2Dout = dD2D
                 dD3Din = dD3D
-                dD3D,bb = stats.outlier_mad(dD3D,seuil=seuil)
+                dD3D,bb = stats.outlier_mad(dD3D,threshold=seuil)
                 TD3D = conv.posix2dt(np.array(Tref[bb]))
                 dD3Dout = dD3D
 
             if verbose:
                 log.info("Stats after cleaning")
 
             if print_report:
@@ -530,18 +530,22 @@
                mode='round'):
     tsout = copy.deepcopy(tsin)
     Tdtin = tsin.to_list(coortype=tsin.initype(),
                          time_as_datetime=True)[3]
     
     Tdtout = conv.round_dt(Tdtin,round_to=round_to,mode=mode,
                            python_dt_out=True)
+
+    tsout.bool_interp_uptodate = False
     
     for pt,t in zip(tsout,Tdtout):
         pt.Tset(conv.numpy_dt2dt(t))
         
+    tsout.interp_set()
+        
     return tsout
 
 def mad_cleaner(tsin,seuil=3.5,method='dist',coortype='ABC',
                 detrend_first=False,output_detrended=False, verbose=False):
     '''
     method : methode d'élimination :
             dist : on élimine les point qu sont trop loin en distance de la posi de ref
@@ -586,17 +590,17 @@
 def sigma_cleaner(tsin,seuil=3,coortype='ABC',cleantype='any', verbose=False):
 
     if coortype == 'ABC':
         coortype = tsin.initype()
 
     A,B,C,T,sA,sB,sC = tsin.to_list(coortype)
 
-    sAout , bbsA = stats.outiler_sigma(sA,seuil)
-    sBout , bbsB = stats.outiler_sigma(sB,seuil)
-    sCout , bbsC = stats.outiler_sigma(sC,seuil)
+    sAout , bbsA = stats.outlier_sigma(sA,seuil)
+    sBout , bbsB = stats.outlier_sigma(sB,seuil)
+    sCout , bbsC = stats.outlier_sigma(sC,seuil)
 
     if cleantype == 'any':
         boolbad = bbsA * bbsB * bbsC
     elif cleantype == 'all':
         boolbad = bbsA + bbsB + bbsC
     tsout = bool_cleaner(tsin,boolbad)
 
@@ -759,295 +763,14 @@
     discont_improved = tsin.discont + [dt.datetime(2099,1,1)]
     for j in range(len(discont_improved)-1):
         log.info('period %s: %s %s',j,discont_improved[j],discont_improved[j+1])
         tsbis = time_win(tsin,[[discont_improved[j],discont_improved[j+1]]])
         datetitle = ' : ' + str(discont_improved[j]) + "\u2192" + str(discont_improved[j+1])
         linear_regress_ts(tsbis,coortype,titledetails=datetitle)
 
-#def export_ts_as_pbo_pos(tsin):
-#    # IN PROGRESS
-#    tswork = copy.deepcopy(tsin)
-#    outtfile.write('{:.5f}   {:+.6f}    {:+.6f}    {:+.6f} {:+.6f} {:+.6f} {:+.6f}\n'.format(t,n-n0,e-e0,u-u0,se,sn,su))
-#
-
-def export_ts_figure_pdf(fig,export_path,filename,close=False):
-    """ fig can accept a int (id of a Figure)
-         OR the figure Object itself """
-
-    if type(fig) is int:
-        f = plt.figure(fig)
-    elif type(fig) is plt.Figure:
-        f = fig
-
-    f.set_size_inches(16.53,11.69)
-    # tralala pour avoir des dates propres
-    # parce que dans des cas + simples f.autofmt_xdate() suffit
-    for a in f.axes[1:]:
-        labels = a.get_xticklabels()
-        for l in labels:
-            l.set_rotation(40)
-            l.set_horizontalalignment('right')
-    out_path = os.path.join(export_path,filename+'.pdf')
-    f.tight_layout()
-    f.subplots_adjust(top=0.94)
-    f.savefig(out_path,papertype='a4',format='pdf')
-
-    if close:
-        plt.close(f)
-
-    return None
-
-def export_ts_plot(tsin,export_path,coortype='ENU',export_type=("pdf","png"),
-                   plot_B = False,close_fig_after_export=True):
-    """ Very beta ...
-        to be implemented : merge w/ the export_figure_pdf fct """
-    # plot A avec les barres de sigma
-    plt.clf()
-    tsin.plot(coortype,fig=1)
-    tsin.plot_discont()
-    f = plt.gcf()
-    f.set_size_inches(16.53,11.69)
-    # tralala pour avoir des dates propres
-    # parce que dans des cas + simples f.autofmt_xdate() suffit
-    for a in f.axes[1:]:
-        labels = a.get_xticklabels()
-        for l in labels:
-            l.set_rotation(40)
-            l.set_horizontalalignment('right')
-    f.tight_layout()
-    f.subplots_adjust(top=0.92)
-    for typ in export_type:
-        export_file = os.path.join(export_path,tsin.stat+'a.' + typ)
-        f.savefig(export_file,
-                  papertype='a4',format=typ)
-        log.info("plot exported in %s" , export_file)
-    if close_fig_after_export:
-        plt.close(f)
-
-    # plot B avec une droite de regression
-    if plot_B:
-        linear_regress_ts(tsin)
-        f = plt.gcf()
-        #    f.set_dpi(300)
-        f.set_size_inches(16.53,11.69)
-        for a in f.axes:
-            labels = a.get_xticklabels()
-            for l in labels:
-                l.set_rotation(40)
-                l.set_horizontalalignment('right')
-        f.tight_layout()
-        f.subplots_adjust(top=0.92)
-        for typ in export_type:
-            export_file = os.path.join(export_path,tsin.stat+'b.' + typ)
-            f.savefig(export_file,
-                      papertype='a4',format=typ)
-        log.info("plot exported in %s" , export_file)
-        if close_fig_after_export:
-            plt.close(f)
-    return None
-
-
-def export_ts(ts,outdir,coordtype = 'ENU',outprefix='',write_header=False):
-    """
-    export the timeserie
-
-    write_header not well implemented !!!
-    """
-
-    proto_str = '{:23} ' * 14
-
-    A,B,C,T,sA,sB,sC = ts.to_list(coordtype)
-    if outprefix != '':
-        outprefix = outprefix + '_'
-
-    outfilenam = outprefix +  ts.stat + "_" +  ts.name + '.' + coordtype + '.ts.dat'
-    outpath = os.path.join(outdir,outfilenam)
-
-    filobj = open(outpath,'w+')
-
-    if write_header:
-        header = "#" + proto_str.format(*(coordtype[0],"sigma"+coordtype[0],
-                                          coordtype[1],"sigma"+coordtype[1],
-                                          coordtype[2],"sigma"+coordtype[2],
-                                          "year","month","day",
-                                          "hour","minute","seconds",
-                                          "year_decimal","posix_time"))
-        filobj.write(header + "\n")
-
-    for a,b,c,t,sa,sb,sc in zip(A,B,C,T,sA,sB,sC):
-        paramstr = [str(e) for e in [a,sa,b,sb,c,sc]]
-        #paramstr = [e.ljust(18, '0') for e in paramstr]
-        
-        tt = conv.posix2dt(t)
-        yr_dec_str = str(conv.dt2year_decimal(tt))
-        posix_str = str(t)
-
-        paramstr_time = list(tt.strftime("%Y %m %d %H %M %S").split())
-
-        paramstr2 = paramstr + paramstr_time + [yr_dec_str,posix_str]
-        
-        outlin =  proto_str.format(*paramstr2) + "\n"
-        filobj.write(outlin)
-    filobj.close()
-
-    log.info('timeserie exported in %s', outpath)
-    return None
-
-
-def export_ts_as_neu(tsin,outdir,outprefix,coordtype = 'ENU'):
-    """
-    export to a HECTOR .neu compatible format
-
-    outfile will be writed in
-    /outdir/outprefixSTAT.neu
-    
-    NB: The XYZ mode is quite dirty (191001)
-    """
-    if not hasattr(tsin[0],'X'):
-        log.warning('no XYZ in ts')
-        noXYZ = True
-    else:
-        noXYZ = False
-
-    tswork = copy.deepcopy(tsin)
-    #if coordtype == 'XYZ':
-    #    mp = tswork.mean_posi()
-    #    tswork.ENUcalc(mp)
-    outpath = outdir +'/' + outprefix + tswork.stat + '.neu'
-    outfile = open(outpath,'w+')
-    E,N,U,T,sE,sN,sU = tswork.to_list(coordtype)
-    first_pt = tswork.pts[0]
-    if noXYZ:
-        first_pt.X = 0.
-        first_pt.Y = 0.
-        first_pt.Z = 0.
-        first_pt.L = 0.
-        first_pt.H = 0.
-        first_pt.F = 0.
-
-
-    e0,n0,u0,t0 = list(zip(E,N,U,T))[0]
-    # write the header
-    outfile.write('# Site : {} \n'.format(tswork.stat))
-    if 'calc_center' in list(tswork.anex.keys()):
-        outfile.write('# Analysis Centre: {} \n'.format(tswork.anex['calc_center']))
-    else:
-        outfile.write('# Analysis Centre: N/A \n')
-
-    outfile.write('# Solution code: GINS_PS \n')
-    outfile.write('# Datum: ITRF2008\n')
-    outfile.write('#\n')
-    outfile.write('# Reference epoch: {}\n'.format(conv.dt2year_decimal(first_pt.Tdt)))
-    outfile.write('# X : {}\n'.format(first_pt.X))
-    outfile.write('# Y : {}\n'.format(first_pt.Y))
-    outfile.write('# Z : {}\n'.format(first_pt.Z))
-    outfile.write('#\n')
-    outfile.write('# Longitude : {}\n'.format(first_pt.L))
-    outfile.write('# Latitude  : {}\n'.format(first_pt.F))
-    outfile.write('# Height    : {}\n'.format(first_pt.H))
-    outfile.write('#\n')
-    if coordtype == "ENU":
-        outfile.write('# Components : ' + "NEU" + "\n")
-    elif coordtype == "XYZ":
-        outfile.write('# Components : ' + "YXZ" + "\n")
-        outfile.write('# Cartesian components are undirect to maintain consistency with NEU\n')                
-    outfile.write('#\n')
-    if tswork.bool_discont:
-        outfile.write('# type_of_offset : from discontinuties got from a station.info\n')
-        outfile.write('#\n')
-        for disc in sorted(tswork.discont):
-            outfile.write('# offset {} 7\n'.format(conv.dt2year_decimal(disc)))
-        outfile.write('#\n')
-    # write the data
-    for e,n,u,t,se,sn,su in zip(E,N,U,T,sE,sN,sU):
-        t = conv.dt2year_decimal(conv.posix2dt(t))
-        if coordtype == "ENU":        
-            outfile.write('{:.5f}   {:+.6f}    {:+.6f}    {:+.6f} {:+.6f} {:+.6f} {:+.6f}\n'.format(t,n-n0,e-e0,u-u0,se,sn,su))
-        elif coordtype == "XYZ":
-            outfile.write('{:.5f}   {:+.6f}    {:+.6f}    {:+.6f} {:+.6f} {:+.6f} {:+.6f}\n'.format(t,n-n0,e-e0,u-u0,se,sn,su))
-
-    log.info('timeserie exported in %s',outpath)
-    return None
-
-
-def export_ts_as_hector_enu(tsin,outdir,outprefix,coordtype = 'ENU'):
-    """
-    export to a HECTOR .enu (and not .neu !) compatible format
-    This format is simpler : just gives MJD E N U
-
-    This format is necessary to force a sampling period.
-
-    outfile will be writed in
-    /outdir/outprefixSTAT.enu
-    """
-
-    log.warning("NOT IMPLEMENTED YET !")
-
-    return None
-
-
-
-def export_ts_as_midas_tenu(tsin,outdir,outprefix,coordtype = 'ENU',
-                            export_step=True):
-    """
-    export to a MIDAS .tneu compatible format
-
-    outfile will be writed in
-    /outdir/outprefixSTAT.tneu
-
-    if export_step == True:
-    export a step file as
-    /outdir/outprefixSTAT.step
-    """
-    if not hasattr(tsin[0],'X'):
-        log.warning('no XYZ in ts')
-        noXYZ = True
-    else:
-        noXYZ = False
-
-    tswork = copy.deepcopy(tsin)
-    stat = tswork.stat
-    if coordtype == 'XYZ':
-        mp = tswork.mean_posi()
-        tswork.ENUcalc(mp)
-    outpath = outdir +'/' + outprefix + tswork.stat + '.tenu'
-    outfile = open(outpath,'w+')
-    E,N,U,T,sE,sN,sU = tswork.to_list('ENU')
-    first_pt = tswork.pts[0]
-    if noXYZ:
-        first_pt.X = 0.
-        first_pt.Y = 0.
-        first_pt.Z = 0.
-        first_pt.L = 0.
-        first_pt.H = 0.
-        first_pt.F = 0.
-
-    e0,n0,u0,t0 = list(zip(E,N,U,T))[0]
-
-    for e,n,u,t in zip(E,N,U,T):
-        t = conv.dt2year_decimal(conv.posix2dt(t))
-        #outfile.write('{} {:.5f} {:+.6f} {:+.6f} {:+.6f} \n'.format(stat,t,n-n0,e-e0,u-u0))
-        outfile.write('{} {:.5f} {:+.6f} {:+.6f} {:+.6f} \n'.format(stat,t,e-e0,n-n0,u-u0))
-
-    log.info('timeserie exported in %s',outpath)
-
-    if export_step and tswork.bool_discont:
-        outpath_step = outdir +'/' + outprefix + tswork.stat + '.step'
-        outfile_step = open(outpath_step,'w+')
-        for d in tswork.discont:
-            d = conv.dt2year_decimal(d)
-            line = tswork.stat + " " + str(d) + "\n"
-            outfile_step.write(line)
-
-            log.info('timeserie discont. (steps) exported in %s',outpath_step)
-
-    return None
-
-
-
 
 def decimate_cleaner(tsin,minval,in_place = False):
     """
     in_place DOES'NT WORK !!!
     """
     if not in_place:
         tsout = copy.deepcopy(tsin)
@@ -1249,42 +972,48 @@
 
     for t2 in T2:
         T1.remove(t2)
 
     return T1
 
 
-def rotate_pt_cls_solo(tsattin,pointin,Rtype='R1', xyzreftuple = ([1, 0, 0], [0, 1, 0], [0, 0, 1]),angtype='deg'):
+def rotate_pt_cls_solo(tsattin,pointin,Rtype='R1',
+                       xyzreftuple = ([1, 0, 0], [0, 1, 0], [0, 0, 1]),
+                       angtype='deg'):
     ''' ENTREE : tsattin : une TS d'attitude  (N angles)
                  pointin : UN Point en entrée
 
         SORTIE : une TSpoint de N points '''
 
     attlisttmp = tsattin.to_list()
     R = attlisttmp[0]
     P = attlisttmp[1]
     Y = attlisttmp[2]
     T = attlisttmp[3]
 
     A,B,C,_,_ = pointin()
 
-    ptrotlis = XXX.rotate_points(R,P,Y,[np.array([A,B,C])],Rtype,xyzreftuple,angtype)
+    ptrotlis = XXX.rotate_points(R,P,Y,[np.array([A,B,C])],
+                                 Rtype,xyzreftuple,angtype)
 
     ptrotlis = utils.shrink_listoflist(ptrotlis)
 
     tsout = time_series.TimeSeriePoint()
 
     for p,t in zip(ptrotlis,T):
         #print p
-        tsout.add_point(time_series.Point(p[0],p[1],p[2],t,initype=pointin.initype))
+        tsout.add_point(time_series.Point(p[0],p[1],p[2],t,
+                                          initype=pointin.initype))
 
     return tsout
 
 
-def rotate_points_class(tsattin,ptslin, Rtype='R1', xyzreftuple = ([1, 0, 0], [0, 1, 0], [0, 0, 1]),angtype='deg'):
+def rotate_points_class(tsattin,ptslin, Rtype='R1',
+                        xyzreftuple = ([1, 0, 0], [0, 1, 0], [0, 0, 1]),
+                        angtype='deg'):
 
     listsout = []
 
     for pt in ptslin:
         ts = rotate_pt_cls_solo(tsattin,pt,Rtype,xyzreftuple,angtype)
         listsout.append(ts)
```

### Comparing `geodezyx-0.4.3.2/geodezyx/utils/dict_utils.py` & `geodezyx-0.4.3.3/geodezyx/utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/utils/list_utils.py` & `geodezyx-0.4.3.3/geodezyx/utils/list_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/utils/pandas_utils.py` & `geodezyx-0.4.3.3/geodezyx/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/utils/plot_utils.py` & `geodezyx-0.4.3.3/geodezyx/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/geodezyx/utils/shell_like.py` & `geodezyx-0.4.3.3/geodezyx/utils/shell_like.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,15 +311,15 @@
         * wildcard (only * and ?) for case_sensitive = True
         * regex for case_sensitive = False
         
     sort_results : bool
         Sort results
         
     case_sensitive : bool
-        Case sensitve or not. If False, the pattern *must* be a regex
+        Case sensitive or not. If False, the pattern *must* be a regex
         
     extended_file_stats : bool
         if True, returns the stats of the files
         the outputed matches list will be a list of tuples
         (file_path,stat_object), where stat_object has the following attributes
         
         - st_mode - protection bits,
@@ -510,29 +510,36 @@
         f.write("{}\n".format(output))
     return None
 
 
 
 
 def write_in_file(string_to_write,outdir_or_outpath,
-                  outname="",ext='.txt',encoding='utf8'):
+                  outname="",ext='.txt',encoding='utf8',append=False):
     """
     encoding : utf8, latin_1
     https://docs.python.org/3/library/codecs.html#standard-encodings
     
     check the following commented old version if troubles
     """
     
     if outname:
         outpath = os.path.join(outdir_or_outpath,outname + ext)
     else:
         outpath = outdir_or_outpath
         
-    F = open(outpath,'w+',encoding=encoding)
-    F.write(string_to_write)
+    if append:
+        aw = "a+"
+        newline = "\n"
+    else:
+        aw = "w+"
+        newline = ""
+        
+    F = open(outpath,aw,encoding=encoding)
+    F.write(string_to_write + newline)
     F.close()
     return outpath
 
 # def write_in_file(string_to_write,outdir,outname,ext='.txt',encoding='utf8'):
 #     """
 
 #     encoding : utf8, latin_1
```

### Comparing `geodezyx-0.4.3.2/geodezyx/utils/utils_core.py` & `geodezyx-0.4.3.3/geodezyx/utils/utils_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 import io
 #### geodeZYX modules
 
 #### Import the logger
 import logging
 log = logging.getLogger(__name__)
 
-
 ##########  END IMPORT  ##########
 
 
 
 def clear_all():
     '''Clears all the variables from the workspace of the spyder
     application.'''
@@ -888,15 +887,19 @@
         return list(string.ascii_lowercase)
     else:
         return alphabet_reverse().index(letter)
 
 
 def dday():
     D = (dt.datetime(2016,10,14) - dt.datetime.now()).days
-    print('J -',  D , 'avant la quille')
+    print("used logger:",log)
+    log.warning('J - %s avant la quille !!!',D)
+    log.info('J - %s avant la quille',D)
+    log.debug('J - %s avant la quille, chill',D)
+            
     return D
 
 def Aformat(A,landscape=True):
     LA = [(841 , 1189),
     (594 , 841),
     (420 , 594),
     (297 , 420),
```

### Comparing `geodezyx-0.4.3.2/geodezyx.egg-info/PKG-INFO` & `geodezyx-0.4.3.3/geodezyx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodezyx
-Version: 0.4.3.2
+Version: 0.4.3.3
 Summary: The GeodeZYX toolbox aims to provide simple but useful functions for Geodesy and Geophysics.
 Home-page: https://github.com/GeodeZYX/geodezyx-toolbox
 Author: Pierre Sakic & Gustavo Mansur
 Author-email: pierre.sakic@gfz-potsdam.de
 Keywords: geodesy,geophysics,reference frames,gnss
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `geodezyx-0.4.3.2/geodezyx.egg-info/SOURCES.txt` & `geodezyx-0.4.3.3/geodezyx.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -30,19 +30,22 @@
 geodezyx/files_rw/read_geo_files_misc.py
 geodezyx/files_rw/read_gnss_prods.py
 geodezyx/files_rw/read_igs_combi.py
 geodezyx/files_rw/read_logsheets.py
 geodezyx/files_rw/read_rinex.py
 geodezyx/files_rw/read_slr.py
 geodezyx/files_rw/write_geo_files.py
+geodezyx/files_rw/write_rinex.py
 geodezyx/geodyn/__init__.py
 geodezyx/geodyn/emsgfz_load_interp.py
 geodezyx/geodyn/euler_pole_calc.py
 geodezyx/geodyn/velo_field_map_plt.py
 geodezyx/geodyn/volcano_mogi.py
+geodezyx/logconfig/__init__.py
+geodezyx/logconfig/loggzyx.py
 geodezyx/marine/__init__.py
 geodezyx/marine/marine.py
 geodezyx/marine/oseanpres_lib.py
 geodezyx/megalib/__init__.py
 geodezyx/megalib/genefun.py
 geodezyx/megalib/geo_files_converter_lib.py
 geodezyx/megalib/geoclass.py
@@ -72,14 +75,15 @@
 geodezyx/reffram/kepler_gzyx.py
 geodezyx/reffram/quaternions.py
 geodezyx/stats/__init__.py
 geodezyx/stats/least_squares.py
 geodezyx/stats/stats.py
 geodezyx/time_series/__init__.py
 geodezyx/time_series/ts_class.py
+geodezyx/time_series/ts_export.py
 geodezyx/time_series/ts_fcts.py
 geodezyx/toolbox_meta/__init__.py
 geodezyx/utils/__init__.py
 geodezyx/utils/dict_utils.py
 geodezyx/utils/list_utils.py
 geodezyx/utils/pandas_utils.py
 geodezyx/utils/plot_utils.py
```

### Comparing `geodezyx-0.4.3.2/misc/import_generic.py` & `geodezyx-0.4.3.3/misc/import_generic.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/misc/refactoring.py` & `geodezyx-0.4.3.3/misc/refactoring.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.2/setup.py` & `geodezyx-0.4.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.4.3.2',  # Required
+    version='0.4.3.3',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='The GeodeZYX toolbox aims to provide simple but useful functions for Geodesy and Geophysics.',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -157,14 +157,15 @@
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=['bs4',
                       'collection',
+                      'colorlog',
                       #'ftplib',
                       #'kepler.py',
                       'natsort',
                       'matplotlib',
                       #'ncompress',
                       'numpy',
                       #'netCDF4',
```

