# Comparing `tmp/fooof-1.0.0rc3.tar.gz` & `tmp/fooof-1.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fooof-1.0.0rc3.tar", last modified: Thu Apr  9 06:01:48 2020, max compression
+gzip compressed data, was "dist/fooof-1.1.0rc0.tar", last modified: Fri Jun 30 19:07:34 2023, max compression
```

## Comparing `fooof-1.0.0rc3.tar` & `fooof-1.1.0rc0.tar`

### file list

```diff
@@ -1,122 +1,126 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/
--rw-r--r--   0 tom        (501) staff       (20)    11340 2019-01-23 01:14:03.000000 fooof-1.0.0rc3/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       16 2019-01-23 01:14:03.000000 fooof-1.0.0rc3/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)     3016 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     9808 2020-03-19 03:42:27.000000 fooof-1.0.0rc3/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/
--rw-r--r--   0 tom        (501) staff       (20)      181 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/analysis/
--rw-r--r--   0 tom        (501) staff       (20)      205 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/analysis/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3462 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/analysis/error.py
--rw-r--r--   0 tom        (501) staff       (20)     7456 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/analysis/periodic.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/bands/
--rw-r--r--   0 tom        (501) staff       (20)       60 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/bands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3923 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/bands/bands.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/core/
--rw-r--r--   0 tom        (501) staff       (20)       47 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/core/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      679 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/core/errors.py
--rw-r--r--   0 tom        (501) staff       (20)     5271 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/core/funcs.py
--rw-r--r--   0 tom        (501) staff       (20)     3859 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/core/info.py
--rw-r--r--   0 tom        (501) staff       (20)     8181 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/core/io.py
--rw-r--r--   0 tom        (501) staff       (20)      411 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/core/items.py
--rw-r--r--   0 tom        (501) staff       (20)     4689 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/core/modutils.py
--rw-r--r--   0 tom        (501) staff       (20)     3533 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/core/reports.py
--rw-r--r--   0 tom        (501) staff       (20)    14869 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/core/strings.py
--rw-r--r--   0 tom        (501) staff       (20)     6653 2020-04-07 21:47:32.000000 fooof-1.0.0rc3/fooof/core/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/data/
--rw-r--r--   0 tom        (501) staff       (20)      106 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/data/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     2691 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/data/data.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/objs/
--rw-r--r--   0 tom        (501) staff       (20)      217 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/objs/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    49971 2020-04-07 19:30:22.000000 fooof-1.0.0rc3/fooof/objs/fit.py
--rw-r--r--   0 tom        (501) staff       (20)    23753 2020-03-11 20:46:47.000000 fooof-1.0.0rc3/fooof/objs/group.py
--rw-r--r--   0 tom        (501) staff       (20)     7007 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/objs/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/plts/
--rw-r--r--   0 tom        (501) staff       (20)      295 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/plts/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    10122 2020-04-09 04:45:49.000000 fooof-1.0.0rc3/fooof/plts/annotate.py
--rw-r--r--   0 tom        (501) staff       (20)     5265 2020-03-24 21:18:58.000000 fooof-1.0.0rc3/fooof/plts/aperiodic.py
--rw-r--r--   0 tom        (501) staff       (20)     3635 2020-03-24 21:25:04.000000 fooof-1.0.0rc3/fooof/plts/fg.py
--rw-r--r--   0 tom        (501) staff       (20)    11542 2020-04-07 22:36:38.000000 fooof-1.0.0rc3/fooof/plts/fm.py
--rw-r--r--   0 tom        (501) staff       (20)     5635 2020-03-24 21:18:48.000000 fooof-1.0.0rc3/fooof/plts/periodic.py
--rw-r--r--   0 tom        (501) staff       (20)      714 2020-04-01 00:43:14.000000 fooof-1.0.0rc3/fooof/plts/settings.py
--rw-r--r--   0 tom        (501) staff       (20)     8572 2020-03-24 21:18:30.000000 fooof-1.0.0rc3/fooof/plts/spectra.py
--rw-r--r--   0 tom        (501) staff       (20)     2398 2020-04-01 00:21:07.000000 fooof-1.0.0rc3/fooof/plts/style.py
--rw-r--r--   0 tom        (501) staff       (20)     3747 2020-03-24 21:46:56.000000 fooof-1.0.0rc3/fooof/plts/templates.py
--rw-r--r--   0 tom        (501) staff       (20)     5093 2020-04-01 00:46:29.000000 fooof-1.0.0rc3/fooof/plts/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/sim/
--rw-r--r--   0 tom        (501) staff       (20)      419 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/sim/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    17323 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/sim/gen.py
--rw-r--r--   0 tom        (501) staff       (20)     9392 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/sim/params.py
--rw-r--r--   0 tom        (501) staff       (20)     7418 2020-03-25 18:23:35.000000 fooof-1.0.0rc3/fooof/sim/transform.py
--rw-r--r--   0 tom        (501) staff       (20)      468 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/sim/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/tests/
--rw-r--r--   0 tom        (501) staff       (20)       23 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/tests/analysis/
--rw-r--r--   0 tom        (501) staff       (20)        0 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/analysis/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      880 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/analysis/test_error.py
--rw-r--r--   0 tom        (501) staff       (20)     2616 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/analysis/test_periodic.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/tests/bands/
--rw-r--r--   0 tom        (501) staff       (20)        0 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/bands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1177 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/bands/test_bands.py
--rw-r--r--   0 tom        (501) staff       (20)     1423 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/conftest.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/tests/core/
--rw-r--r--   0 tom        (501) staff       (20)        0 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/core/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     2961 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/core/test_funcs.py
--rw-r--r--   0 tom        (501) staff       (20)     1485 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/core/test_info.py
--rw-r--r--   0 tom        (501) staff       (20)     5766 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/core/test_io.py
--rw-r--r--   0 tom        (501) staff       (20)     1288 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/core/test_modutils.py
--rw-r--r--   0 tom        (501) staff       (20)      766 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/core/test_reports.py
--rw-r--r--   0 tom        (501) staff       (20)     1355 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/core/test_strings.py
--rw-r--r--   0 tom        (501) staff       (20)     4128 2020-04-01 00:15:37.000000 fooof-1.0.0rc3/fooof/tests/core/test_utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/tests/data/
--rw-r--r--   0 tom        (501) staff       (20)        0 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/data/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1203 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/data/test_data.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/tests/objs/
--rw-r--r--   0 tom        (501) staff       (20)        0 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/objs/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    11950 2020-03-11 20:48:36.000000 fooof-1.0.0rc3/fooof/tests/objs/test_fit.py
--rw-r--r--   0 tom        (501) staff       (20)    10893 2020-03-11 20:47:28.000000 fooof-1.0.0rc3/fooof/tests/objs/test_group.py
--rw-r--r--   0 tom        (501) staff       (20)     4083 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/objs/test_utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/tests/plts/
--rw-r--r--   0 tom        (501) staff       (20)        0 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/plts/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      614 2020-04-07 22:56:18.000000 fooof-1.0.0rc3/fooof/tests/plts/test_annotate.py
--rw-r--r--   0 tom        (501) staff       (20)     1192 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/plts/test_aperiodic.py
--rw-r--r--   0 tom        (501) staff       (20)      832 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/plts/test_fg.py
--rw-r--r--   0 tom        (501) staff       (20)      807 2020-04-07 22:28:58.000000 fooof-1.0.0rc3/fooof/tests/plts/test_fm.py
--rw-r--r--   0 tom        (501) staff       (20)      855 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/plts/test_periodic.py
--rw-r--r--   0 tom        (501) staff       (20)     2011 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/plts/test_spectra.py
--rw-r--r--   0 tom        (501) staff       (20)      909 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/plts/test_styles.py
--rw-r--r--   0 tom        (501) staff       (20)      868 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/plts/test_templates.py
--rw-r--r--   0 tom        (501) staff       (20)     2112 2020-04-01 00:49:13.000000 fooof-1.0.0rc3/fooof/tests/plts/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)      483 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/settings.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/tests/sim/
--rw-r--r--   0 tom        (501) staff       (20)        0 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/sim/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4266 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/sim/test_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     4051 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/sim/test_params.py
--rw-r--r--   0 tom        (501) staff       (20)     2503 2020-03-25 18:22:57.000000 fooof-1.0.0rc3/fooof/tests/sim/test_transform.py
--rw-r--r--   0 tom        (501) staff       (20)      328 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/sim/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)     2096 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/tutils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/tests/utils/
--rw-r--r--   0 tom        (501) staff       (20)        0 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/utils/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1141 2020-03-25 14:47:21.000000 fooof-1.0.0rc3/fooof/tests/utils/test_data.py
--rw-r--r--   0 tom        (501) staff       (20)      315 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/utils/test_debug.py
--rw-r--r--   0 tom        (501) staff       (20)     1268 2020-03-19 03:42:27.000000 fooof-1.0.0rc3/fooof/tests/utils/test_download.py
--rw-r--r--   0 tom        (501) staff       (20)     1430 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/utils/test_io.py
--rw-r--r--   0 tom        (501) staff       (20)      575 2020-04-07 19:23:16.000000 fooof-1.0.0rc3/fooof/tests/utils/test_params.py
--rw-r--r--   0 tom        (501) staff       (20)      573 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/tests/utils/test_reports.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof/utils/
--rw-r--r--   0 tom        (501) staff       (20)      295 2020-03-25 14:47:31.000000 fooof-1.0.0rc3/fooof/utils/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4704 2020-03-25 16:58:25.000000 fooof-1.0.0rc3/fooof/utils/data.py
--rw-r--r--   0 tom        (501) staff       (20)      924 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/utils/debug.py
--rw-r--r--   0 tom        (501) staff       (20)     2421 2020-03-19 03:42:27.000000 fooof-1.0.0rc3/fooof/utils/download.py
--rw-r--r--   0 tom        (501) staff       (20)     1625 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/utils/io.py
--rw-r--r--   0 tom        (501) staff       (20)     1637 2020-04-07 19:28:45.000000 fooof-1.0.0rc3/fooof/utils/params.py
--rw-r--r--   0 tom        (501) staff       (20)     1675 2020-03-11 09:44:54.000000 fooof-1.0.0rc3/fooof/utils/reports.py
--rw-r--r--   0 tom        (501) staff       (20)       24 2020-03-13 03:52:09.000000 fooof-1.0.0rc3/fooof/version.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     3016 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     2553 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       85 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/fooof.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       79 2020-04-09 06:01:48.000000 fooof-1.0.0rc3/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     3545 2020-03-19 03:42:27.000000 fooof-1.0.0rc3/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.426153 fooof-1.1.0rc0/
+-rw-r--r--   0 tom        (501) staff       (20)    11340 2019-01-23 01:14:03.000000 fooof-1.1.0rc0/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       16 2019-01-23 01:14:03.000000 fooof-1.1.0rc0/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)    13337 2023-06-30 19:07:34.425744 fooof-1.1.0rc0/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    11796 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/README.rst
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.390298 fooof-1.1.0rc0/fooof/
+-rw-r--r--   0 tom        (501) staff       (20)      825 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.394756 fooof-1.1.0rc0/fooof/analysis/
+-rw-r--r--   0 tom        (501) staff       (20)      169 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/analysis/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3837 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/analysis/error.py
+-rw-r--r--   0 tom        (501) staff       (20)     9350 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/analysis/periodic.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.395706 fooof-1.1.0rc0/fooof/bands/
+-rw-r--r--   0 tom        (501) staff       (20)       60 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/bands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4091 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/bands/bands.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.399831 fooof-1.1.0rc0/fooof/core/
+-rw-r--r--   0 tom        (501) staff       (20)       47 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      616 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/errors.py
+-rw-r--r--   0 tom        (501) staff       (20)     5271 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/funcs.py
+-rw-r--r--   0 tom        (501) staff       (20)     3860 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/info.py
+-rw-r--r--   0 tom        (501) staff       (20)     8186 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/io.py
+-rw-r--r--   0 tom        (501) staff       (20)      411 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/items.py
+-rw-r--r--   0 tom        (501) staff       (20)     4703 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/modutils.py
+-rw-r--r--   0 tom        (501) staff       (20)     4766 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)    14913 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/strings.py
+-rw-r--r--   0 tom        (501) staff       (20)     6880 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.401025 fooof-1.1.0rc0/fooof/data/
+-rw-r--r--   0 tom        (501) staff       (20)      106 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/data/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3216 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/data/conversions.py
+-rw-r--r--   0 tom        (501) staff       (20)     3784 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/data/data.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.402455 fooof-1.1.0rc0/fooof/objs/
+-rw-r--r--   0 tom        (501) staff       (20)      217 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/objs/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    53885 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/objs/fit.py
+-rw-r--r--   0 tom        (501) staff       (20)    25446 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/objs/group.py
+-rw-r--r--   0 tom        (501) staff       (20)     8153 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/objs/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.406123 fooof-1.1.0rc0/fooof/plts/
+-rw-r--r--   0 tom        (501) staff       (20)      120 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    10159 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/annotate.py
+-rw-r--r--   0 tom        (501) staff       (20)     4754 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/aperiodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     1912 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/error.py
+-rw-r--r--   0 tom        (501) staff       (20)     4046 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/fg.py
+-rw-r--r--   0 tom        (501) staff       (20)    11410 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/fm.py
+-rw-r--r--   0 tom        (501) staff       (20)     5105 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/periodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     2027 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/settings.py
+-rw-r--r--   0 tom        (501) staff       (20)     7604 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/spectra.py
+-rw-r--r--   0 tom        (501) staff       (20)     8892 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/style.py
+-rw-r--r--   0 tom        (501) staff       (20)     3747 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/templates.py
+-rw-r--r--   0 tom        (501) staff       (20)     6682 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.408186 fooof-1.1.0rc0/fooof/sim/
+-rw-r--r--   0 tom        (501) staff       (20)      220 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/sim/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    17522 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/sim/gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     9749 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/sim/params.py
+-rw-r--r--   0 tom        (501) staff       (20)     9002 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/sim/transform.py
+-rw-r--r--   0 tom        (501) staff       (20)      468 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/sim/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.409456 fooof-1.1.0rc0/fooof/tests/
+-rw-r--r--   0 tom        (501) staff       (20)       23 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.410611 fooof-1.1.0rc0/fooof/tests/analysis/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/analysis/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1065 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/analysis/test_error.py
+-rw-r--r--   0 tom        (501) staff       (20)     2771 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/analysis/test_periodic.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.411303 fooof-1.1.0rc0/fooof/tests/bands/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/bands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1176 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/bands/test_bands.py
+-rw-r--r--   0 tom        (501) staff       (20)     1748 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/conftest.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.413500 fooof-1.1.0rc0/fooof/tests/core/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     2960 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_funcs.py
+-rw-r--r--   0 tom        (501) staff       (20)     1485 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_info.py
+-rw-r--r--   0 tom        (501) staff       (20)     5874 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_io.py
+-rw-r--r--   0 tom        (501) staff       (20)     1605 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_modutils.py
+-rw-r--r--   0 tom        (501) staff       (20)      766 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_reports.py
+-rw-r--r--   0 tom        (501) staff       (20)     1355 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_strings.py
+-rw-r--r--   0 tom        (501) staff       (20)     4127 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.414286 fooof-1.1.0rc0/fooof/tests/data/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/data/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1657 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/data/test_conversions.py
+-rw-r--r--   0 tom        (501) staff       (20)     1284 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/data/test_data.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.415642 fooof-1.1.0rc0/fooof/tests/objs/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/objs/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    14153 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/objs/test_fit.py
+-rw-r--r--   0 tom        (501) staff       (20)    11469 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/objs/test_group.py
+-rw-r--r--   0 tom        (501) staff       (20)     4261 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/objs/test_utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.419169 fooof-1.1.0rc0/fooof/tests/plts/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      895 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_annotate.py
+-rw-r--r--   0 tom        (501) staff       (20)     1461 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_aperiodic.py
+-rw-r--r--   0 tom        (501) staff       (20)      637 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_error.py
+-rw-r--r--   0 tom        (501) staff       (20)     1248 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_fg.py
+-rw-r--r--   0 tom        (501) staff       (20)      987 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_fm.py
+-rw-r--r--   0 tom        (501) staff       (20)     1104 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_periodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     4095 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_spectra.py
+-rw-r--r--   0 tom        (501) staff       (20)     2625 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_styles.py
+-rw-r--r--   0 tom        (501) staff       (20)      809 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_templates.py
+-rw-r--r--   0 tom        (501) staff       (20)     3396 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      544 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/settings.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.420603 fooof-1.1.0rc0/fooof/tests/sim/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/sim/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4266 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/sim/test_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     4050 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/sim/test_params.py
+-rw-r--r--   0 tom        (501) staff       (20)     2503 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/sim/test_transform.py
+-rw-r--r--   0 tom        (501) staff       (20)      328 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/sim/test_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     2513 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/tutils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.423155 fooof-1.1.0rc0/fooof/tests/utils/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     2831 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/test_data.py
+-rw-r--r--   0 tom        (501) staff       (20)      315 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/test_debug.py
+-rw-r--r--   0 tom        (501) staff       (20)     1268 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/test_download.py
+-rw-r--r--   0 tom        (501) staff       (20)     1430 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/test_io.py
+-rw-r--r--   0 tom        (501) staff       (20)      575 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/test_params.py
+-rw-r--r--   0 tom        (501) staff       (20)      573 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/test_reports.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.425260 fooof-1.1.0rc0/fooof/utils/
+-rw-r--r--   0 tom        (501) staff       (20)      112 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     6887 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/data.py
+-rw-r--r--   0 tom        (501) staff       (20)      924 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/debug.py
+-rw-r--r--   0 tom        (501) staff       (20)     2419 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/download.py
+-rw-r--r--   0 tom        (501) staff       (20)     1626 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/io.py
+-rw-r--r--   0 tom        (501) staff       (20)     1637 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/params.py
+-rw-r--r--   0 tom        (501) staff       (20)     1675 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)       24 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/version.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.393169 fooof-1.1.0rc0/fooof.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)    13337 2023-06-30 19:07:34.000000 fooof-1.1.0rc0/fooof.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     2658 2023-06-30 19:07:34.000000 fooof-1.1.0rc0/fooof.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-30 19:07:34.000000 fooof-1.1.0rc0/fooof.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      105 2023-06-30 19:07:34.000000 fooof-1.1.0rc0/fooof.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-06-30 19:07:34.000000 fooof-1.1.0rc0/fooof.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-30 19:07:34.426266 fooof-1.1.0rc0/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     2466 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fooof-1.0.0rc3/LICENSE` & `fooof-1.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/analysis/error.py` & `fooof-1.1.0rc0/fooof/analysis/error.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Functions to analyze and investigate FOOOF results - model fit error."""
 
 import numpy as np
 
 from fooof.sim.gen import gen_model
-from fooof.utils import compute_pointwise_error
-from fooof.plts.spectra import plot_spectrum_error
+from fooof.plts.error import plot_spectral_error
 from fooof.core.errors import NoModelError, NoDataError
 
 ###################################################################################################
 ###################################################################################################
 
 def compute_pointwise_error_fm(fm, plot_errors=True, return_errors=False, **plt_kwargs):
     """Calculate the frequency by frequency error of a model fit from a FOOOF object.
@@ -42,15 +41,15 @@
         raise NoDataError("Data must be available in the object to calculate errors.")
     if not fm.has_model:
         raise NoModelError("No model is available to use, can not proceed.")
 
     errors = compute_pointwise_error(fm.fooofed_spectrum_, fm.power_spectrum)
 
     if plot_errors:
-        plot_spectrum_error(fm.freqs, errors, **plt_kwargs)
+        plot_spectral_error(fm.freqs, errors, **plt_kwargs)
 
     if return_errors:
         return errors
 
 
 def compute_pointwise_error_fg(fg, plot_errors=True, return_errors=False, **plt_kwargs):
     """Calculate the frequency by frequency error of model fits from a FOOOFGroup object.
@@ -92,11 +91,30 @@
         model = gen_model(fg.freqs, res.aperiodic_params, res.gaussian_params)
         errors[ind, :] = np.abs(model - data)
 
     mean = np.mean(errors, 0)
     standard_dev = np.std(errors, 0)
 
     if plot_errors:
-        plot_spectrum_error(fg.freqs, mean, standard_dev, **plt_kwargs)
+        plot_spectral_error(fg.freqs, mean, standard_dev, **plt_kwargs)
 
     if return_errors:
         return errors
+
+
+def compute_pointwise_error(model, data):
+    """Calculate point-wise error between original data and a model fit of that data.
+
+    Parameters
+    ----------
+    model : 1d array
+        The model.
+    data : 1d array
+        The original data that is being modeled.
+
+    Returns
+    -------
+    1d array
+        Calculated values of the difference between the data and the model.
+    """
+
+    return np.abs(model - data)
```

### Comparing `fooof-1.0.0rc3/fooof/analysis/periodic.py` & `fooof-1.1.0rc0/fooof/analysis/periodic.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,65 +3,102 @@
 import numpy as np
 
 from fooof.core.items import PEAK_INDS
 
 ###################################################################################################
 ###################################################################################################
 
-def get_band_peak_fm(fm, band, ret_one=True, threshold=None, thresh_param='PW',
+def get_band_peak_fm(fm, band, select_highest=True, threshold=None, thresh_param='PW',
                      attribute='peak_params',):
     """Extract peaks from a band of interest from a FOOOF object.
 
     Parameters
     ----------
     fm : FOOOF
         Object to extract peak data from.
     band : tuple of (float, float)
         Frequency range for the band of interest.
-        Defind as: (lower_frequency_bound, upper_frequency_bound).
-    ret_one : bool, optional, default: True
+        Defined as: (lower_frequency_bound, upper_frequency_bound).
+    select_highest : bool, optional, default: True
         Whether to return single peak (if True) or all peaks within the range found (if False).
         If True, returns the highest power peak within the search range.
-    threshold : float
+    threshold : float, optional
         A minimum threshold value to apply.
     thresh_param : {'PW', 'BW'}
         Which parameter to threshold on. 'PW' is power and 'BW' is bandwidth.
     attribute : {'peak_params', 'gaussian_params'}
         Which attribute of peak data to extract data from.
 
     Returns
     -------
     1d or 2d array
-        Peak data. Each row is a peak, as [CF, PW, BW]
+        Peak data. Each row is a peak, as [CF, PW, BW].
+
+    Examples
+    --------
+    Select an alpha peak from an already fit FOOOF object 'fm', selecting the highest power alpha:
+
+    >>> alpha = get_band_peak_fm(fm, [7, 14], select_highest=True)  # doctest:+SKIP
+
+    Select beta peaks from a FOOOF object 'fm', extracting all peaks in the range:
+
+    >>> betas = get_band_peak_fm(fm, [13, 30], select_highest=False)  # doctest:+SKIP
     """
 
-    return get_band_peak(getattr(fm, attribute + '_'), band, ret_one, threshold, thresh_param)
+    return get_band_peak(getattr(fm, attribute + '_'), band,
+                         select_highest, threshold, thresh_param)
 
 
 def get_band_peak_fg(fg, band, threshold=None, thresh_param='PW', attribute='peak_params'):
     """Extract peaks from a band of interest from a FOOOFGroup object.
 
     Parameters
     ----------
     fg : FOOOFGroup
         Object to extract peak data from.
     band : tuple of (float, float)
         Frequency range for the band of interest.
-        Defind as: (lower_frequency_bound, upper_frequency_bound).
-    threshold : float
+        Defined as: (lower_frequency_bound, upper_frequency_bound).
+    threshold : float, optional
         A minimum threshold value to apply.
     thresh_param : {'PW', 'BW'}
         Which parameter to threshold on. 'PW' is power and 'BW' is bandwidth.
     attribute : {'peak_params', 'gaussian_params'}
         Which attribute of peak data to extract data from.
 
     Returns
     -------
     2d array
         Peak data. Each row is a peak, as [CF, PW, BW].
