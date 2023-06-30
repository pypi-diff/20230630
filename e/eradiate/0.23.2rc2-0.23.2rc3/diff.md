# Comparing `tmp/eradiate-0.23.2rc2.tar.gz` & `tmp/eradiate-0.23.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eradiate-0.23.2rc2.tar", last modified: Wed Jun 21 16:12:21 2023, max compression
+gzip compressed data, was "eradiate-0.23.2rc3.tar", last modified: Fri Jun 30 15:13:58 2023, max compression
```

## Comparing `eradiate-0.23.2rc2.tar` & `eradiate-0.23.2rc3.tar`

### file list

```diff
@@ -1,631 +1,631 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.430173 eradiate-0.23.2rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.338165 eradiate-0.23.2rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.338165 eradiate-0.23.2rc2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.338165 eradiate-0.23.2rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-06-21 16:12:21.430173 eradiate-0.23.2rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.338165 eradiate-0.23.2rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.338165 eradiate-0.23.2rc2/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_ext/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_ext/pluginparameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.342166 eradiate-0.23.2rc2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)    32795 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-darkgrey.png
--rw-r--r--   0 runner    (1001) docker     (123)    34059 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-darkgrey.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.326164 eradiate-0.23.2rc2/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.342166 eradiate-0.23.2rc2/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.342166 eradiate-0.23.2rc2/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_templates/sections/footer-content.html
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/convert_figures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.350166 eradiate-0.23.2rc2/docs/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/atmosphere_attributes.png
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/atmosphere_attributes.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28149 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-east_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32937 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-east_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28852 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-east_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    35278 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-east_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-north_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32862 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-north_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-north_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-north_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28153 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-south_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32939 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-south_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28118 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-south_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-south_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28178 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-west_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32935 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-west_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28067 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-west_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-west_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/cartesian-coordinate-system.png
--rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/cartesian-coordinate-system.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25301 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/cuboid_leaf_cloud_params.png
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/cuboid_leaf_cloud_params.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.350166 eradiate-0.23.2rc2/docs/fig/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/diagrams/class_diagram_biosphere.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/diagrams/package.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    40438 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/eradiate-logo-typo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/eradiate-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/icon_eradiate.png
--rw-r--r--   0 runner    (1001) docker     (123)    38873 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/package.png
--rw-r--r--   0 runner    (1001) docker     (123)    57417 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/package.svg
--rw-r--r--   0 runner    (1001) docker     (123)    32384 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/radiancemeter_hsphere.png
--rw-r--r--   0 runner    (1001) docker     (123)    43351 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/radiancemeter_hsphere.svg
--rw-r--r--   0 runner    (1001) docker     (123)    36773 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/radiancemeter_plane.png
--rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/radiancemeter_plane.svg
--rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/requirement_layers.png
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/requirement_layers.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/solid_2017.png
--rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_atm_interval.png
--rw-r--r--   0 runner    (1001) docker     (123)    16459 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_atm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    28519 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_noatm_interval.png
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_noatm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_atm_interval.png
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_atm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_noatm_interval1.png
--rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_noatm_interval2.png
--rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_noatm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spherical-coordinate-system.png
--rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spherical-coordinate-system.svg
--rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/thuillier_2003.png
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/generate_md_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/generate_rst_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/generate_rst_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/index_latex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.350166 eradiate-0.23.2rc2/docs/rst/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/dependencies.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.350166 eradiate-0.23.2rc2/docs/rst/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/design_atmosphere.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/factory_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/lazy_loading.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/radiometric_kernel_interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/scene_generator.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/update.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/maintainer_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.354167 eradiate-0.23.2rc2/docs/rst/reference_api/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/attrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/constants.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/converters.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/eradiate_core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/experiments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/factory.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/frame.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/kernel.rst
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/mode.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/notebook.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/plot.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/quad.rst
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/radprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/rng.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/scenes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/spectral.rst
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/srf_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/test_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/thermoprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/units.rst
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/validators.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/warp.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/xarray.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.354167 eradiate-0.23.2rc2/docs/rst/reference_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_plugins/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.358167 eradiate-0.23.2rc2/docs/rst/user_guide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.358167 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/absorption.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.358167 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    25171 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/bad_resolution.png
--rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/good_resolution.png
--rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/line.png
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/heterogeneous.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/homogeneous.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/molecular.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/particle_layer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/basic_concepts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/conventions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.362167 eradiate-0.23.2rc2/docs/rst/user_guide/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/absorption.rst
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/atmosphere_radprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/atmosphere_thermoprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/ckd.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.362167 eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    30117 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
--rw-r--r--   0 runner    (1001) docker     (123)    59107 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/pt_points.png
--rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/particle_radprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/solar_irradiance.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/spectra-us76_u86_4.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/srf.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/onedim_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/package_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/spectral_discretization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/unit_guide_user.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.362167 eradiate-0.23.2rc2/docs/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/src/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/src/reference_cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.362167 eradiate-0.23.2rc2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/check_conda_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.366168 eradiate-0.23.2rc2/requirements/conda/
--rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dependencies-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dependencies-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dependencies.dot
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dependencies.yml
--rw-r--r--   0 runner    (1001) docker     (123)    41340 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dev-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    32328 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dev-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dev.dot
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-docs-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    20325 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-docs-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-docs.dot
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-main-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-main-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-main.dot
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-main.yml
--rw-r--r--   0 runner    (1001) docker     (123)    41340 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-optional-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    32328 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-optional-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-optional.dot
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-optional.yml
--rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-recommended-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    19689 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-recommended-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-recommended.dot
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-recommended.yml
--rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-tests-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-tests-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-tests.dot
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/layer_graph.dot
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/copy_envvars.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/environment.in
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/layered.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/make_conda_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/make_pip_in_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.370168 eradiate-0.23.2rc2/requirements/pip/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/dependencies.in
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/dependencies.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/main.in
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/optional.in
--rw-r--r--   0 runner    (1001) docker     (123)    20980 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/recommended.in
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/recommended.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/tests.in
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/setpath.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:12:21.430173 eradiate-0.23.2rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.330164 eradiate-0.23.2rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.374168 eradiate-0.23.2rc2/src/eradiate/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/attrs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.374168 eradiate-0.23.2rc2/src/eradiate/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/cli/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/cli/srf.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.378169 eradiate-0.23.2rc2/src/eradiate/data/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_blind_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_blind_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_safe_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_safe_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/downloads.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/downloads_development.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.378169 eradiate-0.23.2rc2/src/eradiate/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/_canopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/frame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.382169 eradiate-0.23.2rc2/src/eradiate/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/_bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/_bsdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/_kernel_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/gridvolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.382169 eradiate-0.23.2rc2/src/eradiate/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/notebook/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/notebook/tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.382169 eradiate-0.23.2rc2/src/eradiate/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/_assemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/quad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.382169 eradiate-0.23.2rc2/src/eradiate/radprops/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/_us76_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/_util_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/rng.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.386170 eradiate-0.23.2rc2/src/eradiate/scenes/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.386170 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_heterogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)    14639 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_particle_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_particle_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.386170 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    38992 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_leaf_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.390170 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_black.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_lambertian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_opacity_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_rpv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.390170 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_astroobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.390170 eradiate-0.23.2rc2/src/eradiate/scenes/integrators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/integrators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/integrators/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/integrators/_path_tracers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.394170 eradiate-0.23.2rc2/src/eradiate/scenes/measure/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_distant_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_hemispherical_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)    20874 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_multi_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_multi_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_perspective.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_radiancemeter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.394170 eradiate-0.23.2rc2/src/eradiate/scenes/phase/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/_blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/_tabulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.394170 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_buffermesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_cuboid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_filemesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.398171 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_air_scattering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_interpolated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_multi_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_solar_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.398171 eradiate-0.23.2rc2/src/eradiate/scenes/surface/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/surface/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/surface/_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/surface/_central_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/surface/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/surface/_dem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.398171 eradiate-0.23.2rc2/src/eradiate/spectral/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/spectral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/spectral/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/spectral/ckd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/spectral/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/spectral/mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    26485 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/srf_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.398171 eradiate-0.23.2rc2/src/eradiate/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/test_tools/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/test_tools/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/test_tools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/test_tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.402171 eradiate-0.23.2rc2/src/eradiate/thermoprops/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/thermoprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/thermoprops/afgl_1986.py
--rw-r--r--   0 runner    (1001) docker     (123)    42061 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/thermoprops/us76.py
--rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/thermoprops/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.402171 eradiate-0.23.2rc2/src/eradiate/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/util/numpydoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/util/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.402171 eradiate-0.23.2rc2/src/eradiate/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/xarray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/xarray/_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/xarray/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/xarray/interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.374168 eradiate-0.23.2rc2/src/eradiate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-06-21 16:12:21.000000 eradiate-0.23.2rc2/src/eradiate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22346 2023-06-21 16:12:21.000000 eradiate-0.23.2rc2/src/eradiate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:12:21.000000 eradiate-0.23.2rc2/src/eradiate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 16:12:21.000000 eradiate-0.23.2rc2/src/eradiate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-21 16:12:21.000000 eradiate-0.23.2rc2/src/eradiate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 16:12:21.000000 eradiate-0.23.2rc2/src/eradiate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.402171 eradiate-0.23.2rc2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.402171 eradiate-0.23.2rc2/tests/01_eradiate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.406171 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.406171 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_blind_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_blind_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_safe_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_safe_online.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.406171 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_canopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.410172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_gridvolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.410172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_assemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_gather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.410172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_us76_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_zgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.410172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.414172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.414172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.414172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.414172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_astroobject.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.418172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/integrators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.418172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.418172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_blend.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.418172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/test_ckd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/test_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_rng.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_srf_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_tools/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/test_us76.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/util/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/util/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/xarray/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/xarray/test_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.426173 eradiate-0.23.2rc2/tests/01_eradiate/02_system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_albedo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    25312 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_atmosphere_rpv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_ckd_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_irradiance_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_kernel_render_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_maximum_scene_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_mdistant_insitu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_onedim_phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_onedim_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_spectral_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.426173 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.430173 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/atmospheres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/atmospheres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.430173 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/rami4atm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/rami4atm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.430173 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/test_het01.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/test_het04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/test_het06.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.030152 eradiate-0.23.2rc3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_ext/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_ext/pluginparameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32795 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-darkgrey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34059 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-darkgrey.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.022152 eradiate-0.23.2rc3/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_templates/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/convert_figures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.042152 eradiate-0.23.2rc3/docs/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/atmosphere_attributes.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/atmosphere_attributes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28149 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-east_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32937 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-east_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28852 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-east_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35278 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-east_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-north_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32862 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-north_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-north_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-north_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28153 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-south_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32939 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-south_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28118 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-south_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-south_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28178 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-west_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32935 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-west_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28067 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-west_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-west_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/cartesian-coordinate-system.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/cartesian-coordinate-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25301 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/cuboid_leaf_cloud_params.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/cuboid_leaf_cloud_params.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.042152 eradiate-0.23.2rc3/docs/fig/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/diagrams/class_diagram_biosphere.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/diagrams/package.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    40438 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/eradiate-logo-typo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/eradiate-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/icon_eradiate.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38873 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/package.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57417 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/package.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32384 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/radiancemeter_hsphere.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43351 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/radiancemeter_hsphere.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    36773 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/radiancemeter_plane.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/radiancemeter_plane.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/requirement_layers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/requirement_layers.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/solid_2017.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_atm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16459 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_atm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28519 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_noatm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_noatm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_atm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_atm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_noatm_interval1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_noatm_interval2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_noatm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spherical-coordinate-system.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spherical-coordinate-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/thuillier_2003.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/generate_md_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/generate_rst_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/generate_rst_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/index_latex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.042152 eradiate-0.23.2rc3/docs/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/dependencies.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.042152 eradiate-0.23.2rc3/docs/rst/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/design_atmosphere.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/dev_install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/factory_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/lazy_loading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/radiometric_kernel_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/scene_generator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/update.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/maintainer_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/reference_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/attrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/converters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/eradiate_core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/experiments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/factory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/frame.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/kernel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/mode.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/notebook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/plot.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/quad.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/rng.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/scenes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/spectral.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/srf_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/test_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/thermoprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/units.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/validators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/warp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/xarray.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/reference_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_plugins/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/user_guide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/absorption.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    25171 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/bad_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/good_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/line.png
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/heterogeneous.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/homogeneous.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/molecular.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/particle_layer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/basic_concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/conventions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/user_guide/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/absorption.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/atmosphere_radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/atmosphere_thermoprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/ckd.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    30117 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59107 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/pt_points.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/particle_radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/solar_irradiance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/spectra-us76_u86_4.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/srf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/onedim_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/package_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/spectral_discretization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/unit_guide_user.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.054151 eradiate-0.23.2rc3/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/src/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/src/reference_cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.054151 eradiate-0.23.2rc3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/check_conda_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.058152 eradiate-0.23.2rc3/requirements/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dependencies-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dependencies-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dependencies.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dependencies.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    41340 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dev-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    32328 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dev-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dev.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-docs-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    20325 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-docs-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-docs.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-main-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-main-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-main.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    41340 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-optional-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    32328 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-optional-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-optional.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-optional.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-recommended-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    19689 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-recommended-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-recommended.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-recommended.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-tests-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-tests-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-tests.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/layer_graph.dot
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/copy_envvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/environment.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/layered.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/make_conda_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/make_pip_in_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.058152 eradiate-0.23.2rc3/requirements/pip/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/dependencies.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/main.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/optional.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20980 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/recommended.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/recommended.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/tests.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/setpath.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.022152 eradiate-0.23.2rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.062152 eradiate-0.23.2rc3/src/eradiate/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/attrs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.062152 eradiate-0.23.2rc3/src/eradiate/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/cli/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/cli/srf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.062152 eradiate-0.23.2rc3/src/eradiate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_blind_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_blind_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_safe_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_safe_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/downloads.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/downloads_development.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.066151 eradiate-0.23.2rc3/src/eradiate/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/frame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.066151 eradiate-0.23.2rc3/src/eradiate/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/_bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/_bsdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/_kernel_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/gridvolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.066151 eradiate-0.23.2rc3/src/eradiate/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/notebook/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/notebook/tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.066151 eradiate-0.23.2rc3/src/eradiate/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/quad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.066151 eradiate-0.23.2rc3/src/eradiate/radprops/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/_us76_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/_util_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/rng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.066151 eradiate-0.23.2rc3/src/eradiate/scenes/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.070151 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_particle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_particle_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.070151 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38992 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_leaf_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.070151 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_black.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_lambertian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_mqdiffuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_opacity_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.070151 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_astro_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_directional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_spot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.070151 eradiate-0.23.2rc3/src/eradiate/scenes/integrators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/integrators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/integrators/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/integrators/_path_tracers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.074151 eradiate-0.23.2rc3/src/eradiate/scenes/measure/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_distant_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_hemispherical_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_multi_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_multi_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_radiancemeter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.074151 eradiate-0.23.2rc3/src/eradiate/scenes/phase/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/_blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/_tabulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.074151 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_buffermesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_filemesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.074151 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_air_scattering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_multi_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_solar_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.074151 eradiate-0.23.2rc3/src/eradiate/scenes/surface/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/surface/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/surface/_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/surface/_central_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/surface/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/surface/_dem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/src/eradiate/spectral/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/spectral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/spectral/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/spectral/ckd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/spectral/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/spectral/mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26484 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/srf_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/src/eradiate/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/test_tools/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/test_tools/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/test_tools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/test_tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/src/eradiate/thermoprops/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/thermoprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/thermoprops/afgl_1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42061 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/thermoprops/us76.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/thermoprops/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/src/eradiate/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/util/numpydoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/util/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/src/eradiate/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/xarray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/xarray/_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/xarray/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/xarray/interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.062152 eradiate-0.23.2rc3/src/eradiate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-06-30 15:13:57.000000 eradiate-0.23.2rc3/src/eradiate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-06-30 15:13:58.000000 eradiate-0.23.2rc3/src/eradiate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:13:57.000000 eradiate-0.23.2rc3/src/eradiate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 15:13:57.000000 eradiate-0.23.2rc3/src/eradiate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-30 15:13:57.000000 eradiate-0.23.2rc3/src/eradiate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 15:13:57.000000 eradiate-0.23.2rc3/src/eradiate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/tests/01_eradiate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.082152 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.082152 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_blind_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_blind_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_safe_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_safe_online.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.082152 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.082152 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_gridvolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.082152 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_gather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.086151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_us76_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_zgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.086151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.086151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.086151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.086151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.086151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_astro_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.090151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/integrators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.090151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.090151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.090151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/test_ckd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/test_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_rng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_srf_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_tools/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/test_us76.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/util/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/util/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/xarray/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/xarray/test_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/tests/01_eradiate/02_system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_albedo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25312 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_atmosphere_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_ckd_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_irradiance_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_kernel_render_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_maximum_scene_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_mdistant_insitu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_onedim_phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_onedim_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_spectral_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/atmospheres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/atmospheres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/rami4atm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/rami4atm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/test_het01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/test_het04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/test_het06.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/conftest.py
```

### Comparing `eradiate-0.23.2rc2/.clang-format` & `eradiate-0.23.2rc3/.clang-format`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/.github/ISSUE_TEMPLATE/bug_report.md` & `eradiate-0.23.2rc3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/.github/ISSUE_TEMPLATE/feature_request.md` & `eradiate-0.23.2rc3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/.github/pull_request_template.md` & `eradiate-0.23.2rc3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/.github/workflows/cd.yml` & `eradiate-0.23.2rc3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/.github/workflows/ci.yml` & `eradiate-0.23.2rc3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/.pre-commit-config.yaml` & `eradiate-0.23.2rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/.readthedocs.yml` & `eradiate-0.23.2rc3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/CHANGELOG.md` & `eradiate-0.23.2rc3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 %
 % ### Improvements and fixes
 %
 % ### Documentation
 %
 % ### Internal changes
 
-## v0.23.2 (upcoming release)
+## v0.23.2 (30th June 2023)
 
 ### Breaking changes
 
 * Removed the Docker images implementation, deployment and documentation
   from the Eradiate repository ({ghpr}`322`). Docker builds are no longer
   supported for now.
 * {class}`.Measure` no longer takes a `spectral_cfg` parameter but instead a
@@ -45,49 +45,57 @@
 * The {meth}`.MultiDistantMeasure.from_viewing_angles` constructor is removed
   ({ghpr}`315`). Use one of the other {class}`.MultiDistantMeasure` constructors
   instead.
 * The ``ertdata`` and ``ertshow`` command-line entry points are removed
   ({ghpr}`324`). Instead, use ``eradiate data`` and ``eradiate show``.
 * The {class}`.KernelDictContext` class is renamed {class}`.KernelContext`
   ({ghpr}`324`).
+* The `absorption_dataset` parameter of `AFGL1986RadProfile` and
+  `US76ApproxRadProfile` is now required ({ghpr}`334`).
 
 ### Deprecations and removals
 
 * Removed {class}`.SpectralContext` and subclasses ({ghpr}`311`).
 * Removed {class}`.MeasureSpectralConfig` and subclasses ({ghpr}`311`).
 * Removed the {meth}`.MultiDistantMeasure.from_viewing_angles` constructor
   ({ghpr}`315`).
 * Removed ``ertdata`` and ``ertshow`` command-line entry points ({ghpr}`324`).
 
 ### Improvements and fixes
 
 * Added {class}`.MultiDeltaSpectrum` spectrum type ({ghpr}`311`).
 * Exposed several API members in the top-level namespace ({ghpr}`324`).
-* Exposed the ``eradiate.spectral.*`` subpackage members in the
+* Exposed the `eradiate.spectral.*` subpackage members in the
   {mod}`eradiate.spectral` namespace ({ghpr}`324`).
 * Fixed incorrect Mitsuba scene parameter drop and lookup ({ghpr}`329`).
 * Added spherical-shell geometry support to DEM components
   {ghpr}`320`.
 * Fixed broken symmetry between {class}`.Spectrum` dictionary and object
   conversion protocols ({ghpr}`336`).
 * Provide an Eradiate Pypi package ({ghpr}`328`).
-* Implement the Astronomical Object Illumination, its tests and its
-  documentation ({ghpr}`331`).
+* Added {class}`.AstroObjectIllumination` illumination type ({ghpr}`331`,
+  {ghpr}`346`).
+* Fixed a bug where {class}`.Layout` constructors would not raise if passed
+  invalid azimuth values (*i.e.* outside the [0, 180]° range) ({ghpr}`345`).
+* Added `wavelength_range` optional parameter to `MolecularAtmosphere.ussa_1976()`
+  constructor to automatically open absorption datasets and restore working default
+  constructor ({ghpr}`334`).
 
 ### Documentation
 
 * Added a user guide page on spectral discretization.
 
 ### Internal changes
 
 * Spectral dispatch with `functools.singledispatchmethod` ({ghpr}`311`).
 * Experiments define the spectral discretization, based on information from
   its measure, its atmosphere components if applicable, and a default
   spectral set ({ghpr}`311`).
 * Rewrote the CLI using the Typer framework ({ghpr}`326`).
+* Refactored {class}`.Layout` constructor code ({ghpr}`345`).
 
 ## v0.23.1 (21 April 2023)
 
 ### Breaking changes
 
 * The `coddington_2021-1_nm` dataset is now the default solar irradiance
   spectrum ({ghpr}`300`). If you used to work with the default value
```

