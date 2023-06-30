# Comparing `tmp/rod-0.1.dev83.tar.gz` & `tmp/rod-0.1.dev84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rod-0.1.dev83.tar", last modified: Sat Apr 22 17:15:38 2023, max compression
+gzip compressed data, was "rod-0.1.dev84.tar", last modified: Fri Jun 30 10:49:00 2023, max compression
```

## Comparing `rod-0.1.dev83.tar` & `rod-0.1.dev84.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:38.070667 rod-0.1.dev83/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:38.050666 rod-0.1.dev83/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:38.054667 rod-0.1.dev83/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-22 17:15:24.000000 rod-0.1.dev83/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-22 17:15:24.000000 rod-0.1.dev83/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-22 17:15:24.000000 rod-0.1.dev83/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-22 17:15:24.000000 rod-0.1.dev83/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-04-22 17:15:38.070667 rod-0.1.dev83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-22 17:15:24.000000 rod-0.1.dev83/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-22 17:15:24.000000 rod-0.1.dev83/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-22 17:15:38.070667 rod-0.1.dev83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 17:15:24.000000 rod-0.1.dev83/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:38.050666 rod-0.1.dev83/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:38.058667 rod-0.1.dev83/src/rod/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:38.062667 rod-0.1.dev83/src/rod/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/builder/primitive_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/builder/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:38.062667 rod-0.1.dev83/src/rod/kinematics/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/kinematics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/kinematics/kinematic_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/kinematics/tree_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/pretty_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:38.066667 rod-0.1.dev83/src/rod/sdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/physics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/sdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/visual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/sdf/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:38.066667 rod-0.1.dev83/src/rod/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/tree/directed_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/tree/tree_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:38.070667 rod-0.1.dev83/src/rod/urdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/urdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19755 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/urdf/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:38.070667 rod-0.1.dev83/src/rod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/utils/frame_convention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/utils/gazebo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/utils/resolve_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-22 17:15:24.000000 rod-0.1.dev83/src/rod/utils/resolve_uris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:15:38.058667 rod-0.1.dev83/src/rod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-04-22 17:15:38.000000 rod-0.1.dev83/src/rod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-22 17:15:38.000000 rod-0.1.dev83/src/rod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:15:38.000000 rod-0.1.dev83/src/rod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:15:37.000000 rod-0.1.dev83/src/rod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-22 17:15:38.000000 rod-0.1.dev83/src/rod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-22 17:15:38.000000 rod-0.1.dev83/src/rod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:49:00.808334 rod-0.1.dev84/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:49:00.792334 rod-0.1.dev84/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:49:00.796334 rod-0.1.dev84/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-30 10:48:44.000000 rod-0.1.dev84/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-30 10:48:44.000000 rod-0.1.dev84/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-30 10:48:44.000000 rod-0.1.dev84/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-30 10:48:44.000000 rod-0.1.dev84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-06-30 10:49:00.808334 rod-0.1.dev84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-30 10:48:44.000000 rod-0.1.dev84/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-30 10:48:44.000000 rod-0.1.dev84/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-30 10:49:00.808334 rod-0.1.dev84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 10:48:44.000000 rod-0.1.dev84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:49:00.792334 rod-0.1.dev84/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:49:00.796334 rod-0.1.dev84/src/rod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:49:00.800334 rod-0.1.dev84/src/rod/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/builder/primitive_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/builder/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:49:00.800334 rod-0.1.dev84/src/rod/kinematics/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/kinematics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/kinematics/kinematic_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/kinematics/tree_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/pretty_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:49:00.804334 rod-0.1.dev84/src/rod/sdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/physics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/sdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/sdf/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:49:00.804334 rod-0.1.dev84/src/rod/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/tree/directed_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/tree/tree_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:49:00.804334 rod-0.1.dev84/src/rod/urdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/urdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19755 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/urdf/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:49:00.808334 rod-0.1.dev84/src/rod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/utils/frame_convention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/utils/gazebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/utils/resolve_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 10:48:44.000000 rod-0.1.dev84/src/rod/utils/resolve_uris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:49:00.796334 rod-0.1.dev84/src/rod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-06-30 10:49:00.000000 rod-0.1.dev84/src/rod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-30 10:49:00.000000 rod-0.1.dev84/src/rod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:49:00.000000 rod-0.1.dev84/src/rod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:49:00.000000 rod-0.1.dev84/src/rod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-30 10:49:00.000000 rod-0.1.dev84/src/rod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-30 10:49:00.000000 rod-0.1.dev84/src/rod.egg-info/top_level.txt
```

### Comparing `rod-0.1.dev83/.github/workflows/ci_cd.yml` & `rod-0.1.dev84/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/.github/workflows/style.yml` & `rod-0.1.dev84/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/.gitignore` & `rod-0.1.dev84/.gitignore`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/LICENSE` & `rod-0.1.dev84/LICENSE`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/PKG-INFO` & `rod-0.1.dev84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.1.dev83
+Version: 0.1.dev84
 Summary: The ultimate Python tool for RObot Descriptions processing.
 Home-page: https://github.com/ami-iit/rod
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/rod/releases
 Project-URL: Source, https://github.com/ami-iit/rod
