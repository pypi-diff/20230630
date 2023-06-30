# Comparing `tmp/ladybug-vtk-0.8.2.tar.gz` & `tmp/ladybug-vtk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ladybug-vtk-0.8.2.tar", last modified: Fri Feb 18 04:25:59 2022, max compression
+gzip compressed data, was "dist/ladybug-vtk-0.9.0.tar", last modified: Thu Oct 13 20:08:33 2022, max compression
```

## Comparing `ladybug-vtk-0.8.2.tar` & `ladybug-vtk-0.9.0.tar`

### file list

```diff
@@ -1,66 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/docs/_build/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)     3668 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/docs/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    21560 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/ladybug_vtk/
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/_extend_hourly_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/_extend_ladybug_geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     5648 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/_extend_sunpath.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/data_field_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    13018 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/fromgeometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/joined_polydata.py
--rw-r--r--   0 runner    (1001) docker     (121)    23615 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/legend_parameter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     7495 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/model_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     7909 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/polydata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/ladybug_vtk/vtkjs/
--rw-r--r--   0 runner    (1001) docker     (121)     3646 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/vtkjs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10184 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/vtkjs/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3739 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/vtkjs/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/ladybug_vtk/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/ladybug_vtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/ladybug_vtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/ladybug_vtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/ladybug_vtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/ladybug_vtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/ladybug_vtk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/tests/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 04:25:59.000000 ladybug-vtk-0.8.2/tests/assets/weather/
--rw-r--r--   0 runner    (1001) docker     (121)  1642801 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/tests/assets/weather/boston.epw
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     7484 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/tests/fromgeometry_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/tests/hourly_plot_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-02-18 04:24:54.000000 ladybug-vtk-0.8.2/tests/sunpath_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/docs/_build/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     3668 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/docs/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    21560 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/ladybug_vtk/
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/_extend_hourly_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/_extend_ladybug_display.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/_extend_ladybug_display_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/_extend_ladybug_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6251 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/_extend_sunpath.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/_extend_visualization_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8107 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/display_polydata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7047 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/from_display_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14774 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/from_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/fromgeometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/joined_polydata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6591 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/polydata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3430 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/visualization_set.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/ladybug_vtk/vtkjs/
+-rw-r--r--   0 runner    (1001) docker     (121)     3646 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/vtkjs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10184 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/vtkjs/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4058 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/vtkjs/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/ladybug_vtk/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/ladybug_vtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/ladybug_vtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/ladybug_vtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/ladybug_vtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/ladybug_vtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/ladybug_vtk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (121)  3037717 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/tests/assets/visualization.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 20:08:33.000000 ladybug-vtk-0.9.0/tests/assets/weather/
+-rw-r--r--   0 runner    (1001) docker     (121)  1642801 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/tests/assets/weather/boston.epw
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7474 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/tests/from_geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/tests/hourly_plot_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/tests/sunpath_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2022-10-13 20:07:14.000000 ladybug-vtk-0.9.0/tests/visualization_test.py
```

### Comparing `ladybug-vtk-0.8.2/.github/workflows/ci.yaml` & `ladybug-vtk-0.9.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ladybug-vtk-0.8.2/.github/workflows/dependency-release.yaml` & `ladybug-vtk-0.9.0/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `ladybug-vtk-0.8.2/LICENSE` & `ladybug-vtk-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ladybug-vtk-0.8.2/PKG-INFO` & `ladybug-vtk-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-vtk
-Version: 0.8.2
+Version: 0.9.0
 Summary: Provides methods for translating ladybug-geometry objects to VTK PolyData.
 Home-page: https://github.com/ladybug-tools/ladybug-vtk
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ladybug-vtk-0.8.2/README.md` & `ladybug-vtk-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ladybug-vtk-0.8.2/docs/_static/custom.css` & `ladybug-vtk-0.9.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ladybug-vtk-0.8.2/docs/_templates/layout.html` & `ladybug-vtk-0.9.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ladybug-vtk-0.8.2/docs/conf.py` & `ladybug-vtk-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ladybug-vtk-0.8.2/ladybug_vtk/_extend_hourly_plot.py` & `ladybug-vtk-0.9.0/ladybug_vtk/_extend_hourly_plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pathlib import Path
 from ladybug.hourlyplot import HourlyPlot
 from ladybug_geometry.geometry3d import Vector3D
 from ladybug.color import Color
-from .fromgeometry import from_line3d, from_polyline3d, from_mesh3d, to_text
-from .model_dataset import ModelDataSet
-from .model import Model
+
+from ladybug_vtk.vtkjs.schema import DisplayMode
+from .from_geometry import to_text
+from .display_polydata import DisplayPolyData
+from .visualization_set import VisualizationSet
 
 
 def hourly_plot_to_vtkjs(self, output_folder: str, file_name: str = 'hourly plot') -> Path:
     """
     Export the HourlyPlot to a vtkjs file.
 
     Args:
@@ -30,50 +32,58 @@
     # month lines
     month_lines3d_polydata = [line.to_polydata() for line in self.month_lines3d]
     lines.extend(month_lines3d_polydata)
 
     # border polyline
     border_polydata = self.chart_border3d.to_polydata()
     lines.append(border_polydata)
-    datasets.append(ModelDataSet('lines', lines, color=Color()))
+    datasets.append(DisplayPolyData('Hourly Plot::Lines', 'lines', polydata=lines, color=Color()))
 
-    # lalbels
+    # labels
     labels = []
-    left_vector = Vector3D(-1, 0, 0)*5
-    down_vector = Vector3D(0, -1, 0)*3
+    left_vector = Vector3D(-1, 0, 0) * 5
+    down_vector = Vector3D(0, -1, 0) * 3
 
     # month labels
     month_labels_polydata = [
         to_text(label, self.month_label_points3d[count].
                 move(left_vector).move(down_vector), scale=4)
         for count, label in enumerate(self.month_labels)]
     labels.extend(month_labels_polydata)
 
     # hour labels
-    hour_left_vector = Vector3D(-1, 0, 0)*15
+    hour_left_vector = Vector3D(-1, 0, 0) * 15
     hour_labels_polydata = [
         to_text(label, self.hour_label_points3d[count].
                 move(hour_left_vector).move(down_vector), scale=4)
         for count, label in enumerate(self.hour_labels)]
     labels.extend(hour_labels_polydata)
 
     # title text
     title_polydata = to_text(self.title_text, self.lower_title_location.o.move(
         left_vector).move(down_vector), scale=4)
     labels.append(title_polydata)
-    datasets.append(ModelDataSet('labels', labels, color=Color()))
+    datasets.append(DisplayPolyData('Hourly Plot::Labels', 'labels', polydata=labels, color=Color()))
 
     # data
     mesh_polydata = self.colored_mesh3d.to_polydata()
-    mesh_dataset = ModelDataSet('data', [mesh_polydata])
     name = self.data_collection.header.data_type.name
-    mesh_dataset.add_data_fields([self.data_collection], name)
+    mesh_polydata.add_data(
+        self.data_collection.values, name=name, per_face=True,
+        data_type=self.data_collection.header.data_type,
+        unit=self.data_collection.header.unit
+    )
+
+    mesh_dataset = DisplayPolyData(
+        name='Data', identifier='data', polydata=[mesh_polydata],
+        display_mode=DisplayMode.SurfaceWithEdges
+    )
     mesh_dataset.color_by = name
     datasets.append(mesh_dataset)
 
     # write all datasets to a vtkjs file
-    hourly_plot = Model(datasets=datasets)
+    hourly_plot = VisualizationSet(datasets=datasets)
 
     return Path(hourly_plot.to_vtkjs(output_folder, file_name))
 
 
 HourlyPlot.to_vtkjs = hourly_plot_to_vtkjs
```