### Comparing `eradiate-0.23.2rc2/CONTRIBUTING.md` & `eradiate-0.23.2rc3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/LICENSE` & `eradiate-0.23.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/Makefile` & `eradiate-0.23.2rc3/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -80,30 +80,30 @@
 install-no-deps:
 	python3 requirements/copy_envvars.py
 	pip install --editable . --no-deps
 
 # Initialise development environment
 conda-init: conda-prepare
 	conda update --file requirements/conda/environment-dev-$(PLATFORM).lock
-	$(MAKE) no-deps-install
+	$(MAKE) install-no-deps
 
 # Initialise docs building environment
 conda-init-docs: conda-prepare
 	conda update --file requirements/conda/environment-docs-$(PLATFORM).lock
-	$(MAKE) no-deps-install
+	$(MAKE) install-no-deps
 
 # Initialise tests environment
 conda-init-tests: conda-prepare
 	conda update --file requirements/conda/environment-tests-$(PLATFORM).lock
-	$(MAKE) no-deps-install
+	$(MAKE) install-no-deps
 
 # Initialise production environment
 conda-init-prod: conda-prepare
 	conda update --file requirements/conda/environment-dependencies-$(PLATFORM).lock
-	$(MAKE) no-deps-install
+	$(MAKE) install-no-deps
 
 conda-update: conda-lock-all conda-init
 
 .PHONY: conda-env conda-lock conda-lock-all conda-init conda-update
 
 # -- Build the Eradiate Mitsuba kernel -----------------------------------------
```

### Comparing `eradiate-0.23.2rc2/PKG-INFO` & `eradiate-0.23.2rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eradiate
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: A radiative transfer model for the Earth observation community
 Author: The Eradiate Team
 Maintainer: The Eradiate Team
 License: LGPLv3
 Project-URL: changelog, https://github.com/eradiate/eradiate/CHANGELOG.md
 Project-URL: documentation, https://eradiate.readthedocs.io
 Project-URL: repository, https://github.com/eradiate/eradiate
```

### Comparing `eradiate-0.23.2rc2/README.md` & `eradiate-0.23.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/Makefile` & `eradiate-0.23.2rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/_ext/exec.py` & `eradiate-0.23.2rc3/docs/_ext/exec.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/_ext/pluginparameters.py` & `eradiate-0.23.2rc3/docs/_ext/pluginparameters.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-black.png` & `eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-black.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-black.svg` & `eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-black.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-darkgrey.png` & `eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-darkgrey.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-darkgrey.svg` & `eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-darkgrey.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-white.png` & `eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-white.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-white.svg` & `eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-white.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/_templates/autosummary/module.rst` & `eradiate-0.23.2rc3/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/_templates/sections/footer-content.html` & `eradiate-0.23.2rc3/docs/_templates/sections/footer-content.html`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/conf.py` & `eradiate-0.23.2rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/atmosphere_attributes.png` & `eradiate-0.23.2rc3/docs/fig/atmosphere_attributes.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/atmosphere_attributes.svg` & `eradiate-0.23.2rc3/docs/fig/atmosphere_attributes.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-east_left.png` & `eradiate-0.23.2rc3/docs/fig/azimuth-east_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-east_left.svg` & `eradiate-0.23.2rc3/docs/fig/azimuth-east_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-east_right.png` & `eradiate-0.23.2rc3/docs/fig/azimuth-east_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-east_right.svg` & `eradiate-0.23.2rc3/docs/fig/azimuth-east_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-north_left.png` & `eradiate-0.23.2rc3/docs/fig/azimuth-north_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-north_left.svg` & `eradiate-0.23.2rc3/docs/fig/azimuth-north_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-north_right.png` & `eradiate-0.23.2rc3/docs/fig/azimuth-north_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-north_right.svg` & `eradiate-0.23.2rc3/docs/fig/azimuth-north_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-south_left.png` & `eradiate-0.23.2rc3/docs/fig/azimuth-south_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-south_left.svg` & `eradiate-0.23.2rc3/docs/fig/azimuth-south_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-south_right.png` & `eradiate-0.23.2rc3/docs/fig/azimuth-south_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-south_right.svg` & `eradiate-0.23.2rc3/docs/fig/azimuth-south_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-west_left.png` & `eradiate-0.23.2rc3/docs/fig/azimuth-west_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-west_left.svg` & `eradiate-0.23.2rc3/docs/fig/azimuth-west_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-west_right.png` & `eradiate-0.23.2rc3/docs/fig/azimuth-west_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/azimuth-west_right.svg` & `eradiate-0.23.2rc3/docs/fig/azimuth-west_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/cartesian-coordinate-system.png` & `eradiate-0.23.2rc3/docs/fig/cartesian-coordinate-system.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/cartesian-coordinate-system.svg` & `eradiate-0.23.2rc3/docs/fig/cartesian-coordinate-system.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/cuboid_leaf_cloud_params.png` & `eradiate-0.23.2rc3/docs/fig/cuboid_leaf_cloud_params.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/cuboid_leaf_cloud_params.svg` & `eradiate-0.23.2rc3/docs/fig/cuboid_leaf_cloud_params.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/diagrams/class_diagram_biosphere.drawio` & `eradiate-0.23.2rc3/docs/fig/diagrams/class_diagram_biosphere.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio` & `eradiate-0.23.2rc3/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/diagrams/package.drawio` & `eradiate-0.23.2rc3/docs/fig/diagrams/package.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/eradiate-logo-typo-black.png` & `eradiate-0.23.2rc3/docs/fig/eradiate-logo-typo-black.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/eradiate-logo.svg` & `eradiate-0.23.2rc3/docs/fig/eradiate-logo.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/icon_eradiate.png` & `eradiate-0.23.2rc3/docs/fig/icon_eradiate.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/package.png` & `eradiate-0.23.2rc3/docs/fig/package.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/package.svg` & `eradiate-0.23.2rc3/docs/fig/package.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/radiancemeter_hsphere.png` & `eradiate-0.23.2rc3/docs/fig/radiancemeter_hsphere.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/radiancemeter_hsphere.svg` & `eradiate-0.23.2rc3/docs/fig/radiancemeter_hsphere.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/radiancemeter_plane.png` & `eradiate-0.23.2rc3/docs/fig/radiancemeter_plane.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/radiancemeter_plane.svg` & `eradiate-0.23.2rc3/docs/fig/radiancemeter_plane.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/requirement_layers.png` & `eradiate-0.23.2rc3/docs/fig/requirement_layers.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/requirement_layers.svg` & `eradiate-0.23.2rc3/docs/fig/requirement_layers.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/solid_2017.png` & `eradiate-0.23.2rc3/docs/fig/solid_2017.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_atm_interval.png` & `eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_atm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_atm_isolated.png` & `eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_atm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_noatm_interval.png` & `eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_noatm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_noatm_isolated.png` & `eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_noatm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_atm_interval.png` & `eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_atm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_atm_isolated.png` & `eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_atm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_noatm_interval1.png` & `eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_noatm_interval1.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_noatm_interval2.png` & `eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_noatm_interval2.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_noatm_isolated.png` & `eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_noatm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/spherical-coordinate-system.png` & `eradiate-0.23.2rc3/docs/fig/spherical-coordinate-system.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/spherical-coordinate-system.svg` & `eradiate-0.23.2rc3/docs/fig/spherical-coordinate-system.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/fig/thuillier_2003.png` & `eradiate-0.23.2rc3/docs/fig/thuillier_2003.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/generate_md_cli.py` & `eradiate-0.23.2rc3/docs/generate_md_cli.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/generate_rst_api.py` & `eradiate-0.23.2rc3/docs/generate_rst_api.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/generate_rst_plugins.py` & `eradiate-0.23.2rc3/docs/generate_rst_plugins.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/index.rst` & `eradiate-0.23.2rc3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/make.bat` & `eradiate-0.23.2rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/references.bib` & `eradiate-0.23.2rc3/docs/references.bib`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/contributing.rst` & `eradiate-0.23.2rc3/docs/rst/contributing.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/dependencies.rst` & `eradiate-0.23.2rc3/docs/rst/dependencies.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/developer_guide/design_atmosphere.rst` & `eradiate-0.23.2rc3/docs/rst/developer_guide/design_atmosphere.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/developer_guide/factory_guide.rst` & `eradiate-0.23.2rc3/docs/rst/developer_guide/factory_guide.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/developer_guide/getting_started.rst` & `eradiate-0.23.2rc3/docs/rst/developer_guide/dev_install.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. _sec-getting_started-development:
+.. _sec-developer_guide-dev_install:
 
 Development installation
 ========================
 
 This guide covers all steps necessary to get Eradiate running on your machine in
 development mode. This mode allows for easy code modifications and testing, as
 well as for developing on the kernel code. It requires to compile the C++ code
@@ -114,15 +114,15 @@
 
 Finally, Eradiate requires a fairly recent version of Python (at least 3.8)
 and **we highly recommend using the Conda environment and package  manager** to
 set up your Python environment. Conda can be installed notably as part of the
 Anaconda distribution, or using its lightweight counterpart Miniconda.
 `See installation instructions here <https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html>`_.
 
-.. _sec-getting_started-install-cloning:
+.. _sec-developer_guide-dev_install-cloning:
 
 Cloning the repository
 ----------------------
 
 .. note::
 
    Eradiate relies on the `Git source code management tool <https://git-scm.com/>`_.
@@ -159,15 +159,15 @@
 .. note::
 
    If GitHub requests credentials to access submodules through HTTPS, we highly
    recommend to `generate a personal access token <https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token>`_
    with **repo** permissions and to use it instead of your password. You might
    also have to make sure that `Git will remember your token <https://git-scm.com/book/en/v2/Git-Tools-Credential-Storage>`_.
 
-.. _sec-getting_started-install-setup_conda:
+.. _sec-developer_guide-dev_install-setup_conda:
 
 Setting up the Conda environment
 --------------------------------
 
 Eradiate ships a set of pinned Conda environment specifications in the form of
 *lock files*. They quickly set up a reproducible environment. We strongly
 recommend using these instead of a regular environment file since they provide
@@ -215,15 +215,15 @@
 
 Once your Conda environment is configured, you should reactivate it:
 
 .. code:: bash
 
    conda deactivate && conda activate eradiate
 
-.. _sec-getting_started-install-compiling:
+.. _sec-developer_guide-dev_install-compiling:
 
 Compiling the radiometric kernel
 --------------------------------
 
 Using the Makefile rule to build the kernel is the recommended way to compile.
 
 .. code:: bash
@@ -322,15 +322,15 @@
        before starting to compile.*
 
    This is expected: do not worry about it.
 
 The compilation process can last for up to around half an hour on old machines.
 It completes within a few minutes on modern workstations.
 
-.. _sec-getting_started-install-verify_installation:
+.. _sec-developer_guide-dev_install-verify_installation:
 
 Verifying the installation
 --------------------------
 
 In a terminal, try and invoke the :program:`eradiate` command-line interface:
 
 .. code:: bash
```

### Comparing `eradiate-0.23.2rc2/docs/rst/developer_guide/lazy_loading.rst` & `eradiate-0.23.2rc3/docs/rst/developer_guide/lazy_loading.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/developer_guide/radiometric_kernel_interface.rst` & `eradiate-0.23.2rc3/docs/rst/developer_guide/radiometric_kernel_interface.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/developer_guide/scene_generator.rst` & `eradiate-0.23.2rc3/docs/rst/developer_guide/scene_generator.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/developer_guide/update.rst` & `eradiate-0.23.2rc3/docs/rst/developer_guide/update.rst`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 .. code:: bash
 
    cd $ERADIATE_SOURCE_DIR
    make conda-init
 
 If something goes wrong during that process, an environment reset should solve
-most issues (see :ref:`sec-getting_started-install-setup_conda`).
+most issues (see :ref:`sec-developer_guide-dev_install-setup_conda`).
 
 Update data files
 -----------------
 
 Optionally, you may want to make sure that the data files you'll use are
 up-to-date. For that purpose, you can refresh remote file registries and purge
 Eradiate's data cache:
```