+        Each row represents an individual model from the input object.
+
+    Notes
+    -----
+    The returned array keeps track of which model each extracted peak comes from,
+    returning a [n_models, 3] array, with one peak returned per model.
+
+    - To do so, this function necessarily extracts and returns one peak per model fit.
+    - Each row reflects an individual model fit, in order, filled with nan if no peak was present.
+
+    If, instead, you wish to extract all peaks within a band, per model fit,
+    you can do something like:
+
+    >>> peaks = np.empty((0, 3))
+    >>> for f_res in fg:  # doctest:+SKIP
+    ...     peaks = np.vstack((peaks, get_band_peak(f_res.peak_params, band, select_highest=False)))
+
+    Examples
+    --------
+    Extract alpha peaks from a FOOOFGroup object 'fg' that already has model results:
+
+    >>> alphas = get_band_peak_fg(fg, [7, 14])  # doctest:+SKIP
+
+    Extract peaks from a FOOOFGroup object 'fg', selecting those above a power threshold:
+
+    >>> betas = get_band_peak_fg(fg, [13, 30], threshold=0.1)  # doctest:+SKIP
     """
 
     return get_band_peak_group(fg.get_params(attribute), band, len(fg),
                                threshold, thresh_param)
 
 
 def get_band_peak_group(peak_params, band, n_fits, threshold=None, thresh_param='PW'):
@@ -69,118 +106,117 @@
 
     Parameters
     ----------
     peak_params : 2d array
         Peak parameters, for a group fit, with shape of [n_peaks, 4].
     band : tuple of (float, float)
         Frequency range for the band of interest.
-        Defind as: (lower_frequency_bound, upper_frequency_bound).e
+        Defined as: (lower_frequency_bound, upper_frequency_bound).
     n_fits : int
         The number of model fits in the FOOOFGroup data.
-    threshold : float
+    threshold : float, optional
         A minimum threshold value to apply.
     thresh_param : {'PW', 'BW'}
         Which parameter to threshold on. 'PW' is power and 'BW' is bandwidth.
 
     Returns
     -------
     band_peaks : 2d array
         Peak data. Each row is a peak, as [CF, PW, BW].
+        Each row represents an individual model from the input array of all peaks.
 
     Notes
     -----
-    This function conserves the shape of the array, returning a [n_fits, 3] array.
+    The returned array keeps track of which model each extracted peak comes from,
+    returning a [n_models, 3] array, with one peak returned per model.
 
-    * Each row reflects a FOOOF model fit, in order, filled with NaN if no peak was present.
-
-    * To do so, this function necessarily extracts and returns one peak per model fit.
-
-    If, instead, you with to extract all peaks within a band, per model fit, you can do:
-
-    >>> peaks = np.empty((0, 3))
-    >>> for f_res in fg:
-    >>>     peaks = np.vstack((peaks, get_band_peak(f_res.peak_params, band, ret_one=False)))
+    - To do so, this function necessarily extracts and returns one peak per model fit.
+    - Each row reflects an individual model fit, in order, filled with nan if no peak was present.
     """
 
-    band_peaks = np.zeros(shape=[n_fits, 3])
-
     # Extracts an array per FOOOF fit, and extracts band peaks from it
+    band_peaks = np.zeros(shape=[n_fits, 3])
     for ind in range(n_fits):
         band_peaks[ind, :] = get_band_peak(peak_params[tuple([peak_params[:, -1] == ind])][:, 0:3],
-                                           band=band, ret_one=True,
+                                           band=band, select_highest=True,
                                            threshold=threshold,
                                            thresh_param=thresh_param)
 
     return band_peaks
 
 
-def get_band_peak(peak_params, band, ret_one=True, threshold=None, thresh_param='PW'):
+def get_band_peak(peak_params, band, select_highest=True, threshold=None, thresh_param='PW'):
     """Extract peaks within a given band of interest.
 
     Parameters
     ----------
     peak_params : 2d array
         Peak parameters, with shape of [n_peaks, 3].
     band : tuple of (float, float)
         Frequency range for the band of interest.
-        Defind as: (lower_frequency_bound, upper_frequency_bound).
-    ret_one : bool, optional, default: True
+        Defined as: (lower_frequency_bound, upper_frequency_bound).
+    select_highest : bool, optional, default: True
         Whether to return single peak (if True) or all peaks within the range found (if False).
         If True, returns the highest peak within the search range.
-    threshold : float
+    threshold : float, optional
         A minimum threshold value to apply.
     thresh_param : {'PW', 'BW'}
         Which parameter to threshold on. 'PW' is power and 'BW' is bandwidth.
 
     Returns
     -------
     band_peaks : 1d or 2d array
-        Peak data. Each row is a peak, as [CF, PW, BW]
+        Peak data. Each row is a peak, as [CF, PW, BW].
     """
 
     # Return nan array if empty input
     if peak_params.size == 0:
         return np.array([np.nan, np.nan, np.nan])
 
     # Find indices of peaks in the specified range, and check the number found
     peak_inds = (peak_params[:, 0] >= band[0]) & (peak_params[:, 0] <= band[1])
     n_peaks = sum(peak_inds)
 
-    # If there are no peaks within the specified range
+    # If there are no peaks within the specified range, return nan
     #   Note: this also catches and returns if the original input was empty
     if n_peaks == 0:
         return np.array([np.nan, np.nan, np.nan])
 
     band_peaks = peak_params[peak_inds, :]
 
     # Apply a minimum threshold, if one was provided
     if threshold:
         band_peaks = threshold_peaks(band_peaks, threshold, thresh_param)
 
-    # If results > 1 and ret_one, then we return the highest peak
+    # If results > 1 and select_highest, then we return the highest peak
     #    Call a sub-function to select highest power peak in band
-    if n_peaks > 1 and ret_one:
+    if n_peaks > 1 and select_highest:
         band_peaks = get_highest_peak(band_peaks)
 
     # Squeeze so that if there is only 1 result, return single peak in flat array
     return np.squeeze(band_peaks)
 
 
 def get_highest_peak(peak_params):
-    """Extract the highest peak.
+    """Extract the highest power peak.
 
     Parameters
     ----------
     peak_params : 2d array
-        Peak parameters, with shape of [n_peaks, 3] or [n_peaks, 4].
+        Peak parameters, with shape of [n_peaks, 3].
 
     Returns
     -------
     1d array
-        Peak data. Each row is a peak, as [CF, PW, BW].
+        Peak data. The row is a peak, as [CF, PW, BW].
+
+    Notes
+    -----
+    This function returns the singular highest power peak from the input set, and as
+    such is defined to work on periodic parameters from a single model fit.
     """
 
     # Catch & return NaN if empty
     if len(peak_params) == 0:
         return np.array([np.nan, np.nan, np.nan])
 
     high_ind = np.argmax(peak_params[:, 1])
@@ -200,17 +236,23 @@
     param : {'PW', 'BW'}
         Which parameter to threshold on. 'PW' is power and 'BW' is bandwidth.
 
     Returns
     -------
     thresholded_peaks : 2d array
         Peak parameters, with shape of [n_peaks, :].
+
+    Notes
+    -----
+    This function can be applied to periodic parameters from an individual model,
+    or a set or parameters from a group.
     """
 
-    # Catch & return NaN if empty
+    # Catch if input is empty & return nan if so
     if len(peak_params) == 0:
         return np.array([np.nan, np.nan, np.nan])
 
+    # Otherwise, apply a mask to apply the requested threshold
     thresh_mask = peak_params[:, PEAK_INDS[param]] > threshold
     thresholded_peaks = peak_params[thresh_mask]
 
     return thresholded_peaks
```

### Comparing `fooof-1.0.0rc3/fooof/bands/bands.py` & `fooof-1.1.0rc0/fooof/bands/bands.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-"""A data oject for managing band definitions."""
+"""A data object for managing band definitions."""
 
 from collections import OrderedDict
 
 ###################################################################################################
 ###################################################################################################
 
 class Bands():
     """Frequency band definitions.
 
     Attributes
     ----------
     bands : dict
         Band definitions. Each entry should be {'label' : (f_low, f_high)}.
+
+    Examples
+    --------
+    Define a bands object storing canonical frequency bands:
+
+    >>> bands = Bands({'theta' : [4, 8], 'alpha' : [8, 12], 'beta' : [15, 30]})
     """
 
     def __init__(self, input_bands={}):
         """Initialize the Bands object.
 
         Parameters
         ----------
@@ -50,15 +56,15 @@
 
     def __len__(self):
         """Define length as the number of bands it contains."""
 
         return self.n_bands
 
     def __iter__(self):
-        """Define iteratation as stepping across each band."""
+        """Define iteration as stepping across each band."""
 
         for label, band_definition in self.bands.items():
             yield (label, band_definition)
 
     @property
     def labels(self):
         """Labels for all the bands defined in the object."""
```

### Comparing `fooof-1.0.0rc3/fooof/core/funcs.py` & `fooof-1.1.0rc0/fooof/core/funcs.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/core/info.py` & `fooof-1.1.0rc0/fooof/core/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     ----------
     aperiodic_mode : {'fixed', 'knee'}
         Which mode was used for the aperiodic component.
 
     Returns
     -------
     indices : dict
-        Mapping of the column labels and indices for the aperiodc parameters.
+        Mapping of the column labels and indices for the aperiodic parameters.
     """
 
     if aperiodic_mode == 'fixed':
         labels = ('offset', 'exponent')
     elif aperiodic_mode == 'knee':
         labels = ('offset', 'knee', 'exponent')
     else:
```

### Comparing `fooof-1.0.0rc3/fooof/core/io.py` & `fooof-1.1.0rc0/fooof/core/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 def fname(file_name, extension):
     """Check a filename, adding an extension if not already specified.
 
     Parameters
     ----------
     file_name : str
         String that specifies a file name.
-    extensions : str
-        String that specifies the extension to be added, not including a period.
+    extension : str
+        String of the extension (without a period) to be added if one isn't already present.
 
     Outputs
     -------
     file_name : str
         String that specifies a file name.
     """
 
-    if file_name.split('.')[-1] != extension:
+    if len(file_name.split('.')) == 1:
         file_name = file_name + '.' + extension
 
     return file_name
 
 
 def fpath(file_path, file_name):
     """Build the full file path from file name and directory.
@@ -194,15 +194,15 @@
     # Get dictionary of available attributes, and convert specified lists back into arrays
     data = dict_lst_to_array(data, OBJ_DESC['arrays'])
 
     return data
 
 
 def load_jsonlines(file_name, file_path):
-    """Load a jsonlines file, yielding data line by line.
+    """Load a json-lines file, yielding data line by line.
 
     Parameters
     ----------
     file_name : str
         File to load data from.
     file_path : str
         Path to directory from load from.
```

### Comparing `fooof-1.0.0rc3/fooof/core/modutils.py` & `fooof-1.1.0rc0/fooof/core/modutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,46 @@
             mod = import_module(*args)
         except ImportError:
             mod = False
 
     return mod
 
 
+def check_dependency(dep, name):
+    """Decorator that checks if an optional dependency is available.
+
+    Parameters
+    ----------
+    dep : module or False
+        Module, if successfully imported, or boolean (False) if not.
+    name : str
+        Full name of the module, to be printed in message.
+
+    Returns
+    -------
+    wrap : callable
+        The decorated function.
+
+    Raises
+    ------
+    ImportError
+        If the requested dependency is not available.
+    """
+
+    def wrap(func):
+        @wraps(func)
+        def wrapped_func(*args, **kwargs):
+            if not dep:
+                raise ImportError("Optional FOOOF dependency " + name + \
+                                  " is required for this functionality.")
+            return func(*args, **kwargs)
+        return wrapped_func
+    return wrap
+
+
 def docs_drop_param(docstring):
     """Drop the first parameter description for a string representation of a docstring.
 
     Parameters
     ----------
     docstring : str
         Docstring to drop first parameter from.
@@ -75,15 +107,15 @@
 
 
 def docs_append_to_section(docstring, section, add):
     """Append extra information to a specified section of a docstring.
 
     Parameters
     ----------
-    ds : str
+    docstring : str
         Docstring to update.
     section : str
         Name of the section within the docstring to add to.
     add : str
         Text to append to specified section of the docstring.
 
     Returns
@@ -144,39 +176,7 @@
     def wrapper(func):
 
         func.__doc__ = docs_append_to_section(source.__doc__, section, add)
 
         return func
 
     return wrapper
-
-
-def check_dependency(dep, name):
-    """Decorator that checks if an optional dependency is available.
-
-    Parameters
-    ----------
-    dep : module or False
-        Module, if successfully imported, or boolean (False) if not.
-    name : str
-        Full name of the module, to be printed in message.
-
-    Returns
-    -------
-    wrap : callable
-        The decorated function.
-
-    Raises
-    ------
-    ImportError
-        If the requested dependency is not available.
-    """
-
-    def wrap(func):
-        @wraps(func)
-        def wrapped_func(*args, **kwargs):
-            if not dep:
-                raise ImportError("Optional FOOOF dependency " + name + \
-                                  " is required for this functionality.")
-            func(*args, **kwargs)
-        return wrapped_func
-    return wrap
```

### Comparing `fooof-1.0.0rc3/fooof/core/reports.py` & `fooof-1.1.0rc0/fooof/core/reports.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,108 +7,125 @@
 
 plt = safe_import('.pyplot', 'matplotlib')
 gridspec = safe_import('.gridspec', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
 
+## Settings & Globals
+REPORT_FIGSIZE = (16, 20)
+REPORT_FONT = {'family': 'monospace',
+               'weight': 'normal',
+               'size': 16}
+SAVE_FORMAT = 'pdf'
+
+###################################################################################################
+###################################################################################################
+
 @check_dependency(plt, 'matplotlib')
-def save_report_fm(fm, file_name, file_path=None, plt_log=False):
-    """Generate and save out a PDF report for a FOOOF object.
+def save_report_fm(fm, file_name, file_path=None, plt_log=False, add_settings=True, **plot_kwargs):
+    """Generate and save out a PDF report for a power spectrum model fit.
 
     Parameters
     ----------
     fm : FOOOF
         Object with results from fitting a power spectrum.
     file_name : str
         Name to give the saved out file.
     file_path : str, optional
         Path to directory to save to. If None, saves to current directory.
     plt_log : bool, optional, default: False
         Whether or not to plot the frequency axis in log space.
+    add_settings : bool, optional, default: True
+        Whether to add a print out of the model settings to the end of the report.
+    plot_kwargs : keyword arguments
+        Keyword arguments to pass into the plot method.
     """
 
-    font = _report_settings()
+    # Define grid settings based on what is to be plotted
+    n_rows = 3 if add_settings else 2
+    height_ratios = [0.5, 1.0, 0.25] if add_settings else [0.45, 1.0]
 
     # Set up outline figure, using gridspec
-    fig = plt.figure(figsize=(16, 20))
-    grid = gridspec.GridSpec(3, 1, height_ratios=[0.45, 1.0, 0.25])
+    _ = plt.figure(figsize=REPORT_FIGSIZE)
+    grid = gridspec.GridSpec(n_rows, 1, hspace=0.25, height_ratios=height_ratios)
 
     # First - text results
     ax0 = plt.subplot(grid[0])
     results_str = gen_results_fm_str(fm)
-    ax0.text(0.5, 0.7, results_str, font, ha='center', va='center')
+    ax0.text(0.5, 0.7, results_str, REPORT_FONT, ha='center', va='center')
     ax0.set_frame_on(False)
-    ax0.set_xticks([])
-    ax0.set_yticks([])
+    ax0.set(xticks=[], yticks=[])
 
     # Second - data plot
     ax1 = plt.subplot(grid[1])
-    fm.plot(plt_log=plt_log, ax=ax1)
+    fm.plot(plt_log=plt_log, ax=ax1, **plot_kwargs)
 
     # Third - FOOOF settings
-    ax2 = plt.subplot(grid[2])
-    settings_str = gen_settings_str(fm, False)
-    ax2.text(0.5, 0.1, settings_str, font, ha='center', va='center')
-    ax2.set_frame_on(False)
-    ax2.set_xticks([])
-    ax2.set_yticks([])
+    if add_settings:
+        ax2 = plt.subplot(grid[2])
+        settings_str = gen_settings_str(fm, False)
+        ax2.text(0.5, 0.1, settings_str, REPORT_FONT, ha='center', va='center')
+        ax2.set_frame_on(False)
+        ax2.set(xticks=[], yticks=[])
 
     # Save out the report
-    plt.savefig(fpath(file_path, fname(file_name, 'pdf')))
+    plt.savefig(fpath(file_path, fname(file_name, SAVE_FORMAT)))
     plt.close()
 
 
 @check_dependency(plt, 'matplotlib')
-def save_report_fg(fg, file_name, file_path=None):
-    """Generate and save out a PDF report for a FOOOFGroup object.
+def save_report_fg(fg, file_name, file_path=None, add_settings=True):
+    """Generate and save out a PDF report for a group of power spectrum models.
 
     Parameters
     ----------
     fg : FOOOFGroup
         Object with results from fitting a group of power spectra.
     file_name : str
         Name to give the saved out file.
     file_path : str, optional
         Path to directory to save to. If None, saves to current directory.
+    add_settings : bool, optional, default: True
+        Whether to add a print out of the model settings to the end of the report.
     """
 
-    font = _report_settings()
+    # Define grid settings based on what is to be plotted
+    n_rows = 4 if add_settings else 3
+    height_ratios = [1.0, 1.0, 1.0, 0.5] if add_settings else [0.8, 1.0, 1.0]
 
     # Initialize figure
-    fig = plt.figure(figsize=(16, 20))
-    gs = gridspec.GridSpec(3, 2, wspace=0.4, hspace=0.25, height_ratios=[0.8, 1.0, 1.0])
+    _ = plt.figure(figsize=REPORT_FIGSIZE)
+    grid = gridspec.GridSpec(n_rows, 2, wspace=0.4, hspace=0.25, height_ratios=height_ratios)
 
     # First / top: text results
-    ax0 = plt.subplot(gs[0, :])
+    ax0 = plt.subplot(grid[0, :])
     results_str = gen_results_fg_str(fg)
-    ax0.text(0.5, 0.7, results_str, font, ha='center', va='center')
+    ax0.text(0.5, 0.7, results_str, REPORT_FONT, ha='center', va='center')
     ax0.set_frame_on(False)
-    ax0.set_xticks([])
-    ax0.set_yticks([])
+    ax0.set(xticks=[], yticks=[])
+
+    # Second - data plots
 
     # Aperiodic parameters plot
-    ax1 = plt.subplot(gs[1, 0])
+    ax1 = plt.subplot(grid[1, 0])
     plot_fg_ap(fg, ax1)
 
     # Goodness of fit plot
-    ax2 = plt.subplot(gs[1, 1])
+    ax2 = plt.subplot(grid[1, 1])
     plot_fg_gf(fg, ax2)
 
     # Peak center frequencies plot
-    ax3 = plt.subplot(gs[2, :])
+    ax3 = plt.subplot(grid[2, :])
     plot_fg_peak_cens(fg, ax3)
 
+    # Third - Model settings
+    if add_settings:
+        ax4 = plt.subplot(grid[3, :])
+        settings_str = gen_settings_str(fg, False)
+        ax4.text(0.5, 0.1, settings_str, REPORT_FONT, ha='center', va='center')
+        ax4.set_frame_on(False)
+        ax4.set(xticks=[], yticks=[])
+
     # Save out the report
-    plt.savefig(fpath(file_path, fname(file_name, 'pdf')))
+    plt.savefig(fpath(file_path, fname(file_name, SAVE_FORMAT)))
     plt.close()
-
-
-def _report_settings():
-    """Return settings to be used for all reports."""
-
-    # Set the font description for saving out text with matplotlib
-    font = {'family': 'monospace',
-            'weight': 'normal',
-            'size': 16}
-
-    return font
```

### Comparing `fooof-1.0.0rc3/fooof/core/strings.py` & `fooof-1.1.0rc0/fooof/core/strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     output : str
         Formatted string of a warning about the peak width limits setting.
     """
 
     output = '\n'.join([
         '',
         'FOOOF WARNING: Lower-bound peak width limit is < or ~= the frequency resolution: ' + \
-            '{:1.2f} <= {:1.2f}'.format(freq_res, bwl),
+            '{:1.2f} <= {:1.2f}'.format(bwl, freq_res),
         '\tLower bounds below frequency-resolution have no effect ' + \
         '(effective lower bound is the frequency resolution).',
         '\tToo low a limit may lead to overfitting noise as small bandwidth peaks.',
         '\tWe recommend a lower bound of approximately 2x the frequency resolution.',
         ''
     ])
 
@@ -476,26 +476,26 @@
 
     Returns
     -------
     output : str
         Formatted string, ready for printing.
     """
 
-    # Use a smaller centering value if in concise mode
-    cv = SCV if concise else LCV
+    # Set centering value - use a smaller value if in concise mode
+    center_val = SCV if concise else LCV
 
     # Expand the section markers to full width
-    str_lst[0] = str_lst[0] * cv
-    str_lst[-1] = str_lst[-1] * cv
+    str_lst[0] = str_lst[0] * center_val
+    str_lst[-1] = str_lst[-1] * center_val
 
     # Drop blank lines, if concise
     str_lst = list(filter(lambda x: x != '', str_lst)) if concise else str_lst
 
     # Convert list to a single string representation, centering each line
-    output = '\n'.join([string.center(cv) for string in str_lst])
+    output = '\n'.join([string.center(center_val) for string in str_lst])
 
     return output
 
 
 def _no_model_str(concise=False):
     """Creates a null report, for use if the model fit failed, or is unavailable.
```

### Comparing `fooof-1.0.0rc3/fooof/core/utils.py` & `fooof-1.1.0rc0/fooof/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,32 +9,36 @@
 ###################################################################################################
 
 def group_three(vec):
     """Group an array of values into threes.
 
     Parameters
     ----------
-    vec : 1d array
-        Array of items to group by 3. Length of array must be divisible by three.
+    vec : list or 1d array
+        List or array of items to group by 3. Length of array must be divisible by three.
 
     Returns
     -------
-    list of list
-        List of lists, each with three items.
+    array or list of list
+        Array or list of lists, each with three items. Output type will match input type.
 
     Raises
     ------
     ValueError
         If input data cannot be evenly grouped into threes.
     """
 
     if len(vec) % 3 != 0:
         raise ValueError("Wrong size array to group by three.")
 
-    return [list(vec[ii:ii+3]) for ii in range(0, len(vec), 3)]
+    # Reshape, if an array, as it's faster, otherwise asssume lise
+    if isinstance(vec, np.ndarray):
+        return np.reshape(vec, (-1, 3))
+    else:
+        return [list(vec[ii:ii+3]) for ii in range(0, len(vec), 3)]
 
 
 def nearest_ind(array, value):
     """Find the nearest index, in an array, to a given value.
 
     Parameters
     ----------
@@ -206,15 +210,15 @@
     Notes
     -----
     The goal of this function is to convert multiple possible
     ways of indicating a set of indices into one consistent format.
     This function works only on indices defined for 1 dimension.
     """
 
-    # Typcasting: if a single int, convert to an array
+    # Typecasting: if a single int, convert to an array
     if isinstance(inds, int):
         inds = np.array([inds])
     # Typecasting: if a list or range, convert to an array
     elif isinstance(inds, (list, range)):
         inds = np.array(inds)
 
     # Conversion: if array is boolean, get integer indices of True
```

### Comparing `fooof-1.0.0rc3/fooof/data/data.py` & `fooof-1.1.0rc0/fooof/data/data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,100 @@
-"""Data objects for FOOOF."""
+"""Data objects for FOOOF.
+
+Notes on FOOOF data objects:
+- these data objects are NamedTuples, immutable data types with attribute labels
+- the namedtuples are wrapped as classes (they are still immutable when doing this)
+- wrapping in objects helps to be able to render well formed documentation for them.
+- setting `__slots__` as empty voids the dynamic dictionary that usually stores attributes
+    - this means no additional attributes can be defined (which is more memory efficient)
+"""
 
 from collections import namedtuple
 
 ###################################################################################################
 ###################################################################################################
 