### Comparing `ladybug-vtk-0.8.2/ladybug_vtk/_extend_ladybug_geometry.py` & `ladybug-vtk-0.9.0/ladybug_vtk/_extend_ladybug_geometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Add capability to turn a Ladybug geometry object into a VTK polydata object."""
 
-from ladybug_geometry.geometry2d import Point2D, LineSegment2D, Polyline2D
+from ladybug_geometry.geometry2d import Point2D, LineSegment2D, Polyline2D, Mesh2D
 from ladybug_geometry.geometry3d import Point3D, LineSegment3D, Polyline3D, Arc3D, \
     Mesh3D, Face3D, Polyface3D, Cone, Sphere, Cylinder
-from .fromgeometry import from_line2d, from_point2d, from_point3d, from_line3d, \
-    from_polyline3d, from_arc3d, from_mesh3d, from_face3d, from_polyface3d, from_cone,\
+from .from_geometry import from_line2d, from_point2d, from_point3d, from_line3d, \
+    from_polyline3d, from_arc3d, from_mesh3d, from_mesh2d, from_face3d, from_polyface3d, from_cone,\
     from_sphere, from_cylinder, from_polyline2d
 
 # 2d goemetry
 Point2D.to_polydata = from_point2d
 LineSegment2D.to_polydata = from_line2d
 Polyline2D.to_polydata = from_polyline2d
 
 # 3d geometry
 Point3D.to_polydata = from_point3d
 LineSegment3D.to_polydata = from_line3d
 Polyline3D.to_polydata = from_polyline3d
 Arc3D.to_polydata = from_arc3d
 Mesh3D.to_polydata = from_mesh3d
+Mesh2D.to_polydata = from_mesh2d
 Face3D.to_polydata = from_face3d
 Polyface3D.to_polydata = from_polyface3d
 Cone.to_polydata = from_cone
 Sphere.to_polydata = from_sphere
 Cylinder.to_polydata = from_cylinder
```

### Comparing `ladybug-vtk-0.8.2/ladybug_vtk/_extend_sunpath.py` & `ladybug-vtk-0.9.0/ladybug_vtk/_extend_sunpath.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from ladybug.color import Color
 from ladybug_geometry.geometry3d import Point3D
 from ladybug_geometry.geometry2d import Vector2D, Point2D
 from ladybug.sunpath import Sunpath
 from ladybug.compass import Compass
 from ladybug.datacollection import HourlyContinuousCollection
 