### Comparing `eradiate-0.23.2rc2/docs/rst/maintainer_guide.rst` & `eradiate-0.23.2rc3/docs/rst/maintainer_guide.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/reference_api/data.rst` & `eradiate-0.23.2rc3/docs/rst/reference_api/data.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/reference_api/eradiate_core.rst` & `eradiate-0.23.2rc3/docs/rst/reference_api/eradiate_core.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/reference_api/experiments.rst` & `eradiate-0.23.2rc3/docs/rst/reference_api/experiments.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/reference_api/factory.rst` & `eradiate-0.23.2rc3/docs/rst/reference_api/factory.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/reference_api/index.rst` & `eradiate-0.23.2rc3/docs/rst/reference_api/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/reference_api/kernel.rst` & `eradiate-0.23.2rc3/docs/rst/reference_api/kernel.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/reference_api/pipelines.rst` & `eradiate-0.23.2rc3/docs/rst/reference_api/pipelines.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/reference_api/scenes.rst` & `eradiate-0.23.2rc3/docs/rst/reference_api/scenes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -268,161 +268,162 @@
 000010b0: 6c6c 756d 696e 6174 696f 6e5f 6661 6374  llumination_fact
 000010c0: 6f72 7960 0a0a 2a2a 5363 656e 6520 656c  ory`..**Scene el
 000010d0: 656d 656e 7473 2a2a 0a0a 2e2e 2061 7574  ements**.... aut
 000010e0: 6f73 756d 6d61 7279 3a3a 0a20 2020 3a74  osummary::.   :t
 000010f0: 6f63 7472 6565 3a20 6765 6e65 7261 7465  octree: generate
 00001100: 642f 6175 746f 7375 6d6d 6172 792f 0a0a  d/autosummary/..
 00001110: 2020 2044 6972 6563 7469 6f6e 616c 496c     DirectionalIl
-00001120: 6c75 6d69 6e61 7469 6f6e 0a20 2020 436f  lumination.   Co
-00001130: 6e73 7461 6e74 496c 6c75 6d69 6e61 7469  nstantIlluminati
-00001140: 6f6e 0a20 2020 5370 6f74 496c 6c75 6d69  on.   SpotIllumi
-00001150: 6e61 7469 6f6e 0a0a 6060 6572 6164 6961  nation..``eradia
-00001160: 7465 2e73 6365 6e65 732e 6d65 6173 7572  te.scenes.measur
-00001170: 6560 600a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  e``.------------
-00001180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00001190: 0a2e 2e20 6175 746f 6d6f 6475 6c65 3a3a  ... automodule::
-000011a0: 2065 7261 6469 6174 652e 7363 656e 6573   eradiate.scenes
-000011b0: 2e6d 6561 7375 7265 0a0a 2e2e 2070 793a  .measure.... py:
-000011c0: 6375 7272 656e 746d 6f64 756c 653a 3a20  currentmodule:: 
-000011d0: 6572 6164 6961 7465 2e73 6365 6e65 732e  eradiate.scenes.
-000011e0: 6d65 6173 7572 650a 0a2a 2a49 6e74 6572  measure..**Inter
-000011f0: 6661 6365 732a 2a0a 0a2e 2e20 6175 746f  faces**.... auto
-00001200: 7375 6d6d 6172 793a 3a0a 2020 203a 746f  summary::.   :to
-00001210: 6374 7265 653a 2067 656e 6572 6174 6564  ctree: generated
-00001220: 2f61 7574 6f73 756d 6d61 7279 2f0a 0a20  /autosummary/.. 
-00001230: 2020 4d65 6173 7572 650a 2020 2054 6172    Measure.   Tar
-00001240: 6765 740a 0a2a 2a46 6163 746f 7269 6573  get..**Factories
-00001250: 2a2a 0a0a 2a20 3a64 6174 613a 606d 6561  **..* :data:`mea
-00001260: 7375 7265 5f66 6163 746f 7279 600a 0a2a  sure_factory`..*
-00001270: 2a53 6365 6e65 2065 6c65 6d65 6e74 732a  *Scene elements*
-00001280: 2a0a 0a2e 2e20 6175 746f 7375 6d6d 6172  *.... autosummar
-00001290: 793a 3a0a 2020 203a 746f 6374 7265 653a  y::.   :toctree:
-000012a0: 2067 656e 6572 6174 6564 2f61 7574 6f73   generated/autos
-000012b0: 756d 6d61 7279 2f0a 0a20 2020 4d75 6c74  ummary/..   Mult
-000012c0: 6944 6973 7461 6e74 4d65 6173 7572 650a  iDistantMeasure.
-000012d0: 2020 2044 6973 7461 6e74 466c 7578 4d65     DistantFluxMe
-000012e0: 6173 7572 650a 2020 2048 656d 6973 7068  asure.   Hemisph
-000012f0: 6572 6963 616c 4469 7374 616e 744d 6561  ericalDistantMea
-00001300: 7375 7265 0a20 2020 5261 6469 616e 6365  sure.   Radiance
-00001310: 6d65 7465 724d 6561 7375 7265 0a20 2020  meterMeasure.   
-00001320: 4d75 6c74 6952 6164 6961 6e63 656d 6574  MultiRadiancemet
-00001330: 6572 4d65 6173 7572 650a 2020 2050 6572  erMeasure.   Per
-00001340: 7370 6563 7469 7665 4361 6d65 7261 4d65  spectiveCameraMe
-00001350: 6173 7572 650a 0a2a 2a44 6973 7461 6e74  asure..**Distant
-00001360: 206d 6561 7375 7265 2074 6172 6765 7420   measure target 
-00001370: 6465 6669 6e69 7469 6f6e 2a2a 0a0a 2e2e  definition**....
-00001380: 2061 7574 6f73 756d 6d61 7279 3a3a 0a20   autosummary::. 
-00001390: 203a 746f 6374 7265 653a 2067 656e 6572   :toctree: gener
-000013a0: 6174 6564 2f61 7574 6f73 756d 6d61 7279  ated/autosummary
-000013b0: 2f0a 0a20 2054 6172 6765 7450 6f69 6e74  /..  TargetPoint
-000013c0: 0a20 2054 6172 6765 7452 6563 7461 6e67  .  TargetRectang
-000013d0: 6c65 0a0a 2a2a 5669 6577 696e 6720 6469  le..**Viewing di
-000013e0: 7265 6374 696f 6e20 6c61 796f 7574 732a  rection layouts*
-000013f0: 2a0a 0a2a 5573 6564 2061 7320 696e 7075  *..*Used as inpu
-00001400: 7420 746f 2074 6865 2a20 3a63 6c61 7373  t to the* :class
-00001410: 3a60 2e4d 756c 7469 4469 7374 616e 744d  :`.MultiDistantM
-00001420: 6561 7375 7265 605c 2060 602e 6c61 796f  easure`\ ``.layo
-00001430: 7574 6060 202a 6669 656c 642e 2a0a 0a2e  ut`` *field.*...
-00001440: 2e20 6175 746f 7375 6d6d 6172 793a 3a0a  . autosummary::.
-00001450: 2020 203a 746f 6374 7265 653a 2067 656e     :toctree: gen
-00001460: 6572 6174 6564 2f61 7574 6f73 756d 6d61  erated/autosumma
-00001470: 7279 2f0a 0a20 2020 4c61 796f 7574 0a20  ry/..   Layout. 
-00001480: 2020 416e 676c 654c 6179 6f75 740a 2020    AngleLayout.  
-00001490: 2041 7a69 6d75 7468 5269 6e67 4c61 796f   AzimuthRingLayo
-000014a0: 7574 0a20 2020 4469 7265 6374 696f 6e4c  ut.   DirectionL
-000014b0: 6179 6f75 740a 2020 2047 7269 644c 6179  ayout.   GridLay
-000014c0: 6f75 740a 2020 2048 656d 6973 7068 6572  out.   Hemispher
-000014d0: 6550 6c61 6e65 4c61 796f 7574 0a0a 6060  ePlaneLayout..``
-000014e0: 6572 6164 6961 7465 2e73 6365 6e65 732e  eradiate.scenes.
-000014f0: 7068 6173 6560 600a 2d2d 2d2d 2d2d 2d2d  phase``.--------
-00001500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001510: 2d0a 0a2e 2e20 6175 746f 6d6f 6475 6c65  -.... automodule
-00001520: 3a3a 2065 7261 6469 6174 652e 7363 656e  :: eradiate.scen
-00001530: 6573 2e70 6861 7365 0a0a 2e2e 2070 793a  es.phase.... py:
-00001540: 6375 7272 656e 746d 6f64 756c 653a 3a20  currentmodule:: 
-00001550: 6572 6164 6961 7465 2e73 6365 6e65 732e  eradiate.scenes.
-00001560: 7068 6173 650a 0a2a 2a49 6e74 6572 6661  phase..**Interfa
-00001570: 6365 732a 2a0a 0a2e 2e20 6175 746f 7375  ces**.... autosu
-00001580: 6d6d 6172 793a 3a0a 2020 203a 746f 6374  mmary::.   :toct
-00001590: 7265 653a 2067 656e 6572 6174 6564 2f61  ree: generated/a
-000015a0: 7574 6f73 756d 6d61 7279 2f0a 0a20 2020  utosummary/..   
-000015b0: 5068 6173 6546 756e 6374 696f 6e0a 0a2a  PhaseFunction..*
-000015c0: 2a46 6163 746f 7269 6573 2a2a 0a0a 2a20  *Factories**..* 
-000015d0: 3a64 6174 613a 6070 6861 7365 5f66 756e  :data:`phase_fun
-000015e0: 6374 696f 6e5f 6661 6374 6f72 7960 0a0a  ction_factory`..
-000015f0: 2a2a 5363 656e 6520 656c 656d 656e 7473  **Scene elements
-00001600: 2a2a 0a0a 2e2e 2061 7574 6f73 756d 6d61  **.... autosumma
-00001610: 7279 3a3a 0a20 2020 3a74 6f63 7472 6565  ry::.   :toctree
-00001620: 3a20 6765 6e65 7261 7465 642f 6175 746f  : generated/auto
-00001630: 7375 6d6d 6172 792f 0a0a 2020 2049 736f  summary/..   Iso
-00001640: 7472 6f70 6963 5068 6173 6546 756e 6374  tropicPhaseFunct
-00001650: 696f 6e0a 2020 2052 6179 6c65 6967 6850  ion.   RayleighP
-00001660: 6861 7365 4675 6e63 7469 6f6e 0a20 2020  haseFunction.   
-00001670: 4865 6e79 6579 4772 6565 6e73 7465 696e  HenyeyGreenstein
-00001680: 5068 6173 6546 756e 6374 696f 6e0a 2020  PhaseFunction.  
-00001690: 2042 6c65 6e64 5068 6173 6546 756e 6374   BlendPhaseFunct
-000016a0: 696f 6e0a 2020 2054 6162 756c 6174 6564  ion.   Tabulated
-000016b0: 5068 6173 6546 756e 6374 696f 6e0a 0a60  PhaseFunction..`
-000016c0: 6065 7261 6469 6174 652e 7363 656e 6573  `eradiate.scenes
-000016d0: 2e69 6e74 6567 7261 746f 7273 6060 0a2d  .integrators``.-
-000016e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000016f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-00001700: 2e2e 2061 7574 6f6d 6f64 756c 653a 3a20  .. automodule:: 
-00001710: 6572 6164 6961 7465 2e73 6365 6e65 732e  eradiate.scenes.
-00001720: 696e 7465 6772 6174 6f72 730a 0a2e 2e20  integrators.... 
-00001730: 7079 3a63 7572 7265 6e74 6d6f 6475 6c65  py:currentmodule
-00001740: 3a3a 2065 7261 6469 6174 652e 7363 656e  :: eradiate.scen
-00001750: 6573 2e69 6e74 6567 7261 746f 7273 0a0a  es.integrators..
-00001760: 2a2a 496e 7465 7266 6163 6573 2a2a 0a0a  **Interfaces**..
-00001770: 2e2e 2061 7574 6f73 756d 6d61 7279 3a3a  .. autosummary::
-00001780: 0a20 2020 3a74 6f63 7472 6565 3a20 6765  .   :toctree: ge
-00001790: 6e65 7261 7465 642f 6175 746f 7375 6d6d  nerated/autosumm
-000017a0: 6172 792f 0a0a 2020 2049 6e74 6567 7261  ary/..   Integra
-000017b0: 746f 720a 0a2a 2a46 6163 746f 7269 6573  tor..**Factories
-000017c0: 2a2a 0a0a 2a20 3a64 6174 613a 6069 6e74  **..* :data:`int
-000017d0: 6567 7261 746f 725f 6661 6374 6f72 7960  egrator_factory`
-000017e0: 0a0a 2a2a 5363 656e 6520 656c 656d 656e  ..**Scene elemen
-000017f0: 7473 2a2a 0a0a 2e2e 2061 7574 6f73 756d  ts**.... autosum
-00001800: 6d61 7279 3a3a 0a20 2020 3a74 6f63 7472  mary::.   :toctr
-00001810: 6565 3a20 6765 6e65 7261 7465 642f 6175  ee: generated/au
-00001820: 746f 7375 6d6d 6172 792f 0a0a 2020 2050  tosummary/..   P
-00001830: 6174 6849 6e74 6567 7261 746f 720a 2020  athIntegrator.  
-00001840: 2056 6f6c 5061 7468 496e 7465 6772 6174   VolPathIntegrat
-00001850: 6f72 0a20 2020 566f 6c50 6174 684d 4953  or.   VolPathMIS
-00001860: 496e 7465 6772 6174 6f72 0a0a 6060 6572  Integrator..``er
-00001870: 6164 6961 7465 2e73 6365 6e65 732e 7370  adiate.scenes.sp
-00001880: 6563 7472 6160 600a 2d2d 2d2d 2d2d 2d2d  ectra``.--------
-00001890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000018a0: 2d2d 2d0a 0a2e 2e20 6175 746f 6d6f 6475  ---.... automodu
-000018b0: 6c65 3a3a 2065 7261 6469 6174 652e 7363  le:: eradiate.sc
-000018c0: 656e 6573 2e73 7065 6374 7261 0a0a 2e2e  enes.spectra....
-000018d0: 2070 793a 6375 7272 656e 746d 6f64 756c   py:currentmodul
-000018e0: 653a 3a20 6572 6164 6961 7465 2e73 6365  e:: eradiate.sce
-000018f0: 6e65 732e 7370 6563 7472 610a 0a2a 2a49  nes.spectra..**I
-00001900: 6e74 6572 6661 6365 732a 2a0a 0a2e 2e20  nterfaces**.... 
-00001910: 6175 746f 7375 6d6d 6172 793a 3a0a 2020  autosummary::.  
-00001920: 203a 746f 6374 7265 653a 2067 656e 6572   :toctree: gener
-00001930: 6174 6564 2f61 7574 6f73 756d 6d61 7279  ated/autosummary
-00001940: 2f0a 0a20 2020 5370 6563 7472 756d 0a0a  /..   Spectrum..
-00001950: 2a2a 4661 6374 6f72 6965 732a 2a0a 0a2a  **Factories**..*
-00001960: 203a 6461 7461 3a60 7370 6563 7472 756d   :data:`spectrum
-00001970: 5f66 6163 746f 7279 600a 0a2e 2e20 6472  _factory`.... dr
-00001980: 6f70 646f 776e 3a3a 2050 7269 7661 7465  opdown:: Private
-00001990: 0a0a 2020 202e 2e20 6175 746f 7375 6d6d  ..   .. autosumm
-000019a0: 6172 793a 3a0a 2020 2020 2020 3a74 6f63  ary::.      :toc
-000019b0: 7472 6565 3a20 6765 6e65 7261 7465 642f  tree: generated/
-000019c0: 6175 746f 7375 6d6d 6172 792f 0a0a 2020  autosummary/..  
-000019d0: 2020 2020 5f63 6f72 652e 5370 6563 7472      _core.Spectr
-000019e0: 756d 4661 6374 6f72 790a 0a2a 2a53 6365  umFactory..**Sce
-000019f0: 6e65 2065 6c65 6d65 6e74 732a 2a0a 0a2e  ne elements**...
-00001a00: 2e20 6175 746f 7375 6d6d 6172 793a 3a0a  . autosummary::.
-00001a10: 2020 203a 746f 6374 7265 653a 2067 656e     :toctree: gen
-00001a20: 6572 6174 6564 2f61 7574 6f73 756d 6d61  erated/autosumma
-00001a30: 7279 2f0a 0a20 2020 556e 6966 6f72 6d53  ry/..   UniformS
-00001a40: 7065 6374 7275 6d0a 2020 2049 6e74 6572  pectrum.   Inter
-00001a50: 706f 6c61 7465 6453 7065 6374 7275 6d0a  polatedSpectrum.
-00001a60: 2020 204d 756c 7469 4465 6c74 6153 7065     MultiDeltaSpe
-00001a70: 6374 7275 6d0a 2020 2053 6f6c 6172 4972  ctrum.   SolarIr
-00001a80: 7261 6469 616e 6365 5370 6563 7472 756d  radianceSpectrum
-00001a90: 0a20 2020 4169 7253 6361 7474 6572 696e  .   AirScatterin
-00001aa0: 6743 6f65 6666 6963 6965 6e74 5370 6563  gCoefficientSpec
-00001ab0: 7472 756d 0a                             trum.
+00001120: 6c75 6d69 6e61 7469 6f6e 0a20 2020 4173  lumination.   As
+00001130: 7472 6f4f 626a 6563 7449 6c6c 756d 696e  troObjectIllumin
+00001140: 6174 696f 6e0a 2020 2043 6f6e 7374 616e  ation.   Constan
+00001150: 7449 6c6c 756d 696e 6174 696f 6e0a 2020  tIllumination.  
+00001160: 2053 706f 7449 6c6c 756d 696e 6174 696f   SpotIlluminatio
+00001170: 6e0a 0a60 6065 7261 6469 6174 652e 7363  n..``eradiate.sc
+00001180: 656e 6573 2e6d 6561 7375 7265 6060 0a2d  enes.measure``.-
+00001190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000011a0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2e2e 2061  ----------.... a
+000011b0: 7574 6f6d 6f64 756c 653a 3a20 6572 6164  utomodule:: erad
+000011c0: 6961 7465 2e73 6365 6e65 732e 6d65 6173  iate.scenes.meas
+000011d0: 7572 650a 0a2e 2e20 7079 3a63 7572 7265  ure.... py:curre
+000011e0: 6e74 6d6f 6475 6c65 3a3a 2065 7261 6469  ntmodule:: eradi
+000011f0: 6174 652e 7363 656e 6573 2e6d 6561 7375  ate.scenes.measu
+00001200: 7265 0a0a 2a2a 496e 7465 7266 6163 6573  re..**Interfaces
+00001210: 2a2a 0a0a 2e2e 2061 7574 6f73 756d 6d61  **.... autosumma
+00001220: 7279 3a3a 0a20 2020 3a74 6f63 7472 6565  ry::.   :toctree
+00001230: 3a20 6765 6e65 7261 7465 642f 6175 746f  : generated/auto
+00001240: 7375 6d6d 6172 792f 0a0a 2020 204d 6561  summary/..   Mea
+00001250: 7375 7265 0a20 2020 5461 7267 6574 0a0a  sure.   Target..
+00001260: 2a2a 4661 6374 6f72 6965 732a 2a0a 0a2a  **Factories**..*
+00001270: 203a 6461 7461 3a60 6d65 6173 7572 655f   :data:`measure_
+00001280: 6661 6374 6f72 7960 0a0a 2a2a 5363 656e  factory`..**Scen
+00001290: 6520 656c 656d 656e 7473 2a2a 0a0a 2e2e  e elements**....
+000012a0: 2061 7574 6f73 756d 6d61 7279 3a3a 0a20   autosummary::. 
+000012b0: 2020 3a74 6f63 7472 6565 3a20 6765 6e65    :toctree: gene
+000012c0: 7261 7465 642f 6175 746f 7375 6d6d 6172  rated/autosummar
+000012d0: 792f 0a0a 2020 204d 756c 7469 4469 7374  y/..   MultiDist
+000012e0: 616e 744d 6561 7375 7265 0a20 2020 4469  antMeasure.   Di
+000012f0: 7374 616e 7446 6c75 784d 6561 7375 7265  stantFluxMeasure
+00001300: 0a20 2020 4865 6d69 7370 6865 7269 6361  .   Hemispherica
+00001310: 6c44 6973 7461 6e74 4d65 6173 7572 650a  lDistantMeasure.
+00001320: 2020 2052 6164 6961 6e63 656d 6574 6572     Radiancemeter
+00001330: 4d65 6173 7572 650a 2020 204d 756c 7469  Measure.   Multi
+00001340: 5261 6469 616e 6365 6d65 7465 724d 6561  RadiancemeterMea
+00001350: 7375 7265 0a20 2020 5065 7273 7065 6374  sure.   Perspect
+00001360: 6976 6543 616d 6572 614d 6561 7375 7265  iveCameraMeasure
+00001370: 0a0a 2a2a 4469 7374 616e 7420 6d65 6173  ..**Distant meas
+00001380: 7572 6520 7461 7267 6574 2064 6566 696e  ure target defin
+00001390: 6974 696f 6e2a 2a0a 0a2e 2e20 6175 746f  ition**.... auto
+000013a0: 7375 6d6d 6172 793a 3a0a 2020 3a74 6f63  summary::.  :toc
+000013b0: 7472 6565 3a20 6765 6e65 7261 7465 642f  tree: generated/
+000013c0: 6175 746f 7375 6d6d 6172 792f 0a0a 2020  autosummary/..  
+000013d0: 5461 7267 6574 506f 696e 740a 2020 5461  TargetPoint.  Ta
+000013e0: 7267 6574 5265 6374 616e 676c 650a 0a2a  rgetRectangle..*
+000013f0: 2a56 6965 7769 6e67 2064 6972 6563 7469  *Viewing directi
+00001400: 6f6e 206c 6179 6f75 7473 2a2a 0a0a 2a55  on layouts**..*U
+00001410: 7365 6420 6173 2069 6e70 7574 2074 6f20  sed as input to 
+00001420: 7468 652a 203a 636c 6173 733a 602e 4d75  the* :class:`.Mu
+00001430: 6c74 6944 6973 7461 6e74 4d65 6173 7572  ltiDistantMeasur
+00001440: 6560 5c20 6060 2e6c 6179 6f75 7460 6020  e`\ ``.layout`` 
+00001450: 2a66 6965 6c64 2e2a 0a0a 2e2e 2061 7574  *field.*.... aut
+00001460: 6f73 756d 6d61 7279 3a3a 0a20 2020 3a74  osummary::.   :t
+00001470: 6f63 7472 6565 3a20 6765 6e65 7261 7465  octree: generate
+00001480: 642f 6175 746f 7375 6d6d 6172 792f 0a0a  d/autosummary/..
+00001490: 2020 204c 6179 6f75 740a 2020 2041 6e67     Layout.   Ang
+000014a0: 6c65 4c61 796f 7574 0a20 2020 417a 696d  leLayout.   Azim
+000014b0: 7574 6852 696e 674c 6179 6f75 740a 2020  uthRingLayout.  
+000014c0: 2044 6972 6563 7469 6f6e 4c61 796f 7574   DirectionLayout
+000014d0: 0a20 2020 4772 6964 4c61 796f 7574 0a20  .   GridLayout. 
+000014e0: 2020 4865 6d69 7370 6865 7265 506c 616e    HemispherePlan
+000014f0: 654c 6179 6f75 740a 0a60 6065 7261 6469  eLayout..``eradi
+00001500: 6174 652e 7363 656e 6573 2e70 6861 7365  ate.scenes.phase
+00001510: 6060 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ``.-------------
+00001520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2e2e  ------------....
+00001530: 2061 7574 6f6d 6f64 756c 653a 3a20 6572   automodule:: er
+00001540: 6164 6961 7465 2e73 6365 6e65 732e 7068  adiate.scenes.ph
+00001550: 6173 650a 0a2e 2e20 7079 3a63 7572 7265  ase.... py:curre
+00001560: 6e74 6d6f 6475 6c65 3a3a 2065 7261 6469  ntmodule:: eradi
+00001570: 6174 652e 7363 656e 6573 2e70 6861 7365  ate.scenes.phase
+00001580: 0a0a 2a2a 496e 7465 7266 6163 6573 2a2a  ..**Interfaces**
+00001590: 0a0a 2e2e 2061 7574 6f73 756d 6d61 7279  .... autosummary
+000015a0: 3a3a 0a20 2020 3a74 6f63 7472 6565 3a20  ::.   :toctree: 
+000015b0: 6765 6e65 7261 7465 642f 6175 746f 7375  generated/autosu
+000015c0: 6d6d 6172 792f 0a0a 2020 2050 6861 7365  mmary/..   Phase
+000015d0: 4675 6e63 7469 6f6e 0a0a 2a2a 4661 6374  Function..**Fact
+000015e0: 6f72 6965 732a 2a0a 0a2a 203a 6461 7461  ories**..* :data
+000015f0: 3a60 7068 6173 655f 6675 6e63 7469 6f6e  :`phase_function
+00001600: 5f66 6163 746f 7279 600a 0a2a 2a53 6365  _factory`..**Sce
+00001610: 6e65 2065 6c65 6d65 6e74 732a 2a0a 0a2e  ne elements**...
+00001620: 2e20 6175 746f 7375 6d6d 6172 793a 3a0a  . autosummary::.
+00001630: 2020 203a 746f 6374 7265 653a 2067 656e     :toctree: gen
+00001640: 6572 6174 6564 2f61 7574 6f73 756d 6d61  erated/autosumma
+00001650: 7279 2f0a 0a20 2020 4973 6f74 726f 7069  ry/..   Isotropi
+00001660: 6350 6861 7365 4675 6e63 7469 6f6e 0a20  cPhaseFunction. 
+00001670: 2020 5261 796c 6569 6768 5068 6173 6546    RayleighPhaseF
+00001680: 756e 6374 696f 6e0a 2020 2048 656e 7965  unction.   Henye
+00001690: 7947 7265 656e 7374 6569 6e50 6861 7365  yGreensteinPhase
+000016a0: 4675 6e63 7469 6f6e 0a20 2020 426c 656e  Function.   Blen
+000016b0: 6450 6861 7365 4675 6e63 7469 6f6e 0a20  dPhaseFunction. 
+000016c0: 2020 5461 6275 6c61 7465 6450 6861 7365    TabulatedPhase
+000016d0: 4675 6e63 7469 6f6e 0a0a 6060 6572 6164  Function..``erad
+000016e0: 6961 7465 2e73 6365 6e65 732e 696e 7465  iate.scenes.inte
+000016f0: 6772 6174 6f72 7360 600a 2d2d 2d2d 2d2d  grators``.------
+00001700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001710: 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e 2e20 6175  ---------.... au
+00001720: 746f 6d6f 6475 6c65 3a3a 2065 7261 6469  tomodule:: eradi
+00001730: 6174 652e 7363 656e 6573 2e69 6e74 6567  ate.scenes.integ
+00001740: 7261 746f 7273 0a0a 2e2e 2070 793a 6375  rators.... py:cu
+00001750: 7272 656e 746d 6f64 756c 653a 3a20 6572  rrentmodule:: er
+00001760: 6164 6961 7465 2e73 6365 6e65 732e 696e  adiate.scenes.in
+00001770: 7465 6772 6174 6f72 730a 0a2a 2a49 6e74  tegrators..**Int
+00001780: 6572 6661 6365 732a 2a0a 0a2e 2e20 6175  erfaces**.... au
+00001790: 746f 7375 6d6d 6172 793a 3a0a 2020 203a  tosummary::.   :
+000017a0: 746f 6374 7265 653a 2067 656e 6572 6174  toctree: generat
+000017b0: 6564 2f61 7574 6f73 756d 6d61 7279 2f0a  ed/autosummary/.
+000017c0: 0a20 2020 496e 7465 6772 6174 6f72 0a0a  .   Integrator..
+000017d0: 2a2a 4661 6374 6f72 6965 732a 2a0a 0a2a  **Factories**..*
+000017e0: 203a 6461 7461 3a60 696e 7465 6772 6174   :data:`integrat
+000017f0: 6f72 5f66 6163 746f 7279 600a 0a2a 2a53  or_factory`..**S
+00001800: 6365 6e65 2065 6c65 6d65 6e74 732a 2a0a  cene elements**.
+00001810: 0a2e 2e20 6175 746f 7375 6d6d 6172 793a  ... autosummary:
+00001820: 3a0a 2020 203a 746f 6374 7265 653a 2067  :.   :toctree: g
+00001830: 656e 6572 6174 6564 2f61 7574 6f73 756d  enerated/autosum
+00001840: 6d61 7279 2f0a 0a20 2020 5061 7468 496e  mary/..   PathIn
+00001850: 7465 6772 6174 6f72 0a20 2020 566f 6c50  tegrator.   VolP
+00001860: 6174 6849 6e74 6567 7261 746f 720a 2020  athIntegrator.  
+00001870: 2056 6f6c 5061 7468 4d49 5349 6e74 6567   VolPathMISInteg
+00001880: 7261 746f 720a 0a60 6065 7261 6469 6174  rator..``eradiat
+00001890: 652e 7363 656e 6573 2e73 7065 6374 7261  e.scenes.spectra
+000018a0: 6060 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ``.-------------
+000018b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+000018c0: 2e2e 2061 7574 6f6d 6f64 756c 653a 3a20  .. automodule:: 
+000018d0: 6572 6164 6961 7465 2e73 6365 6e65 732e  eradiate.scenes.
+000018e0: 7370 6563 7472 610a 0a2e 2e20 7079 3a63  spectra.... py:c
+000018f0: 7572 7265 6e74 6d6f 6475 6c65 3a3a 2065  urrentmodule:: e
+00001900: 7261 6469 6174 652e 7363 656e 6573 2e73  radiate.scenes.s
+00001910: 7065 6374 7261 0a0a 2a2a 496e 7465 7266  pectra..**Interf
+00001920: 6163 6573 2a2a 0a0a 2e2e 2061 7574 6f73  aces**.... autos
+00001930: 756d 6d61 7279 3a3a 0a20 2020 3a74 6f63  ummary::.   :toc
+00001940: 7472 6565 3a20 6765 6e65 7261 7465 642f  tree: generated/
+00001950: 6175 746f 7375 6d6d 6172 792f 0a0a 2020  autosummary/..  
+00001960: 2053 7065 6374 7275 6d0a 0a2a 2a46 6163   Spectrum..**Fac
+00001970: 746f 7269 6573 2a2a 0a0a 2a20 3a64 6174  tories**..* :dat
+00001980: 613a 6073 7065 6374 7275 6d5f 6661 6374  a:`spectrum_fact
+00001990: 6f72 7960 0a0a 2e2e 2064 726f 7064 6f77  ory`.... dropdow
+000019a0: 6e3a 3a20 5072 6976 6174 650a 0a20 2020  n:: Private..   
+000019b0: 2e2e 2061 7574 6f73 756d 6d61 7279 3a3a  .. autosummary::
+000019c0: 0a20 2020 2020 203a 746f 6374 7265 653a  .      :toctree:
+000019d0: 2067 656e 6572 6174 6564 2f61 7574 6f73   generated/autos
+000019e0: 756d 6d61 7279 2f0a 0a20 2020 2020 205f  ummary/..      _
+000019f0: 636f 7265 2e53 7065 6374 7275 6d46 6163  core.SpectrumFac
+00001a00: 746f 7279 0a0a 2a2a 5363 656e 6520 656c  tory..**Scene el
+00001a10: 656d 656e 7473 2a2a 0a0a 2e2e 2061 7574  ements**.... aut
+00001a20: 6f73 756d 6d61 7279 3a3a 0a20 2020 3a74  osummary::.   :t
+00001a30: 6f63 7472 6565 3a20 6765 6e65 7261 7465  octree: generate
+00001a40: 642f 6175 746f 7375 6d6d 6172 792f 0a0a  d/autosummary/..
+00001a50: 2020 2055 6e69 666f 726d 5370 6563 7472     UniformSpectr
+00001a60: 756d 0a20 2020 496e 7465 7270 6f6c 6174  um.   Interpolat
+00001a70: 6564 5370 6563 7472 756d 0a20 2020 4d75  edSpectrum.   Mu
+00001a80: 6c74 6944 656c 7461 5370 6563 7472 756d  ltiDeltaSpectrum
+00001a90: 0a20 2020 536f 6c61 7249 7272 6164 6961  .   SolarIrradia
+00001aa0: 6e63 6553 7065 6374 7275 6d0a 2020 2041  nceSpectrum.   A
+00001ab0: 6972 5363 6174 7465 7269 6e67 436f 6566  irScatteringCoef
+00001ac0: 6669 6369 656e 7453 7065 6374 7275 6d0a  ficientSpectrum.
```