-FOOOFSettings = namedtuple('FOOOFSettings', ['peak_width_limits', 'max_n_peaks',
-                                             'min_peak_height', 'peak_threshold',
-                                             'aperiodic_mode'])
-FOOOFSettings.__doc__ = """\
-The user defined settings for a FOOOF object.
-
-Attributes
-----------
-peak_width_limits : tuple of (float, float)
-    Limits on possible peak width, in Hz, as (lower_bound, upper_bound).
-max_n_peaks : int
-    Maximum number of peaks to fit.
-min_peak_height : float
-    Absolute threshold for detecting peaks, in units of the input data.
-peak_threshold : float
-    Relative threshold for detecting peaks, in units of standard deviation of the input data.
-aperiodic_mode : {'fixed', 'knee'}
-    Which approach to take for fitting the aperiodic component.
-"""
-
-
-FOOOFMetaData = namedtuple('FOOOFMetaData', ['freq_range', 'freq_res'])
-
-FOOOFMetaData.__doc__ = """\
-The meta-data for a FOOOF object.
-
-Attributes
-----------
-freq_range : list of [float, float]
-    Frequency range of the power spectrum, as [lowest_freq, highest_freq].
-freq_res : float
-    Frequency resolution of the power spectrum.
-"""
-
-
-FOOOFResults = namedtuple('FOOOFResults', ['aperiodic_params', 'peak_params',
-                                           'r_squared', 'error', 'gaussian_params'])
-FOOOFResults.__doc__ = """\
-The results from a FOOOF model fit.
-
-Attributes
-----------
-aperiodic_params : 1d array
-    Parameters that define the aperiodic fit. As [Offset, (Knee), Exponent].
-    The knee parameter is only included if aperiodic is fit with knee.
-peak_params : 2d array
-    Fitted parameter values for the peaks. Each row is a peak, as [CF, PW, BW].
-r_squared : float
-    R-squared of the fit between the full model fit and the input data.
-error : float
-    Total error of the full model fit, compared to the input data.
-gaussian_params : 2d array
-    Parameters that define the gaussian fit(s).
-    Each row is a gaussian, as [mean, height, standard deviation].
-"""
-
-
-SimParams = namedtuple('SimParams', ['aperiodic_params', 'periodic_params', 'nlv'])
-
-SimParams.__doc__ = """\
-Stores parameters used to simulate a single power spectra.
-
-Attributes
-----------
-aperiodic_params : list
-    Parameters that define the aperiodic component.
-periodic_params : list or list of lists
-    Parameters that define the periodic component.
-nlv : float
-    Noise level added to simulated spectrum.
-"""
+class FOOOFSettings(namedtuple('FOOOFSettings', ['peak_width_limits', 'max_n_peaks',
+                                                 'min_peak_height', 'peak_threshold',
+                                                 'aperiodic_mode'])):
+    """User defined settings for the fitting algorithm.
+
+    Parameters
+    ----------
+    peak_width_limits : tuple of (float, float)
+        Limits on possible peak width, in Hz, as (lower_bound, upper_bound).
+    max_n_peaks : int
+        Maximum number of peaks to fit.
+    min_peak_height : float
+        Absolute threshold for detecting peaks, in units of the input data.
+    peak_threshold : float
+        Relative threshold for detecting peaks, in units of standard deviation of the input data.
+    aperiodic_mode : {'fixed', 'knee'}
+        Which approach to take for fitting the aperiodic component.
+
+    Notes
+    -----
+    This object is a data object, based on a NamedTuple, with immutable data attributes.
+    """
+    __slots__ = ()
+
+
+class FOOOFMetaData(namedtuple('FOOOFMetaData', ['freq_range', 'freq_res'])):
+    """Metadata information about a power spectrum.
+
+    Parameters
+    ----------
+    freq_range : list of [float, float]
+        Frequency range of the power spectrum, as [lowest_freq, highest_freq].
+    freq_res : float
+        Frequency resolution of the power spectrum.
+
+    Notes
+    -----
+    This object is a data object, based on a NamedTuple, with immutable data attributes.
+    """
+    __slots__ = ()
+
+
+class FOOOFResults(namedtuple('FOOOFResults', ['aperiodic_params', 'peak_params',
+                                               'r_squared', 'error', 'gaussian_params'])):
+    """Model results from parameterizing a power spectrum.
+
+    Parameters
+    ----------
+    aperiodic_params : 1d array
+        Parameters that define the aperiodic fit. As [Offset, (Knee), Exponent].
+        The knee parameter is only included if aperiodic is fit with knee.
+    peak_params : 2d array
+        Fitted parameter values for the peaks. Each row is a peak, as [CF, PW, BW].
+    r_squared : float
+        R-squared of the fit between the full model fit and the input data.
+    error : float
+        Error of the full model fit.
+    gaussian_params : 2d array
+        Parameters that define the gaussian fit(s).
+        Each row is a gaussian, as [mean, height, standard deviation].
+
+    Notes
+    -----
+    This object is a data object, based on a NamedTuple, with immutable data attributes.
+    """
+    __slots__ = ()
+
+
+class SimParams(namedtuple('SimParams', ['aperiodic_params', 'periodic_params', 'nlv'])):
+    """Parameters that define a simulated power spectrum.
+
+    Parameters
+    ----------
+    aperiodic_params : list
+        Parameters that define the aperiodic component.
+    periodic_params : list or list of lists
+        Parameters that define the periodic component.
+    nlv : float
+        Noise level added to simulated spectrum.
+
+    Notes
+    -----
+    This object is a data object, based on a NamedTuple, with immutable data attributes.
+    """
+    __slots__ = ()
```

### Comparing `fooof-1.0.0rc3/fooof/objs/fit.py` & `fooof-1.1.0rc0/fooof/objs/fit.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,17 +35,23 @@
 _gauss_std_limits : list of [float, float]
     Peak width limits, converted to use for gaussian standard deviation parameter.
     This attribute is computed based on `peak_width_limits` and should not be updated directly.
 _maxfev : int
     The maximum number of calls to the curve fitting function.
 _error_metric : str
     The error metric to use for post-hoc measures of model fit error.
+
+Run Modes
+---------
 _debug : bool
     Whether the object is set in debug mode.
     This should be controlled by using the `set_debug_mode` method.
+_check_data : bool
+    Whether to check added data for NaN or Inf values, and fail out if present.
+    This should be controlled by using the `set_check_data_mode` method.
 
 Code Notes
 ----------
 Methods without defined docstrings import docs at runtime, from aliased external functions.
 """
 
 import warnings
@@ -64,18 +70,18 @@
 from fooof.core.funcs import gaussian_function, get_ap_func, infer_ap_func
 from fooof.core.errors import (FitError, NoModelError, DataError,
                                NoDataError, InconsistentDataError)
 from fooof.core.strings import (gen_settings_str, gen_results_fm_str,
                                 gen_issue_str, gen_width_warning_str)
 
 from fooof.plts.fm import plot_fm
-from fooof.plts.style import style_spectrum_plot
 from fooof.utils.data import trim_spectrum
 from fooof.utils.params import compute_gauss_std
 from fooof.data import FOOOFResults, FOOOFSettings, FOOOFMetaData
+from fooof.data.conversions import model_to_dataframe
 from fooof.sim.gen import gen_freqs, gen_aperiodic, gen_periodic, gen_model
 
 ###################################################################################################
 ###################################################################################################
 
 class FOOOF():
     """Model a physiological power spectrum as a combination of aperiodic and periodic components.
@@ -84,21 +90,23 @@
 
     Passing in logged frequencies and/or power spectra is not detected,
     and will silently produce incorrect results.
 
     Parameters
     ----------
     peak_width_limits : tuple of (float, float), optional, default: (0.5, 12.0)
-        Limits on possible peak width, as (lower_bound, upper_bound).
+        Limits on possible peak width, in Hz, as (lower_bound, upper_bound).
     max_n_peaks : int, optional, default: inf
-        Maximum number of gaussians to be fit in a single spectrum.
+        Maximum number of peaks to fit.
     min_peak_height : float, optional, default: 0
-        Absolute threshold for detecting peaks, in units of the input data.
+        Absolute threshold for detecting peaks.
+        This threshold is defined in absolute units of the power spectrum (log power).
     peak_threshold : float, optional, default: 2.0
-        Relative threshold for detecting peaks, in units of standard deviation of the input data.
+        Relative threshold for detecting peaks.
+        This threshold is defined in relative units of the power spectrum (standard deviation).
     aperiodic_mode : {'fixed', 'knee'}
         Which approach to take for fitting the aperiodic component.
     verbose : bool, optional, default: True
         Verbosity mode. If True, prints out warnings and general status updates.
 
     Attributes
     ----------
@@ -142,14 +150,15 @@
       longer time segments for power spectrum calculation to get smoother power spectra,
       as this will give better model fits.
     - The gaussian params are those that define the gaussian of the fit, where as the peak
       params are a modified version, in which the CF of the peak is the mean of the gaussian,
       the PW of the peak is the height of the gaussian over and above the aperiodic component,
       and the BW of the peak, is 2*std of the gaussian (as 'two sided' bandwidth).
     """
+    # pylint: disable=attribute-defined-outside-init
 
     def __init__(self, peak_width_limits=(0.5, 12.0), max_n_peaks=np.inf, min_peak_height=0.0,
                  peak_threshold=2.0, aperiodic_mode='fixed', verbose=True):
         """Initialize object with desired settings."""
 
         # Set input settings
         self.peak_width_limits = peak_width_limits
@@ -173,26 +182,33 @@
         #   Even if fitting without knee, leave bounds for knee (they are dropped later)
         self._ap_bounds = ((-np.inf, -np.inf, -np.inf), (np.inf, np.inf, np.inf))
         # Threshold for how far a peak has to be from edge to keep.
         #   This is defined in units of gaussian standard deviation
         self._bw_std_edge = 1.0
         # Degree of overlap between gaussians for one to be dropped
         #   This is defined in units of gaussian standard deviation
-        self._gauss_overlap_thresh = 1.5
+        self._gauss_overlap_thresh = 0.75
         # Parameter bounds for center frequency when fitting gaussians, in terms of +/- std dev
         self._cf_bound = 1.5
         # The maximum number of calls to the curve fitting function
         self._maxfev = 5000
         # The error metric to calculate, post model fitting. See `_calc_error` for options
-        #   Note: this is used to check error post-hoc, not an objective function for fitting models
+        #   Note: this is for checking error post fitting, not an objective function for fitting
         self._error_metric = 'MAE'
-        # Set whether in debug mode, in which an error is raised if a model fit fails
+
+        ## RUN MODES
+        # Set default debug mode - controls if an error is raised if model fitting is unsuccessful
         self._debug = False
+        # Set default data checking modes - controls which checks get run on input data
+        #   check_freqs: check the frequency values, and raises an error for uneven spacing
+        self._check_freqs = True
+        #   check_data: checks the power values and raises an error for any NaN / Inf values
+        self._check_data = True
 
-        # Set internal settings, based on inputs, & initialize data & results attributes
+        # Set internal settings, based on inputs, and initialize data & results attributes
         self._reset_internal_settings()
         self._reset_data_results(True, True, True)
 
 
     @property
     def has_data(self):
         """Indicator for if the object contains data."""
@@ -232,23 +248,19 @@
         """
 
         # Only update these settings if other relevant settings are available
         if self.peak_width_limits:
 
             # Bandwidth limits are given in 2-sided peak bandwidth
             #   Convert to gaussian std parameter limits
-            self._gauss_std_limits = tuple([bwl / 2 for bwl in self.peak_width_limits])
-            # Bounds for aperiodic fitting. Drops bounds on knee parameter if not set to fit knee
-            self._ap_bounds = self._ap_bounds if self.aperiodic_mode == 'knee' \
-                else tuple(bound[0::2] for bound in self._ap_bounds)
+            self._gauss_std_limits = tuple(bwl / 2 for bwl in self.peak_width_limits)
 
         # Otherwise, assume settings are unknown (have been cleared) and set to None
         else:
             self._gauss_std_limits = None
-            self._ap_bounds = None
 
 
     def _reset_data_results(self, clear_freqs=False, clear_spectrum=False, clear_results=False):
         """Set, or reset, data & results attributes to empty.
 
         Parameters
         ----------
@@ -281,40 +293,45 @@
 
             self._spectrum_flat = None
             self._spectrum_peak_rm = None
             self._ap_fit = None
             self._peak_fit = None
 
 
-    def add_data(self, freqs, power_spectrum, freq_range=None):
+    def add_data(self, freqs, power_spectrum, freq_range=None, clear_results=True):
         """Add data (frequencies, and power spectrum values) to the current object.
 
         Parameters
         ----------
         freqs : 1d array
             Frequency values for the power spectrum, in linear space.
         power_spectrum : 1d array
             Power spectrum values, which must be input in linear space.
         freq_range : list of [float, float], optional
             Frequency range to restrict power spectrum to.
             If not provided, keeps the entire range.
+        clear_results : bool, optional, default: True
+            Whether to clear prior results, if any are present in the object.
+            This should only be set to False if data for the current results are being re-added.
 
         Notes
         -----
         If called on an object with existing data and/or results
         they will be cleared by this method call.
         """
 
-        # If any data is already present, then clear data & results
+        # If any data is already present, then clear previous data
+        # Also clear results, if present, unless indicated not to
         #   This is to ensure object consistency of all data & results
-        if np.any(self.freqs):
-            self._reset_data_results(True, True, True)
+        self._reset_data_results(clear_freqs=self.has_data,
+                                 clear_spectrum=self.has_data,
+                                 clear_results=self.has_model and clear_results)
 
         self.freqs, self.power_spectrum, self.freq_range, self.freq_res = \
-            self._prepare_data(freqs, power_spectrum, freq_range, 1, self.verbose)
+            self._prepare_data(freqs, power_spectrum, freq_range, 1)
 
 
     def add_settings(self, fooof_settings):
         """Add settings into object from a FOOOFSettings object.
 
         Parameters
         ----------
@@ -357,36 +374,39 @@
         self.peak_params_ = fooof_result.peak_params
         self.r_squared_ = fooof_result.r_squared
         self.error_ = fooof_result.error
 
         self._check_loaded_results(fooof_result._asdict())
 
 
-    def report(self, freqs=None, power_spectrum=None, freq_range=None, plt_log=False):
+    def report(self, freqs=None, power_spectrum=None, freq_range=None,
+               plt_log=False, **plot_kwargs):
         """Run model fit, and display a report, which includes a plot, and printed results.
 
         Parameters
         ----------
         freqs : 1d array, optional
             Frequency values for the power spectrum.
         power_spectrum : 1d array, optional
             Power values, which must be input in linear space.
         freq_range : list of [float, float], optional
             Desired frequency range to fit the model to.
             If not provided, fits across the entire given range.
         plt_log : bool, optional, default: False
             Whether or not to plot the frequency axis in log space.
+        **plot_kwargs
+            Keyword arguments to pass into the plot method.
 
         Notes
         -----
         Data is optional, if data has already been added to the object.
         """
 
         self.fit(freqs, power_spectrum, freq_range)
-        self.plot(plt_log=plt_log)
+        self.plot(plt_log=plt_log, **plot_kwargs)
         self.print_results(concise=False)
 
 
     def fit(self, freqs=None, power_spectrum=None, freq_range=None):
         """Fit the full power spectrum as a combination of periodic and aperiodic components.
 
         Parameters
@@ -426,14 +446,22 @@
         # Check and warn about width limits (if in verbose mode)
         if self.verbose:
             self._check_width_limits()
 
         # In rare cases, the model fails to fit, and so uses try / except
         try:
 
+            # If not set to fail on NaN or Inf data at add time, check data here
+            #   This serves as a catch all for curve_fits which will fail given NaN or Inf
+            #   Because FitError's are by default caught, this allows fitting to continue
+            if not self._check_data:
+                if np.any(np.isinf(self.power_spectrum)) or np.any(np.isnan(self.power_spectrum)):
+                    raise FitError("Model fitting was skipped because there are NaN or Inf "
+                                   "values in the data, which preclude model fitting.")
+
             # Fit the aperiodic component
             self.aperiodic_params_ = self._robust_ap_fit(self.freqs, self.power_spectrum)
             self._ap_fit = gen_aperiodic(self.freqs, self.aperiodic_params_)
 
             # Flatten the power spectrum using fit aperiodic fit
             self._spectrum_flat = self.power_spectrum - self._ap_fit
 
@@ -562,17 +590,15 @@
         Raises
         ------
         NoModelError
             If there are no model fit parameters available to return.
 
         Notes
         -----
-        For further description of the data you can extract, check the FOOOFResults documentation.
-
-        If there is no data on periodic features, this method will return NaN.
+        If there are no fit peak (no peak parameters), this method will return NaN.
         """
 
         if not self.has_model:
             raise NoModelError("No model fit results are available to extract, can not proceed.")
 
         # If col specified as string, get mapping back to integer
         if isinstance(col, str):
@@ -611,26 +637,28 @@
         return FOOOFResults(**{key.strip('_') : getattr(self, key) \
             for key in OBJ_DESC['results']})
 
 
     @copy_doc_func_to_method(plot_fm)
     def plot(self, plot_peaks=None, plot_aperiodic=True, plt_log=False,
              add_legend=True, save_fig=False, file_name=None, file_path=None,
-             ax=None, plot_style=style_spectrum_plot,
-             data_kwargs=None, model_kwargs=None, aperiodic_kwargs=None, peak_kwargs=None):
+             ax=None, data_kwargs=None, model_kwargs=None,
+             aperiodic_kwargs=None, peak_kwargs=None, **plot_kwargs):
 
-        plot_fm(self, plot_peaks, plot_aperiodic, plt_log, add_legend,
-                save_fig, file_name, file_path, ax, plot_style,
-                data_kwargs, model_kwargs, aperiodic_kwargs, peak_kwargs)
+        plot_fm(self, plot_peaks=plot_peaks, plot_aperiodic=plot_aperiodic, plt_log=plt_log,
+                add_legend=add_legend, save_fig=save_fig, file_name=file_name,
+                file_path=file_path, ax=ax, data_kwargs=data_kwargs, model_kwargs=model_kwargs,
+                aperiodic_kwargs=aperiodic_kwargs, peak_kwargs=peak_kwargs, **plot_kwargs)
 
 
     @copy_doc_func_to_method(save_report_fm)
-    def save_report(self, file_name, file_path=None, plt_log=False):
+    def save_report(self, file_name, file_path=None, plt_log=False,
+                    add_settings=True, **plot_kwargs):
 
-        save_report_fm(self, file_name, file_path, plt_log)
+        save_report_fm(self, file_name, file_path, plt_log, add_settings, **plot_kwargs)
 
 
     @copy_doc_func_to_method(save_fm)
     def save(self, file_name, file_path=None, append=False,
              save_results=False, save_settings=False, save_data=False):
 
         save_fm(self, file_name, file_path, append, save_results, save_settings, save_data)
@@ -669,25 +697,56 @@
     def copy(self):
         """Return a copy of the current object."""
 
         return deepcopy(self)
 
 
     def set_debug_mode(self, debug):
-        """Set whether debug mode, wherein an error is raised if fitting is unsuccessful.
+        """Set debug mode, which controls if an error is raised if model fitting is unsuccessful.
 
         Parameters
         ----------
         debug : bool
             Whether to run in debug mode.
         """
 
         self._debug = debug
 
 
+    def set_check_data_mode(self, check_data):
+        """Set check data mode, which controls if an error is raised if NaN or Inf data are added.
+
+        Parameters
+        ----------
+        check_data : bool
+            Whether to run in check data mode.
+        """
+
+        self._check_data = check_data
+
+
+    def to_df(self, peak_org):
+        """Convert and extract the model results as a pandas object.
+
+        Parameters
+        ----------
+        peak_org : int or Bands
+            How to organize peaks.
+            If int, extracts the first n peaks.
+            If Bands, extracts peaks based on band definitions.
+
+        Returns
+        -------
+        pd.Series
+            Model results organized into a pandas object.
+        """
+
+        return model_to_dataframe(self.get_results(), peak_org)
+
+
     def _check_width_limits(self):
         """Check and warn about peak width limits / frequency resolution interaction."""
 
         # Check peak width limits against frequency resolution and warn if too close
         if 1.5 * self.freq_res >= self.peak_width_limits[0]:
             print(gen_width_warning_str(self.freq_res, self.peak_width_limits[0]))
 
@@ -708,34 +767,39 @@
             Parameter estimates for aperiodic fit.
         """
 
         # Get the guess parameters and/or calculate from the data, as needed
         #   Note that these are collected as lists, to concatenate with or without knee later
         off_guess = [power_spectrum[0] if not self._ap_guess[0] else self._ap_guess[0]]
         kne_guess = [self._ap_guess[1]] if self.aperiodic_mode == 'knee' else []
-        exp_guess = [np.abs(self.power_spectrum[-1] - self.power_spectrum[0] /
-                            np.log10(self.freqs[-1]) - np.log10(self.freqs[0]))
+        exp_guess = [np.abs((self.power_spectrum[-1] - self.power_spectrum[0]) /
+                            (np.log10(self.freqs[-1]) - np.log10(self.freqs[0])))
                      if not self._ap_guess[2] else self._ap_guess[2]]
 
+        # Get bounds for aperiodic fitting, dropping knee bound if not set to fit knee
+        ap_bounds = self._ap_bounds if self.aperiodic_mode == 'knee' \
+            else tuple(bound[0::2] for bound in self._ap_bounds)
+
         # Collect together guess parameters
-        guess = np.array([off_guess + kne_guess + exp_guess])
+        guess = np.array(off_guess + kne_guess + exp_guess)
 
         # Ignore warnings that are raised in curve_fit
         #   A runtime warning can occur while exploring parameters in curve fitting
         #     This doesn't effect outcome - it won't settle on an answer that does this
         #   It happens if / when b < 0 & |b| > x**2, as it leads to log of a negative number
         try:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 aperiodic_params, _ = curve_fit(get_ap_func(self.aperiodic_mode),
                                                 freqs, power_spectrum, p0=guess,
-                                                maxfev=self._maxfev, bounds=self._ap_bounds)
-        except RuntimeError:
-            raise FitError("Model fitting failed due to not finding parameters in "
-                           "the simple aperiodic component fit.")
+                                                maxfev=self._maxfev, bounds=ap_bounds)
+        except RuntimeError as excp:
+            error_msg = ("Model fitting failed due to not finding parameters in "
+                         "the simple aperiodic component fit.")
+            raise FitError(error_msg) from excp
 
         return aperiodic_params
 
 
     def _robust_ap_fit(self, freqs, power_spectrum):
         """Fit the aperiodic component of the power spectrum robustly, ignoring outliers.
 
@@ -769,27 +833,34 @@
 
         # Use percentile threshold, in terms of # of points, to extract and re-fit
         perc_thresh = np.percentile(flatspec, self._ap_percentile_thresh)
         perc_mask = flatspec <= perc_thresh
         freqs_ignore = freqs[perc_mask]
         spectrum_ignore = power_spectrum[perc_mask]
 
+        # Get bounds for aperiodic fitting, dropping knee bound if not set to fit knee
+        ap_bounds = self._ap_bounds if self.aperiodic_mode == 'knee' \
+            else tuple(bound[0::2] for bound in self._ap_bounds)
+
         # Second aperiodic fit - using results of first fit as guess parameters
         #  See note in _simple_ap_fit about warnings
         try:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 aperiodic_params, _ = curve_fit(get_ap_func(self.aperiodic_mode),
                                                 freqs_ignore, spectrum_ignore, p0=popt,
-                                                maxfev=self._maxfev, bounds=self._ap_bounds)
-        except RuntimeError:
-            raise FitError("Model fitting failed due to not finding "
-                           "parameters in the robust aperiodic fit.")
-        except TypeError:
-            raise FitError("Model fitting failed due to sub-sampling in the robust aperiodic fit.")
+                                                maxfev=self._maxfev, bounds=ap_bounds)
+        except RuntimeError as excp:
+            error_msg = ("Model fitting failed due to not finding "
+                         "parameters in the robust aperiodic fit.")
+            raise FitError(error_msg) from excp
+        except TypeError as excp:
+            error_msg = ("Model fitting failed due to sub-sampling "
+                         "in the robust aperiodic fit.")
+            raise FitError(error_msg) from excp
 
         return aperiodic_params
 
 
     def _fit_peaks(self, flat_iter):
         """Iteratively fit peaks to flattened spectrum.
 
@@ -812,15 +883,15 @@
         #   Stopping procedures: limit on # of peaks, or relative or absolute height thresholds
         while len(guess) < self.max_n_peaks:
 
             # Find candidate peak - the maximum point of the flattened spectrum
             max_ind = np.argmax(flat_iter)
             max_height = flat_iter[max_ind]
 
-            # Stop searching for peaks peaks once drops below height threshold
+            # Stop searching for peaks once height drops below height threshold
             if max_height <= self.peak_threshold * np.std(flat_iter):
                 break
 
             # Set the guess parameters for gaussian fitting, specifying the mean and height
             guess_freq = self.freqs[max_ind]
             guess_height = max_height
 
@@ -846,15 +917,15 @@
 
                 # Use the shortest side to estimate full-width, half max (converted to Hz)
                 #   and use this to estimate that guess for gaussian standard deviation
                 fwhm = short_side * 2 * self.freq_res
                 guess_std = compute_gauss_std(fwhm)
 
             except ValueError:
-                # This procedure can fail (extremely rarely), if both le & ri ind's end up as None
+                # This procedure can fail (very rarely), if both left & right inds end up as None
                 #   In this case, default the guess to the average of the peak width limits
                 guess_std = np.mean(self.peak_width_limits)
 
             # Check that guess value isn't outside preset limits - restrict if so
             #   Note: without this, curve_fitting fails if given guess > or < bounds
             if guess_std < self._gauss_std_limits[0]:
                 guess_std = self._gauss_std_limits[0]
@@ -910,31 +981,33 @@
         lo_bound = [bound if bound[0] > self.freq_range[0] else \
             [self.freq_range[0], *bound[1:]] for bound in lo_bound]
         hi_bound = [bound if bound[0] < self.freq_range[1] else \
             [self.freq_range[1], *bound[1:]] for bound in hi_bound]
 
         # Unpacks the embedded lists into flat tuples
         #   This is what the fit function requires as input
-        gaus_param_bounds = (tuple([item for sublist in lo_bound for item in sublist]),
-                             tuple([item for sublist in hi_bound for item in sublist]))
+        gaus_param_bounds = (tuple(item for sublist in lo_bound for item in sublist),
+                             tuple(item for sublist in hi_bound for item in sublist))
 
         # Flatten guess, for use with curve fit
         guess = np.ndarray.flatten(guess)
 
         # Fit the peaks
         try:
             gaussian_params, _ = curve_fit(gaussian_function, self.freqs, self._spectrum_flat,
                                            p0=guess, maxfev=self._maxfev, bounds=gaus_param_bounds)
-        except RuntimeError:
-            raise FitError("Model fitting failed due to not finding "
-                           "parameters in the peak component fit.")
-        except LinAlgError:
-            raise FitError("Model fitting failed due to a LinAlgError during peak fitting. "
-                           "This can happen with settings that are too liberal, leading, "
-                           "to a large number of guess peaks that cannot be fit together.")
+        except RuntimeError as excp:
+            error_msg = ("Model fitting failed due to not finding "
+                         "parameters in the peak component fit.")
+            raise FitError(error_msg) from excp
+        except LinAlgError as excp:
+            error_msg = ("Model fitting failed due to a LinAlgError during peak fitting. "
+                         "This can happen with settings that are too liberal, leading, "
+                         "to a large number of guess peaks that cannot be fit together.")
+            raise FitError(error_msg) from excp
 
         # Re-organize params into 2d matrix
         gaussian_params = np.array(group_three(gaussian_params))
 
         return gaussian_params
 
 
@@ -962,26 +1035,24 @@
         The gaussian standard deviation is updated to be 'both-sided', to reflect the
         'bandwidth' of the peak, as opposed to the gaussian parameter, which is 1-sided.
 
         Performing this conversion requires that the model has been run,
         with `freqs`, `fooofed_spectrum_` and `_ap_fit` all required to be available.
         """
 
-        peak_params = np.empty([0, 3])
+        peak_params = np.empty((len(gaus_params), 3))
 
         for ii, peak in enumerate(gaus_params):
 
             # Gets the index of the power_spectrum at the frequency closest to the CF of the peak
-            ind = min(range(len(self.freqs)), key=lambda ii: abs(self.freqs[ii] - peak[0]))
+            ind = np.argmin(np.abs(self.freqs - peak[0]))
 
             # Collect peak parameter data
-            peak_params = np.vstack((peak_params,
-                                     [peak[0],
-                                      self.fooofed_spectrum_[ind] - self._ap_fit[ind],
-                                      peak[2] * 2]))
+            peak_params[ii] = [peak[0], self.fooofed_spectrum_[ind] - self._ap_fit[ind],
+                               peak[2] * 2]
 
         return peak_params
 
 
     def _drop_peak_cf(self, guess):
         """Check whether to drop peaks based on center's proximity to the edge of the spectrum.
 
@@ -992,16 +1063,16 @@
 
         Returns
         -------
         guess : 2d array
             Guess parameters for gaussian peak fits. Shape: [n_peaks, 3].
         """
 
-        cf_params = [item[0] for item in guess]
-        bw_params = [item[2] * self._bw_std_edge for item in guess]
+        cf_params = guess[:, 0]
+        bw_params = guess[:, 2] * self._bw_std_edge
 
         # Check if peaks within drop threshold from the edge of the frequency range
         keep_peak = \
             (np.abs(np.subtract(cf_params, self.freq_range[0])) > bw_params) & \
             (np.abs(np.subtract(cf_params, self.freq_range[1])) > bw_params)
 
         # Drop peaks that fail the center frequency edge criterion
@@ -1022,25 +1093,29 @@
         -------
         guess : 2d array
             Guess parameters for gaussian peak fits. Shape: [n_peaks, 3].
 
         Notes
         -----
         For any gaussians with an overlap that crosses the threshold,
-        the lowest height guess guassian is dropped.
+        the lowest height guess Gaussian is dropped.
         """
 
-        # Sort the peak guesses, so can check overlap of adjacent peaks
+        # Sort the peak guesses by increasing frequency
+        #   This is so adjacent peaks can be compared from right to left
         guess = sorted(guess, key=lambda x: float(x[0]))
 
         # Calculate standard deviation bounds for checking amount of overlap
