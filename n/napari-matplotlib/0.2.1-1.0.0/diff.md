# Comparing `tmp/napari_matplotlib-0.2.1.tar.gz` & `tmp/napari_matplotlib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_matplotlib-0.2.1.tar", last modified: Mon Jun  6 10:10:44 2022, max compression
+gzip compressed data, was "napari_matplotlib-1.0.0.tar", last modified: Fri Jun 30 11:33:34 2023, max compression
```

## Comparing `napari_matplotlib-0.2.1.tar` & `napari_matplotlib-1.0.0.tar`

### file list

```diff
@@ -1,60 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 10:10:44.553085 napari_matplotlib-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 10:10:44.549085 napari_matplotlib-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 10:10:44.549085 napari_matplotlib-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/.github/workflows/napari_hub_preview.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 10:10:44.549085 napari_matplotlib-0.2.1/.napari/
--rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4018 2022-06-06 10:10:44.557085 napari_matplotlib-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2749 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 10:10:44.549085 napari_matplotlib-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 10:10:44.549085 napari_matplotlib-0.2.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/docs/api/napari_matplotlib.HistogramWidget.rst
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2387 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-06-06 10:10:44.557085 napari_matplotlib-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 10:10:44.549085 napari_matplotlib-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 10:10:44.553085 napari_matplotlib-0.2.1/src/napari_matplotlib/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-06-06 10:10:43.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6051 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/histogram.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 10:10:44.553085 napari_matplotlib-0.2.1/src/napari_matplotlib/icons/
--rw-r--r--   0 runner    (1001) docker     (121)     6680 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Back.png
--rw-r--r--   0 runner    (1001) docker     (121)     6951 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Customize.png
--rw-r--r--   0 runner    (1001) docker     (121)     6535 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Forward.png
--rw-r--r--   0 runner    (1001) docker     (121)     7143 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Home.png
--rw-r--r--   0 runner    (1001) docker     (121)     7114 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Pan.png
--rw-r--r--   0 runner    (1001) docker     (121)    11810 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Pan_checked.png
--rw-r--r--   0 runner    (1001) docker     (121)     7381 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Save.png
--rw-r--r--   0 runner    (1001) docker     (121)     6739 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Subplots.png
--rw-r--r--   0 runner    (1001) docker     (121)     8064 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Zoom.png
--rw-r--r--   0 runner    (1001) docker     (121)    12372 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Zoom_checked.png
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6738 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/scatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3417 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/slice.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 10:10:44.553085 napari_matplotlib-0.2.1/src/napari_matplotlib/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     3375 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/tests/test_scatter.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/tests/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/src/napari_matplotlib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 10:10:44.553085 napari_matplotlib-0.2.1/src/napari_matplotlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4018 2022-06-06 10:10:43.000000 napari_matplotlib-0.2.1/src/napari_matplotlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-06-06 10:10:44.000000 napari_matplotlib-0.2.1/src/napari_matplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-06 10:10:43.000000 napari_matplotlib-0.2.1/src/napari_matplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-06-06 10:10:44.000000 napari_matplotlib-0.2.1/src/napari_matplotlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-06-06 10:10:44.000000 napari_matplotlib-0.2.1/src/napari_matplotlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-06 10:10:44.000000 napari_matplotlib-0.2.1/src/napari_matplotlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-06-06 10:10:16.000000 napari_matplotlib-0.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.158736 napari_matplotlib-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.162736 napari_matplotlib-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.github/workflows/napari_hub_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.162736 napari_matplotlib-1.0.0/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.napari/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.162736 napari_matplotlib-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.166736 napari_matplotlib-1.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)  1116521 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/_static/hist.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52586 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/third_party.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.158736 napari_matplotlib-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.166736 napari_matplotlib-1.0.0/src/napari_matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/histogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.158736 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.170736 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Back.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Customize.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Forward.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Home.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Pan.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Pan_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Save.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Subplots.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Zoom_checked.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.170736 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Back.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Customize.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Forward.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Home.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Pan.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Pan_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Save.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Subplots.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Zoom_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/slice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.170736 napari_matplotlib-1.0.0/src/napari_matplotlib/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/styles/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/styles/dark.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/styles/light.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    15662 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_custom_theme.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28728 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_histogram_2D.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20558 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_histogram_3D.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_no_theme_side_effects.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21290 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_slice_2D.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_slice_3D.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/data/test_theme.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    24951 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/baseline/test_features_scatter_widget_2D.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/baseline/test_scatter_2D.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/baseline/test_scatter_3D.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/test_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/test_scatter_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_layer_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.166736 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/tox.ini
```

### Comparing `napari_matplotlib-0.2.1/.github/workflows/napari_hub_preview.yml` & `napari_matplotlib-1.0.0/.github/workflows/napari_hub_preview.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,13 @@
   preview-page:
     if: ${{ github.event.label.name == 'napari hub preview' }}
     name: Preview Page Deploy
     runs-on: ubuntu-latest
 
     steps:
       - name: Checkout repo
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: napari hub Preview Page Builder
-        uses: chanzuckerberg/napari-hub-preview-action@v0.1.5
+        uses: chanzuckerberg/napari-hub-preview-action@v0.1
         with:
           hub-ref: main