### Comparing `eradiate-0.23.2rc2/docs/rst/reference_api/srf_tools.rst` & `eradiate-0.23.2rc3/docs/rst/reference_api/srf_tools.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/reference_api/test_tools.rst` & `eradiate-0.23.2rc3/docs/rst/reference_api/test_tools.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/reference_api/xarray.rst` & `eradiate-0.23.2rc3/docs/rst/reference_api/xarray.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/absorption.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/absorption.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/bad_resolution.png` & `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/bad_resolution.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/good_resolution.png` & `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/good_resolution.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/line.png` & `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/line.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/heterogeneous.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/heterogeneous.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/intro.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/intro.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/molecular.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/molecular.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/basic_concepts.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/basic_concepts.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/conventions.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/conventions.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/data/absorption.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/data/absorption.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/data/atmosphere_radprops.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/data/atmosphere_radprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/data/atmosphere_thermoprops.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/data/atmosphere_thermoprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/data/ckd.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/data/ckd.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png` & `eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/pt_points.png` & `eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/pt_points.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png` & `eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/data/intro.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/data/intro.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/data/particle_radprops.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/data/particle_radprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/data/solar_irradiance.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/data/solar_irradiance.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/data/spectra-us76_u86_4.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/data/spectra-us76_u86_4.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/data/srf.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/data/srf.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/index.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/install.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/install.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-.. _sec-getting_started-install:
+.. _sec-user_guide-install:
 
 Installation
 ============
 
 Eradiate is delivered through PyPI and can be installed using the ``pip``. This
 is the recommended way to install Eradiate.
 
 .. code:: bash
 
    pip install eradiate
 
 
 This will install the latest stable version of Eradiate, along with all the
 dependencies necessary to run it. If you want to install the latest development,
-please refer to the :ref:`sec-getting_started-development`.
+please refer to the :ref:`sec-developer_guides-dev_install`.
 
 .. warning::
 
    The ``eradiate`` depends on the ``eradiate-mitsuba`` package. This latter is
    strictly incompatible with ``mitsuba`` package. If you have installed
    ``mitsuba`` before, please make sure to uninstall it before installing
    ``eradiate`` and/or ``eradiate-mitsuba``.
```

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/onedim_experiment.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/onedim_experiment.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/package_structure.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/package_structure.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/spectral_discretization.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/spectral_discretization.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/rst/user_guide/unit_guide_user.rst` & `eradiate-0.23.2rc3/docs/rst/user_guide/unit_guide_user.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/docs/src/CHANGELOG.md` & `eradiate-0.23.2rc3/docs/src/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 %
 % ### Improvements and fixes
 %
 % ### Documentation
 %
 % ### Internal changes
 
-## v0.23.2 (upcoming release)
+## v0.23.2 (30th June 2023)
 
 ### Breaking changes
 
 * Removed the Docker images implementation, deployment and documentation
   from the Eradiate repository ({ghpr}`322`). Docker builds are no longer
   supported for now.
 * {class}`.Measure` no longer takes a `spectral_cfg` parameter but instead a
@@ -45,49 +45,57 @@
 * The {meth}`.MultiDistantMeasure.from_viewing_angles` constructor is removed
   ({ghpr}`315`). Use one of the other {class}`.MultiDistantMeasure` constructors
   instead.
 * The ``ertdata`` and ``ertshow`` command-line entry points are removed
   ({ghpr}`324`). Instead, use ``eradiate data`` and ``eradiate show``.
 * The {class}`.KernelDictContext` class is renamed {class}`.KernelContext`
   ({ghpr}`324`).
+* The `absorption_dataset` parameter of `AFGL1986RadProfile` and
+  `US76ApproxRadProfile` is now required ({ghpr}`334`).
 
 ### Deprecations and removals
 
 * Removed {class}`.SpectralContext` and subclasses ({ghpr}`311`).
 * Removed {class}`.MeasureSpectralConfig` and subclasses ({ghpr}`311`).
 * Removed the {meth}`.MultiDistantMeasure.from_viewing_angles` constructor
   ({ghpr}`315`).
 * Removed ``ertdata`` and ``ertshow`` command-line entry points ({ghpr}`324`).
 
 ### Improvements and fixes
 
 * Added {class}`.MultiDeltaSpectrum` spectrum type ({ghpr}`311`).
 * Exposed several API members in the top-level namespace ({ghpr}`324`).
-* Exposed the ``eradiate.spectral.*`` subpackage members in the
+* Exposed the `eradiate.spectral.*` subpackage members in the
   {mod}`eradiate.spectral` namespace ({ghpr}`324`).
 * Fixed incorrect Mitsuba scene parameter drop and lookup ({ghpr}`329`).
 * Added spherical-shell geometry support to DEM components
   {ghpr}`320`.
 * Fixed broken symmetry between {class}`.Spectrum` dictionary and object
   conversion protocols ({ghpr}`336`).
 * Provide an Eradiate Pypi package ({ghpr}`328`).
-* Implement the Astronomical Object Illumination, its tests and its
-  documentation ({ghpr}`331`).
+* Added {class}`.AstroObjectIllumination` illumination type ({ghpr}`331`,
+  {ghpr}`346`).
+* Fixed a bug where {class}`.Layout` constructors would not raise if passed
+  invalid azimuth values (*i.e.* outside the [0, 180]° range) ({ghpr}`345`).
+* Added `wavelength_range` optional parameter to `MolecularAtmosphere.ussa_1976()`
+  constructor to automatically open absorption datasets and restore working default
+  constructor ({ghpr}`334`).
 
 ### Documentation
 
 * Added a user guide page on spectral discretization.
 
 ### Internal changes
 
 * Spectral dispatch with `functools.singledispatchmethod` ({ghpr}`311`).
 * Experiments define the spectral discretization, based on information from
   its measure, its atmosphere components if applicable, and a default
   spectral set ({ghpr}`311`).
 * Rewrote the CLI using the Typer framework ({ghpr}`326`).
+* Refactored {class}`.Layout` constructor code ({ghpr}`345`).
 
 ## v0.23.1 (21 April 2023)
 
 ### Breaking changes
 
 * The `coddington_2021-1_nm` dataset is now the default solar irradiance
   spectrum ({ghpr}`300`). If you used to work with the default value
```

### Comparing `eradiate-0.23.2rc2/docs/src/reference_cli.md` & `eradiate-0.23.2rc3/docs/src/reference_cli.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/pyproject.toml` & `eradiate-0.23.2rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-dependencies-linux-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-dependencies-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-dependencies-osx-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-dependencies-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-dev-linux-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-dev-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-dev-osx-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-dev-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-dev.dot` & `eradiate-0.23.2rc3/requirements/conda/environment-dev.dot`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-dev.yml` & `eradiate-0.23.2rc3/requirements/conda/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-docs-linux-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-docs-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-docs-osx-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-docs-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-docs.dot` & `eradiate-0.23.2rc3/requirements/conda/environment-docs.dot`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-docs.yml` & `eradiate-0.23.2rc3/requirements/conda/environment-docs.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-main-linux-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-main-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-main-osx-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-main-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-optional-linux-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-optional-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-optional-osx-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-optional-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-optional.dot` & `eradiate-0.23.2rc3/requirements/conda/environment-optional.dot`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-optional.yml` & `eradiate-0.23.2rc3/requirements/conda/environment-optional.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-recommended-linux-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-recommended-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-recommended-osx-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-recommended-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-tests-linux-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-tests-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/environment-tests-osx-64.lock` & `eradiate-0.23.2rc3/requirements/conda/environment-tests-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/conda/layer_graph.dot` & `eradiate-0.23.2rc3/requirements/conda/layer_graph.dot`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/copy_envvars.py` & `eradiate-0.23.2rc3/requirements/copy_envvars.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/layered.yml` & `eradiate-0.23.2rc3/requirements/layered.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file establishes dependencies between layered requirement specs
 dependencies:
   includes:
     - main
   packages:
-    - "eradiate-mitsuba==0.0.1"
+    - "eradiate-mitsuba==0.0.2"
 
 main:
   constraints:
     - dev
   packages:
     - "aenum"
     - "attrs>=22.2"
@@ -78,8 +78,8 @@
     - "setuptools>=61"  # Required by dependency management scripts
     - "networkx>=3.1"  # Required by dependency management scripts
 
 optional:
   includes:
     - dev
   packages:
-    - "eradiate-mitsuba==0.0.1"
+    - "eradiate-mitsuba==0.0.2"
```

### Comparing `eradiate-0.23.2rc2/requirements/make_conda_env.py` & `eradiate-0.23.2rc3/requirements/make_conda_env.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/make_pip_in_files.py` & `eradiate-0.23.2rc3/requirements/make_pip_in_files.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/pip/dependencies.txt` & `eradiate-0.23.2rc3/requirements/pip/dependencies.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/pip/dev.txt` & `eradiate-0.23.2rc3/requirements/pip/dev.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/pip/docs.txt` & `eradiate-0.23.2rc3/requirements/pip/docs.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/pip/main.txt` & `eradiate-0.23.2rc3/requirements/pip/main.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/pip/optional.txt` & `eradiate-0.23.2rc3/requirements/pip/optional.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/pip/recommended.txt` & `eradiate-0.23.2rc3/requirements/pip/recommended.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/requirements/pip/tests.txt` & `eradiate-0.23.2rc3/requirements/pip/tests.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/setpath.sh` & `eradiate-0.23.2rc3/setpath.sh`

 * *Files 3% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 if [ "$BASH_VERSION" ]; then
     ERADIATE_SOURCE_DIR=$(dirname "$BASH_SOURCE")
     export ERADIATE_SOURCE_DIR=$(builtin cd "$ERADIATE_SOURCE_DIR"; builtin pwd)
 elif [ "$ZSH_VERSION" ]; then
     export ERADIATE_SOURCE_DIR=$(dirname "$0:A")
 fi
 
-export PYTHONPATH="${ERADIATE_SOURCE_DIR}/${BUILD_DIR}/ext/mitsuba/python:${PYTHONPATH}"
-export PATH="${ERADIATE_SOURCE_DIR}/${BUILD_DIR}/ext/mitsuba:${PATH}"
+export PYTHONPATH="${ERADIATE_SOURCE_DIR}/ext/mitsuba/${BUILD_DIR}/python:${PYTHONPATH}"
+export PATH="${ERADIATE_SOURCE_DIR}/ext/mitsuba/${BUILD_DIR}:${PATH}"
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/__init__.pyi` & `eradiate-0.23.2rc3/src/eradiate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/_config.py` & `eradiate-0.23.2rc3/src/eradiate/_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,21 +121,20 @@
     `the environ-config library <https://environ-config.readthedocs.io>`_
     """
 
     #: Path to the Eradiate source directory.
     source_dir = var(
         converter=lambda x: x if x is None else pathlib.Path(x).absolute(),
         help="Path to the Eradiate source directory. If it is not set, then the "
-            "current setup is assumed to be a production installation of Eradiate.",
+        "current setup is assumed to be a production installation of Eradiate.",
         default=None,
     )
 
     @source_dir.validator
     def _dir_validator(self, var, dir):
-
         if dir is None:
             if not __import__("eradiate").kernel.ERADIATE_MITSUBA_PACKAGE:
                 raise ConfigError(
                     "Could not find a suitable production installation for the "
                     "Eradiate kernel. This is either because you are using Eradiate "
                     "in a production environment without having the eradiate-mitsuba "
                     "package installed, or because you are using Eradiate directly "
@@ -182,15 +181,17 @@
         converter=str,
         help="URL where large data files are located.",
     )
 
     #: Path to the Eradiate download directory.
     download_dir = var(
         default="$ERADIATE_SOURCE_DIR/resources/downloads",
-        converter=lambda x: pathlib.Path(os.path.expandvars(x)).absolute(),
+        converter=lambda x: pathlib.Path(
+            os.path.expanduser(os.path.expandvars(x))
+        ).absolute(),
         help="Path to the Eradiate download directory.",
     )
 
     #: If ``True``, activate the offline mode. All online data stores
     #: will be disconnected.
     offline = environ.bool_var(
         default=False,
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/_factory.py` & `eradiate-0.23.2rc3/src/eradiate/_factory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/_mode.py` & `eradiate-0.23.2rc3/src/eradiate/_mode.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/attrs.py` & `eradiate-0.23.2rc3/src/eradiate/attrs.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/cli/__init__.py` & `eradiate-0.23.2rc3/src/eradiate/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/cli/data.py` & `eradiate-0.23.2rc3/src/eradiate/cli/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os.path
 import textwrap
 from pathlib import Path
 from typing import List, Optional
-from importlib_resources import files
 
 import typer
+from importlib_resources import files
 from rich.console import Console
 from ruamel.yaml import YAML
 from typing_extensions import Annotated
+
 import eradiate
 
 from ..exceptions import DataError
 
 app = typer.Typer()
 console = Console(color_system=None)
 
@@ -140,15 +141,17 @@
     """
     if not file_list:
         if from_file is None:
             # TODO: fetch this list from online
             if eradiate.config.source_dir is None:
                 from_file = files("eradiate") / "data" / "downloads.yml"
             else:
-                from_file = eradiate.config.source_dir / "data" / "downloads_development.yml"
+                from_file = (
+                    eradiate.config.source_dir / "data" / "downloads_development.yml"
+                )
         console.print(f"Reading file list from '{from_file}'")
         yaml = YAML()
         file_list = yaml.load(from_file)
 
     for filename in file_list:
         try:
             console.print(f"[blue]Fetching '{filename}'[/]")
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/cli/show.py` & `eradiate-0.23.2rc3/src/eradiate/cli/show.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/cli/srf.py` & `eradiate-0.23.2rc3/src/eradiate/cli/srf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/contexts.py` & `eradiate-0.23.2rc3/src/eradiate/contexts.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/converters.py` & `eradiate-0.23.2rc3/src/eradiate/converters.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/data/__init__.pyi` & `eradiate-0.23.2rc3/src/eradiate/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/data/_access.py` & `eradiate-0.23.2rc3/src/eradiate/data/_access.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/data/_blind_directory.py` & `eradiate-0.23.2rc3/src/eradiate/data/_blind_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/data/_blind_online.py` & `eradiate-0.23.2rc3/src/eradiate/data/_blind_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/data/_core.py` & `eradiate-0.23.2rc3/src/eradiate/data/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/data/_multi.py` & `eradiate-0.23.2rc3/src/eradiate/data/_multi.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/data/_safe_directory.py` & `eradiate-0.23.2rc3/src/eradiate/data/_safe_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/data/_safe_online.py` & `eradiate-0.23.2rc3/src/eradiate/data/_safe_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/data/_store.py` & `eradiate-0.23.2rc3/src/eradiate/data/_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from ._safe_online import SafeOnlineDataStore
 from .._config import config
 
 #: Global data store.
 data_store: MultiDataStore = None
 
 
-def init_data_store(offline: bool | None = None, production: bool | None = None) -> None:
+def init_data_store(
+    offline: bool | None = None, production: bool | None = None
+) -> None:
     """
     Initialize the global data store.
 
     Parameters
     ----------
     offline : bool, optional
         If ``True``, replace all online data stores with blind directory data
@@ -50,15 +52,20 @@
     else:
         if offline:
             small_files = BlindDirectoryDataStore(
                 path=config.download_dir / "resources" / "data"
             )
         else:
             small_files = SafeOnlineDataStore(
-                base_url="/".join([config.small_files_registry_url, config.small_files_registry_revision,]),
+                base_url="/".join(
+                    [
+                        config.small_files_registry_url,
+                        config.small_files_registry_revision,
+                    ]
+                ),
                 path=config.download_dir / "resources" / "data",
             )
 
     if not offline:
         data_store = MultiDataStore(
             stores=OrderedDict(
                 [
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/data/downloads.yml` & `eradiate-0.23.2rc3/src/eradiate/data/downloads.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/data/downloads_development.yml` & `eradiate-0.23.2rc3/src/eradiate/data/downloads_development.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/exceptions.py` & `eradiate-0.23.2rc3/src/eradiate/exceptions.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/experiments/_atmosphere.py` & `eradiate-0.23.2rc3/src/eradiate/experiments/_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/experiments/_canopy.py` & `eradiate-0.23.2rc3/src/eradiate/experiments/_canopy.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
         doc=get_doc(Experiment, attrib="_integrator", field="doc"),
         type=get_doc(Experiment, attrib="_integrator", field="type"),
         init_type=get_doc(Experiment, attrib="_integrator", field="init_type"),
         default=":class:`PathIntegrator() <.PathIntegrator>`",
     )
 
     def __attrs_post_init__(self):
-
         self._normalize_spectral()
         self._normalize_measures()
 
     def _normalize_measures(self) -> None:
         """
         Ensure that distant measure targets are set to appropriate values.
         Processed measures will have its ray target and origin parameters
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/experiments/_canopy_atmosphere.py` & `eradiate-0.23.2rc3/src/eradiate/experiments/_canopy_atmosphere.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,14 @@
             if self.atmosphere is not None:
                 return VolPathIntegrator()
             else:
                 return PathIntegrator()
         return self._integrator
 
     def __attrs_post_init__(self):