-from .fromgeometry import from_points3d, to_circle, to_text, from_points2d
-from .model_dataset import ModelDataSet
-from .model import Model
+from .from_geometry import from_points3d, to_circle, to_text, from_points2d
+from .display_polydata import DisplayPolyData
+from .visualization_set import VisualizationSet
 
 
-def sunpath_to_vtkjs(self, output_folder: str = '.', file_name: str = 'sunpath', radius: int = 100,
-                     data: List[HourlyContinuousCollection] = None,
-                     sun_color: Color = Color(252, 177, 3), make_2d: bool = False) -> Path:
+def sunpath_to_vtkjs(
+    self, output_folder: str = '.', file_name: str = 'sunpath', radius: int = 100,
+    data: List[HourlyContinuousCollection] = None, sun_color: Color = Color(252, 177, 3),
+        make_2d: bool = False) -> Path:
     """Export sunpath as a vtkjs file.
 
     Args:
         output_folder: Path to the target folder to write the vtkjs file. Defaults to
             current working directory.
         file_name: Output file name. Defaults to Sunpath.
         radius: Radius of the sunpath. Defaults to 100.
@@ -41,64 +42,77 @@
 
     if not make_2d:
         polylines = self.hourly_analemma_polyline3d(radius=radius)
         sp_polydata = [pl.to_polydata() for pl in polylines]
     else:
         polylines = self.hourly_analemma_polyline2d(radius=radius)
         sp_polydata = [pl.to_polydata() for pl in polylines]
-    sp_dataset = ModelDataSet(name='hourly_analemmas', data=sp_polydata, color=Color())
+    sp_dataset = DisplayPolyData(
+        name='Sun path::Hourly Analemmas', identifier='hourly_analemmas',
+        polydata=sp_polydata, color=Color()
+    )
     datasets.append(sp_dataset)
 
     # monthly arcs
     if not make_2d:
         arcs = self.monthly_day_arc3d(radius=radius)
         monthly_polydata = [arc.to_polydata(resolution=100) for arc in arcs]
     else:
         polylines = self.monthly_day_polyline2d(radius=radius)
         monthly_polydata = [polyline.to_polydata() for polyline in polylines]
-    arc_dataset = ModelDataSet(name='monthly_arcs', data=monthly_polydata, color=Color())
+    arc_dataset = DisplayPolyData(
+        name='Sun path::Monthly Arcs', identifier='monthly_arcs',
+        polydata=monthly_polydata, color=Color()
+    )
     datasets.append(arc_dataset)
 
     # compass circles
     offset_1 = (radius*1.5)/100
     offset_2 = (radius*4.5)/100
     rads = [radius, radius+offset_1, radius+offset_2]
     base_polydata = [to_circle(origin, radius) for radius in rads]
 
     # compass ticks
     compass = Compass(radius=radius, north_angle=self.north_angle)
     ticks_major = compass.ticks_from_angles(angles=compass.MAJOR_AZIMUTHS, factor=0.55)
     ticks_minor = compass.ticks_from_angles(angles=compass.MINOR_AZIMUTHS)
     ticks_polydata = [tick.to_polydata() for tick in ticks_major+ticks_minor]
     base_polydata.extend(ticks_polydata)
-    base_dataset = ModelDataSet(name='base_circle', data=base_polydata, color=Color())
+    base_dataset = DisplayPolyData(
+        name='Sun path::Compass', identifier='base_circle',
+        polydata=base_polydata, color=Color()
+    )
     datasets.append(base_dataset)
 
     # Since vtkVectorText starts from left bottom we need to move the labels to the left
     # and down by a certain amount.
     moving_factor = (radius*3)/100
     left_vector = Vector2D(-1, 0)*moving_factor
     down_vector = Vector2D(0, -1)*moving_factor
 
     # compass minor labels
     minor_scale = (radius*2)/100
     minor_text_polydata = [to_text(text, compass.minor_azimuth_points[count].
                                    move(left_vector).move(down_vector), minor_scale)
                            for count, text in enumerate(compass.MINOR_TEXT)]
-    minor_label_dataset = ModelDataSet(
-        name='minor_labels', data=minor_text_polydata, color=Color())
+    minor_label_dataset = DisplayPolyData(
+        name='Sun path::Minor Labels', identifier='minor_labels',
+        polydata=minor_text_polydata, color=Color()
+    )
     datasets.append(minor_label_dataset)
 
     # compass major labels
     major_scale = (radius*5)/100
     major_text_polydata = [to_text(text, compass.major_azimuth_points[count].
                                    move(left_vector).move(down_vector), scale=major_scale) for
                            count, text in enumerate(compass.MAJOR_TEXT)]
-    major_label_dataset = ModelDataSet(
-        name='major_labels', data=major_text_polydata, color=Color())
+    major_label_dataset = DisplayPolyData(
+        name='Sun path::Major Labels', identifier='major_labels',
+        polydata=major_text_polydata, color=Color()
+    )
     datasets.append(major_label_dataset)
 
     # add suns
     day = self.hourly_analemma_suns(daytime_only=True)
 
     # calculate sun positions from sun vector
     pts = []
@@ -111,30 +125,38 @@
                 pts.append(origin.move(sun.sun_vector.reverse() * radius))
             hours.append(sun.hoy)
 
     if not make_2d:
         sun_positions = from_points3d(pts)
     else:
         sun_positions = from_points2d(pts)
-    sun_dataset = ModelDataSet(name='suns', data=[sun_positions])
+    sun_dataset = DisplayPolyData(
+        name='data', identifier='data', polydata=[sun_positions]
+    )
 
     # Load data if provided
     if data:
         for dt in data:
             assert isinstance(dt, HourlyContinuousCollection), 'Data needs to be a'\
                 f' Ladybug HourlyContinuousCollection object. Instead got {type(dt)}'
             filtered_data = dt.filter_by_hoys(hours)
             name = filtered_data.header.data_type.name
-            sun_dataset.add_data_fields([filtered_data], name, per_face=False)
+            for data in sun_dataset.polydata:
+                data.add_data(
+                    filtered_data.values, name=name, per_face=False,
+                    data_type=filtered_data.header.data_type,
+                    unit=filtered_data.header.unit
+                )
             sun_dataset.color_by = name
         datasets.append(sun_dataset)
     else:
-        sun_dataset = ModelDataSet(
-            name='suns', data=[sun_positions], color=sun_color)
+        sun_dataset = DisplayPolyData(
+            name='Suns', identifier='suns',
+            polydata=[sun_positions], color=sun_color)
         datasets.append(sun_dataset)
 
     # join polylines into a single polydata
-    sunpath = Model(datasets=datasets)
+    sunpath = VisualizationSet(datasets=datasets)
     return Path(sunpath.to_vtkjs(output_folder, file_name))
 
 
 Sunpath.to_vtkjs = sunpath_to_vtkjs
```

### Comparing `ladybug-vtk-0.8.2/ladybug_vtk/fromgeometry.py` & `ladybug-vtk-0.9.0/ladybug_vtk/from_geometry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Functions to translate ladybug geometry objects into VTK polydata objects."""
 
 
 import vtk
 import math
 from typing import List, Union
