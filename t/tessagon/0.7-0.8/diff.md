# Comparing `tmp/tessagon-0.7.tar.gz` & `tmp/tessagon-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tessagon-0.7.tar", last modified: Fri Sep  9 22:32:28 2022, max compression
+gzip compressed data, was "tessagon-0.8.tar", last modified: Fri Jun 30 02:05:40 2023, max compression
```

## Comparing `tessagon-0.7.tar` & `tessagon-0.8.tar`

### file list

```diff
@@ -1,58 +1,66 @@
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2022-09-09 22:32:28.532067 tessagon-0.7/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)    11357 2020-04-19 17:19:18.000000 tessagon-0.7/LICENSE
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1418 2022-09-09 22:32:28.532067 tessagon-0.7/PKG-INFO
--rw-rw-r--   0 cwant     (1000) cwant     (1000)    19490 2022-09-09 22:28:17.000000 tessagon-0.7/README.md
--rw-rw-r--   0 cwant     (1000) cwant     (1000)       38 2022-09-09 22:32:28.532067 tessagon-0.7/setup.cfg
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1672 2022-09-09 22:28:17.000000 tessagon-0.7/setup.py
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2022-09-09 22:32:28.524067 tessagon-0.7/tessagon/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)       69 2022-09-07 22:50:09.000000 tessagon-0.7/tessagon/__init__.py
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2022-09-09 22:32:28.528067 tessagon-0.7/tessagon/adaptors/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/adaptors/__init__.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)      589 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/adaptors/blender_adaptor.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)      869 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/adaptors/list_adaptor.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1395 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/adaptors/vtk_adaptor.py
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2022-09-09 22:32:28.528067 tessagon-0.7/tessagon/core/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/core/__init__.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     7431 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/core/abstract_tile.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)      445 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/core/grid_tile_generator.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)    10764 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/core/rotate_tile_generator.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     6098 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/core/stamp14_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     2531 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/core/tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3604 2022-09-07 22:50:09.000000 tessagon-0.7/tessagon/core/tessagon_discovery.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1199 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/core/tessagon_metadata.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)    12255 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/core/tile.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5669 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/core/tile_generator.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1606 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/core/value_blend.py
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2022-09-09 22:32:28.528067 tessagon-0.7/tessagon/misc/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/misc/__init__.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3416 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/misc/shapes.py
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2022-09-09 22:32:28.532067 tessagon-0.7/tessagon/types/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/types/__init__.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     2503 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/brick_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     7082 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/dissected_hex_quad_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5674 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/dissected_hex_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     4422 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/types/dissected_square_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5415 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/dissected_triangle_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     8788 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/dodeca_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5804 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/dodeca_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     4918 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/types/floret_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     4456 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/hex_big_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     7082 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/hex_square_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     4795 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/types/hex_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3485 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/hex_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3009 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/octo_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3099 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/penta2_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5487 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/penta_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     7026 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/pythagorean_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3400 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/rhombus_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3345 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/types/square_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3508 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/square_tri2_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5785 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/square_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     4824 2020-04-19 17:19:18.000000 tessagon-0.7/tessagon/types/tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     6800 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/weave_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     6142 2022-09-09 22:28:17.000000 tessagon-0.7/tessagon/types/zig_zag_tessagon.py
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2022-09-09 22:32:28.528067 tessagon-0.7/tessagon.egg-info/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1418 2022-09-09 22:32:28.000000 tessagon-0.7/tessagon.egg-info/PKG-INFO
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1583 2022-09-09 22:32:28.000000 tessagon-0.7/tessagon.egg-info/SOURCES.txt
--rw-rw-r--   0 cwant     (1000) cwant     (1000)        1 2022-09-09 22:32:28.000000 tessagon-0.7/tessagon.egg-info/dependency_links.txt
--rw-rw-r--   0 cwant     (1000) cwant     (1000)        9 2022-09-09 22:32:28.000000 tessagon-0.7/tessagon.egg-info/top_level.txt
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.165679 tessagon-0.8/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)    11357 2020-04-19 17:19:18.000000 tessagon-0.8/LICENSE
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1418 2023-06-30 02:05:40.165679 tessagon-0.8/PKG-INFO
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)    22372 2023-06-30 01:55:14.000000 tessagon-0.8/README.md
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)       38 2023-06-30 02:05:40.165679 tessagon-0.8/setup.cfg
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1719 2023-06-30 01:55:14.000000 tessagon-0.8/setup.py
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.157678 tessagon-0.8/tessagon/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)      102 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/__init__.py
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.157678 tessagon-0.8/tessagon/adaptors/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2023-06-24 19:27:14.000000 tessagon-0.8/tessagon/adaptors/__init__.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)      589 2020-04-19 17:19:18.000000 tessagon-0.8/tessagon/adaptors/blender_adaptor.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)      869 2020-04-19 17:19:18.000000 tessagon-0.8/tessagon/adaptors/list_adaptor.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1395 2020-04-19 17:19:18.000000 tessagon-0.8/tessagon/adaptors/vtk_adaptor.py
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.161678 tessagon-0.8/tessagon/core/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)      735 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/__init__.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     8693 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/abstract_tile.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)      500 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/alternating_tile.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3326 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/grid_tile_generator.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     7697 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/parallelogram_tile_generator.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5663 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4213 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/tessagon_discovery.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1935 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/tessagon_metadata.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)    14420 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/tile.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     2564 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/tile_generator.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)      878 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/tile_utils.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1606 2020-04-19 17:19:18.000000 tessagon-0.8/tessagon/core/value_blend.py
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.161678 tessagon-0.8/tessagon/misc/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2020-04-19 17:19:18.000000 tessagon-0.8/tessagon/misc/__init__.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3416 2020-04-19 17:19:18.000000 tessagon-0.8/tessagon/misc/shapes.py
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.165679 tessagon-0.8/tessagon/types/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2023-06-24 19:30:11.000000 tessagon-0.8/tessagon/types/__init__.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     6053 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/big_hex_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     2600 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/brick_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     6289 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/cloverdale_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     7202 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/dissected_hex_quad_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5748 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/dissected_hex_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4464 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/dissected_square_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5530 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/dissected_triangle_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     8887 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/dodeca_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5911 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/dodeca_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     6808 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/floret_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4252 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/hex_big_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     7194 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/hex_square_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4934 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/hex_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3622 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/hex_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5932 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/islamic_hex_stars_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4828 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/islamic_stars_crosses_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3106 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/octo_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3224 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/penta2_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5585 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/penta_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     7230 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/pythagorean_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3529 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/rhombus_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3387 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/square_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3566 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/square_tri2_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5827 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/square_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5959 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/stanley_park_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4939 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4209 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/valemount_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     7582 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/weave_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     6350 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/zig_zag_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)       20 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/version.py
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.157678 tessagon-0.8/tessagon.egg-info/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1418 2023-06-30 02:05:40.000000 tessagon-0.8/tessagon.egg-info/PKG-INFO
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1886 2023-06-30 02:05:40.000000 tessagon-0.8/tessagon.egg-info/SOURCES.txt
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)        1 2023-06-30 02:05:40.000000 tessagon-0.8/tessagon.egg-info/dependency_links.txt
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)        9 2023-06-30 02:05:40.000000 tessagon-0.8/tessagon.egg-info/top_level.txt
```

### Comparing `tessagon-0.7/LICENSE` & `tessagon-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tessagon-0.7/PKG-INFO` & `tessagon-0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tessagon
-Version: 0.7
+Version: 0.8
 Summary: Tessellate your favorite 2D manifolds with triangles, hexagons, and other interesting patterns.
 Home-page: https://github.com/cwant/tessagon
 Author: Chris Want
 License: UNKNOWN
 Keywords: tesselation tiling modeling blender vtk
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tessagon-0.7/README.md` & `tessagon-0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -71,69 +71,84 @@
 
 ## Tessagon classes
 
 Additional tessagon classes can be added by deconstructing how a tessellation fits within a rectangular patch in the plane (check out the ASCII art in each source file in `tessagon.types`). The current `Tessagon` subclasses include:
 
 ### Regular tilings
 
-* [SquareTessagon](documentation/square_tessagon.md) (8 color patterns)  
-  [![SquareTessagon](documentation/images/square_tessagon_thumb.png)](documentation/square_tessagon.md)
-* [HexTessagon](documentation/hex_tessagon.md) (2 color patterns)  
-  [![HexTessagon](documentation/images/hex_tessagon_thumb.png)](documentation/hex_tessagon.md)
-* [TriTessagon](documentation/tri_tessagon.md) (3 color patterns)  
-  [![TriTessagon](documentation/images/tri_tessagon_thumb.png)](documentation/tri_tessagon.md)
+* [SquareTessagon](documentation/types/square_tessagon.md) (8 color patterns)  
+  [![SquareTessagon](documentation/images/types/square_tessagon_thumb.png)](documentation/types/square_tessagon.md)
+* [HexTessagon](documentation/types/hex_tessagon.md) (2 color patterns)  
+  [![HexTessagon](documentation/images/types/hex_tessagon_thumb.png)](documentation/types/hex_tessagon.md)
+* [TriTessagon](documentation/types/tri_tessagon.md) (3 color patterns)  
+  [![TriTessagon](documentation/images/types/tri_tessagon_thumb.png)](documentation/types/tri_tessagon.md)
 
 ### Archimedean tilings
 
-* [OctoTessagon](documentation/octo_tessagon.md) (1 color patterns)  
-  [![OctoTessagon](documentation/images/octo_tessagon_thumb.png)](documentation/octo_tessagon.md)
-* [HexTriTessagon](documentation/hex_tri_tessagon.md) (1 color patterns)  
-  [![HexTriTessagon](documentation/images/hex_tri_tessagon_thumb.png)](documentation/hex_tri_tessagon.md)
-* [HexSquareTriTessagon](documentation/hex_square_tri_tessagon.md) (1 color patterns)  
-  [![HexSquareTriTessagon](documentation/images/hex_square_tri_tessagon_thumb.png)](documentation/hex_square_tri_tessagon.md)
-* [DodecaTessagon](documentation/dodeca_tessagon.md) (1 color patterns)  
-  [![DodecaTessagon](documentation/images/dodeca_tessagon_thumb.png)](documentation/dodeca_tessagon.md)
-* [SquareTriTessagon](documentation/square_tri_tessagon.md) (2 color patterns)  
-  [![SquareTriTessagon](documentation/images/square_tri_tessagon_thumb.png)](documentation/square_tri_tessagon.md)
-* [SquareTri2Tessagon](documentation/square_tri2_tessagon.md) (1 color patterns)  
-  [![SquareTri2Tessagon](documentation/images/square_tri2_tessagon_thumb.png)](documentation/square_tri2_tessagon.md)
-* [DodecaTriTessagon](documentation/dodeca_tri_tessagon.md) (1 color patterns)  
-  [![DodecaTriTessagon](documentation/images/dodeca_tri_tessagon_thumb.png)](documentation/dodeca_tri_tessagon.md)
+* [OctoTessagon](documentation/types/octo_tessagon.md) (1 color pattern)  
+  [![OctoTessagon](documentation/images/types/octo_tessagon_thumb.png)](documentation/types/octo_tessagon.md)
+* [HexTriTessagon](documentation/types/hex_tri_tessagon.md) (1 color pattern)  
+  [![HexTriTessagon](documentation/images/types/hex_tri_tessagon_thumb.png)](documentation/types/hex_tri_tessagon.md)
+* [HexSquareTriTessagon](documentation/types/hex_square_tri_tessagon.md) (1 color pattern)  
+  [![HexSquareTriTessagon](documentation/images/types/hex_square_tri_tessagon_thumb.png)](documentation/types/hex_square_tri_tessagon.md)
+* [DodecaTessagon](documentation/types/dodeca_tessagon.md) (1 color pattern)  
+  [![DodecaTessagon](documentation/images/types/dodeca_tessagon_thumb.png)](documentation/types/dodeca_tessagon.md)
+* [SquareTriTessagon](documentation/types/square_tri_tessagon.md) (2 color patterns)  
+  [![SquareTriTessagon](documentation/images/types/square_tri_tessagon_thumb.png)](documentation/types/square_tri_tessagon.md)
+* [SquareTri2Tessagon](documentation/types/square_tri2_tessagon.md) (1 color pattern)  
+  [![SquareTri2Tessagon](documentation/images/types/square_tri2_tessagon_thumb.png)](documentation/types/square_tri2_tessagon.md)
+* [DodecaTriTessagon](documentation/types/dodeca_tri_tessagon.md) (1 color pattern)  
+  [![DodecaTriTessagon](documentation/images/types/dodeca_tri_tessagon_thumb.png)](documentation/types/dodeca_tri_tessagon.md)
+* [BigHexTriTessagon](documentation/types/big_hex_tri_tessagon.md) (1 color pattern, 1 extra parameter)  
+  [![BigHexTriTessagon](documentation/images/types/big_hex_tri_tessagon_thumb.png)](documentation/types/big_hex_tri_tessagon.md)
 
 ### Laves tilings
 