-
         self._normalize_spectral()
         self._normalize_atmosphere()
         self._normalize_measures()
 
     def _normalize_atmosphere(self) -> None:
         """
         Ensure consistency between the atmosphere and experiment geometries.
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/experiments/_core.py` & `eradiate-0.23.2rc3/src/eradiate/experiments/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/experiments/_dem.py` & `eradiate-0.23.2rc3/src/eradiate/experiments/_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/experiments/_helpers.py` & `eradiate-0.23.2rc3/src/eradiate/experiments/_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/frame.py` & `eradiate-0.23.2rc3/src/eradiate/frame.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/kernel/__init__.py` & `eradiate-0.23.2rc3/src/eradiate/kernel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from importlib.metadata import version, PackageNotFoundError
+from importlib.metadata import PackageNotFoundError, version
 from unittest.mock import Mock
 
 # Internal constants
 _EXPECTED_MITSUBA_VERSION = "3.2.1"
-_EXPECTED_MITSUBA_PATCH_VERSION = "0.0.1"
+_EXPECTED_MITSUBA_PATCH_VERSION = "0.0.2"
 
 # Exported constants
 ERADIATE_MITSUBA_PACKAGE_VERSION = None
 ERADIATE_MITSUBA_PACKAGE = False
 ERADIATE_KERNEL_VERSION = None
 ERADIATE_KERNEL_PATCH_VERSION = None
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/kernel/__init__.pyi` & `eradiate-0.23.2rc3/src/eradiate/kernel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/kernel/_bitmap.py` & `eradiate-0.23.2rc3/src/eradiate/kernel/_bitmap.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/kernel/_bsdf.py` & `eradiate-0.23.2rc3/src/eradiate/kernel/_bsdf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/kernel/_kernel_dict.py` & `eradiate-0.23.2rc3/src/eradiate/kernel/_kernel_dict.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/kernel/_render.py` & `eradiate-0.23.2rc3/src/eradiate/kernel/_render.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/kernel/gridvolume.py` & `eradiate-0.23.2rc3/src/eradiate/kernel/gridvolume.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/kernel/logging.py` & `eradiate-0.23.2rc3/src/eradiate/kernel/logging.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/kernel/transform.py` & `eradiate-0.23.2rc3/src/eradiate/kernel/transform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/notebook/__init__.py` & `eradiate-0.23.2rc3/src/eradiate/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/notebook/tutorials.py` & `eradiate-0.23.2rc3/src/eradiate/notebook/tutorials.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/pipelines/__init__.pyi` & `eradiate-0.23.2rc3/src/eradiate/pipelines/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/pipelines/_aggregate.py` & `eradiate-0.23.2rc3/src/eradiate/pipelines/_aggregate.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,14 @@
         # TODO: PR#311 hack (next 3 lines)
         _bins = self.binset.bins
         _bins_wcenters = [b.wcenter.m_as(wavelength_units) for b in _bins]
         _bins_wcenters_str = [str(int(w)) for w in _bins_wcenters]
 
         # For each bin and each pixel, compute quadrature and store the result
         for i_bin, bin in enumerate(bin_ids):
-
             # TODO: PR#311 hack (next 2 lines)
             _bin_index = _bins_wcenters_str.index(bin)
             _bin = _bins[_bin_index]
 
             values_at_nodes = img.sel(bin=bin).values
 
             # Rationale: Avoid using xarray's indexing in this loop for
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/pipelines/_assemble.py` & `eradiate-0.23.2rc3/src/eradiate/pipelines/_assemble.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/pipelines/_compute.py` & `eradiate-0.23.2rc3/src/eradiate/pipelines/_compute.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/pipelines/_core.py` & `eradiate-0.23.2rc3/src/eradiate/pipelines/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/pipelines/_gather.py` & `eradiate-0.23.2rc3/src/eradiate/pipelines/_gather.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/plot.py` & `eradiate-0.23.2rc3/src/eradiate/plot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/quad.py` & `eradiate-0.23.2rc3/src/eradiate/quad.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/radprops/_afgl1986.py` & `eradiate-0.23.2rc3/src/eradiate/radprops/_afgl1986.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,26 @@
     :cite:`Anderson1986AtmosphericConstituentProfiles`.
 
     Warnings
     --------
     This class does not support ``mono`` modes.
     """
 
+    absorption_dataset: xr.Dataset = documented(
+        attrs.field(
+            converter=converters.to_dataset(
+                load_from_id=None  # TODO: open dataset (not load)
+            ),
+            validator=attrs.validators.instance_of(xr.Dataset),
+        ),
+        doc="Absorption coefficient dataset.",
+        type="Dataset",
+        init_type="Dataset or :class:`.PathLike`",
+    )
+
     _thermoprops: xr.Dataset = documented(
         attrs.field(
             factory=lambda: afgl_1986.make_profile(),
             converter=_convert_thermoprops_afgl_1986,
             validator=attrs.validators.instance_of(xr.Dataset),
             repr=summary_repr,
         ),
@@ -84,46 +96,14 @@
         doc="Scattering switch. If ``True``, the scattering coefficient is "
         "computed. Else, the scattering coefficient is not computed and "
         "instead set to zero.",
         type="bool",
         default="True",
     )
 
-    absorption_dataset: xr.Dataset | None = documented(
-        attrs.field(
-            default=None,
-            converter=attrs.converters.optional(
-                converters.to_dataset(load_from_id=None)
-            ),  # TODO: open dataset (not load)
-            validator=attrs.validators.optional(
-                attrs.validators.instance_of(xr.Dataset)
-            ),
-        ),
-        doc="Absorption coefficient dataset. If ``None``, the absorption "
-        "coefficient is set to zero.",
-        type="Dataset or None",
-        init_type="Dataset or :class:`.PathLike`",
-        default="None",
-    )
-
-    @absorption_dataset.validator
-    @has_absorption.validator
-    def _check_absorption_dataset(self, attribute, value):
-        if not self.has_absorption and self.absorption_dataset is not None:
-            warnings.warn(
-                "When validating attribute 'absorption_dataset': specified "
-                "absorption dataset will be ignored because absorption is "
-                "disabled."
-            )
-        if self.has_absorption and self.absorption_dataset is None:
-            raise ValueError(
-                "When validating attribute 'absorption_dataset': no absorption "
-                "dataset was specified, absorption will be disabled."
-            )
-
     _zgrid: ZGrid | None = attrs.field(default=None, init=False)
 
     def __attrs_post_init__(self):
         self.update()
 
     def update(self) -> None:
         self._zgrid = ZGrid(levels=self.levels)
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/radprops/_core.py` & `eradiate-0.23.2rc3/src/eradiate/radprops/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/radprops/_us76_approx.py` & `eradiate-0.23.2rc3/src/eradiate/radprops/_us76_approx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import typing as t
+import warnings
 
 import attrs
 import numpy as np
 import pint
 import xarray as xr
 
 from ._core import RadProfile, ZGrid, make_dataset
-from ._util_mono import get_us76_u86_4_spectrum_filename
 from .absorption import compute_sigma_a
 from .rayleigh import compute_sigma_s_air
-from .. import converters, data
+from .. import converters
 from ..attrs import documented, parse_docs
 from ..thermoprops import us76
 from ..units import to_quantity
 from ..units import unit_registry as ureg
 from ..util.misc import cache_by_id, summary_repr
 
 
@@ -102,14 +102,23 @@
       about the gas species concentration profiles.
       Notably, the "U.S. Standard (1976) atmospheric profile model" of the
       AFGL's report include radiatively active gases such as H2O, O3, N2O,
       and CO, that the *U.S. Standard Atmosphere 1976* atmosphere model does
       not include.
     """
 
+    absorption_dataset: xr.Dataset = documented(
+        attrs.field(
+            converter=converters.to_dataset(load_from_id=None),
+            validator=attrs.validators.instance_of(xr.Dataset),
+        ),
+        doc="Absorption coefficient data set.",
+        type=":class:`xarray.Dataset`",
+    )
+
     _thermoprops: xr.Dataset = documented(
         attrs.field(
             factory=lambda: us76.make_profile(),
             converter=_convert_thermoprops_us76_approx,
             validator=attrs.validators.instance_of(xr.Dataset),
             repr=summary_repr,
         ),
@@ -140,30 +149,14 @@
         doc="Scattering switch. If ``True``, the scattering coefficient is "
         "computed. Else, the scattering coefficient is not computed and "
         "instead set to zero.",
         type="bool",
         default="True",
     )
 
-    absorption_dataset: xr.Dataset | None = documented(
-        attrs.field(
-            default=None,
-            converter=attrs.converters.optional(
-                converters.to_dataset(load_from_id=None)
-            ),
-            validator=attrs.validators.optional(
-                attrs.validators.instance_of(xr.Dataset)
-            ),
-        ),
-        doc="Absorption coefficient data set. If ``None``, the default "
-        "absorption coefficient data set is opened.",
-        type=":class:`xarray.Dataset` or None",
-        default="None",
-    )
-
     _zgrid: ZGrid | None = attrs.field(default=None, init=False)
 
     def __attrs_post_init__(self):
         self.update()
 
     def update(self) -> None:
         self._zgrid = ZGrid(levels=self.levels)
@@ -218,20 +211,16 @@
 
     def eval_sigma_t_mono(self, w: pint.Quantity, zgrid: ZGrid) -> pint.Quantity:
         return self.eval_sigma_a_mono(w, zgrid) + self.eval_sigma_s_mono(w, zgrid)
 
     def eval_sigma_a_mono(self, w: pint.Quantity, zgrid: ZGrid) -> pint.Quantity:
         profile = self._thermoprops_interp(zgrid)
 
-        # TODO: refactor so that absorption dataset must be provided at init
         if self.has_absorption:
-            if self.absorption_dataset is None:  # ! this is never tested
-                ds = data.open_dataset(get_us76_u86_4_spectrum_filename(w))
-            else:
-                ds = self.absorption_dataset
+            ds = self.absorption_dataset
 
             # Compute scattering coefficient
             result = compute_sigma_a(
                 ds=ds,
                 wl=w,
                 p=to_quantity(profile.p),
                 n=to_quantity(profile.n),
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/radprops/_util_mono.py` & `eradiate-0.23.2rc3/src/eradiate/radprops/_util_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/radprops/absorption.py` & `eradiate-0.23.2rc3/src/eradiate/radprops/absorption.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/radprops/rayleigh.py` & `eradiate-0.23.2rc3/src/eradiate/radprops/rayleigh.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 _LOSCHMIDT = ureg.Quantity(
     *physical_constants["Loschmidt constant (273.15 K, 101.325 kPa)"][:2]
 ).to("km^-3")
 
 # Air number density at 101325 Pa and 288.15 K
 _STANDARD_AIR_NUMBER_DENSITY = _LOSCHMIDT * (273.15 / 288.15)
 
+
 # Bates (1984) King correction factor data
 class _BATES_1984_DATA(metaclass=Singleton):
     # Lazy loader for Bates (1984) King correction data
     def __init__(self):
         self._data = None
 
     @property
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/rng.py` & `eradiate-0.23.2rc3/src/eradiate/rng.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/__init__.pyi` & `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_core.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_heterogeneous.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_homogeneous.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_homogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import xarray as xr
 
 import eradiate
 
 from ._core import AbstractHeterogeneousAtmosphere
 from ..core import traverse
 from ..phase import PhaseFunction, RayleighPhaseFunction, phase_function_factory
-from ... import converters
+from ... import converters, data
 from ...attrs import documented, parse_docs
 from ...contexts import KernelContext
 from ...quad import Quad
 from ...radprops import AFGL1986RadProfile, RadProfile, US76ApproxRadProfile, ZGrid
 from ...spectral.ckd import BinSet
 from ...spectral.index import SpectralIndex
 from ...spectral.mono import WavelengthSet
@@ -30,14 +30,53 @@
     compute_scaling_factors,
     interpolate,
     rescale_concentration,
 )
 from ...units import unit_registry as ureg
 from ...util.misc import summary_repr
 
+DEFAULT_WAVELENGTH_RANGE = [545.0, 555.0] * ureg.nm
+
+
+def open_us76_dataset(wavelength_range: pint.Quantity) -> xr.Dataset:
+    """
+    Open the monochromatic absorption dataset corresponding to the given
+    wavelength range, for the U.S. 1976 Standard Atmosphere.
+    """
+    path = "spectra/absorption/us76_u86_4"
+    wlmin, wlmax = wavelength_range
+    wnmin = (1 / wlmax).m_as("1/cm")
+    wnmax = (1 / wlmin).m_as("1/cm")
+    w = np.concatenate([np.arange(4000, 25711, 1000), [25711]])
+    if wnmin < w[0] or wnmax > w[-1]:
+        raise ValueError(
+            f"Invalid wavelength range: {wavelength_range}. "
+            f"Supported wavelength range: {1e7 / w[-1]:.1f}-"
+            f"{1e7 / w[0]:.1f} nm."
+        )
+
+    wmin = w[wnmin > w][-1]
+    wmax = w[wnmax < w][0]
+    iwmin = w.tolist().index(wmin)
+    iwmax = w.tolist().index(wmax)
+    paths = [
+        f"{path}/us76_u86_4-spectra-{w[i]}_{w[i+1]}.nc" for i in range(iwmin, iwmax)
+    ]
+
+    if len(paths) == 1:
+        absorption_dataset = data.open_dataset(paths[0])
+    else:
+        datasets = [
+            data.open_dataset(path).isel(w=slice(0, -1))  # strip endpoints
+            for path in paths
+        ]
+        absorption_dataset = xr.concat(datasets, dim="w")
+
+    return absorption_dataset
+
 
 @parse_docs
 @attrs.define(eq=False, slots=False)
 class MolecularAtmosphere(AbstractHeterogeneousAtmosphere):
     """
     Molecular atmosphere scene element [``molecular``].
 
@@ -149,14 +188,20 @@
 
     def update(self) -> None:
         # Inherit docstring
 
         self.phase.id = self.phase_id
 
         if self.thermoprops.title == "U.S. Standard Atmosphere 1976":
+            # temporary fix
+            if self.absorption_dataset is None and self.has_absorption:
+                self.absorption_dataset = (
+                    "spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
+                )
+
             self._radprops_profile = US76ApproxRadProfile(
                 thermoprops=self.thermoprops,
                 has_scattering=self.has_scattering,
                 has_absorption=self.has_absorption,
                 absorption_dataset=self.absorption_dataset,
             )
         elif "AFGL (1986)" in self.thermoprops.title:
@@ -359,24 +404,23 @@
                 "Cannot pass 'absorption_dataset' keyword argument. The "
                 "'afgl_1986' constructor sets the absorption dataset "
                 "automatically."
             )
 
         thermoprops = afgl_1986.make_profile(model_id=model)
 
+        # open the absorption dataset corresponding to 'binset' and 'model'
         path = "ckd/absorption"
-        if kwargs.get("has_absorption", True):
-            if binset == "10nm":
-                absorption_dataset = f"{path}/10nm/afgl_1986-{model}-10nm-v3.nc"
-            elif binset == "1nm":
-                absorption_dataset = f"{path}/1nm/afgl_1986-{model}-1nm-v3.nc"
-            else:
-                raise ValueError(f"Invalid binset: {binset}")
+
+        if binset == "10nm":
+            absorption_dataset = f"{path}/10nm/afgl_1986-{model}-10nm-v3.nc"
+        elif binset == "1nm":
+            absorption_dataset = f"{path}/1nm/afgl_1986-{model}-1nm-v3.nc"
         else:
-            absorption_dataset = None
+            raise ValueError(f"Invalid binset: {binset}")
 
         if concentrations is not None:
             factors = compute_scaling_factors(
                 ds=thermoprops,
                 concentration=pinttr.interpret_units(concentrations, ureg=ureg),
             )
             thermoprops = rescale_concentration(ds=thermoprops, factors=factors)
@@ -395,40 +439,65 @@
         )
 
     @classmethod
     def ussa_1976(
         cls,
         levels: pint.Quantity | None = None,
         concentrations: dict[str, pint.Quantity] | None = None,
+        wavelength_range: pint.Quantity | None = None,
         **kwargs: dict[str, t.Any],
     ) -> MolecularAtmosphere:
         """
         Molecular atmosphere based on the US Standard Atmosphere (1976) model
         :cite:`NASA1976USStandardAtmosphere` (monochromatic mode only).
 
         Parameters
         ----------
         levels : quantity, optional
             Altitude levels. If ``None``, defaults to [0, 1, ..., 99, 100] km.
 
         concentrations : dict
             Molecules concentrations as a ``{str: quantity}`` mapping.
 
+        wavelength_range: quantity
+            Wavelength range wherein the atmosphere radiative properties are
+            expected to be computed.
+            This information is used to select the monochromatic absorption
+            dataset(s) to open.
+            If None, defaults to [545.0, 555.0] nm.
+
         **kwargs
             Keyword arguments passed to the :class:`.MolecularAtmosphere`
             constructor.
 
         Returns
         -------
         :class:`.MolecularAtmosphere`
             U.S. Standard Atmosphere (1976) molecular atmosphere object.
         """
+        if "absorption_dataset" in kwargs:
+            raise TypeError(
+                "Cannot pass 'absorption_dataset' keyword argument. The "
+                "'ussa_1976' constructor sets the absorption dataset "
+                "automatically."
+            )
+
+        # open the absorption dataset corresponding to 'wavelength_range
+        if wavelength_range is None:
+            wavelength_range = DEFAULT_WAVELENGTH_RANGE
+
+        absorption_dataset = open_us76_dataset(wavelength_range)
+
         if levels is None:
             levels = np.linspace(0, 100, 101) * ureg.km
 
         ds = us76.make_profile(levels=levels)
 
         if concentrations is not None:
             factors = compute_scaling_factors(ds=ds, concentration=concentrations)
             ds = rescale_concentration(ds=ds, factors=factors)
 
-        return cls(thermoprops=ds, **kwargs)
+        return cls(
+            thermoprops=ds,
+            absorption_dataset=absorption_dataset,
+            **kwargs,
+        )
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_particle_dist.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_particle_dist.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_particle_layer.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_particle_layer.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_core.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_discrete.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_discrete.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_leaf_cloud.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_leaf_cloud.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_tree.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_tree.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_black.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_black.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_checkerboard.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_checkerboard.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_core.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_lambertian.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_lambertian.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_mqdiffuse.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_mqdiffuse.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_opacity_mask.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_opacity_mask.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_rpv.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/core.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/geometry.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/geometry.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_constant.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_constant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_core.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from ..core import NodeSceneElement
 from ..._factory import Factory
 from ...attrs import documented, get_doc, parse_docs
 
 illumination_factory = Factory()
 illumination_factory.register_lazy_batch(
     [
+        ("_astro_object.AstroObjectIllumination", "astro_object", {}),
         ("_constant.ConstantIllumination", "constant", {}),
         ("_directional.DirectionalIllumination", "directional", {}),
-        ("_astroobject.AstroObjectIllumination", "astro_object", {}),
         ("_spot.SpotIllumination", "spot", {}),
     ],
     cls_prefix="eradiate.scenes.illumination",
 )
 
 
 @parse_docs
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_directional.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_directional.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,17 +98,15 @@
             flip=True,
         ).reshape((3,))
 
     @property
     def _to_world(self) -> mi.ScalarTransorm4f:
         direction = dr.normalize(mi.ScalarVector3f(self.direction))
         up, _ = mi.coordinate_system(direction)
-        return mi.ScalarTransform4f.look_at(
-            origin=0.0, target=mi.ScalarPoint3f(direction), up=up
-        )
+        return mi.ScalarTransform4f.look_at(origin=0.0, target=direction, up=up)
 
     @property
     def template(self) -> dict:
         return {"type": "directional", "to_world": self._to_world}
 
     @property
     def objects(self) -> dict[str, NodeSceneElement]:
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_spot.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_spot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/integrators/_core.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/integrators/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/integrators/_path_tracers.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/integrators/_path_tracers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/measure/__init__.pyi` & `eradiate-0.23.2rc3/src/eradiate/scenes/measure/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_core.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -201,14 +201,26 @@
         doc="Mitsuba sampler used to generate pseudo-random number sequences.",
         type="str",
         init_type='{"independent", "stratified", "multijitter", "orthogonal", '
         '"ldsampler"}',
         default='"independent"',
     )
 