-from ladybug_geometry.geometry2d import Point2D, LineSegment2D, Polyline2D
+from ladybug_geometry.geometry2d import Point2D, LineSegment2D, Polyline2D, Mesh2D
 from ladybug_geometry.geometry3d import Point3D, Polyline3D, Arc3D, LineSegment3D,\
     Mesh3D, Polyface3D, Cone, Cylinder, Sphere, Face3D
 from .polydata import PolyData
 
 
 def from_point2d(point: Point2D) -> PolyData:
     """Create Polydata from a Ladybug Point2D object.
@@ -274,14 +274,43 @@
     polydata = PolyData()
     polydata.SetPoints(points)
     polydata.SetPolys(cells)
 
     return polydata
 
 
+def from_mesh2d(mesh: Mesh2D) -> PolyData:
+    """Create Polydata from a Ladybug mesh 2D.
+
+    Args:
+        mesh: A Ladybug Mesh2D object.
+
+    Returns:
+        Polydata containing face and points of a mesh.
+    """
+    points = vtk.vtkPoints()
+    polygon = vtk.vtkPolygon()
+    cells = vtk.vtkCellArray()
+
+    for ver in mesh.vertices:
+        points.InsertNextPoint(ver[0], ver[1], 0)
+
+    for face in mesh.faces:
+        polygon.GetPointIds().SetNumberOfIds(len(face))
+        for count, i in enumerate(face):
+            polygon.GetPointIds().SetId(count, i)
+        cells.InsertNextCell(polygon)
+
+    polydata = PolyData()
+    polydata.SetPoints(points)
+    polydata.SetPolys(cells)
+
+    return polydata
+
+
 def from_face3d(face: Face3D) -> PolyData:
     """Create Polydata from a Ladybug face.
 
     Args:
         face: A Ladybug Face3D object.
 
     Returns:
@@ -306,24 +335,53 @@
     polydata = PolyData()
     polydata.SetPoints(points)
     polydata.SetPolys(cells)
 
     return polydata
 
 
-def from_polyface3d(polyface: Polyface3D) -> List[PolyData]:
+def from_polyface3d(polyface: Polyface3D) -> PolyData:
     """Create Polydata from a Ladybug Polyface.
 
     Args:
         polyface: A Ladybug Polyface3D object.
 
     Returns:
         A list of Polydata. Each polydata contains a face and points of a face of Polyface.
     """