-        bounds = [[peak[0] - peak[2] * self._gauss_overlap_thresh, peak[0],
+        #   The bounds are the gaussian frequency +/- gaussian standard deviation
+        bounds = [[peak[0] - peak[2] * self._gauss_overlap_thresh,
                    peak[0] + peak[2] * self._gauss_overlap_thresh] for peak in guess]
 
         # Loop through peak bounds, comparing current bound to that of next peak
+        #   If the left peak's upper bound extends pass the right peaks lower bound,
+        #   then drop the Gaussian with the lower height
         drop_inds = []
         for ind, b_0 in enumerate(bounds[:-1]):
             b_1 = bounds[ind + 1]
 
             # Check if bound of current peak extends into next peak
             if b_0[1] > b_1[0]:
 
@@ -1063,15 +1138,18 @@
 
     def _calc_error(self, metric=None):
         """Calculate the overall error of the model fit, compared to the original data.
 
         Parameters
         ----------
         metric : {'MAE', 'MSE', 'RMSE'}, optional
-            Which error measure to calculate.
+            Which error measure to calculate:
+            * 'MAE' : mean absolute error
+            * 'MSE' : mean squared error
+            * 'RMSE' : root mean squared error
 
         Raises
         ------
         ValueError
             If the requested error metric is not understood.
 
         Notes
@@ -1088,35 +1166,32 @@
         elif metric == 'MSE':
             self.error_ = ((self.power_spectrum - self.fooofed_spectrum_) ** 2).mean()
 
         elif metric == 'RMSE':
             self.error_ = np.sqrt(((self.power_spectrum - self.fooofed_spectrum_) ** 2).mean())
 
         else:
-            msg = "Error metric '{}' not understood or not implemented.".format(metric)
-            raise ValueError(msg)
+            error_msg = "Error metric '{}' not understood or not implemented.".format(metric)
+            raise ValueError(error_msg)
 
 
-    @staticmethod
-    def _prepare_data(freqs, power_spectrum, freq_range, spectra_dim=1, verbose=True):
+    def _prepare_data(self, freqs, power_spectrum, freq_range, spectra_dim=1):
         """Prepare input data for adding to current object.
 
         Parameters
         ----------
         freqs : 1d array
             Frequency values for the power_spectrum, in linear space.
         power_spectrum : 1d or 2d array
             Power values, which must be input in linear space.
             1d vector, or 2d as [n_power_spectra, n_freqs].
         freq_range : list of [float, float]
             Frequency range to restrict power spectrum to. If None, keeps the entire range.
         spectra_dim : int, optional, default: 1
             Dimensionality that the power spectra should have.
-        verbose : bool, optional
-            Whether to be verbose in printing out warnings.
 
         Returns
         -------
         freqs : 1d array
             Frequency values for the power_spectrum, in linear space.
         power_spectrum : 1d or 2d array
             Power spectrum values, in log10 scale.
@@ -1160,34 +1235,44 @@
             power_spectrum = power_spectrum.astype('float64')
 
         # Check frequency range, trim the power_spectrum range if requested
         if freq_range:
             freqs, power_spectrum = trim_spectrum(freqs, power_spectrum, freq_range)
 
         # Check if freqs start at 0 and move up one value if so
-        #   Aperiodic fit gets an inf is freq of 0 is included, which leads to an error
+        #   Aperiodic fit gets an inf if freq of 0 is included, which leads to an error
         if freqs[0] == 0.0:
             freqs, power_spectrum = trim_spectrum(freqs, power_spectrum, [freqs[1], freqs.max()])
-            if verbose:
+            if self.verbose:
                 print("\nFOOOF WARNING: Skipping frequency == 0, "
                       "as this causes a problem with fitting.")
 
         # Calculate frequency resolution, and actual frequency range of the data
         freq_range = [freqs.min(), freqs.max()]
         freq_res = freqs[1] - freqs[0]
 
         # Log power values
         power_spectrum = np.log10(power_spectrum)
 
-        # Check if there are any infs / nans, and raise an error if so
-        if np.any(np.isinf(power_spectrum)) or np.any(np.isnan(power_spectrum)):
-            raise DataError("The input power spectra data, after logging, contains NaNs or Infs. "
-                            "This will cause the fitting to fail. "
-                            "One reason this can happen is if inputs are already logged. "
-                            "Inputs data should be in linear spacing, not log.")
+        ## Data checks - run checks on inputs based on check modes
+
+        if self._check_freqs:
+            # Check if the frequency data is unevenly spaced, and raise an error if so
+            freq_diffs = np.diff(freqs)
+            if not np.all(np.isclose(freq_diffs, freq_res)):
+                raise DataError("The input frequency values are not evenly spaced. "
+                                "The model expects equidistant frequency values in linear space.")
+        if self._check_data:
+            # Check if there are any infs / nans, and raise an error if so
+            if np.any(np.isinf(power_spectrum)) or np.any(np.isnan(power_spectrum)):
+                error_msg = ("The input power spectra data, after logging, contains NaNs or Infs. "
+                             "This will cause the fitting to fail. "
+                             "One reason this can happen is if inputs are already logged. "
+                             "Inputs data should be in linear spacing, not log.")
+                raise DataError(error_msg)
 
         return freqs, power_spectrum, freq_range, freq_res
 
 
     def _add_from_dict(self, data):
         """Add data to object from a dictionary.
```

### Comparing `fooof-1.0.0rc3/fooof/objs/group.py` & `fooof-1.1.0rc0/fooof/objs/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from fooof.core.info import get_indices
 from fooof.core.utils import check_inds
 from fooof.core.errors import NoModelError
 from fooof.core.reports import save_report_fg
 from fooof.core.strings import gen_results_fg_str
 from fooof.core.io import save_fg, load_jsonlines
 from fooof.core.modutils import copy_doc_func_to_method, safe_import
+from fooof.data.conversions import group_to_dataframe
 
 ###################################################################################################
 ###################################################################################################
 
 class FOOOFGroup(FOOOF):
     """Model a group of power spectra as a combination of aperiodic and periodic components.
 
@@ -91,14 +92,15 @@
       (`aperiodic_params_`, `peak_params_`, `gaussian_params_`, `r_squared_`, `error_`)
       which are defined in the context of individual model fits. These attributes are
       used during the fitting process, but in the group context do not store results
       post-fitting. Rather, all model fit results are collected and stored into the
       `group_results` attribute. To access individual parameters of the fit, use
       the `get_params` method.
     """
+    # pylint: disable=attribute-defined-outside-init, arguments-differ
 
     def __init__(self, *args, **kwargs):
         """Initialize object with desired settings."""
 
         FOOOF.__init__(self, *args, **kwargs)
 
         self.power_spectra = None
@@ -217,15 +219,15 @@
         # If any data is already present, then clear data & results
         #   This is to ensure object consistency of all data & results
         if np.any(self.freqs):
             self._reset_data_results(True, True, True, True)
             self._reset_group_results()
 
         self.freqs, self.power_spectra, self.freq_range, self.freq_res = \
-            self._prepare_data(freqs, power_spectra, freq_range, 2, self.verbose)
+            self._prepare_data(freqs, power_spectra, freq_range, 2)
 
 
     def report(self, freqs=None, power_spectra=None, freq_range=None, n_jobs=1, progress=None):
         """Fit a group of power spectra and display a report, with a plot and printed results.
 
         Parameters
         ----------
@@ -349,15 +351,16 @@
         NoModelError
             If there are no model fit results available.
         ValueError
             If the input for the `col` input is not understood.
 
         Notes
         -----
-        For further description of the data you can extract, check the FOOOFResults documentation.
+        When extracting peak information ('peak_params' or 'gaussian_params'), an additional column
+        is appended to the returned array, indicating the index of the model that the peak came from.
         """
 
         if not self.has_model:
             raise NoModelError("No model fit results are available, can not proceed.")
 
         # Allow for shortcut alias, without adding `_params`
         if name in ['aperiodic', 'peak', 'gaussian']:
@@ -370,46 +373,43 @@
             if col not in [0, 1, 2]:
                 raise ValueError("Input value for `col` not valid.")
 
         # Pull out the requested data field from the group data
         # As a special case, peak_params are pulled out in a way that appends
         #  an extra column, indicating which FOOOF run each peak comes from
         if name in ('peak_params', 'gaussian_params'):
-            out = np.array([np.insert(getattr(data, name), 3, index, axis=1)
-                            for index, data in enumerate(self.group_results)])
+
+            # Collect peak data, appending the index of the model it comes from
+            out = np.vstack([np.insert(getattr(data, name), 3, index, axis=1)
+                             for index, data in enumerate(self.group_results)])
+
             # This updates index to grab selected column, and the last column
             #  This last column is the 'index' column (FOOOF object source)
             if col is not None:
                 col = [col, -1]
         else:
             out = np.array([getattr(data, name) for data in self.group_results])
 
-        # Some data can end up as a list of separate arrays
-        #   If so, concatenate it all into one 2d array
-        if isinstance(out[0], np.ndarray):
-            out = np.concatenate([arr.reshape(1, len(arr)) \
-                if arr.ndim == 1 else arr for arr in out], 0)
-
         # Select out a specific column, if requested
         if col is not None:
             out = out[:, col]
 
         return out
 
 
     @copy_doc_func_to_method(plot_fg)
-    def plot(self, save_fig=False, file_name=None, file_path=None):
+    def plot(self, save_fig=False, file_name=None, file_path=None, **plot_kwargs):
 
-        plot_fg(self, save_fig, file_name, file_path)
+        plot_fg(self, save_fig=save_fig, file_name=file_name, file_path=file_path, **plot_kwargs)
 
 
     @copy_doc_func_to_method(save_report_fg)
-    def save_report(self, file_name, file_path=None):
+    def save_report(self, file_name, file_path=None, add_settings=True):
 
-        save_report_fg(self, file_name, file_path)
+        save_report_fg(self, file_name, file_path, add_settings)
 
 
     @copy_doc_func_to_method(save_fg)
     def save(self, file_name, file_path=None, append=False,
              save_results=False, save_settings=False, save_data=False):
 
         save_fg(self, file_name, file_path, append, save_results, save_settings, save_data)
@@ -471,16 +471,17 @@
 
         Returns
         -------
         fm : FOOOF
             The FOOOFResults data loaded into a FOOOF object.
         """
 
-        # Initialize a FOOOF object, with same settings as current FOOOFGroup
+        # Initialize a FOOOF object, with same settings & check data mode as current FOOOFGroup
         fm = FOOOF(*self.get_settings(), verbose=self.verbose)
+        fm.set_check_data_mode(self._check_data)
 
         # Add data for specified single power spectrum, if available
         #   The power spectrum is inverted back to linear, as it is re-logged when added to FOOOF
         if self.has_data:
             fm.add_data(self.freqs, np.power(10, self.power_spectra[ind]))
         # If no power spectrum data available, copy over data information & regenerate freqs
         else:
@@ -537,14 +538,57 @@
         concise : bool, optional, default: False
             Whether to print the report in a concise mode, or not.
         """
 
         print(gen_results_fg_str(self, concise))
 
 
+    def save_model_report(self, index, file_name, file_path=None, plt_log=False,
+                          add_settings=True, **plot_kwargs):
+        """"Save out an individual model report for a specified model fit.
+
+        Parameters
+        ----------
+        index : int
+            Index of the model fit to save out.
+        file_name : str
+            Name to give the saved out file.
+        file_path : str, optional
+            Path to directory to save to. If None, saves to current directory.
+        plt_log : bool, optional, default: False
+            Whether or not to plot the frequency axis in log space.
+        add_settings : bool, optional, default: True
+            Whether to add a print out of the model settings to the end of the report.
+        plot_kwargs : keyword arguments
+            Keyword arguments to pass into the plot method.
+        """
+
+        self.get_fooof(ind=index, regenerate=True).save_report(\
+            file_name, file_path, plt_log, **plot_kwargs)
+
+
+    def to_df(self, peak_org):
+        """Convert and extract the model results as a pandas object.
+
+        Parameters
+        ----------
+        peak_org : int or Bands
+            How to organize peaks.
+            If int, extracts the first n peaks.
+            If Bands, extracts peaks based on band definitions.
+
+        Returns
+        -------
+        pd.DataFrame
+            Model results organized into a pandas object.
+        """
+
+        return group_to_dataframe(self.get_results(), peak_org)
+
+
     def _fit(self, *args, **kwargs):
         """Create an alias to FOOOF.fit for FOOOFGroup object, for internal use."""
 
         super().fit(*args, **kwargs)
 
 
     def _get_results(self):
@@ -552,15 +596,15 @@
 
         return super().get_results()
 
     def _check_width_limits(self):
         """Check and warn about bandwidth limits / frequency resolution interaction."""
 
         # Only check & warn on first power spectrum
-        #   This is to avoid spamming stdout for every spectrum in the group
+        #   This is to avoid spamming standard output for every spectrum in the group
         if self.power_spectra[0, 0] == self.power_spectrum[0]:
             super()._check_width_limits()
 
 ###################################################################################################
 ###################################################################################################
 
 def _par_fit(power_spectrum, fg):
```

### Comparing `fooof-1.0.0rc3/fooof/objs/utils.py` & `fooof-1.1.0rc0/fooof/objs/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -129,14 +129,24 @@
     fg : FOOOFGroup
         Resultant object from combining inputs.
 
     Raises
     ------
     IncompatibleSettingsError
         If the input objects have incompatible settings for combining.
+
+    Examples
+    --------
+    Combine FOOOF objects together (where `fm1`, `fm2` & `fm3` are assumed to be defined and fit):
+
+    >>> fg = combine_fooofs([fm1, fm2, fm3])  # doctest:+SKIP
+
+    Combine FOOOFGroup objects together (where `fg1` & `fg2` are assumed to be defined and fit):
+
+    >>> fg = combine_fooofs([fg1, fg2])  # doctest:+SKIP
     """
 
     # Compare settings
     if not compare_info(fooofs, 'settings') or not compare_info(fooofs, 'meta_data'):
         raise IncompatibleSettingsError("These objects have incompatible settings "
                                         "or meta data, and so cannot be combined.")
 
@@ -164,22 +174,25 @@
             if f_obj.power_spectrum is not None:
                 temp_power_spectra = np.vstack([temp_power_spectra, f_obj.power_spectrum])
 
     # If the number of collected power spectra is consistent, then add them to object
     if len(fg) == temp_power_spectra.shape[0]:
         fg.power_spectra = temp_power_spectra
 
+    # Set the check data mode, as True if any of the inputs have it on, False otherwise
+    fg.set_check_data_mode(any(getattr(f_obj, '_check_data') for f_obj in fooofs))
+
     # Add data information information
     fg.add_meta_data(fooofs[0].get_meta_data())
 
     return fg
 
 
 def fit_fooof_3d(fg, freqs, power_spectra, freq_range=None, n_jobs=1):
-    """Fit FOOOF models across a 3D array of power spectra.
+    """Fit FOOOF models across a 3d array of power spectra.
 
     Parameters
     ----------
     fg : FOOOFGroup
         Object to fit with, initialized with desired settings.
     freqs : 1d array
         Frequency values for the power spectra, in linear space.
@@ -191,15 +204,29 @@
         Number of jobs to run in parallel.
         1 is no parallelization. -1 uses all available cores.
 
     Returns
     -------
     fgs : list of FOOOFGroups
         Collected FOOOFGroups after fitting across power spectra, length of n_conditions.
+
+
+    Examples
+    --------
+    Fit a 3d array of power spectra, assuming `freqs` and `spectra` are already defined:
+
+    >>> from fooof import FOOOFGroup
+    >>> fg = FOOOFGroup(peak_width_limits=[1, 6], min_peak_height=0.1)
+    >>> fgs = fit_fooof_3d(fg, freqs, power_spectra, freq_range=[3, 30])  # doctest:+SKIP
     """
 
-    fgs = []
-    for cond_spectra in power_spectra:
-        fg.fit(freqs, cond_spectra, freq_range, n_jobs)
-        fgs.append(fg.copy())
+    # Reshape 3d data to 2d and fit, in order to fit with a single group model object
+    shape = np.shape(power_spectra)
+    powers_2d = np.reshape(power_spectra, (shape[0] * shape[1], shape[2]))
+
+    fg.fit(freqs, powers_2d, freq_range, n_jobs)
+
+    # Reorganize 2d results into a list of model group objects, to reflect original shape
+    fgs = [fg.get_group(range(dim_a * shape[1], (dim_a + 1) * shape[1])) \
+        for dim_a in range(shape[0])]
 
     return fgs
```

### Comparing `fooof-1.0.0rc3/fooof/plts/annotate.py` & `fooof-1.1.0rc0/fooof/plts/annotate.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,95 +2,101 @@
 
 import numpy as np
 
 from fooof.core.utils import nearest_ind
 from fooof.core.errors import NoModelError
 from fooof.core.funcs import gaussian_function
 from fooof.core.modutils import safe_import, check_dependency
+
 from fooof.sim.gen import gen_aperiodic
-from fooof.plts.utils import check_ax
-from fooof.plts.spectra import plot_spectrum
-from fooof.plts.settings import FIGSIZE_SPECTRAL
-from fooof.plts.style import check_n_style, style_spectrum_plot
 from fooof.analysis.periodic import get_band_peak_fm
 from fooof.utils.params import compute_knee_frequency, compute_fwhm
 
+from fooof.plts.spectra import plot_spectra
+from fooof.plts.utils import check_ax, savefig
+from fooof.plts.settings import PLT_FIGSIZES, PLT_COLORS
+from fooof.plts.style import style_spectrum_plot
+
 plt = safe_import('.pyplot', 'matplotlib')
 mpatches = safe_import('.patches', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
 
+@savefig
 @check_dependency(plt, 'matplotlib')
-def plot_annotated_peak_search(fm, plot_style=style_spectrum_plot):
+def plot_annotated_peak_search(fm):
     """Plot a series of plots illustrating the peak search from a flattened spectrum.
 
     Parameters
     ----------
     fm : FOOOF
         FOOOF object, with model fit, data and settings available.
-    plot_style : callable, optional, default: style_spectrum_plot
-        A function to call to apply styling & aesthetics to the plots.
     """
 
     # Recalculate the initial aperiodic fit and flattened spectrum that
     #   is the same as the one that is used in the peak fitting procedure
     flatspec = fm.power_spectrum - \
         gen_aperiodic(fm.freqs, fm._robust_ap_fit(fm.freqs, fm.power_spectrum))
 
     # Calculate ylims of the plot that are scaled to the range of the data
     ylims = [min(flatspec) - 0.1 * np.abs(min(flatspec)), max(flatspec) + 0.1 * max(flatspec)]
 
+    # Sort parameters by peak height
+    gaussian_params = fm.gaussian_params_[fm.gaussian_params_[:, 1].argsort()][::-1]
+
     # Loop through the iterative search for each peak
     for ind in range(fm.n_peaks_ + 1):
 
         # This forces the creation of a new plotting axes per iteration
-        ax = check_ax(None, FIGSIZE_SPECTRAL)
+        ax = check_ax(None, PLT_FIGSIZES['spectral'])
 
-        plot_spectrum(fm.freqs, flatspec, ax=ax, plot_style=None,
-                      label='Flattened Spectrum', linewidth=2.5)
-        plot_spectrum(fm.freqs, [fm.peak_threshold * np.std(flatspec)]*len(fm.freqs),
-                      ax=ax, plot_style=None, label='Relative Threshold',
-                      color='orange', linewidth=2.5, linestyle='dashed')
-        plot_spectrum(fm.freqs, [fm.min_peak_height]*len(fm.freqs),
-                      ax=ax, plot_style=None, label='Absolute Threshold',
-                      color='red', linewidth=2.5, linestyle='dashed')
+        plot_spectra(fm.freqs, flatspec, ax=ax, linewidth=2.5,
+                     label='Flattened Spectrum', color=PLT_COLORS['data'])
+        plot_spectra(fm.freqs, [fm.peak_threshold * np.std(flatspec)]*len(fm.freqs), ax=ax,
+                     label='Relative Threshold', color='orange', linewidth=2.5, linestyle='dashed')
+        plot_spectra(fm.freqs, [fm.min_peak_height]*len(fm.freqs), ax=ax,
+                     label='Absolute Threshold', color='red', linewidth=2.5, linestyle='dashed')
 
         maxi = np.argmax(flatspec)
-        ax.plot(fm.freqs[maxi], flatspec[maxi], '.', markersize=24)
+        ax.plot(fm.freqs[maxi], flatspec[maxi], '.',
+                color=PLT_COLORS['periodic'], alpha=0.75, markersize=30)
 
         ax.set_ylim(ylims)
         ax.set_title('Iteration #' + str(ind+1), fontsize=16)
 
         if ind < fm.n_peaks_:
 
-            gauss = gaussian_function(fm.freqs, *fm.gaussian_params_[ind, :])
-            plot_spectrum(fm.freqs, gauss, ax=ax, plot_style=None,
-                          label='Gaussian Fit', linestyle=':', linewidth=2.5)
+            gauss = gaussian_function(fm.freqs, *gaussian_params[ind, :])
+            plot_spectra(fm.freqs, gauss, ax=ax, label='Gaussian Fit',
+                         color=PLT_COLORS['periodic'], linestyle=':', linewidth=3.0)
 
             flatspec = flatspec - gauss
 
-        check_n_style(plot_style, ax, False, True)
+        style_spectrum_plot(ax, False, True)
 
 
+@savefig
 @check_dependency(plt, 'matplotlib')
-def plot_annotated_model(fm, plt_log=False, annotate_peaks=True, annotate_aperiodic=True,
-                         ax=None, plot_style=style_spectrum_plot):
+def plot_annotated_model(fm, plt_log=False, annotate_peaks=True,
+                         annotate_aperiodic=True, ax=None):
     """Plot a an annotated power spectrum and model, from a FOOOF object.
 
     Parameters
     ----------
     fm : FOOOF
         FOOOF object, with model fit, data and settings available.
     plt_log : boolean, optional, default: False
         Whether to plot the frequency values in log10 spacing.
+    annotate_peaks : boolean, optional, default: True
+        Whether to annotate the periodic components of the model fit.
+    annotate_aperiodic : boolean, optional, default: True
+        Whether to annotate the aperiodic components of the model fit.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
-    plot_style : callable, optional, default: style_spectrum_plot
-        A function to call to apply styling & aesthetics to the plots.
 
     Raises
     ------
     NoModelError
         If there are no model results available to plot.
     """
 
@@ -98,42 +104,40 @@
     if not fm.has_model:
         raise NoModelError("No model is available to plot, can not proceed.")
 
     # Settings
     fontsize = 15
     lw1 = 4.0
     lw2 = 3.0
-    ms = 12
-    colors = {'data' : 'black', 'periodic' : 'green',
-              'aperiodic' : 'blue', 'model' : 'red'}
+    ms1 = 12
 
     # Create the baseline figure
-    ax = check_ax(ax, FIGSIZE_SPECTRAL)
-    fm.plot(plot_peaks='dot-shade-width', plt_log=plt_log, ax=ax, plot_style=None,
+    ax = check_ax(ax, PLT_FIGSIZES['spectral'])
+    fm.plot(plot_peaks='dot-shade-width', plt_log=plt_log, ax=ax,
             data_kwargs={'lw' : lw1, 'alpha' : 0.6},
             aperiodic_kwargs={'lw' : lw1, 'zorder' : 10},
             model_kwargs={'lw' : lw1, 'alpha' : 0.5},
-            peak_kwargs={'dot' : {'color' : colors['periodic'], 'ms' : ms, 'lw' : lw2},
-                         'shade' : {'color' : colors['periodic']},
-                         'width' : {'color' : colors['periodic'], 'alpha' : 0.75, 'lw' : lw2}})
+            peak_kwargs={'dot' : {'color' : PLT_COLORS['periodic'], 'ms' : ms1, 'lw' : lw2},
+                         'shade' : {'color' : PLT_COLORS['periodic']},
+                         'width' : {'color' : PLT_COLORS['periodic'], 'alpha' : 0.75, 'lw' : lw2}})
 
     # Get freqs for plotting, and convert to log if needed
     freqs = fm.freqs if not plt_log else np.log10(fm.freqs)
 
     ## Buffers: for spacing things out on the plot (scaled by plot values)
     x_buff1 = max(freqs) * 0.1
     x_buff2 = max(freqs) * 0.25
     y_buff1 = 0.15 * np.ptp(ax.get_ylim())
     shrink = 0.1
 
     # There is a bug in annotations for some perpendicular lines, so add small offset
     #   See: https://github.com/matplotlib/matplotlib/issues/12820. Fixed in 3.2.1.
     bug_buff = 0.000001
 
-    if annotate_peaks:
+    if annotate_peaks and fm.n_peaks_:
 
         # Extract largest peak, to annotate, grabbing gaussian params
         gauss = get_band_peak_fm(fm, fm.freq_range, attribute='gaussian_params')
 
         peak_ctr, peak_hgt, peak_wid = gauss
         bw_freqs = [peak_ctr - 0.5 * compute_fwhm(peak_wid),
                     peak_ctr + 0.5 * compute_fwhm(peak_wid)]
@@ -146,86 +150,86 @@
 
         # Annotate Peak CF
         ax.annotate('Center Frequency',
                     xy=(peak_ctr, peak_top),
                     xytext=(peak_ctr, peak_top+np.abs(0.6*peak_hgt)),
                     verticalalignment='center',
                     horizontalalignment='center',
-                    arrowprops=dict(facecolor=colors['periodic'], shrink=shrink),
-                    color=colors['periodic'], fontsize=fontsize)
+                    arrowprops=dict(facecolor=PLT_COLORS['periodic'], shrink=shrink),
+                    color=PLT_COLORS['periodic'], fontsize=fontsize)
 
         # Annotate Peak PW
         ax.annotate('Power',
                     xy=(peak_ctr, peak_top-0.3*peak_hgt),
                     xytext=(peak_ctr+x_buff1, peak_top-0.3*peak_hgt),
                     verticalalignment='center',
-                    arrowprops=dict(facecolor=colors['periodic'], shrink=shrink),
-                    color=colors['periodic'], fontsize=fontsize)
+                    arrowprops=dict(facecolor=PLT_COLORS['periodic'], shrink=shrink),
+                    color=PLT_COLORS['periodic'], fontsize=fontsize)
 
         # Annotate Peak BW
         bw_buff = (peak_ctr - bw_freqs[0])/2
         ax.annotate('Bandwidth',
                     xy=(peak_ctr-bw_buff+bug_buff, peak_top-(0.5*peak_hgt)),
                     xytext=(peak_ctr-bw_buff, peak_top-(1.5*peak_hgt)),
                     verticalalignment='center',
                     horizontalalignment='right',
-                    arrowprops=dict(facecolor=colors['periodic'], shrink=shrink),
-                    color=colors['periodic'], fontsize=fontsize, zorder=20)
+                    arrowprops=dict(facecolor=PLT_COLORS['periodic'], shrink=shrink),
+                    color=PLT_COLORS['periodic'], fontsize=fontsize, zorder=20)
 
     if annotate_aperiodic:
 
         # Annotate Aperiodic Offset
         #   Add a line to indicate offset, without adjusting plot limits below it
         ax.set_autoscaley_on(False)
         ax.plot([freqs[0], freqs[0]], [ax.get_ylim()[0], fm.fooofed_spectrum_[0]],
-                 color=colors['aperiodic'], lw=lw2, alpha=0.5)
+                color=PLT_COLORS['aperiodic'], linewidth=lw2, alpha=0.5)
         ax.annotate('Offset',
                     xy=(freqs[0]+bug_buff, fm.power_spectrum[0]-y_buff1),
                     xytext=(freqs[0]-x_buff1, fm.power_spectrum[0]-y_buff1),
                     verticalalignment='center',
                     horizontalalignment='center',
-                    arrowprops=dict(facecolor=colors['aperiodic'], shrink=shrink),
-                    color=colors['aperiodic'], fontsize=fontsize)
+                    arrowprops=dict(facecolor=PLT_COLORS['aperiodic'], shrink=shrink),
+                    color=PLT_COLORS['aperiodic'], fontsize=fontsize)
 
         # Annotate Aperiodic Knee
         if fm.aperiodic_mode == 'knee':
 
             # Find the knee frequency point to annotate
             knee_freq = compute_knee_frequency(fm.get_params('aperiodic', 'knee'),
                                                fm.get_params('aperiodic', 'exponent'))
             knee_freq = np.log10(knee_freq) if plt_log else knee_freq
             knee_pow = fm.power_spectrum[nearest_ind(freqs, knee_freq)]
 
             # Add a dot to the plot indicating the knee frequency
-            ax.plot(knee_freq, knee_pow, 'o', color=colors['aperiodic'], ms=ms*1.5, alpha=0.7)
+            ax.plot(knee_freq, knee_pow, 'o', color=PLT_COLORS['aperiodic'], ms=ms1*1.5, alpha=0.7)
 
             ax.annotate('Knee',
                         xy=(knee_freq, knee_pow),
                         xytext=(knee_freq-x_buff2, knee_pow-y_buff1),
                         verticalalignment='center',
-                        arrowprops=dict(facecolor=colors['aperiodic'], shrink=shrink),
-                        color=colors['aperiodic'], fontsize=fontsize)
+                        arrowprops=dict(facecolor=PLT_COLORS['aperiodic'], shrink=shrink),
+                        color=PLT_COLORS['aperiodic'], fontsize=fontsize)
 
         # Annotate Aperiodic Exponent
         mid_ind = int(len(freqs)/2)
         ax.annotate('Exponent',
                     xy=(freqs[mid_ind], fm.power_spectrum[mid_ind]),
                     xytext=(freqs[mid_ind]-x_buff2, fm.power_spectrum[mid_ind]-y_buff1),
                     verticalalignment='center',
-                    arrowprops=dict(facecolor=colors['aperiodic'], shrink=shrink),
-                    color=colors['aperiodic'], fontsize=fontsize)
+                    arrowprops=dict(facecolor=PLT_COLORS['aperiodic'], shrink=shrink),
+                    color=PLT_COLORS['aperiodic'], fontsize=fontsize)
 
     # Apply style to plot & tune grid styling
-    check_n_style(plot_style, ax, plt_log, True)
+    style_spectrum_plot(ax, plt_log, True)
     ax.grid(True, alpha=0.5)
 
     # Add labels to plot in the legend
-    da_patch = mpatches.Patch(color=colors['data'], label='Original Data')
-    ap_patch = mpatches.Patch(color=colors['aperiodic'], label='Aperiodic Parameters')
-    pe_patch = mpatches.Patch(color=colors['periodic'], label='Peak Parameters')
-    mo_patch = mpatches.Patch(color=colors['model'], label='Full Model')
+    da_patch = mpatches.Patch(color=PLT_COLORS['data'], label='Original Data')
+    ap_patch = mpatches.Patch(color=PLT_COLORS['aperiodic'], label='Aperiodic Parameters')
+    pe_patch = mpatches.Patch(color=PLT_COLORS['periodic'], label='Peak Parameters')
+    mo_patch = mpatches.Patch(color=PLT_COLORS['model'], label='Full Model')
 
     handles = [da_patch, ap_patch if annotate_aperiodic else None,
                pe_patch if annotate_peaks else None, mo_patch]
     handles = [el for el in handles if el is not None]
 
-    ax.legend(handles=handles, handlelength=1, fontsize='xx-large')
+    ax.legend(handles=handles, handlelength=1, fontsize='x-large')
```

### Comparing `fooof-1.0.0rc3/fooof/plts/aperiodic.py` & `fooof-1.1.0rc0/fooof/plts/aperiodic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,107 +1,105 @@
 """Plots for aperiodic fits and parameters."""
 
 from itertools import cycle
 
 import numpy as np
+import matplotlib.pyplot as plt
 
 from fooof.sim.gen import gen_freqs, gen_aperiodic
 from fooof.core.modutils import safe_import, check_dependency
-from fooof.plts.settings import FIGSIZE_PARAMS
-from fooof.plts.style import check_n_style, style_param_plot
-from fooof.plts.utils import check_ax, recursive_plot, check_plot_kwargs
+from fooof.plts.settings import PLT_FIGSIZES
+from fooof.plts.style import style_param_plot, style_plot
+from fooof.plts.utils import check_ax, recursive_plot, savefig, check_plot_kwargs
 
 plt = safe_import('.pyplot', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
 
+@savefig
+@style_plot
 @check_dependency(plt, 'matplotlib')
-def plot_aperiodic_params(aps, colors=None, labels=None,
-                          ax=None, plot_style=style_param_plot, **plot_kwargs):
+def plot_aperiodic_params(aps, colors=None, labels=None, ax=None, **plot_kwargs):
     """Plot aperiodic parameters as dots representing offset and exponent value.
 
     Parameters
     ----------
     aps : 2d array or list of 2d array
         Aperiodic parameters. Each row is a parameter set, as [Off, Exp] or [Off, Knee, Exp].
     colors : str or list of str, optional
         Color(s) to plot data.
     labels : list of str, optional
         Label(s) for plotted data, to be added in a legend.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
-    plot_style : callable, optional, default: style_param_plot
-        A function to call to apply styling & aesthetics to the plot.
     **plot_kwargs
-        Keyword arguments to pass into the plot call.
+        Keyword arguments to pass into the ``style_plot``.
     """
 
-    ax = check_ax(ax, plot_kwargs.pop('figsize', FIGSIZE_PARAMS))
+    ax = check_ax(ax, plot_kwargs.pop('figsize', PLT_FIGSIZES['params']))
 
     if isinstance(aps, list):
-        recursive_plot(aps, plot_aperiodic_params, ax, colors=colors, labels=labels,
-                       plot_style=plot_style, **plot_kwargs)
+        recursive_plot(aps, plot_aperiodic_params, ax, colors=colors, labels=labels)
 
     else:
 
         # Unpack data: offset as x; exponent as y
         xs, ys = aps[:, 0], aps[:, -1]
         sizes = plot_kwargs.pop('s', 150)
 
+        # Create the plot
         plot_kwargs = check_plot_kwargs(plot_kwargs, {'alpha' : 0.7})
         ax.scatter(xs, ys, sizes, c=colors, label=labels, **plot_kwargs)
 
     # Add axis labels
     ax.set_xlabel('Offset')
     ax.set_ylabel('Exponent')
 
-    check_n_style(plot_style, ax)
+    style_param_plot(ax)
 
 
+@savefig
+@style_plot
 @check_dependency(plt, 'matplotlib')
 def plot_aperiodic_fits(aps, freq_range, control_offset=False,
                         log_freqs=False, colors=None, labels=None,
-                        ax=None, plot_style=style_param_plot, **plot_kwargs):
+                        ax=None, **plot_kwargs):
     """Plot reconstructions of model aperiodic fits.
 
     Parameters
     ----------
     aps : 2d array
         Aperiodic parameters. Each row is a parameter set, as [Off, Exp] or [Off, Knee, Exp].
     freq_range : list of [float, float]
         The frequency range to plot the peak fits across, as [f_min, f_max].
-    control_offset : boolean, optonal, default: False
+    control_offset : boolean, optional, default: False
         Whether to control for the offset, by setting it to zero.
-    log_freqs : boolean, optonal, default: False
+    log_freqs : boolean, optional, default: False
         Whether to plot the x-axis in log space.
     colors : str or list of str, optional
         Color(s) to plot data.
     labels : list of str, optional
         Label(s) for plotted data, to be added in a legend.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
-    plot_style : callable, optional, default: style_param_plot
-        A function to call to apply styling & aesthetics to the plot.
     **plot_kwargs
-        Keyword arguments to pass into the plot call.
+        Keyword arguments to pass into the ``style_plot``.
     """
 
-    ax = check_ax(ax, plot_kwargs.pop('figsize', FIGSIZE_PARAMS))
+    ax = check_ax(ax, plot_kwargs.pop('figsize', PLT_FIGSIZES['params']))
 
     if isinstance(aps, list):
 
         if not colors:
             colors = cycle(plt.rcParams['axes.prop_cycle'].by_key()['color'])
 
-        recursive_plot(aps, plot_function=plot_aperiodic_fits, ax=ax,
-                       freq_range=tuple(freq_range),
-                       control_offset=control_offset,
-                       log_freqs=log_freqs, colors=colors, labels=labels,
-                       plot_style=plot_style, **plot_kwargs)
+        recursive_plot(aps, plot_aperiodic_fits, ax=ax, freq_range=tuple(freq_range),
+                       control_offset=control_offset, log_freqs=log_freqs, colors=colors,
+                       labels=labels, **plot_kwargs)
     else:
 
         freqs = gen_freqs(freq_range, 0.1)
         plt_freqs = np.log10(freqs) if log_freqs else freqs
 
         colors = colors[0] if isinstance(colors, list) else colors
 
@@ -114,27 +112,25 @@
                 # Copy the object to not overwrite any data
                 ap_params = ap_params.copy()
                 ap_params[0] = 0
 
             # Recreate & plot the aperiodic component from parameters
             ap_vals = gen_aperiodic(freqs, ap_params)
 
-            plot_kwargs = check_plot_kwargs(plot_kwargs, {'alpha' : 0.35, 'linewidth' : 1.25})
-            ax.plot(plt_freqs, ap_vals, color=colors, **plot_kwargs)
+            ax.plot(plt_freqs, ap_vals, color=colors, alpha=0.35, linewidth=1.25)
 
             # Collect a running average across components
             avg_vals = np.nansum(np.vstack([avg_vals, ap_vals]), axis=0)
 
         # Plot the average component
         avg = avg_vals / aps.shape[0]
         avg_color = 'black' if not colors else colors
-        ax.plot(plt_freqs, avg, color=avg_color, linewidth=plot_kwargs.get('linewidth')*3, label=labels)
+        ax.plot(plt_freqs, avg, linewidth=3.75, color=avg_color, label=labels)
 
     # Add axis labels
     ax.set_xlabel('log(Frequency)' if log_freqs else 'Frequency')
     ax.set_ylabel('log(Power)')
 
     # Set plot limit
     ax.set_xlim(np.log10(freq_range) if log_freqs else freq_range)
 
-    # Apply plot style
-    check_n_style(plot_style, ax)
+    style_param_plot(ax)
```

### Comparing `fooof-1.0.0rc3/fooof/plts/fg.py` & `fooof-1.1.0rc0/fooof/plts/fg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Plots for the FOOOFGroup object.
 
 Notes
 -----
 This file contains plotting functions that take as input a FOOOFGroup object.
 """
 
-from fooof.core.io import fname, fpath
 from fooof.core.errors import NoModelError
 from fooof.core.modutils import safe_import, check_dependency
-from fooof.plts.settings import FIGSIZE_GROUP
+from fooof.plts.settings import PLT_FIGSIZES
 from fooof.plts.templates import plot_scatter_1, plot_scatter_2, plot_hist
+from fooof.plts.utils import savefig
+from fooof.plts.style import style_plot
 
 plt = safe_import('.pyplot', 'matplotlib')
 gridspec = safe_import('.gridspec', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
 
+@savefig
 @check_dependency(plt, 'matplotlib')
-def plot_fg(fg, save_fig=False, file_name=None, file_path=None):
+def plot_fg(fg, save_fig=False, file_name=None, file_path=None, **plot_kwargs):
     """Plot a figure with subplots visualizing the parameters from a FOOOFGroup object.
 
     Parameters
     ----------
     fg : FOOOFGroup
         Object containing results from fitting a group of power spectra.
     save_fig : bool, optional, default: False
@@ -37,79 +39,90 @@
     NoModelError
         If the FOOOF object does not have model fit data available to plot.
     """
 
     if not fg.has_model:
         raise NoModelError("No model fit results are available, can not proceed.")
 
-    fig = plt.figure(figsize=FIGSIZE_GROUP)
+    fig = plt.figure(figsize=plot_kwargs.pop('figsize', PLT_FIGSIZES['group']))
     gs = gridspec.GridSpec(2, 2, wspace=0.4, hspace=0.25, height_ratios=[1, 1.2])
 
+    # Apply scatter kwargs to all subplots
+    scatter_kwargs = plot_kwargs
+    scatter_kwargs['all_axes'] = True
+
     # Aperiodic parameters plot
     ax0 = plt.subplot(gs[0, 0])
-    plot_fg_ap(fg, ax0)
+    plot_fg_ap(fg, ax0, **scatter_kwargs)
 
     # Goodness of fit plot
     ax1 = plt.subplot(gs[0, 1])
-    plot_fg_gf(fg, ax1)
+    plot_fg_gf(fg, ax1, **scatter_kwargs)
 
     # Center frequencies plot
     ax2 = plt.subplot(gs[1, :])
-    plot_fg_peak_cens(fg, ax2)
-
-    if save_fig:
-        if not file_name:
-            raise ValueError("Input 'file_name' is required to save out the plot.")
-        plt.savefig(fpath(file_path, fname(file_name, 'png')))
+    plot_fg_peak_cens(fg, ax2, **plot_kwargs)
 
 
+@savefig
+@style_plot
 @check_dependency(plt, 'matplotlib')
-def plot_fg_ap(fg, ax=None):
+def plot_fg_ap(fg, ax=None, **plot_kwargs):
     """Plot aperiodic fit parameters, in a scatter plot.
 
     Parameters
     ----------
     fg : FOOOFGroup
         Object to plot data from.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
+    **plot_kwargs
+        Keyword arguments to pass into the ``style_plot``.
     """
 
     if fg.aperiodic_mode == 'knee':
-        plot_scatter_2(fg.get_params('aperiodic_params', 'exponent'), 'Knee',
-                       fg.get_params('aperiodic_params', 'knee'), 'Exponent',
+        plot_scatter_2(fg.get_params('aperiodic_params', 'exponent'), 'Exponent',
+                       fg.get_params('aperiodic_params', 'knee'), 'Knee',
                        'Aperiodic Fit', ax=ax)
     else:
         plot_scatter_1(fg.get_params('aperiodic_params', 'exponent'), 'Exponent',
                        'Aperiodic Fit', ax=ax)
 
 
+@savefig
+@style_plot
 @check_dependency(plt, 'matplotlib')
-def plot_fg_gf(fg, ax=None):
+def plot_fg_gf(fg, ax=None, **plot_kwargs):
     """Plot goodness of fit results, in a scatter plot.
 
     Parameters
     ----------
     fg : FOOOFGroup
         Object to plot data from.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
+    **plot_kwargs
+        Keyword arguments to pass into the ``style_plot``.
     """
 
     plot_scatter_2(fg.get_params('error'), 'Error',
                    fg.get_params('r_squared'), 'R^2', 'Goodness of Fit', ax=ax)
 
 
+@savefig
+@style_plot
 @check_dependency(plt, 'matplotlib')
-def plot_fg_peak_cens(fg, ax=None):
+def plot_fg_peak_cens(fg, ax=None, **plot_kwargs):
     """Plot peak center frequencies, in a histogram.
 
     Parameters
     ----------
     fg : FOOOFGroup
         Object to plot data from.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
+    **plot_kwargs
+        Keyword arguments to pass into the ``style_plot``.
     """
 
     plot_hist(fg.get_params('peak_params', 0)[:, 0], 'Center Frequency',
               'Peaks - Center Frequencies', x_lims=fg.freq_range, ax=ax)
```

### Comparing `fooof-1.0.0rc3/fooof/plts/fm.py` & `fooof-1.1.0rc0/fooof/plts/fm.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 Notes
 -----
 This file contains plotting functions that take as input a FOOOF object.
 """
 
 import numpy as np
 
-from fooof.core.io import fname, fpath
 from fooof.core.utils import nearest_ind
 from fooof.core.modutils import safe_import, check_dependency
 from fooof.sim.gen import gen_periodic
 from fooof.utils.data import trim_spectrum
 from fooof.utils.params import compute_fwhm
-from fooof.plts.spectra import plot_spectrum
-from fooof.plts.settings import FIGSIZE_SPECTRAL
-from fooof.plts.utils import check_ax, check_plot_kwargs
-from fooof.plts.style import check_n_style, style_spectrum_plot
+from fooof.plts.spectra import plot_spectra
+from fooof.plts.settings import PLT_FIGSIZES, PLT_COLORS
+from fooof.plts.utils import check_ax, check_plot_kwargs, savefig
+from fooof.plts.style import style_spectrum_plot, style_plot
 
 plt = safe_import('.pyplot', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
 
+@savefig
+@style_plot
 @check_dependency(plt, 'matplotlib')
 def plot_fm(fm, plot_peaks=None, plot_aperiodic=True, plt_log=False, add_legend=True,
-            save_fig=False, file_name=None, file_path=None,
-            ax=None, plot_style=style_spectrum_plot,
-            data_kwargs=None, model_kwargs=None, aperiodic_kwargs=None, peak_kwargs=None):
+            save_fig=False, file_name=None, file_path=None, ax=None, data_kwargs=None,
+            model_kwargs=None, aperiodic_kwargs=None, peak_kwargs=None, **plot_kwargs):
     """Plot the power spectrum and model fit results from a FOOOF object.
 
     Parameters
     ----------
     fm : FOOOF
         Object containing a power spectrum and (optionally) results from fitting.
     plot_peaks : None or {'shade', 'dot', 'outline', 'line'}, optional
@@ -47,67 +47,59 @@
         Whether to save out a copy of the plot.
     file_name : str, optional
         Name to give the saved out file.
     file_path : str, optional
         Path to directory to save to. If None, saves to current directory.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
-    plot_style : callable, optional, default: style_spectrum_plot
-        A function to call to apply styling & aesthetics to the plot.
     data_kwargs, model_kwargs, aperiodic_kwargs, peak_kwargs : None or dict, optional
         Keyword arguments to pass into the plot call for each plot element.
+    **plot_kwargs
+        Keyword arguments to pass into the ``style_plot``.
 
     Notes
     -----
     Since FOOOF objects store power values in log spacing,
     the y-axis (power) is plotted in log spacing by default.
     """
 
-    ax = check_ax(ax, FIGSIZE_SPECTRAL)
+    ax = check_ax(ax, plot_kwargs.pop('figsize', PLT_FIGSIZES['spectral']))
 
     # Log settings - note that power values in FOOOF objects are already logged
     log_freqs = plt_log
     log_powers = False
 
     # Plot the data, if available
     if fm.has_data:
-        data_kwargs = check_plot_kwargs(data_kwargs, \
-            {'color' : 'black', 'linewidth' : 2.0,
-             'label' : 'Original Spectrum' if add_legend else None})
-        plot_spectrum(fm.freqs, fm.power_spectrum, log_freqs, log_powers,
-                      ax=ax, plot_style=None, **data_kwargs)
+        data_defaults = {'color' : PLT_COLORS['data'], 'linewidth' : 2.0,
+                         'label' : 'Original Spectrum' if add_legend else None}
+        data_kwargs = check_plot_kwargs(data_kwargs, data_defaults)
+        plot_spectra(fm.freqs, fm.power_spectrum, log_freqs, log_powers, ax=ax, **data_kwargs)
 
     # Add the full model fit, and components (if requested)
     if fm.has_model:
-        model_kwargs = check_plot_kwargs(model_kwargs, \
-            {'color' : 'red', 'linewidth' : 3.0, 'alpha' : 0.5,
-             'label' : 'Full Model Fit' if add_legend else None})
-        plot_spectrum(fm.freqs, fm.fooofed_spectrum_, log_freqs, log_powers,
-                      ax=ax, plot_style=None, **model_kwargs)
+        model_defaults = {'color' : PLT_COLORS['model'], 'linewidth' : 3.0, 'alpha' : 0.5,
+                          'label' : 'Full Model Fit' if add_legend else None}
+        model_kwargs = check_plot_kwargs(model_kwargs, model_defaults)
+        plot_spectra(fm.freqs, fm.fooofed_spectrum_, log_freqs, log_powers, ax=ax, **model_kwargs)
 
         # Plot the aperiodic component of the model fit
         if plot_aperiodic:
-            aperiodic_kwargs = check_plot_kwargs(aperiodic_kwargs, \
-                {'color' : 'blue', 'linewidth' : 3.0, 'alpha' : 0.5, 'linestyle' : 'dashed',
-                 'label' : 'Aperiodic Fit' if add_legend else None})
-            plot_spectrum(fm.freqs, fm._ap_fit, log_freqs, log_powers,
-                          ax=ax, plot_style=None, **aperiodic_kwargs)
+            aperiodic_defaults = {'color' : PLT_COLORS['aperiodic'], 'linewidth' : 3.0,
+                                  'alpha' : 0.5, 'linestyle' : 'dashed',
+                                  'label' : 'Aperiodic Fit' if add_legend else None}
+            aperiodic_kwargs = check_plot_kwargs(aperiodic_kwargs, aperiodic_defaults)
+            plot_spectra(fm.freqs, fm._ap_fit, log_freqs, log_powers, ax=ax, **aperiodic_kwargs)
 
         # Plot the periodic components of the model fit
         if plot_peaks:
-            _add_peaks(fm, plot_peaks, plt_log, ax=ax, peak_kwargs=peak_kwargs)
-
-    # Apply style to plot
-    check_n_style(plot_style, ax, log_freqs, True)
+            _add_peaks(fm, plot_peaks, plt_log, ax, peak_kwargs)
 
-    # Save out figure, if requested
-    if save_fig:
-        if not file_name:
-            raise ValueError("Input 'file_name' is required to save out the plot.")
-        plt.savefig(fpath(file_path, fname(file_name, 'png')))
+    # Apply default style to plot
+    style_spectrum_plot(ax, log_freqs, True)
 
 
 def _add_peaks(fm, approach, plt_log, ax, peak_kwargs):
     """Add peaks to a model plot.
 
     Parameters
     ----------
@@ -158,25 +150,26 @@
     fm : FOOOF
         FOOOF object containing results from fitting.
     plt_log : boolean
         Whether to plot the frequency values in log10 spacing.
     ax : matplotlib.Axes
         Figure axes upon which to plot.
     **plot_kwargs
-        Keyword arguments to pass into the plot call.
+        Keyword arguments to pass into the ``fill_between``.
     """
 
-    kwargs = check_plot_kwargs(plot_kwargs, {'color' : 'grey', 'alpha' : 0.25})
+    defaults = {'color' : PLT_COLORS['periodic'], 'alpha' : 0.25}
+    plot_kwargs = check_plot_kwargs(plot_kwargs, defaults)
 
-    for peak in fm.get_params('gaussian_params'):
+    for peak in fm.gaussian_params_:
 
         peak_freqs = np.log10(fm.freqs) if plt_log else fm.freqs
         peak_line = fm._ap_fit + gen_periodic(fm.freqs, peak)
 
-        ax.fill_between(peak_freqs, peak_line, fm._ap_fit, **kwargs)
+        ax.fill_between(peak_freqs, peak_line, fm._ap_fit, **plot_kwargs)
 
 
 def _add_peaks_dot(fm, plt_log, ax, **plot_kwargs):
     """Add a short line, from aperiodic to peak, with a dot at the top.
 
     Parameters
     ----------
@@ -186,27 +179,27 @@
         Whether to plot the frequency values in log10 spacing.
     ax : matplotlib.Axes
         Figure axes upon which to plot.
     **plot_kwargs
         Keyword arguments to pass into the plot call.
     """
 
-    kwargs = check_plot_kwargs(plot_kwargs,
-                               {'color' : 'grey', 'alpha' : 0.6, 'lw' : 2.5, 'ms' : 6})
+    defaults = {'color' : PLT_COLORS['periodic'], 'alpha' : 0.6, 'lw' : 2.5, 'ms' : 6}
+    plot_kwargs = check_plot_kwargs(plot_kwargs, defaults)
 
-    for peak in fm.get_params('peak_params'):
+    for peak in fm.peak_params_:
 
         ap_point = np.interp(peak[0], fm.freqs, fm._ap_fit)
         freq_point = np.log10(peak[0]) if plt_log else peak[0]
 
         # Add the line from the aperiodic fit up the tip of the peak
-        ax.plot([freq_point, freq_point], [ap_point, ap_point + peak[1]], **kwargs)
+        ax.plot([freq_point, freq_point], [ap_point, ap_point + peak[1]], **plot_kwargs)
 
         # Add an extra dot at the tip of the peak
-        ax.plot(freq_point, ap_point + peak[1], marker='o', **kwargs)
+        ax.plot(freq_point, ap_point + peak[1], marker='o', **plot_kwargs)
 
 
 def _add_peaks_outline(fm, plt_log, ax, **plot_kwargs):
     """Add an outline of each peak.
 
     Parameters
     ----------
@@ -216,29 +209,29 @@
         Whether to plot the frequency values in log10 spacing.
     ax : matplotlib.Axes
         Figure axes upon which to plot.
     **plot_kwargs
         Keyword arguments to pass into the plot call.
     """
 
-    kwargs = check_plot_kwargs(plot_kwargs,
-                               {'color' : 'green', 'alpha' : 0.7, 'lw' : 1.5})
+    defaults = {'color' : PLT_COLORS['periodic'], 'alpha' : 0.7, 'lw' : 1.5}
+    plot_kwargs = check_plot_kwargs(plot_kwargs, defaults)
 
-    for peak in fm.get_params('gaussian_params'):
+    for peak in fm.gaussian_params_:
 
         # Define the frequency range around each peak to plot - peak bandwidth +/- 3
         peak_range = [peak[0] - peak[2]*3, peak[0] + peak[2]*3]
 
         # Generate a peak reconstruction for each peak, and trim to desired range
         peak_line = fm._ap_fit + gen_periodic(fm.freqs, peak)
         peak_freqs, peak_line = trim_spectrum(fm.freqs, peak_line, peak_range)
 
         # Plot the peak outline
         peak_freqs = np.log10(peak_freqs) if plt_log else peak_freqs
-        ax.plot(peak_freqs, peak_line, **kwargs)
+        ax.plot(peak_freqs, peak_line, **plot_kwargs)
 
 
 def _add_peaks_line(fm, plt_log, ax, **plot_kwargs):
     """Add a long line, from the top of the plot, down through the peak, with an arrow at the top.
 
     Parameters
     ----------
@@ -248,23 +241,24 @@
         Whether to plot the frequency values in log10 spacing.
     ax : matplotlib.Axes
         Figure axes upon which to plot.
     **plot_kwargs
         Keyword arguments to pass into the plot call.
     """
 
-    kwargs = check_plot_kwargs(plot_kwargs,
-                               {'color' : 'green', 'alpha' : 0.7, 'lw' : 1.4, 'ms' : 10})
+    defaults = {'color' : PLT_COLORS['periodic'], 'alpha' : 0.7, 'lw' : 1.4, 'ms' : 10}
+    plot_kwargs = check_plot_kwargs(plot_kwargs, defaults)
 
     ylims = ax.get_ylim()
-    for peak in fm.get_params('peak_params'):
+
+    for peak in fm.peak_params_:
 
         freq_point = np.log10(peak[0]) if plt_log else peak[0]
-        ax.plot([freq_point, freq_point], ylims, '-', **kwargs)
-        ax.plot(freq_point, ylims[1], 'v', **kwargs)
+        ax.plot([freq_point, freq_point], ylims, '-', **plot_kwargs)
+        ax.plot(freq_point, ylims[1], 'v', **plot_kwargs)
 
 
 def _add_peaks_width(fm, plt_log, ax, **plot_kwargs):
     """Add a line across the width of peaks.
 
     Parameters
     ----------
@@ -275,31 +269,31 @@
     ax : matplotlib.Axes
         Figure axes upon which to plot.
     **plot_kwargs
         Keyword arguments to pass into the plot call.
 
     Notes
     -----
-    This line representents the bandwidth (width or gaussian standard deviation) of
+    This line represents the bandwidth (width or gaussian standard deviation) of
     the peak, though what is literally plotted is the full-width half-max.
     """
 
-    kwargs = check_plot_kwargs(plot_kwargs,
-                               {'color' : 'grey', 'alpha' : 0.6, 'lw' : 2.5, 'ms' : 6})
+    defaults = {'color' : PLT_COLORS['periodic'], 'alpha' : 0.6, 'lw' : 2.5, 'ms' : 6}
+    plot_kwargs = check_plot_kwargs(plot_kwargs, defaults)
 
     for peak in fm.gaussian_params_:
 
         peak_top = fm.power_spectrum[nearest_ind(fm.freqs, peak[0])]
         bw_freqs = [peak[0] - 0.5 * compute_fwhm(peak[2]),
                     peak[0] + 0.5 * compute_fwhm(peak[2])]
 
         if plt_log:
             bw_freqs = np.log10(bw_freqs)
 
-        ax.plot(bw_freqs, [peak_top-(0.5*peak[1]), peak_top-(0.5*peak[1])], **kwargs)
+        ax.plot(bw_freqs, [peak_top-(0.5*peak[1]), peak_top-(0.5*peak[1])], **plot_kwargs)
 
 
 # Collect all the possible `add_peak_*` functions together
 ADD_PEAK_FUNCS = {
     'shade' : _add_peaks_shade,
     'dot' : _add_peaks_dot,
     'outline' : _add_peaks_outline,
```

### Comparing `fooof-1.0.0rc3/fooof/plts/periodic.py` & `fooof-1.1.0rc0/fooof/plts/periodic.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,52 +3,50 @@
 from itertools import cycle
 
 import numpy as np
 
 from fooof.sim import gen_freqs
 from fooof.core.funcs import gaussian_function
 from fooof.core.modutils import safe_import, check_dependency
-from fooof.plts.settings import FIGSIZE_PARAMS
-from fooof.plts.style import check_n_style, style_param_plot
-from fooof.plts.utils import check_ax, recursive_plot, check_plot_kwargs
+from fooof.plts.settings import PLT_FIGSIZES
+from fooof.plts.style import style_param_plot, style_plot
+from fooof.plts.utils import check_ax, recursive_plot, savefig, check_plot_kwargs
 
 plt = safe_import('.pyplot', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
 
+@savefig
+@style_plot
 @check_dependency(plt, 'matplotlib')
-def plot_peak_params(peaks, freq_range=None, colors=None, labels=None,
-                     ax=None, plot_style=style_param_plot, **plot_kwargs):
+def plot_peak_params(peaks, freq_range=None, colors=None, labels=None, ax=None, **plot_kwargs):
     """Plot peak parameters as dots representing center frequency, power and bandwidth.
 
     Parameters
     ----------
     peaks : 2d array or list of 2d array
         Peak data. Each row is a peak, as [CF, PW, BW].
     freq_range : list of [float, float] , optional
         The frequency range to plot the peak parameters across, as [f_min, f_max].
     colors : str or list of str, optional
         Color(s) to plot data.
     labels : list of str, optional
         Label(s) for plotted data, to be added in a legend.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
-    plot_style : callable, optional, default: style_param_plot
-        A function to call to apply styling & aesthetics to the plot.
     **plot_kwargs
-        Keyword arguments to pass into the plot call.
+        Keyword arguments to pass into the ``style_plot``.
     """
 
-    ax = check_ax(ax, plot_kwargs.pop('figsize', FIGSIZE_PARAMS))
+    ax = check_ax(ax, plot_kwargs.pop('figsize', PLT_FIGSIZES['params']))
 
     # If there is a list, use recurse function to loop across arrays of data and plot them
     if isinstance(peaks, list):
-        recursive_plot(peaks, plot_peak_params, ax, colors=colors, labels=labels,
-                       plot_style=plot_style, **plot_kwargs)
+        recursive_plot(peaks, plot_peak_params, ax, colors=colors, labels=labels)
 
     # Otherwise, plot the array of data
     else:
 
         # Unpack data: CF as x; PW as y; BW as size
         xs, ys = peaks[:, 0], peaks[:, 1]
         sizes = peaks[:, 2] * plot_kwargs.pop('s', 150)
@@ -62,19 +60,20 @@
     ax.set_ylabel('Power')
 
     # Set plot limits
     if freq_range:
         ax.set_xlim(freq_range)
     ax.set_ylim([0, ax.get_ylim()[1]])
 
-    check_n_style(plot_style, ax)
+    style_param_plot(ax)
 
 
-def plot_peak_fits(peaks, freq_range=None, colors=None, labels=None,
-                   ax=None, plot_style=style_param_plot, **plot_kwargs):
+@savefig
+@style_plot
+def plot_peak_fits(peaks, freq_range=None, colors=None, labels=None, ax=None, **plot_kwargs):
     """Plot reconstructions of model peak fits.
 
     Parameters
     ----------
     peaks : 2d array
         Peak data. Each row is a peak, as [CF, PW, BW].
     freq_range : list of [float, float] , optional
@@ -82,31 +81,28 @@
         If not provided, defaults to +/- 4 around given peak center frequencies.
     colors : str or list of str, optional
         Color(s) to plot data.
     labels : list of str, optional
         Label(s) for plotted data, to be added in a legend.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
-    plot_style : callable, optional, default: style_param_plot
-        A function to call to apply styling & aesthetics to the plot.
     **plot_kwargs
         Keyword arguments to pass into the plot call.
     """
 
-    ax = check_ax(ax, plot_kwargs.pop('figsize', FIGSIZE_PARAMS))
+    ax = check_ax(ax, plot_kwargs.pop('figsize', PLT_FIGSIZES['params']))
 
     if isinstance(peaks, list):
 
         if not colors:
             colors = cycle(plt.rcParams['axes.prop_cycle'].by_key()['color'])
 
         recursive_plot(peaks, plot_function=plot_peak_fits, ax=ax,
                        freq_range=tuple(freq_range) if freq_range else freq_range,
-                       colors=colors, labels=labels,
-                       plot_style=plot_style, **plot_kwargs)
+                       colors=colors, labels=labels, **plot_kwargs)
 
     else:
 
         if not freq_range:
 
             # Extract all the CF values, excluding any NaNs
             cfs = peaks[~np.isnan(peaks[:, 0]), 0]
@@ -124,28 +120,27 @@
 
         avg_vals = np.zeros(shape=[len(freqs)])
 
         for peak_params in peaks:
 
             # Create & plot the peak model from parameters
             peak_vals = gaussian_function(freqs, *peak_params)
-            plot_kwargs = check_plot_kwargs(plot_kwargs, {'alpha' : 0.35, 'linewidth' : 1.25})
-            ax.plot(freqs, peak_vals, color=colors, **plot_kwargs)
+            ax.plot(freqs, peak_vals, color=colors, alpha=0.35, linewidth=1.25)
 
             # Collect a running average average peaks
             avg_vals = np.nansum(np.vstack([avg_vals, peak_vals]), axis=0)
 
         # Plot the average across all components
         avg = avg_vals / peaks.shape[0]
         avg_color = 'black' if not colors else colors
-        ax.plot(freqs, avg, color=avg_color, linewidth=plot_kwargs.get('linewidth')*3, label=labels)
+        ax.plot(freqs, avg, color=avg_color, linewidth=3.75, label=labels)
 
     # Add axis labels
     ax.set_xlabel('Frequency')
     ax.set_ylabel('log(Power)')
 
     # Set plot limits
     ax.set_xlim(freq_range)
     ax.set_ylim([0, ax.get_ylim()[1]])
 
     # Apply plot style
-    check_n_style(plot_style, ax)
+    style_param_plot(ax)
```

### Comparing `fooof-1.0.0rc3/fooof/plts/templates.py` & `fooof-1.1.0rc0/fooof/plts/templates.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/plts/utils.py` & `fooof-1.1.0rc0/fooof/plts/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 -----
 These utility functions should be considered private.
 They are not expected to be called directly by the user.
 """
 
 from itertools import repeat
 from collections.abc import Iterator
+from functools import wraps
 
 import numpy as np
 
+from fooof.core.io import fname, fpath
 from fooof.core.modutils import safe_import
 from fooof.core.utils import resolve_aliases
-from fooof.plts.settings import ALPHA_LEVELS, PLT_ALIASES
+from fooof.plts.settings import PLT_ALPHA_LEVELS, PLT_ALIASES
 
 plt = safe_import('.pyplot', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
 
 def check_ax(ax, figsize=None):
@@ -52,17 +54,17 @@
 
     Returns
     -------
     alpha : float
         Value for alpha to use for plotting.
     """
 
-    for ke, va in ALPHA_LEVELS.items():
-        if n_points > ke:
-            alpha = va
+    for key, val in PLT_ALPHA_LEVELS.items():
+        if n_points > key:
+            alpha = val
 
     return alpha
 
 
 def add_shades(ax, shades, colors='r', add_center=False, logged=False):
     """Add shaded regions to a plot.
 
@@ -76,15 +78,15 @@
         Color(s) to plot shades.
     add_center : boolean, default: False
         Whether to add a line at the center point of the shaded regions.
     logged : boolean, default: False
         Whether the shade values should be logged before applying to plot axes.
     """
 
-    # If only only one shade region is specified, this embeds in a list, so that the loop works
+    # If only one shade region is specified, this embeds in a list, so that the loop works
     if not isinstance(shades[0], list):
         shades = [shades]
 
     colors = repeat(colors) if not isinstance(colors, list) else colors
 
     for shade, color in zip(shades, colors):
 
@@ -167,7 +169,58 @@
         return defaults
 
     for key, value in resolve_aliases(defaults, PLT_ALIASES).items():
         if key not in resolve_aliases(plot_kwargs, PLT_ALIASES):
             plot_kwargs[key] = value
 
     return plot_kwargs
+
+
+def savefig(func):
+    """Decorator function to save out figures."""
+
+    @wraps(func)
+    def decorated(*args, **kwargs):
+
+        # Grab file name and path arguments, if they are in kwargs
+        file_name = kwargs.pop('file_name', None)
+        file_path = kwargs.pop('file_path', None)
+
+        # Check for an explicit argument for whether to save figure or not
+        #   Defaults to saving when file name given (since bool(str)->True; bool(None)->False)
+        save_fig = kwargs.pop('save_fig', bool(file_name))
+
+        # Check any collect any other plot keywords
+        save_kwargs = kwargs.pop('save_kwargs', {})
+        save_kwargs.setdefault('bbox_inches', 'tight')
+
+        # Check and collect whether to close the plot
+        close = kwargs.pop('close', None)
+
+        func(*args, **kwargs)
+
+        if save_fig:
+            save_figure(file_name, file_path, close, **save_kwargs)
+
+    return decorated
+
+
+def save_figure(file_name, file_path=None, close=False, **save_kwargs):
+    """Save out a figure.
+
+    Parameters
+    ----------
+    file_name : str
+        File name for the figure file to save out.
+    file_path : str or Path
+        Path for where to save out the figure to.
+    close : bool, optional, default: False
+        Whether to close the plot after saving.
+    save_kwargs
+        Additional arguments to pass into the save function.
+    """
+
+    full_path = fpath(file_path, fname(file_name, 'png'))
+    plt.savefig(full_path, **save_kwargs)
+
+    if close:
+        plt.close()
```

### Comparing `fooof-1.0.0rc3/fooof/sim/gen.py` & `fooof-1.1.0rc0/fooof/sim/gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Functions for generating model components and simulated power spectra."""
 
 import numpy as np
 
 from fooof.core.utils import check_iter, check_flat
-from fooof.core.funcs import gaussian_function
 from fooof.core.funcs import get_ap_func, get_pe_func, infer_ap_func
 
 from fooof.sim.params import collect_sim_params
 from fooof.sim.transform import rotate_spectrum, compute_rotation_offset
 
 ###################################################################################################
 ###################################################################################################
@@ -22,14 +21,20 @@
     freq_res : float
         Frequency resolution of desired frequency vector.
 
     Returns
     -------
     freqs : 1d array
         Frequency values, in linear spacing.
+
+    Examples
+    --------
+    Generate a vector of frequency values from 1 to 50:
+
+    >>> freqs = gen_freqs([1, 50], freq_res=0.5)
     """
 
     # The end value has something added to it, to make sure the last value is included
     #   It adds a fraction to not accidentally include points beyond range
     #   due to rounding / or uneven division of the freq_res into range to simulate
     freqs = np.arange(freq_range[0], freq_range[1] + (0.5 * freq_res), freq_res)
 
@@ -99,42 +104,43 @@
 
     - Note that rotating power spectra changes the offset.
 
       * If you specify an offset value to simulate as well as 'f_rotation', the returned
         spectrum will NOT have the requested offset. It instead will have the offset
         value required to create the requested aperiodic exponent with the requested
         rotation point.
-      * If you return SimParams, the recorded offset will be actual calculated offset
-        of the data, and not the value entered.
+      * If you return SimParams, the recorded offset will be the calculated offset
+        of the data post rotation, and not the entered value.
 
     - You cannot rotate power spectra simulated with a knee.
 
       * The procedure we use to rotate does not support spectra with a knee, and so
         setting 'f_rotation' with a knee will lead to an error.
 
     Examples
     --------
     Generate a power spectrum with a single peak, at 10 Hz:
 
-    >>> freqs, psd = gen_power_spectrum([1, 50], [0, 2], [10, 0.5, 1])
+    >>> freqs, powers = gen_power_spectrum([1, 50], [0, 2], [10, 0.5, 1])
 
     Generate a power spectrum with alpha and beta peaks:
 
-    >>> freqs, psd = gen_power_spectrum([1, 50], [0, 2], [[10, 0.5, 1], [20, 0.5, 1]])
+    >>> freqs, powers = gen_power_spectrum([1, 50], [0, 2], [[10, 0.5, 1], [20, 0.5, 1]])
 
     Generate a power spectrum, that was rotated around a particular frequency point:
 
-    >>> freqs, psd = gen_power_spectrum([1, 50], [None, 2], [10, 0.5, 1], f_rotation=15)
+    >>> freqs, powers = gen_power_spectrum([1, 50], [None, 2], [10, 0.5, 1], f_rotation=15)
     """
 
     freqs = gen_freqs(freq_range, freq_res)
 
     if f_rotation:
 
-        powers = gen_rotated_power_vals(freqs, aperiodic_params, periodic_params, nlv, f_rotation)
+        powers = gen_rotated_power_vals(freqs, aperiodic_params,
+                                        check_flat(periodic_params), nlv, f_rotation)
 
         # The rotation changes the offset, so recalculate it's value & update params
         new_offset = compute_rotation_offset(aperiodic_params[1], f_rotation)
         aperiodic_params = [new_offset, aperiodic_params[1]]
 
     else:
 
@@ -215,48 +221,48 @@
 
     - Note that rotating power spectra changes the offset.
 
       * If you specify an offset value to simulate as well as 'f_rotation', the returned
         spectrum will NOT have the requested offset. It instead will have the offset
         value required to create the requested aperiodic exponent with the requested
         rotation point.
-      * If you return SimParams, the recorded offset will be actual calculated offset
-        of the data, and not the value entered.
+      * If you return SimParams, the recorded offset will be the calculated offset
+        of the data post rotation, and not the entered value.
 
     - You cannot rotate power spectra simulated with a knee.
 
       * The procedure we use to rotate does not support spectra with a knee, and so
         setting 'f_rotation' with a knee will lead to an error.
 
     Examples
     --------
     Generate 2 power spectra using the same parameters:
 
-    >>> freqs, psds = gen_group_power_spectra(2, [1, 50], [0, 2], [10, 0.5, 1])
+    >>> freqs, powers = gen_group_power_spectra(2, [1, 50], [0, 2], [10, 0.5, 1])
 
     Generate 10 power spectra, randomly sampling possible parameters:
 
     >>> from fooof.sim.params import param_sampler
     >>> ap_opts = param_sampler([[0, 1.0], [0, 1.5], [0, 2]])
     >>> pe_opts = param_sampler([[], [10, 0.5, 1], [10, 0.5, 1, 20, 0.25, 1]])
-    >>> freqs, psds = gen_group_power_spectra(10, [1, 50], ap_opts, pe_opts)
+    >>> freqs, powers = gen_group_power_spectra(10, [1, 50], ap_opts, pe_opts)
 
     Generate 5 power spectra, rotated around 20 Hz:
 
     >>> ap_params = [[None, 1], [None, 1.25], [None, 1.5], [None, 1.75], [None, 2]]
     >>> pe_params = [10, 0.5, 1]
-    >>> freqs, psds = gen_group_power_spectra(5, [1, 50], ap_params, pe_params, f_rotation=20)
+    >>> freqs, powers = gen_group_power_spectra(5, [1, 50], ap_params, pe_params, f_rotation=20)
 
     Generate power spectra stepping across exponent values, and return parameter values:
 
     >>> from fooof.sim.params import Stepper, param_iter
     >>> ap_params = param_iter([0, Stepper(1, 2, 0.25)])
     >>> pe_params = [10, 0.5, 1]
-    >>> freqs, psds, sps = gen_group_power_spectra(5, [1, 50], ap_params, pe_params,
-    ...                                            return_params=True)
+    >>> freqs, powers, sps = gen_group_power_spectra(5, [1, 50], ap_params, pe_params,
+    ...                                              return_params=True)
     """
 
     # Initialize things
     freqs = gen_freqs(freq_range, freq_res)
     powers = np.zeros([n_spectra, len(freqs)])
     sim_params = [None] * n_spectra
 
@@ -266,19 +272,19 @@
     nlvs = check_iter(nlvs, n_spectra)
     f_rots = check_iter(f_rotation, n_spectra)
 
     # Simulate power spectra
     for ind, ap, pe, nlv, f_rot in zip(range(n_spectra), ap_params, pe_params, nlvs, f_rots):
 
         if f_rotation:
-            powers = gen_rotated_power_vals(freqs, ap, pe, nlv, f_rot)
+            powers[ind, :] = gen_rotated_power_vals(freqs, ap, check_flat(pe), nlv, f_rot)
             aperiodic_params = [compute_rotation_offset(ap[1], f_rot), ap[1]]
 
         else:
-            powers[ind, :] = gen_power_vals(freqs, ap, pe, nlv)
+            powers[ind, :] = gen_power_vals(freqs, ap, check_flat(pe), nlv)
 
         sim_params[ind] = collect_sim_params(ap, pe, nlv)
 
     if return_params:
         return freqs, powers, sim_params
     else:
         return freqs, powers
@@ -426,15 +432,15 @@
     ValueError
         If a rotation is requested on a power spectrum with a knee, as this is not supported.
     """
 
     if len(aperiodic_params) == 3:
         raise ValueError('Cannot rotate power spectra generated with a knee.')
 
-    powers = gen_power_vals(freqs, [0, 0], check_flat(periodic_params), nlv)
+    powers = gen_power_vals(freqs, [0, 0], periodic_params, nlv)
     powers = rotate_spectrum(freqs, powers, aperiodic_params[1], f_rotation)
 
     return powers
 
 
 def gen_model(freqs, aperiodic_params, periodic_params, return_components=False):
     """Generate a power spectrum model for a given parameter definition.
```

### Comparing `fooof-1.0.0rc3/fooof/sim/params.py` & `fooof-1.1.0rc0/fooof/sim/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 from fooof.data import SimParams
 
 ###################################################################################################
 ###################################################################################################
 
 def collect_sim_params(aperiodic_params, periodic_params, nlv):
-    """Collect sim parameters together into a SimParams object.
+    """Collect simulation parameters into a SimParams object.
 
     Parameters
     ----------
     aperiodic_params : list of float
         Parameters of the aperiodic component of the power spectrum.
     periodic_params : list of float or list of list of float
         Parameters of the periodic component of the power spectrum.
-    nlv : float, optional, default: 0.005
+    nlv : float
         Noise level of the power spectrum.
 
     Returns
     -------
     SimParams
         Object containing the simulation parameters.
     """
@@ -37,53 +37,51 @@
 
 def update_sim_ap_params(sim_params, delta, field=None):
     """Update the aperiodic parameter definition in a SimParams object.
 
     Parameters
     ----------
     sim_params : SimParams
-        Object storing the current parameter definitions.
-    delta : float or list
+        Object storing the current parameter definition.
+    delta : float or list of float
         Value(s) by which to update the parameters.
     field : {'offset', 'knee', 'exponent'} or list of string
-        Field of the aperiodic parameters to update.
+        Field of the aperiodic parameter(s) to update.
 
     Returns
     -------
     new_sim_params : SimParams
-        Updated object storing the new parameter definitions.
+        Updated object storing the new parameter definition.
 
     Raises
     ------
     InconsistentDataError
         If the input parameters and update values are inconsistent.
-
-    Notes
-    -----
-    SimParams is a `namedtuple`, which is immutable.
-    Therefore, this function constructs and returns a new `SimParams` object.
     """
 
+    # Grab the aperiodic parameters that need updating
     ap_params = sim_params.aperiodic_params.copy()
 
+    # If field isn't specified, check shapes line up and update across parameters
     if not field:
         if not len(ap_params) == len(delta):
             raise InconsistentDataError("The number of items to update and "
                                         "number of new values is inconsistent.")
         ap_params = [param + update for param, update in zip(ap_params, delta)]
 
+    # If labels are given, update deltas according to their labels
     else:
-        field = list([field]) if not isinstance(field, list) else field
-        delta = list([delta]) if not isinstance(delta, list) else delta
-
-        for cur_field, cur_delta in zip(field, delta):
-            dat_ind = get_indices(infer_ap_func(sim_params.aperiodic_params))[cur_field]
-            ap_params[dat_ind] = ap_params[dat_ind] + cur_delta
+        # This loop checks & casts to list, to work for single or multiple passed in values
+        for cur_field, cur_delta in zip(list([field]) if not isinstance(field, list) else field,
+                                        list([delta]) if not isinstance(delta, list) else delta):
+            data_ind = get_indices(infer_ap_func(ap_params))[cur_field]
+            ap_params[data_ind] = ap_params[data_ind] + cur_delta
 
-    new_sim_params = SimParams(ap_params, *sim_params[1:])
+    # Replace parameters. Note that this copies a new object, as data objects are immutable
+    new_sim_params = sim_params._replace(aperiodic_params=ap_params)
 
     return new_sim_params
 
 
 class Stepper():
     """Object for stepping across parameter values.
 
@@ -98,14 +96,20 @@
 
     Attributes
     ----------
     len : int
         Length of generator range.
     data : iterator
         Set of specified parameters to iterate across.
+
+    Examples
+    --------
+    Define a stepper object for center frequency values for an alpha peak:
+
+    >>> alpha_cf_steps = Stepper(8, 12.5, 0.5)
     """
 
     def __init__(self, start, stop, step):
         """Initialize a Stepper object."""
 
         self._check_values(start, stop, step)
 
@@ -135,15 +139,15 @@
         ----------
         start, stop, step : float
             Definition of the parameter range to iterate over.
 
         Raises
         ------
         ValueError
-            If the input values to define the iteration range are inconsistent.
+            If the given values for defining the iteration range are inconsistent.
         """
 
         if any(ii < 0 for ii in [start, stop, step]):
             raise ValueError("Inputs 'start', 'stop', and 'step' should all be positive values.")
 
         if not start < stop:
             raise ValueError("Input 'start' should be less than 'stop'.")
@@ -161,15 +165,15 @@
         Parameters over which to iterate, including a Stepper object.
         The Stepper defines the iterated parameter and its range.
         Floats define the other parameters, that will be held constant.
 
     Yields
     ------
     list of floats
-        Next generated list of parameters across the range.
+        Next generated list of parameters.
 
     Raises
     ------
     ValueError
         If the number of Stepper objects given is greater than one.
 
     Examples
@@ -293,11 +297,11 @@
         params = check_flat(params)
         jitters = check_flat(jitters)
 
     # While loop allows the generator to be called an arbitrary number of times
     while True:
 
         out_params = [None] * len(params)
-        for ind, (p1, j1) in enumerate(zip(params, jitters)):
-            out_params[ind] = p1 + np.random.normal(0, j1)
+        for ind, (param, jitter) in enumerate(zip(params, jitters)):
+            out_params[ind] = param + np.random.normal(0, jitter)
 
         yield out_params
```

### Comparing `fooof-1.0.0rc3/fooof/sim/transform.py` & `fooof-1.1.0rc0/fooof/sim/transform.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,29 +37,37 @@
     Notes
     -----
     Rotating in log-log spacing is equivalent to multiplying with a 1/f shaped mask that is:
 
     - unity at the rotation frequency
     - has an exponent of the desired delta exponent
 
-    This mask, when applied to a spectrum, as 'spectrum * mask should result in:
+    This mask, when applied to a spectrum as 'spectrum * mask', should result in:
 
     - rotated_spectrum = 1/f^(original_exponent + delta_exponent), where
     - spectrum[rotation_frequency] == rotated spectrum[rotation_frequency]
 
     This mask is defined as:
 
     - mask = (freqs / rotation_frequency) ** -delta_exponent
 
     Note that this approach / function should only be applied to spectra without a knee:
 
     - If using simulated data, this is spectra created in 'fixed' mode.
     - This is because the rotation applied is inconsistent with the formulation of spectra
       with a knee. This transformation will change them in an unspecified way, not just
       limited to doing the rotation.
+
+    Examples
+    --------
+    Rotate a simulated spectrum, changing the exponent around a rotation point of 25 Hz:
+
+    >>> from fooof.sim.gen import gen_power_spectrum
+    >>> freqs, powers = gen_power_spectrum([1, 50], [1, 1], [10, 0.5, 1])
+    >>> rotated_powers = rotate_spectrum(freqs, powers, 0.5, 25)
     """
 
     # Rotations are undefined for frequency value of exactly zero
     #   We also do not support (in this implementation) negative frequencies
     if f_rotation <= 0.:
         raise ValueError("The rotation frequency cannot be less than or equal to zero.")
 
@@ -82,14 +90,22 @@
         - positive values are an upwards translation
         - negative are are a downwards translation
 
     Returns
     -------
     translated_spectrum : 1d array
         Translated power spectrum.
+
+    Examples
+    --------
+    Translate a simulated spectrum, moving the offset up:
+
+    >>> from fooof.sim.gen import gen_power_spectrum
+    >>> freqs, powers = gen_power_spectrum([1, 50], [1, 1], [10, 0.5, 1])
+    >>> translated_powers = translate_spectrum(powers, 0.5)
     """
 
     translated_spectrum = np.power(10, delta_offset, dtype='float') * power_spectrum
 
     return translated_spectrum
 
 
@@ -122,14 +138,22 @@
     Notes
     -----
     Warning: This function should only be applied to spectra without a knee.
     If using simulated data, this is spectra created in 'fixed' mode.
     This is because the rotation applied is inconsistent with
     the formulation of knee spectra, and will change them in an
     unspecified way, not just limited to doing the rotation.
+
+    Examples
+    --------
+    Rotate a simulated spectrum, changing the exponent around a rotation point of 25 Hz:
+
+    >>> from fooof.sim.gen import gen_power_spectrum
+    >>> freqs, powers, sp = gen_power_spectrum([1, 50], [1, 1], [10, 0.5, 1], return_params=True)
+    >>> rotated_powers, new_sp = rotate_sim_spectrum(freqs, powers, 0.5, 25, sp)
     """
 
     rotated_spectrum = rotate_spectrum(freqs, power_spectrum, delta_exponent, f_rotation)
     delta_offset = compute_rotation_offset(delta_exponent, f_rotation)
 
     new_sim_params = update_sim_ap_params(sim_params, [delta_offset, delta_exponent])
 
@@ -153,14 +177,22 @@
 
     Returns
     -------
     translated_spectrum : 1d array
         Translated power spectrum.
     new_sim_params : SimParams
         New parameter definitions.
+
+    Examples
+    --------
+    Translate a simulated spectrum, moving the offset up:
+
+    >>> from fooof.sim.gen import gen_power_spectrum
+    >>> freqs, powers, sp = gen_power_spectrum([1, 50], [1, 1], [10, 0.5, 1], return_params=True)
+    >>> translated_powers, new_sp = translate_sim_spectrum(powers, 0.5, sp)
     """
 
     translated_spectrum = translate_spectrum(power_spectrum, delta_offset)
     new_sim_params = update_sim_ap_params(sim_params, delta_offset, 'offset')
 
     return translated_spectrum, new_sim_params
 
@@ -175,14 +207,20 @@
     f_rotation : float
         The frequency value, in Hz, where rotation is applied.
 
     Returns
     -------
     float
         The amount the offset will change for the specified exponent change.
+
+    Examples
+    --------
+    Calculate the induced change in offset of a change in exponent of 0.5 at 25 Hz:
+
+    >>> delta_offset = compute_rotation_offset(0.5, 25)
     """
 
     return -np.log10(f_rotation) * -delta_exponent
 
 
 def compute_rotation_frequency(delta_exponent_b, f_rotation_b, delta_exponent_c, f_rotation_c):
     """Calculate the rotation frequency between two rotated power spectra.
@@ -218,11 +256,17 @@
     - B = A*(f_rotation_b/freqs)^delta_exponent_b
     - C = A*(f_rotation_c/freqs)^delta_exponent_c
 
     Therefore, what you want is f_rotation_bc, which is the frequency where B==C.
 
     To find this, we can plug everything back into the equation, to find where
     B[freqs] == C[freqs], which is how we arrive at the solution below.
+
+    Examples
+    --------
+    Calculate the rotation frequency between two transformed power spectra:
+
+    >>> f_rotation = compute_rotation_frequency(0.5, 25, -0.25, 10)
     """
 
     return (((f_rotation_c**delta_exponent_c) / (f_rotation_b**delta_exponent_b))) ** \
-         (1/(delta_exponent_c-delta_exponent_b))
+        (1/(delta_exponent_c-delta_exponent_b))
```

### Comparing `fooof-1.0.0rc3/fooof/tests/analysis/test_error.py` & `fooof-1.1.0rc0/fooof/tests/analysis/test_error.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,20 +7,28 @@
 
 def test_compute_pointwise_error_fm(tfm):
 
     errs = compute_pointwise_error_fm(tfm, False, True)
     assert np.all(errs)
 
 def test_compute_pointwise_error_fm_plt(tfm, skip_if_no_mpl):
-    """Run a seperate test to run with plot pass-through."""
+    """Run a separate test to run with plot pass-through."""
 
     compute_pointwise_error_fm(tfm, True, False)
 
 def test_compute_pointwise_error_fg(tfg):
 
     errs = compute_pointwise_error_fg(tfg, False, True)
     assert np.all(errs)
 
 def test_compute_pointwise_error_fg_plt(tfg, skip_if_no_mpl):
-    """Run a seperate test to run with plot pass-through."""
+    """Run a separate test to run with plot pass-through."""
 
     compute_pointwise_error_fg(tfg, True, False)
+
+def test_compute_pointwise_error():
+
+    d1 = np.ones(5) * 2
+    d2 = np.ones(5)
+
+    errs = compute_pointwise_error(d1, d2)
+    assert np.array_equal(errs, np.array([1, 1, 1, 1, 1]))
```

### Comparing `fooof-1.0.0rc3/fooof/tests/analysis/test_periodic.py` & `fooof-1.1.0rc0/fooof/tests/analysis/test_periodic.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,21 +34,24 @@
     # Test single result
     assert np.array_equal(get_band_peak(data, [10, 12]), [10, 1, 1.8])
 
     # Test no results - returns nan
     assert np.all(np.isnan(get_band_peak(data, [4, 8])))
 
     # Test multiple results - return all
-    assert np.array_equal(get_band_peak(data, [10, 15], ret_one=False), [[10, 1, 1.8], [14, 2, 4]])
+    assert np.array_equal(get_band_peak(data, [10, 15], select_highest=False),
+                          np.array([[10, 1, 1.8], [14, 2, 4]]))
 
     # Test multiple results - return one
-    assert np.array_equal(get_band_peak(data, [10, 15], ret_one=True), [14, 2, 4])
+    assert np.array_equal(get_band_peak(data, [10, 15], select_highest=True),
+                          np.array([14, 2, 4]))
 
     # Test applying a threshold
-    assert np.array_equal(get_band_peak(data, [10, 15], threshold=1.5, ret_one=False), [14, 2, 4])
+    assert np.array_equal(get_band_peak(data, [10, 15], threshold=1.5, select_highest=False),
+                          np.array([14, 2, 4]))
 
 def test_get_highest_peak():
 
     data = np.array([[10, 1, 1.8], [14, 2, 4], [12, 3, 2]])
 
     assert np.array_equal(get_highest_peak(data), [12, 3, 2])
 
@@ -56,15 +59,16 @@
 
     # Check it works, with a standard power threshold
     data = np.array([[10, 1, 1.8], [14, 2, 4], [12, 3, 2.5]])
     assert np.array_equal(threshold_peaks(data, 2.5), np.array([[12, 3, 2.5]]))
 
     # Check it works using a bandwidth threshold
     data = np.array([[10, 1, 1.8], [14, 2, 4], [12, 3, 2.5]])
-    assert np.array_equal(threshold_peaks(data, 2, param='BW'), np.array([[14, 2, 4], [12, 3, 2.5]]))
+    assert np.array_equal(threshold_peaks(data, 2, param='BW'),
+                          np.array([[14, 2, 4], [12, 3, 2.5]]))
 
     # Check it works with an [n_peaks, 4] array, as from FOOOFGroup
     data = np.array([[10, 1, 1.8, 0], [13, 1, 2, 2], [14, 2, 4, 2]])
     assert np.array_equal(threshold_peaks(data, 1.5), np.array([[14, 2, 4, 2]]))
 
 def test_empty_inputs():
```

### Comparing `fooof-1.0.0rc3/fooof/tests/bands/test_bands.py` & `fooof-1.1.0rc0/fooof/tests/bands/test_bands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Test functions for fooof.data.bands."""
 
-from py.test import raises
+from pytest import raises
 
 from fooof.bands.bands import *
 
 ###################################################################################################
 ###################################################################################################
 
 def test_bands():
```

### Comparing `fooof-1.0.0rc3/fooof/tests/conftest.py` & `fooof-1.1.0rc0/fooof/tests/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import shutil
 import pytest
 
 import numpy as np
 
 from fooof.core.modutils import safe_import
 
-from fooof.tests.tutils import get_tfm, get_tfg, get_tbands
-from fooof.tests.settings import BASE_TEST_FILE_PATH, TEST_DATA_PATH, TEST_REPORTS_PATH
+from fooof.tests.tutils import get_tfm, get_tfg, get_tbands, get_tresults
+from fooof.tests.settings import (BASE_TEST_FILE_PATH, TEST_DATA_PATH,
+                                  TEST_REPORTS_PATH, TEST_PLOTS_PATH)
 
 plt = safe_import('.pyplot', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
 
 def pytest_configure(config):
@@ -29,24 +30,34 @@
     if os.path.exists(BASE_TEST_FILE_PATH):
         shutil.rmtree(BASE_TEST_FILE_PATH)
 
     # Remake (empty) directories
     os.mkdir(BASE_TEST_FILE_PATH)
     os.mkdir(TEST_DATA_PATH)
     os.mkdir(TEST_REPORTS_PATH)
+    os.mkdir(TEST_PLOTS_PATH)
 
 @pytest.fixture(scope='session')
 def tfm():
     yield get_tfm()
 
 @pytest.fixture(scope='session')
 def tfg():
     yield get_tfg()
 
 @pytest.fixture(scope='session')
 def tbands():
     yield get_tbands()
 
 @pytest.fixture(scope='session')
+def tresults():
+    yield get_tresults()
+
+@pytest.fixture(scope='session')
 def skip_if_no_mpl():
     if not safe_import('matplotlib'):
         pytest.skip('Matplotlib not available: skipping test.')
+
+@pytest.fixture(scope='session')
+def skip_if_no_pandas():
+    if not safe_import('pandas'):
+        pytest.skip('Pandas not available: skipping test.')
```

### Comparing `fooof-1.0.0rc3/fooof/tests/core/test_funcs.py` & `fooof-1.1.0rc0/fooof/tests/core/test_funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for fooof.core.funcs."""
 
-from py.test import raises
+from pytest import raises
 
 import numpy as np
 from scipy.stats import norm, linregress
 
 from fooof.core.errors import InconsistentDataError
 
 from fooof.core.funcs import *
```

### Comparing `fooof-1.0.0rc3/fooof/tests/core/test_info.py` & `fooof-1.1.0rc0/fooof/tests/core/test_info.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/tests/core/test_io.py` & `fooof-1.1.0rc0/fooof/tests/core/test_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 def test_fname():
     """Check that the file name checker helper function properly checks / adds file extensions."""
 
     assert fname('data', 'json') == 'data.json'
     assert fname('data.json', 'json') == 'data.json'
     assert fname('pic', 'png') == 'pic.png'
     assert fname('pic.png', 'png') == 'pic.png'
+    assert fname('report.pdf', 'pdf') == 'report.pdf'
+    assert fname('report.png', 'pdf') == 'report.png'
 
 def test_fpath():
     """Check that the file path checker helper function properly checks / combines file paths."""
 
     assert fpath(None, 'data.json') == 'data.json'
     assert fpath('/path/', 'data.json') == '/path/data.json'
```

### Comparing `fooof-1.0.0rc3/fooof/tests/core/test_reports.py` & `fooof-1.1.0rc0/fooof/tests/core/test_reports.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/tests/core/test_strings.py` & `fooof-1.1.0rc0/fooof/tests/core/test_strings.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/tests/core/test_utils.py` & `fooof-1.1.0rc0/fooof/tests/core/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests for fooof.core.utils."""
 
 from collections.abc import Iterable
 from itertools import repeat
 
 from numpy import array_equal
 
-from py.test import raises
+from pytest import raises
 
 from fooof.core.utils import *
 
 ###################################################################################################
 ###################################################################################################
 
 def test_group_three():
```

### Comparing `fooof-1.0.0rc3/fooof/tests/objs/test_fit.py` & `fooof-1.1.0rc0/fooof/tests/objs/test_fit.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 NOTES
 -----
 The tests here are not strong tests for accuracy.
 They serve rather as 'smoke tests', for if anything fails completely.
 """
 
 import numpy as np
-from py.test import raises
+from pytest import raises
 
 from fooof.core.items import OBJ_DESC
 from fooof.core.errors import FitError
 from fooof.core.utils import group_three
-from fooof.sim import gen_power_spectrum
-from fooof.data import FOOOFSettings, FOOOFMetaData, FOOOFResults
+from fooof.core.modutils import safe_import
 from fooof.core.errors import DataError, NoDataError, InconsistentDataError
+from fooof.sim import gen_freqs, gen_power_spectrum
+from fooof.data import FOOOFSettings, FOOOFMetaData, FOOOFResults
+
+pd = safe_import('pandas')
 
 from fooof.tests.settings import TEST_DATA_PATH
 from fooof.tests.tutils import get_tfm, plot_test
 
 from fooof.objs.fit import *
 
 ###################################################################################################
@@ -51,58 +54,61 @@
     assert tfm.n_peaks_
 
 def test_fooof_fit_nk():
     """Test FOOOF fit, no knee."""
 
     ap_params = [50, 2]
     gauss_params = [10, 0.5, 2, 20, 0.3, 4]
+    nlv = 0.0025
 
-    xs, ys = gen_power_spectrum([3, 50], ap_params, gauss_params)
+    xs, ys = gen_power_spectrum([3, 50], ap_params, gauss_params, nlv)
 
     tfm = FOOOF(verbose=False)
     tfm.fit(xs, ys)
 
     # Check model results - aperiodic parameters
-    assert np.all(np.isclose(ap_params, tfm.aperiodic_params_, [0.5, 0.1]))
+    assert np.allclose(ap_params, tfm.aperiodic_params_, [0.5, 0.1])
 
     # Check model results - gaussian parameters
     for ii, gauss in enumerate(group_three(gauss_params)):
-        assert np.all(np.isclose(gauss, tfm.gaussian_params_[ii], [2.0, 0.5, 1.0]))
+        assert np.allclose(gauss, tfm.gaussian_params_[ii], [2.0, 0.5, 1.0])
 
 def test_fooof_fit_nk_noise():
     """Test FOOOF fit on noisy data, to make sure nothing breaks."""
 
     ap_params = [50, 2]
     gauss_params = [10, 0.5, 2, 20, 0.3, 4]
+    nlv = 1.0
 
-    xs, ys = gen_power_spectrum([3, 50], ap_params, gauss_params, nlv=1.0)
+    xs, ys = gen_power_spectrum([3, 50], ap_params, gauss_params, nlv)
 
     tfm = FOOOF(max_n_peaks=8, verbose=False)
     tfm.fit(xs, ys)
 
     # No accuracy checking here - just checking that it ran
     assert tfm.has_model
 
 def test_fooof_fit_knee():
     """Test FOOOF fit, with a knee."""
 
     ap_params = [50, 10, 1]
     gauss_params = [10, 0.3, 2, 20, 0.1, 4, 60, 0.3, 1]
+    nlv = 0.0025
 
-    xs, ys = gen_power_spectrum([1, 150], ap_params, gauss_params, nlv=0)
+    xs, ys = gen_power_spectrum([1, 150], ap_params, gauss_params, nlv)
 
     tfm = FOOOF(aperiodic_mode='knee', verbose=False)
     tfm.fit(xs, ys)
 
     # Check model results - aperiodic parameters
-    assert np.all(np.isclose(ap_params, tfm.aperiodic_params_, [1, 2, 0.2]))
+    assert np.allclose(ap_params, tfm.aperiodic_params_, [1, 2, 0.2])
 
     # Check model results - gaussian parameters
     for ii, gauss in enumerate(group_three(gauss_params)):
-        assert np.all(np.isclose(gauss, tfm.gaussian_params_[ii], [2.0, 0.5, 1.0]))
+        assert np.allclose(gauss, tfm.gaussian_params_[ii], [2.0, 0.5, 1.0])
 
 def test_fooof_fit_measures():
     """Test goodness of fit & error metrics, post model fitting."""
 
     tfm = FOOOF(verbose=False)
 
     # Hack fake data with known properties: total error magnitude 2
@@ -154,15 +160,19 @@
     tfm.fit(xs, ys, [3, 40])
 
     # Check freq of 0 issue
     xs, ys = gen_power_spectrum([3, 50], [50, 2], [10, 0.5, 2])
     tfm.fit(xs, ys)
     assert tfm.freqs[0] != 0
 
-    # Check error if there is a post-logging inf or nan
+    # Check error for `check_freqs` - for if there is non-even frequency values
+    with raises(DataError):
+        tfm.fit(np.array([1, 2, 4]), np.array([1, 2, 3]))
+
+    # Check error for `check_data` - for if there is a post-logging inf or nan
     with raises(DataError):  # Double log (1) -> -inf
         tfm.fit(np.array([1, 2, 3]), np.log10(np.array([1, 2, 3])))
     with raises(DataError):  # Log (-1) -> NaN
         tfm.fit(np.array([1, 2, 3]), np.array([-1, 2, 3]))
 
     ## Check errors & errors done in `fit`
 
@@ -180,15 +190,15 @@
     tfm.load(file_name_res, TEST_DATA_PATH)
     # Check that result attributes get filled
     for result in OBJ_DESC['results']:
         assert not np.all(np.isnan(getattr(tfm, result)))
     # Test that settings and data are None
     #   Except for aperiodic mode, which can be inferred from the data
     for setting in OBJ_DESC['settings']:
-        if setting is not 'aperiodic_mode':
+        if setting != 'aperiodic_mode':
             assert getattr(tfm, setting) is None
     assert getattr(tfm, 'power_spectrum') is None
 
     # Test loading just settings
     tfm = FOOOF(verbose=False)
     file_name_set = 'test_fooof_set'
     tfm.load(file_name_set, TEST_DATA_PATH)
@@ -219,44 +229,76 @@
     for setting in OBJ_DESC['settings']:
         assert getattr(tfm, setting) is not None
     for data in OBJ_DESC['data']:
         assert getattr(tfm, data) is not None
     for meta_dat in OBJ_DESC['meta_data']:
         assert getattr(tfm, meta_dat) is not None
 
-def test_adds():
-    """Tests methods that add data to FOOOF objects.
+def test_add_data():
+    """Tests method to add data to FOOOF objects."""
 
-    Checks: add_data, add_settings, add_results.
-    """
-
-    # Note: uses it's own tfm, to not add stuff to the global one
+    # This test uses it's own FOOOF object, to not add stuff to the global one
     tfm = get_tfm()
 
-    # Test adding data
+    # Test data for adding
     freqs, pows = np.array([1, 2, 3]), np.array([10, 10, 10])
+
+    # Test adding data
     tfm.add_data(freqs, pows)
+    assert tfm.has_data
     assert np.all(tfm.freqs == freqs)
     assert np.all(tfm.power_spectrum == np.log10(pows))
 
+    # Test that prior data does not get cleared, when requesting not to clear
+    tfm._reset_data_results(True, True, True)
+    tfm.add_results(FOOOFResults([1, 1], [10, 0.5, 0.5], 0.95, 0.02, [10, 0.5, 0.25]))
+    tfm.add_data(freqs, pows, clear_results=False)
+    assert tfm.has_data
+    assert tfm.has_model
+
+    # Test that prior data does get cleared, when requesting not to clear
+    tfm._reset_data_results(True, True, True)
+    tfm.add_data(freqs, pows, clear_results=True)
+    assert tfm.has_data
+    assert not tfm.has_model
+
+def test_add_settings():
+    """Tests method to add settings to FOOOF objects."""
+
+    # This test uses it's own FOOOF object, to not add stuff to the global one
+    tfm = get_tfm()
+
     # Test adding settings
     fooof_settings = FOOOFSettings([1, 4], 6, 0, 2, 'fixed')
     tfm.add_settings(fooof_settings)
     for setting in OBJ_DESC['settings']:
         assert getattr(tfm, setting) == getattr(fooof_settings, setting)
 
+def test_add_meta_data():
+    """Tests method to add meta data to FOOOF objects."""
+
+    # This test uses it's own FOOOF object, to not add stuff to the global one
+    tfm = get_tfm()
+
     # Test adding meta data
     fooof_meta_data = FOOOFMetaData([3, 40], 0.5)
     tfm.add_meta_data(fooof_meta_data)
     for meta_dat in OBJ_DESC['meta_data']:
         assert getattr(tfm, meta_dat) == getattr(fooof_meta_data, meta_dat)
 
+def test_add_results():
+    """Tests method to add results to FOOOF objects."""
+
+    # This test uses it's own FOOOF object, to not add stuff to the global one
+    tfm = get_tfm()
+
     # Test adding results
     fooof_results = FOOOFResults([1, 1], [10, 0.5, 0.5], 0.95, 0.02, [10, 0.5, 0.25])
     tfm.add_results(fooof_results)
+    assert tfm.has_model
     for setting in OBJ_DESC['results']:
         assert getattr(tfm, setting) == getattr(fooof_results, setting.strip('_'))
 
 def test_obj_gets(tfm):
     """Tests methods that return FOOOF data objects.
 
     Checks: get_settings, get_meta_data, get_results
@@ -357,17 +399,43 @@
     tfm.fit(*gen_power_spectrum([3, 50], [50, 2], [10, 0.5, 2, 20, 0.3, 4]))
 
     # Check after failing out of fit, all results are reset
     for result in OBJ_DESC['results']:
         assert np.all(np.isnan(getattr(tfm, result)))
 
 def test_fooof_debug():
-    """Test FOOOF fit failure in debug mode."""
+    """Test FOOOF in debug mode, including with fit failures."""
 
     tfm = FOOOF(verbose=False)
     tfm._maxfev = 5
 
     tfm.set_debug_mode(True)
     assert tfm._debug is True
 
     with raises(FitError):
         tfm.fit(*gen_power_spectrum([3, 50], [50, 2], [10, 0.5, 2, 20, 0.3, 4]))
+
+def test_fooof_check_data():
+    """Test FOOOF in with check data mode turned off, including with NaN data."""
+
+    tfm = FOOOF(verbose=False)
+
+    tfm.set_check_data_mode(False)
+    assert tfm._check_data is False
+
+    # Add data, with check data turned off
+    #   In check data mode, adding data with NaN should run
+    freqs = gen_freqs([3, 50], 0.5)
+    powers = np.ones_like(freqs) * np.nan
+    tfm.add_data(freqs, powers)
+    assert tfm.has_data
+
+    # Model fitting should execute, but return a null model fit, given the NaNs, without failing
+    tfm.fit()
+    assert not tfm.has_model
+
+def test_fooof_to_df(tfm, tbands, skip_if_no_pandas):
+
+    df1 = tfm.to_df(2)
+    assert isinstance(df1, pd.Series)
+    df2 = tfm.to_df(tbands)
+    assert isinstance(df2, pd.Series)
```

### Comparing `fooof-1.0.0rc3/fooof/tests/objs/test_group.py` & `fooof-1.1.0rc0/fooof/tests/objs/test_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 
 NOTES
 -----
 The tests here are not strong tests for accuracy.
 They serve rather as 'smoke tests', for if anything fails completely.
 """
 
+import os
+
 import numpy as np
 from numpy.testing import assert_equal
 
-from fooof.data import FOOOFResults
 from fooof.core.items import OBJ_DESC
+from fooof.core.modutils import safe_import
+from fooof.core.errors import DataError, NoDataError, InconsistentDataError
+from fooof.data import FOOOFResults
 from fooof.sim import gen_group_power_spectra
 
-from fooof.tests.settings import TEST_DATA_PATH
+pd = safe_import('pandas')
+
+from fooof.tests.settings import TEST_DATA_PATH, TEST_REPORTS_PATH
 from fooof.tests.tutils import default_group_params, plot_test
 
 from fooof.objs.group import *
 
 ###################################################################################################
 ###################################################################################################
 
@@ -204,14 +210,21 @@
 
 def test_fg_print(tfg):
     """Check print method (alias)."""
 
     tfg.print_results()
     assert True
 
+def test_save_model_report(tfg):
+
+    file_name = 'test_group_model_report'
+    tfg.save_model_report(0, file_name, TEST_REPORTS_PATH)
+
+    assert os.path.exists(os.path.join(TEST_REPORTS_PATH, file_name + '.pdf'))
+
 def test_get_results(tfg):
     """Check get results method."""
 
     assert tfg.get_results()
 
 def test_get_params(tfg):
     """Check get_params method."""
@@ -243,15 +256,15 @@
     # Test loading just results
     tfg = FOOOFGroup(verbose=False)
     tfg.load(file_name_res, TEST_DATA_PATH)
     assert len(tfg.group_results) > 0
     # Test that settings and data are None
     #   Except for aperiodic mode, which can be inferred from the data
     for setting in OBJ_DESC['settings']:
-        if setting is not 'aperiodic_mode':
+        if setting != 'aperiodic_mode':
             assert getattr(tfg, setting) is None
     assert tfg.power_spectra is None
 
     # Test loading just settings
     tfg = FOOOFGroup(verbose=False)
     tfg.load(file_name_set, TEST_DATA_PATH)
     for setting in OBJ_DESC['settings']:
@@ -345,7 +358,14 @@
     # Check that the correct data is extracted
     assert_equal(tfg.power_spectra[inds1, :], nfg1.power_spectra)
     assert_equal(tfg.power_spectra[inds2, :], nfg2.power_spectra)
 
     # Check that the correct results are extracted
     assert [tfg.group_results[ind] for ind in inds1] == nfg1.group_results
     assert [tfg.group_results[ind] for ind in inds2] == nfg2.group_results
+
+def test_fg_to_df(tfg, tbands, skip_if_no_pandas):
+
+    df1 = tfg.to_df(2)
+    assert isinstance(df1, pd.DataFrame)
+    df2 = tfg.to_df(tbands)
+    assert isinstance(df2, pd.DataFrame)
```

### Comparing `fooof-1.0.0rc3/fooof/tests/objs/test_utils.py` & `fooof-1.1.0rc0/fooof/tests/objs/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Test functions for fooof.objs.utils."""
 
-from py.test import raises
+from pytest import raises
 
 import numpy as np
 
 from fooof import FOOOFGroup
 from fooof.objs.utils import compare_info
 from fooof.sim import gen_group_power_spectra
 from fooof.core.errors import NoModelError, IncompatibleSettingsError
@@ -116,17 +116,21 @@
         f_obj2.freq_range = [5, 30]
 
         with raises(IncompatibleSettingsError):
             combine_fooofs([f_obj, f_obj2])
 
 def test_fit_fooof_3d(tfg):
 
-    n_spectra = 2
+    n_groups = 2
+    n_spectra = 3
     xs, ys = gen_group_power_spectra(n_spectra, *default_group_params())
-    ys = np.stack([ys, ys], axis=0)
+    ys = np.stack([ys] * n_groups, axis=0)
+    spectra_shape = np.shape(ys)
 
     tfg = FOOOFGroup()
     fgs = fit_fooof_3d(tfg, xs, ys)
 
-    assert len(fgs) == 2
+    assert len(fgs) == n_groups == spectra_shape[0]
     for fg in fgs:
         assert fg
+        assert len(fg) == n_spectra
+        assert fg.power_spectra.shape == spectra_shape[1:]
```

### Comparing `fooof-1.0.0rc3/fooof/tests/plts/test_fm.py` & `fooof-1.1.0rc0/fooof/tests/plts/test_fm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Tests for fooof.plts.fm."""
 
 from fooof.tests.tutils import plot_test
+from fooof.tests.settings import TEST_PLOTS_PATH
 
 from fooof.plts.fm import *
 
 ###################################################################################################
 ###################################################################################################
 
 @plot_test
 def test_plot_fm(tfm, skip_if_no_mpl):
 
     # Make sure model has been fit
     tfm.fit()
 
-    plot_fm(tfm)
+    plot_fm(tfm, save_fig=True, file_path=TEST_PLOTS_PATH,
+            file_name='test_plot_fm.png')
 
 @plot_test
 def test_plot_fm_add_peaks(tfm, skip_if_no_mpl):
 
     # Make sure model has been fit
     tfm.fit()
 
     # Test run each of the add peak approaches
-    for add_peak in ['shade', 'dot', 'outline', 'line']:
-        plot_fm(tfm, plot_peaks=add_peak)
-
-    # Test run some combinations
-    for add_peak in ['shade-dot', 'outline-line']:
-        plot_fm(tfm, plot_peaks=add_peak)
+    for add_peak in ['shade', 'dot', 'outline', 'line', 'shade-dot', 'outline-line']:
+        file_name = 'test_plot_fm_add_peaks_' + add_peak + '.png'
+        plot_fm(tfm, plot_peaks=add_peak, save_fig=True,
+                file_path=TEST_PLOTS_PATH, file_name=file_name)
```

### Comparing `fooof-1.0.0rc3/fooof/tests/sim/test_gen.py` & `fooof-1.1.0rc0/fooof/tests/sim/test_gen.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/tests/sim/test_params.py` & `fooof-1.1.0rc0/fooof/tests/sim/test_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Test functions for fooof.sim.params."""
 
-from py.test import raises
+from pytest import raises
 
 from numpy import array_equal
 
 from fooof.core.errors import InconsistentDataError
 
 from fooof.sim.params import *
```

### Comparing `fooof-1.0.0rc3/fooof/tests/sim/test_transform.py` & `fooof-1.1.0rc0/fooof/tests/sim/test_transform.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/tests/tutils.py` & `fooof-1.1.0rc0/fooof/tests/tutils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Utilities for testing fooof."""
 
 from functools import wraps
 
+import numpy as np
+
 from fooof.bands import Bands
+from fooof.data import FOOOFResults
 from fooof.objs import FOOOF, FOOOFGroup
 from fooof.core.modutils import safe_import
 from fooof.sim.params import param_sampler
 from fooof.sim.gen import gen_power_spectrum, gen_group_power_spectra
 
 plt = safe_import('.pyplot', 'matplotlib')
 
@@ -39,14 +42,22 @@
     return tfg
 
 def get_tbands():
     """Get a bands object, for testing."""
 
     return Bands({'theta' : (4, 8), 'alpha' : (8, 12), 'beta' : (13, 30)})
 
+def get_tresults():
+    """Get a FOOOFResults objet, for testing."""
+
+    return FOOOFResults(aperiodic_params=np.array([1.0, 1.00]),
+                        peak_params=np.array([[10.0, 1.25, 2.0], [20.0, 1.0, 3.0]]),
+                        r_squared=0.97, error=0.01,
+                        gaussian_params=np.array([[10.0, 1.25, 1.0], [20.0, 1.0, 1.5]]))
+
 def default_group_params():
     """Create default parameters for generating a test group of power spectra."""
 
     freq_range = [3, 50]
     ap_opts = param_sampler([[20, 2], [50, 2.5], [35, 1.5]])
     gauss_opts = param_sampler([[10, 0.5, 2], [10, 0.5, 2, 20, 0.3, 4]])
```

### Comparing `fooof-1.0.0rc3/fooof/tests/utils/test_download.py` & `fooof-1.1.0rc0/fooof/tests/utils/test_download.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/tests/utils/test_io.py` & `fooof-1.1.0rc0/fooof/tests/utils/test_io.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/tests/utils/test_params.py` & `fooof-1.1.0rc0/fooof/tests/utils/test_params.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/tests/utils/test_reports.py` & `fooof-1.1.0rc0/fooof/tests/utils/test_reports.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/utils/debug.py` & `fooof-1.1.0rc0/fooof/utils/debug.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/utils/download.py` & `fooof-1.1.0rc0/fooof/utils/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from urllib.request import urlretrieve
 
 import numpy as np
 
 ###################################################################################################
 ###################################################################################################
 
-DATA_URL = 'https://raw.githubusercontent.com/fooof-tools/fooof/master/data/'
+DATA_URL = 'https://raw.githubusercontent.com/fooof-tools/fooof/main/data/'
 
 def check_data_folder(folder):
     """Check if a data folder exists, and create if not.
 
     Parameters
     ----------
     folder : str
```

### Comparing `fooof-1.0.0rc3/fooof/utils/io.py` & `fooof-1.1.0rc0/fooof/utils/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Utilities for input / ouput for data and models."""
+"""Utilities for input / output for data and models."""
 
 ###################################################################################################
 ###################################################################################################
 
 def load_fooof(file_name, file_path=None, regenerate=True):
     """Load a FOOOF file into a FOOOF object.
```

### Comparing `fooof-1.0.0rc3/fooof/utils/params.py` & `fooof-1.1.0rc0/fooof/utils/params.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof/utils/reports.py` & `fooof-1.1.0rc0/fooof/utils/reports.py`

 * *Files identical despite different names*

### Comparing `fooof-1.0.0rc3/fooof.egg-info/SOURCES.txt` & `fooof-1.1.0rc0/fooof.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
-README.md
-setup.cfg
+README.rst
 setup.py
 fooof/__init__.py
 fooof/version.py
 fooof.egg-info/PKG-INFO
 fooof.egg-info/SOURCES.txt
 fooof.egg-info/dependency_links.txt
 fooof.egg-info/requires.txt
@@ -22,22 +21,24 @@
 fooof/core/io.py
 fooof/core/items.py
 fooof/core/modutils.py
 fooof/core/reports.py
 fooof/core/strings.py
 fooof/core/utils.py
 fooof/data/__init__.py
+fooof/data/conversions.py
 fooof/data/data.py
 fooof/objs/__init__.py
 fooof/objs/fit.py
 fooof/objs/group.py
 fooof/objs/utils.py
 fooof/plts/__init__.py
 fooof/plts/annotate.py
 fooof/plts/aperiodic.py
+fooof/plts/error.py
 fooof/plts/fg.py
 fooof/plts/fm.py
 fooof/plts/periodic.py
 fooof/plts/settings.py
 fooof/plts/spectra.py
 fooof/plts/style.py
 fooof/plts/templates.py
@@ -61,22 +62,24 @@
 fooof/tests/core/test_info.py
 fooof/tests/core/test_io.py
 fooof/tests/core/test_modutils.py
 fooof/tests/core/test_reports.py
 fooof/tests/core/test_strings.py
 fooof/tests/core/test_utils.py
 fooof/tests/data/__init__.py
+fooof/tests/data/test_conversions.py
 fooof/tests/data/test_data.py
 fooof/tests/objs/__init__.py
 fooof/tests/objs/test_fit.py
 fooof/tests/objs/test_group.py
 fooof/tests/objs/test_utils.py
 fooof/tests/plts/__init__.py
 fooof/tests/plts/test_annotate.py
 fooof/tests/plts/test_aperiodic.py
+fooof/tests/plts/test_error.py
 fooof/tests/plts/test_fg.py
 fooof/tests/plts/test_fm.py
 fooof/tests/plts/test_periodic.py
 fooof/tests/plts/test_spectra.py
 fooof/tests/plts/test_styles.py
 fooof/tests/plts/test_templates.py
 fooof/tests/plts/test_utils.py
```