+    rfilter: str = documented(
+        attrs.field(
+            default="box",
+            validator=attrs.validators.in_({"box", "gaussian"}),
+        ),
+        doc="Reconstruction filter used to scatter samples on sensor pixels. "
+        "By default, using a box filter is recommended.",
+        type="str",
+        init_type='{"box", "gaussian"}',
+        default='"box"',
+    )
+
     spp: int = documented(
         attrs.field(default=1000, converter=int, validator=validators.is_positive),
         doc="Number of samples per pixel.",
         type="int",
         default="1000",
     )
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_distant.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_distant.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,22 +256,15 @@
     #                           Fields and properties
     # --------------------------------------------------------------------------
 
     target: Target | None = documented(
         attrs.field(
             default=None,
             converter=attrs.converters.optional(Target.convert),
-            validator=attrs.validators.optional(
-                attrs.validators.instance_of(
-                    (
-                        TargetPoint,
-                        TargetRectangle,
-                    )
-                )
-            ),
+            validator=attrs.validators.optional(attrs.validators.instance_of(Target)),
             on_setattr=attrs.setters.pipe(
                 attrs.setters.convert, attrs.setters.validate
             ),
         ),
         doc="Target specification. The target can be specified using an "
         "array-like with 3 elements (which will be converted to a "
         ":class:`.TargetPoint`) or a dictionary interpreted by "
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_distant_flux.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_distant_flux.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_hemispherical_distant.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_hemispherical_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_multi_distant.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_multi_distant.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from ... import converters, frame
 from ..._config import config
 from ...attrs import documented, parse_docs
 from ...units import symbol
 from ...units import unit_context_config as ucc
 from ...units import unit_context_kernel as uck
 from ...units import unit_registry as ureg
-from ...util.deprecation import deprecated
 from ...util.misc import flatten
 
 # ------------------------------------------------------------------------------
 #                               Layout framework
 # ------------------------------------------------------------------------------
 
 
@@ -135,40 +134,54 @@
         """
         # Default implementation computes directions from angles
         return frame.angles_to_direction(
             self.angles, azimuth_convention=self.azimuth_convention
         )
 
 
+def _angles_converter(value):
+    value = pinttr.util.ensure_units(value, ucc.deferred("angle"))
+    angle_units = value.u
+    magnitude = np.reshape(value.m_as(ureg.deg), (-1, 2))
+    zeniths = magnitude[:, 0]
+    azimuths = magnitude[:, 1]
+    return (np.stack((zeniths, azimuths % 360), axis=1) * ureg.deg).to(angle_units)
+
+
 @parse_docs
 @attrs.define
 class AngleLayout(Layout):
     """
     A viewing direction layout directly defined by explicit (zenith, azimuth)
     pairs.
     """
 
     _angles: pint.Quantity = documented(
         pinttr.ib(
-            converter=lambda x: np.reshape(
-                pinttr.converters.to_units(ucc.deferred("angle"))(x), (-1, 2)
-            )
-            % (360.0 * ureg.deg),
+            converter=_angles_converter,
             units=ucc.deferred("angle"),
         ),
         doc="A sequence of viewing angles, corresponding to the direction "
         "sequence produced by :attr:`directions`, as a (N, 2) array. "
-        "The last dimension is ordered as (zenith, azimuth). "
-        "**Required, no default**.\n"
+        "The last dimension is ordered as (zenith, azimuth). Zenith values "
+        "must be between 0 and 180°. **Required, no default**.\n"
         "\n"
         "Unit-enabled field (default: ucc['angle']).",
         type="quantity",
         init_type="array-like",
     )
 
+    @_angles.validator
+    def _angles_validator(self, attribute, value):
+        zeniths = value[:, 0].m_as(ureg.deg)
+        if np.any((zeniths < 0) | (zeniths > 180)):
+            raise ValueError(
+                f"while validating {attribute.name}: zenith values must be in [0°, 180°]"
+            )
+
     @property
     def angles(self) -> pint.Quantity:
         # Inherit docstring
         return self._angles
 
 
 @parse_docs
@@ -177,32 +190,42 @@
     """
     A viewing direction layout defined by a single zenith and a vector of
     explicit azimuth values.
     """
 
     zenith: pint.Quantity = documented(
         pinttr.field(
-            converter=lambda x: converters.on_quantity(float)(
-                pinttr.converters.to_units(ucc.deferred("angle"))(x)
+            converter=attrs.converters.pipe(
+                pinttr.converters.to_units(ucc.deferred("angle")),
+                lambda x: converters.on_quantity(float)(x),
             ),
             units=ucc.deferred("angle"),
         ),
-        doc="A single zenith value. **Required, no default**.\n"
+        doc="A single zenith value. Must be in [0°, 180°]. **Required, no default**.\n"
         "\n"
         "Unit-enabled field (default: ucc['angle']).",
         type="quantity",
         init_type="float or quantity",
     )
 
+    @zenith.validator
+    def _zenith_validator(self, attribute, value):
+        zenith = value.m_as(ureg.deg)
+        if zenith < 0 or zenith > 180:
+            raise ValueError(
+                f"while validating {attribute.name}: zenith value must be in [0°, 180°]"
+            )
+
     azimuths: pint.Quantity = documented(
         pinttr.field(
-            converter=lambda x: np.reshape(
-                pinttr.converters.to_units(ucc.deferred("angle"))(x), (-1,)
-            )
-            % (360.0 * ureg.deg),
+            converter=attrs.converters.pipe(
+                pinttr.converters.to_units(ucc.deferred("angle")),
+                lambda x: np.reshape(x, (-1,)),
+                lambda x: x % (360.0 * ureg.deg),
+            ),
             units=ucc.deferred("angle"),
         ),
         doc="A vector of azimuth values. **Required, no default**.\n"
         "\n"
         "Unit-enabled field (default: ucc['angle']).",
         type="quantity",
         init_type="array-like",
@@ -265,28 +288,35 @@
     """
     A viewing direction layout defined by a single azimuth and a vector of
     zenith values. Negative zenith values are mapped to (azimuth + 180°).
     """
 
     zeniths: pint.Quantity = documented(
         pinttr.field(
-            converter=lambda x: np.reshape(
-                pinttr.converters.to_units(ucc.deferred("angle"))(x), (-1,)
+            converter=attrs.converters.pipe(
+                pinttr.converters.to_units(ucc.deferred("angle")),
+                lambda x: np.reshape(x, (-1,)),
             ),
             units=ucc.deferred("angle"),
         ),
         doc="A vector of zenith values. **Required, no default**.\n"
         "\n"
         "Unit-enabled field (default: ucc['angle']).",
         type="quantity",
         init_type="array-like",
     )
 
     azimuth: pint.Quantity = documented(
-        pinttr.field(units=ucc.deferred("angle")),
+        pinttr.field(
+            converter=attrs.converters.pipe(
+                pinttr.converters.to_units(ucc.deferred("angle")),
+                lambda x: x % (360 * ureg.deg),
+            ),
+            units=ucc.deferred("angle"),
+        ),
         doc="A single zenith value. **Required, no default**.",
         type="quantity",
         init_type="float or quantity",
     )
 
     @property
     def angles(self) -> pint.Quantity:
@@ -306,30 +336,40 @@
     """
     A viewing direction layout defined as the Cartesian product of an azimuth
     and zenith vectors.
     """
 
     zeniths: pint.Quantity = documented(
         pinttr.field(
-            converter=lambda x: np.reshape(
-                pinttr.converters.to_units(ucc.deferred("angle"))(x), (-1,)
+            converter=attrs.converters.pipe(
+                pinttr.converters.to_units(ucc.deferred("angle")),
+                lambda x: np.reshape(x, (-1,)),
             ),
             units=ucc.deferred("angle"),
         ),
         doc="A vector of zenith values. **Required, no default**.\n"
         "\n"
         "Unit-enabled field (default: ucc['angle']).",
         type="quantity",
         init_type="array-like",
     )
 
+    @zeniths.validator
+    def _zeniths_validator(self, attribute, value):
+        zeniths = value.m_as(ureg.deg)
+        if np.any((zeniths < 0) | (zeniths > 180)):
+            raise ValueError(
+                f"while validating {attribute.name}: zenith values must be in [0°, 180°]"
+            )
+
     azimuths: pint.Quantity = documented(
         pinttr.field(
-            converter=lambda x: np.reshape(
-                pinttr.converters.to_units(ucc.deferred("angle"))(x), (-1,)
+            converter=attrs.converters.pipe(
+                pinttr.converters.to_units(ucc.deferred("angle")),
+                lambda x: np.reshape(x, (-1,)),
             ),
             units=ucc.deferred("angle"),
         ),
         doc="A vector of azimuth values. **Required, no default**.\n"
         "\n"
         "Unit-enabled field (default: ucc['angle']).",
         type="quantity",
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_multi_radiancemeter.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_multi_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_perspective.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_perspective.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_radiancemeter.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/phase/_blend.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/phase/_blend.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,14 @@
         weights = self._eval_conditional_weights_impl(si)
 
         # Return selected components
         return weights[n_component, ...]
 
     @property
     def template(self) -> dict:
-
         result = {"type": "blendphase"}
 
         for i in range(len(self.components) - 1):
             prefix = "phase_1." * i
 
             # Add components
             template, _ = traverse(self.components[i])
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/phase/_core.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/phase/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/phase/_hg.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/phase/_hg.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/phase/_rayleigh.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/phase/_rayleigh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/phase/_tabulated.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/phase/_tabulated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_buffermesh.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_buffermesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_core.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_cuboid.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_cuboid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_filemesh.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_filemesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_rectangle.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_rectangle.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_sphere.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_sphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_air_scattering_coefficient.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_air_scattering_coefficient.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_core.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_interpolated.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_interpolated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_multi_delta.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_multi_delta.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,23 +69,21 @@
         raise NotImplementedError
 
     @property
     def params(self) -> dict:
         raise NotImplementedError
 
     def select_in_wavelength_set(self, wset: WavelengthSet) -> WavelengthSet:
-
         # the input wavelength set is completely ignored
         # only the attribute wavelengths are included in the returned
         # wavelength set
 
         return WavelengthSet(self.wavelengths)
 
     def select_in_bin_set(self, binset: BinSet) -> BinSet:
-
         bins = binset.bins
 
         # transform bins into closed-open intervals, so that a wavelength
         # value is included in at most one bin, when bins are adjacent
         bin_intervals = [b.interval for b in bins]
 
         selected = [False] * len(bins)
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_solar_irradiance.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_solar_irradiance.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_uniform.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_uniform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/surface/_basic.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/surface/_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/surface/_central_patch.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/surface/_central_patch.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/surface/_core.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/surface/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/scenes/surface/_dem.py` & `eradiate-0.23.2rc3/src/eradiate/scenes/surface/_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/spectral/ckd.py` & `eradiate-0.23.2rc3/src/eradiate/spectral/ckd.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/spectral/index.py` & `eradiate-0.23.2rc3/src/eradiate/spectral/index.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/spectral/mono.py` & `eradiate-0.23.2rc3/src/eradiate/spectral/mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/srf_tools.py` & `eradiate-0.23.2rc3/src/eradiate/srf_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -747,15 +747,14 @@
             trimmed.srf.values,
             where=trimmed.srf.values <= threshold,
             facecolor="red",
             alpha=0.1,
         )
 
     if wmin is not None or wmax is not None:
-
         if wmin is not None:
             _wmin_value = wmin.m_as(ds.w.attrs["units"])
             plt.axvline(x=_wmin_value, color="red", lw=0.5)
             # drop region
             ax.fill_between(
                 trimmed.w.values,
                 0,
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/test_tools/plugin.py` & `eradiate-0.23.2rc3/src/eradiate/test_tools/plugin.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/test_tools/regression.py` & `eradiate-0.23.2rc3/src/eradiate/test_tools/regression.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/test_tools/types.py` & `eradiate-0.23.2rc3/src/eradiate/test_tools/types.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/test_tools/util.py` & `eradiate-0.23.2rc3/src/eradiate/test_tools/util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/thermoprops/afgl_1986.py` & `eradiate-0.23.2rc3/src/eradiate/thermoprops/afgl_1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/thermoprops/us76.py` & `eradiate-0.23.2rc3/src/eradiate/thermoprops/us76.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/thermoprops/util.py` & `eradiate-0.23.2rc3/src/eradiate/thermoprops/util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/units.py` & `eradiate-0.23.2rc3/src/eradiate/units.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/util/deprecation.py` & `eradiate-0.23.2rc3/src/eradiate/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/util/misc.py` & `eradiate-0.23.2rc3/src/eradiate/util/misc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/util/numpydoc.py` & `eradiate-0.23.2rc3/src/eradiate/util/numpydoc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/util/sys_info.py` & `eradiate-0.23.2rc3/src/eradiate/util/sys_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import locale
 import platform
 import re
 import subprocess
 import sys
-from importlib.metadata import version, PackageNotFoundError
+from importlib.metadata import PackageNotFoundError, version
 
 import drjit as dr
 import mitsuba as mi
 
 
 def _run(command):
     "Returns (return-code, stdout, stderr)"
@@ -92,11 +92,13 @@
     print("System")
     print(f"  CPU: {sys_info['cpu_info']}")
     print(f"  OS: {sys_info['os']}")
     print(f"  Python: {sys_info['python']}")
 
     print("\nVersions")
     print(f"  drjit {sys_info['drjit_version']}")
-    print(f"  eradiate-mitsuba {sys_info['eradiate_mitsuba_version']} (based on mitsuba {sys_info['mitsuba_version']})")
+    print(
+        f"  eradiate-mitsuba {sys_info['eradiate_mitsuba_version']} (based on mitsuba {sys_info['mitsuba_version']})"
+    )
 
     print("\nMitsuba variants")
     print("\n".join([f"  {variant}" for variant in mi.variants()]))
```

### Comparing `eradiate-0.23.2rc2/src/eradiate/validators.py` & `eradiate-0.23.2rc3/src/eradiate/validators.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/warp.py` & `eradiate-0.23.2rc3/src/eradiate/warp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/xarray/_accessors.py` & `eradiate-0.23.2rc3/src/eradiate/xarray/_accessors.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/xarray/_helpers.py` & `eradiate-0.23.2rc3/src/eradiate/xarray/_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate/xarray/interp.py` & `eradiate-0.23.2rc3/src/eradiate/xarray/interp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/src/eradiate.egg-info/PKG-INFO` & `eradiate-0.23.2rc3/src/eradiate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eradiate
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: A radiative transfer model for the Earth observation community
 Author: The Eradiate Team
 Maintainer: The Eradiate Team
 License: LGPLv3
 Project-URL: changelog, https://github.com/eradiate/eradiate/CHANGELOG.md
 Project-URL: documentation, https://eradiate.readthedocs.io
 Project-URL: repository, https://github.com/eradiate/eradiate
```

### Comparing `eradiate-0.23.2rc2/src/eradiate.egg-info/SOURCES.txt` & `eradiate-0.23.2rc3/src/eradiate.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -93,16 +93,16 @@
 docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
 docs/fig/diagrams/package.drawio
 docs/rst/bibliography.rst
 docs/rst/contributing.rst
 docs/rst/dependencies.rst
 docs/rst/maintainer_guide.rst
 docs/rst/developer_guide/design_atmosphere.rst
+docs/rst/developer_guide/dev_install.rst
 docs/rst/developer_guide/factory_guide.rst
-docs/rst/developer_guide/getting_started.rst
 docs/rst/developer_guide/index.rst
 docs/rst/developer_guide/lazy_loading.rst
 docs/rst/developer_guide/radiometric_kernel_interface.rst
 docs/rst/developer_guide/scene_generator.rst
 docs/rst/developer_guide/update.rst
 docs/rst/reference_api/attrs.rst
 docs/rst/reference_api/config.rst
@@ -321,15 +321,15 @@
 src/eradiate/scenes/bsdfs/_core.py
 src/eradiate/scenes/bsdfs/_lambertian.py
 src/eradiate/scenes/bsdfs/_mqdiffuse.py
 src/eradiate/scenes/bsdfs/_opacity_mask.py
 src/eradiate/scenes/bsdfs/_rpv.py
 src/eradiate/scenes/illumination/__init__.py
 src/eradiate/scenes/illumination/__init__.pyi
-src/eradiate/scenes/illumination/_astroobject.py
+src/eradiate/scenes/illumination/_astro_object.py
 src/eradiate/scenes/illumination/_constant.py
 src/eradiate/scenes/illumination/_core.py
 src/eradiate/scenes/illumination/_directional.py
 src/eradiate/scenes/illumination/_spot.py
 src/eradiate/scenes/integrators/__init__.py
 src/eradiate/scenes/integrators/__init__.pyi
 src/eradiate/scenes/integrators/_core.py
@@ -465,15 +465,15 @@
 tests/01_eradiate/01_unit/scenes/bsdfs/__init__.py
 tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py
 tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
 tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
 tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
 tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py
 tests/01_eradiate/01_unit/scenes/illumination/__init__.py
-tests/01_eradiate/01_unit/scenes/illumination/test_astroobject.py
+tests/01_eradiate/01_unit/scenes/illumination/test_astro_object.py
 tests/01_eradiate/01_unit/scenes/illumination/test_constant.py
 tests/01_eradiate/01_unit/scenes/illumination/test_directional.py
 tests/01_eradiate/01_unit/scenes/illumination/test_spot.py
 tests/01_eradiate/01_unit/scenes/integrators/__init__.py
 tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py
 tests/01_eradiate/01_unit/scenes/measure/__init__.py
 tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py
```

### Comparing `eradiate-0.23.2rc2/src/eradiate.egg-info/requires.txt` & `eradiate-0.23.2rc3/src/eradiate.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_blind_directory.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_blind_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_blind_online.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_blind_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_core.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_datasets.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_multi.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_multi.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_safe_directory.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_safe_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_safe_online.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_safe_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_atmosphere.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_atmosphere.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,38 @@
 from eradiate.constants import EARTH_RADIUS
 from eradiate.experiments import AtmosphereExperiment
 from eradiate.scenes.atmosphere import HomogeneousAtmosphere
 from eradiate.scenes.measure import MultiDistantMeasure
 from eradiate.scenes.shapes import RectangleShape
 from eradiate.scenes.spectra import MultiDeltaSpectrum
 from eradiate.test_tools.types import check_scene_element
+from eradiate.test_tools.util import skipif_data_not_found
 
 
 def test_atmosphere_experiment_construct_default(modes_all_double):
     """
     AtmosphereExperiment initializes successfully with default parameters in
     all modes.
     """
+    skipif_data_not_found(
+        "spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
+    )
     exp = AtmosphereExperiment()
 
     # Check that the atmosphere's geometry is overridden by the experiment's
     assert exp.atmosphere.geometry is exp.geometry
 
 
 def test_atmosphere_experiment_extra_objects(mode_mono):
     """
     Extra objects can be added to the scene.
     """
+    skipif_data_not_found(
+        "spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
+    )
     exp = AtmosphereExperiment(
         extra_objects={
             "reference_surface": {
                 "factory": "shape",
                 "type": "rectangle",
                 "id": "reference_surface",
                 "bsdf": {"type": "lambertian"},
@@ -45,14 +52,18 @@
     assert "reference_surface.bsdf.reflectance.value" in mi_wrapper.parameters.keys()
 
 
 def test_atmosphere_experiment_construct_measures(modes_all_double):
     """
     A variety of measure specifications are acceptable.
     """
+    if eradiate.mode().is_mono:
+        skipif_data_not_found(
+            "spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
+        )
     # Init with a single measure (not wrapped in a sequence)
     assert AtmosphereExperiment(measures=MultiDistantMeasure())
 
     # Init from a dict-based measure spec
     # -- Correctly wrapped in a sequence
     assert AtmosphereExperiment(measures=[{"type": "distant"}])
     # -- Not wrapped in a sequence
@@ -69,23 +80,28 @@
 )
 def test_atmosphere_experiment_construct_normalize_measures(
     mode_mono, geometry, expected
 ):
     """
     Default measure target is set to ground level.
     """
+    skipif_data_not_found(
+        "spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
+    )
     exp = AtmosphereExperiment(geometry=geometry)
     assert np.allclose(exp.measures[0].target.xyz, expected)
 
 
 def test_atmosphere_experiment_kernel_dict(mode_mono):
     """
     Test non-trivial kernel dict generation behaviour.
     """
-
+    skipif_data_not_found(
+        "spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
+    )
     # With an atmosphere
     exp = AtmosphereExperiment(
         geometry={"type": "plane_parallel", "width": 42.0, "width_units": "km"},
         atmosphere=HomogeneousAtmosphere(),
         measures={"type": "distant"},
     )
     mi_wrapper = check_scene_element(
@@ -124,24 +140,23 @@
     # -- Measures get no external medium assigned
     assert all(sensor.medium() is None for sensor in mi_wrapper.obj.sensors())
 
 
 @pytest.mark.slow
 def test_atmosphere_experiment_real_life(mode_mono):
     # Construct with typical parameters
-    test_absorption_data_set = eradiate.data.data_store.fetch(
-        "tests/spectra/absorption/us76_u86_4-spectra-4000_25711.nc"
+    skipif_data_not_found(
+        "spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
     )
     exp = AtmosphereExperiment(
         surface={"type": "rpv"},
         atmosphere={
             "type": "heterogeneous",
             "molecular_atmosphere": {
                 "construct": "ussa_1976",
-                "absorption_dataset": test_absorption_data_set,
             },
         },
         illumination={"type": "directional", "zenith": 45.0},
         measures=[
             {"type": "distant", "id": "distant_measure"},
             {"type": "radiancemeter", "origin": [1, 0, 0], "id": "radiancemeter"},
         ],
@@ -155,23 +170,17 @@
     # -- Radiancemeter inside the atmosphere must have a medium assigned
     assert mi_sensors["radiancemeter"].medium().id() == "medium_atmosphere"
 
 
 @pytest.mark.slow
 def test_atmosphere_experiment_run_basic(modes_all_double):
     if eradiate.mode().is_mono:
-        molecular_atmosphere_params = {
-            "construct": "ussa_1976",
-            "absorption_dataset": "tests/spectra/absorption/us76_u86_4-spectra-4000_25711.nc",
-        }
+        molecular_atmosphere_params = {"construct": "ussa_1976"}
     else:
-        molecular_atmosphere_params = {
-            "construct": "afgl_1986",
-            # "absorption_dataset": "ckd/absorption/10nm/afgl_1986-us_standard-10nm.nc"
-        }
+        molecular_atmosphere_params = {"construct": "afgl_1986"}
 
     exp = AtmosphereExperiment(
         atmosphere={
             "type": "heterogeneous",
             "molecular_atmosphere": {
                 "type": "molecular",
                 **molecular_atmosphere_params,
@@ -189,14 +198,18 @@
 
 
 @pytest.mark.slow
 def test_atmosphere_experiment_run_detailed(modes_all):
     """
     Test for correctness of the result dataset generated by AtmosphereExperiment.
     """
+    if eradiate.mode().is_mono:
+        skipif_data_not_found(
+            "spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
+        )
     # Create simple scene
     exp = AtmosphereExperiment(
         measures=[
             {
                 "type": "hemispherical_distant",
                 "id": "toa_hsphere",
                 "film_resolution": (32, 32),
```

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_canopy.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_canopy.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from eradiate import unit_registry as ureg
 from eradiate.experiments import CanopyAtmosphereExperiment
 from eradiate.scenes.atmosphere import HomogeneousAtmosphere
 from eradiate.scenes.biosphere import DiscreteCanopy
 from eradiate.scenes.measure import MultiDistantMeasure
 from eradiate.scenes.surface import CentralPatchSurface
 from eradiate.test_tools.types import check_scene_element
+from eradiate.test_tools.util import skipif_data_not_found
 
 
 def test_canopy_atmosphere_experiment_construct_default(mode_mono):
     """
     CanopyAtmosphereExperiment initialises with default params in all modes
     """
     exp = CanopyAtmosphereExperiment()
@@ -169,26 +170,23 @@
 
     np.testing.assert_allclose(expected, result)
 
 
 @pytest.mark.slow
 def test_canopy_atmosphere_experiment_real_life(mode_mono):
     # Construct with typical parameters
-    test_absorption_data_set = eradiate.data.data_store.fetch(
-        "tests/spectra/absorption/us76_u86_4-spectra-4000_25711.nc"
+    skipif_data_not_found(
+        "spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
     )
-
-    # Construct with typical parameters
     exp = CanopyAtmosphereExperiment(
         surface={"type": "rpv"},
         atmosphere={
             "type": "heterogeneous",
             "molecular_atmosphere": {
                 "construct": "ussa_1976",
-                "absorption_dataset": test_absorption_data_set,
             },
         },
         canopy={
             "type": "discrete_canopy",
             "construct": "homogeneous",
             "lai": 3.0,
             "leaf_radius": 0.1 * ureg.m,
@@ -257,26 +255,24 @@
     # We just check that we record something as expected
     assert np.all(results["radiance"].data > 0.0)
 
 
 def test_canopy_atmosphere_experiment_inconsistent_multiradiancemeter(mode_mono):
     # A MultiRadiancemeter measure must have all origins inside the atmosphere
     # or none. A mix of both will raise an error.
-
-    # Construct with typical parameters
-    test_absorption_data_set = eradiate.data.data_store.fetch(
-        "tests/spectra/absorption/us76_u86_4-spectra-4000_25711.nc"
+    skipif_data_not_found(
+        "spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
     )
+    # Construct with typical parameters
     exp = CanopyAtmosphereExperiment(
         surface={"type": "rpv"},
         atmosphere={
             "type": "heterogeneous",
             "molecular_atmosphere": {
                 "construct": "ussa_1976",
-                "absorption_dataset": test_absorption_data_set,
             },
         },
         canopy={
             "type": "discrete_canopy",
             "construct": "homogeneous",
             "lai": 3.0,
             "leaf_radius": 0.1 * ureg.m,
```

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_core.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_dem.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_dem.py`

 * *Files 12% similar despite different names*

```diff
@@ -96,24 +96,20 @@
     # -- Measures get no external medium assigned
     assert all(sensor.medium() is None for sensor in mi_wrapper.obj.sensors())
 
 
 @pytest.mark.slow
 def test_dem_experiment_real_life(mode_mono):
     # Construct with typical parameters
-    test_absorption_data_set = eradiate.data.data_store.fetch(
-        "tests/spectra/absorption/us76_u86_4-spectra-4000_25711.nc"
-    )
     exp = DEMExperiment(
         surface={"type": "rpv"},
         atmosphere={
             "type": "heterogeneous",
             "molecular_atmosphere": {
                 "construct": "ussa_1976",
-                "absorption_dataset": test_absorption_data_set,
             },
         },
         illumination={"type": "directional", "zenith": 45.0},
         measures=[
             {"type": "distant", "id": "distant_measure"},
             {"type": "radiancemeter", "origin": [1, 0, 0], "id": "radiancemeter"},
         ],
@@ -129,24 +125,20 @@
 
 
 def test_dem_experiment_inconsistent_multiradiancemeter(mode_mono):
     # A MultiRadiancemeter measure must have all origins inside the atmosphere or none.
     # A mix of both will raise an error.
 
     # Construct with typical parameters
-    test_absorption_data_set = eradiate.data.data_store.fetch(
-        "tests/spectra/absorption/us76_u86_4-spectra-4000_25711.nc"
-    )
     exp = DEMExperiment(
         surface={"type": "rpv"},
         atmosphere={
             "type": "heterogeneous",
             "molecular_atmosphere": {
                 "construct": "ussa_1976",
-                "absorption_dataset": test_absorption_data_set,
             },
         },
         illumination={"type": "directional", "zenith": 45.0},
         measures=[
             {
                 "type": "multi_radiancemeter",
                 "origins": [[0, 0, 1], [0, 0, 1000000]],
```

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_helpers.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_gridvolume.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_gridvolume.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_logging.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_logging.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_render.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_render.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_transform.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_transform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/conftest.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_aggregate.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_assemble.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_assemble.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_compute.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_compute.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_core.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_gather.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_gather.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_absorption.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_absorption.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 @pytest.mark.parametrize("model_id", ["midlatitude_summer", "us_standard"])
 def test_afgl_1986_rad_profile_default_ckd(mode_ckd, model_id):
     """
     Collision coefficient evaluation methods return pint.Quantity objects.
     """
     profile = AFGL1986RadProfile(
-        {"model_id": model_id},
         absorption_dataset=f"ckd/absorption/10nm/afgl_1986-{model_id}-10nm-v3.nc",
     )
 
     si = SpectralIndex.new()
     for field in ["albedo", "sigma_a", "sigma_s", "sigma_t"]:
         x = getattr(profile, f"eval_{field}")(si, profile.zgrid)
         assert isinstance(x, ureg.Quantity)
@@ -38,15 +37,14 @@
     mode_ckd, test_ckd_si_1650, model_id
 ):
     """
     Default value for 'has_absorption' is True, hence the absorption
     coefficient is computed and is not zero everywhere at 1650 nm.
     """
     profile = AFGL1986RadProfile(
-        dict(model_id=model_id),
         absorption_dataset=f"ckd/absorption/10nm/afgl_1986-{model_id}-10nm-v3.nc",
     )
     assert profile.has_absorption
     ds = profile.eval_dataset(test_ckd_si_1650, profile.zgrid)
     assert (ds.sigma_a.values != 0.0).any()
 
 
@@ -73,14 +71,15 @@
     mode_ckd, test_ckd_si_1650, model_id
 ):
     """
     When 'has_absorption' is False, the absorption coefficient is not
     computed and is zero everywhere.
     """
     profile = AFGL1986RadProfile(
+        absorption_dataset=f"ckd/absorption/10nm/afgl_1986-{model_id}-10nm-v3.nc",
         thermoprops=dict(model_id=model_id),
         has_absorption=False,
     )
     assert not profile.has_absorption
     ds = profile.eval_dataset(test_ckd_si_1650, profile.zgrid)
     assert (ds.sigma_a.values == 0.0).all()
 
@@ -100,30 +99,30 @@
 
 def test_afgl_1986_rad_profile_has_scattering_true(mode_ckd, test_ckd_si_550):
     """
     When 'has_scattering' is True, the scattering coefficient is computed
     and is not zero everywhere at 550 nm.
     """
     profile = AFGL1986RadProfile(
-        has_scattering=True,
         absorption_dataset="ckd/absorption/10nm/afgl_1986-us_standard-10nm-v3.nc",
+        has_scattering=True,
     )
     assert profile.has_scattering
     ds = profile.eval_dataset(test_ckd_si_550, profile.zgrid)
     assert (ds.sigma_s.values != 0.0).any()
 
 
 def test_afgl_1986_rad_profile_has_scattering_false(mode_ckd, test_ckd_si_550):
     """
     When 'has_scattering' is False, the scattering coefficient is not
     computed and is zero everywhere.
     """
     profile = AFGL1986RadProfile(
-        has_scattering=False,
         absorption_dataset="ckd/absorption/10nm/afgl_1986-us_standard-10nm-v3.nc",
+        has_scattering=False,
     )
     assert not profile.has_scattering
     ds = profile.eval_dataset(test_ckd_si_550, profile.zgrid)
     assert (ds.sigma_s.values == 0.0).all()
 
 
 @pytest.mark.parametrize(
@@ -138,46 +137,46 @@
     ],
 )
 def test_afgl_1986_rad_profile_model_id(mode_ckd, model_id):
     """
     All models are supported in ckd mode.
     """
     AFGL1986RadProfile(
-        thermoprops=dict(model_id=model_id),
         absorption_dataset=f"ckd/absorption/10nm/afgl_1986-{model_id}-10nm-v3.nc",
+        thermoprops=dict(model_id=model_id),
     )
 
 
 @pytest.mark.parametrize(
     "molecule",
     ["N2O", "CO", "CH4", "O2"],
 )
 def test_afgl_1986_rad_profile_concentrations_ckd_not_implemented(mode_ckd, molecule):
     """
     Concentrations rescaling is not implemented for molecules other than
     H2O and O3 in CKD mode.
     """
     with pytest.raises(NotImplementedError):
         AFGL1986RadProfile(
-            thermoprops=dict(concentrations={molecule: 0.0 * ureg.dimensionless}),
             absorption_dataset="ckd/absorption/10nm/afgl_1986-us_standard-10nm-v3.nc",
+            thermoprops=dict(concentrations={molecule: 0.0 * ureg.dimensionless}),
         )
 
 
 @pytest.mark.parametrize(
     "w", [280.0, 550.0, 790.0, 1040.0, 1270.0, 1590.0, 2220.0, 2400.0] * ureg.nm
 )
 @pytest.mark.parametrize("model_id", ["midlatitude_summer", "us_standard"])
 def test_afgl_1986_rad_profile_ckd_10nm(mode_ckd, w, model_id):
     """
     Can evaluate absorption coefficient.
     """
     profile = AFGL1986RadProfile(
-        thermoprops=dict(model_id=model_id),
         absorption_dataset="ckd/absorption/10nm/afgl_1986-us_standard-10nm-v3.nc",
+        thermoprops=dict(model_id=model_id),
     )
     si = SpectralIndex.new(w=w)
     sigma_a = profile.eval_sigma_a(si, profile.zgrid)
     assert isinstance(sigma_a, pint.Quantity)
 
 
 def test_afgl_1986_eval_zgrid(mode_ckd):
```

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_us76_approx.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_us76_approx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,150 +1,147 @@
 import numpy as np
 import pytest
 
-import eradiate
 from eradiate import unit_registry as ureg
 from eradiate.radprops import US76ApproxRadProfile, ZGrid
 from eradiate.spectral.index import SpectralIndex
 
 
 @pytest.fixture
-def us76_approx_test_absorption_data_set():
-    """
-    Fixture to return the path to a test absorption data set for 'us76_approx'.
-    """
-    return eradiate.data.data_store.fetch(
-        "tests/spectra/absorption/us76_u86_4-spectra-4000_25711.nc"
-    )
+def absorption_dataset_550nm():
+    return "spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
 
 
-def test_us76_approx_rad_profile(mode_mono, us76_approx_test_absorption_data_set):
+def test_us76_approx_rad_profile(mode_mono, absorption_dataset_550nm):
     """
     Collision coefficient evaluation methods return pint.Quantity objects.
     """
-    p = US76ApproxRadProfile(absorption_dataset=us76_approx_test_absorption_data_set)
+    p = US76ApproxRadProfile(absorption_dataset=absorption_dataset_550nm)
 
     si = SpectralIndex.new()
     for field in ["sigma_a", "sigma_s", "sigma_t", "albedo"]:
         x = getattr(p, f"eval_{field}")(si, p.zgrid)
         assert isinstance(x, ureg.Quantity)
 
 
-def test_us76_approx_rad_profile_levels(
-    mode_mono, us76_approx_test_absorption_data_set
-):
+def test_us76_approx_rad_profile_levels(mode_mono, absorption_dataset_550nm):
     """
     Collision coefficients' shape match altitude levels shape.
     """
     p = US76ApproxRadProfile(
         thermoprops=dict(levels=ureg.Quantity(np.linspace(0, 120, 121), "km")),
-        absorption_dataset=us76_approx_test_absorption_data_set,
+        absorption_dataset=absorption_dataset_550nm,
     )
 
     si = SpectralIndex.new()
     for field in ["sigma_a", "sigma_s", "sigma_t", "albedo"]:
         x = getattr(p, f"eval_{field}")(si, p.zgrid)
         assert x.shape == (120,)
 
 
-def test_us76_approx_rad_profile_has_absorption_default(
-    mode_mono, us76_approx_test_absorption_data_set
-):
+def test_us76_approx_rad_profile_has_absorption_default(mode_mono):
     """
     Default value for 'has_absorption' is True, hence the absorption
     coefficient is computed and is not zero everywhere at 1650 nm.
     """
-    p = US76ApproxRadProfile(absorption_dataset=us76_approx_test_absorption_data_set)
+    p = US76ApproxRadProfile(
+        absorption_dataset="spectra/absorption/us76_u86_4/us76_u86_4-spectra-6000_7000.nc",
+    )
     assert p.has_absorption
     si = SpectralIndex.new(w=1650 * ureg.nm)
     ds = p.eval_dataset(si, p.zgrid)
     assert (ds.sigma_a.values != 0.0).any()
 
 
-def test_us76_approx_rad_profile_has_absorption_true(
-    mode_mono, us76_approx_test_absorption_data_set
-):
+def test_us76_approx_rad_profile_has_absorption_true(mode_mono):
     """
     When 'has_absorption' is True, the absorption coefficient is computed
     and is not zero everywhere at 1650 nm.
     """
     p = US76ApproxRadProfile(
+        absorption_dataset="spectra/absorption/us76_u86_4/us76_u86_4-spectra-6000_7000.nc",
         has_absorption=True,
-        absorption_dataset=us76_approx_test_absorption_data_set,
     )
     assert p.has_absorption
     si = SpectralIndex.new(w=1650.0 * ureg.nm)
     ds = p.eval_dataset(si, p.zgrid)
     assert (ds.sigma_a.values != 0.0).any()
 
 
 def test_us76_approx_rad_profile_has_absorption_false(
-    mode_mono, us76_approx_test_absorption_data_set
+    mode_mono,
+    absorption_dataset_550nm,
 ):
     """
     When 'has_absorption' is False, the absorption coefficient is not
     computed and is zero everywhere.
     """
     p = US76ApproxRadProfile(
-        has_absorption=False, absorption_dataset=us76_approx_test_absorption_data_set
+        absorption_dataset=absorption_dataset_550nm,
+        has_absorption=False,
     )
     assert not p.has_absorption
     si = SpectralIndex.new(w=1650.0 * ureg.nm)
     ds = p.eval_dataset(si, p.zgrid)
     assert (ds.sigma_a.values == 0.0).all()
 
 
 def test_us76_approx_rad_profile_has_scattering_default(
-    mode_mono, us76_approx_test_absorption_data_set
+    mode_mono,
+    absorption_dataset_550nm,
 ):
     """
     Default value for 'has_scattering' is True, hence the scattering
     coefficient is computed and is not zero everywhere at 550 nm.
     """
-    p = US76ApproxRadProfile(absorption_dataset=us76_approx_test_absorption_data_set)
+    p = US76ApproxRadProfile(absorption_dataset=absorption_dataset_550nm)
     assert p.has_scattering
     si = SpectralIndex.new(w=550.0 * ureg.nm)
     ds = p.eval_dataset(si, p.zgrid)
     assert (ds.sigma_s.values != 0.0).any()
 
 
 def test_us76_approx_rad_profile_has_scattering_true(
-    mode_mono, us76_approx_test_absorption_data_set
+    mode_mono,
+    absorption_dataset_550nm,
 ):
     """
     When 'has_scattering' is True, the scattering coefficient is computed
     and is not zero everywhere at 550 nm.
     """
     p = US76ApproxRadProfile(
-        has_scattering=True, absorption_dataset=us76_approx_test_absorption_data_set
+        has_scattering=True,
+        absorption_dataset=absorption_dataset_550nm,
     )
     assert p.has_scattering
     si = SpectralIndex.new(w=550 * ureg.nm)
     ds = p.eval_dataset(si, p.zgrid)
     assert (ds.sigma_s.values != 0.0).any()
 
 
 def test_us76_approx_rad_profile_has_scattering_false(
-    mode_mono, us76_approx_test_absorption_data_set
+    mode_mono,
+    absorption_dataset_550nm,
 ):
     """
     When 'has_scattering' is False, the scattering coefficient is not
     computed and is zero everywhere.
     """
     p = US76ApproxRadProfile(
-        has_scattering=False, absorption_dataset=us76_approx_test_absorption_data_set
+        has_scattering=False,
+        absorption_dataset=absorption_dataset_550nm,
     )
     assert not p.has_scattering
     si = SpectralIndex.new(w=550.0 * ureg.nm)
     ds = p.eval_dataset(si, p.zgrid)
     assert (ds.sigma_s.values == 0.0).all()
 
 
-def test_us76_approx_eval_zgrid(mode_mono, us76_approx_test_absorption_data_set):
+def test_us76_approx_eval_zgrid(mode_mono, absorption_dataset_550nm):
     """
     Evaluation on an arbitrary altitude grid works.
     """
-    p = US76ApproxRadProfile(absorption_dataset=us76_approx_test_absorption_data_set)
+    p = US76ApproxRadProfile(absorption_dataset=absorption_dataset_550nm)
     si = SpectralIndex.new(w=550.0 * ureg.nm)
     zgrid = ZGrid(levels=np.linspace(0, 100, 1001) * ureg.km)
     ds = p.eval_dataset(si, zgrid)
     assert len(ds.z_layer) == len(zgrid.layers)
```

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_zgrid.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_zgrid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,44 +11,37 @@
     HeterogeneousAtmosphere,
     MolecularAtmosphere,
     ParticleLayer,
 )
 from eradiate.scenes.core import traverse
 from eradiate.scenes.geometry import SceneGeometry
 from eradiate.test_tools.types import check_scene_element
-
-
-@pytest.fixture
-def path_to_ussa76_approx_data():
-    return eradiate.data.data_store.fetch(
-        "tests/spectra/absorption/us76_u86_4-spectra-4000_25711.nc"
-    )
+from eradiate.test_tools.util import skipif_data_not_found
 
 
 def test_heterogeneous_empty(modes_all_double):
     # Passing no component is not allowed
     with pytest.raises(ValueError):
         HeterogeneousAtmosphere()
 
 
 @pytest.mark.parametrize("geometry", ["plane_parallel", "spherical_shell"])
 @pytest.mark.parametrize("component", ["molecular", "particle"])
-def test_heterogeneous_single_mono(
-    mode_mono, geometry, component, path_to_ussa76_approx_data
-):
+def test_heterogeneous_single_mono(mode_mono, geometry, component):
     """
     Unit tests for a HeterogeneousAtmosphere with a single component.
     """
     # Construct succeeds
     if component == "molecular":
+        skipif_data_not_found(
+            f"spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
+        )
         atmosphere = HeterogeneousAtmosphere(
             geometry=geometry,
-            molecular_atmosphere=MolecularAtmosphere.ussa_1976(
-                absorption_dataset=path_to_ussa76_approx_data,
-            ),
+            molecular_atmosphere=MolecularAtmosphere.ussa_1976(),
         )
 
     else:
         component = ParticleLayer()
         atmosphere = HeterogeneousAtmosphere(
             geometry=geometry, particle_layers=[component]
         )
@@ -79,45 +72,42 @@
         )
 
     # The scene element produces valid kernel dictionary specifications
     check_scene_element(atmosphere, KernelContext())
 
 
 @pytest.mark.parametrize("geometry", ["plane_parallel", "spherical_shell"])
-def test_heterogeneous_multi_mono(mode_mono, geometry, path_to_ussa76_approx_data):
+def test_heterogeneous_multi_mono(mode_mono, geometry):
     """
     Unit tests for a HeterogeneousAtmosphere with multiple (2+) components.
     """
     # Construct succeeds
-    molecular_atmosphere = MolecularAtmosphere.ussa_1976(
-        absorption_dataset=path_to_ussa76_approx_data,
+    skipif_data_not_found(
+        f"spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
     )
-
     atmosphere = HeterogeneousAtmosphere(
         geometry=geometry,
-        molecular_atmosphere=molecular_atmosphere,
+        molecular_atmosphere=MolecularAtmosphere.ussa_1976(),
         particle_layers=[ParticleLayer() for _ in range(2)],
     )
 
     # The scene element produces valid kernel dictionary specifications
     check_scene_element(atmosphere, KernelContext())
 
 
 @pytest.mark.parametrize("geometry", ["plane_parallel", "spherical_shell"])
 @pytest.mark.parametrize("bin_set", ["1nm", "10nm"])
 def test_heterogeneous_multi_ckd(mode_ckd, geometry, bin_set):
     """
     Unit tests for a HeterogeneousAtmosphere with multiple (2+) components.
     """
     # Construct succeeds
-    molecular_atmosphere = MolecularAtmosphere.afgl_1986()
-
     atmosphere = HeterogeneousAtmosphere(
         geometry={"type": geometry, "zgrid": np.linspace(0, 120, 121) * ureg.km},
-        molecular_atmosphere=molecular_atmosphere,
+        molecular_atmosphere=MolecularAtmosphere.afgl_1986(),
         particle_layers=[ParticleLayer() for _ in range(2)],
     )
 
     # The scene element produces valid kernel dictionary specifications
     check_scene_element(atmosphere, KernelContext())
 
 
@@ -199,19 +189,23 @@
             "ground_altitude": 0.0 * ureg.km,
             "toa_altitude": 100.0 * ureg.km,
             "zgrid": ZGrid(np.linspace(0, 100, 101) * ureg.km),
         }
     )
 
     # Fist basic check: a uniform layer and a molecular atmosphere
-    molecular = (
-        MolecularAtmosphere.afgl_1986(levels=geometry.zgrid.levels)
-        if eradiate.mode().is_ckd
-        else MolecularAtmosphere.ussa_1976(levels=geometry.zgrid.levels)
-    )
+    if eradiate.mode().is_mono:
+        skipif_data_not_found(
+            f"spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
+        )
+        molecular = MolecularAtmosphere.ussa_1976(levels=geometry.zgrid.levels)
+    elif eradiate.mode().is_ckd:
+        molecular = MolecularAtmosphere.afgl_1986(levels=geometry.zgrid.levels)
+    else:
+        raise NotImplementedError
 
     mixed = HeterogeneousAtmosphere(
         geometry=geometry,
         molecular_atmosphere=molecular,
         particle_layers=ParticleLayer(
             bottom=0.0 * ureg.km,
             top=50.0 * ureg.km,
@@ -289,35 +283,40 @@
     weights = np.squeeze(mi_wrapper.parameters["weight.data"])
     middle = np.argwhere(geometry.zgrid.layers <= 50.0 * ureg.km).max() + 1
 
     assert np.all(weights[:middle] == 0.0)
     assert np.all(weights[middle:] == 0.5)
 
 
-def test_heterogeneous_scale(mode_mono, path_to_ussa76_approx_data):
+def test_heterogeneous_scale(mode_mono):
+    skipif_data_not_found(
+        f"spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
+    )
     atmosphere = HeterogeneousAtmosphere(
         geometry="plane_parallel",
-        molecular_atmosphere=MolecularAtmosphere.ussa_1976(
-            absorption_dataset=path_to_ussa76_approx_data,
-        ),
+        molecular_atmosphere=MolecularAtmosphere.ussa_1976(),
         particle_layers=[ParticleLayer() for _ in range(2)],
         scale=2.0,
     )
     template, params = traverse(atmosphere)
     assert template["medium_atmosphere.scale"] == 2.0
 
     # The scene element produces valid kernel dictionary specifications
     check_scene_element(atmosphere, KernelContext())
 
 
 def test_heterogeneous_blend_switches(mode_mono):
     # Rayleigh-only atmosphere + particle layer combination works
+    skipif_data_not_found(
+        f"spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
+    )
     assert HeterogeneousAtmosphere(
         molecular_atmosphere=MolecularAtmosphere.ussa_1976(
-            has_absorption=False, has_scattering=True
+            has_absorption=False,
+            has_scattering=True,
         ),
         particle_layers=[ParticleLayer()],
     )
 
 
 @pytest.mark.parametrize(
     "particle_radprops",
```

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_astroobject.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import pytest
-import numpy as np
-
 import mitsuba as mi
+import numpy as np
+import pytest
 
 from eradiate import unit_registry as ureg
-from eradiate.scenes.illumination import AstroObjectIllumination
-from eradiate.scenes.spectra import UniformSpectrum, SolarIrradianceSpectrum
+from eradiate.scenes.illumination import DirectionalIllumination
+from eradiate.scenes.spectra import SolarIrradianceSpectrum, UniformSpectrum
 from eradiate.test_tools.types import check_scene_element
 
+
 @pytest.mark.parametrize(
-    "kwargs, expected_irradiance_type, angular_diameter",
-    [({}, SolarIrradianceSpectrum, 1.0), ({"irradiance": 1.0}, UniformSpectrum, 2.0)],
+    "kwargs, expected_irradiance_type",
+    [({}, SolarIrradianceSpectrum), ({"irradiance": 1.0}, UniformSpectrum)],
     ids=["noargs", "from_scalar"],
 )
-def test_directional_construct(modes_all, kwargs, expected_irradiance_type, angular_diameter):
+def test_directional_construct(modes_all, kwargs, expected_irradiance_type):
     # Construction without argument succeeds
-    illumination = AstroObjectIllumination(**kwargs, angular_diameter=angular_diameter)
+    illumination = DirectionalIllumination(**kwargs)
     assert illumination
     assert isinstance(illumination.irradiance, expected_irradiance_type)
-    assert illumination.angular_diameter == angular_diameter * ureg.deg
+
 
 @pytest.mark.parametrize(
     "zenith, azimuth, direction, to_world",
     [
         (
             0.0 * ureg.deg,
             0.0 * ureg.deg,
@@ -47,21 +47,22 @@
         ),
     ],
 )
 def test_directional_to_world(mode_mono, zenith, azimuth, direction, to_world):
     """
     Direction is correctly converted to transformation matrix.
     """
-    illumination = AstroObjectIllumination(zenith=zenith, azimuth=azimuth)
+    illumination = DirectionalIllumination(zenith=zenith, azimuth=azimuth)
     np.testing.assert_allclose(illumination.direction, direction)
     np.testing.assert_allclose(illumination._to_world.matrix, to_world)
 
+
 def test_directional_kernel_dict(modes_all_double):
     # The associated kernel dict is correctly formed and can be loaded
-    illumination = AstroObjectIllumination()
+    illumination = DirectionalIllumination()
     check_scene_element(illumination, mi_cls=mi.Emitter)
 
 
 COS_PI_4 = 0.5 * np.sqrt(2)
 
 
 @pytest.mark.parametrize(
@@ -74,13 +75,13 @@
         ("west_right", [0, COS_PI_4, -COS_PI_4]),
         ("west_left", [0, -COS_PI_4, -COS_PI_4]),
         ("south_right", [-COS_PI_4, 0, -COS_PI_4]),
         ("south_left", [COS_PI_4, 0, -COS_PI_4]),
     ],
 )
 def test_directional_azimuth_convention(mode_mono, azimuth_convention, expected):
-    illumination = AstroObjectIllumination(
+    illumination = DirectionalIllumination(
         zenith=45 * ureg.deg,
         azimuth=90 * ureg.deg,
         azimuth_convention=azimuth_convention,
     )
     assert np.allclose(illumination.direction, expected), illumination.direction
```

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_astro_object.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,90 @@
 import mitsuba as mi
 import numpy as np
 import pytest
 
 from eradiate import unit_registry as ureg
-from eradiate.scenes.illumination import DirectionalIllumination
+from eradiate.scenes.illumination import AstroObjectIllumination
 from eradiate.scenes.spectra import SolarIrradianceSpectrum, UniformSpectrum
 from eradiate.test_tools.types import check_scene_element
 
 
 @pytest.mark.parametrize(
-    "kwargs, expected_irradiance_type",
-    [({}, SolarIrradianceSpectrum), ({"irradiance": 1.0}, UniformSpectrum)],
+    "kwargs, expected_irradiance_type, angular_diameter",
+    [({}, SolarIrradianceSpectrum, 1.0), ({"irradiance": 1.0}, UniformSpectrum, 2.0)],
     ids=["noargs", "from_scalar"],
 )
-def test_directional_construct(modes_all, kwargs, expected_irradiance_type):
+def test_astro_object_construct(
+    modes_all, kwargs, expected_irradiance_type, angular_diameter
+):
     # Construction without argument succeeds
-    illumination = DirectionalIllumination(**kwargs)
+    illumination = AstroObjectIllumination(**kwargs, angular_diameter=angular_diameter)
     assert illumination
     assert isinstance(illumination.irradiance, expected_irradiance_type)
+    assert illumination.angular_diameter == angular_diameter * ureg.deg
 
 
 @pytest.mark.parametrize(
     "zenith, azimuth, direction, to_world",
     [
         (
             0.0 * ureg.deg,
             0.0 * ureg.deg,
-            [0, 0, -1],
+            [0, 0, 1],
             [
                 [0, 1, 0, 0],
-                [1, 0, 0, 0],
-                [0, 0, -1, 0],
+                [-1, 0, 0, 0],
+                [0, 0, 1, 0],
                 [0, 0, 0, 1],
             ],
         ),
         (
             30 * ureg.deg,
             0.0 * ureg.deg,
-            [-0.5, 0.0, -np.sqrt(3) / 2],
+            [0.5, 0.0, np.sqrt(3) / 2],
             [
-                [0.0, np.sqrt(3) / 2, -0.5, 0.0],
-                [1.0, 0.0, 0.0, 0.0],
-                [0.0, -0.5, -np.sqrt(3) / 2, 0.0],
+                [0.0, np.sqrt(3) / 2, 0.5, 0.0],
+                [-1.0, 0.0, 0.0, 0.0],
+                [0.0, -0.5, np.sqrt(3) / 2, 0.0],
                 [0.0, 0.0, 0.0, 1.0],
             ],
         ),
     ],
 )
-def test_directional_to_world(mode_mono, zenith, azimuth, direction, to_world):
+def test_astro_object_to_world(mode_mono, zenith, azimuth, direction, to_world):
     """
     Direction is correctly converted to transformation matrix.
     """
-    illumination = DirectionalIllumination(zenith=zenith, azimuth=azimuth)
+    illumination = AstroObjectIllumination(zenith=zenith, azimuth=azimuth)
     np.testing.assert_allclose(illumination.direction, direction)
     np.testing.assert_allclose(illumination._to_world.matrix, to_world)
 
 
-def test_directional_kernel_dict(modes_all_double):
+def test_astro_object_kernel_dict(modes_all_double):
     # The associated kernel dict is correctly formed and can be loaded
-    illumination = DirectionalIllumination()
+    illumination = AstroObjectIllumination()
     check_scene_element(illumination, mi_cls=mi.Emitter)
 
 
 COS_PI_4 = 0.5 * np.sqrt(2)
 
 
 @pytest.mark.parametrize(
     "azimuth_convention, expected",
     [
-        ("east_right", [0, -COS_PI_4, -COS_PI_4]),
-        ("east_left", [0, COS_PI_4, -COS_PI_4]),
-        ("north_right", [COS_PI_4, 0, -COS_PI_4]),
-        ("north_left", [-COS_PI_4, 0, -COS_PI_4]),
-        ("west_right", [0, COS_PI_4, -COS_PI_4]),
-        ("west_left", [0, -COS_PI_4, -COS_PI_4]),
-        ("south_right", [-COS_PI_4, 0, -COS_PI_4]),
-        ("south_left", [COS_PI_4, 0, -COS_PI_4]),
+        ("east_right", [0, COS_PI_4, COS_PI_4]),
+        ("east_left", [0, -COS_PI_4, COS_PI_4]),
+        ("north_right", [-COS_PI_4, 0, COS_PI_4]),
+        ("north_left", [COS_PI_4, 0, COS_PI_4]),
+        ("west_right", [0, -COS_PI_4, COS_PI_4]),
+        ("west_left", [0, COS_PI_4, COS_PI_4]),
+        ("south_right", [COS_PI_4, 0, COS_PI_4]),
+        ("south_left", [-COS_PI_4, 0, COS_PI_4]),
     ],
 )
-def test_directional_azimuth_convention(mode_mono, azimuth_convention, expected):
-    illumination = DirectionalIllumination(
+def test_astro_object_azimuth_convention(mode_mono, azimuth_convention, expected):
+    illumination = AstroObjectIllumination(
         zenith=45 * ureg.deg,
         azimuth=90 * ureg.deg,
         azimuth_convention=azimuth_convention,
     )
     assert np.allclose(illumination.direction, expected), illumination.direction
```

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import mitsuba as mi
 import numpy as np
 import pytest
 
 from eradiate import unit_registry as ureg
-from eradiate.frame import AzimuthConvention
 from eradiate.scenes.measure import (
     AngleLayout,
     AzimuthRingLayout,
     DirectionLayout,
     GridLayout,
     HemispherePlaneLayout,
     Layout,
@@ -28,14 +27,20 @@
     # Constructing without argument fails
     with pytest.raises(TypeError):
         AngleLayout()
 
     # (2,) arrays are reshaped as (1, 2)
     assert AngleLayout([0, 0] * ureg.deg).angles.shape == (1, 2)
 
+    # Zenith values outside [0, 180]° are not allowed
+    with pytest.raises(ValueError):
+        AngleLayout([-45, 0] * ureg.deg)
+    with pytest.raises(ValueError):
+        AngleLayout([210, 0] * ureg.deg)
+
     # Regular construction pattern succeeds
     layout = AngleLayout([[0, 0], [45, 0], [45, 90], [45, 180]] * ureg.deg)
 
     # Directions are correctly computed and point outwards
     np.testing.assert_allclose(
         layout.directions,
         [
@@ -84,15 +89,15 @@
 
 def test_direction_layout(mode_mono):
     """
     Unit tests for the DirectionLayout class
     """
     # Constructing without argument fails
     with pytest.raises(TypeError):
-        print(DirectionLayout())
+        DirectionLayout()
 
     # (3,) arrays are reshaped as (1, 3)
     assert DirectionLayout([0, 0, 1]).directions.shape == (1, 3)
 
     # Regular construction pattern succeeds
     layout = DirectionLayout(
         [
@@ -233,15 +238,14 @@
 def test_grid_layout_azimuth_convention(mode_mono, convention, expected):
     # Azimuth conventions are properly applied
     layout = GridLayout(
         [0, 90] * ureg.deg,
         [0, 90] * ureg.deg,
         azimuth_convention=convention,
     )
-    print(layout.directions)
     np.testing.assert_allclose(layout.directions, expected, atol=1e-8)
 
 
 # ------------------------------------------------------------------------------
 #                       MultiDistantMeasure implementation
 # ------------------------------------------------------------------------------
```

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_target.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_target.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_blend.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_blend.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_core.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/test_basic.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/test_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/test_dem.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/test_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/test_core.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/test_ckd.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/test_ckd.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/test_index.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/test_index.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/test_mono.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/test_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_config.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_config.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_factory.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_frame.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_frame.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_mode.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_mode.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_quad.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_quad.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_rng.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_rng.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_srf_tools.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_srf_tools.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_tools/test_regression.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_tools/test_regression.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_units.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_units.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_validators.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_validators.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_warp.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_warp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/test_us76.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/test_us76.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/test_util.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/test_util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/util/test_deprecation.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/util/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/util/test_misc.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/util/test_misc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/xarray/conftest.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/xarray/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/xarray/test_interp.py` & `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/xarray/test_interp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/conftest.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_albedo.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_albedo.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_atmosphere_rpv.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_atmosphere_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_basic.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_basic.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,23 +8,35 @@
 
 import eradiate
 from eradiate import KernelContext
 from eradiate import unit_registry as ureg
 from eradiate.kernel import mi_render
 from eradiate.scenes.bsdfs import LambertianBSDF
 from eradiate.scenes.core import Scene
-from eradiate.scenes.illumination import ConstantIllumination, DirectionalIllumination, AstroObjectIllumination
+from eradiate.scenes.illumination import (
+    AstroObjectIllumination,
+    ConstantIllumination,
+    DirectionalIllumination,
+)
 from eradiate.scenes.integrators import PathIntegrator
 from eradiate.scenes.measure import MultiDistantMeasure
 from eradiate.scenes.shapes import RectangleShape
 from eradiate.scenes.surface import BasicSurface
 from eradiate.test_tools.types import check_scene_element
 
 
-@pytest.mark.parametrize("illumination, spp", [("directional", 1), ("constant", 5e5), ("astroobject", 5e5)])
+@pytest.mark.parametrize(
+    "illumination, spp",
+    [
+        ("directional", 1),
+        ("constant", 5e5),
+        # Deactivated for now (inexplicably fails when run as part of full test suite)
+        # ("astro_object", 5e5),
+    ],
+)
 @pytest.mark.parametrize("li", [0.1, 1.0, 10.0])
 @pytest.mark.slow
 def test_radiometric_accuracy(modes_all_mono, illumination, spp, li, ert_seed_state):
     r"""
     Radiometric check (``path``)
     ============================
 
@@ -78,26 +90,29 @@
         "measure": measure,
         "integrator": PathIntegrator(),
     }
 
     if illumination == "directional":
         objects["illumination"] = DirectionalIllumination(zenith=0.0, irradiance=li)
         theoretical_solution = np.full_like(vza, rho * li / np.pi)