-    return [from_face3d(face) for face in polyface.faces]
+    points = vtk.vtkPoints()
+    polygon = vtk.vtkPolygon()
+    cells = vtk.vtkCellArray()
+
+    for ver in polyface.vertices:
+        points.InsertNextPoint(*ver)
+
+    for face, face_geo in zip(polyface.face_indices, polyface.faces):
+        if face_geo.has_holes or not face_geo.is_convex:
+            meshed_face = face_geo.triangulated_mesh3d
+            for ver in meshed_face.vertices:
+                if ver not in polyface.vertices:
+                    points.InsertNextPoint(*ver)
+            for face in meshed_face.faces:
+                polygon.GetPointIds().SetNumberOfIds(len(face))
+                for count, i in enumerate(face):
+                    polygon.GetPointIds().SetId(count, i)
+                cells.InsertNextCell(polygon)
+        else:
+            face = face[0]
+            polygon.GetPointIds().SetNumberOfIds(len(face))
+            for count, i in enumerate(face):
+                polygon.GetPointIds().SetId(count, i)
+            cells.InsertNextCell(polygon)
+
+    polydata = PolyData()
+    polydata.SetPoints(points)
+    polydata.SetPolys(cells)
+
+    return polydata
 
 
 def from_cone(cone: Cone, resolution: int = 2, cap: bool = True) -> PolyData:
     """Create Polydata from a Ladybug Cone.
 
     Args:
         cone: A Ladybug Cone object.
```

### Comparing `ladybug-vtk-0.8.2/ladybug_vtk/joined_polydata.py` & `ladybug-vtk-0.9.0/ladybug_vtk/joined_polydata.py`

 * *Files identical despite different names*

### Comparing `ladybug-vtk-0.8.2/ladybug_vtk/model_dataset.py` & `ladybug-vtk-0.9.0/ladybug_vtk/display_polydata.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,218 +1,234 @@
-"""ModelDataSet object to control the representation of a Polydata object."""
+"""DisplayPolyData object to control the representation of a Polydata object."""
 
 import pathlib
-from typing import List
-from .polydata import PolyData
-from .data_field_info import DataFieldInfo
+import uuid
+from typing import List, Union
+
 from ladybug.color import Color
-from .vtkjs.schema import DataSetProperty, DataSet, DisplayMode, DataSetMapper
+from ladybug_display.visualization import AnalysisGeometry, ContextGeometry
+
+from .polydata import PolyData
 from .joined_polydata import JoinedPolyData
+from .vtkjs.schema import DataSetProperty, DataSet, DisplayMode, DataSetMapper
 
 
-class ModelDataSet:
-    """A dataset object in honeybee VTK model.
+display_mode_mapper = {
+    'Surface': DisplayMode.Surface,
+    'SurfaceWithEdges': DisplayMode.SurfaceWithEdges,
+    'Wireframe': DisplayMode.Wireframe,
+    'Points': DisplayMode.Points
+}
+
+
+class DisplayPolyData:
+    """A collection of PolyData with display attributes.
+
+    All the PolyData must have data with the same names attached to them.
+
+    This object is similar to an AnalysisGeometry object in ladybug-display.
+
+    Args:
+        name: A display name.
+        identifier: A unique identifier for this DisplayPolyData. This identifier should
+            be unique among all the DisplayPolyData in a VisualizationSet.
+        polydata: A list of PolyData objects.
+        color: A Ladybug color to set the diffuse color for DisplayPolyData to use when
+            there is no data available.
+        display_mode: Display model. It can be set to Surface, SurfaceWithEdges,
+            Wireframe and Points.
 
-    This data set holds the PolyData objects as well as representation information
-    for those PolyData. All the objects in ModelDataSet will have the same
-    representation.
     """
 
-    def __init__(self, name, data: List[PolyData] = None, color: Color = None) -> None:
+    def __init__(
+        self, name: str, identifier: str, * , polydata: List[PolyData] = None,
+        color: Color = None, display_mode: DisplayMode =  DisplayMode.Surface
+            ) -> None:
         self.name = name
-        self.data = data or []
-        self.color = color
-        self.display_mode = DisplayMode.Shaded
-        self.color_by = None
-
-    @ property
-    def fields_info(self) -> dict:
-        return {} if not self.data else self.data[0]._fields
-
-    @ property
-    def active_field_info(self) -> DataFieldInfo:
-        """Get information for active field info.
-
-        It will be the field info for the field that is set in color_by. If color_by
-        is not set the first field will be used. If no field is available a default
-        field will be generated.
-
-        """
-        info = self.fields_info
-        color_by = self.color_by
-        if not info:
-            return DataFieldInfo()
-        if not color_by:
-            return next(iter(info.values()))
-        return info[color_by]
-
-    def add_data_fields(
-        self, data: List[List], name: str, per_face: bool = True, colors=None,
-            data_range=None):
-        """Add data fields to PolyData objects in this dataset.
-
-        Use this method to add data like temperature or illuminance values to PolyData
-        objects. The length of the input data should match the length of the data in
-        DataSet.
-
-        Args:
-            data: A list of list of values. There should be a list per data in DataSet.
-                The order of data should match the order of data in DataSet. You can
-                use data.identifier to match the orders before assigning them to DataSet.
-            name: Name of data (e.g. Useful Daylight Autonomy.)
-            per_face: A Boolean to indicate if the data is per face or per point. In
-                most cases except for sensor points that are loaded as sensors the data
-                are provided per face.
-            colors: A Colors object that defines colors for the legend.
-            data_range: A list with two values for minimum and maximum values for legend
-                parameters.
-        """
+        self.identifier = identifier or str(uuid.uuid4())
+        self.polydata = polydata or []
+        self.color = color or Color(204, 204, 204, 255)
+        self.display_mode = display_mode
+
+    @classmethod
+    def from_visualization_geometry(
+        cls, geometry: Union[AnalysisGeometry, ContextGeometry]
+            ) -> 'DisplayPolyData':
+
+        poly_datas: List[PolyData] = [
+            geometry.to_polydata() for geometry in geometry.geometry
+        ]
+        if isinstance(geometry, AnalysisGeometry):
+            mapping = geometry.matching_method
+            for count, data_set in enumerate(geometry.data_sets):
+                # try to get the name for dataset
+                if data_set.data_type:
+                    ds_name = data_set.data_type.name
+                else:
+                    ds_name = 'untitled'
+
+                if mapping == 'geometry':
+                    # TODO: support per object coloring
+                    # to support this case we need to get the number of faces/cells in PolyData
+                    # and duplicate the values to match the number of cells. PolyData should have
+                    # a method that returns the number of cells. We just need to expose it.
+                    raise NotImplementedError(
+                        'Mapping data per object is not currently supported.'
+                    )
+                # add this dataset to polydatas
+                for poly_data in poly_datas:
+                    poly_data.add_visualization_data(data_set, matching_method=mapping)
+                if count == geometry.active_data:
+                    color_by = ds_name
+
+            vtk_data_set = DisplayPolyData(
+                name=geometry.display_name, identifier=geometry.identifier,
+                polydata=poly_datas,
+                display_mode=display_mode_mapper[geometry.display_mode]
+            )
+            vtk_data_set.color_by = color_by
+        else:
+            # context geometry
+            # the assumption is that all the geometries under the same context geometry
+            # have the same display mode and color. We pick the first item.
+            try:
+                display_mode = geometry.geometry[0].display_mode
+                display_mode = display_mode_mapper[geometry.display_mode]
+            except AttributeError:
+                display_mode = DisplayMode.Wireframe
+            try:
+                color = geometry.geometry[0].color
+            except AttributeError:
+                color = None
+
+            vtk_data_set = DisplayPolyData(
+                name=geometry.display_name, identifier=geometry.identifier,
+                polydata=poly_datas,
+                display_mode=display_mode, color=color
+            )
 
