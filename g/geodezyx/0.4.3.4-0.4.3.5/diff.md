# Comparing `tmp/geodezyx-0.4.3.4.tar.gz` & `tmp/geodezyx-0.4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodezyx-0.4.3.4.tar", last modified: Fri Jun 30 12:37:50 2023, max compression
+gzip compressed data, was "geodezyx-0.4.3.5.tar", last modified: Fri Jun 30 13:19:05 2023, max compression
```

## Comparing `geodezyx-0.4.3.4.tar` & `geodezyx-0.4.3.5.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.730686 geodezyx-0.4.3.4/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    35150 2023-01-16 18:09:24.000000 geodezyx-0.4.3.4/LICENSE
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1562 2023-06-30 12:37:50.730686 geodezyx-0.4.3.4/PKG-INFO
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5074 2023-06-30 12:37:35.000000 geodezyx-0.4.3.4/README.md
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.698686 geodezyx-0.4.3.4/geodezyx/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2152 2023-05-31 13:51:35.000000 geodezyx-0.4.3.4/geodezyx/__init__.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.698686 geodezyx-0.4.3.4/geodezyx/athmo/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       21 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/athmo/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30462 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/athmo/athmo.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.702685 geodezyx-0.4.3.4/geodezyx/conv/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      344 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/conv/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9008 2023-04-27 16:56:08.000000 geodezyx-0.4.3.4/geodezyx/conv/conv_angle.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    23357 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/conv/conv_coords.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9551 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/conv/conv_geometric.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5908 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/conv/conv_interpolators.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3891 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/conv/conv_proj_lambert.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6574 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/conv/conv_proj_utm.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10244 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/conv/conv_rinex.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    12038 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/conv/conv_rotation_matrices.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79808 2023-05-31 13:56:13.000000 geodezyx-0.4.3.4/geodezyx/conv/conv_time.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.702685 geodezyx-0.4.3.4/geodezyx/externlib/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1354 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/externlib/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      763 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/externlib/externlib.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.714686 geodezyx-0.4.3.4/geodezyx/files_rw/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      556 2023-04-23 11:48:52.000000 geodezyx-0.4.3.4/geodezyx/files_rw/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    80903 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/files_rw/geo_files_converter_lib.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9417 2023-04-07 15:57:22.000000 geodezyx-0.4.3.4/geodezyx/files_rw/read_athmo.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     4812 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/files_rw/read_coords_misc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    77264 2023-06-09 15:48:46.000000 geodezyx-0.4.3.4/geodezyx/files_rw/read_coords_time_series.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    19068 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/files_rw/read_eop.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    28668 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/files_rw/read_geo_files_misc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    16650 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/files_rw/read_gnss_prods.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     8729 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/files_rw/read_igs_combi.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    18124 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/files_rw/read_logsheets.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14535 2023-04-23 18:42:34.000000 geodezyx-0.4.3.4/geodezyx/files_rw/read_rinex.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2825 2023-04-07 15:57:22.000000 geodezyx-0.4.3.4/geodezyx/files_rw/read_slr.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    37801 2023-05-31 13:56:43.000000 geodezyx-0.4.3.4/geodezyx/files_rw/write_geo_files.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6437 2023-06-06 10:47:42.000000 geodezyx-0.4.3.4/geodezyx/files_rw/write_rinex.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.714686 geodezyx-0.4.3.4/geodezyx/geodyn/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      102 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/geodyn/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10146 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/geodyn/emsgfz_load_interp.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13599 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/geodyn/euler_pole_calc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    27578 2023-06-30 12:19:55.000000 geodezyx-0.4.3.4/geodezyx/geodyn/velo_field_map_plt.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5317 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/geodyn/volcano_mogi.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.714686 geodezyx-0.4.3.4/geodezyx/logconfig/
--rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       80 2023-04-07 18:12:57.000000 geodezyx-0.4.3.4/geodezyx/logconfig/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2009 2023-06-11 20:05:07.000000 geodezyx-0.4.3.4/geodezyx/logconfig/loggzyx.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.714686 geodezyx-0.4.3.4/geodezyx/marine/
--rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)      109 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/marine/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2590 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/marine/marine.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10788 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/marine/oseanpres_lib.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.718685 geodezyx-0.4.3.4/geodezyx/megalib/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      153 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/megalib/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      139 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/megalib/genefun.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      295 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/megalib/geo_files_converter_lib.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      571 2023-05-12 13:59:17.000000 geodezyx-0.4.3.4/geodezyx/megalib/geoclass.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      334 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/megalib/geodetik.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      408 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/megalib/megalib.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      720 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/megalib/softs_runner.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.722685 geodezyx-0.4.3.4/geodezyx/operational/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      635 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/operational/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9590 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/operational/anubis_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7448 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/operational/cluster_gfz.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7021 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/operational/download_cddis.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6743 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/operational/download_dropbox.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    12881 2023-06-02 09:08:37.000000 geodezyx-0.4.3.4/geodezyx/operational/download_find_files.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    32777 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/operational/download_prods.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17730 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/operational/download_rinex.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    11251 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/operational/download_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79440 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/operational/gins_runner.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    21977 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/operational/groops_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    15766 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/operational/hector_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7930 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/operational/midas_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    26040 2023-06-02 08:02:32.000000 geodezyx-0.4.3.4/geodezyx/operational/rinex_lister_plotter.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    31955 2023-05-31 13:56:13.000000 geodezyx-0.4.3.4/geodezyx/operational/rinex_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7075 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/operational/rtklib_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9160 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/operational/track_frontend.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.722685 geodezyx-0.4.3.4/geodezyx/reffram/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      107 2023-04-07 15:57:22.000000 geodezyx-0.4.3.4/geodezyx/reffram/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    43633 2023-06-30 12:09:16.000000 geodezyx-0.4.3.4/geodezyx/reffram/geometry.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    56868 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/reffram/gnss_products.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7243 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/reffram/kepler_gzyx.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3879 2023-04-07 15:57:22.000000 geodezyx-0.4.3.4/geodezyx/reffram/quaternions.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.726686 geodezyx-0.4.3.4/geodezyx/stats/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       50 2023-04-07 15:57:22.000000 geodezyx-0.4.3.4/geodezyx/stats/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30960 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/stats/least_squares.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    43987 2023-06-22 13:52:44.000000 geodezyx-0.4.3.4/geodezyx/stats/stats.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.726686 geodezyx-0.4.3.4/geodezyx/time_series/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       97 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/time_series/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    48361 2023-06-23 09:38:51.000000 geodezyx-0.4.3.4/geodezyx/time_series/ts_class.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17296 2023-06-28 15:28:03.000000 geodezyx-0.4.3.4/geodezyx/time_series/ts_export.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    35307 2023-06-22 13:50:24.000000 geodezyx-0.4.3.4/geodezyx/time_series/ts_fcts.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.726686 geodezyx-0.4.3.4/geodezyx/toolbox_meta/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       96 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/toolbox_meta/__init__.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.726686 geodezyx-0.4.3.4/geodezyx/utils/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      242 2023-04-07 15:57:22.000000 geodezyx-0.4.3.4/geodezyx/utils/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2026 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/utils/dict_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13518 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/utils/list_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3637 2023-04-07 15:57:23.000000 geodezyx-0.4.3.4/geodezyx/utils/pandas_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7260 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/utils/plot_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17975 2023-04-07 16:22:38.000000 geodezyx-0.4.3.4/geodezyx/utils/shell_like.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    24926 2023-06-28 15:58:55.000000 geodezyx-0.4.3.4/geodezyx/utils/utils_core.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.698686 geodezyx-0.4.3.4/geodezyx.egg-info/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1562 2023-06-30 12:37:50.000000 geodezyx-0.4.3.4/geodezyx.egg-info/PKG-INFO
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3006 2023-06-30 12:37:50.000000 geodezyx-0.4.3.4/geodezyx.egg-info/SOURCES.txt
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)        1 2023-06-30 12:37:50.000000 geodezyx-0.4.3.4/geodezyx.egg-info/dependency_links.txt
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      185 2023-06-30 12:37:50.000000 geodezyx-0.4.3.4/geodezyx.egg-info/requires.txt
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       14 2023-06-30 12:37:50.000000 geodezyx-0.4.3.4/geodezyx.egg-info/top_level.txt
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 12:37:50.730686 geodezyx-0.4.3.4/misc/
--rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       98 2022-12-02 23:12:26.000000 geodezyx-0.4.3.4/misc/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1225 2021-06-22 11:51:35.000000 geodezyx-0.4.3.4/misc/import_generic.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3778 2023-01-16 18:09:24.000000 geodezyx-0.4.3.4/misc/refactoring.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       38 2023-06-30 12:37:50.730686 geodezyx-0.4.3.4/setup.cfg
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10227 2023-06-30 12:35:38.000000 geodezyx-0.4.3.4/setup.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.464567 geodezyx-0.4.3.5/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    35150 2023-01-16 18:09:24.000000 geodezyx-0.4.3.5/LICENSE
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1562 2023-06-30 13:19:05.464567 geodezyx-0.4.3.5/PKG-INFO
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5086 2023-06-30 13:18:46.000000 geodezyx-0.4.3.5/README.md
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.436567 geodezyx-0.4.3.5/geodezyx/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2152 2023-05-31 13:51:35.000000 geodezyx-0.4.3.5/geodezyx/__init__.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.440567 geodezyx-0.4.3.5/geodezyx/athmo/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       21 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/athmo/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30462 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/athmo/athmo.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.440567 geodezyx-0.4.3.5/geodezyx/conv/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      344 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/conv/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9008 2023-04-27 16:56:08.000000 geodezyx-0.4.3.5/geodezyx/conv/conv_angle.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    23357 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/conv/conv_coords.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9551 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/conv/conv_geometric.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5908 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/conv/conv_interpolators.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3891 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/conv/conv_proj_lambert.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6574 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/conv/conv_proj_utm.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10244 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/conv/conv_rinex.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    12038 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/conv/conv_rotation_matrices.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79808 2023-05-31 13:56:13.000000 geodezyx-0.4.3.5/geodezyx/conv/conv_time.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.444567 geodezyx-0.4.3.5/geodezyx/externlib/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1354 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/externlib/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      763 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/externlib/externlib.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.448567 geodezyx-0.4.3.5/geodezyx/files_rw/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      556 2023-04-23 11:48:52.000000 geodezyx-0.4.3.5/geodezyx/files_rw/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    80903 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/files_rw/geo_files_converter_lib.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9417 2023-04-07 15:57:22.000000 geodezyx-0.4.3.5/geodezyx/files_rw/read_athmo.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     4812 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/files_rw/read_coords_misc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    77264 2023-06-09 15:48:46.000000 geodezyx-0.4.3.5/geodezyx/files_rw/read_coords_time_series.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    19068 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/files_rw/read_eop.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    28668 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/files_rw/read_geo_files_misc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    16650 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/files_rw/read_gnss_prods.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     8729 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/files_rw/read_igs_combi.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    18124 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/files_rw/read_logsheets.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14535 2023-04-23 18:42:34.000000 geodezyx-0.4.3.5/geodezyx/files_rw/read_rinex.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2825 2023-04-07 15:57:22.000000 geodezyx-0.4.3.5/geodezyx/files_rw/read_slr.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    37801 2023-05-31 13:56:43.000000 geodezyx-0.4.3.5/geodezyx/files_rw/write_geo_files.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6437 2023-06-06 10:47:42.000000 geodezyx-0.4.3.5/geodezyx/files_rw/write_rinex.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.448567 geodezyx-0.4.3.5/geodezyx/geodyn/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      102 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/geodyn/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10146 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/geodyn/emsgfz_load_interp.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13599 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/geodyn/euler_pole_calc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    27578 2023-06-30 12:19:55.000000 geodezyx-0.4.3.5/geodezyx/geodyn/velo_field_map_plt.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5317 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/geodyn/volcano_mogi.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.448567 geodezyx-0.4.3.5/geodezyx/logconfig/
+-rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       80 2023-04-07 18:12:57.000000 geodezyx-0.4.3.5/geodezyx/logconfig/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2009 2023-06-11 20:05:07.000000 geodezyx-0.4.3.5/geodezyx/logconfig/loggzyx.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.448567 geodezyx-0.4.3.5/geodezyx/marine/
+-rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)      109 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/marine/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2590 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/marine/marine.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10788 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/marine/oseanpres_lib.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.452567 geodezyx-0.4.3.5/geodezyx/megalib/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      153 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/megalib/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      139 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/megalib/genefun.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      295 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/megalib/geo_files_converter_lib.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      571 2023-05-12 13:59:17.000000 geodezyx-0.4.3.5/geodezyx/megalib/geoclass.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      334 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/megalib/geodetik.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      408 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/megalib/megalib.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      720 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/megalib/softs_runner.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.456567 geodezyx-0.4.3.5/geodezyx/operational/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      635 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/operational/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9590 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/operational/anubis_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7448 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/operational/cluster_gfz.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7021 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/operational/download_cddis.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6743 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/operational/download_dropbox.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    12881 2023-06-02 09:08:37.000000 geodezyx-0.4.3.5/geodezyx/operational/download_find_files.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    32777 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/operational/download_prods.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17730 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/operational/download_rinex.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    11251 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/operational/download_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79440 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/operational/gins_runner.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    21977 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/operational/groops_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    15766 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/operational/hector_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7930 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/operational/midas_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    26040 2023-06-02 08:02:32.000000 geodezyx-0.4.3.5/geodezyx/operational/rinex_lister_plotter.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    31955 2023-05-31 13:56:13.000000 geodezyx-0.4.3.5/geodezyx/operational/rinex_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7075 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/operational/rtklib_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9160 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/operational/track_frontend.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.456567 geodezyx-0.4.3.5/geodezyx/reffram/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      107 2023-04-07 15:57:22.000000 geodezyx-0.4.3.5/geodezyx/reffram/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    43633 2023-06-30 12:09:16.000000 geodezyx-0.4.3.5/geodezyx/reffram/geometry.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    56868 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/reffram/gnss_products.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7243 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/reffram/kepler_gzyx.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3879 2023-04-07 15:57:22.000000 geodezyx-0.4.3.5/geodezyx/reffram/quaternions.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.456567 geodezyx-0.4.3.5/geodezyx/stats/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       50 2023-04-07 15:57:22.000000 geodezyx-0.4.3.5/geodezyx/stats/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30960 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/stats/least_squares.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    43987 2023-06-22 13:52:44.000000 geodezyx-0.4.3.5/geodezyx/stats/stats.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.460567 geodezyx-0.4.3.5/geodezyx/time_series/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       97 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/time_series/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    48361 2023-06-23 09:38:51.000000 geodezyx-0.4.3.5/geodezyx/time_series/ts_class.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17296 2023-06-28 15:28:03.000000 geodezyx-0.4.3.5/geodezyx/time_series/ts_export.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    35307 2023-06-22 13:50:24.000000 geodezyx-0.4.3.5/geodezyx/time_series/ts_fcts.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.460567 geodezyx-0.4.3.5/geodezyx/toolbox_meta/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       96 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/toolbox_meta/__init__.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.460567 geodezyx-0.4.3.5/geodezyx/utils/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      242 2023-04-07 15:57:22.000000 geodezyx-0.4.3.5/geodezyx/utils/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2026 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/utils/dict_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13518 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/utils/list_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3637 2023-04-07 15:57:23.000000 geodezyx-0.4.3.5/geodezyx/utils/pandas_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7260 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/utils/plot_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17975 2023-04-07 16:22:38.000000 geodezyx-0.4.3.5/geodezyx/utils/shell_like.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    24926 2023-06-28 15:58:55.000000 geodezyx-0.4.3.5/geodezyx/utils/utils_core.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.440567 geodezyx-0.4.3.5/geodezyx.egg-info/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1562 2023-06-30 13:19:05.000000 geodezyx-0.4.3.5/geodezyx.egg-info/PKG-INFO
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3006 2023-06-30 13:19:05.000000 geodezyx-0.4.3.5/geodezyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)        1 2023-06-30 13:19:05.000000 geodezyx-0.4.3.5/geodezyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      186 2023-06-30 13:19:05.000000 geodezyx-0.4.3.5/geodezyx.egg-info/requires.txt
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       14 2023-06-30 13:19:05.000000 geodezyx-0.4.3.5/geodezyx.egg-info/top_level.txt
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2023-06-30 13:19:05.464567 geodezyx-0.4.3.5/misc/
+-rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       98 2022-12-02 23:12:26.000000 geodezyx-0.4.3.5/misc/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1225 2021-06-22 11:51:35.000000 geodezyx-0.4.3.5/misc/import_generic.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3778 2023-01-16 18:09:24.000000 geodezyx-0.4.3.5/misc/refactoring.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       38 2023-06-30 13:19:05.464567 geodezyx-0.4.3.5/setup.cfg
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10228 2023-06-30 13:19:02.000000 geodezyx-0.4.3.5/setup.py
```

### Comparing `geodezyx-0.4.3.4/LICENSE` & `geodezyx-0.4.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/PKG-INFO` & `geodezyx-0.4.3.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodezyx
-Version: 0.4.3.4
+Version: 0.4.3.5
 Summary: The GeodeZYX toolbox aims to provide simple but useful functions for Geodesy and Geophysics.
 Home-page: https://github.com/GeodeZYX/geodezyx-toolbox
 Author: Pierre Sakic & Gustavo Mansur
 Author-email: sakic@ipgp.fr
 Keywords: geodesy,geophysics,reference frames,gnss
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `geodezyx-0.4.3.4/README.md` & `geodezyx-0.4.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <img src="./geodezyx_toolbox_logo.png" width="300">
 
 # GeodeZYX Toolbox
 
-**Version 0.4.3.4 / 2023-06-30**, README Revision: 2023-06-30
+**Version 0.4.3.5 / 2023-06-30**, README Revision: 2023-06-30
 
 
 **Authors:** Pierre Sakic (IPGP, Paris, France), Gustavo Mansur, and Kitpracha "Na" Chaiyaporn
 (GFZ, Potsdam, Germany), with contributions from Valérie Ballu (CNRS/La Rochelle University, France)
 
 **Documentation:** [https://geodezyx.github.io/geodezyx-toolbox](https://geodezyx.github.io/geodezyx-toolbox/)
 
@@ -64,18 +64,18 @@
 
 and install the Toolbox you downloaded with ``python setup.py install``
 
 Alternatively, you can also add the ``geodezyx`` folder in your ``PYTHONPATH`` (for experimented users)
 
 ## Changelog
 
-### v0.4.3.4, 2023-06-30
+### v0.4.3.5, 2023-06-30
   * a routine version update (bug corrections...)
   * colors in the logger
-  * NB: v0.4.3.4 replaces the v0.4.3.3 (cancelled release)
+  * NB: v0.4.3.5 replaces the v0.4.3.4 & v0.4.3.3 (cancelled releases)
 
 ### v0.4.3.2, 2023-03-08
   * 1000th commit on GitHub 🥳
   * GitHub repository is renamed for simplification 
     * `GeodeZYX-Toolbox_v4` becomes `geodezyx-toolbox` (lowercase and without version)
     * It must be transparent for your clones but updating them is recommended \
       https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository
```