-* [RhombusTessagon](documentation/rhombus_tessagon.md) (2 color patterns)  
-  [![RhombusTessagon](documentation/images/rhombus_tessagon_thumb.png)](documentation/rhombus_tessagon.md)
-* [FloretTessagon](documentation/floret_tessagon.md) (3 color patterns)  
-  [![FloretTessagon](documentation/images/floret_tessagon_thumb.png)](documentation/floret_tessagon.md)
-* [DissectedSquareTessagon](documentation/dissected_square_tessagon.md) (2 color patterns)  
-  [![DissectedSquareTessagon](documentation/images/dissected_square_tessagon_thumb.png)](documentation/dissected_square_tessagon.md)
-* [DissectedTriangleTessagon](documentation/dissected_triangle_tessagon.md) (1 color patterns)  
-  [![DissectedTriangleTessagon](documentation/images/dissected_triangle_tessagon_thumb.png)](documentation/dissected_triangle_tessagon.md)
-* [DissectedHexQuadTessagon](documentation/dissected_hex_quad_tessagon.md) (2 color patterns)  
-  [![DissectedHexQuadTessagon](documentation/images/dissected_hex_quad_tessagon_thumb.png)](documentation/dissected_hex_quad_tessagon.md)
-* [DissectedHexTriTessagon](documentation/dissected_hex_tri_tessagon.md) (1 color patterns)  
-  [![DissectedHexTriTessagon](documentation/images/dissected_hex_tri_tessagon_thumb.png)](documentation/dissected_hex_tri_tessagon.md)
-* [PentaTessagon](documentation/penta_tessagon.md) (1 color patterns)  
-  [![PentaTessagon](documentation/images/penta_tessagon_thumb.png)](documentation/penta_tessagon.md)
-* [Penta2Tessagon](documentation/penta2_tessagon.md) (1 color patterns)  
-  [![Penta2Tessagon](documentation/images/penta2_tessagon_thumb.png)](documentation/penta2_tessagon.md)
+* [RhombusTessagon](documentation/types/rhombus_tessagon.md) (2 color patterns)  
+  [![RhombusTessagon](documentation/images/types/rhombus_tessagon_thumb.png)](documentation/types/rhombus_tessagon.md)
+* [FloretTessagon](documentation/types/floret_tessagon.md) (3 color patterns)  
+  [![FloretTessagon](documentation/images/types/floret_tessagon_thumb.png)](documentation/types/floret_tessagon.md)
+* [DissectedSquareTessagon](documentation/types/dissected_square_tessagon.md) (2 color patterns)  
+  [![DissectedSquareTessagon](documentation/images/types/dissected_square_tessagon_thumb.png)](documentation/types/dissected_square_tessagon.md)
+* [DissectedTriangleTessagon](documentation/types/dissected_triangle_tessagon.md) (1 color pattern)  
+  [![DissectedTriangleTessagon](documentation/images/types/dissected_triangle_tessagon_thumb.png)](documentation/types/dissected_triangle_tessagon.md)
+* [DissectedHexQuadTessagon](documentation/types/dissected_hex_quad_tessagon.md) (2 color patterns)  
+  [![DissectedHexQuadTessagon](documentation/images/types/dissected_hex_quad_tessagon_thumb.png)](documentation/types/dissected_hex_quad_tessagon.md)
+* [DissectedHexTriTessagon](documentation/types/dissected_hex_tri_tessagon.md) (1 color pattern)  
+  [![DissectedHexTriTessagon](documentation/images/types/dissected_hex_tri_tessagon_thumb.png)](documentation/types/dissected_hex_tri_tessagon.md)
+* [PentaTessagon](documentation/types/penta_tessagon.md) (1 color pattern)  
+  [![PentaTessagon](documentation/images/types/penta_tessagon_thumb.png)](documentation/types/penta_tessagon.md)
+* [Penta2Tessagon](documentation/types/penta2_tessagon.md) (1 color pattern)  
+  [![Penta2Tessagon](documentation/images/types/penta2_tessagon_thumb.png)](documentation/types/penta2_tessagon.md)
 
 ### Non-edge-to-edge tilings
 
-* [PythagoreanTessagon](documentation/pythagorean_tessagon.md) (1 color patterns)  
-  [![PythagoreanTessagon](documentation/images/pythagorean_tessagon_thumb.png)](documentation/pythagorean_tessagon.md)
-* [BrickTessagon](documentation/brick_tessagon.md) (1 color patterns)  
-  [![BrickTessagon](documentation/images/brick_tessagon_thumb.png)](documentation/brick_tessagon.md)
-* [WeaveTessagon](documentation/weave_tessagon.md) (1 color patterns)  
-  [![WeaveTessagon](documentation/images/weave_tessagon_thumb.png)](documentation/weave_tessagon.md)
-* [HexBigTriTessagon](documentation/hex_big_tri_tessagon.md) (2 color patterns)  
-  [![HexBigTriTessagon](documentation/images/hex_big_tri_tessagon_thumb.png)](documentation/hex_big_tri_tessagon.md)
-* [ZigZagTessagon](documentation/zig_zag_tessagon.md) (1 color patterns)  
-  [![ZigZagTessagon](documentation/images/zig_zag_tessagon_thumb.png)](documentation/zig_zag_tessagon.md)
+* [PythagoreanTessagon](documentation/types/pythagorean_tessagon.md) (1 color pattern)  
+  [![PythagoreanTessagon](documentation/images/types/pythagorean_tessagon_thumb.png)](documentation/types/pythagorean_tessagon.md)
+* [BrickTessagon](documentation/types/brick_tessagon.md) (1 color pattern)  
+  [![BrickTessagon](documentation/images/types/brick_tessagon_thumb.png)](documentation/types/brick_tessagon.md)
+* [WeaveTessagon](documentation/types/weave_tessagon.md) (1 color pattern, 1 extra parameter)  
+  [![WeaveTessagon](documentation/images/types/weave_tessagon_thumb.png)](documentation/types/weave_tessagon.md)
+* [HexBigTriTessagon](documentation/types/hex_big_tri_tessagon.md) (2 color patterns)  
+  [![HexBigTriTessagon](documentation/images/types/hex_big_tri_tessagon_thumb.png)](documentation/types/hex_big_tri_tessagon.md)
+* [ZigZagTessagon](documentation/types/zig_zag_tessagon.md) (1 color pattern)  
+  [![ZigZagTessagon](documentation/images/types/zig_zag_tessagon_thumb.png)](documentation/types/zig_zag_tessagon.md)
+* [ValemountTessagon](documentation/types/valemount_tessagon.md) (1 color pattern)  
+  [![ValemountTessagon](documentation/images/types/valemount_tessagon_thumb.png)](documentation/types/valemount_tessagon.md)
+* [CloverdaleTessagon](documentation/types/cloverdale_tessagon.md) (1 color pattern)  
+  [![CloverdaleTessagon](documentation/images/types/cloverdale_tessagon_thumb.png)](documentation/types/cloverdale_tessagon.md)
+
+### Non-convex tilings
+
+* [StanleyParkTessagon](documentation/types/stanley_park_tessagon.md) (2 color patterns)  
+  [![StanleyParkTessagon](documentation/images/types/stanley_park_tessagon_thumb.png)](documentation/types/stanley_park_tessagon.md)
+* [IslamicHexStarsTessagon](documentation/types/islamic_hex_stars_tessagon.md) (1 color pattern)  
+  [![IslamicHexStarsTessagon](documentation/images/types/islamic_hex_stars_tessagon_thumb.png)](documentation/types/islamic_hex_stars_tessagon.md)
+* [IslamicStarsCrossesTessagon](documentation/types/islamic_stars_crosses_tessagon.md) (1 color pattern)  
+  [![IslamicStarsCrossesTessagon](documentation/images/types/islamic_stars_crosses_tessagon_thumb.png)](documentation/types/islamic_stars_crosses_tessagon.md)
 
 ## Usage and Options
 
 Each tessagon class is initialized with number of keyword options, e.g.:
 
 ```
 from tessagon.types.dodeca_tessagon import DodecaTessagon
@@ -146,15 +161,18 @@
                           u_cyclic=True,
                           v_cyclic=False,
                           adaptor_class=VtkAdaptor)
 poly_data = tessagon.create_mesh()
 ```
 The `create_mesh()` method creates a tessellated mesh using your provided function and the tile type corresponding to the tessagon class used. The chosen adaptor dictates the 3D data type the mesh will be (for the `BlenderAdaptor` the output is `BMesh`, for the `VTKAdaptor` the output is `vtkPolyData`).
 
-Here are the options:
+Each Tessagon class may supply options that are specific to that class
+(they will be listed on the documentation page for each class).
+
+Here are the options that are common to all Tessagon classes:
 
 * `function`: the function to be used to generate the geometry. This is a function that takes two arguments `u, v` and returns a list of three items `[x, y, z]`
 * `u_range`: a list with two items indicating the minimum and maximum values for u (the first argument to the function passed);
 * `v_range`: a list with two items indicating the minimum and maximum values for v (the second argument to the function passed);
 * `u_num`: the number of tiles to be created in the u-direction;
 * `v_num`: the number of tiles to be created in the v-direction;
 