-        assert len(self.data) == len(data), \
-            f'Length of input data {len(data)} does not match the length of'\
-            f' {name} in this dataset {len(self.data)}.'
-
-        for count, d in enumerate(data):
-            self.data[count].add_data(
-                d, name=name, cell=per_face, colors=colors, data_range=data_range)
+        return vtk_data_set
 
-    @ property
+    @property
     def is_empty(self):
-        return len(self.data) == 0
+        return len(self.polydata) == 0
 
-    @ property
+    @property
     def color(self) -> Color:
         """Diffuse color.
 
         By default the dataset will be colored by this color unless color_by property
         is set to a dataset value.
         """
         return self._color
 
-    @ color.setter
+    @color.setter
     def color(self, value: Color):
         self._color = value if value else Color(204, 204, 204, 255)
 
-    @ property
+    @property
     def color_by(self) -> str:
-        """Set the field that the DataSet should colored-by when exported to vtkjs.
+        """Gat and set the field that the DataSet should colored-by when exported to vtkjs.
 
-        By default the dataset will be colored by surface color and not data fields.
+        By default the dataset will be colored by surface color and not data.
         """
-        return self._color_by
+        return self.polydata[0].color_by
 
-    @ color_by.setter
+    @color_by.setter
     def color_by(self, value: str):
-        fields_info = self.fields_info
-        if not value:
-            self._color_by = None
-            return
-        else:
-            assert value in fields_info, \
-                f'{value} is not a valid data field for this ModelDataSet. Available ' \
-                f'data fields are: {list(fields_info.keys())}'
+        for data in self.polydata:
+            data.color_by = value
 
-        for data in self.data:
-            data.color_by(value, fields_info[value].per_face)
-
-        self._color_by = value
-
-    @ property
+    @property
     def opacity(self) -> float:
-        """Visualization opacity."""
+        """Get and set the visualization opacity."""
         return self.color.a
 
-    @ property
+    @opacity.setter
+    def opacity(self, value):
+        color = self.color.duplicate()
+        color.a = value
+
+    @property
     def display_mode(self) -> DisplayMode:
         """Display model (AKA Representation) mode in VTK Glance viewer.
 
         Valid values are:
-            * Surface / Shaded
+            * Surface
             * SurfaceWithEdges
             * Wireframe
             * Points
 
         Default is 0 for Surface mode.
 
         """
         return self._display_mode
 
-    @ display_mode.setter
+    @display_mode.setter
     def display_mode(self, mode: DisplayMode = DisplayMode.Surface):
         self._display_mode = mode
 
-    @ property
+    @property
     def edge_visibility(self) -> bool:
         """Edge visibility.
 
         The edges will be visible in Wireframe or SurfaceWithEdges modes.
         """
         if self.display_mode.value in (0, 2):
             return False
         else:
             return True
 
-    def rgb_to_decimal(self):
-        """RGB color in decimal."""
-        return (self.color[0] / 255, self.color[1] / 255, self.color[2] / 255)
-
     def to_folder(self, folder, sub_folder=None) -> str:
         """Write data information to a folder.
 
         Args:
             folder: Target folder to write the dataset.
             sub_folder: Subfolder name for this dataset. By default it will be set to
                 the name of the dataset.
         """
-        sub_folder = sub_folder or self.name
+        sub_folder = sub_folder or self.identifier
         target_folder = pathlib.Path(folder, sub_folder)
 
-        if len(self.data) == 0:
-            print(f'ModelDataSet: {self.name} has no data to be exported to folder.')
+        if len(self.polydata) == 0:
             return
-        elif len(self.data) == 1:
-            data = self.data[0]
+        elif len(self.polydata) == 1:
+            data = self.polydata[0]
         else:
-            data = JoinedPolyData.from_polydata(self.data)
+            data = JoinedPolyData.from_polydata(self.polydata)
         return data.to_folder(target_folder.as_posix())
 
-    def as_data_set(self, url=None) -> DataSet:
-        """Convert to a vtkjs DataSet object.
-
-        Args:
-            url: Relative path to where PolyData information should be sourced from.
-                By default url will be set to ModelDataSet name assuming data is dumped
-                to a folder with the same name.
-
-        """
+    def to_vtk_dataset(self) -> DataSet:
+        """Convert to a vtkjs DataSet object."""
         prop = {
             'representation': min(self.display_mode.value, 2),
             'edgeVisibility': int(self.edge_visibility),
             'diffuseColor': [self.color.r / 255, self.color.g / 255, self.color.b / 255],
             'opacity': self.opacity / 255
         }
 
         ds_prop = DataSetProperty.parse_obj(prop)
 
         mapper = DataSetMapper()
         if self.color_by is not None:
             mapper.colorByArrayName = self.color_by
 
-        # Getting legend information for each data added to the ModelDataSet object.
-        legends = []
-        if self.name == 'Grid' and self.fields_info:
-            for field_info in self.fields_info.values():
-                legends.append(field_info.legend_parameter._to_dict())
+        # Collect meta data for each data attached to polydata. Since all the polydata
+        # in a DisplayPolyData most have the same metadata we pick the first one
+        metadata = [
+            metadata.to_vtk_metadata().dict()
+            for metadata in self.polydata[0].data.values()
+        ]
 
         data = {
             'name': self.name,
-            'httpDataSetReader': {'url': url if url is not None else self.name},
+            'httpDataSetReader': {'url': self.identifier},
             'property': ds_prop.dict(),
             'mapper': mapper.dict(),
-            'legends': legends
+            'metadata': metadata
         }
 
         return DataSet.parse_obj(data)
 
     def __repr__(self) -> str:
-        return f'ModelDataSet: {self.name}' \
-            f'\n  DataSets: {len(self.data)}\n  Color:{self.color}'
+        return f'DisplayPolyData: {self.name}' \
+            f'\n  DataSets: #{len(self.polydata)}\n  Color: {self.color}'
```

### Comparing `ladybug-vtk-0.8.2/ladybug_vtk/vtkjs/__init__.py` & `ladybug-vtk-0.9.0/ladybug_vtk/vtkjs/__init__.py`

 * *Files identical despite different names*

### Comparing `ladybug-vtk-0.8.2/ladybug_vtk/vtkjs/helper.py` & `ladybug-vtk-0.9.0/ladybug_vtk/vtkjs/helper.py`

 * *Files identical despite different names*

### Comparing `ladybug-vtk-0.8.2/ladybug_vtk/vtkjs/schema.py` & `ladybug-vtk-0.9.0/ladybug_vtk/vtkjs/schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 """Schema for VTKJS objects."""
 import json
 import pathlib
-from typing import Dict, List, Tuple
+from typing import Dict, List, Union
 import enum
 
 from pydantic import BaseModel, Field, validator
-
+from ladybug_display_schema.visualization import LegendParameters, DataType, GenericDataType
 
 class DisplayMode(enum.Enum):
     """Display mode."""
-    Shaded = 2
     Surface = 2
     SurfaceWithEdges = 3
     Wireframe = 1
     Points = 0
 
 
-class SensorGridOptions(enum.Enum):
-    """Settings for loading sensor grids."""
-    Ignore = 0  # no loading
-    Sensors = 1  # load them as sensor points
-    Mesh = 2  # load them as mesh
-
-
 class Camera(BaseModel):
     """Camera in vtkjs viewer."""
     focalPoint: List[float] = Field(
         [2.5, 5, 1.5],
         description='Camera focal point.', max_items=3, min_items=3
     )
     position: List[float] = Field(
@@ -66,30 +58,42 @@
         [0.8, 0.8, 0.8],
         description='Surface color.', max_items=3, min_items=3
     )
     pointSize: int = Field(5)
     opacity: float = Field(1)
 
 
+class DataSetMetaData(BaseModel):
+    legend_parameters: LegendParameters = Field(None, description='Legend Parameters.')
+    unit: str = Field('', description='Unit as a string')
+    data_type: Union[DataType, GenericDataType] = Field(
+        GenericDataType(name='', base_unit=''),
+        description='Data type for data set.'
+    )
+
+
 class DataSet(BaseModel):
     """A VTKJS dataset."""
     name: str = Field(..., description='DataSet name.')
     type: str = Field('httpDataSetReader')  # I don't know enough about this field!
     httpDataSetReader: DataSetResource = Field(...)
     actor: DataSetActor = Field(DataSetActor())
     actorRotation: List[float] = Field(
         [0, 0, 0, 1],
         description='Actor rotation axis.', max_items=4, min_items=4
     )
     mapper: DataSetMapper = Field(DataSetMapper())
     property: DataSetProperty = Field(DataSetProperty())
     legends: List[dict] = Field(
+        [], deprecated=True,
+        description='This field is deprecated. Use the metadata field instead.'
+    )
+    metadata: List[DataSetMetaData] = Field(
         [],
-        description='A list of dictionaries representing legend information for the'
-        ' data added to the Dataset object.'
+        description='List of metadata objects for each dataset.'
     )
 
 
 class IndexJSON(BaseModel):
     """VTKJS index class.
 
     These information will be translated to an index.json file.
```

### Comparing `ladybug-vtk-0.8.2/ladybug_vtk/writer.py` & `ladybug-vtk-0.9.0/ladybug_vtk/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,18 @@
 def write_to_folder(polydata: Union[vtk.vtkPolyData, vtk.vtkAppendPolyData],
                     target_folder: str):
     """Write PolyData to a folder using vtkJSONDataSetWriter."""
 
     writer = vtk.vtkJSONDataSetWriter()
     folder = pathlib.Path(target_folder)
     folder.mkdir(parents=True, exist_ok=True)
-    writer.SetFileName(folder.as_posix())
+    try:
+        writer.SetFileName(folder.as_posix())
+    except:
+        writer.SetArchiveName(folder.as_posix())
 
     if isinstance(polydata, vtk.vtkPolyData):
         writer.SetInputData(polydata)
     else:
         writer.SetInputConnection(polydata.GetOutputPort())
     writer.Write()
     return folder.as_posix()