```

### Comparing `napari_matplotlib-0.2.1/.github/workflows/test_and_deploy.yml` & `napari_matplotlib-1.0.0/.github/workflows/test_and_deploy.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-# This workflows will upload a Python Package using Twine when a release is created
-# For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
-
 name: tests
 
 on:
   push:
     branches:
       - main
     tags:
       - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
   pull_request:
     branches:
       - main
   workflow_dispatch:
+  merge_group:
 
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
+      fail-fast: false
       matrix:
-        platform: [ubuntu-latest]
+        platform: [ubuntu-latest, macos-latest, windows-latest]
         python-version: ['3.8', '3.9', '3.10']
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3
@@ -46,35 +45,52 @@
           python -m pip install --upgrade pip
           python -m pip install tox tox-gh-actions
 
       # this runs the platform-specific tests declared in tox.ini
       - name: Test with tox
         run: python -m tox
 
+      - name: Upload pytest test results
+        uses: actions/upload-artifact@v3
+        with:
+          name: pytest-results-${{ matrix.platform }} py${{ matrix.python-version }}
+          path: reports/
+        # Use always() to always run this step to publish test results when there are test failures
+        if: ${{ always() }}
+
       - name: Coverage
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v3
+        # Don't run coverage on merge queue CI to avoid duplicating reports
+        # to codecov. See https://github.com/matplotlib/napari-matplotlib/issues/155
+        if: github.event_name != 'merge_group'
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+          fail_ci_if_error: true
 
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your
     # github secrets (see readme for details)
     needs: [test]
     runs-on: ubuntu-latest
     if: contains(github.ref, 'tags')
+    environment: pypi-deploy
+    permissions:
+      id-token: write
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: "3.x"
-      - name: Install dependencies
+      - name: Install build
         run: |
           python -m pip install --upgrade pip
-          pip install -U setuptools setuptools_scm wheel twine build
-      - name: Build and publish
-        env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
+          python -m pip install --upgrade build
+
+      - name: Build package
         run: |
           git tag
           python -m build .
-          twine upload dist/*
+
+      - name: Publish package
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `napari_matplotlib-0.2.1/.gitignore` & `napari_matplotlib-1.0.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox/
+report/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *,cover
 .hypothesis/
@@ -80,7 +81,10 @@
 .python-version
 
 # OS
 .DS_Store
 
 # written by setuptools_scm
 **/_version.py
+
+# Generated by test runs
+reports
```

### Comparing `napari_matplotlib-0.2.1/LICENSE` & `napari_matplotlib-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-0.2.1/PKG-INFO` & `napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,76 @@
 Metadata-Version: 2.1
-Name: napari_matplotlib
-Version: 0.2.1
+Name: napari-matplotlib
+Version: 1.0.0
 Summary: A plugin to use Matplotlib with napari
 Home-page: https://github.com/matplotlib/napari-matplotlib
 Author: David Stansby
 Author-email: d.stansby@ucl.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/matplotlib/napari-matplotlib/issues
-Project-URL: Documentation, https://github.com/matplotlib/napari-matplotlib#README.md
+Project-URL: Documentation, https://napari-matplotlib.github.io
 Project-URL: Source Code, https://github.com/matplotlib/napari-matplotlib
 Project-URL: User Support, https://github.com/matplotlib/napari-matplotlib/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: testing
 License-File: LICENSE
 
 # napari-matplotlib
 