@@ -175,17 +193,19 @@
 * `rot_factor`: this is an integer greater than zero that allows you to rotate the tiles in the UV-domain is such a way that the tiling can still be cyclic.
   
   ![rot_factor](documentation/images/rot_factor.png)
   
   The `rot_factor` specifies how many tiles you go across before you go up one unit (essentially the reciprocal of the slope of the grid lines. The image depicts a `rot_factor` of three, which generates 45 tiles (the purple interior and the blue boundary squares, each of which is blasted with the tessellation pattern when the function is applied). Here the meaning of `u_num` and `v_num` are interpreted differently: whereas in the non-rotated case, `u_num = 3` and `v_num = 2` would yeild 6 tiles, here we have 45 tiles. Niether U nor V are cyclic in the picture; had they both been cyclic, 60 tiles whould have been generated. The interior tiles form groups of `(rot_factor-1)**2` tiles (here each group is 2 x 2, for 24 total interior tiles), and each boundary shares `rot_factor x 1` tiles with it's neighbors (there are 7 such boundaries, so 21 boundary tiles).
   
   It hurt my brain developing this feature, so don't feel bad if it does't make any sense for you. Play around with it, and keep in mind that the number of tiles generated is somewhere between `u_num * v_num * (rot_factor - 1)**2` and `u_num * v_num * (rot_factor**2 + 1)` (depending on which tiles have neighbors, due to periodicity), so you typically want to set `u_num` and `v_num` to be a lot lower than you would in the non-rotated case.
+* `parallelogram_vectors`: two vectors (e.g., `[[5, 1], [-1, 6]]`) that form a parallelogram to warp the tiles in a way that cyclic tiles can occur (this is more general than `rot_factor`, in fact the `rot_factor` implementation uses `parallelogram_vectors`). This one will require it's own [page](documentation/parallelogram_vectors.md) to describe.
 * `u_twist`: this is used with `v_cyclic` (note that says `v_cyclic` not `u_cyclic`). As the `v` values wrap around, the `u` values reconnect in the opposite direction: the low `u` values connect to the high `u` values, and vice versa. This allows you to make things like Möbius strips and Klein bottles.
 * `v_twist`: works with `u_cyclic`, analogous to how `u_twist` works.
 * `color_pattern`: some Tessagon types support some curated patterns (applying more than one material/color to the output shape). These are identified by a number (e.g., `color_pattern=2`). The number has no meaning other than as an identifier. Checkout the description of the Tessagon types above to see what color patterns exist. The values of `u_num` and `v_num` may need to be tweaked to make a specific color pattern wrap correctly for cyclic tilings.
+* `simple_2d` (default: `False`), `multiplier_2d`, `translate_2d`: these parameters (when `simple_2d` is `True`) help with creating tilings in the XY-plane (2D). The "natural" undistorted aspect ratio of the tiling is preserved. `multiplier_2d` (a number) allows you to scale such tilings, and `translate_2d` (a tuple) places a corner of the tiling (either top-left or bottom-left, depending on how you handle the up direction). With `simple_2d`, no function should be supplied to the Tessagon class.
 
 ## Writing your own tessellation classes
 
 All tesselations are found in the `types` module, so check out the source code there for numerous examples. The source code documentation in `hex_tessagon` is more verbose than the others, which hopefully will aid understanding.
 
 Each tessellation involve two classes: a tile class (a child of `Tile`) and a child of class `Tessagon`. The `Tessagon` subclass is easy (it just declares which tile class with be used), so writing the tile class will take most of your time. 
 (The `FloretTessagon` is an exception because the math is more complex.)
@@ -200,15 +220,15 @@
 
 * `calculate_verts`: here you define the locations of the vertices in the tiling, via the `add_vert` method. The method takes an array of keys to indicate which vertex is being defined, and a location expressed as a `u_ratio` and a `v_ratio`, both between 0 and 1. A `u_ratio` of 0 is `left` and a `u_ratio` of 1 is right. A `v_ratio` of 0 is `bottom` and a `v_ratio` of 1 is `top`. The symmetry of the tile may cause additional reflected vertices to be defined. Using the boolean keywords `u_boundary`, `v_boundary` and `corner`, you can tell the system whether the vert is shared with neighboring tiles (this reduces the work that needs to be done, and can also keep the model topologically sound and water-tight).
 
 * `calculate_faces`: here you define the faces for the tiling using the previously defined vertices, via the `add_face` method. The method takes an array of face to indicate which face is being defined, and an array of vertex keys that indicate which vertices are in the face. These vertices are either on the current tile, or some of them can being on neighboring tiles (in which case the keys for the neighboring tile are also included). The symmetry of the tile may cause other reflected faces to be defined. Using the boolean keywords `u_boundary`, `v_boundary` and `corner`, you can tell the system whether the face is shared with neighboring tiles.
 
 ## Metadata and Discovery
 
-Each `Tessagon` subclass has some metadata attached to it (class `TessagonMetadata`) that describes the properties of the tiling. This metadata will be expanded as needs require, but currently consists of information about how many color patterns the tiling has, what type (`regular`, `archimedean`, `laves`, `non_edge`), and what sorts of shapes are produced by instances of the class.
+Each `Tessagon` subclass has some metadata attached to it (class `TessagonMetadata`) that describes the properties of the tiling. This metadata will be expanded as needs require, but currently consists of information about how many color patterns the tiling has, what type (`regular`, `archimedean`, `laves`, `non_edge`, `non_convex`), and what sorts of shapes are produced by instances of the class.
 
 A nascent helper class `tessagon.TessagonDiscovery` exists that can help you search for tilings with certain properties (for example, this could be used to create a menu for an external application that categorizes the tilings). The methods in the class are intended to support chaining of operations (e.g., they results returned are also of type `TessagonDiscovery`, that can then be reified using the `to_list` method). Some examples:
 
 ```python
 find_all = TessagonDiscovery()
 find_all.to_list() # a list of all of the tessagons
 regular = find_all.with_classification('regular')
```

### Comparing `tessagon-0.7/setup.py` & `tessagon-0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 
 or::
 
     pip3 install tessagon
 
 '''[1:-1]
 
+exec(open('tessagon/version.py').read())
 setup(
     name='tessagon',
-    version='0.7',
+    version=__version__,
     description='Tessellate your favorite 2D manifolds with triangles, ' +
     'hexagons, and other interesting patterns.',
     long_description=long_description,
     url='https://github.com/cwant/tessagon',
     author='Chris Want',
     classifiers=['Development Status :: 3 - Alpha',
                  'Intended Audience :: Developers',
```

### Comparing `tessagon-0.7/tessagon/adaptors/blender_adaptor.py` & `tessagon-0.8/tessagon/adaptors/blender_adaptor.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.7/tessagon/adaptors/list_adaptor.py` & `tessagon-0.8/tessagon/adaptors/list_adaptor.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.7/tessagon/adaptors/vtk_adaptor.py` & `tessagon-0.8/tessagon/adaptors/vtk_adaptor.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.7/tessagon/core/abstract_tile.py` & `tessagon-0.8/tessagon/core/abstract_tile.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 class AbstractTile(ValueBlend):
     def __init__(self, tessagon, **kwargs):
         self.tessagon = tessagon
         self.f = tessagon.f
 
         # Verts/faces indexed with 'left', 'right', 'center'
-        self.u_symmetric = False
+        self.u_symmetric = kwargs.get('u_symmetric', False)
         # Verts/faces indexed with 'bottom', 'middle', 'top'
-        self.v_symmetric = False
+        self.v_symmetric = kwargs.get('v_symmetric', False)
 
-        if 'u_symmetric' in kwargs:
-            self.u_symmetric = kwargs['u_symmetric']
-        if 'v_symmetric' in kwargs:
-            self.v_symmetric = kwargs['v_symmetric']
+        # Verts/faces with 'rotate' and a number.
+        # Only rot_symmetric = 180 supported
+        # TODO: implement rot_symmetric = 90 as needed
+        self.rot_symmetric = kwargs.get('rot_symmetry', None)
 
         self.id = None
         # This is not necessary to any of the calculations, just
         # makes debugging easier
         if 'id' in kwargs:
             self.id = kwargs['id']
 
@@ -64,14 +64,30 @@
         tile = self
         for key in self._neighbor_path(neighbor_keys):
             if not tile.neighbors[key]:
                 return None
             tile = tile.neighbors[key]
         return tile
 
+    @property
+    def left(self):
+        return self.get_neighbor_tile(["left"])
+
+    @property
+    def right(self):
+        return self.get_neighbor_tile(["right"])
+
+    @property
+    def top(self):
+        return self.get_neighbor_tile(["top"])
+
+    @property
+    def bottom(self):
+        return self.get_neighbor_tile(["bottom"])
+
     def inspect(self, **kwargs):
         # For debugging topology
         if not self.id:
             return
         prefix = 'Tile'
         if 'tile_number' in kwargs:
             prefix += " #%s" % (kwargs['tile_number'])
@@ -98,14 +114,15 @@
     # and setting the vertices and faces on a tile
     def _get_nested_list_value(self, nested_list, index_keys):
         if not isinstance(index_keys, list):
             return nested_list[index_keys]
         value = nested_list
         for index in index_keys:
             value = value[index]
+
         return value
 
     def _set_nested_list_value(self, nested_list, index_keys, value):
         if not isinstance(index_keys, list):
             nested_list[index_keys] = value
             return
         reference = nested_list
@@ -136,37 +153,56 @@
         path = index_keys
         if self._should_twist_u(neighbor_keys):
             path = self._u_flip(path)
         if self._should_twist_v(neighbor_keys):
             path = self._v_flip(path)
         return path
 
-    def _swap_value(self, index_keys, val1, val2):
-        # abstract function to swap two values in a list
+    def _permute_value(self, index_keys, vals):
+        # abstract function to permute values in a list
         # e.g., 'left' and 'right' in u_flip below
         if isinstance(index_keys, list):
-            return [self._swap_value(u, val1, val2) for u in index_keys]
-        if index_keys == val1:
-            return val2
-        if index_keys == val2:
-            return val1
+            return [self._permute_value(u, vals) for u in index_keys]
+        for i in range(len(vals)):
+            if index_keys == vals[i]:
+                return vals[(i+1) % len(vals)]
+
         return index_keys
 
+    def _swap_value(self, index_keys, val1, val2):
+        # abstract function to swap two values in a list
+        # e.g., 'left' and 'right' in u_flip below
+        return self._permute_value(index_keys, [val1, val2])
+
     def _u_flip(self, index_keys):
         # swap each left with right (and vice versa) in list
         if not self.u_symmetric:
             return index_keys
         return self._swap_value(index_keys, 'left', 'right')
 
     def _v_flip(self, index_keys):
         # swap each top with bottom (and vice versa) in list
         if not self.v_symmetric:
             return index_keys
         return self._swap_value(index_keys, 'bottom', 'top')
 
+    def _rotate_index(self, index_keys):
+        # rotate
+        if not self.rot_symmetric:
+            return index_keys
+        elif self.rot_symmetric == 180:
+            keys = self._permute_value(index_keys, ['rotate0', 'rotate180'])
+            keys = self._permute_value(keys, ['left', 'right'])
+            keys = self._permute_value(keys, ['top', 'bottom'])
+            return keys
+        elif self.rot_symmetric == 90:
+            return self._permute_value(index_keys,
+                                       ['rotate0', 'rotate90'
+                                        'rotate180', 'rotate270'])
+
     def _v_index(self, index_keys):
         # find either 'top' or 'bottom' in the list
         if ('bottom' in index_keys):
             return 'bottom'
         if ('top' in index_keys):
             return 'top'
         raise ValueError("no v_index found in %s" % (index_keys))
```

### Comparing `tessagon-0.7/tessagon/core/tessagon_discovery.py` & `tessagon-0.8/tessagon/core/tessagon_discovery.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,41 +20,55 @@
     import DissectedTriangleTessagon
 from tessagon.types.dissected_hex_quad_tessagon \
     import DissectedHexQuadTessagon
 from tessagon.types.dissected_hex_tri_tessagon \
     import DissectedHexTriTessagon
 from tessagon.types.penta_tessagon import PentaTessagon
 from tessagon.types.penta2_tessagon import Penta2Tessagon
+from tessagon.types.big_hex_tri_tessagon import BigHexTriTessagon
+from tessagon.types.stanley_park_tessagon import StanleyParkTessagon
+from tessagon.types.valemount_tessagon import ValemountTessagon
+from tessagon.types.cloverdale_tessagon import CloverdaleTessagon
+from tessagon.types.islamic_hex_stars_tessagon import IslamicHexStarsTessagon
+from tessagon.types.islamic_stars_crosses_tessagon \
+    import IslamicStarsCrossesTessagon
 
 ALL = [SquareTessagon,
        HexTessagon,
        TriTessagon,
 
        OctoTessagon,
        HexTriTessagon,
        HexSquareTriTessagon,
        DodecaTessagon,
        SquareTriTessagon,
        SquareTri2Tessagon,
        DodecaTriTessagon,
+       BigHexTriTessagon,
 
        RhombusTessagon,
        FloretTessagon,
        DissectedSquareTessagon,
        DissectedTriangleTessagon,
        DissectedHexQuadTessagon,
        DissectedHexTriTessagon,
        PentaTessagon,
        Penta2Tessagon,
 
        PythagoreanTessagon,
        BrickTessagon,
        WeaveTessagon,
        HexBigTriTessagon,
-       ZigZagTessagon]
+       ZigZagTessagon,
+       ValemountTessagon,
+       CloverdaleTessagon,
+
+       StanleyParkTessagon,
+       IslamicHexStarsTessagon,
+       IslamicStarsCrossesTessagon]
 
 
 class TessagonDiscovery:
     def __init__(self, **kwargs):
         self.classes = kwargs.get('classes', ALL)
 
     def count(self):
@@ -76,15 +90,15 @@
         return TessagonDiscovery(classes=new_classes)
 
     def with_color_patterns(self):
         results = []
         for klass in self.classes:
             if klass.metadata is None:
                 continue
-            if klass.metadata.has_color_patterns():
+            if klass.metadata.has_color_patterns:
                 results.append(klass)
         return TessagonDiscovery(classes=results)
 
     def with_classification(self, classification):
         results = []
         for klass in self.classes:
             if klass.metadata is None:
```

### Comparing `tessagon-0.7/tessagon/core/tile.py` & `tessagon-0.8/tessagon/core/tile.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,28 +10,37 @@
 
         self.verts = self.init_verts()
         self.faces = self.init_faces()
         self.color_pattern = kwargs.get('color_pattern') or None
         if self.faces and self.color_pattern:
             self.face_paths = self.all_face_paths()
 
+    def validate(self):
+        # Subclass decides if this should be done
+        pass
+
     def add_vert(self, index_keys, ratio_u, ratio_v, **kwargs):
         # Use the mesh adaptor to create a vertex.
         # In reality, multiple vertices may get defined if symmetry is declared
         vert = self._get_vert(index_keys)
         if vert is None:
             coords = self.f(*self.blend(ratio_u, ratio_v))
             vert = self.mesh_adaptor.create_vert(coords)
 
             self._set_vert(index_keys, vert)
             if 'vert_type' in kwargs:
                 if not kwargs['vert_type'] in self.tessagon.vert_types:
                     self.tessagon.vert_types[kwargs['vert_type']] = []
                 self.tessagon.vert_types[kwargs['vert_type']].append(vert)
 
+        if vert is not None:
+            equivalent_verts = kwargs.get('equivalent', [])
+            for equivalent_vert in equivalent_verts:
+                self.set_equivalent_vert(*equivalent_vert, vert)
+
         # We add additional vertices by flipping 'left', 'right' etc
         # if the tile has some kind of symmetry defined
         self._create_symmetric_verts(index_keys, ratio_u, ratio_v, **kwargs)
 
         # On the boundary, make sure equivalent vertices are set on
         # neighbor tiles
         self._set_equivalent_neighbor_verts(index_keys, vert, **kwargs)
@@ -50,35 +59,44 @@
             return None
 
         tile._set_vert(self._index_path(index_keys, neighbor_keys), vert)
 
     def add_face(self, index_keys, vert_index_keys_list, **kwargs):
         # Use the mesh adaptor to create a face.
         # In reality, multiple faces may get defined if symmetry is declared
-        if self._get_face(index_keys) is not None:
-            return None
+        face = self._get_face(index_keys)
 
-        verts = self._get_verts_from_list(vert_index_keys_list)
-        if verts is None:
-            return None
+        if face is None:
+            verts = self._get_verts_from_list(vert_index_keys_list)
+            if verts is not None:
+                face = \
+                    self._make_face(index_keys, verts, **kwargs)
+
+        if face is not None:
+            equivalent_faces = kwargs.get('equivalent', [])
+            for equivalent_face in equivalent_faces:
+                self.set_equivalent_face(*equivalent_face, face)
+
+        # We add additional faces by flipping 'left', 'right' etc
+        # if the tile has some kind of symmetry defined
+        self._create_symmetric_faces(index_keys, vert_index_keys_list,
+                                     **kwargs)
 
+        return face
+
+    def _make_face(self, index_keys, verts, **kwargs):
         face = self.mesh_adaptor.create_face(verts)
         self._set_face(index_keys, face)
 
         # The tessagon might keep a list of specific face types
         if 'face_type' in kwargs:
             if not kwargs['face_type'] in self.tessagon.face_types:
                 self.tessagon.face_types[kwargs['face_type']] = []
             self.tessagon.face_types[kwargs['face_type']].append(face)
 
-        # We add additional faces by flipping 'left', 'right' etc
-        # if the tile has some kind of symmetry defined
-        self._create_symmetric_faces(index_keys, vert_index_keys_list,
-                                     **kwargs)
-
         # On the boundary, make sure equivalent faces are set on neighbor tiles
         self._set_equivalent_neighbor_faces(index_keys, face, **kwargs)
 
         return face
 
     def num_color_patterns(self):
         return self.tessagon.num_color_patterns()
@@ -163,14 +181,32 @@
             return None
         return tile._get_vert(self._index_path(index_keys, neighbor_keys))
 
     def _create_symmetric_verts(self, index_keys, ratio_u, ratio_v, **kwargs):
         # The 'symmetry' keyword is just to ensure we don't recurse forever
         if 'symmetry' not in kwargs:
             extra_args = {'symmetry': True}
+            if self.rot_symmetric == 180:
+                rot_keys = self._rotate_index(index_keys)
+                self.add_vert(rot_keys, 1.0 - ratio_u, 1 - ratio_v,
+                              **{**kwargs, **extra_args})
+
+            elif self.rot_symmetric == 90:
+                rot_keys = self._rotate_index(index_keys)
+                self.add_vert(rot_keys, 1.0 - ratio_v, ratio_u,
+                              **{**kwargs, **extra_args})
+
+                rot_keys = self._rotate_index(rot_keys)
+                self.add_vert(rot_keys, 1.0 - ratio_u, 1 - ratio_v,
+                              **{**kwargs, **extra_args})
+
+                rot_keys = self._rotate_index(rot_keys)
+                self.add_vert(rot_keys, ratio_v, 1 - ratio_u,
+                              **{**kwargs, **extra_args})
+
             if self.u_symmetric:
                 # Add reflection about u
                 u_flip_keys = self._u_flip(index_keys)
                 self.add_vert(u_flip_keys, 1.0 - ratio_u, ratio_v,
                               **{**kwargs, **extra_args})
                 if self.v_symmetric:
                     # Add diagonally across
@@ -213,15 +249,16 @@
         uv_flip_keys = self._v_flip(u_flip_keys)
         self.set_equivalent_vert([u_index, v_index], uv_flip_keys, vert,
                                  **kwargs)
 
     def _get_verts_from_list(self, vert_index_keys_list):
         verts = []
         for vert_index_keys in vert_index_keys_list:
-            if isinstance(vert_index_keys[0], list):
+            if isinstance(vert_index_keys, list) \
+               and isinstance(vert_index_keys[0], list):
                 vert = self._get_neighbor_vert(vert_index_keys[0],
                                                vert_index_keys[1])
             else:
                 vert = self._get_vert(vert_index_keys)
 
             if vert is None:
                 return None
@@ -230,14 +267,27 @@
         return verts
 
     def _create_symmetric_faces(self, index_keys, vert_index_keys_list,
                                 **kwargs):
         # The 'symmetry' keyword is just to ensure we don't recurse forever
         if 'symmetry' not in kwargs:
             extra_args = {'symmetry': True}
+            if self.rot_symmetric == 180:
+                rot_keys = self._rotate_index(index_keys)
+                rot_vert_index_keys_list \
+                    = self._rotate_index(vert_index_keys_list)
+                if 'equivalent' in kwargs:
+                    equivalent_faces = kwargs['equivalent']
+                    kwargs = kwargs.copy()
+                    kwargs['equivalent'] = \
+                        [self._rotate_index(equivalent_face)
+                         for equivalent_face in equivalent_faces]
+
+                self.add_face(rot_keys, rot_vert_index_keys_list,
+                              **{**kwargs, **extra_args})
             if self.u_symmetric:
                 # Add reflection about u
                 u_flip_keys = self._u_flip(index_keys)
                 u_flip_vert_index_keys_list \
                     = self._u_flip(vert_index_keys_list)
                 self.add_face(u_flip_keys, u_flip_vert_index_keys_list,
                               **{**kwargs, **extra_args})
```

### Comparing `tessagon-0.7/tessagon/core/value_blend.py` & `tessagon-0.8/tessagon/core/value_blend.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.7/tessagon/misc/shapes.py` & `tessagon-0.8/tessagon/misc/shapes.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.7/tessagon/types/brick_tessagon.py` & `tessagon-0.8/tessagon/types/brick_tessagon.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import left_tile, bottom_tile
 
 metadata = TessagonMetadata(name='Bricks',
                             num_color_patterns=1,
                             classification='non_edge',
                             shapes=['rectangles'],
-                            sides=[4])
+                            sides=[4],
+                            uv_ratio=1.0)
 
 
 class BrickTile(Tile):
     #                 top
     #
     #    -o..o-      -o..o- r
     # ^  .|..|.    l .|..|. i
@@ -42,28 +44,28 @@
     def calculate_faces(self):
         # Add left, symmetry gives the right side face
         self.add_face('left',
                       [['left', 'top'],
                        ['left', 'middle'],
                        ['left', 'bottom'],
                        # Verts on neighbor tiles:
-                       [['left'], ['right', 'bottom']],
-                       [['left'], ['right', 'middle']],
-                       [['left'], ['right', 'top']]],
+                       left_tile(['right', 'bottom']),
+                       left_tile(['right', 'middle']),
+                       left_tile(['right', 'top'])],
                       u_boundary=True)
 
         # Add bottom, symmetry gives the top face
         self.add_face('bottom',
                       [['right', 'bottom'],
                        ['right', 'middle'],
                        ['left', 'middle'],
                        ['left', 'bottom'],
                        # Verts on neighbor tiles:
-                       [['bottom'], ['left', 'middle']],
-                       [['bottom'], ['right', 'middle']]],
+                       bottom_tile(['left', 'middle']),
+                       bottom_tile(['right', 'middle'])],
                       v_boundary=True)
 
     def color_pattern1(self):
         self.color_paths([
             ['left'],
             ['right']
         ], 1, 0)
```

### Comparing `tessagon-0.7/tessagon/types/dissected_hex_quad_tessagon.py` & `tessagon-0.8/tessagon/types/dissected_hex_quad_tessagon.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from math import sqrt
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import left_tile
 
 metadata = TessagonMetadata(name='Hexagons Dissected with Quads',
                             num_color_patterns=2,
                             classification='laves',
                             shapes=['quads'],
-                            sides=[4])
+                            sides=[4],
+                            uv_ratio=1.0/sqrt(3.0))
 
 
 class DissectedHexQuadTile(Tile):
     # 19 verts, 14 quad faces (10 internal, 4 on boundary)
     #
     #  O+++++++++++++++++++O+++++++++++++++++++O
     #   +                  +                  +
@@ -112,15 +115,15 @@
                        ['center', 'top', 'interior'],
                        ['left', 'top', 'interior']])
 
         self.add_face(['left', 'top', 'u_boundary'],
                       [['left', 'top', 'corner'],
                        ['left', 'top', 'interior'],
                        ['left', 'top', 'u_boundary'],
-                       [['left'], ['right', 'top', 'interior']]],
+                       left_tile(['right', 'top', 'interior'])],
                       u_boundary=True)
 
         self.add_face(['left', 'top', 'middle'],
                       [['left', 'top', 'interior'],
                        ['center', 'middle'],
                        ['left', 'middle'],
                        ['left', 'top', 'u_boundary']])
```

### Comparing `tessagon-0.7/tessagon/types/dissected_hex_tri_tessagon.py` & `tessagon-0.8/tessagon/types/dissected_hex_tri_tessagon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from math import sqrt
 from tessagon.types.dissected_hex_quad_tessagon import DissectedHexQuadTile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
 
 metadata = TessagonMetadata(name='Hexagons Dissected with Triangles',
                             num_color_patterns=1,
                             classification='laves',
                             shapes=['triangles'],
-                            sides=[3])
+                            sides=[3],
+                            uv_ratio=1.0/sqrt(3.0))
 
 
 # Uses the same configuration of vertices as DissectedHexQuadTile
 class DissectedHexTriTile(DissectedHexQuadTile):
 
     # 19 verts, 24 internal triangle faces
     #
```

### Comparing `tessagon-0.7/tessagon/types/dissected_square_tessagon.py` & `tessagon-0.8/tessagon/types/dissected_square_tessagon.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon_metadata import TessagonMetadata
 
 metadata = TessagonMetadata(name='Dissected Square',
                             num_color_patterns=2,
                             classification='laves',
                             shapes=['triangles'],
-                            sides=[3])
+                            sides=[3],
+                            uv_ratio=1.0)
 
 
 class DissectedSquareTile(Tile):
 
     #    VERTS:     a = ['top', 'left']
     #    a---b---c  b = ['top', 'center']
     # ^  |\..|../|  c = ['top', 'right']
```

### Comparing `tessagon-0.7/tessagon/types/dissected_triangle_tessagon.py` & `tessagon-0.8/tessagon/types/dissected_triangle_tessagon.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from math import sqrt
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import top_tile
 
 metadata = TessagonMetadata(name='Dissected Triangle',
                             num_color_patterns=1,
                             classification='laves',
                             shapes=['triangles'],
-                            sides=[3])
+                            sides=[3],
+                            uv_ratio=sqrt(3.0))
 
 
 class DissectedTriangleTile(Tile):
     #     11 verts:
     #
     #     O++++++++++++O      +      O++++++++++++O
     #     ++ ++         ++    +    ++         ++ ++
@@ -88,15 +91,15 @@
                       [['left', 'middle'],
                        ['left', 'top', 'corner'],
                        ['left', 'bottom', 'corner']])
 
         self.add_face(['left', 'top', 'center'],
                       [['center'],
                        ['left', 'top', 'v_boundary'],
-                       [['top'], ['center']]], v_boundary=True)
+                       top_tile(['center'])], v_boundary=True)
 
         self.add_face(['left', 'top', 'interior1'],
                       [['center'],
                        ['left', 'top', 'v_boundary'],
                        ['left', 'top', 'corner']])
 
         self.add_face(['left', 'top', 'interior2'],
```

### Comparing `tessagon-0.7/tessagon/types/dodeca_tessagon.py` & `tessagon-0.8/tessagon/types/dodeca_tessagon.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from math import sqrt
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import top_tile, left_tile, left_top_tile
 
 # Will my brain survive this one?
 
 metadata = TessagonMetadata(name='Dodecagons, Hexagons, and Squares',
                             num_color_patterns=1,
                             classification='archimedean',
                             shapes=['dodecagons', 'hexagons', 'squares'],
-                            sides=[12, 6, 4])
+                            sides=[12, 6, 4],
+                            uv_ratio=1.0/sqrt(3.0))
 
 
 class DodecaTile(Tile):
     # 24 verts, 19 faces (7 internal, 12 on boundary)
     # The angles make it hard to draw all edges, some excluded
 
     #     .......|.4.|.......
@@ -122,23 +124,23 @@
 
     def calculate_faces(self):
         # Top left Dodecagon
         self.add_face(['dodec', 'top', 'left'],
                       [['top', 'left', 'v_square'],
                        ['top', 'left', 'sq4'],
                        ['top', 'left', 'sq3'],
-                       [['left'], ['top', 'right', 'sq3']],
-                       [['left'], ['top', 'right', 'sq4']],
-                       [['left'], ['top', 'right', 'v_square']],
-                       [['left', 'top'], ['bottom', 'right', 'v_square']],
-                       [['left', 'top'], ['bottom', 'right', 'sq4']],
-                       [['left', 'top'], ['bottom', 'right', 'sq3']],
-                       [['top'], ['bottom', 'left', 'sq3']],
-                       [['top'], ['bottom', 'left', 'sq4']],
-                       [['top'], ['bottom', 'left', 'v_square']]],
+                       left_tile(['top', 'right', 'sq3']),
+                       left_tile(['top', 'right', 'sq4']),
+                       left_tile(['top', 'right', 'v_square']),
+                       left_top_tile(['bottom', 'right', 'v_square']),
+                       left_top_tile(['bottom', 'right', 'sq4']),
+                       left_top_tile(['bottom', 'right', 'sq3']),
+                       top_tile(['bottom', 'left', 'sq3']),
+                       top_tile(['bottom', 'left', 'sq4']),
+                       top_tile(['bottom', 'left', 'v_square'])],
                       face_type='dodecagon', corner=True)
         # Middle Dodecagon
         self.add_face(['dodec', 'middle'],
                       [['top', 'left', 'u_square'],
                        ['top', 'left', 'sq1'],
                        ['top', 'left', 'sq2'],
                        ['top', 'right', 'sq2'],
@@ -151,23 +153,23 @@
                        ['bottom', 'left', 'sq1'],
                        ['bottom', 'left', 'u_square']],
                       face_type='dodecagon')
         # Upper square
         self.add_face(['square', 'top', 'center'],
                       [['top', 'left', 'v_square'],
                        ['top', 'right', 'v_square'],
-                       [['top'], ['bottom', 'right', 'v_square']],
-                       [['top'], ['bottom', 'left', 'v_square']]],
+                       top_tile(['bottom', 'right', 'v_square']),
+                       top_tile(['bottom', 'left', 'v_square'])],
                       face_type='square', v_boundary=True)
         # Left square
         self.add_face(['square', 'middle', 'left'],
                       [['top', 'left', 'u_square'],
                        ['bottom', 'left', 'u_square'],
-                       [['left'], ['bottom', 'right', 'u_square']],
-                       [['left'], ['top', 'right', 'u_square']]],
+                       left_tile(['bottom', 'right', 'u_square']),
+                       left_tile(['top', 'right', 'u_square'])],
                       face_type='square', u_boundary=True)
         # Interior square
         self.add_face(['square', 'top', 'left'],
                       [['top', 'left', 'sq1'],
                        ['top', 'left', 'sq2'],
                        ['top', 'left', 'sq4'],
                        ['top', 'left', 'sq3']],
@@ -182,17 +184,17 @@
                        ['top', 'right', 'sq2']],
                       face_type='hexagon')
         # Left Hex
         self.add_face(['hex', 'top', 'left'],
                       [['top', 'left', 'sq3'],
                        ['top', 'left', 'sq1'],
                        ['top', 'left', 'u_square'],
-                       [['left'], ['top', 'right', 'u_square']],
-                       [['left'], ['top', 'right', 'sq1']],
-                       [['left'], ['top', 'right', 'sq3']]],
+                       left_tile(['top', 'right', 'u_square']),
+                       left_tile(['top', 'right', 'sq1']),
+                       left_tile(['top', 'right', 'sq3'])],
                       face_type='hexagon', u_boundary=True)
 
     def color_pattern1(self):
         self.color_face(['dodec', 'middle'], 1)
         self.color_face(['dodec', 'top', 'left'], 1)
 
         self.color_face(['hex', 'top', 'left'], 2)
```

### Comparing `tessagon-0.7/tessagon/types/dodeca_tri_tessagon.py` & `tessagon-0.8/tessagon/types/stanley_park_tessagon.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,143 +1,142 @@
 from math import sqrt
-from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
+from tessagon.core.tile import Tile
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import top_tile, bottom_tile, \
+    top_left_tile, left_tile
 
-metadata = TessagonMetadata(name='Dodecagons and Triangles',
-                            num_color_patterns=1,
-                            classification='archimedean',
-                            shapes=['dodecagons', 'triangles'],
-                            sides=[12, 3])
-
-
-class DodecaTriTile(Tile):
-    # 14 verts, 11 faces (3 internal, 8 on boundary)
-    # The angles make it hard to draw all edges, some excluded
-
-    #     . ....|3.o---o.3|......
-    #  ^  .     o         o     .
-    #  |  . 12 /           \ 12 .
-    #  |  .   o             o   .
-    #  |  .-o3|      12     |3o-. Number is verts in face
-    #  |  .   o             o   .
-    #     .    \           /    .
-    #  V  . 12  o         o 12  .
-    #     . ....|3.o---o.3|......
+metadata = TessagonMetadata(name='Stanley Park',
+                            num_color_patterns=2,
+                            classification='non_convex',
+                            sides=[12],
+                            uv_ratio=sqrt(3.0))
+
+# Non-convex pattern. Might work better for 2D than 3D
+# Also, the ASCII art below is a bit hard to visualize,
+# so check out preview images linked from README.md
+
+
+class StanleyParkTile(Tile):
+    #    VERTS:
+    #   ....a...b....  a = ['top', 'left']
+    # ^ .../.....\...  b = ['top', 'right']
+    # | ..c.......d..  c = ['mid1', 'left']
+    # | ..|.......|..  d = ['mid1', 'right']
+    # | ..e...f...g .  e = ['mid2', 'left']
+    # | ./.\./.\./.\.  f = ['mid2', 'center']
+    #   h...i...j...k  g = ['mid2', 'right']
+    # V ....|...|....  h = ['mid3', 'left', 'outer']
+    #   ....l...m....  i = ['mid3', 'left', 'inner']
+    #                  j = ['mid3', 'right', 'inner']
+    #     U --->       k = ['mid3', 'right', 'outer']
+    #                  l = ['bottom', 'left']
+    #                  m = ['bottom', 'right']
+
+    #    FACES:
+    #   ....o...o....
+    # ^ .A./.....\.C.  A = ['top', 'left']
+    # | ..o...B...o..  B = ['top', 'middle']
+    # | ..|.......|..  C = ['top', 'right']
+    # | ..o...o...o .  D = ['bottom', 'left']
+    # | ./.\./.\./.\.  E = ['bottom', 'middle']
+    #   o...o...o...o  F = ['bottom', 'right']
+    # V ..D.|.E.|.F..
+    #   ....o...o....
     #
-    #            U ---->
+    #     U --->
 
     def __init__(self, tessagon, **kwargs):
         super().__init__(tessagon, **kwargs)
         self.u_symmetric = True
-        self.v_symmetric = True
+        self.v_symmetric = False
 
     def init_verts(self):
-        # u_square means on the square that is on the U-boundary
-        return {'left': {'top': {'v_boundary': None,
-                                 'diag': None,
-                                 'tri': None},  # on the triangle
-                         'middle': None,
-                         'bottom': {'v_boundary': None,
-                                    'diag': None,
-                                    'tri': None}},
-                'right': {'top': {'v_boundary': None,
-                                  'diag': None,
-                                  'tri': None},  # on the triangle
-                          'middle': None,
-                          'bottom': {'v_boundary': None,
-                                     'diag': None,
-                                     'tri': None}}}
+        return {'top': {'left': None,
+                        'right': None},
+                'mid1': {'left': None,
+                         'right': None},
+                'mid2': {'left': None,
+                         'center': None,
+                         'right': None},
+                'mid3': {'left': {'outer': None,
+                                  'inner': None},
+                         'right': {'inner': None,
+                                   'outer': None}},
+                'bottom': {'left': None,
+                           'right': None}}
 
     def init_faces(self):
-        return {'dodec': {'left': {'top': None,
-                                   'bottom': None},
-                          'right': {'top': None,
-                                    'bottom': None},
-                          'center': None},
-                'tri': {'left': {'top': None,
-                                 'middle': None,
-                                 'bottom': None},
-                        'right': {'top': None,
-                                  'middle': None,
-                                  'bottom': None}}}
+        return {'top': {'left': None,
+                        'center': None,
+                        'right': None},
+                'bottom': {'left': None,
+                           'center': None,
+                           'right': None}}
 
     def calculate_verts(self):
-        # u_unit is the length of the edges expressed as a
-        # proportion of the tile
-        u_unit = 1.0 / (3.0 + 2.0 * sqrt(3))
-        u_h = 0.5*sqrt(3)*u_unit  # height of triangle of side u_unit
-
-        u1 = 0.5*u_unit
-        u2 = u1 + u_h
-        u3 = u2 + u1
-        u4 = u3 + u_h
-
-        v_unit = 1.0 / (2.0 + sqrt(3))
-        v_h = 0.5*sqrt(3)*v_unit  # height of triangle of side v_unit
-        v1 = 0
-        v2 = 0.5 * v_unit
-        v3 = v2 + v_h
-        v4 = 0.5
-
-        # Sweet symmetry makes this easy work
-        self.add_vert(['left', 'middle'], u1, v4)  # 2 verts added
-        self.add_vert(['left', 'bottom', 'v_boundary'], u4, v1,
-                      v_boundary=True)  # 4 verts
-        self.add_vert(['left', 'bottom', 'diag'], u3, v2)  # 4 verts
-        self.add_vert(['left', 'bottom', 'tri'], u2, v3)  # 4 verts
+        vert = self.add_vert(['top', 'left'], 2.0/6.0, 1.0)
+        self.set_equivalent_vert(*top_tile(['bottom', 'left']), vert)
+        # Reflection doesn't handle 'set_equivalent_vert' so ...
+        vert = self.add_vert(['top', 'right'], 4.0/6.0, 1.0)
+        self.set_equivalent_vert(*top_tile(['bottom', 'right']), vert)
+
+        self.add_vert(['mid1', 'left'], 1.0/6.0, 5.0/6.0)
+        self.add_vert(['mid2', 'left'], 1.0/6.0, 3.0/6.0)
+        self.add_vert(['mid2', 'center'], 3.0/6.0, 3.0/6.0)
+        self.add_vert(['mid3', 'left', 'outer'], 0.0, 2.0/6.0,
+                      u_boundary=True)
+        self.add_vert(['mid3', 'left', 'inner'], 2.0/6.0, 2.0/6.0)
+
+        vert = self.add_vert(['bottom', 'left'], 2.0/6.0, 0.0)
+        self.set_equivalent_vert(*bottom_tile(['top', 'left']), vert)
+        vert = self.add_vert(['bottom', 'right'], 4.0/6.0, 0.0)
+        self.set_equivalent_vert(*bottom_tile(['top', 'right']), vert)
 
     def calculate_faces(self):
-        # Top left Dodecagon
-        self.add_face(['dodec', 'left', 'bottom'],
-                      [['left', 'middle'],
-                       ['left', 'bottom', 'tri'],
-                       ['left', 'bottom', 'diag'],
-                       [['bottom'], ['left', 'top', 'diag']],
-                       [['bottom'], ['left', 'top', 'tri']],
-                       [['bottom'], ['left', 'middle']],
-                       [['bottom', 'left'], ['right', 'middle']],
-                       [['bottom', 'left'], ['right', 'top', 'tri']],
-                       [['bottom', 'left'], ['right', 'top', 'diag']],
-                       [['left'], ['right', 'bottom', 'diag']],
-                       [['left'], ['right', 'bottom', 'tri']],
-                       [['left'], ['right', 'middle']]],
-                      face_type='dodecagon', corner=True)
-
-        # Middle Dodecagon
-        self.add_face(['dodec', 'center'],
-                      [['left', 'bottom', 'tri'],
-                       ['left', 'bottom', 'diag'],
-                       ['left', 'bottom', 'v_boundary'],
-                       ['right', 'bottom', 'v_boundary'],
-                       ['right', 'bottom', 'diag'],
-                       ['right', 'bottom', 'tri'],
-                       ['right', 'top', 'tri'],
-                       ['right', 'top', 'diag'],
-                       ['right', 'top', 'v_boundary'],
-                       ['left', 'top', 'v_boundary'],
-                       ['left', 'top', 'diag'],
-                       ['left', 'top', 'tri']],
-                      face_type='dodecagon')
-
-        # Left triangle
-        self.add_face(['tri', 'left', 'middle'],
-                      [['left', 'top', 'tri'],
-                       ['left', 'bottom', 'tri'],
-                       ['left', 'middle']],
-                      face_type='triangle')
-
-        # bottom-left triangle
-        self.add_face(['tri', 'left', 'bottom'],
-                      [['left', 'bottom', 'diag'],
-                       ['left', 'bottom', 'v_boundary'],
-                       [['bottom'], ['left', 'top', 'diag']]],
-                      face_type='triangle', v_boundary=True)
+        face = self.add_face(['top', 'left'],
+                             [['mid3', 'left', 'outer'],
+                              ['mid2', 'left'],
+                              ['mid1', 'left'],
+                              ['top', 'left'],
+                              top_tile(['mid3', 'left', 'inner']),
+                              top_tile(['mid2', 'left']),
+                              top_tile(['mid3', 'left', 'outer']),
+                              top_left_tile(['mid2', 'right']),
+                              top_left_tile(['mid3', 'right', 'inner']),
+                              left_tile(['top', 'right']),
+                              left_tile(['mid1', 'right']),
+                              left_tile(['mid2', 'right'])],
+                             u_boundary=True)
+        self.set_equivalent_face(*top_tile(['bottom', 'left']), face)
+        self.set_equivalent_face(*top_left_tile(['bottom', 'right']), face)
+        self.set_equivalent_face(*left_tile(['top', 'right']), face)
+
+        face = self.add_face(['top', 'center'],
+                             [['top', 'left'],
+                              ['mid1', 'left'],
+                              ['mid2', 'left'],
+                              ['mid3', 'left', 'inner'],
+                              ['mid2', 'center'],
+                              ['mid3', 'right', 'inner'],
+                              ['mid2', 'right'],
+                              ['mid1', 'right'],
+                              ['top', 'right'],
+                              top_tile(['mid3', 'right', 'inner']),
+                              top_tile(['mid2', 'center']),
+                              top_tile(['mid3', 'left', 'inner'])])
+        self.set_equivalent_face(*top_tile(['bottom', 'center']), face)
 
     def color_pattern1(self):
-        self.color_paths([['dodec', 'left', 'bottom'],
-                          ['dodec', 'center']], 1, 0)
+        self.color_face(['top', 'center'], 1)
+        self.color_face(['bottom', 'center'], 1)
+
+    def color_pattern2(self):
+        if self.fingerprint[1] % 2 == 0:
+            self.color_face(['top', 'left'], 1)
+            self.color_face(['top', 'center'], 1)
+            self.color_face(['top', 'right'], 1)
 
 
-class DodecaTriTessagon(Tessagon):
-    tile_class = DodecaTriTile
+class StanleyParkTessagon(Tessagon):
+    tile_class = StanleyParkTile
     metadata = metadata
```

### Comparing `tessagon-0.7/tessagon/types/hex_square_tri_tessagon.py` & `tessagon-0.8/tessagon/types/hex_square_tri_tessagon.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from math import sqrt
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import left_tile, top_tile, left_top_tile
 
 metadata = TessagonMetadata(name='Hexagons, Squares, and Triangles',
                             num_color_patterns=1,
                             classification='archimedean',
                             shapes=['hexagons', 'squares', 'triangles'],
-                            sides=[6, 4, 3])
+                            sides=[6, 4, 3],
+                            uv_ratio=1.0/sqrt(3.0))
 
 
 class HexSquareTriTile(Tile):
     # 14 verts, 19 faces (7 internal, 12 on boundary)
     # The angles make it hard to draw all edges, some excluded
     #
     #     ...|...|...  6..|.4.|..6
@@ -81,15 +83,15 @@
         u2 = 0.5*(1.0-u_unit)
         u3 = 0.5
 
         v_unit = 1.0 / (3.0 + sqrt(3))
         v0 = 1.0 - 0.5*v_unit
         v1 = 1.0 - v_unit
         v2 = 0.5 + v_unit
-        v3 = 1.0 - 2.0*v_unit
+        v3 = 0.5 + 0.5*v_unit
 
         # Define top left square, other verts defined through symmetry
         self.add_vert(['top', 'left', 'v_square'], u2, v0)
         self.add_vert(['top', 'center'], u3, v2)
         self.add_vert(['top', 'left', 'u_square'], u1, v3)
         self.add_vert(['top', 'left', 'u_boundary'], u0, v1, u_boundary=True)
 
@@ -105,23 +107,23 @@
                       face_type='hexagon')
 
         # Six top-left faces, rest defined via symmetry
         # Top square
         self.add_face(['square', 'top', 'center'],
                       [['top', 'left', 'v_square'],
                        ['top', 'right', 'v_square'],
-                       [['top'], ['bottom', 'right', 'v_square']],
-                       [['top'], ['bottom', 'left', 'v_square']]],
+                       top_tile(['bottom', 'right', 'v_square']),
+                       top_tile(['bottom', 'left', 'v_square'])],
                       face_type='square', v_boundary=True)
         # Left square
         self.add_face(['square', 'middle', 'left'],
                       [['top', 'left', 'u_square'],
                        ['bottom', 'left', 'u_square'],
-                       [['left'], ['bottom', 'right', 'u_square']],
-                       [['left'], ['top', 'right', 'u_square']]],
+                       left_tile(['bottom', 'right', 'u_square']),
+                       left_tile(['top', 'right', 'u_square'])],
                       face_type='square', u_boundary=True)
         # Interior square
         self.add_face(['square', 'top', 'left'],
                       [['top', 'left', 'v_square'],
                        ['top', 'center'],
                        ['top', 'left', 'u_square'],
                        ['top', 'left', 'u_boundary']],
@@ -132,24 +134,24 @@
                        ['top', 'left', 'v_square'],
                        ['top', 'right', 'v_square']],
                       face_type='triangle')
         # Left triangle
         self.add_face(['tri', 'top', 'left'],
                       [['top', 'left', 'u_square'],
                        ['top', 'left', 'u_boundary'],
-                       [['left'], ['top', 'right', 'u_square']]],
+                       left_tile(['top', 'right', 'u_square'])],
                       face_type='triangle', u_boundary=True)
         # Corner hexagon
         self.add_face(['hex', 'top', 'left'],
                       [['top', 'left', 'v_square'],
                        ['top', 'left', 'u_boundary'],
-                       [['left'], ['top', 'right', 'v_square']],
-                       [['left', 'top'], ['bottom', 'right', 'v_square']],
-                       [['top'], ['bottom', 'left', 'u_boundary']],
-                       [['top'], ['bottom', 'left', 'v_square']]],
+                       left_tile(['top', 'right', 'v_square']),
+                       left_top_tile(['bottom', 'right', 'v_square']),
+                       top_tile(['bottom', 'left', 'u_boundary']),
+                       top_tile(['bottom', 'left', 'v_square'])],
                       face_type='hexagon', corner=True)
 
     def color_pattern1(self):
         self.color_face(['hex', 'middle'], 1)
         self.color_face(['hex', 'top', 'left'], 1)
 
         # TODO: I'm not sure why I have to explicitely color
```

### Comparing `tessagon-0.7/tessagon/types/hex_tessagon.py` & `tessagon-0.8/tessagon/types/hex_tessagon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from math import sqrt
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import top_tile, top_left_tile, left_tile
 
 metadata = TessagonMetadata(name='Regular Hexagons',
                             num_color_patterns=2,
                             classification='regular',
                             shapes=['hexagons'],
-                            sides=[6])
+                            sides=[6],
+                            uv_ratio=1.0/sqrt(3.0))
 
 
 class HexTile(Tile):
     #    VERTS:
     #    ..|..
     #    ..a..  a = ['top', 'center']
     # ^  ./.\.  b = ['top', 'left']
@@ -82,18 +85,18 @@
         self.add_face(['top', 'left'],
                       # The first two verts of the face are on this tile
                       [['top', 'left'],
                        ['top', 'center'],
                        # The other four verts are on neighboring tiles.
                        # E.g., the next one is the ['bottom', 'center']
                        # vert on the top neighbor tile.
-                       [['top'], ['bottom', 'center']],
-                       [['top'], ['bottom', 'left']],
-                       [['top', 'left'], ['bottom', 'center']],
-                       [['left'], ['top', 'center']]],
+                       top_tile(['bottom', 'center']),
+                       top_tile(['bottom', 'left']),
+                       top_left_tile(['bottom', 'center']),
+                       left_tile(['top', 'center'])],
                       # Defining the face as a 'corner' also associates the
                       # created face as one that is shared with
                       # neighboring tiles.
                       corner=True)
 
     def color_pattern1(self):
         if self.fingerprint[0] % 3 == 0:
```

### Comparing `tessagon-0.7/tessagon/types/hex_tri_tessagon.py` & `tessagon-0.8/tessagon/types/hex_tri_tessagon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from math import sqrt
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
-
+from tessagon.core.tile_utils import left_tile, left_top_tile, top_tile
 metadata = TessagonMetadata(name='Hexagons and Triangles',
                             num_color_patterns=1,
                             classification='archimedean',
                             shapes=['hexagons', 'triangles'],
-                            sides=[6, 3])
+                            sides=[6, 3],
+                            uv_ratio=1.0/sqrt(3.0))
 
 
 class HexTriTile(Tile):
     #    ....o....
     #    .../.\...
     #  ^ --o---o--
     #  | ./.....\.
@@ -70,26 +72,26 @@
                       face_type='triangle')
 
         # Exterior left triangle
         self.add_face(['left', 'top', 'triangle'],
                       [['left', 'top'],
                        ['left', 'middle'],
                        # Verts on neighbor tiles
-                       [['left'], ['right', 'top']]],
+                       left_tile(['right', 'top'])],
                       face_type='triangle', u_boundary=True)
 
         # Exterior top-left hexagon
         self.add_face(['left', 'top', 'hexagon'],
                       [['top'],
                        ['left', 'top'],
                        # Verts on neighbor tiles
-                       [['left'], ['right', 'top']],
-                       [['left'], 'top'],
-                       [['left', 'top'], ['right', 'bottom']],
-                       [['top'], ['left', 'bottom']]],
+                       left_tile(['right', 'top']),
+                       left_tile('top'),
+                       left_top_tile(['right', 'bottom']),
+                       top_tile(['left', 'bottom'])],
                       face_type='hexagon', corner=True)
 
     def color_pattern1(self):
         # Color the hexagons
         self.color_face(['center', 'middle'], 1)
         self.color_face(['left', 'top', 'hexagon'], 1)
```

### Comparing `tessagon-0.7/tessagon/types/octo_tessagon.py` & `tessagon-0.8/tessagon/types/octo_tessagon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from math import sqrt
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import left_tile, top_tile
 
 # TODO: gulp, 'octagon' does not begin with 'octo'
 
 metadata = TessagonMetadata(name='Octagons and Squares',
                             num_color_patterns=1,
                             classification='archimedean',
                             shapes=['octagons', 'squares'],
-                            sides=[8, 4])
+                            sides=[8, 4],
+                            uv_ratio=1.0)
 
 
 class OctoTile(Tile):
     # ^  ..o-o..
     # |  ./...\.
     # |  o.....o
     # |  |.....|
@@ -65,16 +67,16 @@
                                  ['right', 'top', 'v_boundary']])
 
         # Four faces, define top left corner, others via symmetry
         self.add_face(['left', 'top'],
                       [['left', 'top', 'v_boundary'],
                        ['left', 'top', 'u_boundary'],
                        # Verts on neighbor tiles
-                       [['left'], ['right', 'top', 'v_boundary']],
-                       [['top'], ['left', 'bottom', 'u_boundary']]],
+                       left_tile(['right', 'top', 'v_boundary']),
+                       top_tile(['left', 'bottom', 'u_boundary'])],
                       corner=True)
 
     def color_pattern1(self):
         self.color_face(['middle'], 1)
 
 
 class OctoTessagon(Tessagon):
```

### Comparing `tessagon-0.7/tessagon/types/penta2_tessagon.py` & `tessagon-0.8/tessagon/types/penta2_tessagon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from math import sqrt
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import left_tile
 
 metadata = TessagonMetadata(name='Other Pentagons',
                             num_color_patterns=1,
                             classification='laves',
                             shapes=['pentagons'],
-                            sides=[5])
+                            sides=[5],
+                            uv_ratio=1.0/(2.0+sqrt(3.0)))
 
 
 class Penta2Tile(Tile):
     # 11 verts, 6 faces (2 internal, 4 on boundary)
     #
     #     O---O
     #     |...|
@@ -74,16 +76,17 @@
                        ['center', 'bottom'],
                        ['right', 'bottom', 'u_boundary'],
                        ['right', 'bottom', 'corner']])
         self.add_face(['left', 'bottom'],
                       [['center', 'middle'],
                        ['center', 'bottom'],
                        ['left', 'bottom', 'u_boundary'],
-                       [['left'], ['center', 'bottom']],
-                       [['left'], ['center', 'middle']]], u_boundary=True)
+                       left_tile(['center', 'bottom']),
+                       left_tile(['center', 'middle'])],
+                      u_boundary=True)
 
     def color_pattern1(self):
         self.color_paths([
             ['center', 'top'],
             ['left', 'bottom'],
             ['right', 'bottom']
         ], 1, 0)
```

### Comparing `tessagon-0.7/tessagon/types/penta_tessagon.py` & `tessagon-0.8/tessagon/types/penta_tessagon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from math import sqrt
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import left_tile, bottom_tile
 
 metadata = TessagonMetadata(name='Pentagons',
                             num_color_patterns=1,
                             classification='laves',
                             shapes=['pentagons'],
-                            sides=[5])
+                            sides=[5],
+                            uv_ratio=1.0)
 
 
 class PentaTile(Tile):
     # 16 verts, 12 faces (4 internal, 8 on boundaries)
     #
     #  +              O+++++++++O              +
     #  +             +           +             +
@@ -91,24 +93,24 @@
         self.add_vert(['center', 'bottom'], u4, v3)
 
     def calculate_faces(self):
         self.add_face(['left', 'bottom', 'u_boundary'],
                       [['left', 'bottom', 'u_boundary'],
                        ['left', 'bottom', 'interior'],
                        ['left', 'middle'],
-                       [['left'], ['right', 'middle']],
-                       [['left'], ['right', 'bottom', 'interior']]],
+                       left_tile(['right', 'middle']),
+                       left_tile(['right', 'bottom', 'interior'])],
                       u_boundary=True)
 
         self.add_face(['left', 'bottom', 'v_boundary'],
                       [['left', 'bottom', 'u_boundary'],
                        ['left', 'bottom', 'interior'],
                        ['left', 'bottom', 'v_boundary'],
-                       [['bottom'], ['left', 'top', 'interior']],
-                       [['bottom'], ['left', 'top', 'u_boundary']]],
+                       bottom_tile(['left', 'top', 'interior']),
+                       bottom_tile(['left', 'top', 'u_boundary'])],
                       v_boundary=True)
 
         self.add_face(['left', 'middle'],
                       [['left', 'middle'],
                        ['left', 'bottom', 'interior'],
                        ['center', 'bottom'],
                        ['center', 'top'],
```

### Comparing `tessagon-0.7/tessagon/types/rhombus_tessagon.py` & `tessagon-0.8/tessagon/types/rhombus_tessagon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from math import sqrt
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import left_tile, top_tile
 
 metadata = TessagonMetadata(name='Rhombuses',
                             num_color_patterns=2,
                             classification='laves',
                             shapes=['rhombuses'],
-                            sides=[4])
+                            sides=[4],
+                            uv_ratio=1.0/sqrt(3.0))
 
 
 class RhombusTile(Tile):
     #    ..o..
     #    ./|\.
     #    o.|.o
     # ^  |.o.|
@@ -62,16 +65,16 @@
                        ['left', 'top'],
                        ['left', 'middle'],
                        ['center', 'top', 'interior']], face_type='upward')
         self.add_face(['left', 'top', 'exterior'],
                       [['center', 'top', 'boundary'],
                        ['left', 'top'],
                        # Verts on neighbor tile
-                       [['left'], ['center', 'top', 'boundary']],
-                       [['top'], ['left', 'bottom']]],
+                       left_tile(['center', 'top', 'boundary']),
+                       top_tile(['left', 'bottom'])],
                       face_type='horizontal', corner=True)
 
     def color_pattern1(self):
         self.color_face(['middle'], 1)
         self.color_face(['left', 'top', 'exterior'], 1)
 
         self.color_face(['left', 'top', 'interior'], 2)
```

### Comparing `tessagon-0.7/tessagon/types/square_tessagon.py` & `tessagon-0.8/tessagon/types/square_tessagon.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon_metadata import TessagonMetadata
 
 metadata = TessagonMetadata(name='Regular Squares',
                             num_color_patterns=8,
                             classification='regular',
                             shapes=['squares'],
-                            sides=[4])
+                            sides=[4],
+                            uv_ratio=1.0)
 
 
 class SquareTile(Tile):
 
     def __init__(self, tessagon, **kwargs):
         super().__init__(tessagon, **kwargs)
         self.u_symmetric = True
```

### Comparing `tessagon-0.7/tessagon/types/square_tri2_tessagon.py` & `tessagon-0.8/tessagon/types/square_tri2_tessagon.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
 
 metadata = TessagonMetadata(name='Other Squares and Triangles',
                             num_color_patterns=1,
                             classification='archimedean',
                             shapes=['squares', 'triangles'],
-                            sides=[4, 3])
+                            sides=[4, 3],
+                            uv_ratio=1.0/(2.0+sqrt(3.0)))
 
 
 class SquareTri2Tile(Tile):
     # 6 verts, 11 faces (3 internal, 8 on boundary)
     #
     #  ^  ..|..
     #  |  --O--
```

### Comparing `tessagon-0.7/tessagon/types/square_tri_tessagon.py` & `tessagon-0.8/tessagon/types/square_tri_tessagon.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
 
 metadata = TessagonMetadata(name='Squares and Triangles',
                             num_color_patterns=2,
                             classification='archimedean',
                             shapes=['squares', 'triangles'],
-                            sides=[4, 3])
+                            sides=[4, 3],
+                            uv_ratio=1.0)
 
 
 class SquareTriTile(Tile):
     # 12 verts, 16 faces (8 internal, 8 on boundary)
     # The angles make it hard to draw all edges, some excluded
     #
     #
```

### Comparing `tessagon-0.7/tessagon/types/tri_tessagon.py` & `tessagon-0.8/tessagon/types/tri_tessagon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from math import sqrt
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import top_tile
 
 metadata = TessagonMetadata(name='Regular Triangles',
                             num_color_patterns=3,
                             classification='regular',
                             shapes=['triangles'],
-                            sides=[3])
+                            sides=[3],
+                            uv_ratio=sqrt(3.0))
 
 
 class TriTile(Tile):
 
     #  ^  0.|.1   This is the topology of the tile.
     #  |  |\|/|   (Not a Dead Kennedy's logo ...).
     #  |  |.2.|
@@ -41,15 +44,15 @@
 
     def calculate_faces(self):
         # Four corners, via symmetry
         self.add_face(['left', 'top'],
                       [['left', 'top'],
                        ['middle'],
                        # Vert on neighboring tile
-                       [['top'], ['middle']]], v_boundary=True)
+                       top_tile(['middle'])], v_boundary=True)
         # Two interior faces, via symmetry
         self.add_face(['left', 'middle'],
                       [['left', 'top'],
                        ['left', 'bottom'],
                        ['middle']])
 
     def color_pattern1(self):
```

### Comparing `tessagon-0.7/tessagon/types/weave_tessagon.py` & `tessagon-0.8/tessagon/types/weave_tessagon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import left_tile, top_tile, left_top_tile
 
 metadata = TessagonMetadata(name='Weave',
                             num_color_patterns=1,
                             classification='non_edge',
                             shapes=['quads', 'rectangles'],
-                            sides=[4])
+                            sides=[4],
+                            uv_ratio=1.0,
+                            extra_parameters={
+                                'square_ratio': {
+                                    'type': 'float',
+                                    'min': 0.0,
+                                    'max': 1.0,
+                                    'default': 0.5,
+                                    'description':
+                                    'Control the size of the squares'
+                                }
+                            })
 
 
 class WeaveTile(Tile):
     # 16 verts, 13 faces (5 internal, 8 on boundary)
     #
     #      ....|..|....  .8..|.8|.8..
     #      -o--o..o--o-  -o--o..o--o-
@@ -24,14 +36,15 @@
     #
     #        U ----->
 
     def __init__(self, tessagon, **kwargs):
         super().__init__(tessagon, **kwargs)
         self.u_symmetric = True
         self.v_symmetric = True
+        self.square_ratio = kwargs.get('square_ratio', 0.5)
 
     def init_verts(self):
         # u_square means on the square that is on the U-boundary
         return {'top': {'left': {'u_inner': {'v_inner': None,
                                              'v_outer': None},
                                  'u_outer': {'v_inner': None,
                                              'v_outer': None}},
@@ -60,19 +73,20 @@
                                    'center': None,
                                    'right': None},
                         'bottom': {'left': None,
                                    'center': None,
                                    'right': None}}}
 
     def calculate_verts(self):
-        u0 = 1.0/8.0
-        u1 = 3.0/8.0
+        half_square_size = 0.25 * self.square_ratio
+        u0 = 0.25 - half_square_size
+        u1 = 0.25 + half_square_size
 
-        v0 = 5.0/8.0
-        v1 = 7.0/8.0
+        v0 = 0.75 - half_square_size
+        v1 = 0.75 + half_square_size
 
         # Define top left square, other verts defined through symmetry
         self.add_vert(['top', 'left', 'u_inner', 'v_inner'], u1, v0)
         self.add_vert(['top', 'left', 'u_inner', 'v_outer'], u1, v1)
         self.add_vert(['top', 'left', 'u_outer', 'v_inner'], u0, v0)
         self.add_vert(['top', 'left', 'u_outer', 'v_outer'], u0, v1)
 
@@ -97,46 +111,46 @@
                        ['bottom', 'left', 'u_outer', 'v_inner']],
                       face_type='oct')
 
         # 4 corner strips
         self.add_face(['oct', 'top', 'left'],
                       [['top', 'left', 'u_inner', 'v_outer'],
                        ['top', 'left', 'u_outer', 'v_outer'],
-                       [['left'], ['top', 'right', 'u_outer', 'v_outer']],
-                       [['left'], ['top', 'right', 'u_inner', 'v_outer']],
-                       [['left', 'top'],
-                        ['bottom', 'right', 'u_inner', 'v_outer']],
-                       [['left', 'top'],
-                        ['bottom', 'right', 'u_outer', 'v_outer']],
-                       [['top'], ['bottom', 'left', 'u_outer', 'v_outer']],
-                       [['top'], ['bottom', 'left', 'u_inner', 'v_outer']]],
+                       left_tile(['top', 'right', 'u_outer', 'v_outer']),
+                       left_tile(['top', 'right', 'u_inner', 'v_outer']),
+                       left_top_tile(['bottom', 'right',
+                                      'u_inner', 'v_outer']),
+                       left_top_tile(['bottom', 'right',
+                                      'u_outer', 'v_outer']),
+                       top_tile(['bottom', 'left', 'u_outer', 'v_outer']),
+                       top_tile(['bottom', 'left', 'u_inner', 'v_outer'])],
                       face_type='oct', corner=True)
 
         # 2 side strips
         self.add_face(['oct', 'middle', 'left'],
                       [['top', 'left', 'u_outer', 'v_outer'],
                        ['top', 'left', 'u_outer', 'v_inner'],
                        ['bottom', 'left', 'u_outer', 'v_inner'],
                        ['bottom', 'left', 'u_outer', 'v_outer'],
-                       [['left'], ['bottom', 'right', 'u_outer', 'v_outer']],
-                       [['left'], ['bottom', 'right', 'u_outer', 'v_inner']],
-                       [['left'], ['top', 'right', 'u_outer', 'v_inner']],
-                       [['left'], ['top', 'right', 'u_outer', 'v_outer']]],
+                       left_tile(['bottom', 'right', 'u_outer', 'v_outer']),
+                       left_tile(['bottom', 'right', 'u_outer', 'v_inner']),
+                       left_tile(['top', 'right', 'u_outer', 'v_inner']),
+                       left_tile(['top', 'right', 'u_outer', 'v_outer'])],
                       face_type='oct', u_boundary=True)
 
         # 2 top/bottom strips
         self.add_face(['oct', 'top', 'center'],
                       [['top', 'left', 'u_inner', 'v_outer'],
                        ['top', 'left', 'u_inner', 'v_inner'],
                        ['top', 'right', 'u_inner', 'v_inner'],
                        ['top', 'right', 'u_inner', 'v_outer'],
-                       [['top'], ['bottom', 'right', 'u_inner', 'v_outer']],
-                       [['top'], ['bottom', 'right', 'u_inner', 'v_inner']],
-                       [['top'], ['bottom', 'left', 'u_inner', 'v_inner']],
-                       [['top'], ['bottom', 'left', 'u_inner', 'v_outer']]],
+                       top_tile(['bottom', 'right', 'u_inner', 'v_outer']),
+                       top_tile(['bottom', 'right', 'u_inner', 'v_inner']),
+                       top_tile(['bottom', 'left', 'u_inner', 'v_inner']),
+                       top_tile(['bottom', 'left', 'u_inner', 'v_outer'])],
                       face_type='oct', v_boundary=True)
 
     def color_pattern1(self):
         self.color_face(['oct', 'top', 'center'], 1)
         self.color_face(['oct', 'middle', 'left'], 1)
 
         self.color_face(['oct', 'top', 'left'], 2)
```

### Comparing `tessagon-0.7/tessagon/types/zig_zag_tessagon.py` & `tessagon-0.8/tessagon/types/zig_zag_tessagon.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from tessagon.core.tile import Tile
 from tessagon.core.tessagon import Tessagon
 from tessagon.core.tessagon_metadata import TessagonMetadata
+from tessagon.core.tile_utils import left_tile, right_tile, \
+    top_tile, bottom_tile, left_top_tile, left_bottom_tile, \
+    right_bottom_tile, right_top_tile
 
 metadata = TessagonMetadata(name='Zig-Zag',
                             num_color_patterns=1,
                             classification='non_edge',
                             shapes=['rectangles'],
-                            sides=[4])
+                            sides=[4],
+                            uv_ratio=1.0)
 
 
 class ZigZagTile(Tile):
     # 25 verts in five rows, five columns
     # 10 faces (2 sets shared with neighbors)
     #
     #    o-o-o-o.o  row5  o-o-o-o.o
@@ -56,33 +60,33 @@
                             if row == 4:
                                 continue
                         if not self.get_neighbor_tile(['bottom']):
                             if row == 1:
                                 continue
                 vert = self.add_vert([col, row], c[col], c[row])
                 if col == 1:
-                    self.set_equivalent_vert(['left'], [5, row], vert)
+                    self.set_equivalent_vert(*left_tile([5, row]), vert)
                     if row == 5:
-                        self.set_equivalent_vert(['left', 'top'], [5, 1],
+                        self.set_equivalent_vert(*left_top_tile([5, 1]),
                                                  vert)
                     elif row == 1:
-                        self.set_equivalent_vert(['left', 'bottom'], [5, 5],
+                        self.set_equivalent_vert(*left_bottom_tile([5, 5]),
                                                  vert)
                 elif col == 5:
-                    self.set_equivalent_vert(['right'], [1, row], vert)
+                    self.set_equivalent_vert(*right_tile([1, row]), vert)
                     if row == 5:
-                        self.set_equivalent_vert(['right', 'top'], [1, 1],
+                        self.set_equivalent_vert(*right_top_tile([1, 1]),
                                                  vert)
                     elif row == 1:
-                        self.set_equivalent_vert(['right', 'bottom'], [1, 5],
+                        self.set_equivalent_vert(*right_bottom_tile([1, 5]),
                                                  vert)
                 if row == 5:
-                    self.set_equivalent_vert(['top'], [col, 1], vert)
+                    self.set_equivalent_vert(*top_tile([col, 1]), vert)
                 elif row == 1:
-                    self.set_equivalent_vert(['bottom'], [col, 5], vert)
+                    self.set_equivalent_vert(*bottom_tile([col, 5]), vert)
 
     def calculate_faces(self):
         self.add_face(1, [[1, 5],
                           [1, 4],
                           [2, 4],
                           [3, 4],
                           [3, 5],
@@ -95,40 +99,40 @@
                           [4, 4],
                           [4, 5]])
 
         face = self.add_face(3, [[4, 5],
                                  [4, 4],
                                  [5, 4],
                                  [5, 5],
-                                 [['top'], [5, 2]],
-                                 [['top'], [4, 2]]])
-        self.set_equivalent_face(['top'], 10, face)
+                                 top_tile([5, 2]),
+                                 top_tile([4, 2])])
+        self.set_equivalent_face(*top_tile(10), face)
 
         face = self.add_face(4, [[1, 3],
                                  [2, 3],
                                  [2, 4],
                                  [1, 4],
-                                 [['left'], [4, 4]],
-                                 [['left'], [4, 3]]])
-        self.set_equivalent_face(['left'], 6, face)
+                                 left_tile([4, 4]),
+                                 left_tile([4, 3])])
+        self.set_equivalent_face(*left_tile(6), face)
 
         self.add_face(5, [[3, 2],
                           [3, 3],
                           [3, 4],
                           [2, 4],
                           [2, 3],
                           [2, 2]])
 
         face = self.add_face(6, [[5, 4],
                                  [4, 4],
                                  [4, 3],
                                  [5, 3],
-                                 [['right'], [2, 3]],
-                                 [['right'], [2, 4]]])
-        self.set_equivalent_face(['right'], 4, face)
+                                 right_tile([2, 3]),
+                                 right_tile([2, 4])])
+        self.set_equivalent_face(*right_tile(4), face)
 
         self.add_face(7, [[2, 1],
                           [2, 2],
                           [2, 3],
                           [1, 3],
                           [1, 2],
                           [1, 1]])
@@ -147,17 +151,17 @@
                           [2, 1],
                           [3, 1]])
 
         face = self.add_face(10, [[5, 1],
                                   [5, 2],
                                   [4, 2],
                                   [4, 1],
-                                  [['bottom'], [4, 4]],
-                                  [['bottom'], [5, 4]]])
-        self.set_equivalent_face(['bottom'], 3, face)
+                                  bottom_tile([4, 4]),
+                                  bottom_tile([5, 4])])
+        self.set_equivalent_face(*bottom_tile(3), face)
 
     def color_pattern1(self):
         self.color_face(1, 1)
         self.color_face(2, 1)
         self.color_face(7, 1)
         self.color_face(8, 1)
```

### Comparing `tessagon-0.7/tessagon.egg-info/PKG-INFO` & `tessagon-0.8/tessagon.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tessagon
-Version: 0.7
+Version: 0.8
 Summary: Tessellate your favorite 2D manifolds with triangles, hexagons, and other interesting patterns.
 Home-page: https://github.com/cwant/tessagon
 Author: Chris Want
 License: UNKNOWN
 Keywords: tesselation tiling modeling blender vtk
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tessagon-0.7/tessagon.egg-info/SOURCES.txt` & `tessagon-0.8/tessagon.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 LICENSE
 README.md
 setup.py
 tessagon/__init__.py
+tessagon/version.py
 tessagon.egg-info/PKG-INFO
 tessagon.egg-info/SOURCES.txt
 tessagon.egg-info/dependency_links.txt
 tessagon.egg-info/top_level.txt
 tessagon/adaptors/__init__.py
 tessagon/adaptors/blender_adaptor.py
 tessagon/adaptors/list_adaptor.py
 tessagon/adaptors/vtk_adaptor.py
 tessagon/core/__init__.py
 tessagon/core/abstract_tile.py
+tessagon/core/alternating_tile.py
 tessagon/core/grid_tile_generator.py
-tessagon/core/rotate_tile_generator.py
-tessagon/core/stamp14_tessagon.py
+tessagon/core/parallelogram_tile_generator.py
 tessagon/core/tessagon.py
 tessagon/core/tessagon_discovery.py
 tessagon/core/tessagon_metadata.py
 tessagon/core/tile.py
 tessagon/core/tile_generator.py
+tessagon/core/tile_utils.py
 tessagon/core/value_blend.py
 tessagon/misc/__init__.py
 tessagon/misc/shapes.py
 tessagon/types/__init__.py
+tessagon/types/big_hex_tri_tessagon.py
 tessagon/types/brick_tessagon.py
+tessagon/types/cloverdale_tessagon.py
 tessagon/types/dissected_hex_quad_tessagon.py
 tessagon/types/dissected_hex_tri_tessagon.py
 tessagon/types/dissected_square_tessagon.py
 tessagon/types/dissected_triangle_tessagon.py
 tessagon/types/dodeca_tessagon.py
 tessagon/types/dodeca_tri_tessagon.py
 tessagon/types/floret_tessagon.py
 tessagon/types/hex_big_tri_tessagon.py
 tessagon/types/hex_square_tri_tessagon.py
 tessagon/types/hex_tessagon.py
 tessagon/types/hex_tri_tessagon.py
+tessagon/types/islamic_hex_stars_tessagon.py
+tessagon/types/islamic_stars_crosses_tessagon.py
 tessagon/types/octo_tessagon.py
 tessagon/types/penta2_tessagon.py
 tessagon/types/penta_tessagon.py
 tessagon/types/pythagorean_tessagon.py
 tessagon/types/rhombus_tessagon.py
 tessagon/types/square_tessagon.py
 tessagon/types/square_tri2_tessagon.py
 tessagon/types/square_tri_tessagon.py
+tessagon/types/stanley_park_tessagon.py
 tessagon/types/tri_tessagon.py
+tessagon/types/valemount_tessagon.py
 tessagon/types/weave_tessagon.py
 tessagon/types/zig_zag_tessagon.py
```