```

### Comparing `ladybug-vtk-0.8.2/ladybug_vtk.egg-info/PKG-INFO` & `ladybug-vtk-0.9.0/ladybug_vtk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-vtk
-Version: 0.8.2
+Version: 0.9.0
 Summary: Provides methods for translating ladybug-geometry objects to VTK PolyData.
 Home-page: https://github.com/ladybug-tools/ladybug-vtk
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ladybug-vtk-0.8.2/ladybug_vtk.egg-info/SOURCES.txt` & `ladybug-vtk-0.9.0/ladybug_vtk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,32 +19,37 @@
 docs/_build/README.md
 docs/_build/docs/README.md
 docs/_static/custom.css
 docs/_templates/layout.html
 docs/cli/index.rst
 ladybug_vtk/__init__.py
 ladybug_vtk/_extend_hourly_plot.py
+ladybug_vtk/_extend_ladybug_display.py
+ladybug_vtk/_extend_ladybug_display_schema.py
 ladybug_vtk/_extend_ladybug_geometry.py
 ladybug_vtk/_extend_sunpath.py
-ladybug_vtk/_helper.py
-ladybug_vtk/data_field_info.py
+ladybug_vtk/_extend_visualization_set.py
+ladybug_vtk/display_polydata.py
+ladybug_vtk/from_display_geometry.py
+ladybug_vtk/from_geometry.py
 ladybug_vtk/fromgeometry.py
 ladybug_vtk/joined_polydata.py
-ladybug_vtk/legend_parameter.py
-ladybug_vtk/model.py
-ladybug_vtk/model_dataset.py
+ladybug_vtk/metadata.py
 ladybug_vtk/polydata.py
+ladybug_vtk/visualization_set.py
 ladybug_vtk/writer.py
 ladybug_vtk.egg-info/PKG-INFO
 ladybug_vtk.egg-info/SOURCES.txt
 ladybug_vtk.egg-info/dependency_links.txt
 ladybug_vtk.egg-info/requires.txt
 ladybug_vtk.egg-info/top_level.txt
 ladybug_vtk/vtkjs/__init__.py
 ladybug_vtk/vtkjs/helper.py
 ladybug_vtk/vtkjs/schema.py
 tests/__init__.py
 tests/conftest.py
-tests/fromgeometry_test.py
+tests/from_geometry_test.py
 tests/hourly_plot_test.py
 tests/sunpath_test.py
+tests/visualization_test.py
+tests/assets/visualization.json
 tests/assets/weather/boston.epw
```

### Comparing `ladybug-vtk-0.8.2/setup.py` & `ladybug-vtk-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ladybug-vtk-0.8.2/tests/assets/weather/boston.epw` & `ladybug-vtk-0.9.0/tests/assets/weather/boston.epw`

 * *Files identical despite different names*

### Comparing `ladybug-vtk-0.8.2/tests/fromgeometry_test.py` & `ladybug-vtk-0.9.0/tests/from_geometry_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-"""testing functions in fromgeometry module."""
+"""testing functions in from_geometry module."""
 
 from ladybug_geometry.geometry2d import Point2D, LineSegment2D
 from ladybug_geometry.geometry3d import Point3D, Polyline3D, Arc3D, Vector3D, Mesh3D,\
     Face3D, Plane, LineSegment3D, Polyface3D, Cone, Sphere, Cylinder
-from ladybug_vtk.fromgeometry import from_point2d, from_points2d, from_line2d, \
+from ladybug_vtk.from_geometry import from_point2d, from_points2d, from_line2d, \
     from_point3d, from_points3d, from_line3d, from_polyline3d, from_arc3d, from_mesh3d,\
     from_face3d, from_polyface3d, from_cone, from_sphere, from_cylinder, to_circle,\
     to_text
 
 
 def test_from_point2d():
     """Test point to Polydata conversion."""
@@ -132,18 +132,18 @@
     """Test polyface to Polydata conversion."""
     pts = [Point3D(0, 0, 0), Point3D(0, 2, 0), Point3D(2, 2, 0), Point3D(2, 0, 0),
            Point3D(0, 0, 2), Point3D(0, 2, 2), Point3D(2, 2, 2), Point3D(2, 0, 2)]
     face_indices = [[(0, 1, 2, 3)], [(0, 4, 5, 1)], [(0, 3, 7, 4)],
                     [(2, 1, 5, 6)], [(2, 3, 7, 6)], [(4, 5, 6, 7)]]
     polyface = Polyface3D(pts, face_indices)
     polydata = from_polyface3d(polyface)
-    assert polydata[0].GetNumberOfPoints() == 4
-    assert polydata[0].GetNumberOfCells() == 1
-    assert polydata[0].GetNumberOfPolys() == 1
-    assert polydata[0].GetBounds() == (0.0, 2.0, 0.0, 2.0, 0.0, 0.0)
+    assert polydata.GetNumberOfPoints() == 8
+    assert polydata.GetNumberOfCells() == 6
+    assert polydata.GetNumberOfPolys() == 6
+    assert polydata.GetBounds() == (0.0, 2.0, 0.0, 2.0, 0.0, 2.0)
 
 
 def test_from_cone():
     """Test cone to Polydata conversion."""
     vertex = Point3D(2, 0, 2)
     axis = Vector3D(0, 2, 2)
     angle = 0.7
```