-[![License](https://img.shields.io/pypi/l/napari-matplotlib.svg?color=green)](https://github.com/dstansby/napari-matplotlib/raw/main/LICENSE)
+[![License](https://img.shields.io/pypi/l/napari-matplotlib.svg?color=green)](https://github.com/matplotlib/napari-matplotlib/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-matplotlib.svg?color=green)](https://pypi.org/project/napari-matplotlib)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-matplotlib.svg?color=green)](https://python.org)
-[![tests](https://github.com/dstansby/napari-matplotlib/workflows/tests/badge.svg)](https://github.com/dstansby/napari-matplotlib/actions)
-[![codecov](https://codecov.io/gh/dstansby/napari-matplotlib/branch/main/graph/badge.svg)](https://codecov.io/gh/dstansby/napari-matplotlib)
+[![tests](https://github.com/matplotlib/napari-matplotlib/workflows/tests/badge.svg)](https://github.com/matplotlib/napari-matplotlib/actions)
+[![codecov](https://codecov.io/gh/matplotlib/napari-matplotlib/branch/main/graph/badge.svg)](https://codecov.io/gh/matplotlib/napari-matplotlib)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/matplotlib/pytest-mpl/master.svg)](https://results.pre-commit.ci/latest/github/matplotlib/pytest-mpl/master)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-matplotlib)](https://napari-hub.org/plugins/napari-matplotlib)
 
 A plugin to create Matplotlib plots from napari layers
 
 ----------------------------------
 
 ## Introduction
 `napari-matplotlib` is a bridge between `napari` and `matplotlib`, making it easy to create publication quality `Matplotlib` plots based on the data loaded in `napari` layers.
 
 ## Available widgets
 
 ### `Slice`
 Plots 1D slices of data along a specified axis.
-![](https://raw.githubusercontent.com/dstansby/napari-matplotlib/main/examples/slice.png)
+![](https://raw.githubusercontent.com/matplotlib/napari-matplotlib/main/examples/slice.png)
 
 ### `Histogram`
 Plots histograms of individual image layers, or RGB histograms of an RGB image
-![](https://raw.githubusercontent.com/dstansby/napari-matplotlib/main/examples/hist.png)
+![](https://raw.githubusercontent.com/matplotlib/napari-matplotlib/main/examples/hist.png)
 
 ### `Scatter`
 Scatters the values of two similarly sized images layers against each other.
-![](https://raw.githubusercontent.com/dstansby/napari-matplotlib/main/examples/scatter.png)
+![](https://raw.githubusercontent.com/matplotlib/napari-matplotlib/main/examples/scatter.png)
 
 ## Installation
 
 You can install `napari-matplotlib` via [pip]:
 
     pip install napari-matplotlib
 
 
 
 To install latest development version :
 
-    pip install git+https://github.com/dstansby/napari-matplotlib.git
+    pip install git+https://github.com/matplotlib/napari-matplotlib.git
 
 
 ## Contributing
 
 Contributions are very welcome! Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
```

### Comparing `napari_matplotlib-0.2.1/README.md` & `napari_matplotlib-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # napari-matplotlib
 
-[![License](https://img.shields.io/pypi/l/napari-matplotlib.svg?color=green)](https://github.com/dstansby/napari-matplotlib/raw/main/LICENSE)
+[![License](https://img.shields.io/pypi/l/napari-matplotlib.svg?color=green)](https://github.com/matplotlib/napari-matplotlib/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-matplotlib.svg?color=green)](https://pypi.org/project/napari-matplotlib)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-matplotlib.svg?color=green)](https://python.org)
-[![tests](https://github.com/dstansby/napari-matplotlib/workflows/tests/badge.svg)](https://github.com/dstansby/napari-matplotlib/actions)
-[![codecov](https://codecov.io/gh/dstansby/napari-matplotlib/branch/main/graph/badge.svg)](https://codecov.io/gh/dstansby/napari-matplotlib)
+[![tests](https://github.com/matplotlib/napari-matplotlib/workflows/tests/badge.svg)](https://github.com/matplotlib/napari-matplotlib/actions)
+[![codecov](https://codecov.io/gh/matplotlib/napari-matplotlib/branch/main/graph/badge.svg)](https://codecov.io/gh/matplotlib/napari-matplotlib)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/matplotlib/pytest-mpl/master.svg)](https://results.pre-commit.ci/latest/github/matplotlib/pytest-mpl/master)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-matplotlib)](https://napari-hub.org/plugins/napari-matplotlib)
 
 A plugin to create Matplotlib plots from napari layers
 
 ----------------------------------
 
 ## Introduction
 `napari-matplotlib` is a bridge between `napari` and `matplotlib`, making it easy to create publication quality `Matplotlib` plots based on the data loaded in `napari` layers.
 
 ## Available widgets
 
 ### `Slice`
 Plots 1D slices of data along a specified axis.
-![](https://raw.githubusercontent.com/dstansby/napari-matplotlib/main/examples/slice.png)
+![](https://raw.githubusercontent.com/matplotlib/napari-matplotlib/main/examples/slice.png)
 
 ### `Histogram`
 Plots histograms of individual image layers, or RGB histograms of an RGB image
-![](https://raw.githubusercontent.com/dstansby/napari-matplotlib/main/examples/hist.png)
+![](https://raw.githubusercontent.com/matplotlib/napari-matplotlib/main/examples/hist.png)
 
 ### `Scatter`
 Scatters the values of two similarly sized images layers against each other.
-![](https://raw.githubusercontent.com/dstansby/napari-matplotlib/main/examples/scatter.png)
+![](https://raw.githubusercontent.com/matplotlib/napari-matplotlib/main/examples/scatter.png)
 
 ## Installation
 
 You can install `napari-matplotlib` via [pip]:
 
     pip install napari-matplotlib
 
 
 
 To install latest development version :
 
-    pip install git+https://github.com/dstansby/napari-matplotlib.git
+    pip install git+https://github.com/matplotlib/napari-matplotlib.git
 
 
 ## Contributing
 
 Contributions are very welcome! Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
```

### Comparing `napari_matplotlib-0.2.1/docs/make.bat` & `napari_matplotlib-1.0.0/docs/make.bat`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 pushd %~dp0
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
+if "%SPHINXOPTS%" == "" (
+	set SPHINXOPTS="--keep-going"
+)
 set SOURCEDIR=.
 set BUILDDIR=_build
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
```

### Comparing `napari_matplotlib-0.2.1/setup.cfg` & `napari_matplotlib-1.0.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -3,40 +3,38 @@
 description = A plugin to use Matplotlib with napari
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/matplotlib/napari-matplotlib
 author = David Stansby
 author_email = d.stansby@ucl.ac.uk
 license = BSD-3-Clause
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
 	Framework :: napari
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 	Topic :: Software Development :: Testing
 project_urls = 
 	Bug Tracker = https://github.com/matplotlib/napari-matplotlib/issues
-	Documentation = https://github.com/matplotlib/napari-matplotlib#README.md
+	Documentation = https://napari-matplotlib.github.io
 	Source Code = https://github.com/matplotlib/napari-matplotlib
 	User Support = https://github.com/matplotlib/napari-matplotlib/issues
 
 [options]
 packages = find:
 install_requires = 
 	matplotlib
 	napari
 	numpy
+	tinycss2
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = 
 	setuptools-scm
 
@@ -45,24 +43,29 @@
 
 [options.entry_points]
 napari.manifest = 
 	napari-matplotlib = napari_matplotlib:napari.yaml
 
 [options.extras_require]
 docs = 
+	napari[all]
 	numpydoc
 	pydata-sphinx-theme
 	qtgallery
 	sphinx
 	sphinx-automodapi
 	sphinx-gallery
 testing = 
-	napari[pyqt5]
+	napari[pyqt6-experimental]
+	pooch
+	pyqt6
 	pytest
 	pytest-cov
+	pytest-mock
+	pytest-mpl
 	pytest-qt
 	tox
 	pytest-xvfb;sys_platform == 'linux'
 
 [options.package_data]
 * = *.yaml
```

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/histogram.py` & `napari_matplotlib-1.0.0/src/napari_matplotlib/histogram.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-import numpy as np
-
-from .base import NapariMPLWidget
-
-__all__ = ["HistogramWidget"]
+from typing import Optional
 
 import napari
+import numpy as np
+from qtpy.QtWidgets import QWidget
 
+from .base import SingleAxesWidget
 from .util import Interval
 
+__all__ = ["HistogramWidget"]
+
 _COLORS = {"r": "tab:red", "g": "tab:green", "b": "tab:blue"}
 
 
-class HistogramWidget(NapariMPLWidget):
+class HistogramWidget(SingleAxesWidget):
     """
     Display a histogram of the currently selected layer.
     """
 
     n_layers_input = Interval(1, 1)
     input_layer_types = (napari.layers.Image,)
 
-    def __init__(self, napari_viewer: napari.viewer.Viewer):
-        super().__init__(napari_viewer)
-        self.axes = self.canvas.figure.subplots()
-        self.update_layers(None)
-
-    def clear(self) -> None:
-        self.axes.clear()
+    def __init__(
+        self,
+        napari_viewer: napari.viewer.Viewer,
+        parent: Optional[QWidget] = None,
+    ):
+        super().__init__(napari_viewer, parent=parent)
+        self._update_layers(None)
 
     def draw(self) -> None:
         """
         Clear the axes and histogram the currently selected layer/slice.
         """
         layer = self.layers[0]
         bins = np.linspace(np.min(layer.data), np.max(layer.data), 100)
```

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Back.png` & `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Back.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Customize.png` & `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Customize.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Forward.png` & `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Forward.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Home.png` & `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Home.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Pan.png` & `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Pan.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Pan_checked.png` & `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Pan_checked.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Save.png` & `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Save.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Subplots.png` & `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Subplots.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Zoom.png` & `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Zoom.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/icons/Zoom_checked.png` & `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Zoom_checked.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/napari.yaml` & `napari_matplotlib-1.0.0/src/napari_matplotlib/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/scatter.py` & `napari_matplotlib-1.0.0/src/napari_matplotlib/scatter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,224 +1,230 @@
-from typing import List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 
-import matplotlib.colors as mcolor
 import napari
-import numpy as np
-from magicgui import magicgui
-from magicgui.widgets import ComboBox
+import numpy.typing as npt
+from qtpy.QtWidgets import QComboBox, QLabel, QVBoxLayout, QWidget
 
-from .base import NapariMPLWidget
+from .base import SingleAxesWidget
 from .util import Interval
 
-__all__ = ["ScatterWidget", "FeaturesScatterWidget"]
+__all__ = ["ScatterBaseWidget", "ScatterWidget", "FeaturesScatterWidget"]
 
 
-class ScatterBaseWidget(NapariMPLWidget):
-    # opacity value for the markers
-    _marker_alpha = 0.5
-
-    # flag set to True if histogram should be used
-    # for plotting large points
-    _histogram_for_large_data = True
+class ScatterBaseWidget(SingleAxesWidget):
+    """
+    Base class for widgets that scatter two datasets against each other.
+    """
 
     # if the number of points is greater than this value,
-    # the scatter is plotted as a 2dhist
+    # the scatter is plotted as a 2D histogram
     _threshold_to_switch_to_histogram = 500
 
-    def __init__(self, napari_viewer: napari.viewer.Viewer):
-        super().__init__(napari_viewer)
-
-        self.axes = self.canvas.figure.subplots()
-        self.update_layers(None)
-
-    def clear(self) -> None:
-        """
-        Clear the axes.
-        """
-        self.axes.clear()
-
     def draw(self) -> None:
         """
         Scatter the currently selected layers.
         """
-        data, x_axis_name, y_axis_name = self._get_data()
-
-        if len(data) == 0:
-            # don't plot if there isn't data
+        if len(self.layers) == 0:
             return
+        x, y, x_axis_name, y_axis_name = self._get_data()
 
-        if self._histogram_for_large_data and (
-            data[0].size > self._threshold_to_switch_to_histogram
-        ):
+        if x.size > self._threshold_to_switch_to_histogram:
             self.axes.hist2d(
-                data[0].ravel(),
-                data[1].ravel(),
+                x.ravel(),
+                y.ravel(),
                 bins=100,
-                norm=mcolor.LogNorm(),
             )
         else:
-            self.axes.scatter(data[0], data[1], alpha=self._marker_alpha)
+            self.axes.scatter(x, y, alpha=0.5)
 
         self.axes.set_xlabel(x_axis_name)
         self.axes.set_ylabel(y_axis_name)
 
-    def _get_data(self) -> Tuple[List[np.ndarray], str, str]:
-        """Get the plot data.
+    def _get_data(self) -> Tuple[npt.NDArray[Any], npt.NDArray[Any], str, str]:
+        """
+        Get the plot data.
 
         This must be implemented on the subclass.
 
         Returns
         -------
-        data : np.ndarray
-            The list containing the scatter plot data.
-        x_axis_name : str
-            The label to display on the x axis
-        y_axis_name: str
-            The label to display on the y axis
+        x, y : np.ndarray
+            x and y values of plot data.
+        x_axis_name, y_axis_name : str
+            Label to display on the x/y axis
         """
         raise NotImplementedError
 
 
 class ScatterWidget(ScatterBaseWidget):
     """
-    Widget to display scatter plot of two similarly shaped image layers.
+    Scatter data in two similarly shaped layers.
 
     If there are more than 500 data points, a 2D histogram is displayed instead
     of a scatter plot, to avoid too many scatter points.
     """
 
     n_layers_input = Interval(2, 2)
     input_layer_types = (napari.layers.Image,)
 
-    def _get_data(self) -> Tuple[List[np.ndarray], str, str]:
-        """Get the plot data.
+    def _get_data(self) -> Tuple[npt.NDArray[Any], npt.NDArray[Any], str, str]:
+        """
+        Get the plot data.
 
         Returns
         -------
         data : List[np.ndarray]
             List contains the in view slice of X and Y axis images.
         x_axis_name : str
             The title to display on the x axis
         y_axis_name: str
             The title to display on the y axis
         """
-        data = [layer.data[self.current_z] for layer in self.layers]
+        x = self.layers[0].data[self.current_z]
+        y = self.layers[1].data[self.current_z]
         x_axis_name = self.layers[0].name
         y_axis_name = self.layers[1].name
 
-        return data, x_axis_name, y_axis_name
+        return x, y, x_axis_name, y_axis_name
 
 
 class FeaturesScatterWidget(ScatterBaseWidget):
+    """
+    Widget to scatter data stored in two layer feature attributes.
+    """
+
     n_layers_input = Interval(1, 1)
     # All layers that have a .features attributes
     input_layer_types = (
         napari.layers.Labels,
         napari.layers.Points,
         napari.layers.Shapes,
         napari.layers.Tracks,
         napari.layers.Vectors,
     )
 
-    def __init__(self, napari_viewer: napari.viewer.Viewer):
-        super().__init__(napari_viewer)
-        self._key_selection_widget = magicgui(
-            self._set_axis_keys,
-            x_axis_key={"choices": self._get_valid_axis_keys},
-            y_axis_key={"choices": self._get_valid_axis_keys},
-            call_button="plot",
-        )
+    def __init__(
+        self,
+        napari_viewer: napari.viewer.Viewer,
+        parent: Optional[QWidget] = None,
+    ):
+        super().__init__(napari_viewer, parent=parent)
+
+        self.layout().addLayout(QVBoxLayout())
+
+        self._selectors: Dict[str, QComboBox] = {}
+        for dim in ["x", "y"]:
+            self._selectors[dim] = QComboBox()
+            # Re-draw when combo boxes are updated
+            self._selectors[dim].currentTextChanged.connect(self._draw)
+
+            self.layout().addWidget(QLabel(f"{dim}-axis:"))
+            self.layout().addWidget(self._selectors[dim])
 
-        self.layout().addWidget(self._key_selection_widget.native)
+        self._update_layers(None)
 
     @property
-    def x_axis_key(self) -> Optional[str]:
-        """Key to access x axis data from the FeaturesTable"""
-        return self._x_axis_key
+    def x_axis_key(self) -> Union[str, None]:
+        """
+        Key for the x-axis data.
+        """
+        if self._selectors["x"].count() == 0:
+            return None
+        else:
+            return self._selectors["x"].currentText()
 
     @x_axis_key.setter
-    def x_axis_key(self, key: Optional[str]) -> None:
-        self._x_axis_key = key
+    def x_axis_key(self, key: str) -> None:
+        self._selectors["x"].setCurrentText(key)
         self._draw()
 
     @property
-    def y_axis_key(self) -> Optional[str]:
-        """Key to access y axis data from the FeaturesTable"""
-        return self._y_axis_key
+    def y_axis_key(self) -> Union[str, None]:
+        """
+        Key for the y-axis data.
+        """
+        if self._selectors["y"].count() == 0:
+            return None
+        else:
+            return self._selectors["y"].currentText()
 
     @y_axis_key.setter
-    def y_axis_key(self, key: Optional[str]) -> None:
-        self._y_axis_key = key
+    def y_axis_key(self, key: str) -> None:
+        self._selectors["y"].setCurrentText(key)
         self._draw()
 
-    def _set_axis_keys(self, x_axis_key: str, y_axis_key: str) -> None:
-        """Set both axis keys and then redraw the plot"""
-        self._x_axis_key = x_axis_key
-        self._y_axis_key = y_axis_key
-        self._draw()
-
-    def _get_valid_axis_keys(
-        self, combo_widget: Optional[ComboBox] = None
-    ) -> List[str]:
+    def _get_valid_axis_keys(self) -> List[str]:
         """
         Get the valid axis keys from the layer FeatureTable.
 
         Returns
         -------
         axis_keys : List[str]
             The valid axis keys in the FeatureTable. If the table is empty
             or there isn't a table, returns an empty list.
         """
         if len(self.layers) == 0 or not (hasattr(self.layers[0], "features")):
             return []
         else:
             return self.layers[0].features.keys()
 
-    def _get_data(self) -> Tuple[List[np.ndarray], str, str]:
-        """Get the plot data.
+    def _ready_to_scatter(self) -> bool:
+        """
+        Return True if selected layer has a feature table we can scatter with,
+        and the two columns to be scatterd have been selected.
+        """
+        if not hasattr(self.layers[0], "features"):
+            return False
+
+        feature_table = self.layers[0].features
+        valid_keys = self._get_valid_axis_keys()
+        return (
+            feature_table is not None
+            and len(feature_table) > 0
+            and self.x_axis_key in valid_keys
+            and self.y_axis_key in valid_keys
+        )
+
+    def draw(self) -> None:
+        """
+        Scatter two features from the currently selected layer.
+        """
+        if self._ready_to_scatter():
+            super().draw()
+
+    def _get_data(self) -> Tuple[npt.NDArray[Any], npt.NDArray[Any], str, str]:
+        """
+        Get the plot data from the ``features`` attribute of the first
+        selected layer.
 
         Returns
         -------
         data : List[np.ndarray]
             List contains X and Y columns from the FeatureTable. Returns
             an empty array if nothing to plot.
         x_axis_name : str
             The title to display on the x axis. Returns
             an empty string if nothing to plot.
         y_axis_name: str
             The title to display on the y axis. Returns
             an empty string if nothing to plot.
         """
-        if not hasattr(self.layers[0], "features"):
-            # if the selected layer doesn't have a featuretable,
-            # skip draw
-            return [], "", ""
-
         feature_table = self.layers[0].features
 
-        if (
-            (len(feature_table) == 0)
-            or (self.x_axis_key is None)
-            or (self.y_axis_key is None)
-        ):
-            return [], "", ""
+        x = feature_table[self.x_axis_key]
+        y = feature_table[self.y_axis_key]
 
-        data_x = feature_table[self.x_axis_key]
-        data_y = feature_table[self.y_axis_key]
-        data = [data_x, data_y]
+        x_axis_name = str(self.x_axis_key)
+        y_axis_name = str(self.y_axis_key)
 
-        x_axis_name = self.x_axis_key.replace("_", " ")
-        y_axis_name = self.y_axis_key.replace("_", " ")
+        return x, y, x_axis_name, y_axis_name
 
-        return data, x_axis_name, y_axis_name
-
-    def _on_update_layers(self) -> None:
+    def on_update_layers(self) -> None:
         """
-        This is called when the layer selection changes by
-        ``self.update_layers()``.
+        Called when the layer selection changes by ``self.update_layers()``.
         """
-        if hasattr(self, "_key_selection_widget"):
-            self._key_selection_widget.reset_choices()
-
-        # reset the axis keys
-        self._x_axis_key = None
-        self._y_axis_key = None
+        # Clear combobox
+        for dim in ["x", "y"]:
+            while self._selectors[dim].count() > 0:
+                self._selectors[dim].removeItem(0)
+            # Add keys for newly selected layer
+            self._selectors[dim].addItems(self._get_valid_axis_keys())
```

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/slice.py` & `napari_matplotlib-1.0.0/src/napari_matplotlib/slice.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from typing import Dict, Tuple
+from typing import Any, Dict, Optional, Tuple
 
+import matplotlib.ticker as mticker
 import napari
 import numpy as np
-from qtpy.QtWidgets import QComboBox, QHBoxLayout, QLabel, QSpinBox
+import numpy.typing as npt
+from qtpy.QtWidgets import QComboBox, QHBoxLayout, QLabel, QSpinBox, QWidget
 
-from .base import NapariMPLWidget
+from .base import SingleAxesWidget
 from .util import Interval
 
 __all__ = ["SliceWidget"]
 
 _dims_sel = ["x", "y"]
 _dims = ["x", "y", "z"]
 
 
-class SliceWidget(NapariMPLWidget):
+class SliceWidget(SingleAxesWidget):
     """
     Plot a 1D slice along a given dimension.
     """
 
     n_layers_input = Interval(1, 1)
     input_layer_types = (napari.layers.Image,)
 
-    def __init__(self, napari_viewer: napari.viewer.Viewer):
+    def __init__(
+        self,
+        napari_viewer: napari.viewer.Viewer,
+        parent: Optional[QWidget] = None,
+    ):
         # Setup figure/axes
-        super().__init__(napari_viewer)
-        self.axes = self.canvas.figure.subplots()
+        super().__init__(napari_viewer, parent=parent)
 
         button_layout = QHBoxLayout()
         self.layout().addLayout(button_layout)
 
         self.dim_selector = QComboBox()
         button_layout.addWidget(QLabel("Slice axis:"))
         button_layout.addWidget(self.dim_selector)
@@ -42,18 +47,21 @@
 
         # Setup callbacks
         # Re-draw when any of the combon/spin boxes are updated
         self.dim_selector.currentTextChanged.connect(self._draw)
         for d in _dims_sel:
             self.slice_selectors[d].textChanged.connect(self._draw)
 
-        self.update_layers(None)
+        self._update_layers(None)
 
     @property
-    def layer(self):
+    def _layer(self) -> napari.layers.Layer:
+        """
+        Layer being plotted.
+        """
         return self.layers[0]
 
     @property
     def current_dim(self) -> str:
         """
         Currently selected slice dimension.
         """
@@ -65,56 +73,51 @@
         Currently selected slice dimension index.
         """
         # Note the reversed list because in napari the z-axis is the first
         # numpy axis
         return _dims[::-1].index(self.current_dim)
 
     @property
-    def selector_values(self) -> Dict[str, int]:
-        return {d: self.slice_selectors[d].value() for d in _dims_sel}
-
-    def update_slice_selectors(self) -> None:
+    def _selector_values(self) -> Dict[str, int]:
         """
-        Update range and enabled status of the slice selectors, and the value
-        of the z slice selector.
+        Values of the slice selectors.
         """
-        # Update min/max
-        for i, dim in enumerate(_dims_sel):
-            self.slice_selectors[dim].setRange(0, self.layer.data.shape[i])
+        return {d: self.slice_selectors[d].value() for d in _dims_sel}
 
-    def get_xy(self) -> Tuple[np.ndarray, np.ndarray]:
+    def _get_xy(self) -> Tuple[npt.NDArray[Any], npt.NDArray[Any]]:
         """
         Get data for plotting.
         """
-        x = np.arange(self.layer.data.shape[self.current_dim_index])
+        x = np.arange(self._layer.data.shape[self.current_dim_index])
 
-        vals = self.selector_values
+        vals = self._selector_values
         vals.update({"z": self.current_z})
 
         slices = []
         for d in _dims:
             if d == self.current_dim:
                 # Select all data along this axis
                 slices.append(slice(None))
             else:
                 # Select specific index
                 val = vals[d]
                 slices.append(slice(val, val + 1))
 
         # Reverse since z is the first axis in napari
         slices = slices[::-1]
-        y = self.layer.data[tuple(slices)].ravel()
+        y = self._layer.data[tuple(slices)].ravel()
 
         return x, y
 
-    def clear(self) -> None:
-        self.axes.cla()
-
     def draw(self) -> None:
         """
         Clear axes and draw a 1D plot.
         """
-        x, y = self.get_xy()
+        x, y = self._get_xy()
 
         self.axes.plot(x, y)
         self.axes.set_xlabel(self.current_dim)
-        self.axes.set_title(self.layer.name)
+        self.axes.set_title(self._layer.name)
+        # Make sure all ticks lie on integer values
+        self.axes.xaxis.set_major_locator(
+            mticker.MaxNLocator(steps=[1, 2, 5, 10], integer=True)
+        )
```

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib/tests/test_scatter.py` & `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/test_scatter_features.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,62 @@
+from copy import deepcopy
+from typing import Any, Dict, Tuple
+
 import numpy as np
+import numpy.typing as npt
+import pytest
 
-from napari_matplotlib import FeaturesScatterWidget, ScatterWidget
+from napari_matplotlib import FeaturesScatterWidget
 
 
-def test_scatter(make_napari_viewer):
-    # Smoke test adding a scatter widget
+@pytest.mark.mpl_image_compare
+def test_features_scatter_widget_2D(
+    make_napari_viewer, points_with_features_data
+):
     viewer = make_napari_viewer()
-    viewer.add_image(np.random.random((100, 100)))
-    viewer.add_image(np.random.random((100, 100)))
-    ScatterWidget(viewer)
+    viewer.theme = "light"
+    widget = FeaturesScatterWidget(viewer)
 
+    viewer.add_points(
+        points_with_features_data[0], **points_with_features_data[1]
+    )
+    assert len(viewer.layers) == 1
+    # De-select existing selection
+    viewer.layers.selection.clear()
 
-def test_features_scatter_widget(make_napari_viewer):
-    # Smoke test adding a features scatter widget
-    viewer = make_napari_viewer()
-    viewer.add_image(np.random.random((100, 100)))
-    viewer.add_labels(np.random.randint(0, 5, (100, 100)))
-    FeaturesScatterWidget(viewer)
+    # Select points data and chosen features
+    viewer.layers.selection.add(viewer.layers[0])  # images need to be selected
+    widget.x_axis_key = "feature_0"
+    widget.y_axis_key = "feature_1"
+
+    fig = widget.figure
+
+    return deepcopy(fig)
 
 
-def make_labels_layer_with_features():
-    label_image = np.zeros((100, 100), dtype=np.uint16)
+def make_labels_layer_with_features() -> (
+    Tuple[npt.NDArray[np.uint16], Dict[str, Any]]
+):
+    label_image: npt.NDArray[np.uint16] = np.zeros((100, 100), dtype=np.uint16)
     for label_value, start_index in enumerate([10, 30, 50], start=1):
         end_index = start_index + 10
         label_image[start_index:end_index, start_index:end_index] = label_value
     feature_table = {
         "index": [1, 2, 3],
         "feature_0": np.random.random((3,)),
         "feature_1": np.random.random((3,)),
         "feature_2": np.random.random((3,)),
     }
     return label_image, feature_table
 
 
 def test_features_scatter_get_data(make_napari_viewer):
-    """test the get data method"""
+    """
+    Test the get data method.
+    """
     # make the label image
     label_image, feature_table = make_labels_layer_with_features()
 
     viewer = make_napari_viewer()
     labels_layer = viewer.add_labels(label_image, features=feature_table)
     scatter_widget = FeaturesScatterWidget(viewer)
 
@@ -46,25 +64,24 @@
     viewer.layers.selection = [labels_layer]
 
     x_column = "feature_0"
     scatter_widget.x_axis_key = x_column
     y_column = "feature_2"
     scatter_widget.y_axis_key = y_column
 
-    data, x_axis_name, y_axis_name = scatter_widget._get_data()
-    np.testing.assert_allclose(
-        data, np.stack((feature_table[x_column], feature_table[y_column]))
-    )
-    assert x_axis_name == x_column.replace("_", " ")
-    assert y_axis_name == y_column.replace("_", " ")
+    x, y, x_axis_name, y_axis_name = scatter_widget._get_data()
+    np.testing.assert_allclose(x, feature_table[x_column])
+    np.testing.assert_allclose(y, np.stack(feature_table[y_column]))
+    assert x_axis_name == x_column
+    assert y_axis_name == y_column
 
 
 def test_get_valid_axis_keys(make_napari_viewer):
-    """test the values returned from
-    FeaturesScatterWidget._get_valid_keys() when there
+    """
+    Test the values returned from _get_valid_keys() when there
     are valid keys.
     """
     # make the label image
     label_image, feature_table = make_labels_layer_with_features()
 
     viewer = make_napari_viewer()
     labels_layer = viewer.add_labels(label_image, features=feature_table)
@@ -72,15 +89,15 @@
 
     viewer.layers.selection = [labels_layer]
     valid_keys = scatter_widget._get_valid_axis_keys()
     assert set(valid_keys) == set(feature_table.keys())
 
 
 def test_get_valid_axis_keys_no_valid_keys(make_napari_viewer):
-    """test the values returned from
+    """Test the values returned from
     FeaturesScatterWidget._get_valid_keys() when there
     are not valid keys.
     """
     # make the label image
     label_image, _ = make_labels_layer_with_features()
 
     viewer = make_napari_viewer()
```

### Comparing `napari_matplotlib-0.2.1/src/napari_matplotlib.egg-info/PKG-INFO` & `napari_matplotlib-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,76 @@
 Metadata-Version: 2.1
-Name: napari-matplotlib
-Version: 0.2.1
+Name: napari_matplotlib
+Version: 1.0.0
 Summary: A plugin to use Matplotlib with napari
 Home-page: https://github.com/matplotlib/napari-matplotlib
 Author: David Stansby
 Author-email: d.stansby@ucl.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/matplotlib/napari-matplotlib/issues
-Project-URL: Documentation, https://github.com/matplotlib/napari-matplotlib#README.md
+Project-URL: Documentation, https://napari-matplotlib.github.io
 Project-URL: Source Code, https://github.com/matplotlib/napari-matplotlib
 Project-URL: User Support, https://github.com/matplotlib/napari-matplotlib/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: testing
 License-File: LICENSE
 
 # napari-matplotlib
 
-[![License](https://img.shields.io/pypi/l/napari-matplotlib.svg?color=green)](https://github.com/dstansby/napari-matplotlib/raw/main/LICENSE)
+[![License](https://img.shields.io/pypi/l/napari-matplotlib.svg?color=green)](https://github.com/matplotlib/napari-matplotlib/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-matplotlib.svg?color=green)](https://pypi.org/project/napari-matplotlib)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-matplotlib.svg?color=green)](https://python.org)
-[![tests](https://github.com/dstansby/napari-matplotlib/workflows/tests/badge.svg)](https://github.com/dstansby/napari-matplotlib/actions)
-[![codecov](https://codecov.io/gh/dstansby/napari-matplotlib/branch/main/graph/badge.svg)](https://codecov.io/gh/dstansby/napari-matplotlib)
+[![tests](https://github.com/matplotlib/napari-matplotlib/workflows/tests/badge.svg)](https://github.com/matplotlib/napari-matplotlib/actions)
+[![codecov](https://codecov.io/gh/matplotlib/napari-matplotlib/branch/main/graph/badge.svg)](https://codecov.io/gh/matplotlib/napari-matplotlib)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/matplotlib/pytest-mpl/master.svg)](https://results.pre-commit.ci/latest/github/matplotlib/pytest-mpl/master)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-matplotlib)](https://napari-hub.org/plugins/napari-matplotlib)
 
 A plugin to create Matplotlib plots from napari layers
 
 ----------------------------------
 
 ## Introduction
 `napari-matplotlib` is a bridge between `napari` and `matplotlib`, making it easy to create publication quality `Matplotlib` plots based on the data loaded in `napari` layers.
 
 ## Available widgets
 
 ### `Slice`
 Plots 1D slices of data along a specified axis.
-![](https://raw.githubusercontent.com/dstansby/napari-matplotlib/main/examples/slice.png)
+![](https://raw.githubusercontent.com/matplotlib/napari-matplotlib/main/examples/slice.png)
 
 ### `Histogram`
 Plots histograms of individual image layers, or RGB histograms of an RGB image
-![](https://raw.githubusercontent.com/dstansby/napari-matplotlib/main/examples/hist.png)
+![](https://raw.githubusercontent.com/matplotlib/napari-matplotlib/main/examples/hist.png)
 
 ### `Scatter`
 Scatters the values of two similarly sized images layers against each other.
-![](https://raw.githubusercontent.com/dstansby/napari-matplotlib/main/examples/scatter.png)
+![](https://raw.githubusercontent.com/matplotlib/napari-matplotlib/main/examples/scatter.png)
 
 ## Installation
 
 You can install `napari-matplotlib` via [pip]:
 
     pip install napari-matplotlib
 
 
 
 To install latest development version :
 
-    pip install git+https://github.com/dstansby/napari-matplotlib.git
+    pip install git+https://github.com/matplotlib/napari-matplotlib.git
 
 
 ## Contributing
 
 Contributions are very welcome! Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
```