```

### Comparing `rod-0.1.dev83/README.md` & `rod-0.1.dev84/README.md`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/setup.cfg` & `rod-0.1.dev84/setup.cfg`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/__init__.py` & `rod-0.1.dev84/src/rod/__init__.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/builder/primitive_builder.py` & `rod-0.1.dev84/src/rod/builder/primitive_builder.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/builder/primitives.py` & `rod-0.1.dev84/src/rod/builder/primitives.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/kinematics/kinematic_tree.py` & `rod-0.1.dev84/src/rod/kinematics/kinematic_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,19 +109,14 @@
             TreeFrame.MODEL: TreeFrame(
                 _source=rod.Frame(
                     name=TreeFrame.MODEL,
                     attached_to=root_node_name,
                     pose=model.pose,
                 ),
             ),
-            model.name: TreeFrame(
-                _source=rod.Frame(
-                    name=model.name, attached_to=root_node_name, pose=model.pose
-                )
-            ),
         }
 
         # Check that links and frames have unique names
         assert len(
             set(list(nodes_links_dict.keys()) + list(nodes_frames_dict.keys()))
         ) == (len(nodes_links_dict) + len(nodes_frames_dict))
```

### Comparing `rod-0.1.dev83/src/rod/kinematics/tree_transforms.py` & `rod-0.1.dev84/src/rod/kinematics/tree_transforms.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/logging.py` & `rod-0.1.dev84/src/rod/logging.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/pretty_printer.py` & `rod-0.1.dev84/src/rod/pretty_printer.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/sdf/common.py` & `rod-0.1.dev84/src/rod/sdf/common.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/sdf/element.py` & `rod-0.1.dev84/src/rod/sdf/element.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/sdf/geometry.py` & `rod-0.1.dev84/src/rod/sdf/geometry.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/sdf/joint.py` & `rod-0.1.dev84/src/rod/sdf/joint.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/sdf/link.py` & `rod-0.1.dev84/src/rod/sdf/link.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/sdf/material.py` & `rod-0.1.dev84/src/rod/sdf/material.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/sdf/model.py` & `rod-0.1.dev84/src/rod/sdf/model.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/sdf/physics.py` & `rod-0.1.dev84/src/rod/sdf/physics.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/sdf/scene.py` & `rod-0.1.dev84/src/rod/sdf/scene.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/sdf/sdf.py` & `rod-0.1.dev84/src/rod/sdf/sdf.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/sdf/world.py` & `rod-0.1.dev84/src/rod/sdf/world.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/tree/directed_tree.py` & `rod-0.1.dev84/src/rod/tree/directed_tree.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/tree/tree_elements.py` & `rod-0.1.dev84/src/rod/tree/tree_elements.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/urdf/exporter.py` & `rod-0.1.dev84/src/rod/urdf/exporter.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/utils/frame_convention.py` & `rod-0.1.dev84/src/rod/utils/frame_convention.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/utils/gazebo.py` & `rod-0.1.dev84/src/rod/utils/gazebo.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/utils/resolve_frames.py` & `rod-0.1.dev84/src/rod/utils/resolve_frames.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod/utils/resolve_uris.py` & `rod-0.1.dev84/src/rod/utils/resolve_uris.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev83/src/rod.egg-info/PKG-INFO` & `rod-0.1.dev84/src/rod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.1.dev83
+Version: 0.1.dev84
 Summary: The ultimate Python tool for RObot Descriptions processing.
 Home-page: https://github.com/ami-iit/rod
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/rod/releases
 Project-URL: Source, https://github.com/ami-iit/rod
```

### Comparing `rod-0.1.dev83/src/rod.egg-info/SOURCES.txt` & `rod-0.1.dev84/src/rod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