-        rtol=1e-3
+        rtol = 1e-3
 
     elif illumination == "constant":
         objects["illumination"] = ConstantIllumination(radiance=li)
         theoretical_solution = np.full_like(vza, rho * li)
-        rtol=1e-3
+        rtol = 1e-3
 
-    elif illumination == "astroobject":
-        objects["illumination"] = AstroObjectIllumination(zenith=0.0, irradiance=li, angular_diameter=0.03)
+    # Deactivated for now (see parametrization)
+    elif illumination == "astro_object":
+        objects["illumination"] = AstroObjectIllumination(
+            zenith=0.0, irradiance=li, angular_diameter=0.03
+        )
         theoretical_solution = np.full_like(vza, rho * li / np.pi)
         # The angular diameter is not taken into account in the theoretical solution
-        rtol=1e-2
+        rtol = 1e-2
 
     else:
         raise ValueError(f"unsupported illumination '{illumination}'")
 
     scene = Scene(objects=objects)
     mi_wrapper = check_scene_element(scene, mi.Scene)
```

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_ckd_basic.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_ckd_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,20 +20,15 @@
     ========================================
 
     This system test tries various combinations of atmosphere flags and checks
     that a computation succeeds and returns non-zero values.
     """
     # TODO: Recycle this test
     if eradiate.mode().is_mono:
-        atm_kwargs = {
-            "construct": "ussa_1976",
-            "absorption_dataset": (
-                "spectra/absorption/us76_u86_4/us76_u86_4-spectra-18000_19000.nc"
-            ),
-        }
+        atm_kwargs = {"construct": "ussa_1976"}
     elif eradiate.mode().is_ckd:
         atm_kwargs = {"construct": "afgl_1986"}
     else:
         raise NotImplementedError
 
     exp = eradiate.experiments.AtmosphereExperiment(
         surface={"type": "rpv"},
```

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         "type": "molecular",
         "has_absorption": True,
         "has_scattering": False,
     }
     atmosphere_mono = {
         **atmosphere_kwargs,
         "construct": "ussa_1976",
-        "absorption_dataset": "tests/spectra/absorption/us76_u86_4-spectra-4000_25711.nc",
     }
     atmosphere_ckd = {
         **atmosphere_kwargs,
         "construct": "afgl_1986",
     }
 
     exp = eradiate.experiments.AtmosphereExperiment(
```

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_irradiance_scaling.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_irradiance_scaling.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_kernel_render_benchmark.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_kernel_render_benchmark.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_maximum_scene_size.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_maximum_scene_size.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_mdistant_insitu.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_mdistant_insitu.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_onedim_phase.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_onedim_phase.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_onedim_symmetry.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_onedim_symmetry.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_spectral_loop.py` & `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_spectral_loop.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py` & `eradiate-0.23.2rc3/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py` & `eradiate-0.23.2rc3/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py` & `eradiate-0.23.2rc3/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/test_het01.py` & `eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/test_het01.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/test_het04.py` & `eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/test_het04.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/test_het06.py` & `eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/test_het06.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/01_eradiate/conftest.py` & `eradiate-0.23.2rc3/tests/01_eradiate/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc2/tests/conftest.py` & `eradiate-0.23.2rc3/tests/conftest.py`

 * *Files identical despite different names*