### Comparing `geodezyx-0.4.3.4/geodezyx/__init__.py` & `geodezyx-0.4.3.5/geodezyx/__init__.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/athmo/athmo.py` & `geodezyx-0.4.3.5/geodezyx/athmo/athmo.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/conv/conv_angle.py` & `geodezyx-0.4.3.5/geodezyx/conv/conv_angle.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/conv/conv_coords.py` & `geodezyx-0.4.3.5/geodezyx/conv/conv_coords.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/conv/conv_geometric.py` & `geodezyx-0.4.3.5/geodezyx/conv/conv_geometric.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/conv/conv_interpolators.py` & `geodezyx-0.4.3.5/geodezyx/conv/conv_interpolators.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/conv/conv_proj_lambert.py` & `geodezyx-0.4.3.5/geodezyx/conv/conv_proj_lambert.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/conv/conv_proj_utm.py` & `geodezyx-0.4.3.5/geodezyx/conv/conv_proj_utm.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/conv/conv_rinex.py` & `geodezyx-0.4.3.5/geodezyx/conv/conv_rinex.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/conv/conv_rotation_matrices.py` & `geodezyx-0.4.3.5/geodezyx/conv/conv_rotation_matrices.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/conv/conv_time.py` & `geodezyx-0.4.3.5/geodezyx/conv/conv_time.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/externlib/__init__.py` & `geodezyx-0.4.3.5/geodezyx/externlib/__init__.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/externlib/externlib.py` & `geodezyx-0.4.3.5/geodezyx/externlib/externlib.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/__init__.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/__init__.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/geo_files_converter_lib.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/geo_files_converter_lib.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/read_athmo.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/read_athmo.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/read_coords_misc.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/read_coords_misc.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/read_coords_time_series.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/read_coords_time_series.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/read_eop.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/read_eop.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/read_geo_files_misc.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/read_geo_files_misc.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/read_gnss_prods.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/read_gnss_prods.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/read_igs_combi.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/read_igs_combi.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/read_logsheets.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/read_logsheets.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/read_rinex.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/read_rinex.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/read_slr.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/read_slr.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/write_geo_files.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/write_geo_files.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/files_rw/write_rinex.py` & `geodezyx-0.4.3.5/geodezyx/files_rw/write_rinex.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/geodyn/emsgfz_load_interp.py` & `geodezyx-0.4.3.5/geodezyx/geodyn/emsgfz_load_interp.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/geodyn/euler_pole_calc.py` & `geodezyx-0.4.3.5/geodezyx/geodyn/euler_pole_calc.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/geodyn/velo_field_map_plt.py` & `geodezyx-0.4.3.5/geodezyx/geodyn/velo_field_map_plt.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/geodyn/volcano_mogi.py` & `geodezyx-0.4.3.5/geodezyx/geodyn/volcano_mogi.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/logconfig/loggzyx.py` & `geodezyx-0.4.3.5/geodezyx/logconfig/loggzyx.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/marine/marine.py` & `geodezyx-0.4.3.5/geodezyx/marine/marine.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/marine/oseanpres_lib.py` & `geodezyx-0.4.3.5/geodezyx/marine/oseanpres_lib.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/megalib/geoclass.py` & `geodezyx-0.4.3.5/geodezyx/megalib/geoclass.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/megalib/softs_runner.py` & `geodezyx-0.4.3.5/geodezyx/megalib/softs_runner.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/__init__.py` & `geodezyx-0.4.3.5/geodezyx/operational/__init__.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/anubis_frontend.py` & `geodezyx-0.4.3.5/geodezyx/operational/anubis_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/cluster_gfz.py` & `geodezyx-0.4.3.5/geodezyx/operational/cluster_gfz.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/download_cddis.py` & `geodezyx-0.4.3.5/geodezyx/operational/download_cddis.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/download_dropbox.py` & `geodezyx-0.4.3.5/geodezyx/operational/download_dropbox.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/download_find_files.py` & `geodezyx-0.4.3.5/geodezyx/operational/download_find_files.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/download_prods.py` & `geodezyx-0.4.3.5/geodezyx/operational/download_prods.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/download_rinex.py` & `geodezyx-0.4.3.5/geodezyx/operational/download_rinex.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/download_utils.py` & `geodezyx-0.4.3.5/geodezyx/operational/download_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/gins_runner.py` & `geodezyx-0.4.3.5/geodezyx/operational/gins_runner.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/groops_frontend.py` & `geodezyx-0.4.3.5/geodezyx/operational/groops_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/hector_frontend.py` & `geodezyx-0.4.3.5/geodezyx/operational/hector_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/midas_frontend.py` & `geodezyx-0.4.3.5/geodezyx/operational/midas_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/rinex_lister_plotter.py` & `geodezyx-0.4.3.5/geodezyx/operational/rinex_lister_plotter.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/rinex_utils.py` & `geodezyx-0.4.3.5/geodezyx/operational/rinex_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/rtklib_frontend.py` & `geodezyx-0.4.3.5/geodezyx/operational/rtklib_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/operational/track_frontend.py` & `geodezyx-0.4.3.5/geodezyx/operational/track_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/reffram/geometry.py` & `geodezyx-0.4.3.5/geodezyx/reffram/geometry.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/reffram/gnss_products.py` & `geodezyx-0.4.3.5/geodezyx/reffram/gnss_products.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/reffram/kepler_gzyx.py` & `geodezyx-0.4.3.5/geodezyx/reffram/kepler_gzyx.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/reffram/quaternions.py` & `geodezyx-0.4.3.5/geodezyx/reffram/quaternions.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/stats/least_squares.py` & `geodezyx-0.4.3.5/geodezyx/stats/least_squares.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/stats/stats.py` & `geodezyx-0.4.3.5/geodezyx/stats/stats.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/time_series/ts_class.py` & `geodezyx-0.4.3.5/geodezyx/time_series/ts_class.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/time_series/ts_export.py` & `geodezyx-0.4.3.5/geodezyx/time_series/ts_export.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/time_series/ts_fcts.py` & `geodezyx-0.4.3.5/geodezyx/time_series/ts_fcts.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/utils/dict_utils.py` & `geodezyx-0.4.3.5/geodezyx/utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/utils/list_utils.py` & `geodezyx-0.4.3.5/geodezyx/utils/list_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/utils/pandas_utils.py` & `geodezyx-0.4.3.5/geodezyx/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/utils/plot_utils.py` & `geodezyx-0.4.3.5/geodezyx/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/utils/shell_like.py` & `geodezyx-0.4.3.5/geodezyx/utils/shell_like.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx/utils/utils_core.py` & `geodezyx-0.4.3.5/geodezyx/utils/utils_core.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/geodezyx.egg-info/PKG-INFO` & `geodezyx-0.4.3.5/geodezyx.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodezyx
-Version: 0.4.3.4
+Version: 0.4.3.5
 Summary: The GeodeZYX toolbox aims to provide simple but useful functions for Geodesy and Geophysics.
 Home-page: https://github.com/GeodeZYX/geodezyx-toolbox
 Author: Pierre Sakic & Gustavo Mansur
 Author-email: sakic@ipgp.fr
 Keywords: geodesy,geophysics,reference frames,gnss
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `geodezyx-0.4.3.4/geodezyx.egg-info/SOURCES.txt` & `geodezyx-0.4.3.5/geodezyx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/misc/import_generic.py` & `geodezyx-0.4.3.5/misc/import_generic.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/misc/refactoring.py` & `geodezyx-0.4.3.5/misc/refactoring.py`

 * *Files identical despite different names*

### Comparing `geodezyx-0.4.3.4/setup.py` & `geodezyx-0.4.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.4.3.4',  # Required
+    version='0.4.3.5',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='The GeodeZYX toolbox aims to provide simple but useful functions for Geodesy and Geophysics.',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -159,15 +159,15 @@
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=['bs4',
                       'collection',
                       'colorlog',
                       #'ftplib',
-                      'hatanka',
+                      'hatanaka',
                       #'kepler.py',
                       'natsort',
                       'matplotlib',
                       #'ncompress',
                       'numpy',
                       #'netCDF4',
                       'pybind11',
```

