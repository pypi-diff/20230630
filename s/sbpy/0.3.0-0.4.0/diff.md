# Comparing `tmp/sbpy-0.3.0.tar.gz` & `tmp/sbpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbpy-0.3.0.tar", last modified: Thu Apr 28 21:01:50 2022, max compression
+gzip compressed data, was "sbpy-0.4.0.tar", last modified: Fri Jun 30 18:30:20 2023, max compression
```

## Comparing `sbpy-0.3.0.tar` & `sbpy-0.4.0.tar`

### file list

```diff
@@ -1,283 +1,285 @@
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.854374 sbpy-0.3.0/
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:49.890372 sbpy-0.3.0/.github/
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:49.978372 sbpy-0.3.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 msk       (1000) msk       (1000)      993 2020-07-25 03:16:14.000000 sbpy-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 msk       (1000) msk       (1000)      780 2020-07-25 03:16:14.000000 sbpy-0.3.0/.github/ISSUE_TEMPLATE/issue-report.md
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:49.986372 sbpy-0.3.0/.github/workflows/
--rw-rw-r--   0 msk       (1000) msk       (1000)      652 2022-02-05 15:11:02.000000 sbpy-0.3.0/.github/workflows/ci_cron_weekly.yml
--rw-rw-r--   0 msk       (1000) msk       (1000)     3219 2022-02-05 15:11:02.000000 sbpy-0.3.0/.github/workflows/ci_tests.yml
--rw-rw-r--   0 msk       (1000) msk       (1000)      882 2022-02-05 15:11:02.000000 sbpy-0.3.0/.gitignore
--rw-rw-r--   0 msk       (1000) msk       (1000)     4099 2022-04-28 21:00:51.000000 sbpy-0.3.0/CHANGES.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)      183 2019-07-04 13:18:29.000000 sbpy-0.3.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 msk       (1000) msk       (1000)      332 2019-07-04 13:18:29.000000 sbpy-0.3.0/CONTRIBUTING.md
--rw-rw-r--   0 msk       (1000) msk       (1000)     1521 2022-02-24 15:58:38.000000 sbpy-0.3.0/LICENSE.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)      363 2022-02-05 15:11:02.000000 sbpy-0.3.0/MANIFEST.in
--rw-rw-r--   0 msk       (1000) msk       (1000)     3113 2022-04-28 21:01:50.854374 sbpy-0.3.0/PKG-INFO
--rw-rw-r--   0 msk       (1000) msk       (1000)     2367 2022-02-18 14:43:25.000000 sbpy-0.3.0/README.rst
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.038372 sbpy-0.3.0/docs/
--rw-rw-r--   0 msk       (1000) msk       (1000)     4581 2018-08-16 15:44:25.000000 sbpy-0.3.0/docs/Makefile
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:49.890372 sbpy-0.3.0/docs/_static/
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.038372 sbpy-0.3.0/docs/_static/spectroscopy/
--rw-rw-r--   0 msk       (1000) msk       (1000)    27077 2019-06-10 11:54:18.000000 sbpy-0.3.0/docs/_static/spectroscopy/spectroscopy-1.png
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:49.890372 sbpy-0.3.0/docs/_templates/
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.058372 sbpy-0.3.0/docs/_templates/autosummary/
--rw-rw-r--   0 msk       (1000) msk       (1000)      250 2018-08-16 15:44:25.000000 sbpy-0.3.0/docs/_templates/autosummary/base.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)      251 2018-08-16 15:44:25.000000 sbpy-0.3.0/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)      252 2018-08-16 15:44:25.000000 sbpy-0.3.0/docs/_templates/autosummary/module.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)    19250 2022-04-28 21:00:51.000000 sbpy-0.3.0/docs/about.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     2110 2022-02-24 18:59:16.000000 sbpy-0.3.0/docs/api_reference.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     3807 2022-02-05 15:11:02.000000 sbpy-0.3.0/docs/compile_fieldnames.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     7263 2022-02-24 19:45:47.000000 sbpy-0.3.0/docs/conf.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.066372 sbpy-0.3.0/docs/development/
--rw-rw-r--   0 msk       (1000) msk       (1000)     4362 2020-07-25 03:16:14.000000 sbpy-0.3.0/docs/development/design-principles.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     6239 2022-02-24 19:39:53.000000 sbpy-0.3.0/docs/development/index.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     3748 2022-02-18 15:04:48.000000 sbpy-0.3.0/docs/index.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     2562 2022-02-24 17:36:00.000000 sbpy-0.3.0/docs/install.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     4513 2018-08-16 15:44:25.000000 sbpy-0.3.0/docs/make.bat
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.098373 sbpy-0.3.0/docs/sbpy/
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.122372 sbpy-0.3.0/docs/sbpy/activity/
--rw-rw-r--   0 msk       (1000) msk       (1000)     8509 2020-07-25 03:16:14.000000 sbpy-0.3.0/docs/sbpy/activity/dust.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)    17120 2022-02-17 21:32:36.000000 sbpy-0.3.0/docs/sbpy/activity/gas.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     2135 2020-07-25 03:16:14.000000 sbpy-0.3.0/docs/sbpy/activity/index.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     6644 2020-07-25 03:16:14.000000 sbpy-0.3.0/docs/sbpy/bib.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)    12216 2022-02-05 15:11:02.000000 sbpy-0.3.0/docs/sbpy/calib.rst
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.214373 sbpy-0.3.0/docs/sbpy/data/
--rw-rw-r--   0 msk       (1000) msk       (1000)    24046 2022-02-17 21:32:36.000000 sbpy-0.3.0/docs/sbpy/data/dataclass.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)    12964 2022-02-05 15:11:02.000000 sbpy-0.3.0/docs/sbpy/data/ephem.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)    42500 2022-02-05 15:11:02.000000 sbpy-0.3.0/docs/sbpy/data/fieldnames.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     1134 2020-07-25 03:16:14.000000 sbpy-0.3.0/docs/sbpy/data/index.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     3129 2020-07-25 03:16:14.000000 sbpy-0.3.0/docs/sbpy/data/names.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     4898 2022-02-05 15:11:02.000000 sbpy-0.3.0/docs/sbpy/data/obs.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     5811 2022-02-05 15:11:02.000000 sbpy-0.3.0/docs/sbpy/data/orbit.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     2693 2020-07-25 03:16:14.000000 sbpy-0.3.0/docs/sbpy/data/phys.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)      602 2022-02-05 15:11:02.000000 sbpy-0.3.0/docs/sbpy/exceptions.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     6288 2022-02-17 21:32:36.000000 sbpy-0.3.0/docs/sbpy/photometry.rst
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.214373 sbpy-0.3.0/docs/sbpy/spectroscopy/
--rw-rw-r--   0 msk       (1000) msk       (1000)     4349 2022-02-05 15:11:02.000000 sbpy-0.3.0/docs/sbpy/spectroscopy/index.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     1821 2022-02-05 15:11:02.000000 sbpy-0.3.0/docs/sbpy/spectroscopy/sources.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)     5995 2022-02-05 15:11:02.000000 sbpy-0.3.0/docs/sbpy/units.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)      236 2019-06-10 11:54:18.000000 sbpy-0.3.0/docs/sbpy/utils.rst
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.230373 sbpy-0.3.0/docs/static/
--rw-rw-r--   0 msk       (1000) msk       (1000)    16661 2018-08-16 15:44:25.000000 sbpy-0.3.0/docs/static/structure.pdf
--rw-rw-r--   0 msk       (1000) msk       (1000)    68568 2018-08-16 15:44:25.000000 sbpy-0.3.0/docs/static/structure.png
--rw-rw-r--   0 msk       (1000) msk       (1000)    17559 2022-04-28 21:00:51.000000 sbpy-0.3.0/docs/status.rst
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.234373 sbpy-0.3.0/examples/
--rw-rw-r--   0 msk       (1000) msk       (1000)      314 2018-08-16 15:44:25.000000 sbpy-0.3.0/examples/README.rst
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.254373 sbpy-0.3.0/examples/activity/
--rw-rw-r--   0 msk       (1000) msk       (1000)       66 2018-08-16 15:44:25.000000 sbpy-0.3.0/examples/activity/README.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)   111616 2018-08-16 15:44:25.000000 sbpy-0.3.0/examples/activity/estimating-coma-continuum.ipynb
--rw-rw-r--   0 msk       (1000) msk       (1000)   162949 2018-08-16 15:44:25.000000 sbpy-0.3.0/examples/activity/haser-model.ipynb
--rw-rw-r--   0 msk       (1000) msk       (1000)   215331 2022-02-17 21:32:36.000000 sbpy-0.3.0/examples/activity/vectorial-model.ipynb
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.266373 sbpy-0.3.0/licenses/
--rw-rw-r--   0 msk       (1000) msk       (1000)     1486 2020-07-25 03:16:14.000000 sbpy-0.3.0/licenses/LICENSE.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)      162 2018-08-16 15:44:25.000000 sbpy-0.3.0/licenses/README.rst
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.294373 sbpy-0.3.0/logo/
--rw-rw-r--   0 msk       (1000) msk       (1000)    22125 2018-08-16 15:44:25.000000 sbpy-0.3.0/logo/LICENSE
--rw-rw-r--   0 msk       (1000) msk       (1000)    12296 2018-08-16 15:44:25.000000 sbpy-0.3.0/logo/sbpy_logo.svg
--rw-rw-r--   0 msk       (1000) msk       (1000)    28819 2018-08-16 15:44:25.000000 sbpy-0.3.0/logo/sbpy_logo_full.pdf
--rw-rw-r--   0 msk       (1000) msk       (1000)    31326 2018-08-16 15:44:25.000000 sbpy-0.3.0/logo/sbpy_logo_full.png
--rw-rw-r--   0 msk       (1000) msk       (1000)    11459 2018-08-16 15:44:25.000000 sbpy-0.3.0/logo/sbpy_logo_logoonly.pdf
--rw-rw-r--   0 msk       (1000) msk       (1000)    18413 2018-08-16 15:44:25.000000 sbpy-0.3.0/logo/sbpy_logo_logoonly.png
--rw-rw-r--   0 msk       (1000) msk       (1000)    10379 2018-08-16 15:44:25.000000 sbpy-0.3.0/logo/sbpy_logo_logoonly.svg
--rw-rw-r--   0 msk       (1000) msk       (1000)     8508 2018-08-16 15:44:25.000000 sbpy-0.3.0/logo/sbpy_logo_logoonly_inverted.svg
--rw-rw-r--   0 msk       (1000) msk       (1000)    20113 2018-08-16 15:44:25.000000 sbpy-0.3.0/logo/sbpy_logo_short.pdf
--rw-rw-r--   0 msk       (1000) msk       (1000)    30794 2018-08-16 15:44:25.000000 sbpy-0.3.0/logo/sbpy_logo_short.png
--rw-rw-r--   0 msk       (1000) msk       (1000)    11582 2018-08-16 15:44:25.000000 sbpy-0.3.0/logo/sbpy_logo_short.svg
--rw-rw-r--   0 msk       (1000) msk       (1000)      334 2022-02-05 15:11:02.000000 sbpy-0.3.0/pep8speaks.yml
--rw-rw-r--   0 msk       (1000) msk       (1000)      265 2020-07-25 03:16:14.000000 sbpy-0.3.0/pip-requirements
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:49.890372 sbpy-0.3.0/publications/
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.310373 sbpy-0.3.0/publications/joss/
--rw-rw-r--   0 msk       (1000) msk       (1000)     8256 2020-07-25 03:16:14.000000 sbpy-0.3.0/publications/joss/paper.bib
--rw-rw-r--   0 msk       (1000) msk       (1000)     5115 2019-07-04 13:18:29.000000 sbpy-0.3.0/publications/joss/paper.md
--rw-rw-r--   0 msk       (1000) msk       (1000)    68568 2019-06-10 11:54:18.000000 sbpy-0.3.0/publications/joss/structure.png
--rw-rw-r--   0 msk       (1000) msk       (1000)      132 2022-02-05 15:11:02.000000 sbpy-0.3.0/pyproject.toml
--rw-rw-r--   0 msk       (1000) msk       (1000)      452 2022-02-24 16:23:14.000000 sbpy-0.3.0/readthedocs.yml
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.314373 sbpy-0.3.0/sbpy/
--rw-rw-r--   0 msk       (1000) msk       (1000)      521 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)      355 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/_astropy_init.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.318373 sbpy-0.3.0/sbpy/activity/
--rw-rw-r--   0 msk       (1000) msk       (1000)      131 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/activity/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     8296 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/activity/core.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    20315 2022-02-17 21:32:36.000000 sbpy-0.3.0/sbpy/activity/dust.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.334373 sbpy-0.3.0/sbpy/activity/gas/
--rw-rw-r--   0 msk       (1000) msk       (1000)      194 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/activity/gas/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    51760 2022-02-17 21:32:36.000000 sbpy-0.3.0/sbpy/activity/gas/core.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.354373 sbpy-0.3.0/sbpy/activity/gas/data/
--rw-rw-r--   0 msk       (1000) msk       (1000)     7065 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/activity/gas/data/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     8056 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/activity/gas/data/schleicher88.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    34332 2022-02-17 21:32:36.000000 sbpy-0.3.0/sbpy/activity/gas/productionrate.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.386373 sbpy-0.3.0/sbpy/activity/gas/tests/
--rw-rw-r--   0 msk       (1000) msk       (1000)        0 2019-07-05 14:31:45.000000 sbpy-0.3.0/sbpy/activity/gas/tests/__init__.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.394373 sbpy-0.3.0/sbpy/activity/gas/tests/data/
--rw-rw-r--   0 msk       (1000) msk       (1000)     1707 2019-07-05 14:31:45.000000 sbpy-0.3.0/sbpy/activity/gas/tests/data/CH3OH.csv
--rw-rw-r--   0 msk       (1000) msk       (1000)      322 2019-07-05 14:31:45.000000 sbpy-0.3.0/sbpy/activity/gas/tests/data/CO.csv
--rw-rw-r--   0 msk       (1000) msk       (1000)     2530 2019-07-05 14:31:45.000000 sbpy-0.3.0/sbpy/activity/gas/tests/data/HCN.csv
--rw-rw-r--   0 msk       (1000) msk       (1000)    12220 2022-02-17 21:32:36.000000 sbpy-0.3.0/sbpy/activity/gas/tests/data/wm_fortran_test_output.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    30115 2022-02-17 21:32:36.000000 sbpy-0.3.0/sbpy/activity/gas/tests/test_core.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     1000 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/activity/gas/tests/test_data.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     4300 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/activity/gas/tests/test_prodrate.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    14510 2022-02-10 14:11:49.000000 sbpy-0.3.0/sbpy/activity/gas/tests/test_prodrate_remote.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.402373 sbpy-0.3.0/sbpy/activity/tests/
--rw-rw-r--   0 msk       (1000) msk       (1000)        0 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/activity/tests/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     3408 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/activity/tests/test_core.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    10673 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/activity/tests/test_dust.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.402373 sbpy-0.3.0/sbpy/bib/
--rw-rw-r--   0 msk       (1000) msk       (1000)      171 2019-07-04 13:18:29.000000 sbpy-0.3.0/sbpy/bib/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    11530 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/bib/core.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.402373 sbpy-0.3.0/sbpy/bib/tests/
--rw-rw-r--   0 msk       (1000) msk       (1000)        0 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/bib/tests/__init__.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.422373 sbpy-0.3.0/sbpy/bib/tests/data/
--rw-rw-r--   0 msk       (1000) msk       (1000)      465 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/bib/tests/data/neatm.bib
--rw-rw-r--   0 msk       (1000) msk       (1000)     6917 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/bib/tests/test_bib.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.434373 sbpy-0.3.0/sbpy/calib/
--rw-rw-r--   0 msk       (1000) msk       (1000)     1282 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    21710 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/calib/core.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.494373 sbpy-0.3.0/sbpy/calib/data/
--rw-rw-r--   0 msk       (1000) msk       (1000)   112320 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/data/alpha_lyr_stis_008-edit.fits
--rw-rw-r--   0 msk       (1000) msk       (1000)    21520 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/data/e490-00a_2014_hires.csv
--rw-rw-r--   0 msk       (1000) msk       (1000)     1471 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/data/e490-00a_2014_lores.csv
--rw-rw-r--   0 msk       (1000) msk       (1000)    49140 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/data/e490-00a_2014_table3.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)     1775 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/data/e490-00a_2014_table4.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    22778 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/data/solar-photometry-willmer2018.json
--rw-rw-r--   0 msk       (1000) msk       (1000)    21507 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/data/vega-photometry-willmer2018.json
--rw-rw-r--   0 msk       (1000) msk       (1000)     3512 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/solar_sources.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.510373 sbpy-0.3.0/sbpy/calib/tests/
--rw-rw-r--   0 msk       (1000) msk       (1000)        0 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/tests/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    11640 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/tests/test_core.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     5048 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/tests/test_sun.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     4771 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/tests/test_vega.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     2420 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/calib/vega_sources.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     2125 2022-02-10 14:11:49.000000 sbpy-0.3.0/sbpy/conftest.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.558373 sbpy-0.3.0/sbpy/data/
--rw-rw-r--   0 msk       (1000) msk       (1000)    34277 2022-02-17 21:32:36.000000 sbpy-0.3.0/sbpy/data/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    34862 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/data/core.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     8586 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/data/decorators.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     2755 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/data/dimensions.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    37255 2022-02-24 16:08:22.000000 sbpy-0.3.0/sbpy/data/ephem.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    43245 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/data/fieldnames.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)    23206 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/data/names.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     8612 2022-02-24 16:08:19.000000 sbpy-0.3.0/sbpy/data/obs.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    30134 2022-02-24 16:08:10.000000 sbpy-0.3.0/sbpy/data/orbit.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    11743 2022-02-17 21:32:36.000000 sbpy-0.3.0/sbpy/data/phys.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.590373 sbpy-0.3.0/sbpy/data/tests/
--rw-rw-r--   0 msk       (1000) msk       (1000)        0 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/data/tests/__init__.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.642373 sbpy-0.3.0/sbpy/data/tests/data/
--rw-rw-r--   0 msk       (1000) msk       (1000)      122 2018-09-12 11:24:49.000000 sbpy-0.3.0/sbpy/data/tests/data/test.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    22401 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/data/tests/test_dataclass.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     5777 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/data/tests/test_decorators.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     2727 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/data/tests/test_ephem.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    16190 2022-02-17 21:32:36.000000 sbpy-0.3.0/sbpy/data/tests/test_ephem_remote.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     8935 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/data/tests/test_names.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     3662 2022-02-17 21:32:36.000000 sbpy-0.3.0/sbpy/data/tests/test_obs_remote.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     6000 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/data/tests/test_orbit.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     6927 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/data/tests/test_orbit_remote.py
--rw-rw-r--   0 msk       (1000) msk       (1000)      392 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/data/tests/test_phys_remote.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.642373 sbpy-0.3.0/sbpy/data_archive/
--rw-rw-r--   0 msk       (1000) msk       (1000)      257 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/data_archive/README.rst
--rw-rw-r--   0 msk       (1000) msk       (1000)      696 2022-02-17 21:32:36.000000 sbpy-0.3.0/sbpy/exceptions.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.646374 sbpy-0.3.0/sbpy/extern/
--rw-rw-r--   0 msk       (1000) msk       (1000)      397 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/extern/__init__.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.650374 sbpy-0.3.0/sbpy/ginga_plugins/
--rw-rw-r--   0 msk       (1000) msk       (1000)     9971 2022-02-17 21:32:36.000000 sbpy-0.3.0/sbpy/ginga_plugins/CometaryEnhancements.py
--rw-rw-r--   0 msk       (1000) msk       (1000)      633 2018-12-08 16:44:09.000000 sbpy-0.3.0/sbpy/ginga_plugins/__init__.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.654374 sbpy-0.3.0/sbpy/imageanalysis/
--rw-rw-r--   0 msk       (1000) msk       (1000)       66 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/imageanalysis/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     4869 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/imageanalysis/core.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.658373 sbpy-0.3.0/sbpy/imageanalysis/tests/
--rw-rw-r--   0 msk       (1000) msk       (1000)        0 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/imageanalysis/tests/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     2053 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/imageanalysis/tests/test_utils.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     6376 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/imageanalysis/utils.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.658373 sbpy-0.3.0/sbpy/obsutil/
--rw-rw-r--   0 msk       (1000) msk       (1000)       66 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/obsutil/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     3219 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/obsutil/core.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.666374 sbpy-0.3.0/sbpy/photometry/
--rw-rw-r--   0 msk       (1000) msk       (1000)       91 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     5562 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/photometry/bandpass.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    44518 2022-02-24 16:18:31.000000 sbpy-0.3.0/sbpy/photometry/core.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.714374 sbpy-0.3.0/sbpy/photometry/data/
--rw-rw-r--   0 msk       (1000) msk       (1000)     1447 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/2mass-h-rsr.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)     2548 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/2mass-j-rsr.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)     1859 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/2mass-ks-rsr.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)     1467 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/README
--rw-rw-r--   0 msk       (1000) msk       (1000)    10074 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/WISE-RSR-W1.EE.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    13824 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/WISE-RSR-W2.EE.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    66658 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/WISE-RSR-W3.EE.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    66658 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/WISE-RSR-W4.EE.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)     1413 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/photometry/data/atlas-c.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)     1419 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/photometry/data/atlas-o.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/photometry/data/cousins_i_004_syn.fits
--rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/cousins_r_004_syn.fits
--rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/johnson_b_004_syn.fits
--rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/johnson_u_004_syn.fits
--rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/photometry/data/johnson_v_004_syn.fits
--rw-rw-r--   0 msk       (1000) msk       (1000)    18218 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/ps1-gp1.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    18218 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/ps1-ip1.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    18218 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/ps1-rp1.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    18218 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/ps1-wp1.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    18218 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/ps1-yp1.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    18218 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/photometry/data/ps1-zp1.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/photometry/data/sdss-g.fits
--rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/photometry/data/sdss-i.fits
--rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/photometry/data/sdss-r.fits
--rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/photometry/data/sdss-u.fits
--rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/photometry/data/sdss-z.fits
--rw-rw-r--   0 msk       (1000) msk       (1000)    28800 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/photometry/data/wfc3_uvis_f438w_004_syn.fits
--rw-rw-r--   0 msk       (1000) msk       (1000)    20160 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/photometry/data/wfc3_uvis_f606w_004_syn.fits
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.730374 sbpy-0.3.0/sbpy/photometry/tests/
--rw-rw-r--   0 msk       (1000) msk       (1000)        0 2018-09-29 15:27:45.000000 sbpy-0.3.0/sbpy/photometry/tests/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     1326 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/photometry/tests/test_bandpass.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    29638 2022-02-24 19:45:10.000000 sbpy-0.3.0/sbpy/photometry/tests/test_core.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.746374 sbpy-0.3.0/sbpy/shape/
--rw-rw-r--   0 msk       (1000) msk       (1000)       63 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/shape/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     1905 2018-09-12 11:24:49.000000 sbpy-0.3.0/sbpy/shape/core.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.770374 sbpy-0.3.0/sbpy/spectroscopy/
--rw-rw-r--   0 msk       (1000) msk       (1000)       92 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/spectroscopy/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    12512 2022-02-17 21:32:36.000000 sbpy-0.3.0/sbpy/spectroscopy/core.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    15859 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/spectroscopy/sources.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.786374 sbpy-0.3.0/sbpy/spectroscopy/tests/
--rw-rw-r--   0 msk       (1000) msk       (1000)        0 2018-12-08 16:44:09.000000 sbpy-0.3.0/sbpy/spectroscopy/tests/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     3816 2022-02-05 15:11:02.000000 sbpy-0.3.0/sbpy/spectroscopy/tests/test_sources.py
--rw-rw-r--   0 msk       (1000) msk       (1000)      359 2018-12-08 16:44:09.000000 sbpy-0.3.0/sbpy/spectroscopy/tests/test_spec.py
--rw-rw-r--   0 msk       (1000) msk       (1000)      472 2019-07-05 14:31:45.000000 sbpy-0.3.0/sbpy/spectroscopy/tests/test_spec_remote.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     3355 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/spectroscopy/tests/test_specgrad.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.790374 sbpy-0.3.0/sbpy/tests/
--rw-rw-r--   0 msk       (1000) msk       (1000)      121 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/tests/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)      768 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/tests/coveragerc
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.790374 sbpy-0.3.0/sbpy/thermal/
--rw-rw-r--   0 msk       (1000) msk       (1000)       62 2018-08-16 15:44:25.000000 sbpy-0.3.0/sbpy/thermal/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     1900 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/thermal/core.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.794374 sbpy-0.3.0/sbpy/units/
--rw-rw-r--   0 msk       (1000) msk       (1000)      474 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/units/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)    11431 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/units/core.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.794374 sbpy-0.3.0/sbpy/units/tests/
--rw-rw-r--   0 msk       (1000) msk       (1000)        0 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/units/tests/__init__.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.814374 sbpy-0.3.0/sbpy/units/tests/data/
--rw-rw-r--   0 msk       (1000) msk       (1000)    49708 2019-07-04 13:18:29.000000 sbpy-0.3.0/sbpy/units/tests/data/hi05070405_9000036-avg-spec.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)    15944 2019-07-04 13:18:29.000000 sbpy-0.3.0/sbpy/units/tests/data/hi05070405_9000036-avg-spec_ref.pdf
--rw-rw-r--   0 msk       (1000) msk       (1000)     8002 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/units/tests/test_core.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.814374 sbpy-0.3.0/sbpy/utils/
--rw-rw-r--   0 msk       (1000) msk       (1000)      169 2019-06-10 11:54:18.000000 sbpy-0.3.0/sbpy/utils/__init__.py
--rw-rw-r--   0 msk       (1000) msk       (1000)      132 2020-07-25 03:16:14.000000 sbpy-0.3.0/sbpy/utils/core.py
--rw-rw-r--   0 msk       (1000) msk       (1000)      337 2022-04-28 21:01:46.000000 sbpy-0.3.0/sbpy/version.py
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.314373 sbpy-0.3.0/sbpy.egg-info/
--rw-rw-r--   0 msk       (1000) msk       (1000)     3113 2022-04-28 21:01:47.000000 sbpy-0.3.0/sbpy.egg-info/PKG-INFO
--rw-rw-r--   0 msk       (1000) msk       (1000)     6460 2022-04-28 21:01:49.000000 sbpy-0.3.0/sbpy.egg-info/SOURCES.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)        1 2022-04-28 21:01:47.000000 sbpy-0.3.0/sbpy.egg-info/dependency_links.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)       88 2022-04-28 21:01:47.000000 sbpy-0.3.0/sbpy.egg-info/entry_points.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)      249 2022-04-28 21:01:48.000000 sbpy-0.3.0/sbpy.egg-info/requires.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)        5 2022-04-28 21:01:48.000000 sbpy-0.3.0/sbpy.egg-info/top_level.txt
--rw-rw-r--   0 msk       (1000) msk       (1000)     2194 2022-04-28 21:01:50.858374 sbpy-0.3.0/setup.cfg
--rw-rw-r--   0 msk       (1000) msk       (1000)     1953 2022-02-05 15:11:02.000000 sbpy-0.3.0/setup.py
--rw-rw-r--   0 msk       (1000) msk       (1000)     5576 2022-02-24 17:00:17.000000 sbpy-0.3.0/tox.ini
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.818374 sbpy-0.3.0/website/
--rw-rw-r--   0 msk       (1000) msk       (1000)       54 2019-07-04 13:18:29.000000 sbpy-0.3.0/website/.firebaserc
--rw-rw-r--   0 msk       (1000) msk       (1000)      366 2019-07-04 13:18:29.000000 sbpy-0.3.0/website/README.md
--rw-rw-r--   0 msk       (1000) msk       (1000)      134 2019-07-04 13:18:29.000000 sbpy-0.3.0/website/firebase.json
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.834374 sbpy-0.3.0/website/public/
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.834374 sbpy-0.3.0/website/public/css/
--rw-rw-r--   0 msk       (1000) msk       (1000)    10310 2020-07-25 03:16:14.000000 sbpy-0.3.0/website/public/css/style.css
-drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2022-04-28 21:01:50.854374 sbpy-0.3.0/website/public/images/
--rw-rw-r--   0 msk       (1000) msk       (1000)     6592 2020-04-25 15:45:25.000000 sbpy-0.3.0/website/public/images/NASA_logo.svg
--rw-rw-r--   0 msk       (1000) msk       (1000)    31326 2019-07-04 13:18:29.000000 sbpy-0.3.0/website/public/images/sbpy_logo_full.png
--rw-rw-r--   0 msk       (1000) msk       (1000)     6085 2022-02-05 15:11:02.000000 sbpy-0.3.0/website/public/index.html
--rw-rw-r--   0 msk       (1000) msk       (1000)     3944 2020-07-25 03:16:14.000000 sbpy-0.3.0/website/public/team.html
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.136742 sbpy-0.4.0/
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.096742 sbpy-0.4.0/.github/
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.104742 sbpy-0.4.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      993 2021-07-15 14:45:26.000000 sbpy-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 msk       (1000) msk       (1000)      780 2021-07-15 14:45:26.000000 sbpy-0.4.0/.github/ISSUE_TEMPLATE/issue-report.md
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.104742 sbpy-0.4.0/.github/workflows/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1185 2023-06-12 17:22:19.000000 sbpy-0.4.0/.github/workflows/ci_cron_weekly.yml
+-rw-rw-r--   0 msk       (1000) msk       (1000)     2163 2023-06-12 17:22:19.000000 sbpy-0.4.0/.github/workflows/ci_tests.yml
+-rw-rw-r--   0 msk       (1000) msk       (1000)      894 2023-06-12 17:22:19.000000 sbpy-0.4.0/.gitignore
+-rw-rw-r--   0 msk       (1000) msk       (1000)      482 2023-04-27 18:38:05.000000 sbpy-0.4.0/.readthedocs.yaml
+-rw-rw-r--   0 msk       (1000) msk       (1000)     6413 2023-06-30 18:29:45.000000 sbpy-0.4.0/CHANGES.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)      183 2021-07-15 14:45:26.000000 sbpy-0.4.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 msk       (1000) msk       (1000)      332 2021-07-15 14:45:26.000000 sbpy-0.4.0/CONTRIBUTING.md
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1521 2023-04-27 18:38:05.000000 sbpy-0.4.0/LICENSE.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)      363 2021-09-27 14:40:36.000000 sbpy-0.4.0/MANIFEST.in
+-rw-rw-r--   0 msk       (1000) msk       (1000)     3112 2023-06-30 18:30:20.136742 sbpy-0.4.0/PKG-INFO
+-rw-rw-r--   0 msk       (1000) msk       (1000)     2386 2023-04-27 18:38:05.000000 sbpy-0.4.0/README.rst
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.104742 sbpy-0.4.0/docs/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     4581 2017-12-01 01:50:43.000000 sbpy-0.4.0/docs/Makefile
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.096742 sbpy-0.4.0/docs/_static/
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.104742 sbpy-0.4.0/docs/_static/spectroscopy/
+-rw-rw-r--   0 msk       (1000) msk       (1000)    27077 2021-10-19 14:55:28.000000 sbpy-0.4.0/docs/_static/spectroscopy/spectroscopy-1.png
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.096742 sbpy-0.4.0/docs/_templates/
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.104742 sbpy-0.4.0/docs/_templates/autosummary/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      250 2021-10-19 14:55:34.000000 sbpy-0.4.0/docs/_templates/autosummary/base.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)      251 2021-10-19 14:55:34.000000 sbpy-0.4.0/docs/_templates/autosummary/class.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)      252 2021-10-19 14:55:34.000000 sbpy-0.4.0/docs/_templates/autosummary/module.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)    19245 2023-06-30 18:29:45.000000 sbpy-0.4.0/docs/about.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     2110 2021-07-15 14:45:26.000000 sbpy-0.4.0/docs/api_reference.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     3807 2021-09-27 14:40:36.000000 sbpy-0.4.0/docs/compile_fieldnames.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     7261 2023-04-27 18:38:05.000000 sbpy-0.4.0/docs/conf.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.104742 sbpy-0.4.0/docs/development/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     4426 2023-06-12 17:22:19.000000 sbpy-0.4.0/docs/development/design-principles.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     6219 2023-06-30 18:29:45.000000 sbpy-0.4.0/docs/development/index.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     3741 2023-06-30 18:29:45.000000 sbpy-0.4.0/docs/index.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     3242 2023-06-30 18:29:45.000000 sbpy-0.4.0/docs/install.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     4513 2017-12-01 01:50:43.000000 sbpy-0.4.0/docs/make.bat
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.104742 sbpy-0.4.0/docs/sbpy/
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.108742 sbpy-0.4.0/docs/sbpy/activity/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8593 2023-06-12 17:22:19.000000 sbpy-0.4.0/docs/sbpy/activity/dust.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)    16872 2023-06-30 18:29:45.000000 sbpy-0.4.0/docs/sbpy/activity/gas.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     2135 2021-07-15 14:45:26.000000 sbpy-0.4.0/docs/sbpy/activity/index.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     6644 2021-07-15 14:45:26.000000 sbpy-0.4.0/docs/sbpy/bib.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)    13132 2023-06-12 17:22:19.000000 sbpy-0.4.0/docs/sbpy/calib.rst
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.108742 sbpy-0.4.0/docs/sbpy/data/
+-rw-rw-r--   0 msk       (1000) msk       (1000)    25420 2023-06-12 17:22:19.000000 sbpy-0.4.0/docs/sbpy/data/dataclass.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)    15133 2023-06-30 18:29:45.000000 sbpy-0.4.0/docs/sbpy/data/ephem.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)    42574 2023-04-27 18:38:05.000000 sbpy-0.4.0/docs/sbpy/data/fieldnames.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1121 2023-04-27 18:38:05.000000 sbpy-0.4.0/docs/sbpy/data/index.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     4454 2023-04-27 18:38:05.000000 sbpy-0.4.0/docs/sbpy/data/names.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     4736 2023-06-12 17:22:19.000000 sbpy-0.4.0/docs/sbpy/data/obs.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8422 2023-06-30 18:29:45.000000 sbpy-0.4.0/docs/sbpy/data/orbit.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     2859 2023-06-30 18:29:45.000000 sbpy-0.4.0/docs/sbpy/data/phys.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)      602 2021-09-27 14:40:36.000000 sbpy-0.4.0/docs/sbpy/exceptions.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     6789 2023-06-12 17:22:19.000000 sbpy-0.4.0/docs/sbpy/photometry.rst
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.108742 sbpy-0.4.0/docs/sbpy/spectroscopy/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     4639 2023-06-12 17:22:19.000000 sbpy-0.4.0/docs/sbpy/spectroscopy/index.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1821 2021-09-27 14:40:36.000000 sbpy-0.4.0/docs/sbpy/spectroscopy/sources.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)     6840 2023-06-12 17:22:19.000000 sbpy-0.4.0/docs/sbpy/units.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)      236 2021-07-15 14:45:26.000000 sbpy-0.4.0/docs/sbpy/utils.rst
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.108742 sbpy-0.4.0/docs/static/
+-rw-rw-r--   0 msk       (1000) msk       (1000)    16661 2017-12-01 01:50:43.000000 sbpy-0.4.0/docs/static/structure.pdf
+-rw-rw-r--   0 msk       (1000) msk       (1000)    68568 2017-12-01 01:50:43.000000 sbpy-0.4.0/docs/static/structure.png
+-rw-rw-r--   0 msk       (1000) msk       (1000)    17541 2023-06-30 18:29:45.000000 sbpy-0.4.0/docs/status.rst
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.108742 sbpy-0.4.0/examples/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      314 2019-03-21 22:59:01.000000 sbpy-0.4.0/examples/README.rst
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.112742 sbpy-0.4.0/examples/activity/
+-rw-rw-r--   0 msk       (1000) msk       (1000)       66 2017-12-05 11:53:08.000000 sbpy-0.4.0/examples/activity/README.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)   111616 2017-12-05 11:53:08.000000 sbpy-0.4.0/examples/activity/estimating-coma-continuum.ipynb
+-rw-rw-r--   0 msk       (1000) msk       (1000)   162949 2017-12-05 11:53:08.000000 sbpy-0.4.0/examples/activity/haser-model.ipynb
+-rw-rw-r--   0 msk       (1000) msk       (1000)   295740 2023-06-30 18:29:45.000000 sbpy-0.4.0/examples/activity/vectorial-model.ipynb
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.112742 sbpy-0.4.0/licenses/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1486 2021-07-15 14:45:26.000000 sbpy-0.4.0/licenses/LICENSE.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)      162 2017-12-01 01:50:43.000000 sbpy-0.4.0/licenses/README.rst
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.112742 sbpy-0.4.0/logo/
+-rw-rw-r--   0 msk       (1000) msk       (1000)    22125 2019-03-21 22:59:01.000000 sbpy-0.4.0/logo/LICENSE
+-rw-rw-r--   0 msk       (1000) msk       (1000)    12296 2019-03-21 22:59:01.000000 sbpy-0.4.0/logo/sbpy_logo.svg
+-rw-rw-r--   0 msk       (1000) msk       (1000)    28819 2019-03-21 22:59:01.000000 sbpy-0.4.0/logo/sbpy_logo_full.pdf
+-rw-rw-r--   0 msk       (1000) msk       (1000)    31326 2019-03-21 22:59:01.000000 sbpy-0.4.0/logo/sbpy_logo_full.png
+-rw-rw-r--   0 msk       (1000) msk       (1000)    11459 2019-03-21 22:59:01.000000 sbpy-0.4.0/logo/sbpy_logo_logoonly.pdf
+-rw-rw-r--   0 msk       (1000) msk       (1000)    18413 2019-03-21 22:59:01.000000 sbpy-0.4.0/logo/sbpy_logo_logoonly.png
+-rw-rw-r--   0 msk       (1000) msk       (1000)    10379 2019-03-21 22:59:01.000000 sbpy-0.4.0/logo/sbpy_logo_logoonly.svg
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8508 2019-03-21 22:59:01.000000 sbpy-0.4.0/logo/sbpy_logo_logoonly_inverted.svg
+-rw-rw-r--   0 msk       (1000) msk       (1000)    20113 2019-03-21 22:59:01.000000 sbpy-0.4.0/logo/sbpy_logo_short.pdf
+-rw-rw-r--   0 msk       (1000) msk       (1000)    30794 2019-03-21 22:59:01.000000 sbpy-0.4.0/logo/sbpy_logo_short.png
+-rw-rw-r--   0 msk       (1000) msk       (1000)    11582 2019-03-21 22:59:01.000000 sbpy-0.4.0/logo/sbpy_logo_short.svg
+-rw-rw-r--   0 msk       (1000) msk       (1000)      334 2021-09-27 14:40:36.000000 sbpy-0.4.0/pep8speaks.yml
+-rw-rw-r--   0 msk       (1000) msk       (1000)      265 2021-07-15 14:45:26.000000 sbpy-0.4.0/pip-requirements
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.096742 sbpy-0.4.0/publications/
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.112742 sbpy-0.4.0/publications/joss/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8256 2021-07-15 14:45:26.000000 sbpy-0.4.0/publications/joss/paper.bib
+-rw-rw-r--   0 msk       (1000) msk       (1000)     5115 2021-07-15 14:45:26.000000 sbpy-0.4.0/publications/joss/paper.md
+-rw-rw-r--   0 msk       (1000) msk       (1000)    68568 2021-07-15 14:45:26.000000 sbpy-0.4.0/publications/joss/structure.png
+-rw-rw-r--   0 msk       (1000) msk       (1000)      132 2021-09-27 14:40:36.000000 sbpy-0.4.0/pyproject.toml
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.112742 sbpy-0.4.0/sbpy/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      521 2017-12-01 01:50:43.000000 sbpy-0.4.0/sbpy/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)      355 2021-09-27 14:40:36.000000 sbpy-0.4.0/sbpy/_astropy_init.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.116742 sbpy-0.4.0/sbpy/activity/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      131 2019-03-21 23:04:44.000000 sbpy-0.4.0/sbpy/activity/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8296 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/activity/core.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    22130 2023-06-30 18:29:45.000000 sbpy-0.4.0/sbpy/activity/dust.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.116742 sbpy-0.4.0/sbpy/activity/gas/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      194 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/activity/gas/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    58271 2023-06-30 18:29:45.000000 sbpy-0.4.0/sbpy/activity/gas/core.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.116742 sbpy-0.4.0/sbpy/activity/gas/data/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     7065 2021-09-27 14:40:36.000000 sbpy-0.4.0/sbpy/activity/gas/data/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8056 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/activity/gas/data/schleicher88.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    34424 2023-06-12 17:22:19.000000 sbpy-0.4.0/sbpy/activity/gas/productionrate.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.116742 sbpy-0.4.0/sbpy/activity/gas/tests/
+-rw-rw-r--   0 msk       (1000) msk       (1000)        0 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/activity/gas/tests/__init__.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.116742 sbpy-0.4.0/sbpy/activity/gas/tests/data/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1707 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/activity/gas/tests/data/CH3OH.csv
+-rw-rw-r--   0 msk       (1000) msk       (1000)      322 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/activity/gas/tests/data/CO.csv
+-rw-rw-r--   0 msk       (1000) msk       (1000)     2530 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/activity/gas/tests/data/HCN.csv
+-rw-rw-r--   0 msk       (1000) msk       (1000)    12220 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/activity/gas/tests/data/wm_fortran_test_output.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    33865 2023-06-30 18:29:45.000000 sbpy-0.4.0/sbpy/activity/gas/tests/test_core.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1000 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/activity/gas/tests/test_data.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     4300 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/activity/gas/tests/test_prodrate.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    15179 2023-06-12 17:22:19.000000 sbpy-0.4.0/sbpy/activity/gas/tests/test_prodrate_remote.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.116742 sbpy-0.4.0/sbpy/activity/tests/
+-rw-rw-r--   0 msk       (1000) msk       (1000)        0 2017-12-05 11:53:08.000000 sbpy-0.4.0/sbpy/activity/tests/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     3408 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/activity/tests/test_core.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    10673 2021-08-31 14:59:26.000000 sbpy-0.4.0/sbpy/activity/tests/test_dust.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.116742 sbpy-0.4.0/sbpy/bib/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      171 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/bib/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    11530 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/bib/core.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.116742 sbpy-0.4.0/sbpy/bib/tests/
+-rw-rw-r--   0 msk       (1000) msk       (1000)        0 2017-12-05 11:53:08.000000 sbpy-0.4.0/sbpy/bib/tests/__init__.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.116742 sbpy-0.4.0/sbpy/bib/tests/data/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      465 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/bib/tests/data/neatm.bib
+-rw-rw-r--   0 msk       (1000) msk       (1000)     6917 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/bib/tests/test_bib.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.120742 sbpy-0.4.0/sbpy/calib/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1282 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/calib/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    21705 2023-06-12 17:22:19.000000 sbpy-0.4.0/sbpy/calib/core.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.120742 sbpy-0.4.0/sbpy/calib/data/
+-rw-rw-r--   0 msk       (1000) msk       (1000)   112320 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/calib/data/alpha_lyr_stis_008-edit.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)    21520 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/calib/data/e490-00a_2014_hires.csv
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1471 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/calib/data/e490-00a_2014_lores.csv
+-rw-rw-r--   0 msk       (1000) msk       (1000)    49140 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/calib/data/e490-00a_2014_table3.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1775 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/calib/data/e490-00a_2014_table4.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    22778 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/calib/data/solar-photometry-willmer2018.json
+-rw-rw-r--   0 msk       (1000) msk       (1000)    21507 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/calib/data/vega-photometry-willmer2018.json
+-rw-rw-r--   0 msk       (1000) msk       (1000)     3964 2023-06-12 17:22:19.000000 sbpy-0.4.0/sbpy/calib/solar_sources.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.120742 sbpy-0.4.0/sbpy/calib/tests/
+-rw-rw-r--   0 msk       (1000) msk       (1000)        0 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/calib/tests/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    11640 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/calib/tests/test_core.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     6096 2023-06-12 17:22:19.000000 sbpy-0.4.0/sbpy/calib/tests/test_sun.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     4726 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/calib/tests/test_vega.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     2420 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/calib/vega_sources.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     2125 2022-04-28 18:35:06.000000 sbpy-0.4.0/sbpy/conftest.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.124742 sbpy-0.4.0/sbpy/data/
+-rw-rw-r--   0 msk       (1000) msk       (1000)    34277 2022-02-07 14:14:31.000000 sbpy-0.4.0/sbpy/data/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    40766 2023-06-12 17:22:19.000000 sbpy-0.4.0/sbpy/data/core.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8586 2021-09-27 14:40:36.000000 sbpy-0.4.0/sbpy/data/decorators.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     2755 2021-09-27 14:40:36.000000 sbpy-0.4.0/sbpy/data/dimensions.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    37313 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/data/ephem.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    43245 2022-02-07 14:14:31.000000 sbpy-0.4.0/sbpy/data/fieldnames.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)    23642 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/data/names.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8609 2023-06-30 18:29:45.000000 sbpy-0.4.0/sbpy/data/obs.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    37128 2023-06-30 18:29:45.000000 sbpy-0.4.0/sbpy/data/orbit.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    11798 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/data/phys.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.124742 sbpy-0.4.0/sbpy/data/tests/
+-rw-rw-r--   0 msk       (1000) msk       (1000)        0 2017-12-01 01:50:43.000000 sbpy-0.4.0/sbpy/data/tests/__init__.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.124742 sbpy-0.4.0/sbpy/data/tests/data/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      122 2019-03-21 23:01:06.000000 sbpy-0.4.0/sbpy/data/tests/data/test.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    27437 2023-06-12 17:22:19.000000 sbpy-0.4.0/sbpy/data/tests/test_dataclass.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     5777 2021-09-27 14:40:36.000000 sbpy-0.4.0/sbpy/data/tests/test_decorators.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     2727 2021-09-27 14:40:36.000000 sbpy-0.4.0/sbpy/data/tests/test_ephem.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    16190 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/data/tests/test_ephem_remote.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8931 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/data/tests/test_names.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     3662 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/data/tests/test_obs_remote.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    11447 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/data/tests/test_orbit.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     7855 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/data/tests/test_orbit_remote.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)      955 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/data/tests/test_phys_remote.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.124742 sbpy-0.4.0/sbpy/data_archive/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      257 2017-12-01 01:50:43.000000 sbpy-0.4.0/sbpy/data_archive/README.rst
+-rw-rw-r--   0 msk       (1000) msk       (1000)      696 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/exceptions.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.124742 sbpy-0.4.0/sbpy/extern/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      397 2017-12-01 01:50:43.000000 sbpy-0.4.0/sbpy/extern/__init__.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.124742 sbpy-0.4.0/sbpy/ginga_plugins/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     9971 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/ginga_plugins/CometaryEnhancements.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)      633 2019-03-21 23:04:44.000000 sbpy-0.4.0/sbpy/ginga_plugins/__init__.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.124742 sbpy-0.4.0/sbpy/imageanalysis/
+-rw-rw-r--   0 msk       (1000) msk       (1000)       66 2017-12-01 01:50:43.000000 sbpy-0.4.0/sbpy/imageanalysis/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     4869 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/imageanalysis/core.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.124742 sbpy-0.4.0/sbpy/imageanalysis/tests/
+-rw-rw-r--   0 msk       (1000) msk       (1000)        0 2017-12-01 01:50:43.000000 sbpy-0.4.0/sbpy/imageanalysis/tests/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     2053 2019-03-21 23:04:44.000000 sbpy-0.4.0/sbpy/imageanalysis/tests/test_utils.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     6376 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/imageanalysis/utils.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.124742 sbpy-0.4.0/sbpy/obsutil/
+-rw-rw-r--   0 msk       (1000) msk       (1000)       66 2017-12-01 01:50:43.000000 sbpy-0.4.0/sbpy/obsutil/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     3219 2019-03-21 23:04:44.000000 sbpy-0.4.0/sbpy/obsutil/core.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.128742 sbpy-0.4.0/sbpy/photometry/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      110 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/photometry/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     5562 2022-02-07 14:14:31.000000 sbpy-0.4.0/sbpy/photometry/bandpass.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    28565 2023-06-12 17:22:19.000000 sbpy-0.4.0/sbpy/photometry/core.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.132742 sbpy-0.4.0/sbpy/photometry/data/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1447 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/2mass-h-rsr.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)     2548 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/2mass-j-rsr.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1859 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/2mass-ks-rsr.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1467 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/README
+-rw-rw-r--   0 msk       (1000) msk       (1000)    10074 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/WISE-RSR-W1.EE.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    13824 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/WISE-RSR-W2.EE.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    66658 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/WISE-RSR-W3.EE.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    66658 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/WISE-RSR-W4.EE.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1413 2022-02-07 14:14:31.000000 sbpy-0.4.0/sbpy/photometry/data/atlas-c.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1419 2022-02-07 14:14:31.000000 sbpy-0.4.0/sbpy/photometry/data/atlas-o.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2019-03-21 23:04:44.000000 sbpy-0.4.0/sbpy/photometry/data/cousins_i_004_syn.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/cousins_r_004_syn.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/johnson_b_004_syn.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/johnson_u_004_syn.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/johnson_v_004_syn.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)    18218 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/ps1-gp1.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    18218 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/ps1-ip1.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    18218 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/ps1-rp1.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    18218 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/ps1-wp1.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    18218 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/ps1-yp1.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    18218 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/ps1-zp1.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/sdss-g.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/sdss-i.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2019-03-21 23:04:44.000000 sbpy-0.4.0/sbpy/photometry/data/sdss-r.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/sdss-u.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8640 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/photometry/data/sdss-z.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)    28800 2019-03-21 23:04:44.000000 sbpy-0.4.0/sbpy/photometry/data/wfc3_uvis_f438w_004_syn.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)    20160 2019-03-21 23:04:44.000000 sbpy-0.4.0/sbpy/photometry/data/wfc3_uvis_f606w_004_syn.fits
+-rw-rw-r--   0 msk       (1000) msk       (1000)    17206 2023-06-12 17:22:19.000000 sbpy-0.4.0/sbpy/photometry/iau.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.132742 sbpy-0.4.0/sbpy/photometry/tests/
+-rw-rw-r--   0 msk       (1000) msk       (1000)        0 2019-03-21 23:01:06.000000 sbpy-0.4.0/sbpy/photometry/tests/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1326 2022-02-07 14:14:31.000000 sbpy-0.4.0/sbpy/photometry/tests/test_bandpass.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     6672 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/photometry/tests/test_core.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    23698 2023-06-12 17:22:19.000000 sbpy-0.4.0/sbpy/photometry/tests/test_iau.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.132742 sbpy-0.4.0/sbpy/shape/
+-rw-rw-r--   0 msk       (1000) msk       (1000)       63 2017-12-01 01:50:43.000000 sbpy-0.4.0/sbpy/shape/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1905 2019-03-21 23:01:06.000000 sbpy-0.4.0/sbpy/shape/core.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.132742 sbpy-0.4.0/sbpy/spectroscopy/
+-rw-rw-r--   0 msk       (1000) msk       (1000)       92 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/spectroscopy/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    12697 2023-06-12 17:22:19.000000 sbpy-0.4.0/sbpy/spectroscopy/core.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    15859 2023-06-30 18:29:45.000000 sbpy-0.4.0/sbpy/spectroscopy/sources.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.132742 sbpy-0.4.0/sbpy/spectroscopy/tests/
+-rw-rw-r--   0 msk       (1000) msk       (1000)        0 2019-03-21 23:04:44.000000 sbpy-0.4.0/sbpy/spectroscopy/tests/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     3816 2022-02-07 14:14:31.000000 sbpy-0.4.0/sbpy/spectroscopy/tests/test_sources.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)      359 2019-03-21 23:04:44.000000 sbpy-0.4.0/sbpy/spectroscopy/tests/test_spec.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)      144 2023-04-27 18:38:05.000000 sbpy-0.4.0/sbpy/spectroscopy/tests/test_spec_remote.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     3355 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/spectroscopy/tests/test_specgrad.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.132742 sbpy-0.4.0/sbpy/tests/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      121 2017-12-01 01:50:43.000000 sbpy-0.4.0/sbpy/tests/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)      768 2017-12-01 01:50:43.000000 sbpy-0.4.0/sbpy/tests/coveragerc
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.132742 sbpy-0.4.0/sbpy/thermal/
+-rw-rw-r--   0 msk       (1000) msk       (1000)       62 2017-12-01 01:50:43.000000 sbpy-0.4.0/sbpy/thermal/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1900 2019-03-21 23:04:44.000000 sbpy-0.4.0/sbpy/thermal/core.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.136742 sbpy-0.4.0/sbpy/units/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      474 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/units/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)    11431 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/units/core.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.136742 sbpy-0.4.0/sbpy/units/tests/
+-rw-rw-r--   0 msk       (1000) msk       (1000)        0 2019-03-21 23:04:44.000000 sbpy-0.4.0/sbpy/units/tests/__init__.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.136742 sbpy-0.4.0/sbpy/units/tests/data/
+-rw-rw-r--   0 msk       (1000) msk       (1000)    49708 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/units/tests/data/hi05070405_9000036-avg-spec.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)    15944 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/units/tests/data/hi05070405_9000036-avg-spec_ref.pdf
+-rw-rw-r--   0 msk       (1000) msk       (1000)     8002 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/units/tests/test_core.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.136742 sbpy-0.4.0/sbpy/utils/
+-rw-rw-r--   0 msk       (1000) msk       (1000)      169 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/utils/__init__.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)      132 2021-07-15 14:45:26.000000 sbpy-0.4.0/sbpy/utils/core.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)      337 2023-06-30 18:30:20.000000 sbpy-0.4.0/sbpy/version.py
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.116742 sbpy-0.4.0/sbpy.egg-info/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     3112 2023-06-30 18:30:20.000000 sbpy-0.4.0/sbpy.egg-info/PKG-INFO
+-rw-rw-r--   0 msk       (1000) msk       (1000)     6519 2023-06-30 18:30:20.000000 sbpy-0.4.0/sbpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)        1 2023-06-30 18:30:20.000000 sbpy-0.4.0/sbpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)       88 2023-06-30 18:30:20.000000 sbpy-0.4.0/sbpy.egg-info/entry_points.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)      275 2023-06-30 18:30:20.000000 sbpy-0.4.0/sbpy.egg-info/requires.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)        5 2023-06-30 18:30:20.000000 sbpy-0.4.0/sbpy.egg-info/top_level.txt
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1834 2023-06-30 18:30:20.136742 sbpy-0.4.0/setup.cfg
+-rw-rw-r--   0 msk       (1000) msk       (1000)     1953 2021-09-27 14:40:36.000000 sbpy-0.4.0/setup.py
+-rw-rw-r--   0 msk       (1000) msk       (1000)     5162 2023-06-12 17:22:19.000000 sbpy-0.4.0/tox.ini
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.136742 sbpy-0.4.0/website/
+-rw-rw-r--   0 msk       (1000) msk       (1000)       54 2021-07-15 14:45:26.000000 sbpy-0.4.0/website/.firebaserc
+-rw-rw-r--   0 msk       (1000) msk       (1000)      366 2021-07-15 14:45:26.000000 sbpy-0.4.0/website/README.md
+-rw-rw-r--   0 msk       (1000) msk       (1000)      134 2021-07-15 14:45:26.000000 sbpy-0.4.0/website/firebase.json
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.136742 sbpy-0.4.0/website/public/
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.136742 sbpy-0.4.0/website/public/css/
+-rw-rw-r--   0 msk       (1000) msk       (1000)    10241 2023-04-27 18:38:05.000000 sbpy-0.4.0/website/public/css/style.css
+drwxrwxr-x   0 msk       (1000) msk       (1000)        0 2023-06-30 18:30:20.136742 sbpy-0.4.0/website/public/images/
+-rw-rw-r--   0 msk       (1000) msk       (1000)     6592 2021-07-15 14:45:26.000000 sbpy-0.4.0/website/public/images/NASA_logo.svg
+-rw-rw-r--   0 msk       (1000) msk       (1000)    31326 2021-07-15 14:45:26.000000 sbpy-0.4.0/website/public/images/sbpy_logo_full.png
+-rw-rw-r--   0 msk       (1000) msk       (1000)     7042 2023-04-27 18:38:05.000000 sbpy-0.4.0/website/public/index.html
+-rw-rw-r--   0 msk       (1000) msk       (1000)     4967 2023-04-27 18:38:05.000000 sbpy-0.4.0/website/public/team.html
```

### Comparing `sbpy-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `sbpy-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/.github/ISSUE_TEMPLATE/issue-report.md` & `sbpy-0.4.0/.github/ISSUE_TEMPLATE/issue-report.md`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/.gitignore` & `sbpy-0.4.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
 # Other
 .cache
 .tox
 .*.sw[op]
 *~
 \#*
+.hypothesis
 .project
 .pydevproject
 .settings
 *py#
 .firebase
 .tmp
```

### Comparing `sbpy-0.3.0/LICENSE.rst` & `sbpy-0.4.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/PKG-INFO` & `sbpy-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: sbpy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python module for small-body planetary astronomy
 Home-page: https://sbpy.org
 Author: sbpy team
 Author-email: msk@astro.umd.edu
 License: BSD 3-Clause
 Keywords: astronomy,astrophysics,planetary,asteroid,comet,space,science
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.rst
 
-.. image:: https://github.com/NASA-Planetary-Science/sbpy/raw/master/logo/sbpy_logo_short.png
+.. image:: https://github.com/NASA-Planetary-Science/sbpy/raw/main/logo/sbpy_logo_short.png
     :width: 400px
     :align: center	    
     :alt: sbpy	     
 	  
        
 sbpy is an `Astropy <https://www.astropy.org/>`_ affiliated package for small-body
 planetary astronomy.
@@ -42,15 +41,15 @@
     :target: https://sbpy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation status
 
 .. image:: https://joss.theoj.org/papers/10.21105/joss.01426/status.svg
     :target: https://doi.org/10.21105/joss.01426
     :alt: JOSS documentation
 
-.. image:: https://codecov.io/gh/NASA-Planetary-Science/sbpy/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/NASA-Planetary-Science/sbpy/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/NASA-Planetary-Science/sbpy
     :alt: codecov status
 	  
 
 Overview
 --------
 
@@ -81,14 +80,12 @@
 
 sbpy is still under development, with v1.0 scheduled for delivery in 2024. For an overview on the status of individual features see the `Status Page <https://sbpy.readthedocs.io/en/latest/status.html>`_.
 
 
 Acknowledgements
 ----------------
 
-`sbpy` is supported by NASA PDART Grant No. 80NSSC18K0987.
+`sbpy` support provided by NASA PDART Grant Nos. 80NSSC18K0987 and 80NSSC22K0143.
 
 If you use `sbpy` in your work, please acknowledge it by citing
 
     `Mommert, Kelley, de-Val Borro, Li et al., (2019). sbpy: A Python module for small-body planetary astronomy. Journal of Open Source Software, 4(38), 1426 <https://joss.theoj.org/papers/8b8e7bb15fb4a14f80f2afd06b6ce060>`_
-
-
```

### Comparing `sbpy-0.3.0/README.rst` & `sbpy-0.4.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. image:: https://github.com/NASA-Planetary-Science/sbpy/raw/master/logo/sbpy_logo_short.png
+.. image:: https://github.com/NASA-Planetary-Science/sbpy/raw/main/logo/sbpy_logo_short.png
     :width: 400px
     :align: center	    
     :alt: sbpy	     
 	  
        
 sbpy is an `Astropy <https://www.astropy.org/>`_ affiliated package for small-body
 planetary astronomy.
@@ -19,15 +19,15 @@
     :target: https://sbpy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation status
 
 .. image:: https://joss.theoj.org/papers/10.21105/joss.01426/status.svg
     :target: https://doi.org/10.21105/joss.01426
     :alt: JOSS documentation
 
-.. image:: https://codecov.io/gh/NASA-Planetary-Science/sbpy/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/NASA-Planetary-Science/sbpy/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/NASA-Planetary-Science/sbpy
     :alt: codecov status
 	  
 
 Overview
 --------
 
@@ -58,12 +58,12 @@
 
 sbpy is still under development, with v1.0 scheduled for delivery in 2024. For an overview on the status of individual features see the `Status Page <https://sbpy.readthedocs.io/en/latest/status.html>`_.
 
 
 Acknowledgements
 ----------------
 
-`sbpy` is supported by NASA PDART Grant No. 80NSSC18K0987.
+`sbpy` support provided by NASA PDART Grant Nos. 80NSSC18K0987 and 80NSSC22K0143.
 
 If you use `sbpy` in your work, please acknowledge it by citing
 
     `Mommert, Kelley, de-Val Borro, Li et al., (2019). sbpy: A Python module for small-body planetary astronomy. Journal of Open Source Software, 4(38), 1426 <https://joss.theoj.org/papers/8b8e7bb15fb4a14f80f2afd06b6ce060>`_
```

### Comparing `sbpy-0.3.0/docs/Makefile` & `sbpy-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/docs/_static/spectroscopy/spectroscopy-1.png` & `sbpy-0.4.0/docs/_static/spectroscopy/spectroscopy-1.png`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/docs/about.rst` & `sbpy-0.4.0/docs/about.rst`

 * *Files 1% similar despite different names*

```diff
@@ -307,15 +307,15 @@
 not an `astropy.units.Quantity` object, i.e., it did not have units of length.
 Of course, we know that Ceres' diameter is 945 km, but it was not clear from our
 definition.  Any functionality in `sbpy` would have to presume that diameters
 are always given in km. This makes sense for large objects - but what about
 meter-sized objects like near-Earth asteroids?
 
 Following the
-`Zen of Python <https://www.python.org/dev/peps/pep-0020/>`_ (explicit
+`Zen of Python <https://peps.python.org/pep-0020/>`_ (explicit
 is better than implicit), we require that units are explicitly
 defined:
 
     >>> import astropy.units as u
     >>> ceres = Phys.from_dict({'targetname': 'Ceres',
     ...                         'diameter': 945*u.km})
     >>> ceres
@@ -385,22 +385,22 @@
 
 This containerization makes it possible to keep data neatly formatted
 and to minimize the number of input parameters for functions and
 methods.
 
 
 
-.. _JPL Horizons: https://ssd.jpl.nasa.gov/horizons.cgi
+.. _JPL Horizons: https://ssd.jpl.nasa.gov/horizons/
 .. _Minor Planet Center: https://minorplanetcenter.net/
 .. _IMCCE: http://vo.imcce.fr/webservices/miriade/
-.. _Lowell Observatory: https://asteroid.lowell.edu
+.. _Lowell Observatory: https://asteroid.lowell.edu/gui/
 .. _PyEphem: https://rhodesmill.org/pyephem
 .. _REBOUND: https://github.com/hannorein/rebound
 .. _OpenOrb: https://github.com/oorb/oorb
 .. _SpiceyPy: https://github.com/AndrewAnnex/SpiceyPy
 .. _web-API: https://minorplanetcenter.net/search_db
-.. _Solar System Object Image Search function of the Canadian Astronomy Data Centre: http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca/en/ssois/
+.. _Solar System Object Image Search function of the Canadian Astronomy Data Centre: https://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca/en/ssois/
 .. _skybot: http://vo.imcce.fr/webservices/skybot/
 .. _small bodies data ferret: https://sbnapps.psi.edu/ferret
 .. _github wiki: https://github.com/mommermi/sbpy/wiki
 .. _Ginga Image Viewer: https://ejeschke.github.io/ginga/
 .. _photutils: https://github.com/astropy/photutils
```

### Comparing `sbpy-0.3.0/docs/api_reference.rst` & `sbpy-0.4.0/docs/api_reference.rst`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/docs/compile_fieldnames.py` & `sbpy-0.4.0/docs/compile_fieldnames.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/docs/conf.py` & `sbpy-0.4.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     extensions += ['sphinx_astropy.ext.edit_on_github']
 
     versionmod = __import__(setup_cfg['package_name'] + '.version')
     edit_on_github_project = setup_cfg['github_project']
     if versionmod.version.release:
         edit_on_github_branch = "v" + versionmod.version.version
     else:
-        edit_on_github_branch = "master"
+        edit_on_github_branch = "main"
 
     edit_on_github_source_root = ""
     edit_on_github_doc_root = "docs"
 
 # -- Resolving issue number to links in changelog -----------------------------
 github_issues_url = 'https://github.com/{0}/issues/'.format(
     setup_cfg['github_project'])
```

### Comparing `sbpy-0.3.0/docs/development/design-principles.rst` & `sbpy-0.4.0/docs/development/design-principles.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,68 +15,68 @@
 
 * Note magnitudes may also carry physical units.  Compare `astropy.units.mag` (unitless) to `astropy.units.ABmag` (flux density per unit frequency), and `sbpy.units.VEGAmag` (units of Vega spectral flux density).
 
 Epochs must be Time objects
 ---------------------------
 
 * Any kind of epoch or point in time must be of type `~astropy.time.Time`; time scales must be properly set and propagated through all functions.
-  
+
 
 Use sbpy ``DataClass`` objects
 ------------------------------
 
 * `~sbpy.data.Orbit`, `~sbpy.data.Phys`, `~sbpy.data.Ephem`, and `~sbpy.data.Obs` are the `sbpy` `~sbpy.data.DataClass` objects.  See :doc:`../sbpy/data/index` for details.
 
 * All inputs based on ephemeris, orbit, and physical parameters must use these classes.
 
 * The classes enable easy parameter passing from online sources.  Compare the following:
 
-  .. code-block:: python
-     
-     eph = Ephem.from_horizons('2P')
-     # rh, delta required, phase angle is optional:
-     Afrho(wave, fluxd, aper, eph['rh'], eph['delta'], phase=eph['phase'])
-     # more to the point:
-     Afrho(wave, fluxd, aper, eph)
+    .. code-block:: python
+
+        eph = Ephem.from_horizons('2P')
+        # rh, delta required, phase angle is optional:
+        Afrho(wave, fluxd, aper, eph['rh'], eph['delta'], phase=eph['phase'])
+        # more to the point:
+        Afrho(wave, fluxd, aper, eph)
 
-  Carefully document which fields are used by your function or method.
+    Carefully document which fields are used by your function or method.
      
 * Dictionary-like objects may be allowed for user input, but should be internally converted to a ``DataClass`` object with the `~sbpy.data.dataclass_input` decorator:
 
-  .. code-block:: python
-     
-     @dataclass_input(eph=Ephem)
-     def H11(eph):
-         ...
-
-  The same, but using function annotations:
-  
-  .. code-block:: python
-     
-     @dataclass_input
-     def H11(eph: Ephem):
-         ...
+    .. code-block:: python
+
+        @dataclass_input(eph=Ephem)
+        def H11(eph):
+            ...
+
+    The same, but using function annotations:
+
+    .. code-block:: python
+
+        @dataclass_input
+        def H11(eph: Ephem):
+            ...
 
 * Exceptions are allowed when only one parameter is needed, e.g., ``phase_func(phase)``.  But instead consider using the relevant ``DataClass`` object, and decorating the function with `~sbpy.data.quantity_to_dataclass`:
 
-  .. code-block:: python
+    .. code-block:: python
 
-     @quantity_to_dataclass(eph=(Ephem, 'phase'))
-     def phase_func(eph):
-         ...
+        @quantity_to_dataclass(eph=(Ephem, 'phase'))
+        def phase_func(eph):
+            ...
 
-  The decorator may be stacked with ``dataclass_input`` for maximum
-  flexibility:
+    The decorator may be stacked with ``dataclass_input`` for maximum
+    flexibility:
 
-  .. code-block:: python
+    .. code-block:: python
 
-     @dataclass_input
-     @quantity_to_dataclass(eph=(Ephem, 'phase'))
-     def phase_func(eph):
-         ...
+        @dataclass_input
+        @quantity_to_dataclass(eph=(Ephem, 'phase'))
+        def phase_func(eph):
+            ...
 
 
 Append fields to ``DataClass`` at the user's request
 ----------------------------------------------------
 
 * If a function takes a `~sbpy.data.DataClass` object as input, the
   results of this function may be optionally appended to this object,
@@ -90,19 +90,19 @@
 Cite relevant works
 -------------------
 
 * All important references for methods, data sources, parameters, software, etc., must be cited.
 
 * Citations may be executed internally with :func:`sbpy.bib.register`, or via the `~sbpy.bib.cite` decorator:
 
-  .. code-block:: python
+    .. code-block:: python
 
-     @cite({'method': '1687pnpm.book.....N'})
-     def force(mass, acceleration):
-         return mass * acceleration
+        @cite({'method': '1687pnpm.book.....N'})
+        def force(mass, acceleration):
+            return mass * acceleration
 
 * Labels describing references (``'method'`` in the above example) are
   required to start with the following strings: ``'method'`` (for
   general method descriptions), ``'data source'`` (for data provenance
   referencing), ``'parameter'`` (for use of specific parameters),
   ``'software'`` (for use of specific software packages). Each of
   these labels can be suffixed at the users discretion (e.g.,
```

### Comparing `sbpy-0.3.0/docs/development/index.rst` & `sbpy-0.4.0/docs/development/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 might be useful to others, please let us know.
 
 Communicating with the developers
 ---------------------------------
 
 We would prefer any communication with the development team to go
 through the `github issue system
-<https://guides.github.com/features/issues/>`_. This way, all
+<https://docs.github.com/issues>`_. This way, all
 communications are centralized in one place and accessible to
 everyone. `sbpy` issues can be posted `here
 <https://github.com/NASA-Planetary-Science/sbpy/issues>`__.
 
 Another way to communicate in a less official way (if you don't think
 your question or suggestion is worth being remembered in the far
 future) is the sbpy slack channel, which is part of the Astropy slack
@@ -92,15 +92,15 @@
   
 Technical requirements
 ^^^^^^^^^^^^^^^^^^^^^^
 
 * code must adhere to `astropy's contributing guidelines
   <https://www.astropy.org/contribute.html>`__, the guidelines
   described in this document and `PEP8
-  <https://www.python.org/dev/peps/pep-0008/>`_
+  <https://peps.python.org/pep-0008/>`_
 * code must be accompanied by corresponding tests; 100% of the
   implemented tests must pass, a test coverage >= 90% is required; if
   possible, results should be checked against results from the
   literature
 * code must be accompanied by docstrings that describe the input and
   output parameters and includes example code, documentation, and at
   least one science task-oriented notebook that goes into the `sbpy
```

### Comparing `sbpy-0.3.0/docs/index.rst` & `sbpy-0.4.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     :target: https://doi.org/10.21105/joss.01426
     :alt: JOSS documentation
 
 .. image:: https://github.com/NASA-Planetary-Science/sbpy/actions/workflows/ci_cron_weekly.yml/badge.svg
     :target: https://github.com/NASA-Planetary-Science/sbpy/actions
     :alt: GitHub testing status
 
-.. image:: https://codecov.io/gh/NASA-Planetary-Science/sbpy/branch/master/graph/badge.svg
-    :target: https://app.codecov.io/gh/NASA-Planetary-Science/sbpy/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/NASA-Planetary-Science/sbpy/branch/main/graph/badge.svg
+    :target: https://app.codecov.io/gh/NASA-Planetary-Science/sbpy
     :alt: codecov status
 
 	     
 ***************
 Getting Started
 ***************
 
@@ -55,18 +55,20 @@
 User Documentation
 ******************
 
 Data Structures: Orbits, Ephemerides, Observations, and Physical Properties
 ---------------------------------------------------------------------------
 
 .. toctree::
-   :maxdepth: 2
+   :maxdepth: 1
+   :glob:
 
    sbpy/data/index.rst
    sbpy/data/fieldnames.rst
+   sbpy/data/*
 
 Photometry and Spectroscopy
 ---------------------------
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `sbpy-0.3.0/docs/install.rst` & `sbpy-0.4.0/docs/install.rst`

 * *Files 9% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 
 Requirements
 ^^^^^^^^^^^^
 
 `sbpy` has the following requirements that will be automatically taken
 care of with installation using pip:
 
-* Python 3.7 or later
-* `numpy <https://numpy.org/>`__ 1.17.0 or later
-* `astropy <https://www.astropy.org/>`__ 4.0 or later
-* `astroquery <https://astroquery.readthedocs.io/en/latest/>`__ 0.4.5 or later: For retrieval of online data, e.g., ephemerides and orbits.
-* `scipy <https://www.scipy.org/>`__: For numerical integrations in `sbpy.activity.gas` and `sbpy.photometry`, among others.
-* `synphot <https://github.com/spacetelescope/synphot_refactor>`__ 1.0.0 or later: For calibration with respect to the Sun and Vega, filtering spectra through bandpasses.
+* Python 3.8 or later
+* `ads <https://github.com/andycasey/ads/>`__ 0.12 or later, to fetch citation details for bibliography tracking.
+* `astropy <https://www.astropy.org/>`__ 4.3 or later.
+* `astroquery <https://astroquery.readthedocs.io/en/latest/>`__ 0.4.5 or later, for retrieval of online data, e.g., ephemerides and orbits.
+* `numpy <https://numpy.org/>`__ 1.18 or later.
+* `scipy <https://scipy.org/>`__: 1.3 or later, for numerical integrations in `sbpy.activity.gas` and `sbpy.photometry`, among others.
+* `synphot <https://github.com/spacetelescope/synphot_refactor>`__ 1.1.1 or later, for calibration with respect to the Sun and Vega, filtering spectra through bandpasses.
 
 Optional dependencies
 ^^^^^^^^^^^^^^^^^^^^^
 
 * Python extensions for `oorb <https://github.com/oorb/oorb/>`__: For orbit
   transformations (`~sbpy.data.Orbit.oo_transform`) and propagations
   (`~sbpy.data.Orbit.oo_propagate`), as well as ephemerides calculations
   (`~sbpy.data.Ephem.from_oo`).
 * `pyradex <https://github.com/keflavich/pyradex>`__: For non-LTE production
-  rate calculation related to cometary activity (`~sbpy.activity.gas.NonLTE`).
+  rate calculations related to cometary activity (`~sbpy.activity.gas.NonLTE`).
 * `ginga <https://ejeschke.github.io/ginga/>`__ and `photutils
   <https://photutils.readthedocs.io/en/stable/>`__: To interactively enhance
   images of comets with the `~sbpy.imageanalysis.CometaryEnhancement` Ginga
   plugin.
 
 
 Using pip
@@ -50,29 +51,53 @@
 The latest development version of `sbpy` can be easily installed using:
 
 .. code-block:: bash
 
     $ pip install git+https://github.com/NASA-Planetary-Science/sbpy.git
 
 
-Using GitHub
-^^^^^^^^^^^^
+Using conda
+^^^^^^^^^^^
+
+The latest stable version of `sbpy` can be installed with `Anaconda
+<https://www.anaconda.com/>`__ via the `conda-forge <https://conda-forge.org/>`__
+channel:
+
+.. code-block:: bash
+
+    $ conda install sbpy --channel=conda-forge
+
+If you do not have the conda-forge channel available, add it and re-run the
+installation command:
+
+.. code-block:: bash
+
+    $ conda config --add channels conda-forge
+    $ conda install sbpy --channel=conda-forge
 
-This way of installing `sbpy` is recommended if you plan to contribute
-to the module. The current development version of `sbpy` can be
-obtained from `GitHub <https://github.com/NASA-Planetary-Science/sbpy>`__ using
+
+Using Git+Pip
+^^^^^^^^^^^^^
+
+This way of installing `sbpy` is recommended if you plan to contribute to the
+module. The current development version of `sbpy` can be obtained from `GitHub
+<https://github.com/NASA-Planetary-Science/sbpy>`__ using:
 
 .. code-block:: bash
 
     $ git clone https://github.com/NASA-Planetary-Science/sbpy.git
 
-This will create a new directory (``sbpy/``). In this directory, run
+This will create a new directory (``sbpy/``). In this directory, run:
 
 .. code-block:: bash
 
-    $ python setup.py install --user
+    $ pip install .
+
+As above, to install optional dependencies, instead use ``pip install .[all]``.
 
-in order to use `sbpy` in your default Python environment. If you plan to work on the code and always want to use the latest version of your code, you can install it with
+If you plan to work on the code and always want to use the latest version of
+your code, we recommend installing in "editable" mode with the optional
+dependences and the testing dependencies:
 
 .. code-block:: bash
 
-    $ python setup.py develop --user
+    $ pip install -e .[all,test]
```

### Comparing `sbpy-0.3.0/docs/make.bat` & `sbpy-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/docs/sbpy/activity/dust.rst` & `sbpy-0.4.0/docs/sbpy/activity/dust.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,48 +4,48 @@
 *Afρ* and *εfρ*
 ---------------
 
 `sbpy` has two classes to support observations and models of a coma continuum: `~sbpy.activity.dust.Afrho` and `~sbpy.activity.dust.Efrho`.
 
 The *Afρ* parameter of A'Hearn et al (1984) is based on observations of idealized cometary dust comae.  It is proportional to the observed flux density within a circular aperture.  The quantity is the product of dust albedo, dust filling factor, and the radius of the aperture at the distance of the comet.  It carries the units of *ρ* (length), and under certain assumptions is proportional to the dust production rate of the comet:
 
-  .. math::
+.. math::
 
-     Afρ = \frac{4 Δ^2 r_h^2}{ρ}\frac{F_c}{F_⊙}
+   Afρ = \frac{4 Δ^2 r_h^2}{ρ}\frac{F_c}{F_⊙}
 
 where *Δ* and *ρ* have the same (linear) units, but :math:`r_h` is in units of au.  :math:`F_c` * is the flux density of the comet in the aperture, and :math:`F_⊙` is that of the Sun at 1 au in the same units.  See A'Hearn et al. (1984) and Fink & Rubin (2012) for more details.
 
 The *εfρ* parameter is the thermal emission counterpart to *Afρ*, replacing albedo with IR emissivity, *ε*, and the solar spectrum with the Planck function, *B*:
 
-  .. math::
+.. math::
 
-     εfρ = \frac{F_c Δ^2}{π ρ B(T_c)}
+   εfρ = \frac{F_c Δ^2}{π ρ B(T_c)}
 
 where :math:`T_c` is the spectral temperature of the continuum (Kelley et al. 2013).
 
 *Afρ* and *εfρ* are quantities
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 `Afrho` and `Efrho` are subclasses of `astropy`'s `~astropy.units.Quantity` and carry units of length.
 
-  >>> import numpy as np
-  >>> import astropy.units as u
-  >>> from sbpy.activity import Afrho, Efrho
-  >>>
-  >>> afrho = Afrho(100 * u.cm)
-  >>> print(afrho)    # doctest: +FLOAT_CMP
-  100.0 cm
-  >>> efrho = Efrho(afrho * 3.5)
-  >>> print(efrho)    # doctest: +FLOAT_CMP
-  350.0 cm
+   >>> import numpy as np
+   >>> import astropy.units as u
+   >>> from sbpy.activity import Afrho, Efrho
+   >>>
+   >>> afrho = Afrho(100 * u.cm)
+   >>> print(afrho)    # doctest: +FLOAT_CMP
+   100.0 cm
+   >>> efrho = Efrho(afrho * 3.5)
+   >>> print(efrho)    # doctest: +FLOAT_CMP
+   350.0 cm
 
 They may be converted to other units of length just like any `Quantity`:
 
-  >>> afrho.to('m')    # doctest: +FLOAT_CMP
-  <Afrho 1. m>
+   >>> afrho.to('m')    # doctest: +FLOAT_CMP
+   <Afrho 1. m>
 
 .. _afrho-to-from-flux-density:
 
 Convert to/from flux density
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The quantities may be initialized from flux densities.  Here, we reproduce one of the calculations from the original A'Hearn et al. (1984) work:
@@ -54,46 +54,46 @@
 * *Δ* = 3.822 au
 * phase angle = 3.3°
 * aperture radius = 9.8" (27200 km)
 * :math:`\log{F_λ}` = -13.99 erg/(cm\ :sup:`2` s Å) at *λ* = 5240 Å
 
 The solar flux density at 1 au is also needed.  We use 1868 W/(m2 μm).
 
-  >>> from sbpy.data import Ephem
-  >>> from sbpy.calib import solar_fluxd
-  >>>
-  >>> solar_fluxd.set({
-  ...     'λ5240': 1868 * u.W / u.m**2 / u.um,
-  ...     'λ5240(lambda pivot)': 5240 * u.AA
-  ... })              # doctest: +IGNORE_OUTPUT
-  >>>
-  >>> flam = 10**-13.99 * u.Unit('erg/(s cm2 AA)')
-  >>> aper = 27200 * u.km
-  >>>
-  >>> eph = Ephem.from_dict({'rh': 4.785 * u.au, 'delta': 3.822 * u.au})
-  >>>
-  >>> afrho = Afrho.from_fluxd('λ5240', flam, aper, eph)
-  >>> print(afrho)    # doctest: +FLOAT_CMP
-  6029.90248952895 cm
+   >>> from sbpy.data import Ephem
+   >>> from sbpy.calib import solar_fluxd
+   >>>
+   >>> solar_fluxd.set({
+   ...     'λ5240': 1868 * u.W / u.m**2 / u.um,
+   ...     'λ5240(lambda pivot)': 5240 * u.AA
+   ... })              # doctest: +IGNORE_OUTPUT
+   >>>
+   >>> flam = 10**-13.99 * u.Unit('erg/(s cm2 AA)')
+   >>> aper = 27200 * u.km
+   >>>
+   >>> eph = Ephem.from_dict({'rh': 4.785 * u.au, 'delta': 3.822 * u.au})
+   >>>
+   >>> afrho = Afrho.from_fluxd('λ5240', flam, aper, eph)
+   >>> print(afrho)    # doctest: +FLOAT_CMP
+   6029.90248952895 cm
 
 Which is within a few percent of 6160 cm computed by A'Hearn et al.. The difference is likely due to the assumed solar flux density in the bandpass.
 
 The `Afrho` class may be converted to a flux density, and the original value is recovered.
 
-  >>> f = afrho.to_fluxd('λ5240', aper, eph).to('erg/(s cm2 AA)')
-  >>> print(np.log10(f.value))    # doctest: +FLOAT_CMP
-  -13.99
+   >>> f = afrho.to_fluxd('λ5240', aper, eph).to('erg/(s cm2 AA)')
+   >>> print(np.log10(f.value))    # doctest: +FLOAT_CMP
+   -13.99
 
 `Afrho` works seamlessly with `sbpy`'s spectral calibration framework (:ref:`sbpy-calib`) when the `astropy` affiliated package `synphot` is installed.  The solar flux density (via `~sbpy.calib.solar_fluxd`) is not required, but instead the spectral wavelengths or the system transmission of the instrument and filter:
 
-.. doctest-requires:: synphot
+.. doctest-requires:: synphot; astropy>=5.3
 
    >>> wave = [0.4, 0.5, 0.6] * u.um
    >>> print(afrho.to_fluxd(wave, aper, eph))    # doctest: +FLOAT_CMP
-   [7.76770018e-14 1.05542873e-13 9.57978939e-14] W / (m2 um)
+   [7.76770018e-14 1.05542873e-13 9.57978939e-14] W / (um m2)
 
 .. doctest-requires:: synphot
 
    >>> from synphot import SpectralElement, Box1D
    >>> # bandpass width is a guess
    >>> bp = SpectralElement(Box1D, x_0=5240 * u.AA, width=50 * u.AA)
    >>> print(Afrho.from_fluxd(bp, flam, aper, eph))    # doctest: +FLOAT_CMP
@@ -104,96 +104,96 @@
    
 The `Efrho` class has the same functionality as the `Afrho` class.  The most important difference is that *εfρ* is calculated using a Planck function and temperature.  `sbpy` follows common practice and parameterizes the temperature as a constant scale factor of :math:`T_{BB} = 278\,r_h^{1/2}`\  K, the equilibrium temperature of a large blackbody sphere at a distance :math:`r_h` from the Sun.
 
 Reproduce the *εfρ* of 246P/NEAT from Kelley et al. (2013).
 
 .. doctest-requires:: synphot
 
-  >>> wave = [15.8, 22.3] * u.um
-  >>> fluxd = [25.75, 59.2] * u.mJy
-  >>> aper = 11.1 * u.arcsec
-  >>> eph = Ephem.from_dict({'rh': 4.28 * u.au, 'delta': 3.71 * u.au})
-  >>> efrho = Efrho.from_fluxd(wave, fluxd, aper, eph)
-  >>> for i in range(len(wave)):
-  ...     print('{:5.1f} at {:.1f}'.format(efrho[i], wave[i]))    # doctest: +FLOAT_CMP
-  406.2 cm at 15.8 um
-  427.9 cm at 22.3 um
+   >>> wave = [15.8, 22.3] * u.um
+   >>> fluxd = [25.75, 59.2] * u.mJy
+   >>> aper = 11.1 * u.arcsec
+   >>> eph = Ephem.from_dict({'rh': 4.28 * u.au, 'delta': 3.71 * u.au})
+   >>> efrho = Efrho.from_fluxd(wave, fluxd, aper, eph)
+   >>> for i in range(len(wave)):
+   ...     print('{:5.1f} at {:.1f}'.format(efrho[i], wave[i]))    # doctest: +FLOAT_CMP
+   406.2 cm at 15.8 um
+   427.9 cm at 22.3 um
 
 Compare to 397.0 cm and 424.6 cm listed in Kelley et al. (2013).
 
 
 To/from magnitudes
 ^^^^^^^^^^^^^^^^^^
 
 `Afrho` and `Efrho` work with `astropy`'s magnitude units.  If the conversion between Vega-based magnitudes is required, then `sbpy`'s calibration framework (:ref:`sbpy-calib`) will be used.
 
 Estimate the *Afρ* of comet C/2012 S1 (ISON) based on Pan-STARRS 1 photometry in the *r* band (Meech et al. 2013)
 
 .. doctest-requires:: synphot
 
-  >>> w = 0.617 * u.um
-  >>> m = 16.02 * u.ABmag
-  >>> aper = 5 * u.arcsec
-  >>> eph = {'rh': 5.234 * u.au, 'delta': 4.275 * u.au, 'phase': 2.6 * u.deg}
-  >>> afrho = Afrho.from_fluxd(w, m, aper, eph)
-  >>> print(afrho)    # doctest: +FLOAT_CMP
-  1948.496075629444 cm
-  >>> m2 = afrho.to_fluxd(w, aper, eph, unit=u.ABmag)    # doctest: +FLOAT_CMP
-  >>> print(m2)
-  16.02 mag(AB)
+   >>> w = 0.617 * u.um
+   >>> m = 16.02 * u.ABmag
+   >>> aper = 5 * u.arcsec
+   >>> eph = {'rh': 5.234 * u.au, 'delta': 4.275 * u.au, 'phase': 2.6 * u.deg}
+   >>> afrho = Afrho.from_fluxd(w, m, aper, eph)
+   >>> print(afrho)    # doctest: +FLOAT_CMP
+   1948.496075629444 cm
+   >>> m2 = afrho.to_fluxd(w, aper, eph, unit=u.ABmag)    # doctest: +FLOAT_CMP
+   >>> print(m2)
+   16.02 mag(AB)
 
 
 Phase angles and functions
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Phase angle was not used in the previous section.  In the *Afρ* formalism, "albedo" includes the scattering phase function, and is more precisely written *A(θ)*, where *θ* is the phase angle.  The default behavior for `Afrho` is to compute *A(θ)fρ* as opposed to *A(0°)fρ*.  Returning to the A'Hearn et al. data, we scale *Afρ* to 0° from 3.3° phase using the :func:`~sbpy.activity.Afrho.to_phase` method:
 
-  >>> afrho = Afrho(6029.9 * u.cm)
-  >>> print(afrho.to_phase(0 * u.deg, 3.3 * u.deg))    # doctest: +FLOAT_CMP
-  6886.825981017757 cm
+   >>> afrho = Afrho(6029.9 * u.cm)
+   >>> print(afrho.to_phase(0 * u.deg, 3.3 * u.deg))    # doctest: +FLOAT_CMP
+   6886.825981017757 cm
 
 The default phase function is the Halley-Marcus composite phase function (:func:`~sbpy.activity.phase_HalleyMarcus`).  Any function or callable object that accepts an angle as a `~astropy.units.Quantity` and returns a scalar value may be used:
 
-  >>> Phi = lambda phase: 10**(-0.016 / u.deg * phase.to('deg'))
-  >>> print(afrho.to_phase(0 * u.deg, 3.3 * u.deg, Phi=Phi))    # doctest: +FLOAT_CMP
-  6809.419810008357 cm
+   >>> Phi = lambda phase: 10**(-0.016 / u.deg * phase.to('deg'))
+   >>> print(afrho.to_phase(0 * u.deg, 3.3 * u.deg, Phi=Phi))    # doctest: +FLOAT_CMP
+   6809.419810008357 cm
 
 To correct an observed flux density for the phase function, use the ``phasecor`` option of :func:`~sbpy.activity.Afrho.to_fluxd` and :func:`~sbpy.activity.Afrho.from_fluxd` methods:
 
-  >>> flam = 10**-13.99 * u.Unit('erg/(s cm2 AA)')
-  >>> aper = 27200 * u.km
-  >>> eph = Ephem.from_dict({
-  ...     'rh': 4.785 * u.au,
-  ...     'delta': 3.822 * u.au,
-  ...     'phase': 3.3 * u.deg
-  ... })
-  >>>
-  >>> afrho = Afrho.from_fluxd('λ5240', flam, aper, eph, phasecor=True)
-  >>> print(afrho)    # doctest: +FLOAT_CMP
-  6886.828824340642 cm
+   >>> flam = 10**-13.99 * u.Unit('erg/(s cm2 AA)')
+   >>> aper = 27200 * u.km
+   >>> eph = Ephem.from_dict({
+   ...     'rh': 4.785 * u.au,
+   ...     'delta': 3.822 * u.au,
+   ...     'phase': 3.3 * u.deg
+   ... })
+   >>>
+   >>> afrho = Afrho.from_fluxd('λ5240', flam, aper, eph, phasecor=True)
+   >>> print(afrho)    # doctest: +FLOAT_CMP
+   6886.828824340642 cm
 
 
 Apertures
 ^^^^^^^^^
 
 Other apertures may be used, as long as they can be converted into an equivalent radius, assuming a coma with a *1/ρ* surface brightness distribution.  `~sbpy.activity` has a collection of useful geometries.
 
-  >>> from sbpy.activity import CircularAperture, AnnularAperture, RectangularAperture, GaussianAperture
-  >>> apertures = (
-  ...   ( '10" radius circle', CircularAperture(10 * u.arcsec)),
-  ...   (    '5"–10" annulus', AnnularAperture([5, 10] * u.arcsec)),
-  ...   (       '2"x10" slit', RectangularAperture([2, 10] * u.arcsec)),
-  ...   ('σ=5" Gaussian beam', GaussianAperture(5 * u.arcsec))
-  ... )
-  >>> for name, aper in apertures:
-  ...     afrho = Afrho.from_fluxd('λ5240', flam, aper, eph)
-  ...     print('{:18s} = {:5.0f}'.format(name, afrho))    # doctest: +FLOAT_CMP
+   >>> from sbpy.activity import CircularAperture, AnnularAperture, RectangularAperture, GaussianAperture
+   >>> apertures = (
+   ...   ( '10" radius circle', CircularAperture(10 * u.arcsec)),
+   ...   (    '5"–10" annulus', AnnularAperture([5, 10] * u.arcsec)),
+   ...   (       '2"x10" slit', RectangularAperture([2, 10] * u.arcsec)),
+   ...   ('σ=5" Gaussian beam', GaussianAperture(5 * u.arcsec))
+   ... )
+   >>> for name, aper in apertures:
+   ...     afrho = Afrho.from_fluxd('λ5240', flam, aper, eph)
+   ...     print('{:18s} = {:5.0f}'.format(name, afrho))    # doctest: +FLOAT_CMP
    10" radius circle =  5917 cm
       5"–10" annulus = 11834 cm
          2"x10" slit = 28114 cm
-  σ=5" Gaussian beam =  9442 cm
+   σ=5" Gaussian beam =  9442 cm
 
 
 Reference/API
 -------------
 .. automodapi:: sbpy.activity.dust
    :no-heading:
```

### Comparing `sbpy-0.3.0/docs/sbpy/activity/gas.rst` & `sbpy-0.4.0/docs/sbpy/activity/gas.rst`

 * *Files 1% similar despite different names*

```diff
@@ -99,20 +99,14 @@
   >>> ap = AnnularAperture((5000, 10000) * u.km)
   >>> print(coma.total_number(ap))    # doctest: +FLOAT_CMP
   3.8133654170856037e+31
 
 Vectorial Model
 ^^^^^^^^^^^^^^^
 
-.. warning::
-
-  Literature tests with the Vectorial model are generally in agreement at the
-  20% level or better.  The cause for the differences with the Festou FORTRAN
-  code are not yet precisely known.  Help testing this feature is appreciated.
-
 The Vectorial model (`Festou 1981
 <https://ui.adsabs.harvard.edu/abs/1981A%26A....95...69F/abstract>`_) describes
 the spatial distribution of coma photolysis products.  Unlike the Haser model,
 daughter products in the Vectorial model may receive an additional velocity
 component from the excess energy after photodissociation.  With the
 `~sbpy.activity.gas.Vectorial` class we may compute the column density and total
 number of molecules in an aperture.  Parent and daughter data is provided via
@@ -142,17 +136,17 @@
   >>> hydroxyl = Phys.from_dict({
   ...     'tau_T': gas.photo_timescale('OH') * 0.8,  # approximate
   ...     'v_photo': 1.05 * u.km / u.s
   ... })
   >>> Q = 1e28 / u.s        # water production rate
   >>> coma = gas.VectorialModel(Q, water, hydroxyl)
   >>> print(coma.column_density(10 * u.km))    # doctest: +FLOAT_CMP
-  2.951278139718558e+17 1 / m2
+  2.8976722840952486e+17 1 / m2
   >>> print(coma.total_number(1000 * u.km))    # doctest: +FLOAT_CMP
-  6.96687966256294e+29
+  6.995158827300034e+29
 
 Production Rate calculations
 ----------------------------
 
 Various functions that aid in the calculation of production rates are offered.
 `~sbpy.data.Phys` has a function called `~sbpy.data.Phys.from_jplspec`
 which takes care of querying the JPL Molecular Spectral Catalog through the use of
```

### Comparing `sbpy-0.3.0/docs/sbpy/activity/index.rst` & `sbpy-0.4.0/docs/sbpy/activity/index.rst`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/docs/sbpy/bib.rst` & `sbpy-0.4.0/docs/sbpy/bib.rst`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/docs/sbpy/calib.rst` & `sbpy-0.4.0/docs/sbpy/calib.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,259 +1,279 @@
 .. _sbpy-calib:
 
 Spectral Standards and Photometric Calibration (`sbpy.calib`)
 =============================================================
 
 sbpy's photometric calibration is based on spectra of the Sun and Vega.  For example, they are used to convert between :ref:`reflectance, cross-section, and magnitude <reflectance-equivalencies>`, between :ref:`Afρ and spectral flux density <afrho-to-from-flux-density>`, and between :ref:`Vega-based and other magnitude systems <vega-magnitudes>`.   sbpy has built-in spectra for each, and users may provide their own.
 
-The spectrum of `Bohlin (2014) <https://dx.doi.org/10.1088/0004-6256/147/6/127>`_ is the default and only built-in spectrum for Vega.  It is distributed with sbpy.  Four solar spectra are built-in:
+The spectrum of `Bohlin (2014) <https://dx.doi.org/10.1088/0004-6256/147/6/127>`_ is the default and only built-in spectrum for Vega.  It is distributed with sbpy.  Five solar spectra are built-in:
 
   * Castelli1996 - Castelli model from Colina et al. (1996).
   * E490_2014 - E490 (2014) standard.
   * E490_2014LR - A low resolution version of the E490 standard.
   * Kurucz1993 - Kurucz (1993) model.
+  * calspec - R=5000, created by R. Bohlin from Kurucz Special Model
 
-The E490 spectra are included with sbpy, and the Kurucz and Castelli spectra are downloaded as needed from `STScI's astronomical catalog <https://www.stsci.edu/hst/instrumentation/reference-data-for-calibration-and-tools/astronomical-catalogs>`_.
+The E490 spectra are included with sbpy, and the others are downloaded as needed from MAST's `Spectral Atlas Files for Synphot Software (REFERENCE-ATLASES) <https://archive.stsci.edu/hlsp/reference-atlases>`_ or STScI's `CALSPEC Database <https://www.stsci.edu/hst/instrumentation/reference-data-for-calibration-and-tools/astronomical-catalogs/calspec>`_.
 
 Each star has a class for use within sbpy.  The classes can be initialized with the default spectrum using :func:`~sbpy.calib.SpectralStandard.from_default`:
 
 .. doctest-requires:: synphot
 
-  >>> from sbpy.calib import Sun
-  >>> sun = Sun.from_default()
-  >>> print(sun)
-  <Sun: E490-00a (2014) reference solar spectrum (Table 3)>
+    >>> from sbpy.calib import Sun
+    >>> sun = Sun.from_default()
+    >>> print(sun)
+    <Sun: E490-00a (2014) reference solar spectrum (Table 3)>
 
 The names of the built-in sources are stored as an internal array.  They can be discovered with :func:`~sbpy.calib.SpectralStandard.show_builtin`, and used to initialize an object with :func:`~sbpy.calib.SpectralStandard.from_builtin`:
 
 .. doctest-requires:: synphot
 
-  >>> from sbpy.calib import Sun
-  >>> Sun.show_builtin()
-      name                                description
-  ------------ -----------------------------------------------------------------
-  Castelli1996      Castelli model, scaled and presented by Colina et al. (1996)
-     E490_2014                E490-00a (2014) reference solar spectrum (Table 3)
-   E490_2014LR E490-00a (2014) low resolution reference solar spectrum (Table 4)
-    Kurucz1993               Kurucz (1993) model, scaled by Colina et al. (1996)
-  >>> sun = Sun.from_builtin('E490_2014LR')
-  >>> print(sun)
-  <Sun: E490-00a (2014) low resolution reference solar spectrum (Table 4)>
+    >>> from sbpy.calib import Sun
+    >>> Sun.show_builtin()
+        name                                description
+    ------------ -----------------------------------------------------------------
+    Castelli1996      Castelli model, scaled and presented by Colina et al. (1996)
+       E490_2014                E490-00a (2014) reference solar spectrum (Table 3)
+     E490_2014LR E490-00a (2014) low resolution reference solar spectrum (Table 4)
+      Kurucz1993               Kurucz (1993) model, scaled by Colina et al. (1996)
+         calspec            R=5000, created by R. Bohlin from Kurucz Special Model
+    >>> sun = Sun.from_builtin('E490_2014LR')
+    >>> print(sun)
+    <Sun: E490-00a (2014) low resolution reference solar spectrum (Table 4)>
 
 Controlling the default spectra
 -------------------------------
 
 The Vega and solar spectra in current use are respectively controlled with `~astropy.utils.state.ScienceState` objects named `~sbpy.calib.vega_spectrum` and `~sbpy.calib.solar_spectrum`:
 
 .. doctest-requires:: synphot
 
-  >>> from sbpy.calib import Sun, solar_spectrum
-  >>> solar_spectrum.set('E490_2014LR')
-  <ScienceState solar_spectrum: <Sun: E490-00a (2014) low resolution reference solar spectrum (Table 4)>>
-  >>> # E490 low-resolution spectrum in effect for all of sbpy
-  >>> sun = Sun.from_default()
-  >>> print(sun)
-  <Sun: E490-00a (2014) low resolution reference solar spectrum (Table 4)>
+    >>> from sbpy.calib import Sun, solar_spectrum
+    >>> solar_spectrum.set('E490_2014LR')
+    <ScienceState solar_spectrum: <Sun: E490-00a (2014) low resolution reference solar spectrum (Table 4)>>
+    >>> # E490 low-resolution spectrum in effect for all of sbpy
+    >>> sun = Sun.from_default()
+    >>> print(sun)
+    <Sun: E490-00a (2014) low resolution reference solar spectrum (Table 4)>
 
 `~sbpy.calib.vega_spectrum` and `~sbpy.calib.solar_spectrum` can also be used as a context manager to temporarily change the default spectrum:
 
 .. doctest-requires:: synphot
 
-  >>> from sbpy.calib import Sun, solar_spectrum
-  >>> solar_spectrum.set('E490_2014')  # E490 in effect
-  <ScienceState solar_spectrum: <Sun: E490-00a (2014) reference solar spectrum (Table 3)>>
-  >>> with solar_spectrum.set('E490_2014LR'):
-  ...   # E490 low-res in effect
-  ...   print(Sun.from_default())
-  <Sun: E490-00a (2014) low resolution reference solar spectrum (Table 4)>
-  >>> # Back to module default.
-  >>> print(Sun.from_default())
-  <Sun: E490-00a (2014) reference solar spectrum (Table 3)>
+    >>> from sbpy.calib import Sun, solar_spectrum
+    >>> solar_spectrum.set('E490_2014')  # E490 in effect
+    <ScienceState solar_spectrum: <Sun: E490-00a (2014) reference solar spectrum (Table 3)>>
+    >>> with solar_spectrum.set('E490_2014LR'):
+    ...   # E490 low-res in effect
+    ...   print(Sun.from_default())
+    <Sun: E490-00a (2014) low resolution reference solar spectrum (Table 4)>
+    >>> # Back to module default.
+    >>> print(Sun.from_default())
+    <Sun: E490-00a (2014) reference solar spectrum (Table 3)>
 
 Provide your own solar spectrum with the `~sbpy.calib.Sun` class:
 
 .. doctest-requires:: synphot
 
-  >>> from sbpy.calib import Sun, solar_spectrum
-  >>> with solar_spectrum.set(Sun.from_file('sun.txt')):  # doctest: +SKIP
-  ...   # sun.txt in effect
+    >>> from sbpy.calib import Sun, solar_spectrum
+    >>> with solar_spectrum.set(Sun.from_file('sun.txt')):  # doctest: +SKIP
+    ...   # sun.txt in effect
 
 See `~sbpy.calib.Sun` for more information on ways to create solar spectra.
 
 An example showing how to change the default Vega spectrum:
 
 .. doctest-requires:: synphot
 
-  >>> from sbpy.calib import Vega, vega_spectrum
-  >>> print(Vega.from_default())     # doctest: +SKIP
-  <Vega: Dust-free template spectrum of Bohlin 2014>
-  >>> with vega_spectrum.set(Vega.from_file('vega.txt')):  # doctest: +SKIP
-  ...   # vega.txt in effect
+    >>> from sbpy.calib import Vega, vega_spectrum
+    >>> print(Vega.from_default())     # doctest: +SKIP
+    <Vega: Dust-free template spectrum of Bohlin 2014>
+    >>> with vega_spectrum.set(Vega.from_file('vega.txt')):  # doctest: +SKIP
+    ...   # vega.txt in effect
 
 
 Photometric calibration (without spectra or `synphot`)
 ------------------------------------------------------
 
 The `~astropy.utils.state.ScienceState` objects `~sbpy.calib.solar_fluxd` and `~sbpy.calib.vega_fluxd` control photometric calibration by filter name.  These are completely independent of the spectroscopic calibration and can be used without the optional `synphot` package.  The spectral flux densities (per unit wavelength) of the Sun and Vega are provided and enabled by default.  Values and filters are from Willmer (2018):
 
-  >>> from sbpy.calib import Sun, solar_fluxd, vega_fluxd
-  >>> import sbpy.units as sbu
-  >>>
-  >>> solar_fluxd.set('Willmer2018')   # doctest: +IGNORE_OUTPUT
-  >>> sun = Sun(None)
-  >>> print(sun.observe('PS1 r'))    # doctest: +FLOAT_CMP
-  167.49428760264365 erg / (Angstrom cm2 s)
-  >>> vega_fluxd.set('Willmer2018')   # doctest: +IGNORE_OUTPUT
-  >>> print(sun.observe('PS1 r', unit=sbu.VEGAmag))    # doctest: +FLOAT_CMP
-  -27.05 mag(VEGA)
+.. testsetup::
+.. doctest-requires:: astropy<5.3
+
+    >>> from sbpy.calib import Sun, solar_fluxd, vega_fluxd
+    >>> import sbpy.units as sbu
+
+    .. doctest-requires:: astropy>=5.3
+
+    >>> from sbpy.calib import Sun, solar_fluxd, vega_fluxd
+    >>> import sbpy.units as sbu
+    >>>
+    >>> solar_fluxd.set('Willmer2018')   # doctest: +IGNORE_OUTPUT
+    >>> sun = Sun(None)
+    >>> print(sun.observe('PS1 r'))    # doctest: +FLOAT_CMP
+    167.49428760264365 erg / (Angstrom s cm2)
+    >>> vega_fluxd.set('Willmer2018')   # doctest: +IGNORE_OUTPUT
+    >>> print(sun.observe('PS1 r', unit=sbu.VEGAmag))    # doctest: +FLOAT_CMP
+    -27.05 mag(VEGA)
 
 Use ``solar_fluxd.get('Willmer2018')`` to discover all built-in values.
 
 Users wanting to calibrate data with their own flux densities may do so.  For example, set the *V*-band apparent magnitude of the Sun to that in Colina et al. (1996).  Observations through the ``'V'`` filter will use the specified value:
 
-  >>> solar_fluxd.set({'V': -26.75 * sbu.VEGAmag})  # doctest: +IGNORE_OUTPUT
-  >>> sun = Sun.from_default()
-  >>> print(sun.observe('V'))
-  -26.75 mag(VEGA)
+    >>> solar_fluxd.set({'V': -26.75 * sbu.VEGAmag})  # doctest: +IGNORE_OUTPUT
+    >>> sun = Sun.from_default()
+    >>> print(sun.observe('V'))
+    -26.75 mag(VEGA)
 
 Some sbpy calculations will require the effective wavelength or the pivot wavelength.  These are optional parameters that may be specified with `~sbpy.calib.solar_fluxd` and `~sbpy.calib.vega_fluxd`:
 
-  >>> import astropy.units as u
-  >>> from sbpy.calib import vega_fluxd, Vega
-  >>>
-  >>> # values from Willmer (2018)
-  >>> vega_fluxd.set({
-  ...     'V': 3674.73 * u.Jy,
-  ...     'V(lambda eff)': 5476 * u.AA
-  ... })    # doctest: +IGNORE_OUTPUT
-  <ScienceState vega_fluxd: {'V': <Quantity 3674.73 Jy>, 'V(lambda eff)': <Quantity 5476. Angstrom>}>
-  >>> vega = Vega.from_default()
-  >>> print(vega.observe('V'))
-  3674.73 Jy
-  >>> print(vega.observe('V', unit='erg/(s cm2 AA)'))
-  ...     # doctest: +IGNORE_EXCEPTION_DETAIL
-  Traceback (most recent call last):
-  ...
-  UnitConversionError: 'Jy' (spectral flux density) and 'erg / (Angstrom cm2 s)' (spectral flux density wav) are not convertible  Is "V(lambda pivot)" required and was it provided?
-  >>> vega_fluxd.set({
-  ...     'V': 3674.73 * u.Jy,
-  ...     'V(lambda eff)': 5476 * u.AA,
-  ...     'V(lambda pivot)': 5511 * u.AA
-  ... })    # doctest: +IGNORE_OUTPUT
-  <ScienceState vega_fluxd: {'V': <Quantity 3674.73 Jy>, 'V(lambda eff)': <Quantity 5476. Angstrom>, 'V(lambda pivot)': <Quantity 5511. Angstrom>}>
-  >>> print(vega.observe('V', unit='erg/(s cm2 AA)'))   # doctest: +FLOAT_CMP
-  3.62701e-9 erg / (Angstrom cm2 s)
+.. doctest-requires:: astropy>=5.3
+
+    >>> import astropy.units as u
+    >>> from sbpy.calib import vega_fluxd, Vega
+    >>>
+    >>> # values from Willmer (2018)
+    >>> vega_fluxd.set({
+    ...     'V': 3674.73 * u.Jy,
+    ...     'V(lambda eff)': 5476 * u.AA
+    ... })    # doctest: +IGNORE_OUTPUT
+    <ScienceState vega_fluxd: {'V': <Quantity 3674.73 Jy>, 'V(lambda eff)': <Quantity 5476. Angstrom>}>
+    >>> vega = Vega.from_default()
+    >>> print(vega.observe('V'))
+    3674.73 Jy
+    >>> print(vega.observe('V', unit='erg/(s cm2 AA)'))
+    ...     # doctest: +IGNORE_EXCEPTION_DETAIL
+    Traceback (most recent call last):
+    ...
+    UnitConversionError: 'Jy' (spectral flux density) and 'erg / (Angstrom s cm2)' (spectral flux density wav) are not convertible  Is "V(lambda pivot)" required and was it provided?
+    >>> vega_fluxd.set({
+    ...     'V': 3674.73 * u.Jy,
+    ...     'V(lambda eff)': 5476 * u.AA,
+    ...     'V(lambda pivot)': 5511 * u.AA
+    ... })    # doctest: +IGNORE_OUTPUT
+    <ScienceState vega_fluxd: {'V': <Quantity 3674.73 Jy>, 'V(lambda eff)': <Quantity 5476. Angstrom>, 'V(lambda pivot)': <Quantity 5511. Angstrom>}>
+    >>> print(vega.observe('V', unit='erg/(s cm2 AA)'))   # doctest: +FLOAT_CMP
+    3.62701e-9 erg / (Angstrom s cm2)
 
 Observe the Sun
 ---------------
 
 sbpy can simulate observations of comets and asteroids through spectrometers and filter bandpasses.  To support this functionality, the `~sbpy.calib.Sun` and `~sbpy.calib.Vega` classes have the :func:`~sbpy.calib.SpectralStandard.observe` method that returns simulated flux densities.  Users may request observations through filter bandpasses, or at a set of wavelengths (the default is to rebin the source spectrum).
 
 Get the default solar spectrum, observe it through the Johnson V-band filter (distributed with sbpy), returning the result as a Vega-based magnitude in the Johnson-Morgan system:
 
 .. doctest-requires:: synphot
 
-  >>> from sbpy.calib import Sun
-  >>> from sbpy.photometry import bandpass
-  >>> from sbpy.units import JMmag
-  >>>
-  >>> sun = Sun.from_default()
-  >>> bp = bandpass('Johnson V')
-  >>> fluxd = sun.observe(bp, unit=JMmag)
-  >>> print(fluxd)    # doctest: +FLOAT_CMP
-  -26.744715028702647 mag(JM)
+    >>> from sbpy.calib import Sun
+    >>> from sbpy.photometry import bandpass
+    >>> from sbpy.units import JMmag
+    >>>
+    >>> sun = Sun.from_default()
+    >>> bp = bandpass('Johnson V')
+    >>> fluxd = sun.observe(bp, unit=JMmag)
+    >>> print(fluxd)    # doctest: +FLOAT_CMP
+    -26.744715028702647 mag(JM)
 
 
 Binning versus interpolation with ``observe()``
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If a user requests a series of wavelengths or frequencies with a `~astropy.units.Quantity` object, the default for :func:`~sbpy.calib.SpectralStandard.observe` is to rebin the source spectrum using the requested values as bin centers.  This behavior is appropriate when the source spectrum is at a higher spectral resolution than the requested wavelengths.  This is because `~synphot` assumes source spectra are continuous functions, rather than observations taken through a spectrometer (binned data).
 
 When the requested spectral resolution is comparable to the spectral resolution of the source, rebinning may result in errors at the percent-level or more.  Instead, use the ``interpolate=True`` parameter for ``observe``.
 
 Compare interpolation and rebinning for the E490 low-resolution solar spectrum, using the stored wavelengths of the spectrum.  Initialize a `~sbpy.calib.Sun` object with the low-resolution spectrum.
 
-  >>> import numpy as np
-  >>> from sbpy.calib import Sun
-  >>> sun = Sun.from_builtin('E490_2014LR')
+    >>> import numpy as np
+    >>> from sbpy.calib import Sun
+    >>> sun = Sun.from_builtin('E490_2014LR')
 
 Inspect a sub-set of the data for this example.
 
-  >>> wave = sun.wave[430:435]
-  >>> S = sun.fluxd[430:435]
-  >>> print(wave)    # doctest: +FLOAT_CMP
-  [5495. 5505. 5515. 5525. 5535.] Angstrom
-  >>> print(S)       # doctest: +FLOAT_CMP
-  [1895. 1862. 1871. 1846. 1882.] W / (m2 um)
+.. doctest-requires:: astropy>=5.3
+
+    >>> wave = sun.wave[430:435]
+    >>> S = sun.fluxd[430:435]
+    >>> print(wave)    # doctest: +FLOAT_CMP
+    [5495. 5505. 5515. 5525. 5535.] Angstrom
+    >>> print(S)       # doctest: +FLOAT_CMP
+    [1895. 1862. 1871. 1846. 1882.] W / (um m2)
 
 Interpolate with observe() and compare to the original values.
 
-  >>> S_interp = sun.observe(wave, interpolate=True)
-  >>> np.allclose(S.value, S_interp.value)
-  True
+.. testsetup::
+.. doctest-requires:: astropy<5.3
+
+    >>> wave = sun.wave[430:435]
+    >>> S = sun.fluxd[430:435]
+
+    >>> S_interp = sun.observe(wave, interpolate=True)
+    >>> np.allclose(S.value, S_interp.value)
+    True
 
 Re-bin with observe using the same wavelengths as band centers.
 
-  >>> S_rebin = sun.observe(wave)
-  >>> np.allclose(S.value, S_rebin.value)
-  False
+    >>> S_rebin = sun.observe(wave)
+    >>> np.allclose(S.value, S_rebin.value)
+    False
 
 Inspect the differences.
 
-  >>> print((S_rebin - S) / (S_rebin + S) * 2)    # doctest: +FLOAT_CMP
-  [-0.00429693  0.00281266 -0.00227604  0.00412338 -0.00132301]
+    >>> print((S_rebin - S) / (S_rebin + S) * 2)    # doctest: +FLOAT_CMP
+    [-0.00429693  0.00281266 -0.00227604  0.00412338 -0.00132301]
 
 
 Plot solar spectra
 ^^^^^^^^^^^^^^^^^^
 
 Solar spectra in Sun objects can be plotted at the native resolution of the data, or rebinned. Plot the solar spectrum at the native resolution, and at a resolution of ~25:
 
 .. doctest-skip::
 
-  >>> import astropy.units as u
-  >>> import numpy as np
-  >>> import matplotlib.pyplot as plt
-  >>> from sbpy.calib import Sun
-  >>> # Create an array of wavelengths at R~25
-  >>> wrange = 0.3, 0.8  # wavelength range
-  >>> d = 1 + 1 / 25
-  >>> n = int(np.ceil(np.log(wrange[1] / wrange[0]) / np.log(d)))
-  >>> wave_binned = wrange[0] * d**np.arange(n) * u.um
-  >>> # Get the default solar spectrum, and rebin it
-  >>> sun = Sun.from_default()
-  >>> fluxd_binned = sun.observe(wave_binned, unit='W / (m2 um)')
-  >>> # Plot
-  >>> plt.plot(sun.wave.to('um'), sun.fluxd.to('W/(m2 um)'),
-  ...          drawstyle='steps-mid', color='#1f77b4',
-  ...          label='Native resolution')
-  >>> plt.plot(wave_binned, fluxd_binned, drawstyle='steps-mid',
-  ...          color='#ff7f0e', label='R~25')
-  >>> plt.setp(plt.gca(), xlim=wrange, xlabel='Wavelength (μm)',
-  ...          ylabel='Flux density (W/(m2 μm)')
-  >>> plt.legend()
-  >>> plt.tight_layout()
+    >>> import astropy.units as u
+    >>> import numpy as np
+    >>> import matplotlib.pyplot as plt
+    >>> from sbpy.calib import Sun
+    >>> # Create an array of wavelengths at R~25
+    >>> wrange = 0.3, 0.8  # wavelength range
+    >>> d = 1 + 1 / 25
+    >>> n = int(np.ceil(np.log(wrange[1] / wrange[0]) / np.log(d)))
+    >>> wave_binned = wrange[0] * d**np.arange(n) * u.um
+    >>> # Get the default solar spectrum, and rebin it
+    >>> sun = Sun.from_default()
+    >>> fluxd_binned = sun.observe(wave_binned, unit='W / (m2 um)')
+    >>> # Plot
+    >>> plt.plot(sun.wave.to('um'), sun.fluxd.to('W/(m2 um)'),
+    ...          drawstyle='steps-mid', color='#1f77b4',
+    ...          label='Native resolution')
+    >>> plt.plot(wave_binned, fluxd_binned, drawstyle='steps-mid',
+    ...          color='#ff7f0e', label='R~25')
+    >>> plt.setp(plt.gca(), xlim=wrange, xlabel='Wavelength (μm)',
+    ...          ylabel='Flux density (W/(m2 μm)')
+    >>> plt.legend()
+    >>> plt.tight_layout()
 
 .. plot::
 
-  import astropy.units as u
-  import numpy as np
-  import matplotlib.pyplot as plt
-  from sbpy.calib import Sun
-  wrange = 0.3, 0.8  # wavelength range
-  d = 1 + 1 / 25
-  n = int(np.ceil(np.log(wrange[1] / wrange[0]) / np.log(d)))
-  wave_binned = wrange[0] * d**np.arange(n) * u.um
-  sun = Sun.from_default()
-  fluxd_binned = sun.observe(wave_binned, unit='W / (m2 um)')
-  plt.plot(sun.wave.to('um'), sun.fluxd.to('W/(m2 um)'), drawstyle='steps-mid', color='#1f77b4', label='Native resolution')
-  plt.plot(wave_binned, fluxd_binned, drawstyle='steps-mid', color='#ff7f0e', label='R~25')
-  plt.setp(plt.gca(), xlim=wrange, xlabel='Wavelength (μm)', ylabel='Flux density (W/(m2 μm)')
-  plt.legend()
-  plt.tight_layout()
+    import astropy.units as u
+    import numpy as np
+    import matplotlib.pyplot as plt
+    from sbpy.calib import Sun
+    wrange = 0.3, 0.8  # wavelength range
+    d = 1 + 1 / 25
+    n = int(np.ceil(np.log(wrange[1] / wrange[0]) / np.log(d)))
+    wave_binned = wrange[0] * d**np.arange(n) * u.um
+    sun = Sun.from_default()
+    fluxd_binned = sun.observe(wave_binned, unit='W / (m2 um)')
+    plt.plot(sun.wave.to('um'), sun.fluxd.to('W/(m2 um)'), drawstyle='steps-mid', color='#1f77b4', label='Native resolution')
+    plt.plot(wave_binned, fluxd_binned, drawstyle='steps-mid', color='#ff7f0e', label='R~25')
+    plt.setp(plt.gca(), xlim=wrange, xlabel='Wavelength (μm)', ylabel='Flux density (W/(m2 μm)')
+    plt.legend()
+    plt.tight_layout()
 
 
 Reference/API
 -------------
 .. automodapi:: sbpy.calib
    :no-heading:
    :inherited-members:
```

### Comparing `sbpy-0.3.0/docs/sbpy/data/dataclass.rst` & `sbpy-0.4.0/docs/sbpy/data/dataclass.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .. _data containers:
 
-===============
-Data Containers
-===============
+=======================================
+Data Containers (`sbpy.data.DataClass`)
+=======================================
 
 `sbpy` relies heavily on the use of `~sbpy.data.DataClass` data
 containers that are used to encapsulate data and to propagate them
 through your workflow.
 
 `sbpy` provides data containers for orbital elements
 (`~sbpy.data.Orbit`), ephemerides (`~sbpy.data.Ephem`), observational
@@ -309,14 +309,23 @@
     >>> obs = Obs.from_columns([ra, dec, epoch], names=['ra', 'dec', 't'])
 
 .. doctest::
 
     >>> obs.field_names
     ['ra', 'dec', 't']
 
+You can also use the `in` operator to check if a field is contained in
+a `~sbpy.data.DataClass` object.  Alternative field names can be used
+for the `in` test:
+
+    >>> 'ra' in obs
+    True
+    >>> 'RA' in obs
+    True
+
 Each of these columns can be accessed easily, for instance:
 
     >>> obs['ra']
     <Quantity [10.223423, 10.233453, 10.243452] deg>
 
 which will return an `~astropy.units.quantity.Quantity` object if that
 column has a `~astropy.units.Unit` attached to it or a `~astropy.table.Column`
@@ -398,29 +407,25 @@
 
     >>> obs['ra']
     <Quantity [10.223423, 10.233453, 10.243452] deg>
     >>> obs['ra'] = obs['ra'] + 0.1 * u.deg
     >>> obs['ra']
     <Quantity [10.323423, 10.333453, 10.343452] deg>
 
-More complex data table modifications are possible by directly
-accessing the underlying `~astropy.table.QTable` object as shown below.
-
-`~sbpy.data.DataClass` provides a direct interface to the table
-modification functions provided by `~astropy.table.Table`:
-`~astropy.table.Table.add_row`, `~astropy.table.Table.add_column`,
-`~astropy.table.Table.add_columns`, etc. For instance, it is trivial to add
-additional rows and columns to these objects.
+The basic functionalities to modify the data table are implemented in
+`~sbpy.data.DataClass`, including adding rows and columns and stack a
+DataClass with another DataClass object or an `~astropy.table.Table`
+object.
 
 Let's assume you want to add some more observations to your ``obs``
 object:
 
 .. doctest-requires:: astropy>=5
 
-    >>> obs.table.add_row([10.255460 * u.deg, -12.39460 * u.deg, 2451523.94653 * u.d])
+    >>> obs.add_row([10.255460 * u.deg, -12.39460 * u.deg, 2451523.94653 * u.d])
     >>> obs
     <QTable length=4>
         ra       dec          t      
        deg       deg      
      float64   float64      Time
     --------- --------- -------------
     10.323423 -12.42123  2451523.6234
@@ -429,21 +434,20 @@
      10.25546  -12.3946 2451523.94653
   
 
 or if you want to add a column to your object:
 
 .. doctest-requires:: astropy>=5
 
-    >>> from astropy.table import Column
-    >>> obs.table.add_column(Column(['V', 'V', 'R', 'i'], name='filter'))
+    >>> obs.apply(['V', 'V', 'R', 'i'], name='filter')
     >>> obs
     <QTable length=4>
         ra       dec          t       filter
        deg       deg                        
-     float64   float64       Time      str1 
+     float64   float64       Time     str32
     --------- --------- ------------- ------
     10.323423 -12.42123  2451523.6234      V
     10.333453 -12.41562  2451523.7345      V
     10.343452 -12.40435  2451523.8525      R
      10.25546  -12.3946 2451523.94653      i
 
 The same result can be achieved using the following syntax:
@@ -451,37 +455,64 @@
 .. doctest-requires:: astropy>=5
 
     >>> obs['filter2'] = ['V', 'V', 'R', 'i']
     >>> obs
     <QTable length=4>
         ra       dec          t       filter filter2
        deg       deg                                
-     float64   float64       Time      str1    str1 
+     float64   float64       Time     str32    str1
     --------- --------- ------------- ------ -------
     10.323423 -12.42123  2451523.6234      V       V
     10.333453 -12.41562  2451523.7345      V       V
     10.343452 -12.40435  2451523.8525      R       R
      10.25546  -12.3946 2451523.94653      i       i
 
 Similarly, existing columns can be modified using:
 
 .. doctest-requires:: astropy>=5
 
     >>> obs['filter'] = ['g', 'i', 'R', 'V']
 
-Note how the `~astropy.table.Table.add_column` and
-`~astropy.table.Table.add_row` functions are called from
-``obs.table``. `~sbpy.data.DataClass.table` is a property that exposes
-the underlying `~astropy.table.QTable` object so that the user can
-directly interact with it. Please refer to the `~astropy.table.Table`
-reference and
-[documentation](https://docs.astropy.org/en/stable/table/index.html)
-for more information on how to modify `~astropy.table.QTable` objects.
+If you want to stack two observations into a single object:
 
+.. doctest-requires:: astropy>=5
 
+    >>> ra = [20.223423, 20.233453, 20.243452] * u.deg
+    >>> dec = [12.42123, 12.41562, 12.40435] * u.deg
+    >>> phase = [10.1, 12.3, 15.6] * u.deg
+    >>> epoch = Time(2451623.5 + array([0.1234, 0.2345, 0.3525]), format='jd')
+    >>> obs2 = Obs.from_columns([ra, dec, epoch, phase],
+    ...     names=['ra', 'dec', 't', 'phase'])
+    >>>
+    >>> obs.vstack(obs2)
+    >>> obs
+    <QTable length=7>
+        ra       dec          t       filter filter2  phase
+       deg       deg                                   deg
+     float64   float64       Time      str1    str1  float64
+    --------- --------- ------------- ------ ------- -------
+    10.323423 -12.42123  2451523.6234      g       V     ———
+    10.333453 -12.41562  2451523.7345      i       V     ———
+    10.343452 -12.40435  2451523.8525      R       R     ———
+     10.25546  -12.3946 2451523.94653      V       i     ———
+    20.223423  12.42123  2451623.6234     --      --    10.1
+    20.233453  12.41562  2451623.7345     --      --    12.3
+    20.243452  12.40435  2451623.8525     --      --    15.6
+
+Note that the data table to be stacked doesn't have to have the same
+columns as the original data table.  A keyword `join_type` is used to
+decide how to process the different sets of columns.  See
+`~astropy.table.Table.vstack()` for more detail.
+
+Because the underlying `~astropy.table.QTable` can be exposed by the
+`~sbpy.data.DataClass.table` property, it is possible to modify the data
+table by directly accessing the underlying `~astropy.table.QTable` object.
+However, this is not generally advised.  You should use the mechanisms provided
+by `~sbpy.data.DataClass` to manipulate the data table as much as possible
+to maintain the integrity of the data table.
 
 Additional Data Container Concepts
 ==================================
 
 .. _fieldnames:
 
 Alternative field names
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sbpy-0.3.0/docs/sbpy/data/fieldnames.rst` & `sbpy-0.4.0/docs/sbpy/data/fieldnames.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 .. _field name list:
 
-sbpy Field Names
-================
+===================================
+Data Container Field Name Reference
+===================================
 
 The following table lists field names that are recognized by `sbpy`
 when accessing `~sbpy.data.DataClass` objects, i.e.,
 `~sbpy.data.Ephem`, `~sbpy.data.Orbit`, or `~sbpy.data.Phys`
 objects. Each row of the following table represents one property; for
 each property it lists its description, acceptable field names,
 provenance (which `~sbpy.data.DataClass` class should be used to store
```

### Comparing `sbpy-0.3.0/docs/sbpy/data/index.rst` & `sbpy-0.4.0/docs/sbpy/data/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
 Content
 -------
 
 .. toctree::
    :maxdepth: 2
 
-   dataclass.rst	     
+   dataclass.rst
    ephem.rst
    obs.rst
    orbit.rst
-   phys.rst	      
+   phys.rst
    names.rst
 
 
 Reference/API
 -------------
 .. automodapi:: sbpy.data
     :no-heading:
```

### Comparing `sbpy-0.3.0/docs/sbpy/data/obs.rst` & `sbpy-0.4.0/docs/sbpy/data/obs.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,57 @@
-===========
- Using Obs
-===========
+============================================
+Observational Data Objects (`sbpy.data.Obs`)
+============================================
 
 `~sbpy.data.Obs` objects mostly share their functionality with
 `~sbpy.data.Ephem`, but there are some unique features tailored to observational data.
 
-For instance, this class allows you to query observations reported to
-the Minor Planet Center for a given target:
+For instance, this class allows you to query observations reported to the Minor
+Planet Center for a given target via `astroquery.mpc.MPCClass.get_observations`:
 
-    >>> from sbpy.data import Obs
-    >>> data = Obs.from_mpc('2019 AA', id_type='asteroid designation') # doctest: +REMOTE_DATA
-    >>> data # doctest: +REMOTE_DATA +SKIP
-    <QTable masked=True length=33>
-    number  desig  discovery note1 ...        DEC           mag   band observatory
-				   ...        deg           mag
-    int64    str7     str1    str1 ...      float64       float64 str1     str3
-    ------ ------- --------- ----- ... ------------------ ------- ---- -----------
-	-- 2019 AA        --    -- ...  42.32416944444445    20.2    G         F51
-	-- 2019 AA        --    -- ...  42.32879722222223    20.3    G         F51
-	-- 2019 AA        --    -- ... 42.333225000000006    20.3    G         F51
-	-- 2019 AA         *    -- ...  46.52321666666666    20.0    w         F51
-	-- 2019 AA        --    -- ...  46.52748611111111    20.0    w         F51
-	-- 2019 AA        --    -- ... 46.531755555555556    20.0    w         F51
-       ...     ...       ...   ... ...                ...     ...  ...         ...
-	-- 2019 AA        --    -- ... 46.706500000000005    20.2    V         033
-	-- 2019 AA        --    -- ...  46.70652777777778    20.2    V         033
-	-- 2019 AA        --    -- ...  49.73566111111111    20.1    i         F52
-	-- 2019 AA        --    -- ...  49.73788888888889    20.1    i         F52
-	-- 2019 AA        --    -- ...  49.74008611111111    20.1    i         F52
-	-- 2019 AA        --    -- ... 49.742266666666666    20.2    i         F52
+.. doctest-remote-data:: 
 
+    >>> from sbpy.data import Obs
+    >>> data = Obs.from_mpc('2019 AA', id_type='asteroid designation')
+    >>> data = data[:10]  # limit the number of rows for this example
+    >>> data # doctest: +SKIP
+    <QTable length=10>
+    number  desig  discovery note1 ...         DEC           mag   band observatory
+                                   ...         deg           mag                   
+    int64    str7     str1    str1 ...       float64       float64 str1     str3   
+    ------ ------- --------- ----- ... ------------------- ------- ---- -----------
+        -- 2019 AA        --    -- ... -2.6917250000000004    22.2    w         F51
+        -- 2019 AA        --    -- ... -2.6893833333333337    22.1    w         F51
+        -- 2019 AA        --    -- ... -2.6872222222222226    22.2    w         F51
+        -- 2019 AA        --    -- ...   18.10141666666667    20.3    V         703
+        -- 2019 AA        --    -- ...  18.100916666666667    19.4    V         703
+        -- 2019 AA        --    -- ...  18.100555555555555    20.2    V         703
+        -- 2019 AA        --    -- ...   18.10086111111111    20.8    V         703
+        -- 2019 AA        --    -- ...   22.21022222222222    19.6    V         G96
+        -- 2019 AA        --    -- ...  22.210083333333333    19.8    V         G96
+        -- 2019 AA        --    -- ...   22.21022222222222    20.2    V         G96
 
 For a given `~sbpy.data.Obs` object, `~sbpy.data.Obs.supplement`
 allows you to supplement the information content of this object by
 adding ephemeris data for the target(s) and epochs provided. This
 function makes use of the query functions that are part of
 `~sbpy.data.Ephem` and allows you to pick a service from which you
 would like to obtain the data.
 
-    >>> data.field_names # doctest: +REMOTE_DATA
+.. doctest-remote-data:: 
+
+    >>> data.field_names
     ['number', 'desig', 'discovery', 'note1', 'note2', 'epoch', 'RA', 'DEC', 'mag', 'band', 'observatory']
-    >>> data_sup = data.supplement(id_field='desig') # doctest: +REMOTE_DATA
-    >>> data_sup.field_names # doctest: +REMOTE_DATA
+    >>> data_sup = data.supplement(id_field='desig')
+    >>> data_sup.field_names
     ['number', 'desig', 'discovery', 'note1', 'note2', 'epoch', 'RA_obs', 'DEC_obs', 'mag', 'band', 'observatory', 'targetname', 'H', 'G', 'solar_presence', 'flags', 'RA', 'DEC', 'RA_app', 'DEC_app', 'RA*cos(Dec)_rate', 'DEC_rate', 'AZ', 'EL', 'AZ_rate', 'EL_rate', 'sat_X', 'sat_Y', 'sat_PANG', 'siderealtime', 'airmass', 'magextinct', 'V', 'surfbright', 'illumination', 'illum_defect', 'sat_sep', 'sat_vis', 'ang_width', 'PDObsLon', 'PDObsLat', 'PDSunLon', 'PDSunLat', 'SubSol_ang', 'SubSol_dist', 'NPole_ang', 'NPole_dist', 'EclLon', 'EclLat', 'r', 'r_rate', 'delta', 'delta_rate', 'lighttime', 'vel_sun', 'vel_obs', 'elong', 'elongFlag', 'alpha', 'lunar_elong', 'lunar_illum', 'sat_alpha', 'sunTargetPA', 'velocityPA', 'OrbPlaneAng', 'constellation', 'TDB-UT', 'ObsEclLon', 'ObsEclLat', 'NPole_RA', 'NPole_DEC', 'GlxLon', 'GlxLat', 'solartime', 'earth_lighttime', 'RA_3sigma', 'DEC_3sigma', 'SMAA_3sigma', 'SMIA_3sigma', 'Theta_3sigma', 'Area_3sigma', 'RSS_3sigma', 'r_3sigma', 'r_rate_3sigma', 'SBand_3sigma', 'XBand_3sigma', 'DoppDelay_3sigma', 'true_anom', 'hour_angle', 'alpha_true', 'PABLon', 'PABLat']
     >>> data_sup['r']  # doctest: +SKIP
-    [1.87637455 1.87638696 1.87639935 1.8891401  1.88915504 1.88916999
-     1.88918492 1.88963885 1.88964435 1.88965078 1.8896515  1.88965233
-     1.88965306 1.88970198 1.88970271 1.88970353 1.88970426 1.88970508
-     1.88970581 1.88978031 1.88978103 1.88978186 1.8897826  1.88978341
-     1.88978415 1.88978497 1.88978569 1.88978653 1.88978725 1.90342431
-     1.903438   1.90345164 1.90346529] AU
+    <MaskedQuantity [1.74110682, 1.74111208, 1.74111672, 1.97466336,
+                     1.97465973, 1.97465603, 1.97465236, 1.98676694,
+                     1.98676467, 1.9867624 ] AU>
 
 `~sbpy.data.Obs.supplement` queries in this case ephemerides from the
 JPL Horizons system (the default ``service`` to be used) and appends
 the additional data as new columns to the `~sbpy.data.Obs`
 object. Targetnames and epochs are taken from the underlying
 `~sbpy.data.Obs` object and must hence be present there; keyword
 arguments ``id_field`` and ``epoch_field`` control the fieldnames from
```

### Comparing `sbpy-0.3.0/docs/sbpy/data/orbit.rst` & `sbpy-0.4.0/docs/sbpy/data/orbit.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-=============
- Using Orbit
-=============
+======================================
+Orbit Data Objects (`sbpy.data.Orbit`)
+======================================
 
 Orbit Queries
 =============
 
 `~sbpy.data.Orbit.from_horizons` enables the query of Solar System
 body osculating elements from the `JPL Horizons service
-<https://ssd.jpl.nasa.gov/horizons.cgi>`_:
+<https://ssd.jpl.nasa.gov/horizons/>`_:
 
+.. doctest-remote-data::
+    
     >>> from sbpy.data import Orbit
     >>> from astropy.time import Time
     >>> epoch = Time('2018-05-14', scale='utc')
-    >>> elem = Orbit.from_horizons('Ceres', epochs=epoch)  # doctest: +REMOTE_DATA
+    >>> elem = Orbit.from_horizons('Ceres', epochs=epoch)
     >>> elem  # doctest: +SKIP
     <...>/sbpy/data/orbit.py:113: TimeScaleWarning: converting utc epochs to tdb for use in astroquery.jplhorizons
       TimeScaleWarning)
     <QTable masked=True length=1>
     targetname    H       G    ...         P               epoch      
 		 mag           ...         d                          
        str7    float64 float64 ...      float64            object     
@@ -34,32 +36,36 @@
 If ``epochs`` is not set, the osculating elements for the current
 epoch (current time) are queried. Similar to
 `~sbpy.data.Ephem.from_horizons`, this function is a wrapper for
 `~astroquery.jplhorizons.HorizonsClass.elements` and passes optional
 parameter on to that function. Furthermore, it is possible to query
 orbital elements for a number of targets:
 
+.. doctest-remote-data::
+
     >>> epoch = Time('2018-08-03 14:20', scale='tdb')
     >>> elem = Orbit.from_horizons(['3749', '2009 BR60'],
     ...                            epochs=epoch,
-    ...                            refplane='earth')  # doctest: +REMOTE_DATA
+    ...                            refplane='earth')
     >>> elem # doctest: +SKIP
     <QTable masked=True length=2>
 	  targetname         H       G    ...         P               epoch      
 			    mag           ...         d                          
 	    str21         float64 float64 ...      float64            object     
     --------------------- ------- ------- ... ----------------- -----------------
     3749 Balam (1982 BG1)    13.3    0.15 ... 1221.865723743203 2458334.097222222
        312497 (2009 BR60)    17.7    0.15 ... 1221.776912893334 2458334.097222222
 
 Alternatively, orbital elements can also be queried from the `Minor
 Planet Center <https://minorplanetcenter.net/iau/MPEph/MPEph.html>`_,
 although in this case only the most recent elements are accessible:
 
-    >>> elem = Orbit.from_mpc(['3552', '12893']) # doctest: +SKIP
+.. doctest-remote-data::
+
+    >>> elem = Orbit.from_mpc(['3552', '12893'])
     >>> elem # doctest: +SKIP
     <QTable length=2>
      absmag    Q      arc       w     ...     a        Tj   moid_uranus moid_venus
       mag      AU      d       deg    ...     AU                 AU         AU
     float64 float64 float64  float64  ...  float64  float64   float64    float64
     ------- ------- ------- --------- ... --------- ------- ----------- ----------
        12.9   7.278 12955.0 316.44802 ... 4.2589272     2.3     11.7518    0.56105
@@ -77,15 +83,17 @@
 `sbpy` to provide an interface to `pyoorb
 <https://github.com/oorb/oorb/tree/master/python>`_, a Python module
 using `OpenOrb <https://github.com/oorb/oorb>`_.
 
 In order to transform some current orbits to a state vector in
 cartesian coordinates, one could use the following code:
 
-    >>> elem = Orbit.from_horizons(['Ceres', 'Pallas', 'Vesta'])  # doctest: +REMOTE_DATA
+.. doctest-remote-data::
+
+    >>> elem = Orbit.from_horizons(['Ceres', 'Pallas', 'Vesta'])
     >>> statevec = elem.oo_transform('CART') # doctest: +SKIP 
     >>> statevec # doctest: +SKIP
     <QTable length=3>
        id             x                   y          ...    H       G   
 		      AU                  AU         ...   mag          
       str8         float64             float64       ... float64 float64
     -------- ------------------- ------------------- ... ------- -------
@@ -101,20 +109,79 @@
 ==================
 
 Orbit propagation requires the epoch to which the orbit should be
 propagated to either as `~astropy.time.Time` object, or as float in
 terms of Julian date. The following example propagates the current
 orbit of Ceres back to year 2000:
 
-    >>> elem = Orbit.from_horizons('Ceres')  # doctest: +REMOTE_DATA
-    >>> epoch = Time('2000-01-01')
-    >>> newelem = elem.oo_propagate(epoch) # doctest: +SKIP 
+.. doctest-remote-data::
+
+    >>> elem = Orbit.from_horizons('Ceres')
+    >>> epoch = Time('2000-01-01', scale='tdb')
+    >>> newelem = elem.oo_propagate(epoch) 
     >>> newelem # doctest: +SKIP
     <QTable length=1>
        id           a                  e          ...   epoch      H       G   
 		    AU                            ...             mag          
       str7       float64            float64       ...   object  float64 float64
     ------- ----------------- ------------------- ... --------- ------- -------
     1 Ceres 2.766494220549446 0.07837504411299284 ... 2451544.5    3.34    0.12
 
 Note that both functions require `pyoorb
 <https://github.com/oorb/oorb/tree/master/python>`_ to be installed.
+
+
+Calculate dynamical parameters
+==============================
+
+The Tisserand parameter is a commonly used dynamic parameter to characterize
+the orbit of a small body, especially a comet, when its orbital evolution is
+dominated by the gravitational effect of a particular planet.  The Tisserand
+parameter with respect to Jupiter is used in the dynamical classification of
+comets.  The Tisserand parameter can be calculated by `~sbpy.Orbit.tisserand`
+as follows:
+
+.. doctest-remote-data::
+
+    >>> epoch = Time(2449400.5, format='jd', scale='tdb')
+    >>> halley = Orbit.from_horizons('1P', id_type='designation',
+    ...     closest_apparition=True, epochs=epoch)
+    >>> T = halley.tisserand()
+    >>> print('{:.4f}'.format(T)) # doctest: +SKIP
+    -0.6050
+
+One can also specify the planet with respect to which the Tisserand parameter
+is calculated with optional parameter `planet`.  It also allows multiple
+planet to be specified simultaneously:
+
+.. doctest-remote-data::
+
+    >>> import numpy as np
+    >>> chariklo = Orbit.from_horizons('chariklo', id_type='name')
+    >>> T = chariklo.tisserand(planet=['599', '699', '799', '899'])
+    >>> with np.printoptions(precision=3):
+    ...     print(T)  # doctest: +FLOAT_CMP
+    [3.485 2.931 2.858 3.224]
+
+`~sbpy.Orbit` also provides a method to compare the orbits of two objects
+in terms of the "D-criterion" (`Jopek 1993 <https://ui.adsabs.harvard.edu/abs/1993Icar..106..603J/abstract>`_).  The `~sbpy.Orbit.D_criterion` method
+implements all three versions of the D-criterion, including
+Southworth & Hawkins function (`Southworth and Hawkins 1963 <https://ui.adsabs.harvard.edu/abs/1963SCoA....7..261S/abstract>`_),
+Drummond function (`Drummond 1991 <https://ui.adsabs.harvard.edu/abs/1981Icar...45..545D/abstract>`_), and the hybrid function (`Jopek 1993 <https://ui.adsabs.harvard.edu/abs/1993Icar..106..603J/abstract>`_).
+The code example below demonstrates the calculation of three versions of
+D_criterion:
+
+.. doctest-remote-data::
+
+    >>> comets = Orbit.from_horizons(['252P', 'P/2016 BA14'],
+    ...     id_type='designation', closest_apparition=True)
+    >>>
+    >>> # Southworth & Hawkins function
+    >>> D_SH = comets[0].D_criterion(comets[1])
+    >>> # Drummond function
+    >>> D_D = comets[0].D_criterion(comets[1], version='d')
+    >>> # hybrid function
+    >>> D_H = comets[0].D_criterion(comets[1], version='h')
+    >>> print('D_SH = {:.4f}, D_D = {:.4f}, D_H = {:.4f}'.
+    ...    format(D_SH, D_D, D_H))
+    D_SH = 0.1560, D_D = 0.0502, D_H = 0.1556
+
```

### Comparing `sbpy-0.3.0/docs/sbpy/data/phys.rst` & `sbpy-0.4.0/docs/sbpy/data/phys.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-============
- Using Phys
-============
+========================================
+Physical Data Objects (`sbpy.data.Phys`)
+========================================
 
 `~sbpy.data.Phys` is designed to contain and query physical properties for
 small bodies; functions to query these properties are
 available. `~sbpy.data.Phys.from_sbdb` queries the `JPL Small-body
-Database Browser (SBDB) <https://ssd.jpl.nasa.gov/sbdb.cgi>`_ for physical
+Database Browser (SBDB) <https://ssd.jpl.nasa.gov/tools/sbdb_lookup.html>`_ for physical
 properties and stores the data in a `~sbpy.data.Phys` object, offering
 the same functionality as all the other `~sbpy.data` functions,
 including the use of `~astropy.units`.
 
 As an example, the following code will query the properties for a
 small number of asteroids:
 
     >>> from sbpy.data import Phys
     >>> phys = Phys.from_sbdb(['Ceres', '12893', '3552'])  # doctest: +REMOTE_DATA
     >>> phys['targetname', 'H', 'diameter'] # doctest: +SKIP
     <QTable length=3>
-	    targetname            H    diameter
-					  km
-	      str26            float64 float64
+            targetname            H    diameter
+                                 mag      km   
+              str26            float64 float64 
     -------------------------- ------- --------
-		       1 Ceres    3.34    939.4
-     12893 Mommert (1998 QS55)    13.9    5.214
-    3552 Don Quixote (1983 SA)    12.9     19.0
+             1 Ceres (A801 AA)    3.56    939.4
+     12893 Mommert (1998 QS55)   13.98    5.214
+    3552 Don Quixote (1983 SA)   12.96     19.0
 
 
 Please note that the SBDB database is not complete with respect to
 physical properties and should be considered as a sparse dataset.
 
 `~sbpy.data.Phys` also contains a function to query molecular data that
 might be useful for various calculations such as production rate calculations.
```

### Comparing `sbpy-0.3.0/docs/sbpy/exceptions.rst` & `sbpy-0.4.0/docs/sbpy/exceptions.rst`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/docs/sbpy/photometry.rst` & `sbpy-0.4.0/docs/sbpy/photometry.rst`

 * *Files 10% similar despite different names*

```diff
@@ -81,68 +81,76 @@
 `~sbpy.data.DataClass`, such as `~sbpy.data.Phys`, as long as it contains the
 model parameters:
 
   >>> from sbpy.data import Phys
   >>> phys = Phys.from_sbdb('Ceres')    # doctest: +REMOTE_DATA
   >>> m = HG.from_phys(phys)            # doctest: +REMOTE_DATA
   INFO: Model initialized for 1 Ceres (A801 AA). [sbpy.photometry.core]
-  >>> print(m)                          # doctest: +REMOTE_DATA 
+  >>> print(m)                          # doctest: +SKIP
   Model: HG
   Inputs: ('x',)
   Outputs: ('y',)
   Model set size: 1
   Parameters:
        H    G 
       mag
       ---- ----
-      3.54 0.12
+      3.31 0.12
 
-Note that model set is not supported.  Only one model can be initialized with
-the first set of valid parameters in the input `~sbpy.data.DataClass`.
+Note that in this case, model set is not supported.  Only one model can be
+initialized with the first set of valid parameters in the input
+`~sbpy.data.DataClass`.
 
 To fit a photometric model, one may follow the standard procedure defined in
 `astropy.modeling` submodule, first initializing a model, then using one of
 the fitter classes defined in `astropy.modeling.fitting`
-submodule, such as `~astropy.modeling.fitting.LevMarLSQFitter`.
+submodule, such as `~astropy.modeling.fitting.SLSQPLSQFitter`.  Note that
+the `~sbpy.photometry.HG1G2` model requires that the G1 and G2 parameters
+are bounded within [0, 1], as well as an inequality constraint,
+0 <= 1 - G1 - G2 <= 1.  These constraints are implemented in sbpy via the
+`bounds` parameter of `~astropy.modeling.Parameter` and the `ineqcons`
+parameter of `~astropy.modeling.Model`.  Some fitters, such as
+`astropy.modeling.LevMarLSQFitter`, do not support constrained fit via
+the `ineqcons` parameter, though.
 
   >>> import numpy as np
   >>> import astropy.units as u
-  >>> from astropy.modeling.fitting import LevMarLSQFitter
+  >>> from astropy.modeling.fitting import SLSQPLSQFitter
   >>> # generate data to be fitted
   >>> model1 = HG(3.34 * u .mag, 0.12)
   >>> alpha = np.linspace(0, 40, 20) * u.deg
   >>> mag = model1(alpha) + (np.random.rand(20)*0.2 - 0.1) * u.mag
   >>> # fit new model
-  >>> fitter = LevMarLSQFitter()
+  >>> fitter = SLSQPLSQFitter()
   >>> model2 = HG()
-  >>> model2 = fitter(model2, alpha, mag)
+  >>> model2 = fitter(model2, alpha, mag, verblevel=0)
 
 Alternatively, one may use the class method
 `~sbpy.photometry.DiskIntegratedPhaseFunc.from_obs` to
 initialize a model directly from an `~sbpy.data.Obs` object by fitting the
 data contained therein.
 
   >>> # use class method .from_obs
-  >>> from astropy.modeling.fitting import LevMarLSQFitter
-  >>> fitter = LevMarLSQFitter()
+  >>> from astropy.modeling.fitting import SLSQPLSQFitter
+  >>> fitter = SLSQPLSQFitter()
   >>> from sbpy.data import Obs
   >>> obs = Obs.from_dict({'alpha': alpha, 'mag': mag})
-  >>> model3 = HG12.from_obs(obs, fitter, 'mag')
+  >>> model3 = HG12.from_obs(obs, fitter, 'mag', verblevel=0)
 
 One can also initialize a model set from multiple columns in the input
 `~sbpy.data.Obs` object if it contains more than one columns of brightness
 measurements.  The columns to be fitted are specified by a keyward argument
 ``fields``.  By default, the column ``'mag'`` will be fitted.
 
   >>> # Initialize model set
   >>> model4 = HG(5.2 * u.mag, 0.18)
   >>> mag4 = model4(alpha) + (np.random.rand(20)*0.2 - 0.1) * u.mag
-  >>> fitter = LevMarLSQFitter()
+  >>> fitter = SLSQPLSQFitter()
   >>> obs = Obs.from_dict({'alpha': alpha, 'mag': mag, 'mag1': mag4})
-  >>> model5 = HG.from_obs(obs, fitter, fields=['mag', 'mag1'])
+  >>> model5 = HG.from_obs(obs, fitter, fields=['mag', 'mag1'], verblevel=0)
 
 .. _filter-bandpasses:
 
 Filter Bandpasses
 -----------------
 A few filter bandpasses are included with `sbpy` for internal tests and your convenience.  The function `~sbpy.photometry.bandpass` will return the filter transmission as a `~synphot.spectrum.SpectralElement` (requires `synphot`):
```

### Comparing `sbpy-0.3.0/docs/sbpy/spectroscopy/index.rst` & `sbpy-0.4.0/docs/sbpy/spectroscopy/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -25,41 +25,54 @@
 conversion between spectral gradient and color index (magnitudes), and
 re-normalization to other wavelengths.
 
 `SpectralGradient` is a `~astropy.units.Quantity` with units of
 inverse length.  For convenience, `sbpy` includes a
 `~sbpy.units.hundred_nm` unit, which is equal to 100 nm:
 
+.. testsetup::
+.. doctest-requires:: astropy<5.3
+
+  >>> import astropy.units as u
+  >>> from sbpy.spectroscopy import SpectralGradient
+  >>> from sbpy.units import hundred_nm
+
+.. doctest-requires:: astropy>=5.3
+
   >>> import astropy.units as u
   >>> from sbpy.spectroscopy import SpectralGradient
   >>> from sbpy.units import hundred_nm
   >>> S = SpectralGradient(10 * u.percent / hundred_nm)
   >>> print(S)
-  10.0 % / 100 nm
+  10.0 % / (100 nm)
 
 Initialize a spectral gradient from a color index:
 
+.. doctest-requires:: astropy>=5.3
+
   >>> w = (550, 650) * u.nm
   >>> SpectralGradient.from_color(w, 0.1 * u.mag)  # doctest: +FLOAT_CMP
-  <SpectralGradient 9.20383492 % / 100 nm>
+  <SpectralGradient 9.20383492 % / (100 nm)>
 
 Note we use the dimensionless magnitude unit from `astropy`, i.e., not
 one that carries flux density units such as `astropy.units.ABmag`.
 
 Convert spectral gradient (normalized to 550 nm) to a color index:
 
   >>> S = SpectralGradient(10 * u.percent / hundred_nm, wave0=550 * u.nm)
   >>> S.to_color((500, 600) * u.nm)  # doctest: +FLOAT_CMP
   <Quantity 0.10866423 mag>
 
 Renormalize to 1.0 μm:
 
+.. doctest-requires:: astropy>=5.3
+
   >>> S = SpectralGradient(10 * u.percent / hundred_nm, wave0=550 * u.nm)
   >>> S.renormalize(1 * u.um)  # doctest: +FLOAT_CMP
-  <SpectralGradient 6.89655172 % / 100 nm>
+  <SpectralGradient 6.89655172 % / (100 nm)>
 
 
 Spectral Reddening
 ------------------
 
 Linear spectral reddening is enabled by class `~sbpy.spectroscopy.Reddening`,
 which is based on `~synphot.spectrum.BaseUnitlessSpectrum`.
```

### Comparing `sbpy-0.3.0/docs/sbpy/spectroscopy/sources.rst` & `sbpy-0.4.0/docs/sbpy/spectroscopy/sources.rst`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/docs/sbpy/units.rst` & `sbpy-0.4.0/docs/sbpy/units.rst`

 * *Files 12% similar despite different names*

```diff
@@ -22,17 +22,19 @@
   >>> print(u.percent / (100 * u.nm))
   0.01 % / nm
   >>> print(u.Unit('% / (100 nm)'))    # doctest: +SKIP
   ValueError: '% / (100 nm)' did not parse as unit: Syntax error parsing unit '% / 100 nm'
 
 As a convenience, sbpy defines the `~sbpy.units.hundred_nm` unit, which has an appropriate string representation:
 
+.. doctest-requires:: astropy>=5.3
+
   >>> from sbpy.units import hundred_nm
   >>> print(u.percent / hundred_nm)
-  % / 100 nm
+  % / (100 nm)
 
 .. _vega-magnitudes:
 
 Vega Magnitudes
 ---------------
 
 With the synphot package, sbpy has the capability to convert between flux densities and Vega-based magnitude systems.  The conversions require a spectrum of Vega, which is provided by sbpy's :ref:`calibration system <sbpy-calib>`.
@@ -71,32 +73,48 @@
 expressed in magnitude), and bidirectional reflectance (in unit of 1/sr) and
 scattering cross-section through function `~sbpy.units.reflectance`.
 
 For example, the absolute magnitude of Ceres in V-band is 3.4 in ``VEGAmag``
 system, the radius is 460 km, its disk-averaged bidirectional reflectance at 0
 phase angle can be calculated:
 
+.. doctest-requires:: astropy>=5.3
+
   >>> import numpy as np
   >>> from astropy import units as u
   >>> from sbpy.calib import solar_fluxd, vega_fluxd
   >>> from sbpy.units import reflectance, VEGAmag, spectral_density_vega
   >>>
-  >>> solar_fluxd.set({'V': -26.775 * VEGAmag})
-  <ScienceState solar_fluxd: {'V': <Magnitude -26.775 mag(VEGA)>}>
-  >>> vega_fluxd.set({'V': 3.5885e-08 * u.Unit('W / (m2 um)')})
-  <ScienceState vega_fluxd: {'V': <Quantity 3.5885e-08 W / (m2 um)>}>
+  >>> solar_fluxd.set({"V": -26.775 * VEGAmag, "V(lambda pivot)": 0.55 * u.um})
+  <ScienceState solar_fluxd: {'V': <Magnitude -26.775 mag(VEGA)>, 'V(lambda pivot)': <Quantity 0.55 um>}>
+  >>> vega_fluxd.set({"V": 3.5885e-08 * u.Unit("W / (m2 um)"), "V(lambda pivot)": 0.55 * u.um})
+  <ScienceState vega_fluxd: {'V': <Quantity 3.5885e-08 W / (um m2)>, 'V(lambda pivot)': <Quantity 0.55 um>}>
   >>> mag = 3.4 * VEGAmag
   >>> radius = 460 * u.km
   >>> cross_sec = np.pi * (radius)**2
   >>> ref = mag.to('1/sr', reflectance('V', cross_section=cross_sec))
   >>> print('{0:.4f}'.format(ref))
   0.0287 1 / sr
 
 `~sbpy.units.reflectance` works with `sbpy`'s spectral calibration system (see :ref:`sbpy-calib`):
 
+.. testsetup::
+.. doctest-requires:: astropy<5.3
+
+  >>> import numpy as np
+  >>> from astropy import units as u
+  >>> from sbpy.calib import solar_fluxd, vega_fluxd
+  >>> from sbpy.units import reflectance, VEGAmag, spectral_density_vega
+  >>> solar_fluxd.set({"V": -26.775 * VEGAmag, "V(lambda pivot)": 0.55 * u.um})  # doctest: +IGNORE_OUTPUT
+  >>> vega_fluxd.set({"V": 3.5885e-08 * u.Unit("W / (m2 um)"), "V(lambda pivot)": 0.55 * u.um})  # doctest: +IGNORE_OUTPUT
+  >>> mag = 3.4 * VEGAmag
+  >>> radius = 460 * u.km
+  >>> cross_sec = np.pi * (radius)**2
+  >>> ref = mag.to('1/sr', reflectance('V', cross_section=cross_sec))
+
   >>> from sbpy.photometry import bandpass
   >>> V = bandpass('Johnson V')
   >>> ref = 0.0287 / u.sr
   >>> cross_sec = mag.to('km2', reflectance(V, reflectance=ref))
   >>> radius = np.sqrt(cross_sec / np.pi)
   >>> print('{0:.2f}'.format(radius))
   459.69 km
```

### Comparing `sbpy-0.3.0/docs/static/structure.pdf` & `sbpy-0.4.0/docs/static/structure.pdf`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/docs/static/structure.png` & `sbpy-0.4.0/docs/static/structure.png`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/docs/status.rst` & `sbpy-0.4.0/docs/status.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 .. _status page:
 
 Status Page
 ===========
 
 This page indicates the development status of `sbpy`. The development
-is expected to conclude in 2021.
+is expected to conclude in 2024.
 
-The current development version is **v0.2dev**; its status is as follows:
+The current development version is **v0.5.dev**; its status is as follows:
 
 .. image:: https://github.com/NASA-Planetary-Science/sbpy/actions/workflows/ci_cron_weekly.yml/badge.svg
     :target: https://github.com/NASA-Planetary-Science/sbpy/actions
     :alt: GitHub testing status
 
-.. image:: https://codecov.io/gh/NASA-Planetary-Science/sbpy/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/NASA-Planetary-Science/sbpy/branch/main/graph/badge.svg
     :target: https://app.codecov.io/gh/NASA-Planetary-Science/sbpy
     :alt: codecov status
 
 .. image:: https://readthedocs.org/projects/sbpy/badge/?version=latest
     :target: https://sbpy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
@@ -233,21 +233,21 @@
             </td>
         </tr>
         <tr>
             <td>
                 <em>sbpy.activity.gas</em>
             </td>
             <td align='center'>
-                <span class="dev"></span>
+                <span class="stable"></span>
             </td>
             <td align='center'>
                 MSK / MdVB
             </td>
              <td>
-                Haser model implemented; Vectorial model partially tested;
+                Haser and Vectorial models implemented
             </td>
         </tr>
         <tr>
             <td>
                 <em>sbpy.activity.sublimation</em>
             </td>
             <td align='center'>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 .. _status page: Status Page =========== This page indicates the development
-status of `sbpy`. The development is expected to conclude in 2021. The current
-development version is **v0.2dev**; its status is as follows: .. image:: https:
-//github.com/NASA-Planetary-Science/sbpy/actions/workflows/ci_cron_weekly.yml/
-badge.svg :target: https://github.com/NASA-Planetary-Science/sbpy/actions :alt:
-GitHub testing status .. image:: https://codecov.io/gh/NASA-Planetary-Science/
-sbpy/branch/master/graph/badge.svg :target: https://app.codecov.io/gh/NASA-
-Planetary-Science/sbpy :alt: codecov status .. image:: https://readthedocs.org/
-projects/sbpy/badge/?version=latest :target: https://sbpy.readthedocs.io/en/
-latest/?badge=latest :alt: Documentation Status Current development status
-~~~~~~~~~~~~~~~~~~~~~~~~~~ The current development status of `sbpy` sub-modules
-is indicated in the following tables. The column `Dev` indicates the lead
-developer (MM: Michael Mommert, MSK: Michael S. Kelley, MdVB: Miguel de Val-
-Borro, JYL: Jian-Yang Li) for the respective sub-packages and classes. .. raw::
-html
+status of `sbpy`. The development is expected to conclude in 2024. The current
+development version is **v0.5.dev**; its status is as follows: .. image::
+https://github.com/NASA-Planetary-Science/sbpy/actions/workflows/
+ci_cron_weekly.yml/badge.svg :target: https://github.com/NASA-Planetary-
+Science/sbpy/actions :alt: GitHub testing status .. image:: https://codecov.io/
+gh/NASA-Planetary-Science/sbpy/branch/main/graph/badge.svg :target: https://
+app.codecov.io/gh/NASA-Planetary-Science/sbpy :alt: codecov status .. image::
+https://readthedocs.org/projects/sbpy/badge/?version=latest :target: https://
+sbpy.readthedocs.io/en/latest/?badge=latest :alt: Documentation Status Current
+development status ~~~~~~~~~~~~~~~~~~~~~~~~~~ The current development status of
+`sbpy` sub-modules is indicated in the following tables. The column `Dev`
+indicates the lead developer (MM: Michael Mommert, MSK: Michael S. Kelley,
+MdVB: Miguel de Val-Borro, JYL: Jian-Yang Li) for the respective sub-packages
+and classes. .. raw:: html
     Planned
     Actively developed, be prepared for possible significant changes.
     Reasonably stable, but potentially incomplete; any significant changes/
     additions will generally include backwards-compatiblity.
     Mature. Additions/improvements possible, but no major changes planned.
     Pending deprecation. Might be deprecated in a future version.
     Deprecated. Might be removed in a future version.
@@ -32,15 +32,15 @@
 |________________________|_|_________|for_physical_properties_queries________|
 `sbpy.activity` --------------- .. raw:: html
  _________________________________________________________________________________________________________________
 |Sub-Packages_and_Classes_|�|Dev_|Comments________________________________________________________________________|
 |sbpy.activity.dust       | |MSK |Halley-Marcus phase function implemented; *AfÏ* and *ÎµfÏ* classes fully|
 |_________________________|_|____|implemented;_syndynes_and_synchrones_TBD________________________________________|
 |                         | |MSK |                                                                                |
-|sbpy.activity.gas        | | /  |Haser model implemented; Vectorial model partially tested;                      |
+|sbpy.activity.gas        | | /  |Haser and Vectorial models implemented                                          |
 |_________________________|_|MdVB|________________________________________________________________________________|
 |sbpy.activity.sublimation|_|JYL_|TBD_____________________________________________________________________________|
 `sbpy.photometry` ----------------- .. raw:: html
  _____________________________________________________________________________
 |Sub-Packages_and_Classes|�|Dev|Comments______________________________________|
 |                        | |   |Disk integrated phase functions implemented:  |
 |sbpy.photometry         | |JYL|HG, HG1G2, HG12, HG12_Pen16, linear           |
```

### Comparing `sbpy-0.3.0/examples/activity/estimating-coma-continuum.ipynb` & `sbpy-0.4.0/examples/activity/estimating-coma-continuum.ipynb`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/examples/activity/haser-model.ipynb` & `sbpy-0.4.0/examples/activity/haser-model.ipynb`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/examples/activity/vectorial-model.ipynb` & `sbpy-0.4.0/examples/activity/vectorial-model.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9802266865722793%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(5, 'from astropy.visualization import "*

 * *            "quantity_support\\n'), (6, 'from sbpy.activity.gas.core import VMResult')], delete: "*

 * *            "[5]}}, 5: {'execution_count': 2}, 10: {'execution_count': 11}, 12: "*

 * *            "{'execution_count': 12, 'outputs': {1: {'text': ['Performing setup "*

 * *            "calculations...\\n', 'Starting fragment density computations...\\n', 'Interpolating "*

 * *            "radial fragment density...\\n', 'Computing column densitie […]*

```diff
@@ -8,15 +8,16 @@
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import astropy.units as u\n",
                 "import sbpy.activity as sba\n",
                 "import matplotlib.pyplot as plt\n",
                 "from sbpy.data import Phys\n",
-                "from astropy.visualization import quantity_support"
+                "from astropy.visualization import quantity_support\n",
+                "from sbpy.activity.gas.core import VMResult"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "abstract-paradise",
             "metadata": {},
             "source": [
@@ -49,15 +50,15 @@
                 "\n",
                 "We begin by specifying some physical details about our parent and fragment molecules.\n",
                 "In our example calculations, the parent and fragment molecules are H2O and OH respectively:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 2,
             "id": "narrow-script",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -153,15 +154,15 @@
                 "If no q_t is given, then production is assumed to be steady at base_q.\n",
                 "\n",
                 "Here we construct a water production that varies sinusoidally between 1e28 and 3e28 with a period of 10 hours:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 11,
             "id": "constant-software",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -201,23 +202,35 @@
             "metadata": {},
             "source": [
                 "And we hand this off to the model:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 12,
             "id": "danish-coverage",
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/Users/selfreference/repos/my_sbpy_fork/sbpy/activity/gas/core.py:974: TestingNeeded: Literature tests with the Vectorial model are generally in agreement at the 20% level or better.  The cause for the differences with the Festou FORTRAN code are not yet precisely known.  Help testing this feature is appreciated.\n",
+                        "  warnings.warn(\n"
+                    ]
+                },
+                {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Computing: 100.0 %\r"
+                        "Performing setup calculations...\n",
+                        "Starting fragment density computations...\n",
+                        "Interpolating radial fragment density...\n",
+                        "Computing column densities...\n",
+                        "Vectorial model calculations complete!\n"
                     ]
                 }
             ],
             "source": [
                 "coma_sine = sba.VectorialModel(base_q=base_q*(1/u.s),\n",
                 "                          parent=parent_species,\n",
                 "                          fragment=fragment_species,\n",
@@ -228,15 +241,55 @@
         },
         {
             "cell_type": "markdown",
             "id": "danish-canberra",
             "metadata": {},
             "source": [
                 "# Examining the results\n",
-                "After the calculations are finished, the results are stored in the dictionary `vmodel` and contain information about the volume & column densities, the grids used to in the calculations, and some other things that might be useful."
+                "After the calculations are finished, the results are stored in a VMResult dataclass that holds the volume and column densities, the grids used for both, interpolations of both, and some other quantities to help gauge the quality of the calculation.  It is accessible as the class variable 'vmr':"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "id": "a21c4dfa",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "vmr = coma_sine.vmr"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "cc74ca71",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "## VMResult dataclass overview\n",
+                "### vmr.volume_density_grid, vmr.column_density_grid\n",
+                "Numpy arrays of the radial points around the nucleus that were used in the fragment density calculations\n",
+                "### vmr.volume_density, vmr.column_density\n",
+                "Numpy arrays of volume and column density at the respective grid points given above, with astropy units attached\n",
+                "### vmr.fragment_sputter, vmr.solid_angle_sputter\n",
+                "Two-dimensional information detailing how fragments are ejected from a single column of outflowing parents\n",
+                "### vmr.volume_density_interpolation, vmr.column_density_interpolation\n",
+                "Interpolations of the volume and column density dervide from the gridded values.  The volume density is given in units of 1/m^3, and column density in units of 1/m^2.\n",
+                "### vmr.collision_sphere_radius\n",
+                "Estimate of where the outflowing parents transition from collisional to non-collisional\n",
+                "### vmr.max_grid_radius\n",
+                "How far from the nucleus the grid reaches.  Beyond this value the interpolators above will give an answer, but typically not a useful one.\n",
+                "### vmr.coma_radius\n",
+                "Defines the radius beyond which the model considers there to be no more parents\n",
+                "### vmr.num_fragments_theory\n",
+                "Theoretical count of the total number of fragments we expect - most accurate when there is no time-dependent production\n",
+                "### vmr.num_fragments_grid\n",
+                "Count produced by integrating the volume density over the volume of the entire grid\n",
+                "### vmr.t_perm_flow\n",
+                "Time necessary to reach the permanent flow regime, where production of parents is exactly balanced by parent loss due to photodissociation"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "comfortable-keeping",
             "metadata": {},
             "source": [
@@ -249,95 +302,92 @@
             "metadata": {},
             "source": [
                 "If we need to see the number density of the fragments as computed on the model's grid, we can see that here:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 14,
             "id": "freelance-prime",
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "\n",
                         "Radius (km) vs Fragment density (1/cm3)\n",
                         "---------------------------------------\n",
-                        "    176 km :\t1.506e+05 1 / cm3\n",
-                        "    210 km :\t1.271e+05 1 / cm3\n",
-                        "    250 km :\t1.074e+05 1 / cm3\n",
-                        "    297 km :\t9.092e+04 1 / cm3\n",
-                        "    354 km :\t7.706e+04 1 / cm3\n",
-                        "    421 km :\t6.539e+04 1 / cm3\n",
-                        "    501 km :\t5.555e+04 1 / cm3\n",
-                        "    597 km :\t4.725e+04 1 / cm3\n",
-                        "    710 km :\t4.028e+04 1 / cm3\n",
-                        "    845 km :\t3.443e+04 1 / cm3\n",
-                        "   1006 km :\t2.949e+04 1 / cm3\n",
-                        "   1197 km :\t2.531e+04 1 / cm3\n",
-                        "   1424 km :\t2.179e+04 1 / cm3\n",
-                        "   1695 km :\t1.881e+04 1 / cm3\n",
-                        "   2017 km :\t1.628e+04 1 / cm3\n",
-                        "   2401 km :\t1.413e+04 1 / cm3\n",
-                        "   2857 km :\t1.229e+04 1 / cm3\n",
-                        "   3400 km :\t1.071e+04 1 / cm3\n",
-                        "   4047 km :\t9.350e+03 1 / cm3\n",
-                        "   4816 km :\t8.168e+03 1 / cm3\n",
-                        "   5731 km :\t7.133e+03 1 / cm3\n",
-                        "   6821 km :\t6.215e+03 1 / cm3\n",
-                        "   8118 km :\t5.384e+03 1 / cm3\n",
-                        "   9661 km :\t4.608e+03 1 / cm3\n",
-                        "  11497 km :\t3.863e+03 1 / cm3\n",
-                        "  13682 km :\t3.137e+03 1 / cm3\n",
-                        "  16283 km :\t2.437e+03 1 / cm3\n",
-                        "  19379 km :\t1.793e+03 1 / cm3\n",
-                        "  23062 km :\t1.247e+03 1 / cm3\n",
-                        "  27446 km :\t8.475e+02 1 / cm3\n",
-                        "  32663 km :\t6.049e+02 1 / cm3\n",
-                        "  38872 km :\t4.702e+02 1 / cm3\n",
-                        "  46262 km :\t3.600e+02 1 / cm3\n",
-                        "  55055 km :\t2.477e+02 1 / cm3\n",
-                        "  65521 km :\t1.713e+02 1 / cm3\n",
-                        "  77976 km :\t1.195e+02 1 / cm3\n",
-                        "  92798 km :\t7.363e+01 1 / cm3\n",
-                        " 110438 km :\t4.693e+01 1 / cm3\n",
-                        " 131431 km :\t2.933e+01 1 / cm3\n",
-                        " 156414 km :\t1.726e+01 1 / cm3\n",
-                        " 186147 km :\t9.656e+00 1 / cm3\n",
-                        " 221532 km :\t5.481e+00 1 / cm3\n",
-                        " 263643 km :\t2.977e+00 1 / cm3\n",
-                        " 313758 km :\t1.519e+00 1 / cm3\n",
-                        " 373401 km :\t7.649e-01 1 / cm3\n",
-                        " 444380 km :\t3.623e-01 1 / cm3\n",
-                        " 528852 km :\t1.660e-01 1 / cm3\n",
-                        " 629381 km :\t6.543e-02 1 / cm3\n",
-                        " 749020 km :\t2.549e-02 1 / cm3\n",
-                        " 891401 km :\t9.045e-03 1 / cm3\n"
+                        "    176 km :\t1.553e+05 1 / cm3\n",
+                        "    210 km :\t1.310e+05 1 / cm3\n",
+                        "    250 km :\t1.106e+05 1 / cm3\n",
+                        "    297 km :\t9.353e+04 1 / cm3\n",
+                        "    354 km :\t7.912e+04 1 / cm3\n",
+                        "    421 km :\t6.701e+04 1 / cm3\n",
+                        "    501 km :\t5.684e+04 1 / cm3\n",
+                        "    597 km :\t4.829e+04 1 / cm3\n",
+                        "    710 km :\t4.110e+04 1 / cm3\n",
+                        "    845 km :\t3.505e+04 1 / cm3\n",
+                        "   1006 km :\t2.996e+04 1 / cm3\n",
+                        "   1197 km :\t2.567e+04 1 / cm3\n",
+                        "   1424 km :\t2.206e+04 1 / cm3\n",
+                        "   1695 km :\t1.901e+04 1 / cm3\n",
+                        "   2017 km :\t1.643e+04 1 / cm3\n",
+                        "   2401 km :\t1.424e+04 1 / cm3\n",
+                        "   2857 km :\t1.237e+04 1 / cm3\n",
+                        "   3400 km :\t1.077e+04 1 / cm3\n",
+                        "   4047 km :\t9.394e+03 1 / cm3\n",
+                        "   4816 km :\t8.201e+03 1 / cm3\n",
+                        "   5731 km :\t7.155e+03 1 / cm3\n",
+                        "   6821 km :\t6.232e+03 1 / cm3\n",
+                        "   8118 km :\t5.395e+03 1 / cm3\n",
+                        "   9661 km :\t4.616e+03 1 / cm3\n",
+                        "  11497 km :\t3.868e+03 1 / cm3\n",
+                        "  13682 km :\t3.140e+03 1 / cm3\n",
+                        "  16283 km :\t2.440e+03 1 / cm3\n",
+                        "  19379 km :\t1.795e+03 1 / cm3\n",
+                        "  23062 km :\t1.248e+03 1 / cm3\n",
+                        "  27446 km :\t8.478e+02 1 / cm3\n",
+                        "  32663 km :\t6.053e+02 1 / cm3\n",
+                        "  38872 km :\t4.707e+02 1 / cm3\n",
+                        "  46262 km :\t3.602e+02 1 / cm3\n",
+                        "  55055 km :\t2.475e+02 1 / cm3\n",
+                        "  65521 km :\t1.711e+02 1 / cm3\n",
+                        "  77976 km :\t1.198e+02 1 / cm3\n",
+                        "  92798 km :\t7.374e+01 1 / cm3\n",
+                        " 110438 km :\t4.676e+01 1 / cm3\n",
+                        " 131431 km :\t2.942e+01 1 / cm3\n",
+                        " 156414 km :\t1.725e+01 1 / cm3\n",
+                        " 186147 km :\t9.686e+00 1 / cm3\n",
+                        " 221532 km :\t5.478e+00 1 / cm3\n",
+                        " 263643 km :\t2.962e+00 1 / cm3\n",
+                        " 313758 km :\t1.525e+00 1 / cm3\n",
+                        " 373401 km :\t7.704e-01 1 / cm3\n",
+                        " 444380 km :\t3.687e-01 1 / cm3\n",
+                        " 528852 km :\t1.647e-01 1 / cm3\n",
+                        " 629381 km :\t6.962e-02 1 / cm3\n",
+                        " 749020 km :\t2.709e-02 1 / cm3\n",
+                        " 891401 km :\t9.271e-03 1 / cm3\n"
                     ]
                 }
             ],
             "source": [
                 "print(\"\\n\\nRadius (km) vs Fragment density (1/cm3)\\n---------------------------------------\")\n",
-                "volume_densities = list(zip(coma_sine.vmodel['radial_grid'], coma_sine.vmodel['radial_density']))\n",
-                "for pair in volume_densities:\n",
-                "    print(f'{pair[0].to(u.km):7.0f} :\\t{pair[1].to(1/(u.cm**3)):5.3e}')"
+                "for r, n_r in zip(vmr.volume_density_grid, vmr.volume_density):\n",
+                "    print(f'{r.to(u.km):7.0f} :\\t{n_r.to(1/(u.cm**3)):5.3e}')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "capable-barrel",
             "metadata": {},
             "source": [
-                "An interpolated function of this volume density is also available at `coma.vmodel['r_dens_interpolation']` that takes its argument in meters (no astropy units) and returns the volume density in 1/m^3 (also no units).\n",
-                "\n",
                 "Note that the volume density is only tracked out to a certain radius, which can cause the column density at the edge of the coma to behave strangely if there is a significant amount of fragments near the edge of the model's grid."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "anticipated-amendment",
             "metadata": {},
@@ -345,238 +395,242 @@
                 "## Fragment column density\n",
                 "\n",
                 "### Printing the results from the grid"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 15,
             "id": "static-bookmark",
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "Radius (km) vs Column density (1/cm2)\n",
                         "-------------------------------------\n",
-                        "    176 km :\t4.196e+13 1 / cm2\n",
-                        "    210 km :\t4.105e+13 1 / cm2\n",
-                        "    250 km :\t4.015e+13 1 / cm2\n",
-                        "    297 km :\t3.925e+13 1 / cm2\n",
-                        "    354 km :\t3.834e+13 1 / cm2\n",
-                        "    421 km :\t3.744e+13 1 / cm2\n",
-                        "    501 km :\t3.653e+13 1 / cm2\n",
-                        "    597 km :\t3.561e+13 1 / cm2\n",
-                        "    710 km :\t3.470e+13 1 / cm2\n",
-                        "    845 km :\t3.378e+13 1 / cm2\n",
-                        "   1006 km :\t3.285e+13 1 / cm2\n",
-                        "   1197 km :\t3.191e+13 1 / cm2\n",
-                        "   1424 km :\t3.096e+13 1 / cm2\n",
-                        "   1695 km :\t3.000e+13 1 / cm2\n",
-                        "   2017 km :\t2.902e+13 1 / cm2\n",
-                        "   2401 km :\t2.801e+13 1 / cm2\n",
-                        "   2857 km :\t2.698e+13 1 / cm2\n",
-                        "   3400 km :\t2.590e+13 1 / cm2\n",
-                        "   4047 km :\t2.478e+13 1 / cm2\n",
-                        "   4816 km :\t2.360e+13 1 / cm2\n",
-                        "   5731 km :\t2.235e+13 1 / cm2\n",
-                        "   6821 km :\t2.100e+13 1 / cm2\n",
-                        "   8118 km :\t1.953e+13 1 / cm2\n",
-                        "   9661 km :\t1.792e+13 1 / cm2\n",
-                        "  11497 km :\t1.615e+13 1 / cm2\n",
-                        "  13682 km :\t1.423e+13 1 / cm2\n",
-                        "  16283 km :\t1.223e+13 1 / cm2\n",
-                        "  19379 km :\t1.025e+13 1 / cm2\n",
-                        "  23062 km :\t8.468e+12 1 / cm2\n",
-                        "  27446 km :\t7.021e+12 1 / cm2\n",
-                        "  32663 km :\t5.934e+12 1 / cm2\n",
-                        "  38872 km :\t5.043e+12 1 / cm2\n",
-                        "  46262 km :\t4.140e+12 1 / cm2\n",
+                        "    176 km :\t4.243e+13 1 / cm2\n",
+                        "    210 km :\t4.148e+13 1 / cm2\n",
+                        "    250 km :\t4.055e+13 1 / cm2\n",
+                        "    297 km :\t3.962e+13 1 / cm2\n",
+                        "    354 km :\t3.868e+13 1 / cm2\n",
+                        "    421 km :\t3.774e+13 1 / cm2\n",
+                        "    501 km :\t3.681e+13 1 / cm2\n",
+                        "    597 km :\t3.587e+13 1 / cm2\n",
+                        "    710 km :\t3.492e+13 1 / cm2\n",
+                        "    845 km :\t3.398e+13 1 / cm2\n",
+                        "   1006 km :\t3.302e+13 1 / cm2\n",
+                        "   1197 km :\t3.207e+13 1 / cm2\n",
+                        "   1424 km :\t3.110e+13 1 / cm2\n",
+                        "   1695 km :\t3.012e+13 1 / cm2\n",
+                        "   2017 km :\t2.912e+13 1 / cm2\n",
+                        "   2401 km :\t2.810e+13 1 / cm2\n",
+                        "   2857 km :\t2.705e+13 1 / cm2\n",
+                        "   3400 km :\t2.597e+13 1 / cm2\n",
+                        "   4047 km :\t2.484e+13 1 / cm2\n",
+                        "   4816 km :\t2.365e+13 1 / cm2\n",
+                        "   5731 km :\t2.238e+13 1 / cm2\n",
+                        "   6821 km :\t2.103e+13 1 / cm2\n",
+                        "   8118 km :\t1.955e+13 1 / cm2\n",
+                        "   9661 km :\t1.794e+13 1 / cm2\n",
+                        "  11497 km :\t1.616e+13 1 / cm2\n",
+                        "  13682 km :\t1.424e+13 1 / cm2\n",
+                        "  16283 km :\t1.224e+13 1 / cm2\n",
+                        "  19379 km :\t1.026e+13 1 / cm2\n",
+                        "  23062 km :\t8.473e+12 1 / cm2\n",
+                        "  27446 km :\t7.025e+12 1 / cm2\n",
+                        "  32663 km :\t5.937e+12 1 / cm2\n",
+                        "  38872 km :\t5.046e+12 1 / cm2\n",
+                        "  46262 km :\t4.141e+12 1 / cm2\n",
                         "  55055 km :\t3.256e+12 1 / cm2\n",
-                        "  65521 km :\t2.549e+12 1 / cm2\n",
-                        "  77976 km :\t1.935e+12 1 / cm2\n",
-                        "  92798 km :\t1.393e+12 1 / cm2\n",
+                        "  65521 km :\t2.550e+12 1 / cm2\n",
+                        "  77976 km :\t1.938e+12 1 / cm2\n",
+                        "  92798 km :\t1.394e+12 1 / cm2\n",
                         " 110438 km :\t1.012e+12 1 / cm2\n",
-                        " 131431 km :\t7.060e+11 1 / cm2\n",
-                        " 156414 km :\t4.734e+11 1 / cm2\n",
-                        " 186147 km :\t3.080e+11 1 / cm2\n",
-                        " 221532 km :\t1.985e+11 1 / cm2\n",
-                        " 263643 km :\t1.214e+11 1 / cm2\n",
-                        " 313758 km :\t7.121e+10 1 / cm2\n",
-                        " 373401 km :\t4.046e+10 1 / cm2\n",
-                        " 444380 km :\t2.154e+10 1 / cm2\n",
-                        " 528852 km :\t1.077e+10 1 / cm2\n",
-                        " 629381 km :\t4.645e+09 1 / cm2\n",
-                        " 749020 km :\t1.846e+09 1 / cm2\n",
-                        " 891401 km :\t0.000e+00 1 / cm2\n"
+                        " 131431 km :\t7.079e+11 1 / cm2\n",
+                        " 156414 km :\t4.738e+11 1 / cm2\n",
+                        " 186147 km :\t3.091e+11 1 / cm2\n",
+                        " 221532 km :\t1.987e+11 1 / cm2\n",
+                        " 263643 km :\t1.218e+11 1 / cm2\n",
+                        " 313758 km :\t7.209e+10 1 / cm2\n",
+                        " 373401 km :\t4.121e+10 1 / cm2\n",
+                        " 444380 km :\t2.219e+10 1 / cm2\n",
+                        " 528852 km :\t1.122e+10 1 / cm2\n",
+                        " 629381 km :\t5.316e+09 1 / cm2\n",
+                        " 749020 km :\t2.293e+09 1 / cm2\n",
+                        " 891401 km :\t8.475e+08 1 / cm2\n"
                     ]
                 }
             ],
             "source": [
                 "print(\"\\nRadius (km) vs Column density (1/cm2)\\n-------------------------------------\")\n",
-                "column_densities = list(zip(coma_sine.vmodel['column_density_grid'], coma_sine.vmodel['column_densities']))\n",
-                "for pair in column_densities:\n",
-                "    print(f'{pair[0].to(u.km):7.0f} :\\t{pair[1].to(1/(u.cm**2)):5.3e}')"
+                "for r, cd in zip(vmr.column_density_grid, vmr.column_density):\n",
+                "    print(f'{r.to(u.km):7.0f} :\\t{cd.to(1/(u.cm**2)):5.3e}')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "academic-beaver",
             "metadata": {},
             "source": [
                 "### Graphing the column density\n",
                 "\n",
                 "To visualize the results, we can see the column density results from the grid used in the calculations alongside the interpolated column density, with an additional comparison to a linear interpolation of the grid:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 16,
             "id": "activated-graduation",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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c84gOyeXl197l5KSEg4dKmTpstUAXDz6PJ58+hX27t3Pvn15PD7lZS47QdDRIbkNn335LTabjbk/z2fBn/8cklcdhp09mA2bUvn62zlYrVZefeN9cvYcC6duvO5ynn7utbJJv/PzC5jx9exKHXvG17PJyMgGoEFIMAYDFc4v9fefD4CPjw8jzx/K5dfcTrcuHWgSW3Evru5dO+Ln58uzL0zFYrHw+4LFzP5xHheNHlGpGh9+4C4WL13JQ488TV7eAQ4dKuS1qR8w7dOZTHl8QqWOISIiIq6ngEhERMQF7r7zRp576mGefPoVGjVpT1zL7rz+5oecN/wsAJ6Z8hCfffktwRGJ3HjreMaMHH7CYz075SHatkmke99zCYtux4SHnsRutxMcHMRrLz3BDbeMJza+K/7+vsRER1Z4jCsuG0WTJtHExnelbadBdO/Wqdz6a6+6mE2b0mgY2YYLxlyHyWRi1swPWJOygRZJvYmIbc8Nt4wnv+AQ4AwNmjSJoUXr3pw94jIuv+SfkyMfFRgYwE+zP2H2j/OIataZVu368fsCZw+mB++/g86dkunQbQjtu55Jxw5tefD+Oyo8zovPPsrsH+fRMLINn37xbdm1rG5hYQ35YvpUHnh4CuExyaRt3UHvnsd6B11w3jnce/ctXHrVrYQ0SiK5yxnM/Wl+pY69YuVaevYfTlB4K84ffS0vPvsYzZv9czje338+R115+SjWrd/MZScYXgbg5eXFd1+9z9yf5xMR257bxj7Ih++8SGKr+ErV2DK+GQvmzWTtuk00T+pFdPPOfP3tj8yZNZ3ePbv++wFERESkVjDYitIr6LAuIiIiInXd7vRMWncYQNaOVQQFBbq6HBEREanF1INIREREpB6y2+28+Mo7XDRqhMIhERER+Vcnfr6uiIiIiNRJhw8XEdm0I3FNYvjxu4rnrxIRERE5noaYiYiIiIiIiIi4OQ0xExERERERERFxcwqIRERERERERETcnAIiERERERERERE3p4BIRERERERERMTNKSASEREREREREXFzCohERERERERERNycAiIRERERERERETengEhERERERERExM0pIBIRERERERERcXMKiERERERERERE3JwCIhERERERERERN6eASERERERERETEzSkgEhERERERERFxcwqIRERERERERETcnAIiERERERERERE3p4BIRERERERERMTNKSASEREREREREXFzCohERERERERERNycAiIRERERERERETengEhERERERERExM0pIBIRERERERERcXMKiERERERERERE3JwCIhERERERERERN6eASERERERERETEzSkgEhERERERERFxcwqIRERERERERETcnAIiERERERERERE3p4BIRERERERERMTNKSASEREREREREXFzCohERERERERERNycAiIRERERERERETengEhERERERERExM0pIBIRERERERERcXMKiERERERERERE3JwCIhERERERERERN6eASERERERERETEzSkgEhERERERERFxcwqIRERERERERETcnAIiERERERERERE3p4BIRERERERERMTNKSASEREREREREXFzCohERERERERERNycAiIRERERERERETengEhERERERERExM0pIBIRERERERERcXMKiERERERERERE3JwCIhERERERERERN+fh6gJO5uPv/2Td1gwC/X14+IbzT7pt2u4cvvx5GZm5B7jugv50TmoKwJad2cz4ZVnZdjn787n+gv50aBVXjZWLiIiIiIiIiNQdtTog6tk+ngFdkvjw+4X/um2DIH+uGt6HX5ZuKLe8VdNIHvrfeQAcNpcw8Y2ZtG4eXS31ioiIiIiIiIjURbU6IGrZpDH7Dh4qt2zvgQI+m7uEwqISvDxNXD60F43DQggLCQTAYDjx8VZt2kmbFjF4edbqZouIiIiIiIiI1Kg6l5RM/3Exl57Tk0YNg9iRuZfP5i7hrsvPrtS+KzbuYHD3NtVcoYiIiIiIiIhI3VKnAqLiUgvbM3J5Z+b8smVWm71S++YfKiJz7wHaaHiZiIiIiIiIiEg5dSogcjgc+Hp7lc0pdCpWbNpJh4Q4TCY9uE1ERERERERE5Hh1Ki3x9fYiLCSAlZt2As7AKGNPXqX2XbFhO13bNKvG6kRERERERERE6iaDrSjd4eoiTuTdb/4gdVcOheZigvx9Gd6vA62aRvLpnMXkF5qx2e10bd2MYX07sDNrH29+9RtFxaV4epgI8vflkRvPB2DfwUM8+9EcptwxGuPJZrEWEREREREREXFDtTogEhERERERERGR6lenhpiJiIiIiIiIiEjVq7WTVOcXFFT5MTftdw4vSwqt3Z2mDAYDDkftrrG6uHPbwb3b785t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\n",
+                        "image/png": "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n3zL2P6dKV865F/tc82mHVxRNZIyJYPyOVoRERERERERERERESlIxaZw+5ETCWz4azf972hDzUrlKRcawi3N6lOjYnnWbt7xr/Z5KjGFv3YdpMWVGkUiIiIiIiIiIiIiIlLYFJuRJPvjj2MCz0xd6NFudzgI9Pf7V/tcu2Un/iV8ubJ2pXyIUERERERERERERERELqVikyQxTROLYTCqbzQWw/BY5+d78afBNE3WbN5B0wbVsVmt+RWmiIiIiIiIiIiIiIhcIsUmSVKxfGmcpklicho1K5X/z/vbvj+eIycSaaGC7SIiIiIiIiIiIiIihVKRSpKkZdg5cjzBvXz0ZBIH4o8R6O9H+TIlaVK/GjOXrKLbTddSMbw0SSnp/LM3jsiwUBrUiAIg9shJHA4HKakZpGXYORB/DICK4WU8jvXzph1UjSxLhbDQS/cBRUREREREREREREQk3xiOlAOmt4PIL//si+O12d/kaG/WsDq9o1vhcDj5cvVm1v2xi5OJKQT6+1EtqhzRra9yJztGvzWf46eSc+zjnad6u9+npmXw5Otz6XFLU1pdVavAPo+IiIiIiIiIiIiIiBScIpUkERERERERERERERERySuLtwMQERERERERERERERHxhkJfk8TpdLrfG4bhxUhERERERC4N08weDG6x6LknuTD9v0lEREREipOL+T9ToU+SACQmJXk7BBERERGRSy44KMjbIUghov83iYiIiEhxk5f/M+mxs/+gx2IfbvzUlx6LfbwdSoExDIOQ4GA9bVZAdH4Lls5vwdL5LVg6vwVP57hg6fyKyNn0e6Hw0zUsPM51v0LXsPDTNSzcdP0KP13DoqnQJ0lOf0N64xszNdMgxW6Qmll0fygMw3C/JP/p/BYsnd+CpfNbsHR+C57OccHS+S1Y3vwbWAqny+F7Rb8XCj9dw8LjXPcrdA0LP13Dwk3Xr/DTNSx88nKtCn2SRERERERERERERERE5N9QkkRERERERERERERERIolJUlERERERERERERERKRYUpJERERERERERERERESKJZu3AxAREREREZGCsWLDVlZs3IavzcqQ7m28HY6IiIiIyGVHSRIREREREZEiqk3jOrRpXAfTNElITPR2OCIiIiIilx1NtyUiIiIiIiIiIiIiIsWSkiQiIiIiIiIiIiIiIlIsKUkiIiIiIiIiIiIi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",
                         "text/plain": [
-                            "<Figure size 1440x720 with 2 Axes>"
+                            "<Figure size 2000x1000 with 2 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "solarbluecol = np.array([38, 139, 220]) / 255.\n",
                 "solarblue = (solarbluecol[0], solarbluecol[1], solarbluecol[2], 1)\n",
                 "solargreencol = np.array([133, 153, 0]) / 255.\n",
                 "solargreen = (solargreencol[0], solargreencol[1], solargreencol[2], 1)\n",
                 "solarblackcol = np.array([0, 43, 54]) / 255.\n",
                 "solarblack = (solarblackcol[0], solarblackcol[1], solarblackcol[2], 1)\n",
                 "\n",
-                "def show_column_density_plots(coma, r_units, cd_units, frag_name):\n",
+                "def show_column_density_plots(vmr, r_units, cd_units, frag_name):\n",
                 "    \"\"\" Show the radial density of the fragment species \"\"\"\n",
                 "\n",
                 "    x_min_logplot = 3\n",
                 "    x_max_logplot = 9\n",
                 "\n",
                 "    x_min_linear = (0 * u.km).to(u.m)\n",
                 "    x_max_linear = (2000 * u.km).to(u.m)\n",
                 "\n",
                 "    lin_interp_x = np.linspace(x_min_linear.value, x_max_linear.value, num=200)\n",
-                "    lin_interp_y = coma.vmodel['column_density_interpolation'](lin_interp_x)/(u.m**2)\n",
+                "    lin_interp_y = vmr.column_density_interpolation(lin_interp_x)/(u.m**2)\n",
                 "    lin_interp_x *= u.m\n",
-                "    lin_interp_x.to(r_units)\n",
                 "\n",
                 "    log_interp_x = np.logspace(x_min_logplot, x_max_logplot, num=200)\n",
-                "    log_interp_y = coma.vmodel['column_density_interpolation'](log_interp_x)/(u.m**2)\n",
+                "    log_interp_y = vmr.column_density_interpolation(log_interp_x)/(u.m**2)\n",
                 "    log_interp_x *= u.m\n",
-                "    log_interp_x.to(r_units)\n",
                 "\n",
                 "    plt.style.use('Solarize_Light2')\n",
                 "\n",
                 "    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(20, 10))\n",
                 "\n",
                 "    ax1.set(xlabel=f'Distance from nucleus, {r_units.to_string()}')\n",
                 "    ax1.set(ylabel=f\"Fragment column density, {cd_units.unit.to_string()}\")\n",
                 "    ax2.set(xlabel=f'Distance from nucleus, {r_units.to_string()}')\n",
                 "    ax2.set(ylabel=f\"Fragment column density, {cd_units.unit.to_string()}\")\n",
                 "    fig.suptitle(f\"Calculated column density of {frag_name}\")\n",
                 "\n",
                 "    ax1.set_xlim([x_min_linear, x_max_linear])\n",
                 "    ax1.plot(lin_interp_x, lin_interp_y, color=\"red\",  linewidth=2.5, linestyle=\"-\", label=\"cubic spline\")\n",
-                "    ax1.plot(coma.vmodel['column_density_grid'], coma.vmodel['column_densities'], 'bo', label=\"model\")\n",
-                "    ax1.plot(coma.vmodel['column_density_grid'], coma.vmodel['column_densities'], 'g--', label=\"linear interpolation\")\n",
+                "    ax1.plot(vmr.column_density_grid, vmr.column_density, 'bo', label=\"model\")\n",
+                "    ax1.plot(vmr.column_density_grid, vmr.column_density, 'g--', label=\"linear interpolation\")\n",
                 "\n",
                 "    ax2.set_xscale('log')\n",
                 "    ax2.set_yscale('log')\n",
                 "    ax2.loglog(log_interp_x, log_interp_y, color=\"red\",  linewidth=2.5, linestyle=\"-\", label=\"cubic spline\")\n",
-                "    ax2.loglog(coma.vmodel['column_density_grid'], coma.vmodel['column_densities'], 'bo', label=\"model\")\n",
-                "    ax2.loglog(coma.vmodel['column_density_grid'], coma.vmodel['column_densities'], 'g--', label=\"linear interpolation\")\n",
+                "    ax2.loglog(vmr.column_density_grid, vmr.column_density, 'bo', label=\"model\")\n",
+                "    ax2.loglog(vmr.column_density_grid, vmr.column_density, 'g--', label=\"linear interpolation\")\n",
                 "\n",
                 "    ax1.set_ylim(bottom=0)\n",
                 "\n",
-                "    ax2.set_xlim(right=coma.vmodel['max_grid_radius'])\n",
-                "\n",
                 "    # Mark the beginning of the collision sphere\n",
-                "    ax1.axvline(x=coma.vmodel['collision_sphere_radius'], color=solarblue)\n",
-                "    ax2.axvline(x=coma.vmodel['collision_sphere_radius'], color=solarblue)\n",
+                "    ax1.axvline(x=vmr.collision_sphere_radius, color=solarblue)\n",
+                "    ax2.axvline(x=vmr.collision_sphere_radius, color=solarblue)\n",
                 "\n",
                 "    # Only plot as far as the maximum radius of our grid on log-log plot\n",
-                "    ax2.axvline(x=coma.vmodel['max_grid_radius'])\n",
+                "    ax2.set_xlim(right=vmr.max_grid_radius)\n",
                 "\n",
                 "    # Mark the collision sphere\n",
-                "    plt.text(coma.vmodel['collision_sphere_radius']*1.1, lin_interp_y[0]/10, 'Collision Sphere Edge', color=solarblue)\n",
+                "    plt.text(vmr.collision_sphere_radius*1.1, lin_interp_y[0]/10, 'Collision Sphere Edge', color=solarblue)\n",
                 "\n",
                 "    legend = plt.legend(loc='upper right', frameon=False)\n",
                 "    for l_text in legend.get_texts():\n",
                 "        l_text.set_color(solarblack)\n",
                 "    plt.show()\n",
                 "\n",
                 "\n",
                 "# for graphing with astropy units\n",
                 "quantity_support()\n",
-                "show_column_density_plots(coma_sine, u.km, 1/u.cm**2, 'OH')"
+                "show_column_density_plots(vmr, u.km, 1/u.cm**2, 'OH')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "acceptable-reggae",
             "metadata": {},
             "source": [
                 "\n",
                 "\n",
                 "### 3D plot of the interpolated column density"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 23,
             "id": "nasty-reliance",
-            "metadata": {
-                "scrolled": false
-            },
+            "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/var/folders/1n/8mdnjzr95m3c_nwpkkxth8340000gn/T/ipykernel_34424/414349715.py:30: MatplotlibDeprecationWarning: The w_xaxis attribute was deprecated in Matplotlib 3.1 and will be removed in 3.8. Use xaxis instead.\n",
+                        "  ax.w_xaxis.set_pane_color(solargreen)\n",
+                        "/var/folders/1n/8mdnjzr95m3c_nwpkkxth8340000gn/T/ipykernel_34424/414349715.py:31: MatplotlibDeprecationWarning: The w_yaxis attribute was deprecated in Matplotlib 3.1 and will be removed in 3.8. Use yaxis instead.\n",
+                        "  ax.w_yaxis.set_pane_color(solarblue)\n",
+                        "/var/folders/1n/8mdnjzr95m3c_nwpkkxth8340000gn/T/ipykernel_34424/414349715.py:32: MatplotlibDeprecationWarning: The w_zaxis attribute was deprecated in Matplotlib 3.1 and will be removed in 3.8. Use zaxis instead.\n",
+                        "  ax.w_zaxis.set_pane_color(solarblack)\n"
+                    ]
+                },
+                {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAABEYAAAOdCAYAAACI5md3AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjMuNCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8QVMy6AAAACXBIWXMAAAsTAAALEwEAmpwYAAEAAElEQVR4nOzdd5wbxf3/8dfMSjqdC2CMsY0rxXQIEIzpEAg9BEIohgAGDCGFBBIS6o8AIaF9Cb33DqEFTMcG0wI4Bky1MbaxwRj3Xq5I2vn9oTtZd9Jp13C+1Z3ez8dD9t1qNPPZ2d3RztzsrgEcIiIiIiIiIiIVyEYdgIiIiIiIiIhIVDQwIiIiIiIiIiIVSwMjIiIiIiIiIlKxNDAiIiIiIiIiIhVLAyMiIiIiIiIiUrE0MCIiIiIiIiIiFUsDIyIieXbccUf+/e9/M2PGDOrq6pg3bx6vvPIKxx9/PNauWpN54YUX4tzqeyK6c44LL7xwlT83bNgwTjzxxFaPZ/To0YwePbrV823JPffcw9SpU9usvNVpwIABOOcYNmxYZDHsscceOOfYY489cstOP/10fvGLX0QSzyabbMKrr77K4sWLcc5xyCGHlEy//fbb88QTTzBr1ixqa2uZOnUqN910E+utt15B2tGjR/PWW28VzWf48OE45xgwYECrrIeIiIiUPw2MiIg0OP300/nvf//L2muvzdlnn81Pf/pTTjrpJL788ktuueUWfvazn0UdYqs44YQTOOmkk6IOQ8rMhx9+yI477siHH36YW3bGGWdw2GGHRRLP1VdfzQYbbMCRRx7JjjvuyBtvvNFi2mOPPZZ3332X7t27c/rpp7PPPvtw2WWXsd9++zFu3Di22mqrNoxcRERE2ptY1AGIiJSD3Xbbjauvvpobb7yR008/vcl7I0aM4Oqrr6Zz584RRSey+i1dupQxY8ZEHUbOZpttxptvvsnLL79cMt0mm2zCHXfcwdNPP82RRx6Zm6X11ltv8cQTTzBmzBieeOIJtthiC9LpdFuELiIiIu2MZoyIiABnn302CxYs4Kyzzir6/ldffcWnn34KwDrrrMOtt97KxIkTWb58Od988w0PPfRQ0Sn7zXmex1lnncXnn39OTU0Nc+bM4cUXX2STTTYBspe5FJvGH+aynA033JD777+fr776ihUrVjBlyhRuvvlm1lprrVya0aNHs+eee7LrrrvinMM51+Tyl4EDB/Lggw8yZ84camtrGTduHIceemhBWUcddRQTJkygtraWzz77rGialnTq1InLLruMyZMnU1tby8yZM3niiSdYd911c2kGDx7MyJEjWbp0KcuWLWPUqFEMHjy4ZL7FLgWB4nU6depUHnjgAY499li++OILVqxYwZtvvslGG21Ep06duPXWW5k3bx6zZs3iqquuwvO8gnIOPvhgbrjhBubOncvcuXN54IEHWHPNNQPXv7q6mptuuol58+axdOlSnnnmGfr27Vs07e67786oUaNYsmQJy5Yt46WXXmKLLbZokqbxspC9996bDz74gOXLl/Ppp58WbJNBgwbx1FNPMXv2bGpqavj666957LHHcuvWvP6mTp3KwIEDOfbYY3P7yj333MNhhx2Gc46tt966IN7Ro0fz7rvvllz/WCzGJZdcwtSpU6mrq2Pq1KlccsklxGKxJnGsv/76HH/88bmyW3L66afjeR5/+MMfCtItWLCA8847j4033jiymS8iIiJS/jRjREQqnrWWn/zkJzz99NPU1dUFpl977bWpra3l3HPPZe7cuay33nqceeaZ/Pe//2XTTTctmcejjz7KoYceyrXXXsuoUaNIJpPsvvvu9O7dm4kTJ/6g9VhvvfWYPn06Z5xxBgsXLmSDDTbgvPPO44UXXmDnnXcG4He/+x0PPvggnudx6qmnArBkyRIA+vbty5gxY5gzZw5/+tOfmDt3LkcddRRPPvkkhx56KM8++ywAe++9Nw8//DDPP/88Z555Jj169OC6664jHo8HrkM8HmfkyJH86Ec/4vLLL+e9995jzTXXZL/99qNbt27MmTOHrbbaijfeeIPx48dzwgkn4JzjnHPO4Y033mDHHXfkk08++UH11Gj33Xdnww035OyzzyaRSHDttdfy5JNP8tVXXzF58mSGDh3K7rvvzgUXXMCUKVO45ZZbmnz+uuuu47nnnuOYY45hk0024corrySTyXDCCSeULPe2227jqKOO4uKLL2bs2LHss88+PPzwwwXpDjzwQJ555hmef/55jj32WCA7gPfWW2+x9dZb8+233+bSbrjhhlx33XVcdtllzJs3jzPPPJPHH3+cTTfdlClTpgDw/PPPs3DhQn77298yb948+vTpw4EHHoi1lkwmU1D+L37xC1544QU+/vhjLrroIgDmzp3L119/zYwZMzj11FP5/e9/n0u/ySabsOeeewau/3333ceRRx7JpZdeyttvv83OO+/M+eefzwYbbMCvfvWr3CU9I0aMYOzYsVxyySUl89t77715//33mTVrVtH3n3/+eTKZDHvttRePPfZYk/fyB7wareq9hERERKRjcHrppZdelfxad911nXPOXXrppd/r89Za17dvX+ecc4ceemhu+YUXXuhc9k/YDnA/+clPnHPO/eEPf2gxr2HDhjnnnBswYECT5c3zApxzzl144YUt5uV5nttll12cc85ts802ueWjR492b731VkH6O++8082ZM8etvfbaTZa/8sorbty4cbnf3377bff55587Y0xu2ZAhQ5xzzo0ePbpkXZ144onOOecOPvjgFtM8/vjjbuHChW7NNdfMLevataubP3++e/LJJ3PL7rnnHjd16tTc73vssYdzzrk99tgjsE6nTp3q5s+f79ZYY43csj/84Q/OOefuuOOOJp//4IMP3GuvvVZQzr333tsk3Q033OBqampKrv/GG2/s0um0O/vss5ssv/nmm51zzg0bNiy3bNKkSW7UqFFN0nXt2tXNnTvXXXPNNU22Z319vdtoo41yy3r06OHS6bQ799xzHeC6d+8eWO/F6m/q1KnugQceKEh74YUXukWLFrlOnTrllv3rX/9yCxYscMlkssUytthii6L77fnnn++cc26rrbbKLZs+fbq75557Ao+/FStWuIcffrhkmpkzZ7rnn3++SZ0FaX4M6qWXXnrppZdeHfelP4uIiHwPv/nNb/joo49YunQpmUyG6dOnA+QuiSlm3333xfd97rjjjtUSUzwe59xzz2XChAmsWLGCdDrN22+/HRhXo/33358XXniBxYsX43le7vXyyy+zzTbb0LVrV6y1DB48mCeeeKLJZQtjxowJ9YSYfffdl5kzZ+ZmnxSz++6789xzz7F48eLcsqVLlzJixIiCy2R+iHfffTc3Wwbgiy++ACi4p8UXX3xBv379Cj7//PPPN/n9008/JZlM0rNnzxbLHDJkCJ7nFcxcePTRR5v8vtFGG7HRRhvx0EMPNdkWK1as4N1332X33Xdvkn7SpElMnjw59/vcuXOZM2cO/fv3B2D+/PlMmTKFyy+/nJNPPpmNNtqoxRjDuP322+nUqRNHH300AFVVVQwbNoz777+f2traFj/XGPeDDz7YZHnj7625fYN89NFHbL/99gWvoBkqIiIi0vFoYEREKt78+fNZsWJF6Mdznnbaadxyyy2MGjWKww47jMGDBzNkyBAAkslki5/r3r07CxYsKNlx/CEuu+wyLrroIh588EEOOuggBg8enHvUaqm4Gq277roMGzaMdDrd5HXVVVfl4l9nnXVIJBLMnj274PPFljXXvXt3ZsyYUTLN2muvzcyZMwuWz5o1i27dugWWEdbChQub/F5fX9/i8mL1t2DBgia/N15CVaque/fuDRTWVfPfG++3cvfddxdsj4MPPpju3buXjKUxnvxY9tlnH95//30uu+wyJk2axJQpU/jNb37TYqylzJw5k2eeeSb3+SOOOILu3btz2223lfzc2muvnft8vsbLYBrfXxXffvstAwcObPH9Tp060aNHj9zgZaNly5bxwQcfFLy+/vrrVY5BRERE2jfdY0REKl4mk+H1119nn332IZFI5DrILRk6dCijRo3iL3/5S25ZqY5Zo3nz5rH22muTTCZbHBxpXJ5IJJosb94Rbimu+++/n3/+85+5ZV26dAn8XKP58+fz1ltvccUVVxR9/7vvviOdTlNfX190VkTPnj0DO5Xz5s1jyy23LJlmwYIF9OrVq2B5r169CgYt8v2QumsrjQMCPXv2bDLDpnl9zp8/H4BzzjmHUaNGFeQTtI8WM3XqVIYNGwbAj370o9wA37Rp03jppZdWOb+bb76Z1157je22245TTz2VN998kwkTJpT8TOMATq9evfjqq69yyxu3d7EBniCvvvoqw4cPp1evXkXvM3LQQQfheR6vvfbaKuctIiIilUEzRkREgMsvv5zu3btz5ZVXFn1/4MCBbLXVVkD2L9CpVKrJ+yeeeGJgGa+88grWWk4++eQW0zQOLOQPHniex7777huYf9i46urqqK6uLlj+0ksvsfXWW/P5558X/Ut6fX09vu8zduxYDj/8cIwxuc/usMMOrL/++oExvvLKK/Tu3Zuf/exnLaZ54403OPDAA5sM6nTp0oWDDz6Y119/vcXPFas7yHaMy8WYMWPIZDIceeSRTZYPHTq0ye8TJ05k6tSpbLHFFkW3ReMTkr6vjz/+mD//+c9AYX3la2lfgewTaCZMmMDVV1/Nrrvuyq233hpY7ptvvgkUru+vfvUrgJLbtyXXXXcdvu9zww03NNknAbp168all17KpEmTeOqpp1Y5bxEREakMmjEiIgK89dZb/PnPf+bqq69m880359577+Wbb76hW7du7L333px88skcc8wxfPrpp7z00kucffbZnHvuufzvf/9jr7324vDDDw8s4/XXX+eJJ57g6quvpl+/frz22mvE43F23313nn/+ed544w3Gjh3L5MmT+b//+z+stdTV1fG73/2OqqqqwPxfeuklhg0bxqeffsrkyZM57LDDck+jyTd+/Hh+97vfceSRRzJlyhSWLl3Kl19+yd/+9jf+97//8eabb3LjjTcybdo0unXrxpZbbskGG2zA8OHDgeyjg1955RWefvppbrvtNnr06MHFF19c9PKX5h588EFOOeUUHnnkES677DLGjBlD165d2W+//bj22muZOHEil1xyCT/72c949dVXueKKK3DOcfbZZ9OpUyf+/ve/t5j3rFmzeP311zn33HOZN28ec+bM4dhjj2WDDTYIjKutfPnllzz88MP8/e9/x1rL2LFj2XfffTnwwAML0v7+97/nmWeeIZFI8NhjjzFv3jx69uzJzjvvzDfffMM111wTutytttqK6667jn//+99MnjwZz/M44YQTSKVSJWdSjB8/nt12242DDjqIWbNmMW/evCazgm655Rauv/565s6dy5NPPhkYx+eff87DDz/MRRddRCwW45133mGnnXbiggsu4OGHH+azzz4LvU6NvvjiC0499VTuvPNOXn31VW699VZmzpzJpptuyllnncVaa63FPvvsQzqdXuW8RUREpHJEfgdYvfTSS69yee20007usccec999952rr6938+fPdy+//LL71a9+lXsKSzKZdDfffLObM2eOW7JkiXv22WfdwIEDC562UexJMp7nufPOO89NnDjR1dXVuTlz5rjnn3/ebbzxxrk0m2++uRs9erRbunSp+/rrr92f/vSnUE+l6d69u3vkkUfcggUL3IIFC9yDDz7ott9++4KnnfTs2dM9//zzbsmSJQVPkunTp4+744473Lfffuvq6urcd99951555RX3q1/9qknZQ4cOdV988YWrra11n332mTv00EPd6NGjA59KA7jOnTu7K6+80k2bNi1XxuOPP+569OiRS7PDDju4kSNHuqVLl7ply5a5UaNGucGDBzfJp/lTaRrjHzFihFu4cKGbOXOm++c//+mGDx9e9Kk0zZ+20vhUlr333rugnOnTpwema+mJQs1f1dXV7uabb3bz5893S5cudc8884zbeeedC7YT4HbccUf37LPPugULFriamho3depU98gjj7gdd9wxl6alpwxNnTo191SXHj16uHvvvddNnDjRLV++3M2fP9+9/vrrbt999y1Yr/yn0myyySbuzTffdMuXL3fOuYKnxPTq1cs559yVV14Z+hiLx+PukksucdOmTXP19fVu2rRp7pJLLnGxWKxJurBPpWl8DRkyxD311FNuzpw5rq6uzk2bNs3dcsstrm/fvgVpW6ozoOj+opdeeumll156deyXafhBREREZJWcfPLJ3HbbbWy88cZMmTIl6nBEREREvhddSiMiIiKrZLPNNmPDDTfk4osv5umnn9agiIiIiLRrmjEiIiIiq2T06NHsvPPOvPPOOxxzzDGh7i8jIiIiUq40MCIiIiIiIiIiFUuP6xURERERERGRiqWBERERERERERGpWBoYEREREREREZGKpYEREREREREREalYGhgRERERERERkYqlgRERERERERERqVgaGBERERERERGRiqWBERERERERERGpWBoYEREREREREZGKpYEREREREREREalYGhgRERERERERkYqlgRERERERERERqVgaGBERERERERGRiqWBERERERERERGpWBoYEREREREREZGKpYEREREREREREalYGhgRERERERERkYqlgRERERERERERqVgaGBERERERERGRiqWBERERERERERGpWBoYEREREREREZGKpYEREREREREREalYGhgRERERERERkYqlgRERERERERERqVgaGBERERERERGRiqWBERERERERERGpWBoYEREREREREZGKpYEREREREREREalYGhgRERERERERkYqlgRERERERERERqVgaGBERERERERGRiqWBERERERERERGpWBoYEREREREREZGKpYEREREREREREalYGhgRERERERERkYqlgRERERERERERqVgaGBERERERERGRiqWBERERERERERGpWBoYEREREREREZGKpYEREREREREREalYGhgRERERERERkYqlgRERERERERERqVgaGBERERERERGRiqWBERERERERERGpWBoYEREREREREZGKpYEREREREREREalYGhgRERERERERkYqlgRERERERERERqVgaGBERERERERGRiqWBERERERERERGpWBoYEREREREREZGKpYEREREREREREalYGhgRERERERERkYqlgRERERERERERqVgaGBERERERERGRiqWBERERERERERGpWBoYEREREREREZGKpYEREREREREREalYGhgRERERERERkYqlgRERERERERERqVgaGBERERERERGRiqWBERERERERERGpWBoYEREREREREZGKpYEREREREREREalYsagDkJXWXnttunbtyvLly1m4cCGZTAZrLb7vRx2aiIiIiIiISIekgZEyUF1dzTHHHMPf/vY30uk033zzDYsXL+bYY49l2bJlGGNwzkUdpoiIiIiIiEiHo0tpIlZdXc15553Htddey6233spRRx3FGWecwYIFC3j//ffp0qWLBkVEREREREREVhMDqNcdoRNOOIEbb7yRU045hUceeaTJe9dddx09evTguOOOI5PJRBShiIiIiIiISMelGSMR6tatG3/729+4/PLLc4Mixhg8zwPgxhtvZO7cuXTt2jXKMEVEREREREQ6LA2MRKhz5874vs9rr70GkLuXSOPskOnTpzNu3DgWLVoUYZQiIiIiIiIiHZcGRiK0fPlypk6dSm1tLQDWrtwcsViM2tpa7r333oiiExEREREREen4NDASoYULF7JgwQLOOussgNxMkXg8TjqdBmDjjTdm0003ZZ111gGaDp6IiIiIiIiIyA+jm69GLBaL8cEHHzB27FiuvPJK5syZk7t05sknn6R37954nkd1dTXHHnssn3zySbQBi4iIiIiIiHQgmn4QIc/zSKfTbLfddlhr+c1vfsOBBx4IwJtvvkmPHj04/fTT2W+//bj22mu577776N69e5M8kslkFKGLiIiIiIiIdBhOr+he1trcz2ussYYD3DHHHOPefPNN16tXr9x7PXv2dO+9957bcMMNc8sGDBjgnnzySffTn/408vXQSy+99NJLL7300ksvvfTSS6/2+NKMkYj5vp/7ecmSJQD06dOHmTNnMmfOnNx7G2ywAb7v5+490r9/f/7xj3+w2Wab8fHHH7dt0CIiIiIiIiIdhAZGypBzjlgshu/7xGIx+vTpw80338zkyZP5+uuv6dOnD5dffjmbb745u+22G3PnzsXzvKjDFhEREREREWl3dPPVMuR5HuPGjWPKlCn4vk/fvn2ZP38+Bx54IN26deO2225jo4024oADDmD27NlA9mk1+bNPRERERERERCSYBkbKTOMAh+d5nHbaaWQyGebPn88jjzzCmmuuyZ133smGG26YGxT5+c9/zoQJE5g0aVLUoYuIiIiIiIi0OxoYKUPFZn+su+663HjjjU1mivzyl7/kscce49RTT+XOO++MKFoRERERERGR9isWdQBSqPmgSM+ePbn//vtZe+21c4MiRxxxBI8++ih/+MMfCgZFjDE4p/EuERERERERkSC6+Wo7MGfOHL799lsOPvhgZs+ezSGHHMJDDz3EGWecwc0335xLd+ihh9K7d28NioiIiIiIiIiEpEtpylzz2R99+/blhRde4OGHH+byyy/PLT/iiCP4zW9+w+uvv86ll15KJpOJIlwRERERERGRdkUzRspc89kfmUyGxYsXM2LEiNyyo446iqOPPpp3332Xhx56iEwmQ6dOnYDswIqIiIiIiIiIFKeBkXZm1qxZdOrUidNPP52ePXvypz/9iV/96ldMnDiRO+64g6+++orDDz+cl19+mZ49e+Kcw1ptZhEREREREZFi1GNuRxovqxkyZAjLly/n3//+NxdeeCGff/45t9xyC19//TWHHnoo119/Pf369eOYY45hs802w/d9zRwRERERERERKUIDI+1I4+yPdDrNmWeeyUsvvcRDDz3EtddeyzfffMMhhxzCddddx8MPP8wvfvELamtrGTduHH369NENWUVERERERESK0M1X26H8G7L27t2bmTNn8vOf/5yrr76aBx98kIsuuiiX9pVXXuHvf/87b7/9NgDW2oLHAYuIiIiIiIhUqljUAciqy5/9MXPmTHbddVcefvhhrrzySv7+97/n3jvhhBPYe++9+fbbb9lzzz35z3/+w+eff17wpBsRERERERGRSqUZIx2AtZYTTjiBu+++O7fs2GOP5d577+Xss8/mvffeY+utt+Yf//gHW265JTNnzowwWhEREREREZHyoYGRdq7YpTHHHHMM9913H7/+9a+55557css/+OAD/vrXv/Laa6+1dZgiIiIiIiIiZUk3X23nmg+K7LvvvjzwwAOccsopTQZFLrroIrp37864ceMAiMfjAHpajYiIiIiIiFQ0DYx0MK+++io///nPuffee3PLzj33XH7yk5/w5z//mYULF7L55ptzzjnn0KNHD5xzGhwRERERERGRiqWbr3YgnueRyWR4/vnnc8vOPvtsDjjgAO644w6efvppBg4cyMknn8xxxx1Ht27dco/61dNqREREREREpBJpxkgHkslkmvx+7LHHcsIJJ3Dbbbfx0EMPMWDAAH7/+9+zww478PjjjzNlyhTGjBnD5ptvrkERERERERERqUi6+WoHZq1ln332YeTIkfTv35/f/e53bLTRRtxzzz08++yzADz00EPMnTuXM844I9pgRURERERERCKgS2k6qMZLY15++WV69erFeeedR/fu3bn33ntzgyLGGKy1rFixIuJoRURERERERKKhgZEOKv/SmFmzZjF//nxGjRrFiBEjcsvPPvtsDjroIPbcc88IIhQRERERERGJni6l6eCMMThXuInPPfdcLr74Yvbdd19ef/31FtOJiIiIiIiIdGSaMdLBFRvsuOyyyzj99NPZb7/9NCgiIiIiIiIiFU1PpalAO+20E4cddhijR49ucVAkkUgQi8VyP3fq1KmtwxQRERERERFZ7XQpTQUrNigyePBgjjnmGH784x+zdOlSLrjgAmbOnMndd99NTU0N1157LW+++WZEEYuIiIiIiIi0Ls0YqWDNB0UOPPBAzjjjDDbddFOuvfZa3nvvPe655x48zyOdTvPzn/+cwYMHY612GxEREREREekYNGNEcu69914ymQxnn3028+bNA+Caa65h/fXX58c//jHTpk1j//33Z/ny5RFHKiIiIiIiItI6NDAiAOyyyy688sorbL311kyZMiW3fNKkSay99tpMmDCB/fbbj+XLl2OtbfI4YBEREREREZH2StdECAA1NTW89957TJkyhbXWWguAm2++mZ49ezJ+/Hj22Wef3EwR3/cxxkQYrYiIiIiIiEjr0IwRAcBay/jx43nzzTfZYYcdMMbQu3dvJk6cyG677caGG27IiSeeyNKlS5k3bx533XWXZo6IiIiIiIhIu6cZI5Ib4Nhiiy2YOHEi66yzDptvvjmpVIrddtuNX/3qV4wcOZKzzjqL/fffnxtvvJFLL71UgyIiIiIiIiLS7mnGiAArB0eMMVx00UWkUimOP/54/vWvf3HZZZfRuXNn3nvvPZ588knWWGMN/vKXvzBkyBAmTpwIQKdOnVixYkXEayEiIiIiIiKyajQwIjnGmNwjfDt16kS3bt04++yz2XrrrampqWHddddl7ty5TJ48mYMPPpidd96ZGTNmsMEGG3DyySfz9ttv88ILL0S8FiIiIiIiIiLh6VIayWkcFAFYsWIFM2bMoHPnzjjnGDVqFBMnTiSRSLDPPvvQuXNnFi9eDMDMmTOpra3l2WefZbPNNosqfBEREREREZFVpoERKWnWrFksXryY4447jpEjR/LNN9+w0UYbcdRRR7Fs2TL23Xdfvv76a3r06MHVV19NJpOJOmQRERERERGR0HQpjZQUi8V4//33mTZtGsuXL+f6668nlUrx4Ycf8tOf/pRnnnkG3/d5++23ueWWWxgxYkSTS3JEREREREREyplmjEiLrLWk02m23357MpkMs2bN4uOPP2bChAnsvffevPjii0yaNIlnn32WDz74gPvuu4+BAwcCsOOOO7LnnntGGr+IiIiIiIhIGE4vvVp6WWsd4IwxrmvXrs7zPPf000+7dDrtXn/9dXfRRRe5rbbaygHu7bffdieeeKID3O677+6++OILt//++0e+DnrppZdeeumll1566aWXXnrp1dIrhkgJvu8D4Jxj6dKlDBkyhIMPPpjly5dTV1fHddddx8KFCznqqKPo06cPn376KdZa3nzzTYYNG8Ydd9zBpEmTmDJlSsRrIiIiIiIiIlJIAyOySt5//32OP/54xo0bx5tvvsk+++xDfX09hx9+OA888ACffvop//rXv3jooYeYOnUqM2bMoFu3blGHLSIiIiIiIlKUbr4qoXme1+SpM5tuuil77LEH+++/P9OmTePGG2/EOcfIkSNZb7318H2fzz77jJ122il3M1bdlFVERERERETKiW6+KqE1fxRvjx49OProo4nH48ycOZMpU6bQt29fPvnkE1599VVuuOEG+vfvz4YbbohzLjcosuWWW0YRvoiIiIiIiEgBDYzI9/b222/zxBNPcNVVVzFs2DCGDh0KwHbbbcfChQs555xzuPvuuzn44IMBiMfjrLfeerz++uv069cvytBFREREREREAF1KI9+TMSY3A2TNNdfk2muvZZtttmHOnDlsuummzJ07l+23357evXszc+ZMALp37878+fNz/4uIiIiIiIhETTNG5HvJv1fIkiVL6NGjB1999RWnnXYa2223HQsWLGDAgAG5QZGLLrqITz/9lC5dujB//nzWW2894vF4VOGLiIiIiIiIAJoxIj9Q48yRWCzGhx9+yEcffUSfPn3YZJNN2GyzzVi6dClnnnkmf//73zn++ON577336NWrF7/97W+ZO3cu559/fu6RwCIiIiIiIiJtTTNG5AdxzuF5Hul0mh//+Mfstdde9O/fn5/85CcsXbqUv/71r1x22WUMGzaMI444grFjxzJmzBjWX399Xn31VQ2KiIiIiIiISKQ0MCI/WCaTwVrLaaedxhtvvMEXX3zBpEmT+POf/8w//vEPjjzySHr06EE6nebhhx9m+vTp7LbbbsyYMQMAa7UbioiIiIiISDTUI5VW0bt3bw466CDuvPNOAI455hj+7//+jyOPPJKnn36ao446is6dO9O7d2+GDRtGXV0dN998M+uttx6+72OMiXgNREREREREpBJpYERaxbXXXstZZ52VuzTm3//+N3vssQfPPPMMvXv3ZquttsL3fZ588knefPNNZs+ezT//+U+OO+441l133SY3cxURERERERFpK7GoA5D276CDDmLOnDl8+OGH7LHHHniexzvvvENVVRWxWIxx48YRj8d57rnneOqppwDo2rUrjz32GF27dmX48OFcccUV3HXXXRGviYiIiIiIiFQaDYzID7bLLrvw85//nAMPPJBkMskaa6zBiBEjOProo4nFYkyaNAlrLRMmTAAgFovRqVMnvvvuO2699VbOO++8iNdAREREREREKpUupZEf7LzzzqNfv36sv/76DB06lNdee42jjz4agHg8zoIFC1i2bBk33ngjAL/85S+ZPHkysViMZ599NpfPNttsQ/fu3SNZBxEREREREalMmjEiq4W1lhkzZrDmmmuycOFCZs+ezaabbsr8+fOZPHkyvu/Tu3dvbr31VmbOnMnAgQNZf/31WbhwIXvssQcTJ06MehVERERERESkAmjGiLSqN954g4MPPjg38NG7d28mT57MMcccw1prrcWkSZO45pprWLp0KQcffDBjxoxh8803Z+DAgey5555ccsklXHzxxVGvhoiIiIiIiFQIDYzIarV48WJGjRrFoYceSjweJx6Ps8MOOzBkyBBuuukm1llnHWbMmEE6nebdd9/l1ltvZe+99446bBEREREREakQBtBzUqVVrbPOOqRSKRYvXkwymWTUqFHssMMOGGOoqamhc+fOLFy4kEceeYQ//OEPTJs2jfnz57P99tuz++678+qrrzJ+/HgymQxPPfUUl1xySdSrJCIiIiIiIh2U7jEira53797c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1heg227DWPT2fbhm+2RHley7FXXffYGfros6FFlNar/5iGT/baIOo80sfuch1tju5xUxKAKw5H+PkaldSrfdT4o6lDaxbMLrzB95PX2G31VWgyIiItL2Ov6fqaXiFLsh60knncRJJ2VP9Pp0S+Nn6vjko4msA+zZCb4aD+u9czvPR3RZzeIx/46k3KhU2g06K206+uRzK+fJHY0q6VKaZZ+8xKxHzow6jDa16L8PRB1Cm5p0zqZRh9Cmpl2xd9QhAODFLYfdGHUUIiKVSQMj0uEUuyFro2uuuYbhw4fz85//nP+78WYGH3UCAO88eCdb7fFTeOdjAHbYags233B9/v3SSGpq6wouz2lVkz+FvhtCstPqyb/caH07tkpbX4DP/wdb7BB1FG1j0ifQfxBUVUcdSdvQ+nZskz6G/huXzfpmPv9f1CGIiFQsXUojFWXrrbfmiCOO4PXXX88tu+7cP7Nk+XKuuvchAGIxj4F9erPH9tvy7kN30bVz59U3KCIiIiIiIiKR0sCIVJS9996bl19+Off79eeeycYD+nPDw4/x3dy5AKTTGR57aRQn/r9LeOP9D3nptmtJxONRhSwiIiIiIiKrkQZGpGKt32c9NuzXlxsfeZxR744lnc7k3ovHsleZnX31TTjn2LBf36jCFBERERERkdVIAyNSkYwxpDMZ7nzqGV757xjq6uubvJ9KpwE4cLedscZSW6+nbIiIiIiIiNx1113Mnj2bTz/9NDDtbrvtxgcffEAqleKXv/xlbnn//v354IMPGDduHJ999hmnnhrtc8p181WpOMYYnHNMnzWb/4x6nV22/RF9evagrr6eDfr2IZ3J4Ps+++48BIDPJk9h1rz5EUctIiIiIiISvXvvvZcbb7yR+++/PzDtN998wwknnMBf/vKXJstnzpzJTjvtRH19PZ07d+azzz5jxIgRzJw5c3WFXZIGRqTiOOea/H7WScfysz125Zr7H6F/714ATPtuJlOmz+CVd8bw33GfUFOrGSMiIiIiIiJvvfUWAwYMaLJsgw024KabbqJHjx6sWLGCU045hYkTJ/L1118DFDzMIpVK5X6uqqrC2mgvZtHAiFS8w844h3cevINO1UmOPPO8qMMRERERERFpV26//XZ+85vfMHnyZHbYYQduvvlm9t5775Kf6du3L88//zwbbbQRf/3rXyObLQK6x4hU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vPdKbdwRT5Ue3El7PqaF9q5JXlWQqAvutdZ5jlhA/adjDi8dIq+qDLHavPqwXYretyZjwQZcr55OGEyo+yYZvLrS9ZGNKLjO0kkPG3S/EoAYxdv4vPbZj3uY+hDfPUmLDZHOx2EC7jHie4lQ3z3OWkw6oEzPQlAaPIzThByRiqB7jHQYffv25f7776dnz54457j99tu5/vrrC9Jdd911HHjggaxYsYITTjiBcePGlcxXAyMSmX322SdUujvuuIPnnnsOgBkzZtCvX7/ce3379mXGjOzNS4stnz9/PmuttRae55HJZJqkr0+n6ddrXWbMnoPneazZpUubzxaRiLX378j2Hr+sVuF2jxLTYdoLHQcrhd2UYW98HCqv1stKREQkSDqd5swzz2TcuHF06dKFDz74gJEjRzJhwoRcmgMOOIBBgwYxaNAghgwZwi233MKOO+5YMt9oLuARCZA/k+QXv/gFn332GQAjRoxg6NChJBIJBg4cyKBBg/jf//7H2LFjGTRoEAMHDiQejzN06FBGjBgBwOjRozn88MMBGDZsGM888wwAi5YuY9ghBwFw+L578dqY99tyFSOks9hKU75bvHw75K0fWXmua2vvG6HWsjyrIjqqDxERkdBmzZqVm/2xbNkyJkyYkLtVQqNDDjmE+++/H4AxY8aw1lprFb1SIZ9mjEhZuvLKK9lmm21wzjFt2jROPfVUAMaPH89jjz3G+PHjSafT/P73v8dveIThaaedxssvv4znedx9992MHz8egLPPPptHH32Uf/zjH4wbN4677roLgHkLF9F9zTWZ9MITLFi8hKF//X/RrKy0vvIdCQjdCQq6jCYyZRrWqijfVYggsgg65eVb/9JE0KN1RUTaEacbCnVIAwYMYNttt2XMmDFNlvfp06fg/pN9+vRh1qxZLealgREpS8cff3yL71166aVceumlBctffPHF3GN9802dOpUhQ4YULHfOceSZ5/2wQNuh5jfAlBBas39QKZWvPlXktAlWimRmTFitGVzIvCpi36iIlRQR6ZjWWWcdxo4dm/v99ttv54477miSpnPnzjz55JOcccYZLF269AeXqYERkShF8tfaViw0ghP6stXe449A+D1RPZzolfEOHsXuEaY6WrmpbfvVbO1tHmYtdKyLyGrQ+LheaTfmzZvH4MGDW3w/Fovx5JNP8tBDD/Gf//yn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u/zUU0/Viy++qKamJt15551OZQyVCRMmaO3atdnXnj179LWvfU033HCDtm3bll2ee13n9ddfr6amJm3cuFHnnntudvl5552njRs3qqmpSXPmzMkuHzdunFatWqWmpiYtXrxY8XhlvxrbsmWLXnzxRa1duzZ7Q6ih6O9KGDNmjJ566in9z//8j9avX69rr71Wkuq6fw9UqXbVmttvv10bNmzQunXr9Mtf/lKHH364JGns2LHav39/tq/nzZuX/ZuDGZtK7Q9DbSi24UQiocWLF6upqUmrVq3S2LFjh66BORYvXpxt55YtW7R27VpJ9dW3F198sdavX690Oq3TTjst73dD0Z+lyhhsXFYDAAPP8uLF6+BeZ5xxhp00aZJ96aWXsstuu+02O2fOHCvJzpkzx956661Wkp02bZp97LHHrCQ7ZcoUu2rVKivJjhgxwm7evNmOGDHCNjY22s2bN9vGxkYrya5evdpOmTLFSrKPPfaYPf/888uWUamX53n2zTfftMcdd5y94YYb7HXXXVeQZuLEifaFF16wiUTCjhs3zjY3N1vP86zneba5udkef/zxNh6P2xdeeMFOnDjRSrJLliyxl1xyiZVk582bZ6+++uqKtnPLli125MiRecuGor8r8Ro1apSdNGmSlWQPPfRQ+8orr9iJEyfWdf8e6DZfql219po6dar1fd9Ksrfeemt2Gx47dmze2Jb7OtCxqdT+UInXUGzDX/rSl+y8efOsJHvJJZfYxYsXV7yff/CDH9i/+7u/q7u+/cAHPmAnTJhgn376aXvaaacNaX+WKmMo299wiOxHzpS98S7Zm/85s+zmfy79fs5tld0OefHixataX8wYAd6F3/72t9q5M//rmhkzZuj++++XJN1///266KKLsssXLVokSVq9erUaGxs1atQonXfeeVq5cqV27dql3bt3a+XKlTr//PM1atQoHXbYYVq9erUkadGiRXl5FSujUs4++2xt3rxZr7/+esk0M2bM0OLFi9XZ2anXXntNzc3Nmjx5siZPnqzm5mZt2bJFXV1dWrx4sWbMmCFJOuuss/TQQw9Jqo52FjMU/V0Jra2t2W+X9+3bpw0bNhQ8Iz5XvfZvKeXaVWtWrlypdDotSVq1apXGjBlTNv3BjE2l9odqMpDbcO56eOihh3T22WdXpE25Pve5z+nnP/952TS12LcbN27U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MAIAAAAAACKLwAgAAAAAAIgsAiMAAAAAACCyCIwAAAAAAIDIIjACAAAAAAAii8AIAAAAAACILAIjAAAAAAAgsgiMAAAAAACAyCIwAgAAAAAAIovACAAAAAAAiCwCIwAAAAAAILIIjAAAAAAAgMgiMAIAAAAAACKLwAgAAAAAAIgsAiMAAAAAACCyCIwAAAAAAIDIIjACAAAAAAAii8AIAAAAAACILAIjAAAAAAAgsgiMAAAAAACAyCIwAgAAAAAAIovACAAAAAAAiCwCIwAAAAAAILIIjAAAAAAAgMgiMAIAAAAAACKLwAgAAAAAAIgsAiMAAAAAACCyCIwAAAAAAIDIIjACAAAAAAAii8AIAAAAAACILAIjAAAAAAAgsgiMAAAAAACAyCIwAgAAAAAAIovACAAAAAAAiCwCIwAAAAAAILIIjAAAAAAAgMgiMAIAAAAAACKLwAgAAAAAAIgsAiMAAAAAACCyCIwAAAAAAIDIIjACAAAAAAAii8AIAAAAAACILAIjAAAAAAAgsgiMAAAAAACAyCIwAgAAAAAAIovACAAAAAAAiCwCIwAAAAAAILIIjAAAAAAAgMgiMAIAAAAAACKLwAgAAAAAAIgsAiMAAAAAACCyCIwAAAAAAIDIIjACAAAAAAAii8AIAAAAAACILAIjAAAAAAAgsgiMAAAAAACAyCIwAgAAAAAAIovACAAAAAAAiCwCIwAAAAAAILIIjAAAAAAAgMgiMAIAAAAAACKLwAgAAAAAAIgsAiMAAAAAACCyCIwAAAAAAIDIIjACAAAAAAAii8AIAAAAAACILAIjAAAAAAAgsgiMAAAAAACAyCIwAgAAAAAAIovACAAAAAAAiCwCIwAAAAAAILIIjAAAAAAAgMgiMAIAAAAAACKLwAgAAAAAAIgsAiMAAAAAACCyCIwAAAAAAIDIIjACAAAAAAAii8AIAAAAAACILAIjAAAAAAAgsgiMAAAAAACAyCIwAgAAAAAAIovACAAAAAAAiCwCIwAAAAAAILIIjAAAAAAAgMgiMAIAAAAAACKLwAgAAAAAAIgsAiMAAAAAACCyCIwAAAAAAIDIIjACAAAAAAAii8AIAAAAAACILAIjAAAAAAAgsgiMAAAAAACAyCIwAgAAAAAAIovACAAAAAAAiCwCIwAAAAAAILIIjAAAAAAAgMgiMAIAAAAAACKLwAgAAAAAAIgsAiMAAAAAACCyCIwAAAAAAIDI+r81Mbs41mzhowAAAABJRU5ErkJggg==\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAABIMAAAPQCAYAAACltrsgAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOzdeZhTRdo28LvqZGsQQUUEkUXHBUUFBQUUwUEBRx0XdNxfkcHd0XEb5XMZmFdF5lVQEbdxAZdRB0dQHFHEEREFQRBcAFERZG32penurOf5/kgnZE8F0qST3L/rOkqfVOpU1alTST05iwIgICIiIiIiIiKisqALXQAiIiIiIiIiItpzGAwiIiIiIiIiIiojDAYREREREREREZURBoOIiIiIiIiIiMoIg0FERERERERERGWEwSAiIiIiIiIiojLCYBARERERERERURlhMIiIiIiIiIiIqIwwGEREREREREREVEYYDCIiAjBt2jSICHr37l2Q7ffu3RsigmnTphVk+/kkIhCRQhcjpWXLlkFE0K5du0IXpcEpxrYZOnQoRARDhw4tdFF2y7777ot//OMfWLVqFYLBYEnUiYiIiBo2BoOIqEE76aST8Nxzz2Hx4sXYunUrvF4vVq1ahffeew+DBw9Go0aNCl3EBqlTp04YOnQozj333EIXhWiPa9euHYYOHYqBAwcWuihG3n33XVxzzTVo3Lgx5s6di88//xwrVqzIKY9jjz0WTz31FH744Qds374dVVVVWLJkCZ5++ml06tQp7fvatWsXDeBmCwRG0hUqaE5ERET5JVy4cOHS0JaKigp58803JaKmpka+++47mTNnjqxevTq6fvXq1XL00Ufv9vamTZsmIiK9e/cuSH179+4tIiLTpk3LS34DBw4UEZGxY8fu8bpEFLoPpVqWLVsmIiLt2rUreFka2lKMbXPTTTfJ4sWL5aabbopbn+/jqT6XY445RkREVq5cKXvvvfcu5fHwww9LMBgUEZGqqir5+uuv5ZtvvpGamhoREQkGg/L3v/895XvbtWsXPWaz7fuIQo2TXLhw4cKFC5f8LTwziIgaHIfDgY8++ggXX3wx1q5diyuvvBL77rsvjjnmGJx44olo3bo1jjrqKDz77LPYf//98Zvf/KbQRSaiAnjqqadw5JFH4qmnnip0UXZZhw4dAABffPEFtm/fnvP7n3ji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woVLdJkwYYKIiIwcOTLveXs8HvF6vbJkyZKk19JN9r///nsREbnvvvuMtlEfwaBMyyuvvCIiknQGT7YJptPplDVr1kggEJDOnTunTPPWW2+JiMgVV1wRXffHP/5RRMJPPooNjEWWd955JzphNK1Dq1atokGknj17Gr3n119/FRGRP//5z0mvHXjggdEzhH7729/GvVZfwaB58+Ylveewww6LtsXEiROTXu/Xr5+IiCxYsCBufezk/Lbbbkt639lnn53yfZmWPn36iEj4TLJUZxQ9/vjjKQMCzZs3l9raWtm6dau0bt066X1KKZk9e3bSvou9BCo28BBZ/vSnP4mIyDvvvBO3vra2VjZt2mRcr10NBgGQl19+OW0firTH//3f/xmX5dVXX027rwHId999JyIif/vb3+LW72ow6JZbbknb99ItkbOUbr755pT9zRSDQVy4cOHChUvxL3yaGBE1KE2aNAEAVFdX73IeSimcc845GDNmDCZPnozPPvsMM2bMwNSpUyEiOPzww6M3bc3kN7/5DTp27Aifz1fwp/AcccQRGDZsGN5++21MmzYNM2bMwIwZM9C7d28AQKdOnXLKr0ePHmjVqhW+/vprLFiwIGWaSZMmAUB0G0D4hrUA8OKLLyIYDCa95+mnn86pHABw5plnwuVyYdasWfj888+zpj/yyCPRtm1b1NbW4vnnn096fc2aNXj77bcBAP369cu5PLti7NixSet++umnaD9+8cUXk16fP38+AOCQQw5Jm2+q93311VdZ35cost/eeustbNq0Ken1dPvtzDPPhMfjwZQpU7B69eqk10UE//nPfwDE95OIzZs3Y+LEicZ1WLlyJZo1a4bTTz89S41230svvQQAGDhwYNx6h8OBSy+9FAAwbtw44/wife3JJ59M+fro0aPj0u2uXRkrI2kj70301Vdf4fPPP0+7EBERUeng08SIqEGpqqoCADRu3HiX3t+0aVNMnjwZJ510UsZ0++yzT9an9xx55JEAgEWLFmHHjh27VJ58GDJkCB588EFYlpU2zb777ptTnscccwwAoH379pgxY0bKNM2aNQMAtG7dOrru8MMPBxB+mlsq6dZnEmnnL7/80ih9pAwrVqxATU1NyjQLFy6MS1vfli5dmnL9xo0b0bhx45Svb9iwAUD6ifmGDRtSPmp8/fr1Gd+XSrb99tNPPyEQ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kJqaGvnmm2/kpptuMirr7373O5kwYYKsWbNGfD6fVFZWyldffSWjR4+WXr16xZ3NsyvBIK21XH755fLyyy/LokWLZMuWLVJdXS0//PCDvPLKK3Lssccm5ZOp/7do0UJeeuklWblyZfTMmHRt2rlz52ibHnXUUbvUdyPLSSedJBMmTJB169aJz+eTVatWySuvvCJHHnlkyvT5CAZFjslnnnlGlixZIjt27JAdO3bIjz/+KM8995wcd9xxad/HYBAXLly4cOFSnouq+wcRERFRWerfvz8+/PBDfPXVVzjxxBMLXRwiIiKiescbSBMREVFZGzx4MABg7NixBS4JERER0Z7BM4OIiIiobJ144on44osvUF1djbZt22L79u2FLhIRERFRvUt+LjARERFRiXvjjTfQvn17HH/88XA4HBgxYgQDQURERFQ2eGYQERERlZ1ly5ahbdu2WLVqFV544QU8+OCDCN+Tm4iIiKj0MRhERERERERERFRGeANpIiIiIiIiIqIywmAQEREREREREVEZYTCIiIiIiIiIiKiMMBhERERERERERFRGGAwiIiIiIiIiIiojDAYREREREREREZURBoOIiIiIiIiIiMoIg0FERERERERERGWEwSAiIiIiIiIiojLCYBARERERERERURlhMIiIiIiIiIiIqIwwGEREREREREREVEYYDCIiIiIiIiIiKiMMBhERERERERERlREGg4iIiIiIiIiIygiDQUREREREREREZYTBICIiIiIiIiKiMsJgEBERERERERFRGWEwiIiIiIiIiIiojDAYRERERERERERURhgMIiIiIiIiIiIqIwwGERERERERERGVEQaDiIiIiIiIiIjKCINBRERERERERERlhMEgIiIiIiIiIqIywmAQEREREREREVEZYTCIiIiIiIiIiKiMMBhERERERERERFRGGAwiIiIiIiIiIiojDAYREREREREREZURBoOIiIiIiIiIiMoIg0FERERERERERGWEwSAiIiIiIiIiojLCYBARERERERERURlhMIiIiIiIiIiIqIwwGEREREREREREVEYYDCIiIiIiIiIiKiMMBhERERERERERlREGg4iIiIiIiIiIygiDQUREREREREREZYTBICIiIiIiIiKiMsJgEBERERERERFRGWEwiIiIiIiIiIiojDAYRERERERERERURhgMIiIiIiIiIiIqIwwGERERERERERGVEQaDiIiIiIiIiIjKCINBRERERERERERlhMEgIiIiIiIiIqIywmAQEREREREREVEZYTCIiIiIiIiIiKiMMBhERERERERERFRGGAwiIiIiIiIiIiojDAYREREREREREZURBoOIiIiIiIiIiMoIg0FERERERERERGWEwSAiIiIiIiIiojLCYBARERERERERURlhMIiIiIiIiIiIqIwwGEREREREREREVEYYDCIiIiIiIiIiKiMMBhERERERERERlREGg4iIiIiIiIiIygiDQUREREREREREZYTBICIiIiIiIiKiMsJgEBERERERERFRGWEwiIiIiIiIiIiojDAYRERERERERERURhgMIiIiIiIiIiIqIwwGERERERERERGVEQaDiIiIiIiIiIjKCINBRERERERERERlhMEgIiIiIiIiIqIywmAQEREREREREVEZYTCIiIiIiIiIiKiMMBhERERERERERFRGGAwiIiIiIiIiIiojDAYREREREREREZURBoOIiIiIiIiIiMoIg0FERERERERERGWEwSAiIiIiIiIiojLCYBARERERERERURlhMIiIiIiIiIiIqIwwGEREREREREREVEYYDCIiIiIiIiIiKiMMBhERERERERERlREGg4iIiIiIiIiIygiDQUREREREREREZYTBICIiIiIiIiKiMsJgEBERERERERFRGWEwiIiIiIiIiIiojDAYRERERERERERURhgMIiIiIiIiIiIqIwwGERERERERERGVEQaDiIiIiIiIiIjKCINBRERERERERERlhMEgIiIiIiIiIqIywmAQEREREREREVEZYTCIiIiIiIiIiKiMMBhERERERERERFRGGAwiIiIiIiIiIiojDAYREREREREREZURBoOIiIiIiIiIiMoIg0FERERERERERGWEwSAiIiIiIiIiojLCYBARERERERERURlhMIiIiIiIiIiIqIwwGEREREREREREVEYYDCIiIiIiIiIiKiMMBhERERERERERlREGg4iIiIiIiIiIygiDQUREREREREREZYTBICIiIiIiIiKiMsJgEBERERERERFRGWEwiIiIiIiIiIiojDAYRERERERERERURhgMIiIiIiIiIiIqIwwGERERERERERGVEQaDiIiIiIiIiIjKCINBRERERERERERlhMEgIiIiIiIiIqIywmAQEREREREREVEZYTCIiIgavIEDB0JEokttbS3Wrl2LTz75BEOGDMH++++f9J6hQ4dCRHLaTkVFBYYOHYrevXvnq+gN2scff4xnnnkm+neknbt06VKv2+3Tpw+qqqpw4IEH1ut2iIiIiCg1BoOIiKhoXHXVVejevTv69u2Lm266CQsWLMDdd9+NxYsX47TTTotL+8ILL6B79+455d+oUSMMGzYMp556ah5L3TCdc845OPnkk/HAAw/s8W1/8sknmDNnDoYPH77Ht01EREREDAYREVER+f777zF79mx8/vnnmDBhAm6//XYce+yxqK6uxoQJE9CiRYto2tWrV2P27NkFLG3Dds8992DixIlYs2ZNQbb/1FNP4fLLL8dBBx1UkO0TERERlTMGg4iIqKitXLkSd9xxB/bee29cd9110fWpLhP77W9/i2nTpmHjxo2oqanBr7/+in//+9+oqKhAu3btsHHjRgDAsGHDopekjR07FgDwm9/8Bi+99BJ+/PFHVFdXY9WqVZg0aRKOPvrouG307t0bIoJLLrkEDz74IFavXo1t27Zh6tSpOPzww5PK379/f3z88cfYunUrqqursWjRIgwZMiQuTZcuXfDuu+9i06ZNqK2txddff40//OEPu9xmnTt3Rrdu3fDqq69mTduyZUvMnTsXP/74Iw499FAAwNixY1FVVYUjjjgCH374IXbs2IE1a9bg7rvvBgB069YNM2bMwI4dO7BkyRJceeWVSfm+99572LFjB6655ppdrgcRERER7RoGg4iIqOhNnjwZwWAQvXr1SpumXbt2eP/99+H3+/HHP/4RZ5xxBoYMGYLq6mq4XC6sXbsW/fv3B7DzErPu3btHL6M68MADsWnTJgwZMgRnnHEGbrrpJgSDQcyePTtlkGf48OFo164drr76alx77bU47LDD8N5770HrnR+9f/zjHzF58mRorXH99dfj97//PUaPHh13tsypp56KL774As2aNcP111+Pc889FwsWLMD48eMxcODAXWqvs88+G8FgEJ999lnGdB07dsTs2bPh8/nQo0cP/Pzzz9HXnE4nJkyYgPfffx/nnnsuPvjgA4wYMQIPPfQQXn75Zbz00ks4//zzsWTJErz88ss4/vjj4/IOBAKYOXMmzjrrrF2qAxERERHtHuHChQsXLlwa8jJw4EAREenSpUvaNGvXrpWFCxdG/x46dKhI+NQgASADBgwQEZFjjz02bR777befiIgMHTo0a5m01uJwOGTJkiUycuTI6PrevXuLiMh//vOfuPQXXnihiIh069ZNAEjjxo1l69at8tlnn2XczqJFi2TevHliWVbc+kmTJsnq1atFKZVze77//vuyaNGijO182mmnydatW2X8+PHidrvj0o0dO1ZERM4///zoOsuyZN26dSIi0rlz5+j6ffbZRwKBgDz66KNJ23vggQckGAxKo0aNCt7HuHDhwoULFy5cymnhmUFERFQSlFIZX1+wYAF8Ph/+8Y9/4Morr8TBBx+cU/6WZeH//b//h4ULF8Ln8yEUCiEQCODwww/HkUcemZR+0qRJcX9/++23AMJnKAHASSedhKZNm+Lpp59Ou83f/OY3OPLII/HPf/4zWobIMnnyZBx44IE44ogjcqoHED7Laf369WlfHzhwICZPnowXXngBF110EXw+X1Ia27YxefLk6N+hUAg///wz1qxZgwULFkTXb9myBevXr4/WO9b69ethWRZatmyZcx2IiIiIaNcxGEREREWvUaNG2G+//TLeDPmXX37B6aefjvXr1+Opp57CL7/8gp9//hm33HKL0TZGjRqFBx54AO+88w5+//vf48QTT0TXrl2xYMECVFRUJKXftGlT3N+RgEok7f777w8AWLVqVdptHnDAAQCAkSNHIhgMxi2RR8I3b97cqPyxKioq4PV6075+ySWXoLa2Fi+88ELaNDU1NUlBIr/fj82bNyel9fv98Hg8SesjZUjVfkRERERUfxyFLgAREdHuOuuss+BwOPDpp59mTPf555/j888/h9YaXbt2xc0334wnnngC69atw7/+9a+M773iiivwyiuv4N57741b37x5c2zdujXnMm/YsAEAMj5NK3JD6+HDh2PChAkp0yxZsiTnbW/cuBH77rtv2tcvv/xyPPDAA5g+fTr69euHb775JudtmIiUIVJPIiIiItozeGYQEREVtTZt2uDRRx/F1q1b8dxzzxm9x7ZtzJkzBzfddBMARG9unHj2TiwRSToT5swzz9zlR6PPnDkTW7duxfXXX582zY8//ogff/wRnTp1wrx581IuO3bsyHnbP/zwAw455JC0r2/evBmnn346Fi9ejGnTpqFbt245b8PEIYccgo0bN2LdunX1kj8RERERpcYzg4iIqGgcffTRcDgccDgcaNGiBU455RQMGjQIoVAI559/fsYzTK677jr06dMH77//PlasWAGPx4M//vGPAICPP/4YALBjxw4sX74c5557Lv773/9i8+bN2LhxI3799Vf85z//wVVXXYUffvgB3377Lbp06YK//OUvWLly5S7Vpbq6GnfccQdefPFFfPzxx3j++eexbt06HHrooejUqRNuvvnmaLk/+OADfPjhhxg3bhxWr16NfffdF0ceeSSOP/54XHTRRdE8ly1bBgBZ74f06aefYvDgwTjssMPw008/pUyzY8cOnHHGGZgwYQKmTp2Kc845J+uZV7nq3r07pk+fntc8iYiIiMhMwe9izYULFy5cuGRaIk+5ivB6vVJZWSnTpk2TIUOGSPPmzZPek/g0sW7dusnbb78ty5Ytk9raWtmwYYNMmzZNzj777Lj39enTR+bNmye1tbUiIjJ27FgBIE2bNpXnn39eKisrZceOHfLZZ5/JySefLNOmTZNp06ZF3x95mtgFF1wQl2+7du1ERGTgwIFx68844wyZNm2aVFVVyY4dO+T777+Xv/zlL3FpjjnmGHnzzTelsrJSfD6frFmzRj7++GO59tpr49KtX79eZs6cmbU9mzRpItu3b5c777wzZTvHPrXN6XTKW2+9JTU1NfK73/1OgPDTxKqqqpLynTZtmnz33XdJ65ctWybvvfde3LpDDjkk6YlkXLhw4cKFCxcuXPbMour+QUREREXsyCOPxKJFi3DWWWfFPeUrndGjR+O0005Dx44d90Dpkv3v//4vrrzySvzmN79BKBQqSBmIiIiIyhXvGURERFQCfvvb32LmzJlGgSAAePDBB9G6dWtccMEF9VyyZE2bNsVNN92Ee+65h4EgIiIiogLgmUFERERl6qyzzsI+++yD1157bY9ut3Pnzjj99NPx6KOP7tHtEhEREVEYg0FERERERERERGWEl4kREREREREREZURBoOIiIiIiIiIiMoIg0FERERERERERGWEwSAqOod0AG79G+ByF7okRERERERERMWHwSAqOo0aA/u3BM69DFCq0KUhIiIiIiIiKi4MBlHR6twdGHAlA0JEREREREREuWAwiIraoR2BDscWuhRERERERERExYPBICpqVduAxd8Afc7mGUJEREREREREJhgMopLQoRMvGSMiIiIiIiIywWAQlYzjT2JAiIiIiIiIiCgbBoOopDAgRERERERERJQZg0FUcnhTaSIiIiIiIqL0GAyiksObShMRERERERGlx2AQlaxC3VT6lFNOwaRJk7B69WqICM4999ykNEOHDsXq1atRU1ODadOm4aijjop73eVyYfTo0diwYQN27NiBd999F61bt45L06xZM7zyyivYunUrtm7dildeeQVNmzaNS9OmTRtMmjQJO3bswIYNG/DEE0/A6XTGpTn66KPx6aefoqamBqtWrcL999+fp5YAli1bBhFJWsaMGQMAGDt2bNJrs2bNKlhb5MvQoUOT6rV27dqkNA2lD+TLkCFDMGfOHGzfvh3r1q3DxIkTcfjhh8elKdV9nk833HADfvnlF9TW1mLu3Lno2bNnoYtkrF27dnjhhRfwyy+/oKamBj///DOGDRuW1O6pxoXrrrsuLo3J2NSrVy/MnTsXtbW1WLp0aVIeADBgwAAsXLgQXq8XCxcuxHnnnZfXOsdKNeY9/PDDcWnyNS43lLr37t075f4UEXTt2jWarhT2+T333IMvvvgC1dXV2LJlS8o0DW3/FvN4QkRE9U+4cCmm5egukIeeCy833hted+O96dddMBCi1J4r3xlnnCEPPPCAnH/++SIicu6558a9ftddd8m2bdvk/PPPl44dO8obb7whq1evlr322iua5umnn5aVK1fKaaedJp07d5b//ve/Mn/+fNFaR9NMnjxZvv32W+nevbt0795dvv32W5k0aVL0da21fPvtt/Lf//5XOnfuLKeddpqsWrVKRo8eHU3TpEkTWbt2rbz++uvSsWNHOf/882Xbtm1y++2356UtmjdvLgcccEB0Oe2000REpHfv3gJAxo4dK5MnT45Ls88++8TlsafaIp/L0KFD5bvvvourV/PmzRtkH8jn8sEHH8jAgQPlqKOOkmOPPVbee+89Wb58uTRq1CiaplT3eb6Wiy66SHw+nwwePFg6dOggjz32mFRVVUmbNm0KXjaTpX///vLSSy9J37595eCDD5bf//73UllZKY888khcOhGRgQMHxvUDj8cTfd1kbGrfvr3s2LFDHnvsMenQoYMMHjxYfD6fDBgwIJqme/fuEggEZMiQIXLEEUfIkCFDxO/3y4knnlgv9V+2bJncd999cfVq3LhxTv2y2OrudDrj6nvAAQfIP/7xD/nll19Kbp8PGzZM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0TJk0lD2+e7s30QNaf825PGEiIgajoLfxZoLl1yWXXmaWKZ1+V4aN24snTp1kk6dOomIyK233iqdOnWKPsr1rrvuki1btsh5550nHTt2lH/+858pHyu+YsUK6dOnj3Tu3Fk+/vjj6KO1XS6XDB06VD788ENZsGCBdOvWTbp16ybffPNNykdrT506VTp37ix9+vSRFStWxD3idu+995a1a9fKP//5T+nYsaOcd955snXr1rw9Wh6AKKVk+fLl8vDDDye10yOPPCLdu3eXdu3aSe/eveWLL76QlStXpmyL/v37yzPPPCOffPJJyseM725b5HN55JFHpFevXtK+fXs58cQTZdKkSbJt2zZp27btLvWBE044QZYuXSoLFixo0PV+6qmnZMuWLdKrV6+Uj48u5X2eryXyKOhrrrlGnnzySXniiSekqqoq2nca+tKqVSv58ccf5eOPP5YDDzwwrh9E0px99tly9dVXS8eOHeWQQw6RwYMHy9atW+Xxxx+Pjm/NmzfPOjZFHr89cuRI6dChgwwaNCjp8ds9evSQQCAgd911lxxxxBFy11131duj5bt37x4d79u3by9/+MMfZNWqVfLOO+8Y9ctirjsA6dOnj4iIdOjQIem1Utnnbdq0kU6dOsn9998v27dvj37WN27cOOv+jeQR+7nbuXNneeONN+qtnpHxZNCgQdKhQwcZNWpUUY0nXLhw4cKl3peCF4ALl5yWfAeD+pyd38fO9+7dW1IZO3ZsNM3QoUNlzZo1UltbK59++ql07NgxLg+32y2jR4+WjRs3SnV1tUyaNEkOOuggASBNmjQREZG2bdvKq6++Ktu2bZNt27bJq6++Kk2bNo3Lp02bNvLee+9JdXW1bNy4MTrhiGvPo4+W6dOnS21traxZs0b++te/5nV/9e3bV0REDjvssLj1Ho9HPvzwQ1m3bp34fD5Zvny5jB07NlrPxLbYtGmTiIhMnjw5Kc0+++yTl7bI1/LGG2/I6tWrxefzyapVq+Tf//63HHnkkXFpcu0DqSZZDa3e6QwcOLDk93k+lxtuuEGWL18uIiJff/21nHLKKQUvk+kycODAtP0gkqZ///7y9ddfy/bt22XHjh3y7bffyi233CKWZUXHtyZNmhiNTb169ZJ58+aJ1+uVX375Ra677rqkNBdccIEsXrxYfD6fLFq0SM4///x6qftxxx0n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98d6OK7zfszURxnzvA8LWcZ8H6/1cVwXsE+YxlnN+4RVsO8UfmWhKhBCVSCEmwf9D9559kkopbBw4UJUVVUlLc2aNcM///lPbN68GRs2bMATTzwBpzP+DK2jjz4an376KWpqarBq1Srcf//9SVXu1asX5s6di9raWixduhTXXXddUpoBAwZg4cKF8Hq9WLhwIc4777ykNDfccAN++eUX1NbWYu7cuejZs6dZmxMREQAGg4hKVD1MJEx/faaGqR66BBFRVvXx0WEavOHHljGX04l3/js97etaa7z//vto3LgxevbsiUsuuQQXXHABRo4cGU3TpEkTTJ06FWvWrMEJJ5yAm2++GXfeeSduv/32aJr27dtj8uTJmDFjBo477jgMHz4co0ePxoABA6Jpunfvjn/961949dVX0alTJ7z66qsYP348TjzxxGiaiy66CI8//jgeeughHHfccZgxYwY++OADtGnTJs8tQ0RUuniZGBGZyXswoRiiE0UwkyhoMxZB+1AJKIaxgqi4DXvqeTRp3BgP33Zjytf79euHo446Cm3atMHatWsBAHfccQfGjRuHe++9F1VVVbj88svh8Xhw1VVXwe/3Y+HChTj88MNx++23Y9SoUQCA66+/HitWrMBtt90GAPjhhx/QtWtX3HnnnZgwYQIA4NZbb8XUqVMxYsQIAMCIESPQu3dv3HrrrbjssssAALfffjtefPFFvPjiiwCA2267Df3798cNN9yAe+65p/4aiqi+8TKxEsHLxIioUDh3yg+2Y2b1cSlLwZRSXYiI8qtHjx74/vvvo4EgAJgyZQo8Hg+6dOkSTTN9+vS4J41NmTIFrVu3Rvv27aNpPvroo7i8p0yZgq5du8JRdyl8ujQnnXQSAMDpdKJLly5JaT766KNoGiIiyo5nBhFRfpXUnLqkKkNEOSjo0V8fGy+Gszs55DZYLVu2xLp16+LWbd26FT6fDy1btoymWb58eVyayHsir6XKZ926dXA6nWjevDkqKyvTpolsp3nz5nA4HBnTEBWvECA8M6joGT5luNCKo5REVHpyuaeoaUJetUREpcB4LMtl0MvvAKk44DZ4Q2+8GsNuvCZjmq4XD8S8hT8Y5Scp7h2olIpbn5hG1Z1Bmo80ietM0hARUXoMBhFRfpl+Dyul72sK9VCfUmogovpnGjQurZNP6mXwoRIx5vW38OYHUzOmWb56bcbXIyorK9GtW7e4dc2aNYPL5YqeoRM5qydWixYtACBrmkAggE2bNmVME8lj48aNCAaDGdMQFStlB3lmUClQxbEPGQwiKjIiNuB0hR9Hm5ICFCCOhHXpKAVxWFnnE6I14PFkL5+lIWnSScx/oS2Ilea2ZZGyqMj/FOD3ArYNeBolp1c7y6gsgzJqBbvCJJ2GXVGRNV24yNmnmAoCURaQ8Cje1Ik1pJEOP8WtZke43lbyPg+XMb+PHBcFiNOZnDphv0BrSKQdM/Qf21KAx2WwXRV/Izu/F7AF4qlIKosoBTgdWbcNrSEe985yp0krltqZLmMZs2wvNq1WKfdZxjJG2CHA5w0/AjpyrBuWEeZFDOeZdiyJyS9VGSNi28RSkEyP1I7ZkanKKH4vlC2AZ+dxJwqwtUH/yTZGRcYJpYAKK74QCR1Mkldl2TZgpxvPYtMpBTRKMabYNlBbXXecO4z7jgCA2EbjD5SCWNm/9ollOj4qKIN0gAJcGY5VnxeQ8NguAMQpafdLlNawo/1Rpa+9Tv95lJQu2z3QIi/bkiFtTAW1hrg8SD/o2IDfV6/3Xtu0dRs2bd2Wl7xmzZqFe++9Fy1btkRlZSWA8E2lvV4v5s2bF00zfPhwOJ1OBAKBaJrVq1dHLx+bNWsWfv/738fl3a9fP8ydOxfBYDCapm/fvnj88cfj0sycORMAEAgEMG/ePPTt2xfvvPNONE3fvn3x7rvv5qW+RETlgMEgoiKjlAMI2gDstGnEsqBCIaP8TNMqVQHl9WdNZ1dYUF5v6jxit+tyQfmz5xfetq57twV4fWnTicsJ5Q8YlNEDXZu6jHHpPB5ogzqLVuEJrAHldEEFs7e3XeGGrq3btnYD/hCA5PfZHpdZGS0NbdYlIA7LrIyG20YuZYzr1nWTYW/yPs2pjL7sfQIep1G6XPa17bSgAyb7Ok0ZtQsI7DzWbbdhGRWgDKNBtsuC9mcvo6QrY2J+bge0b3d+DUve5+K0oI2Oa7N+ZtqOuRCXaRljjutEMce58b4GAAkZBa7Mx0e30fgoHjdUhvE4ms7SUKH0n1exY7ttaahg9v4THpuzbxsVZp9b4nKGAzMGTAOFRp9xytFgLmtq0/IAtGl5AADAsix06tQJAPDzzz+juroaH330ERYtWoRXX30Vf/nLX7Dvvvvi0UcfxfPPP4+qqioAwOuvv46hQ4di3LhxGD58OA477DDcc889+N///d/odp599ln86U9/wsiRI/H888+jR48eGDx4MC699NJomieeeAKfffYZ7rrrLrz77rs499xzcfrpp6Nnz57RNKNGjcKrr76KuXPnYtasWbj22mvRtm1bPPvss3uiuYjqD88MKg08M4iIaPfl9gt9aV0AQlR8SusYzPUMIaKoIus4//una3HVeWcDAJo0aYIFCxYAAE499VRMnz4dtm3jrLPOwtNPP40vvvgCtbW1eP3113HnnXdG89i+fTv69u2Lp556CnPnzsWWLVswatSo6GPlAWD58uU488wz8dhjj+Gmm27CmjVrcMstt0QfKw+Ezwy65JJL8OCDD+KBBx7A0qVLcfHFF2POnDnRNOPHj8d+++2Hv/71r2jVqhW+//57nHnmmVixYkU9txQRUelgMIiIDBXZN9s9Kodrh0ybsWH8WNyAsYGoAeHwuGexvfNu0H0P4JaHR2H77E+w9957R8/2ibVy5cqkS7wSff/99+jdu3fGNJ999ln0cfTpvP3223j77bczpnnmmWfwzDPPZExDRETpmd5ogojKHiffeVEvTwkyUAyTp2IoI+15+e4XHMqIiKihsoNcSmUxNGTIEMyZMwfbt2/HunXrMHHiRBx++OEZ39O7d2+ISNJyxBFH5NTdGAwiKiacxGRRQg1UjzcVJdqJ/Sw/2I5pldCwnBvDPlG27UNEREA4sPPUU0+he/fu6Nu3LxwOBz766CM0apTioTkJDj/8cLRs2TK6/PTTTzltm5eJEZWiQs5LOCdqoHJ5DFYZnpVEexzvx0NJ8t4hGGkhouKihDeQLg3m+/B3v/td3N+DBg3Chg0b0KVLF8yYMSPje9evX49t23b9qZE8M4iICoOzQCLKq9IZVEqnJkREROWrSZMmcYvL5cr6nqZNmwIANm/enDXt/PnzsWbNGnz88cc49dRTcy4fzwwiKkmcSlCJ4w/+DVMDeUw2UU7YbYmoobBtQEKFLgXtLmUDAFavXh23etiwYfjb3/6W8a2jRo3CjBkzsHDhwrRp1q5di2uuuQbz5s2D2+3G//zP/+C///0vTj311KxnE8ViMIiIGrZiuHdOfRSRkxOiesKDi4iIiOpf69at457O6PP5MqYfM2YMjj32WPTs2TNjuh9//BE//vhj9O8vv/wSbdq0wZ133slgEFGp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OXgGlTwgfWPs5AsgXbDFNU/MIH/RhaHoITSXgN1FsxE7+iBz3569/Octt079+a9bbwOg0+kAaeyeq666im984xucfvrpU7eRH+cJT3gCq6ur7NmzB4BrrrmGU045hXp94AV42mmnsWvXrv7ysWuuuYZnPOMZfUNQT+baa68ljuMRmWFOO+00vvzlL/c9khRFUZR8qDFIURTlIOGrjM1j0VJ5zCHvgpOchzGofHx3y8pnDiqSXHlXIIB08SWszmjLRI08leOoo47iqquu4rbbbuPss8/moQ99KEceeSRHHnlkX+Y5z3kOL3/5yznxxBM57rjjOOOMM3jb297G+973vn7A6IsuuohOp8OFF17IiSeeyPOf/3ze8IY3jCzr+sd//Ece+chHcv755/OYxzyG008/nTPOOIPzzjuvL/Pud7+b0047jde//vWccMIJvP71r+fpT38673rXuw5amyiKoiwaukxMUaqEvlArQ8zBAcNf/SxYsLzdovLmXbRBz98oks9sMwfPIN92qoANw7eIZVZlPjvsSTU8hJTSOe2003j0ox/Nox/9aHbt2jVyrrdcPYoiXvWqV/GOd7wDay0333wzf/Znf8Z73vOevuy+fft4xjOewXve8x6uvfZa7r//ft7xjneMGIN++MMf8qxnPYt3vvOdvPrVr+b222/nta99LTfffDN//dd/zSMf+UharRbXXXcdb3rTm3j729/O8vIyL3jBC/ja1752cBpEUQ4SukxsQahIH6oxSFGUQqnG1Le+KbUNi7YwzaEyZSqz8/ATKW35IPkcboru8jXC0k/Ju2jjVvGeU/618U2vRHJFaFYWkQ9+8IN88IMfXFPmiiuu4IorrshM6zvf+Q5Pe9rT1pTpxf/p8ZKXvIRrr70W5xx3331339Po3nvv5d5770VE+PjHP+5RE0VRFGUWagxSFKUU1GhUAFVoRO/dcspbZDMPY8w8vLHm0d1zMax5fhuWz9xQ4mD3DSJdeEcukDGm1LmqpMwXqPvK4I1vfCOf+tSneOlLX9qPP6QoGwFx6Nbyi4DHzpjrATUGKUql8Hy7rMJLaBXKuM7JtVLLe4VPOS8g5QaQLi/veaZafM4FLxPLNQcUHigqh6jf0irvJKsw96keopTMzp07efWrX62GIEVRlDmixiBFUZSK4rOzy7woM3R10QarPMu61xJ1OKTrZ5Tg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W/nEEt2oa9+trge4lY+JO5YPuO9nCcd8Jxz3R3CvH9dtx5vc8+0y0AqYJsfjwfm4caxryLVTLvlxPm6aIO3QThnjPiAUS7i1z00DIeUYLumQxkgUMo47mhd1y09iAKRcvhcGQavDthMDIOUQzo+4z+TxI24/x7tuu2kQtDp8X8cHwPgtqofrBRfdfh+X3f0A53zty5zz9ZOK3lu2bBlbbrll/vk555zDiSeeSHNzM3vttRe33347L730Uv79WCzGJZdcwtFHH01TUxNz5szh1FNPLRpYam5u5oorruDggw8G4J577uFb3/oW77/fMTNqwoQJXH311ey99960tLRw6623cuaZZ5JOuzZ+IrXNoouE60Gt1KEGg6ThpVrh3w/kHpA7rz36a/Dx7eDFF9sGg6Kx3GBD2DzX22k7Tisxhh5vrlwHjTwPpx698XCb6t8L6zO4bttzLEevN9LouuiL4z7h9cJScp5xG7xx3bZrXqCt8+0SrDvHjPPG3YK57he9kG/nbXdr3+3h/DiWuTVgnJszxzid90nXPHdjMMi1yGumLXVNo0t83ShvV67fhz19zBgT2vlFCkilMySDgHmvvsahM8/mv/f/Lx/72Md4//33WbduHQBnn3023/jGNzjxxBNZuHAhP/jBD3jggQfYaqutWL9+PQCXX345Bx10EEcddRQrV67k0ksv5d5772Xq1KkEbZf23nrrrYwfP5799tsPgOuvv55bbrklPzjkeR733XcfK1asYLfddmP48OHcfPPNGGOYOXNm3xeQiEid02CQNKw1K3P/3nRFblbQR7eBdS/CYSfAuInhpq0i3yOwqdwviX77wFDnE07rG2gqObm0bf8rOjk2BI7jS/koqvE8gkTBFPoKH7IGgniVJsiC9QxBLALpZK4TVXrS3Ba/9SCo1HErSYMxXkl/zJZPp4HANx1l1/Fy8bYpub18mbgaeSnRMH8dcb0LVq38giN9qxaO2/Y0lt2HizJgO9opU+4zBkyuLbV+mZybThFiCbCFr1UoMOsZgqife7/03uzpVFvbnsi147FI1YIPfA8Tr3CpVsFnLQYibgNMFouJVj8ttj4Ehd+vtiBDhds2BttU7nLWtlIPLLSud7tUsg9kslmWr1oNwPLly/MDQQDf/va3+clPfsJdd90FwAknnMCyZcs45phjuP766xkyZAgnnXQSxx9/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j9tGZdFm2Ge/jJcYrPJoM/qwH7Luub8SG70lXjQednJCN/7km1h66+lEBg4jNqrnB9gTA30AoiM/QiKTzL8++aOjGDEozg9mr+D/Fq/k6O2GcMz2k/jz7OV8nCjpppG8sG4NX7nrPb779bN465mHAPjFL37Bz372s3w8K1asIAiCHk+3iIgU02ViUpMGfWwHGDAy7GRUZK1t+MWiS6lMRNwF6VbSKxcRHT6xV37ZF6kn7QtI6zumQ29+50YjEZY/eSdfOusi/vrQE/nX/zvn9wRBwKR9v4TneQRBwH/uuo77Hp7LTtt9nOdfeY3vXnw9ACcduheXnf8dPM9jq622YuHCxl5XUUQkDBoMEhERERERZ3PnzuWZZ57hG9/4BpBbRyiZTHLnnXfyxS9+MR+ufR2huXPnctBBBzF58mROPfVUrrzyShYtWsTmm2/OG2+8QSKR4KWXXuLHP/4xDz/8cEi5EhFpLI19b2cREREREemWyy67jK985SvMmDGDrbfemquuugpjDH/4wx8AuPDCC7n55ptZtmwZY8aM4brrrmOzzTbjX//6F5dffjn/+te/2HTTTbn22mv5whe+wGGHHcaCBQuYM2cOu+++e8i5ExFpDFqcQUREREREnN12220MHz6c8847j7Fjx7JgwQIAlixZAsDYsWOZOHEiyWSScePG8dhjjzFw4EA+/elP43keH/3oR5k5cya/+tWv8nHOnTuXCRMmcNFFF5FIJJg8eTLvvvsuF198Mb/61a8wxuQvCRQRkZ5h9dBDDz300EMPPfTQQw89PsgjGo3adDptDz300KLX77rrLvvmm2/az3/+89Zaaw899FA7ZsyYivH8/Oc/t9ls1v7iF7+wu+++uz3vvPNsMpm0hx9+uAWs7/uh51UPPfTQo14eukxMREREREQ+sHQ6zTPPPMO+++5b9PqkSZO49dZbueuuuwCw1rJ06dKK8Rx00EG0tLSwZs0abrrpJs4//3zS6TQ33HADgwYNIpvNApBIJBg+fHjvZUhEpEGEPiKlhx566KGHHnrooYceetTu44gjjrDJZNLOmDHDbr311vayyy6z69atsxMnTrSAtdbahx56KB/+tNNOs4cccoj92Mc+ZidPnmwvvPBCa621b731ls1ms3bOnDn2y1/+sr3xxhttNpu1zz77rIXc7KBvfetb9t1337VbbbVV6PnWQw899KjVh9YMEhERERGRD6V0HaF58+Yxffp0Fi1alA8zcuTI/N+xWIxLLrmEcePG0dLSwvz581m7di3jx4/n5z//Oddddx1vvvkmL7/8Ml/+8pdZu3Ytn/vc55g4cSLnnXcey5cvz69VJCIi3adby4uIiIiISK+y1nLooYeyatUqzjrrLKZOncqmm27KoYceyt13383o0aNZtGgR77zzDvvssw9vvPEGAN/4xje46qqrOsW39dZbs2DBAnzfz18+JiIi7rRmkIiIiIiI9ImBAwfy/PPP881vfrPo9U022YRoNMqbb76ZHwgyxtDc3AzAa6+9RhAEPP3004wZM4ZXX30Vz/M0ECQi8gHpMjEREREREekTf//73/n73//e6fXW1lbWrVvH5MmT87eRt9ay8847A7DFFlswZ84cpk2bBuQuM0ulUn2adhGReqKZQSIiIiIi0uMGDhzIdtttx3bbbQfkBnS22247JkyYkA9z2mmnAfDmm2/y7LPPMmLECH7zm9+w9dZb89WvfpX9998fgFQqxZQpU3jwwQfZc889Ow0EeZ66NSIi3aE1g0REREREpMftsccePPzww51ev+mmm5gxYwbWWubNm8e2226LtZZIJMJzzz3HxIkTGThwINlsFt/3eeONNzj88MOJx+N8/etf5/jjj+cvf/kLr732GvPmzeO2226jtbVV6weJiHSDhtBFRERERKTHPfLIIxhjOj1mzJiRD/Pss8/y5JNPsnbtWhYvXsyrr77KN7/5Te644w583+eBBx7gYx/7GM8++2x+wMgYw3777cfMmTP57W9/y5o1a5g5cybZbFYzhEREHKm1FBERERGRUEyePJmrr76anXfemWnTphGJRPjhD39IIpHgtddeY7/99gNg3LhxfOtb3+LQQw/l1VdfJZFI8Otf/5qjjjqK119/nV/84hcceeSRBEEQco5ERGqH1UMPPfTQQw899NBDDz306MuHtdYecsghRa+NGDHCWmvtHnvsUfT6PvvsY7PZrH3ggQdsEAS2paXFAtb3fbvnnnvadevW2fnz54eeJz300EOPWnloZpCIiIiIiPSJaotK/+hHPwLgvffeA+A73/kOhxxyCMcccwzz58/n6aefxhhDPB7n6KOPJpvN8uyzzxKPx5k0aRKRiG6WLCLiQq2liIiIiIj0iU9/+tNFi0r/4he/ADoWlZ4+fTpr1qxh/vz5APi+zyWXXMJmm22G53msW7eOxYsX8+KLL/L73/+etWvXAmCMIRKJMGLECJYuXZqP3/M8XTomIlJB6NOT9NBDDz300EMPPfTQQ4/Gflx11VX2jTfesOPGjev03iGHHGKfeeYZu/vuu9sFCxbY733ve/acc86x6XTarl692j733HPWWmtHjx5tATtz5kzb1NQUep700EMPPfrrQ5eJiYiIiIhIqK644goOPvhg9tprLxYvXsz3vvc9nnrqKdauXcuyZcuYMWMG6XSaiy++mPfff58xY8Zw0UUXccYZZ9Da2srs2bPJZDIsXboUay2//OUv2bhxI9ZattpqK91lTESkhFpFEREREREJzZVXXslhhx3G3nvvzZtvvgnAHnvskb/L2Oc+9zl832fMmDHEYjFGjx7N4YcfzuDBg7niiivYfffdGTRoEAsWLAAgnU6zevVq/vznP/PlL3+ZxYsXEwQBvu+HmEsRkf5Fg0EiIiIiIhKKq6++muOOO45jjjmGdevWMXr0aEaPHs3nP/95br75Zl566SWOOOIINm7cyGabbcYZZ5zBE088wahRo7jzzjvZdttt2X333TnppJNYvXo1AG+99RZnnnkmr7/+OkcccQRz585l4MCBZLPZkHMrItJ/aDBIRERERERCceqpp9Lc3MwjjzzC0qVL848jjzwyH2bs2LFsttlmAKxYsYKjjjqKE088kdGjR/PUU0/xP//zPzz00EN84hOfACAWi/HjH/+YHXfckd///vdYa7n44osxxoSSRxGR/siQWzxIRERERESkX7r77rvZZJNN2GOPPbC2uPty0UUX8ZWvfIWFCxdy55138tBDDzFo0CCOOuoovv71r/P000+zbt069t9/fzKZTEg5EBHpX3RreRERERER6beuuuoqtt12W3bbbbdOA0Ff//rXOfvss3nggQc48cQTWbp0Kb7vk81mefTRR5k8eTI77rgjt9xyC0EQYIzpFIeISCPSYJCIiIiIiPRL7XcZ++xnP8vixYs7vX/DDTew1VZbcckllxQNBAF84hOfYPjw4UQiEf7xj38QBEGnz3ueV/Z1EZF6p8vERERERESk37nyyiv5/Oc/z5577sl///vfTu8XDvwARCKR/GVg2267Leeddx4HHXQQb731FpMmTQJg+vTpjB07lo0bN3LXXXfR2traKR4RkUagwSAREREREelXrr76ao455hgOOeSQ/C3jAd5//31aW1sBuPDCCxk3bhwnnHACAKeddhpvvvkmmUyGmTNnsvvuu9PU1MRhhx3GXXfdxXHHHcd5553H+PHjWbRoEWvXrmXvvfdm/fr1miEkIg1HdxMTEREREZF+xfUuYxMnTsw/j8Vi/PKXv+Tuu+9mn332YcmSJUyfPp277roLgMmTJzNixAh23HFHjjjiCNauXcu///1vBg4cqIEgEWk4mhkkIiIiIiJ1wRjDfffdx1NPPcWsWbOKXj/ttNM4+eSTmT59Om+99RZbbrklN9xwA6+++ipf//rX85eKGWMYNGgQ69atCykXIiK9TzODRERERESk5rXfKWz69On5gaBvfvObDB8+HGstDzzwAM3NzZxyyikAvP7669x8882sW7eOoUOH5uP5yEc+wsMPP8wOO+wQRjZERPqEBoNERERERKTmld4yfvLkyRx11FEcddRRRKNR5s+fz1lnncVZZ53FPvvsQzab5Y9//COXX345q1atwhiDMYbXXnuN++67jw0bNoSUExGR3qfLxEREREREpC7dcMMNTJkyhZNPPpl58+YRi8V49NFHee655zj11FPzl4Z5nsc+++zDl7/8ZU488cT8ItUiIvVKM4NERERERKSuGGMA+PrXv47v+1x33XXssMMOfPzjH6epqYmtt96aSCSSD7vbbrtx4YUX8vnPf55x48bl44nH4+y+++40NzeHkQ0RkV6jwSAREREREakr1lo8zyObzbLrrrvS2trKzTffzL/+9S8mT57MLbfcQjKZxBjD7rvvzhVXXMHw4cPZfvvtee2119huu+0YOnQo55xzDldeeSX77bdf2FkSEelRukxMRERERETqku/7ZLNZPM/jgAMOYNKkSSxYsIB7770Xz/PYfffd+eUvf0lzczMHHHAA8+fPB+Dqq6/miCOOwPd9XnzxRb7whS/w3nvvhZwbEZGeEwk7ASIiIiIiIr2hfSAoCAL++te/5l/3fZ/PfOYzZQeCfN8nk8kwdOhQkskkX/rSl3jvvfeIx+Mkk8mwsiIi0qM0M0hERERERBrKtGnTuOiiixg2bBgHHnhgfiAoGo1y/vnnc8opp/DKK6+QyWQYNWoUn/nMZ1i1alXIqRYR6TlaM0hERERERBrKMcccwzbbbFM0IygSiTBr1ixOOeUUnn/+eQ488ED23Xdf1q9fz9NPP53/rOepCyUitU8zg0REREREpKF4nsfEiRN58803gdylYRdccEF+IOjwww9n5cqVeJ7HqFGjiEQijB49mpdffpmNGzeGm3gRkR6gwSAREREREWkY7WsIFTrxxBO57LLLeO655/IDQe2LTwM0NTXxwgsv8PTTT3PsscdirbpQIlLbNMdRREREREQaRulAEMAnP/lJrLUce+yxnQaCADbffHM222wznnzySQ0EiUhd0GCQiIiIiIg0tEwmw8qVK4lEcjdbLhwIikQinHnmmbz++uv87ne/CyuJIiI9SoNBIiIiIiLS0L773e+ydu1a7rnnHsaOHVv0XiQSYbfdduPJJ59kzZo1ZT/v+34fpFJEpOdoMEhERERERBqW53lks1l23nlnotEoY8aMKXr/a1/7GhMmTODCCy8sukRs6NChzJgxgwEDBhTNJBIRqQWRsBMgIiIiIiISliAIiEQiZDIZpkyZAoAxBoBoNMoee+zBE088wYIFCxg2bBhjx47l7LPPZuedd+ZjH/sYn/jEJ/jOd74TZhZERLpNM4NERERERKShZTIZoGMQyFqLtZZtttmG6dOnM2fOHKZNm8af//xnnn76aXbddVfmzp3L5MmTufjii8NMuojIB6Jby4uIiIiISMOLxWJMnjyZV155hZaWFgYPHswFF1zAaaedxjvvvMP48eN57LHHuOeee7jppptYtWpV2TuTiYjUAg0GiYiIiIhIwxs6dCjPPvssCxcu5PHHH2fPPfdk6tSpLF++nKeeeoqrrrqKefPmsW7durCTKiLyoWkwSEREREREBPjUpz7FVVddxbhx41iwYAFPPPEEV155JevWrSOZTIadPBGRHqPBIBERERERkTZDhgyhqamJlStX5tcSEhGpNxoMEhERERERceB5XtE6Qb7v67byIlKTdDcxERERERGRKowx+YGgs846i0033bTbA0GRSIRYLNYbyRMR6RYNBomIiIiIiFRhrWXIkCH8+te/5qc//Sm33357/lb0LoYOHcp3v/tdfvSjH7H55pv3XkJFRBxoMEhERERERKSKnXbaiTfeeIO9996bO++8k6OOOgpr3VfceP/995k0aRIzZszg9ttv59Of/nQvplZEpGtaM0hERERERMTBYYcdxj333IMxhnQ67bxmkDEmP3B03HHH8bOf/YzRo0ez5ZZb8sYbb/R2skVEOtHMIBERERERkS60Xw525513kslkSKfTAM5rBllr83Fs3LiRIUOGMGfOHIYNG9Y7CRYRqUKDQSIiIiIiIl3ozuVgXcVx5JFHcvPNN/P444/zve99j2eeeaYHUici0n26TExERERERKSXHX744fzmN7/hscce45xzzuHZZ58NO0ki0sA0M0hERERERKQXaSBIRPobDQaJiIiIiIj0kL322otddtkl//zII4/kN7/5DY8//rgGgkSk39BlYiIiIiIiIj3k5ZdfJpFIcNRRR7H55pvz61//Or9GkAaCRKS/0GCQiIiIiIhID4lEIjz55JNMnDiReDzO448/zllnncWLL74YdtJERPJ0mZiIiIiIiEgP8H2fTCbDjjvuyCuvvMLAgQP5wx/+wLx584COW9SLiIRNM4NERERERER6iO/7ZLNZfN/nySefJJFI8NWvfpUnnniiR25RLyLSEzQzSEREREREpIe0DwRls1l23nlnhg8fzrRp0z7QQNCgQYOYPHkyU6ZM6YWUikgj08wgERERERGRHtY+IGSMcRoIKg23xx57cNJJJ/GFL3yBxx57jAMOOIB0Ot2bSRaRBqKZQSIiIiIiIj2sdCDI87ruerWH22+//fjlL3/J7NmzGTp0KGeeeSbTpk3TQJCI9KhI2AkQERERERGpR4UzfYIg6PR++2DRgAED2HTTTfnxj3/MdtttRyaT4YQTTuAf//gHq1ev7sski0iD0GViIiIiIiIiIdlmm2347ne/y2677UYqleKHP/whjz32GIsWLQo7aSJSxzQYJCIiIiIi0sd23313pk+fzumnn86///1v5syZw0UXXRR2skSkQWgwSEREREREpA9dc801HHHEEbz99tv89re/5eabb+b9998HcmsLlbukTESkJ2kwSEREREREpA/tt99+jB8/nkcffZQFCxaEnRwRaUAaDBIREREREalBrretFxEppbuJiYiIiIiI1ID/9//+H/F4nLfffpuXX36ZTCaD7/tks9mwkyYiNUaDQSIiIiIiIv2U53kccMABfPvb32bPPfcE4PXXX+fVV1/liCOOYP369VpnSES6TZeJiYiIiIiI9FMHHnggl19+OdFolJ/97Ge8+OKLTJo0iRkzZrDJJpuw4447smHDhrCTKSI1RoNBIiIiIiIi/dQDDzzAVlttxfTp05k3b17+9S222ILf/va3vPnmm5x00km6VExEusULOwEiIiIiIiLS2R577MHee+/Nz3/+86KBIIA33niDX//612zYsIGRI0eGlEIRqVVaM0hERERERKQfisViAMyfP7/s+3fccQfz589n6dKlAEQiETKZjNYQEpGqNDNIRERERESkH1qyZAmvvfYakyZNwhjT6f3W1laeffZZAK688kpmz55NPB7XQJCIVKXBIBERERERkX5o3rx5vPzyy5x88sl89KMfLRoQ8ryOrtx5553HIYccwjbbbMOECRPy7/m+3+dpFpHaoAWkRURERERE+hljDNZaIpEIc+fOJZlM8qtf/Yo777yT9evX58NdcMEFfO9732Pjxo2sWLGCRx55hI997GMcdNBBrF+/Ph+PiEghzQwSERERERHpZ6y1+L5PJpNhp5124oUXXmDq1KlMmjQpH+ZHP/oRp556Ks899xw77rgjO+ywA1dddRVBEPDwww8Ti8U0ECQiZWlmkIiIiIiISD9VuBj0yJEjWbFiBQA//OEPOfXUU3nhhRc44YQTePvtt/Of+dKXvsSll17KgQceyJNPPhlKukWkf9PdxERERERERPqpwsWg2weCrrjiCo444oiigaBIJEI2m8VaSyKRYNiwYUQiue5e+6Vivu+TzWZDyYeI9C+aGSQiIiIiIlJD7rvvPiZOnMj+++/PO++8k7+lPMD+++/P7bffTlNTE3fccQexWIx169Zx6qmnsn79et12XkQADQaJiIiIiIjUFM/zGD58OCtWrCia7fO5z32O3/zmN2zcuJFf/vKX/OlPf2KHHXbglFNOYeLEiey88860traGnHoR6Q80GCQiIiIiIlIjCmf2FP7dPhC0Zs0azj//fO644478Z/bZZx9uu+02jjvuOP72t7+Fkm4R6V90NzEREREREZEaUXiJV/vfhxxyCDfccANr1qxh1qxZ+YGgeDwOwMaNGxk6dChDhgwpimv8+PHsuOOODBs2rI9SLyL9hQaDREREREREatiMGTMYMGAA5513HrfffjsAsViMZDKJ53lceumlvPHGG8yePTv/Gc/zmDFjBtdffz033ngjn/zkJ0NKvYiEQZeJiYiIiIiI1DDP8/jsZz/Lww8/DOQGglKpFAD//ve/+dSnPsXZZ5/Nddddl19out2MGTPYc889OeCAAzjwwAOZO3duXydfREKgwSAR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qDQng8756aefaiFo7ty5tdeXLl2alStX/tMQdPHFF2f27Nm55pprRnNdAAAAgPOqdDHonCuvvDLd3d158cUX8+CDD2bFihX54Ycfsn79+n94Iujqq6/OwoULs3379kyfPr2AjQEAAAD+e6W7JvZbN998cz744IM0NDTk3Xffzfr16/Pll1+moaEh1eqf/yxtbW1ZtWpVVq1alXnz5mXfvn0FbA0AAADw15U6BiXJ9OnTs3Pnzmzbti3t7e3/1nc2bNiQGTNmZOHChTl58uQF3hAAAADg/CntNbFz9u3bl7vvvjsPPPBAnnnmmTQ0NPzpMwsWLMjjjz9e+3nXrl259tprPXYeAAAA+L/TVPQC/wv6+voyc+bMnDhxItVqNePHj8/g4GDt/VOnTuXpp5/OuHHj0t3dnQULFuTo0aMZGRkpcGsAAACA/1zpr4n90YQJE/LII4+kp6cnn376ae319vb2bNy4Mb29vRkzZkzefvvtvPzyywVuCgAAAPCfczLoD06fPp1bbrklEydO/F0MOnDgQH7++eesWbMmR44cydDQUIFbAgAAAPw1YtAfDA0N5amnnspHH32UoaGhPPvss2lsbMx1112XQ4cOZXh4WAgCAAAA/m+5JvZPzJo1K1u2bEl/f39aW1szduzY9PX15f777y96NQAAAIC/TAz6F1pbW3PPPfekra0thw4dyqZNm4peCQAAAOC/8jfeoV2erv5NZQAAAABJRU5ErkJggg==",
                         "text/plain": [
-                            "<Figure size 1440x1440 with 2 Axes>"
+                            "<Figure size 1500x1500 with 2 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "def show_3d_column_density_plot(coma, x_min, x_max, y_min, y_max, grid_step_x, grid_step_y, r_units, cd_units, frag_name):\n",
+                "def show_3d_column_density_plot(vmr, x_min, x_max, y_min, y_max, grid_step_x, grid_step_y, r_units, cd_units, frag_name):\n",
                 "    \"\"\" 3D plot of column density \"\"\"\n",
                 "\n",
                 "    x = np.linspace(x_min.to(u.m).value, x_max.to(u.m).value, grid_step_x)\n",
                 "    y = np.linspace(y_min.to(u.m).value, y_max.to(u.m).value, grid_step_y)\n",
                 "    xv, yv = np.meshgrid(x, y)\n",
-                "    z = coma.vmodel['column_density_interpolation'](np.sqrt(xv**2 + yv**2))\n",
+                "    z = vmr.column_density_interpolation(np.sqrt(xv**2 + yv**2))\n",
                 "    # column_density_interpolation spits out m^-2\n",
                 "    fz = (z/u.m**2).to(cd_units)\n",
                 "\n",
                 "    xu = np.linspace(x_min.to(r_units), x_max.to(r_units), grid_step_x)\n",
                 "    yu = np.linspace(y_min.to(r_units), y_max.to(r_units), grid_step_y)\n",
                 "    xvu, yvu = np.meshgrid(xu, yu)\n",
                 "\n",
                 "    plt.style.use('Solarize_Light2')\n",
                 "    plt.style.use('dark_background')\n",
                 "    plt.rcParams['grid.color'] = \"black\"\n",
                 "\n",
-                "    fig = plt.figure(figsize=(20, 20))\n",
+                "    fig = plt.figure(figsize=(15, 15))\n",
                 "    ax = plt.axes(projection='3d')\n",
-                "    # ax.grid(False)\n",
                 "    surf = ax.plot_surface(xvu, yvu, fz, cmap='inferno', vmin=0, edgecolor='none')\n",
                 "\n",
                 "    plt.gca().set_zlim(bottom=0)\n",
                 "\n",
                 "    ax.set_xlabel(f'Distance, ({r_units.to_string()})')\n",
                 "    ax.set_ylabel(f'Distance, ({r_units.to_string()})')\n",
                 "    ax.set_zlabel(f\"Column density, {cd_units.unit.to_string()}\")\n",
@@ -587,51 +641,52 @@
                 "    ax.w_zaxis.set_pane_color(solarblack)\n",
                 "\n",
                 "    fig.colorbar(surf, shrink=0.5, aspect=5)\n",
                 "    ax.view_init(90, 90)\n",
                 "    plt.show()\n",
                 "\n",
                 "\n",
-                "show_3d_column_density_plot(coma_sine, -100000*u.km, 100000*u.km, -100000*u.km, 100000*u.km, 1000, 1000, u.km, 1/u.cm**2, 'OH')"
+                "show_3d_column_density_plot(vmr, -100000*u.km, 100000*u.km, -100000*u.km, 100000*u.km, 50, 50, u.km, 1/u.cm**2, 'OH')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "induced-telephone",
             "metadata": {},
             "source": [
-                "### Obtaining total counts of fragments within apertures\n",
-                "The model is compatible with any sbpy aperture for obtaining total counts of fragments:"
+                "### Obtaining total counts of fragments within apertures with total_number()\n",
+                "The model's coma object is compatible with any sbpy aperture for obtaining total counts of fragments:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 24,
             "id": "challenging-trigger",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Number of fragments in\n",
-                        "\tLarge rectangular aperture:  1.9456948716998955e+33\n",
-                        "\tLarge circular aperture:  2.008412781839869e+33\n"
+                        "\tLarge rectangular aperture:  1.9513579963113747e+33\n",
+                        "\tLarge circular aperture:  2.023818343905977e+33\n"
                     ]
                 }
             ],
             "source": [
+                "max_r = vmr.max_grid_radius.to_value(u.m)\n",
                 "print(\"Number of fragments in\")\n",
                 "# Set rectangular aperture to be the size of the entire grid\n",
-                "ap1 = sba.RectangularAperture((coma_sine.vmodel['max_grid_radius'].value, \n",
-                "                               coma_sine.vmodel['max_grid_radius'].value) * u.m)\n",
+                "ap1 = sba.RectangularAperture((max_r, \n",
+                "                               max_r) * u.m )\n",
                 "print(\"\\tLarge rectangular aperture: \", coma_sine.total_number(ap1))\n",
                 "\n",
                 "# One more time with a circular aperture\n",
-                "ap2 = sba.CircularAperture((coma_sine.vmodel['max_grid_radius'].value) * u.m)\n",
+                "ap2 = sba.CircularAperture((max_r) * u.m)\n",
                 "print(\"\\tLarge circular aperture: \", coma_sine.total_number(ap2))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "specific-truck",
             "metadata": {},
@@ -652,28 +707,34 @@
             "id": "eastern-protection",
             "metadata": {},
             "source": [
                 "Beyond the production and time dependence, the following can be passed to VectorialModel to tweak its behavior:\n",
                 "\n",
                 "radial_points (int): Number of grid points to use for the radial density grids, both volume and column density\n",
                 "\n",
-                "radial_substeps (int): Controls how much each grid point will slice up the density-contributing sections of the coma\n",
+                "radial_substeps (int): Controls how much each grid point will slice up the density-contributing sections of the outflowing column of parents\n",
                 "\n",
-                "angular_points (int): Number of angular slices to take around the coma\n",
-                "\n",
-                "angular_substeps (int): Controls the angular slicing of the density-contributing sections of the coma\n",
+                "angular_points (int): Number of angular slices to take of the space around the nucleus\n",
                 "\n",
                 "parent_destruction_level (float): Percentage of parent molecules that will be destroyed before the grid gets cut off\n",
                 "\n",
-                "fragment_destruction_level (float): Similar but for fragments\n",
+                "fragment_destruction_level (float): Similar, but for fragments\n",
                 "\n",
                 "max_fragment_lifetimes (float): If a fragment has to travel farther than this many lifetimes to contribute to the density at another point in the coma, we ignore it entirely\n",
                 "\n",
                 "print_progess (bool): This will periodically print out progress while calculating fragment density"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "e7aec478-423a-4468-8f3e-af7e1316ebb1",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -684,13 +745,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.10.4"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `sbpy-0.3.0/licenses/LICENSE.rst` & `sbpy-0.4.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/logo/LICENSE` & `sbpy-0.4.0/logo/LICENSE`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/logo/sbpy_logo.svg` & `sbpy-0.4.0/logo/sbpy_logo.svg`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/logo/sbpy_logo_full.pdf` & `sbpy-0.4.0/logo/sbpy_logo_full.pdf`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/logo/sbpy_logo_full.png` & `sbpy-0.4.0/logo/sbpy_logo_full.png`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/logo/sbpy_logo_logoonly.pdf` & `sbpy-0.4.0/logo/sbpy_logo_logoonly.pdf`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/logo/sbpy_logo_logoonly.png` & `sbpy-0.4.0/logo/sbpy_logo_logoonly.png`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/logo/sbpy_logo_logoonly.svg` & `sbpy-0.4.0/logo/sbpy_logo_logoonly.svg`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/logo/sbpy_logo_logoonly_inverted.svg` & `sbpy-0.4.0/logo/sbpy_logo_logoonly_inverted.svg`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/logo/sbpy_logo_short.pdf` & `sbpy-0.4.0/logo/sbpy_logo_short.pdf`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/logo/sbpy_logo_short.png` & `sbpy-0.4.0/logo/sbpy_logo_short.png`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/logo/sbpy_logo_short.svg` & `sbpy-0.4.0/logo/sbpy_logo_short.svg`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/publications/joss/paper.bib` & `sbpy-0.4.0/publications/joss/paper.bib`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/publications/joss/paper.md` & `sbpy-0.4.0/publications/joss/paper.md`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/publications/joss/structure.png` & `sbpy-0.4.0/publications/joss/structure.png`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/__init__.py` & `sbpy-0.4.0/sbpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/activity/core.py` & `sbpy-0.4.0/sbpy/activity/core.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/activity/dust.py` & `sbpy-0.4.0/sbpy/activity/dust.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 ===================
 
 All things dust coma related.
 
 
 """
 
-__all__ = [
-    'phase_HalleyMarcus',
-    'Afrho',
-    'Efrho'
-]
+__all__ = ["phase_HalleyMarcus", "Afrho", "Efrho"]
 
+__doctest_requires__ = {"Afrho.to_fluxd": ["astropy>=5.3"]}
 
 from warnings import warn
 import abc
 
 import numpy as np
 import astropy.units as u
 import astropy.version as astropy_version
+
 try:
     from astropy.utils.misc import InheritDocstrings
 except ImportError:
     InheritDocstrings = None
 
 from .. import bib
 from ..calib import Sun
@@ -32,19 +30,21 @@
 from .. import data as sbd
 from .. import exceptions as sbe
 from .. import units as sbu
 from ..spectroscopy.sources import SinglePointSpectrumError
 from .core import Aperture
 
 
-@bib.cite({
-    'Halley-Marcus phase function': '2011AJ....141..177S',
-    'Halley phase function': '1998Icar..132..397S',
-    'Marcus phase function': '2007ICQ....29...39M'
-})
+@bib.cite(
+    {
+        "Halley-Marcus phase function": "2011AJ....141..177S",
+        "Halley phase function": "1998Icar..132..397S",
+        "Marcus phase function": "2007ICQ....29...39M",
+    }
+)
 def phase_HalleyMarcus(phase):
     """Halley-Marcus composite dust phase function.
 
     Uses `~scipy.interpolate` for spline interpolation, otherwise uses
     linear interpolation from `~numpy.interp`.
 
 
@@ -100,97 +100,238 @@
         import scipy
         from scipy.interpolate import splrep, splev
     except ImportError:
         scipy = None
 
     th = np.arange(181)
     ph = np.array(
-        [1.0000e+00, 9.5960e-01, 9.2170e-01, 8.8590e-01,
-         8.5220e-01, 8.2050e-01, 7.9060e-01, 7.6240e-01,
-         7.3580e-01, 7.1070e-01, 6.8710e-01, 6.6470e-01,
-         6.4360e-01, 6.2370e-01, 6.0490e-01, 5.8720e-01,
-         5.7040e-01, 5.5460e-01, 5.3960e-01, 5.2550e-01,
-         5.1220e-01, 4.9960e-01, 4.8770e-01, 4.7650e-01,
-         4.6590e-01, 4.5590e-01, 4.4650e-01, 4.3770e-01,
-         4.2930e-01, 4.2150e-01, 4.1420e-01, 4.0730e-01,
-         4.0090e-01, 3.9490e-01, 3.8930e-01, 3.8400e-01,
-         3.7920e-01, 3.7470e-01, 3.7060e-01, 3.6680e-01,
-         3.6340e-01, 3.6030e-01, 3.5750e-01, 3.5400e-01,
-         3.5090e-01, 3.4820e-01, 3.4580e-01, 3.4380e-01,
-         3.4210e-01, 3.4070e-01, 3.3970e-01, 3.3890e-01,
-         3.3850e-01, 3.3830e-01, 3.3850e-01, 3.3890e-01,
-         3.3960e-01, 3.4050e-01, 3.4180e-01, 3.4320e-01,
-         3.4500e-01, 3.4700e-01, 3.4930e-01, 3.5180e-01,
-         3.5460e-01, 3.5760e-01, 3.6090e-01, 3.6450e-01,
-         3.6830e-01, 3.7240e-01, 3.7680e-01, 3.8150e-01,
-         3.8650e-01, 3.9170e-01, 3.9730e-01, 4.0320e-01,
-         4.0940e-01, 4.1590e-01, 4.2280e-01, 4.3000e-01,
-         4.3760e-01, 4.4560e-01, 4.5400e-01, 4.6270e-01,
-         4.7200e-01, 4.8160e-01, 4.9180e-01, 5.0240e-01,
-         5.1360e-01, 5.2530e-01, 5.3750e-01, 5.5040e-01,
-         5.6380e-01, 5.7800e-01, 5.9280e-01, 6.0840e-01,
-         6.2470e-01, 6.4190e-01, 6.5990e-01, 6.7880e-01,
-         6.9870e-01, 7.1960e-01, 7.4160e-01, 7.6480e-01,
-         7.8920e-01, 8.1490e-01, 8.4200e-01, 8.7060e-01,
-         9.0080e-01, 9.3270e-01, 9.6640e-01, 1.0021e+00,
-         1.0399e+00, 1.0799e+00, 1.1223e+00, 1.1673e+00,
-         1.2151e+00, 1.2659e+00, 1.3200e+00, 1.3776e+00,
-         1.4389e+00, 1.5045e+00, 1.5744e+00, 1.6493e+00,
-         1.7294e+00, 1.8153e+00, 1.9075e+00, 2.0066e+00,
-         2.1132e+00, 2.2281e+00, 2.3521e+00, 2.4861e+00,
-         2.6312e+00, 2.7884e+00, 2.9592e+00, 3.1450e+00,
-         3.3474e+00, 3.5685e+00, 3.8104e+00, 4.0755e+00,
-         4.3669e+00, 4.6877e+00, 5.0418e+00, 5.4336e+00,
-         5.8682e+00, 6.3518e+00, 6.8912e+00, 7.4948e+00,
-         8.1724e+00, 8.9355e+00, 9.7981e+00, 1.0777e+01,
-         1.1891e+01, 1.3166e+01, 1.4631e+01, 1.6322e+01,
-         1.8283e+01, 2.0570e+01, 2.3252e+01, 2.6418e+01,
-         3.0177e+01, 3.4672e+01, 4.0086e+01, 4.6659e+01,
-         5.4704e+01, 6.4637e+01, 7.7015e+01, 9.2587e+01,
-         1.1237e+02, 1.3775e+02, 1.7060e+02, 2.1348e+02,
-         2.6973e+02, 3.4359e+02, 4.3989e+02, 5.6292e+02,
-         7.1363e+02, 8.8448e+02, 1.0533e+03, 1.1822e+03,
-         1.2312e+03])
+        [
+            1.0000e00,
+            9.5960e-01,
+            9.2170e-01,
+            8.8590e-01,
+            8.5220e-01,
+            8.2050e-01,
+            7.9060e-01,
+            7.6240e-01,
+            7.3580e-01,
+            7.1070e-01,
+            6.8710e-01,
+            6.6470e-01,
+            6.4360e-01,
+            6.2370e-01,
+            6.0490e-01,
+            5.8720e-01,
+            5.7040e-01,
+            5.5460e-01,
+            5.3960e-01,
+            5.2550e-01,
+            5.1220e-01,
+            4.9960e-01,
+            4.8770e-01,
+            4.7650e-01,
+            4.6590e-01,
+            4.5590e-01,
+            4.4650e-01,
+            4.3770e-01,
+            4.2930e-01,
+            4.2150e-01,
+            4.1420e-01,
+            4.0730e-01,
+            4.0090e-01,
+            3.9490e-01,
+            3.8930e-01,
+            3.8400e-01,
+            3.7920e-01,
+            3.7470e-01,
+            3.7060e-01,
+            3.6680e-01,
+            3.6340e-01,
+            3.6030e-01,
+            3.5750e-01,
+            3.5400e-01,
+            3.5090e-01,
+            3.4820e-01,
+            3.4580e-01,
+            3.4380e-01,
+            3.4210e-01,
+            3.4070e-01,
+            3.3970e-01,
+            3.3890e-01,
+            3.3850e-01,
+            3.3830e-01,
+            3.3850e-01,
+            3.3890e-01,
+            3.3960e-01,
+            3.4050e-01,
+            3.4180e-01,
+            3.4320e-01,
+            3.4500e-01,
+            3.4700e-01,
+            3.4930e-01,
+            3.5180e-01,
+            3.5460e-01,
+            3.5760e-01,
+            3.6090e-01,
+            3.6450e-01,
+            3.6830e-01,
+            3.7240e-01,
+            3.7680e-01,
+            3.8150e-01,
+            3.8650e-01,
+            3.9170e-01,
+            3.9730e-01,
+            4.0320e-01,
+            4.0940e-01,
+            4.1590e-01,
+            4.2280e-01,
+            4.3000e-01,
+            4.3760e-01,
+            4.4560e-01,
+            4.5400e-01,
+            4.6270e-01,
+            4.7200e-01,
+            4.8160e-01,
+            4.9180e-01,
+            5.0240e-01,
+            5.1360e-01,
+            5.2530e-01,
+            5.3750e-01,
+            5.5040e-01,
+            5.6380e-01,
+            5.7800e-01,
+            5.9280e-01,
+            6.0840e-01,
+            6.2470e-01,
+            6.4190e-01,
+            6.5990e-01,
+            6.7880e-01,
+            6.9870e-01,
+            7.1960e-01,
+            7.4160e-01,
+            7.6480e-01,
+            7.8920e-01,
+            8.1490e-01,
+            8.4200e-01,
+            8.7060e-01,
+            9.0080e-01,
+            9.3270e-01,
+            9.6640e-01,
+            1.0021e00,
+            1.0399e00,
+            1.0799e00,
+            1.1223e00,
+            1.1673e00,
+            1.2151e00,
+            1.2659e00,
+            1.3200e00,
+            1.3776e00,
+            1.4389e00,
+            1.5045e00,
+            1.5744e00,
+            1.6493e00,
+            1.7294e00,
+            1.8153e00,
+            1.9075e00,
+            2.0066e00,
+            2.1132e00,
+            2.2281e00,
+            2.3521e00,
+            2.4861e00,
+            2.6312e00,
+            2.7884e00,
+            2.9592e00,
+            3.1450e00,
+            3.3474e00,
+            3.5685e00,
+            3.8104e00,
+            4.0755e00,
+            4.3669e00,
+            4.6877e00,
+            5.0418e00,
+            5.4336e00,
+            5.8682e00,
+            6.3518e00,
+            6.8912e00,
+            7.4948e00,
+            8.1724e00,
+            8.9355e00,
+            9.7981e00,
+            1.0777e01,
+            1.1891e01,
+            1.3166e01,
+            1.4631e01,
+            1.6322e01,
+            1.8283e01,
+            2.0570e01,
+            2.3252e01,
+            2.6418e01,
+            3.0177e01,
+            3.4672e01,
+            4.0086e01,
+            4.6659e01,
+            5.4704e01,
+            6.4637e01,
+            7.7015e01,
+            9.2587e01,
+            1.1237e02,
+            1.3775e02,
+            1.7060e02,
+            2.1348e02,
+            2.6973e02,
+            3.4359e02,
+            4.3989e02,
+            5.6292e02,
+            7.1363e02,
+            8.8448e02,
+            1.0533e03,
+            1.1822e03,
+            1.2312e03,
+        ]
+    )
 
-    _phase = np.abs(u.Quantity(phase, 'deg').value)
+    _phase = np.abs(u.Quantity(phase, "deg").value)
 
     if scipy:
         Phi = splev(_phase, splrep(th, ph))
     else:
-        warn(sbe.OptionalPackageUnavailable(
-            'scipy is not present, using linear interpolation.'))
+        warn(
+            sbe.OptionalPackageUnavailable(
+                "scipy is not present, using linear interpolation."
+            )
+        )
         Phi = np.interp(_phase, th, ph)
 
     if np.iterable(_phase):
         Phi = np.array(Phi).reshape(np.shape(_phase))
     else:
         Phi = float(Phi)
 
     return Phi
 
 
 # checks if the installed astropy version is up-to-date
 if astropy_version.major < 4:
+
     class DustComaQuantityMeta(InheritDocstrings, abc.ABCMeta):
         pass
+
 else:
     # astropy >= 4.0
     DustComaQuantityMeta = abc.ABCMeta
 
 
-class DustComaQuantity(u.SpecificTypeQuantity,
-                       metaclass=DustComaQuantityMeta):
-    """Abstract base class for dust coma photometric models: Afrho, Efrho.
-    """
+class DustComaQuantity(u.SpecificTypeQuantity, metaclass=DustComaQuantityMeta):
+    """Abstract base class for dust coma photometric models: Afrho, Efrho."""
+
     _equivalent_unit = u.meter
     _include_easy_conversion_members = False
 
     def __new__(cls, value, unit=None, dtype=None, copy=True):
-        return super().__new__(cls, value, unit=unit, dtype=dtype,
-                               copy=copy)
+        return super().__new__(cls, value, unit=unit, dtype=dtype, copy=copy)
 
     @classmethod
     def from_fluxd(cls, wfb, fluxd, aper, eph, **kwargs):
         """Initialize from spectral flux density.
 
 
         Parameters
@@ -212,16 +353,16 @@
             Optional: 'phase'.
 
         **kwargs
             Keyword arguments for `~to_fluxd`.
 
         """
 
-        fluxd1cm = cls(1 * u.cm).to_fluxd(wfb, aper, eph, unit=fluxd.unit,
-                                          **kwargs)
+        fluxd1cm = cls(1 * u.cm).to_fluxd(wfb, aper,
+                                          eph, unit=fluxd.unit, **kwargs)
 
         if isinstance(fluxd1cm, u.Magnitude):
             coma = cls((fluxd - fluxd1cm).physical * u.cm)
         else:
             coma = cls((fluxd / fluxd1cm).decompose() * u.cm)
 
         return coma
@@ -261,15 +402,15 @@
         # objects can needlessly increase the number of dimensions.
         if isinstance(aper, Aperture):
             rho = aper.coma_equivalent_radius()
             ndim = np.ndim(rho)
         else:
             rho = aper
             ndim = np.ndim(rho)
-        rho = rho.to('km', sbu.projected_size(eph))
+        rho = rho.to("km", sbu.projected_size(eph))
 
         ndim = max(ndim, np.ndim(self))
 
         # validate unit
         if unit is not None:
             unit = u.Unit(unit)
 
@@ -280,15 +421,15 @@
         # must have spectral flux density units
         source = self._source_fluxd(wfb, eph, unit=unit, **kwargs)
 
         if isinstance(source, u.Magnitude):
             _source = source.physical
         else:
             _source = source
-        fluxd = self * rho / eph['delta']**2 * _source
+        fluxd = self * rho / eph["delta"] ** 2 * _source
 
         # using Ephem can unnecessarily promote fluxd to an array
         if np.ndim(fluxd) > ndim:
             fluxd = np.squeeze(fluxd)
 
         # and back to magnitudes, as needed
         return fluxd.to(source.unit)
@@ -348,24 +489,26 @@
     ----------
     A'Hearn et al. 1984, AJ 89, 579-591.
 
 
     Examples
     --------
     >>> from sbpy.activity import Afrho
-    >>> print(Afrho(1000, 'cm'))
+    >>> print(Afrho(1000.0, 'cm'))
     1000.0 cm
 
     """
 
     @classmethod
     def from_fluxd(cls, wfb, fluxd, aper, eph, **kwargs):
         return super().from_fluxd(wfb, fluxd, aper, eph, **kwargs)
 
-    from_fluxd.__doc__ = DustComaQuantity.from_fluxd.__doc__ + """
+    from_fluxd.__doc__ = (
+        DustComaQuantity.from_fluxd.__doc__
+        + """
         Examples
         --------
         Convert observed flux density to Afρ, with a user-provided
         solar flux density for the V-band:
         >>> from sbpy.activity import Afrho
         >>> import astropy.units as u
         >>> from sbpy.calib import solar_fluxd
@@ -376,21 +519,22 @@
         >>> aper = 1 * u.arcsec
         >>> eph = dict(rh=1.5 * u.au, delta=1.0 * u.au)
         >>> afrho = Afrho.from_fluxd('V', fluxd, aper, eph=eph)
         >>> print(afrho)                        # doctest: +FLOAT_CMP
         999.9999999999999 cm
 
         """
+    )
 
-    def to_fluxd(self, wfb, aper, eph, unit=None, phasecor=False,
-                 Phi=None):
-        return super().to_fluxd(wfb, aper, eph, unit=unit, phasecor=phasecor,
-                                Phi=Phi)
+    def to_fluxd(self, wfb, aper, eph, unit=None, phasecor=False, Phi=None):
+        return super().to_fluxd(wfb, aper, eph, unit=unit, phasecor=phasecor, Phi=Phi)
 
-    to_fluxd.__doc__ = DustComaQuantity.to_fluxd.__doc__ + """
+    to_fluxd.__doc__ = (
+        DustComaQuantity.to_fluxd.__doc__
+        + """
         phasecor: bool, optional
             Scale the result by the phase function ``Phi``, assuming
             ``Afrho`` is quoted for 0° phase.  Requires phase angle in
             ``eph``.
 
         Phi : callable, optional
             Phase function, see :func:`~Afrho.to_phase`.
@@ -411,59 +555,62 @@
         >>> import astropy.units as u
         >>> afrho = Afrho(1000 * u.cm)
         >>> wave = 0.55 * u.um
         >>> aper = 1 * u.arcsec
         >>> eph = dict(rh=1.5 * u.au, delta=1.0 * u.au)
         >>> fluxd = afrho.to_fluxd(wave, aper, eph)
         >>> print(fluxd)    # doctest: +FLOAT_CMP
-        6.730018324465526e-14 W / (m2 um)
+        6.730018324465526e-14 W / (um m2)
 
         With a phase correction:
         >>> eph['phase'] = 30 * u.deg
         >>> fluxd = afrho.to_fluxd(wave, aper, eph, phasecor=True)
         >>> print(fluxd)    # doctest: +FLOAT_CMP
-        2.8017202649540757e-14 W / (m2 um)
+        2.8017202649540757e-14 W / (um m2)
 
         In magnitudes through the Johnson V filter:
         >>> import sbpy.units as sbu
         >>> from sbpy.photometry import bandpass
         >>> bp = bandpass('Johnson V')
         >>> fluxd = afrho.to_fluxd(bp, aper, eph, unit=sbu.JMmag,
         ...                     phasecor=True)
         >>> print(fluxd)    # doctest: +FLOAT_CMP
         15.321242371548918 mag(JM)
 
         """
+    )
 
-    @bib.cite({'model': '1984AJ.....89..579A'})
-    def _source_fluxd(self, wfb, eph, unit=None, phasecor=False,
-                      Phi=None, **kwargs):
+    @bib.cite({"model": "1984AJ.....89..579A"})
+    def _source_fluxd(self, wfb, eph, unit=None, phasecor=False, Phi=None, **kwargs):
         # get solar flux density
         sun = Sun.from_default()
         try:
             S = sun.observe(wfb, unit=unit, **kwargs)
         except SinglePointSpectrumError:
             S = sun(wfb, unit=unit)
 
-        if not (S.unit.is_equivalent(u.W / u.m**2 / u.um)
-                or S.unit.is_equivalent(u.W / u.m**2 / u.Hz)
-                or isinstance(S, u.Magnitude)):
+        if not (
+            S.unit.is_equivalent(u.W / u.m**2 / u.um)
+            or S.unit.is_equivalent(u.W / u.m**2 / u.Hz)
+            or isinstance(S, u.Magnitude)
+        ):
             raise ValueError(
-                'Solar flux density must have units of spectral flux '
-                'density, e.g., W/m2/μm or W/m2/Hz')
+                "Solar flux density must have units of spectral flux "
+                "density, e.g., W/m2/μm or W/m2/Hz"
+            )
 
         if phasecor:
             Phi = phase_HalleyMarcus if Phi is None else Phi
-            _Phi = Phi(eph['phase']) / Phi(0 * u.deg)
+            _Phi = Phi(eph["phase"]) / Phi(0 * u.deg)
         else:
             _Phi = 1
 
         # compute
         _S = S.physical if isinstance(S, u.Magnitude) else S
-        source = _S * _Phi / 4 * u.au**2 / eph['rh']**2
+        source = _S * _Phi / 4 * u.au**2 / eph["rh"] ** 2
 
         return source.to(S.unit)
 
     def to_phase(self, to_phase, from_phase, Phi=None):
         """Scale to another phase angle.
 
 
@@ -539,44 +686,47 @@
     A'Hearn et al. 1984, AJ 89, 579-591.
     Kelley et al. 2013, Icarus 225, 475-494.
 
 
     Examples
     --------
     >>> from sbpy.activity import Efrho
-    >>> print(Efrho(1000, 'cm'))
+    >>> print(Efrho(1000.0, 'cm'))
     1000.0 cm
 
     """
 
     @classmethod
     def from_fluxd(cls, wfb, fluxd, aper, eph, **kwargs):
         return super().from_fluxd(wfb, fluxd, aper, eph, **kwargs)
 
-    from_fluxd.__doc__ = DustComaQuantity.from_fluxd.__doc__ + """
+    from_fluxd.__doc__ = (
+        DustComaQuantity.from_fluxd.__doc__
+        + """
         Examples
         --------
         >>> from sbpy.activity import Efrho
         >>> import astropy.units as u
         >>> wave = 15.8 * u.um
         >>> fluxd = 6.52 * u.mJy
         >>> aper =  11.1 * u.arcsec
         >>> eph = {'rh': 4.42 * u.au, 'delta': 4.01 * u.au}
         >>> efrho = Efrho.from_fluxd(wave, fluxd, aper, eph=eph)
         >>> print(efrho)                          # doctest: +FLOAT_CMP
         120.00836963059808 cm
 
     """
+    )
 
-    def to_fluxd(self, wfb, aper, eph, unit=None, Tscale=1.1,
-                 T=None, B=None):
-        return super().to_fluxd(wfb, aper, eph, unit=unit, Tscale=Tscale,
-                                T=T, B=B)
+    def to_fluxd(self, wfb, aper, eph, unit=None, Tscale=1.1, T=None, B=None):
+        return super().to_fluxd(wfb, aper, eph, unit=unit, Tscale=Tscale, T=T, B=B)
 
-    to_fluxd.__doc__ = DustComaQuantity.to_fluxd.__doc__ + """
+    to_fluxd.__doc__ = (
+        DustComaQuantity.to_fluxd.__doc__
+        + """
         Tscale : float, optional
             Scale factor for blackbody in LTE with sunlight.  Ignored
             if ``T`` or ``B`` is provided.
 
         T : `~astropy.units.Quantity`, optional
             Blackbody temperature.  Ignored if ``B`` is provided.
 
@@ -601,28 +751,32 @@
         >>> aper = 11.1 * u.arcsec
         >>> eph = {'rh': 4.42 * u.au, 'delta': 4.01 * u.au}
         >>> fluxd = efrho.to_fluxd(freq, aper, eph=eph, unit='Jy')
         >>> print(fluxd)                           # doctest: +FLOAT_CMP
         0.006519545281786034 Jy
 
     """
+    )
 
-    @bib.cite({'model': '2013Icar..225..475K'})
+    @bib.cite({"model": "2013Icar..225..475K"})
     def _source_fluxd(self, wfb, eph, unit=None, Tscale=1.1, T=None, B=None):
         if T is None:
-            T = Tscale * 278 / np.sqrt(eph['rh'].to('au').value)
+            T = Tscale * 278 / np.sqrt(eph["rh"].to("au").value)
 
         if B is None:
             BB = BlackbodySource(T)
             try:
                 B = BB.observe(wfb, unit=unit)
             except SinglePointSpectrumError:
                 B = BB(wfb, unit=unit)
         else:
-            if not (B.unit.is_equivalent(u.W / u.m**2 / u.um)
-                    or B.unit.is_equivalent(u.W / u.m**2 / u.Hz)
-                    or isinstance(B, u.Magnitude)):
+            if not (
+                B.unit.is_equivalent(u.W / u.m**2 / u.um)
+                or B.unit.is_equivalent(u.W / u.m**2 / u.Hz)
+                or isinstance(B, u.Magnitude)
+            ):
                 raise ValueError(
-                    'B must be a magnitude or have units of spectral '
-                    'flux density, e.g., W/m2/μm or W/m2/Hz')
+                    "B must be a magnitude or have units of spectral "
+                    "flux density, e.g., W/m2/μm or W/m2/Hz"
+                )
 
         return B
```

### Comparing `sbpy-0.3.0/sbpy/activity/gas/core.py` & `sbpy-0.4.0/sbpy/activity/gas/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """activity.gas core
 
 """
 
 __all__ = [
-    'photo_lengthscale',
-    'photo_timescale',
-    'fluorescence_band_strength',
-    'Haser',
-    'VectorialModel'
+    "photo_lengthscale",
+    "photo_timescale",
+    "fluorescence_band_strength",
+    "Haser",
+    "VectorialModel",
 ]
 
 from abc import ABC, abstractmethod
+
+# distutils is deprecated in python 3.10 and will be removed in 3.12 (PEP 632).
+# Migration from distutils.log -> logging
 from distutils.log import warn
 import warnings
+from dataclasses import dataclass
+from typing import Callable, Tuple
 
 import numpy as np
 import astropy.units as u
 
 try:
     import scipy
     from scipy import special
@@ -26,16 +31,21 @@
 except ImportError:
     scipy = None
 
 from ... import bib
 from ... import data as sbd
 from ... import units as sbu
 from ...exceptions import RequiredPackageUnavailable, TestingNeeded
-from .. core import (Aperture, RectangularAperture, GaussianAperture,
-                     AnnularAperture, CircularAperture)
+from ..core import (
+    Aperture,
+    RectangularAperture,
+    GaussianAperture,
+    AnnularAperture,
+    CircularAperture,
+)
 
 
 def photo_lengthscale(species, source=None):
     """Photodissociation lengthscale for a gas species.
 
 
     Parameters
@@ -66,34 +76,34 @@
     Icarus 105, 235-253.  Quoted for intermediate solar activity.
 
     """
 
     from .data import photo_lengthscale as data
 
     default_sources = {
-        'H2O': 'CS93',
-        'OH': 'CS93',
+        "H2O": "CS93",
+        "OH": "CS93",
     }
 
     if species not in data:
-        summary = ''
+        summary = ""
         for k, v in sorted(data.items()):
-            summary += '\n{} [{}]'.format(k, ', '.join(v.keys()))
+            summary += "\n{} [{}]".format(k, ", ".join(v.keys()))
 
-        raise ValueError(
-            'Invalid species {}.  Choose from:{}'
-            .format(species, summary))
+        raise ValueError("Invalid species {}.  Choose from:{}".format(species, summary))
 
     gas = data[species]
     source = default_sources[species] if source is None else source
 
     if source not in gas:
         raise ValueError(
-            'Source key {} not available for {}.  Choose from: {}'
-            .format(source, species, ', '.join(gas.keys())))
+            "Source key {} not available for {}.  Choose from: {}".format(
+                source, species, ", ".join(gas.keys())
+            )
+        )
 
     gamma, bibcode = gas[source]
     bib.register(photo_lengthscale, bibcode)
 
     return gamma
 
 
@@ -135,40 +145,40 @@
     [H92] Huebner et al. 1992, Astroph. & Space Sci. 195, 1-294.
 
     """
 
     from .data import photo_timescale as data
 
     default_sources = {
-        'H2O': 'CS93',
-        'OH': 'CS93',
-        'HCN': 'C94',
-        'CH3OH': 'C94',
-        'H2CO': 'C94',
-        'CO2': 'CE83',
-        'CO': 'CE83',
-        'CN': 'H92'
+        "H2O": "CS93",
+        "OH": "CS93",
+        "HCN": "C94",
+        "CH3OH": "C94",
+        "H2CO": "C94",
+        "CO2": "CE83",
+        "CO": "CE83",
+        "CN": "H92",
     }
 
     if species not in data:
-        summary = ''
+        summary = ""
         for k, v in sorted(data.items()):
-            summary += '\n{} [{}]'.format(k, ', '.join(v.keys()))
+            summary += "\n{} [{}]".format(k, ", ".join(v.keys()))
 
-        raise ValueError(
-            "Invalid species {}.  Choose from:{}"
-            .format(species, summary))
+        raise ValueError("Invalid species {}.  Choose from:{}".format(species, summary))
 
     gas = data[species]
     source = default_sources[species] if source is None else source
 
     if source not in gas:
         raise ValueError(
-            'Source key {} not available for {}.  Choose from: {}'
-            .format(source, species, ', '.join(gas.keys())))
+            "Source key {} not available for {}.  Choose from: {}".format(
+                source, species, ", ".join(gas.keys())
+            )
+        )
 
     tau, bibcode = gas[source]
     bib.register(photo_timescale, bibcode)
 
     return tau
 
 
@@ -209,36 +219,40 @@
     [1.54e-15] erg / s
 
     """
 
     from .data import fluorescence_band_strength as data
 
     default_sources = {
-        'OH 0-0': 'SA88',
-        'OH 1-0': 'SA88',
-        'OH 1-1': 'SA88',
-        'OH 2-2': 'SA88',
-        'OH 0-1': 'SA88',
-        'OH 0-2': 'SA88',
-        'OH 2-0': 'SA88',
-        'OH 2-1': 'SA88',
+        "OH 0-0": "SA88",
+        "OH 1-0": "SA88",
+        "OH 1-1": "SA88",
+        "OH 2-2": "SA88",
+        "OH 0-1": "SA88",
+        "OH 0-2": "SA88",
+        "OH 2-0": "SA88",
+        "OH 2-1": "SA88",
     }
 
     if species not in data:
         raise ValueError(
-            'No data available for {}.  Choose one of: {}'
-            .format(species, ', '.join(data.keys())))
+            "No data available for {}.  Choose one of: {}".format(
+                species, ", ".join(data.keys())
+            )
+        )
 
     band = data[species]
     source = default_sources[species] if source is None else source
 
     if source not in band:
         raise ValueError(
-            'No source {} for {}.  Choose one of: {}'
-            .format(source, species, ', '.join(band.keys())))
+            "No source {} for {}.  Choose one of: {}".format(
+                source, species, ", ".join(band.keys())
+            )
+        )
 
     LN, note, bibcode = band[source]
     if bibcode is not None:
         bib.register(fluorescence_band_strength, bibcode)
 
     return LN(eph)
 
@@ -253,15 +267,15 @@
         Production rate, number per time.
 
     v : `~astropy.units.Quantity`
         Radial outflow speed, distance per time.
 
     """
 
-    @u.quantity_input(Q=(u.s ** -1, u.mol / u.s), v=u.m / u.s)
+    @u.quantity_input(Q=(u.s**-1, u.mol / u.s), v=u.m / u.s)
     def __init__(self, Q, v):
         self.Q = Q
         self.v = v
 
     @u.quantity_input(r=u.m)
     def volume_density(self, r):
         """Coma volume density.
@@ -276,18 +290,18 @@
         Returns
         -------
         n : `~astropy.units.Quantity`
             Local number density.
 
         """
 
-        return self._volume_density(r.to_value('m')) / u.m ** 3
+        return self._volume_density(r.to_value("m")) / u.m**3
 
     @sbd.dataclass_input(eph=sbd.Ephem)
-    @sbd.quantity_to_dataclass(eph=(sbd.Ephem, 'delta'))
+    @sbd.quantity_to_dataclass(eph=(sbd.Ephem, "delta"))
     def column_density(self, rho, eph=None):
         """Coma column density at a projected distance from nucleus.
 
 
         Parameters
         ----------
         rho : `~astropy.units.Quantity`
@@ -307,19 +321,19 @@
 
         """
 
         equiv = []
         if eph is not None:
             equiv = sbu.projected_size(eph)
 
-        rho = rho.to_value('m', equiv)
-        return self._column_density(rho) / u.m ** 2
+        rho = rho.to_value("m", equiv)
+        return self._column_density(rho) / u.m**2
 
     @sbd.dataclass_input(eph=sbd.Ephem)
-    @sbd.quantity_to_dataclass(eph=(sbd.Ephem, 'delta'))
+    @sbd.quantity_to_dataclass(eph=(sbd.Ephem, "delta"))
     def total_number(self, aper, eph=None):
         """Total number of molecules in aperture.
 
 
         Parameters
         ----------
         aper : `~astropy.units.Quantity`, `~sbpy.activity.Aperture`
@@ -424,26 +438,27 @@
 
         err : float
             Estimated integration error.
 
         """
 
         if not scipy:
-            raise RequiredPackageUnavailable('scipy')
+            raise RequiredPackageUnavailable("scipy")
 
         def f(s, rho2):
-            r = np.sqrt(rho2 + s ** 2)
+            r = np.sqrt(rho2 + s**2)
             return self._volume_density(r)
 
         # quad diverges integrating to infinity, but 1e6 × rho is good
         # enough
         limit = 30
         points = rho * np.logspace(-4, 4, limit // 2)
-        sigma, err = quad(f, 0, 1e6 * rho, args=(rho ** 2,),
-                          limit=limit, points=points, epsabs=epsabs)
+        sigma, err = quad(
+            f, 0, 1e6 * rho, args=(rho**2,), limit=limit, points=points, epsabs=epsabs
+        )
 
         # spherical symmetry
         sigma *= 2
         err *= 2
 
         return sigma, err
 
@@ -469,36 +484,36 @@
 
         err : float
             Estimated integration error.
 
         """
 
         if not scipy:
-            raise RequiredPackageUnavailable('scipy')
+            raise RequiredPackageUnavailable("scipy")
 
         if isinstance(aper, (CircularAperture, AnnularAperture)):
             if isinstance(aper, CircularAperture):
-                limits = (0, aper.radius.to_value('m'))
+                limits = (0, aper.radius.to_value("m"))
             else:
-                limits = aper.shape.to_value('m')
+                limits = aper.shape.to_value("m")
 
             # integrate in polar coordinates
             def f(rho):
                 """Column density integration in polar coordinates.
 
                 rho in m, column_density in m**-2
 
                 """
                 return rho * self._column_density(rho)
 
             N, err = quad(f, *limits, epsabs=epsabs)
             N *= 2 * np.pi
             err *= 2 * np.pi
         elif isinstance(aper, RectangularAperture):
-            shape = aper.shape.to_value('m')
+            shape = aper.shape.to_value("m")
 
             def f(rho, th):
                 """Column density integration in polar coordinates.
 
                 rho in m, column_density in m**-2
 
                 th is ignored (azimuthal symmetry)
@@ -534,18 +549,21 @@
             # integrate in polar coordinates
             def f(rho, sigma):
                 """Column density integration in polar coordinates.
 
                 rho and sigma in m, column_density in m**-2
 
                 """
-                return (rho * np.exp(-rho ** 2 / sigma ** 2 / 2)
-                        * self._column_density(rho))
+                return (
+                    rho
+                    * np.exp(-(rho**2) / sigma**2 / 2)
+                    * self._column_density(rho)
+                )
 
-            sigma = aper.sigma.to_value('m')
+            sigma = aper.sigma.to_value("m")
             N, err = quad(f, 0, np.inf, args=(sigma,), epsabs=epsabs)
             N *= 2 * np.pi
             err *= 2 * np.pi
 
         return N, err
 
 
@@ -575,169 +593,398 @@
     Haser 1957, Bulletin de la Societe Royale des Sciences de Liege
     43, 740.
 
     Newburn and Johnson 1978, Icarus 35, 360-368.
 
     """
 
-    @bib.cite({'model': '1957BSRSL..43..740H'})
+    @bib.cite({"model": "1957BSRSL..43..740H"})
     @u.quantity_input(parent=u.m, daughter=u.m)
     def __init__(self, Q, v, parent, daughter=None):
         super().__init__(Q, v)
         self.parent = parent
         self.daughter = daughter
 
     def _volume_density(self, r):
-        n = (self.Q / self.v).to_value('1/m') / r ** 2 / 4 / np.pi
-        parent = self.parent.to_value('m')
+        n = (self.Q / self.v).to_value("1/m") / r**2 / 4 / np.pi
+        parent = self.parent.to_value("m")
         if self.daughter is None or self.daughter == 0:
             # parent only
             n *= np.exp(-r / parent)
         else:
-            daughter = self.daughter.to_value('m')
-            n *= (daughter / (parent - daughter)
-                  * (np.exp(-r / parent) - np.exp(-r / daughter)))
+            daughter = self.daughter.to_value("m")
+            n *= (
+                daughter
+                / (parent - daughter)
+                * (np.exp(-r / parent) - np.exp(-r / daughter))
+            )
 
         return n
 
     def _iK0(self, x):
         """Integral of the modified Bessel function of 2nd kind, 0th order."""
         if not scipy:
-            raise RequiredPackageUnavailable('scipy')
+            raise RequiredPackageUnavailable("scipy")
         return special.iti0k0(x)[1]
 
     def _K1(self, x):
         """Modified Bessel function of 2nd kind, 1st order."""
         if not scipy:
-            raise RequiredPackageUnavailable('scipy')
+            raise RequiredPackageUnavailable("scipy")
         return special.k1(x)
 
-    @bib.cite({'model': '1978Icar...35..360N'})
+    @bib.cite({"model": "1978Icar...35..360N"})
     def _column_density(self, rho):
-        sigma = (self.Q / self.v).to_value('1/m') / rho / 2 / np.pi
-        parent = self.parent.to_value('m')
+        sigma = (self.Q / self.v).to_value("1/m") / rho / 2 / np.pi
+        parent = self.parent.to_value("m")
         if self.daughter is None or self.daughter == 0:
             sigma *= np.pi / 2 - self._iK0(rho / parent)
         else:
-            daughter = self.daughter.to_value('m')
-            sigma *= (daughter / (parent - daughter)
-                      * (self._iK0(rho / daughter) - self._iK0(rho / parent)))
+            daughter = self.daughter.to_value("m")
+            sigma *= (
+                daughter
+                / (parent - daughter)
+                * (self._iK0(rho / daughter) - self._iK0(rho / parent))
+            )
         return sigma
 
     def _total_number(self, aper):
         # Inspect aper and handle as appropriate
         if isinstance(aper, (RectangularAperture, GaussianAperture)):
             return self._integrate_column_density(aper)[0]
         elif isinstance(aper, AnnularAperture):
             N0 = self._total_number(CircularAperture(aper.shape[0]))
             N1 = self._total_number(CircularAperture(aper.shape[1]))
             return N1 - N0
 
         # Solution for the circular aperture of radius rho:
-        bib.register(self.total_number, {'model': '1978Icar...35..360N'})
+        bib.register(self.total_number, {"model": "1978Icar...35..360N"})
 
         rho = aper.radius
         parent = self.parent.to(rho.unit)
         x = (rho / parent).to_value(u.dimensionless_unscaled)
         N = (self.Q * rho / self.v).to_value(u.dimensionless_unscaled)
         if self.daughter is None or self.daughter == 0:
             N *= 1 / x - self._K1(x) + np.pi / 2 - self._iK0(x)
         else:
             daughter = self.daughter.to(rho.unit)
-            y = (rho / daughter).to_value('')
-            N *= ((daughter / (parent - daughter)).to_value('')
-                  * (self._iK0(y) - self._iK0(x) + x ** -1 - y ** -1
-                     + self._K1(y) - self._K1(x)))
+            y = (rho / daughter).to_value("")
+            N *= (daughter / (parent - daughter)).to_value("") * (
+                self._iK0(y)
+                - self._iK0(x)
+                + x**-1
+                - y**-1
+                + self._K1(y)
+                - self._K1(x)
+            )
 
         return N
 
 
+@dataclass
+class VMParent:
+    """
+    Physical information about the parent necessary for the vectorial model
+
+    Parameters
+    ----------
+    v_outflow : float
+        See VectorialModel documentation.
+
+    tau_d : float
+        See VectorialModel documentation.
+
+    tau_T : float
+        See VectorialModel documentation.
+
+    sigma : float
+        See VectorialModel documentation.
+    """
+    v_outflow: float
+    tau_d: float
+    tau_T: float
+    sigma: float
+
+
+@dataclass
+class VMFragment:
+    """
+    Physical information about the fragment necessary for the vectorial model
+
+    Parameters
+    ----------
+    v_photo : float
+        See VectorialModel documentation.
+
+    tau_T : float
+        See VectorialModel documentation.
+    """
+    v_photo: float
+    tau_T: float
+
+
+@dataclass
+class VMGridParams:
+    """
+    Vectorial model gridding parameters to control how finely the space around
+    the comet should be gridded, and how detailed the outflow sampling should
+    be.
+
+    Parameters
+    ----------
+    radial_points : int
+        See VectorialModel documentation.
+
+    angular_points : int
+        See VectorialModel documentation.
+
+    radial_substeps : int
+        See VectorialModel documentation.
+    """
+    radial_points: int
+    angular_points: int
+    radial_substeps: int
+
+
+@dataclass
+class VMParams:
+    """
+    Vectorial model parameters unrelated to physical inputs, dealing with the
+    model's assumptions and detalis of the calculations.
+
+    Parameters
+    ----------
+    parent_destrution_level : float
+        See VectorialModel documentation.
+
+    fragment_destruction_level : float
+        See VectorialModel documentation.
+
+    max_fragment_lifetimes : float
+        See VectorialModel documentation.
+    """
+    parent_destruction_level: float
+    fragment_destruction_level: float
+    max_fragment_lifetimes: float
+
+
+@dataclass
+class VMFragmentSputterPolar:
+    """
+    Describes the distribution of fragment volume density
+    (``fragment_density[i][j]``) as function of (``rs[i]``, ``thetas[j]``) in a
+    spherical coordinate system, given a column of parent molecules flowing
+    outward along the azimuthal (z) axis.
+
+    Parameters
+    ----------
+    rs : `np.ndarray`
+        List of radii (`astropy.units.Quantity`).
+
+    thetas: `np.ndarray`
+        List of polar angles theta (radians) in a spherical coordinate system.
+
+    fragment_density: `np.ndarray`
+        List of fragment densities at the corresponding ``rs[i]`` and
+        ``thetas[j]``.
+    """
+    rs: np.ndarray
+    thetas: np.ndarray
+    fragment_density: np.ndarray
+
+
+@dataclass
+class VMResult:
+    """
+    Dataclass to hold a collection of vectorial model details and results in a
+    language- and model-independent way.
+
+    Parameters
+    ----------
+    volume_density_grid : `np.ndarray`
+        List of radii (`~astropy.units.Quantity`) that the model used for
+        volume density calculations.
+
+    volume_density : `np.ndarray`
+        List of volume densities (`~astropy.units.Quantity`) computed at the
+        corresponding radius: at radius = ``volume_density_grid[i]``, the volume
+        density is ``volume_density[i]``.
+
+    column_density_grid : `np.ndarray`
+        List of radii (`~astropy.units.Quantity`) that the model used for
+        column density calculations.
+
+    column_density : `np.ndarray`
+        List of column densities (`~astropy.units.Quantity`), computed at the
+        corresponding radius: at radius = ``column_density_grid[i]``, the column
+        density is ``column_density[i]``.
+
+    fragment_sputter : `VMFragmentSputterPolar`
+        Describes the distribution of fragment volume density as function of
+        (r, theta) in a spherical coordinate system, given a column of parent
+        molecules flowing outward along the azimuthal (z) axis.
+
+    solid_angle_sputter : `VMFragmentSputterPolar`
+        Similar to ``fragment_sputter``, but adjusted by a factor of
+        ``sin(theta)``.
+
+    volume_density_interpolation : `scipy.interpolate.PPoly`
+        Function that takes radius as a float in meters (no astropy units) and
+        returns the volume density in 1/m^3.  Not reliable beyond
+        ``max_grid_radius``, and questionable for radii less than
+        ``collision_sphere_radius``.
+
+    column_density_interpolation : `scipi.interpolate.PPoly`
+        Function that takes radius as a float in meters (no astropy units) and
+        returns the column density in 1/m^2.  Not relaible beyond
+        ``max_grid_radius``, and questionable for radii less than
+        ``collision_sphere_radius``.
+
+    collision_sphere_radius : `astropy.units.Quantity`
+        The radius of the collision sphere as described and calculated in
+        Festou (1981): the radius beyond which a molecule can expect to see one
+        collision over its lifetime.
+
+    max_grid_radius : `astropy.units.Quantity`
+        Cutoff radius for the model calculations.  Attempting to take results
+        from the model beyond this radius will be wrong or unreliable at best.
+
+    coma_radius : `astropy.units.Quantity`
+        Cutoff radius beyond which we take the parents to be entirely
+        dissociated.
+
+    num_fragments_theory : `float`
+        Total number of fragments that we expect based on a steady-state
+        calculation.  Unreliable when time dependence is strong.
+
+    num_fragments_grid : `float`
+        Total number of fragments based on the actual results of the model.
+        Agreement with ``num_fragments_theory`` is generally very good in the
+        steady-state case.
+
+    t_perm_flow : `float`
+        Time for the comet to reach a steady state/permanent flow regime, where
+        the number of fragments produced is equal to the number of fragments
+        lost to dissociation.  In a time-dependent production context, this
+        will also measure how long the effects of a single outburst can affect
+        the density.
+    """
+    volume_density_grid: np.ndarray = None
+    volume_density: np.ndarray = None
+    column_density_grid: np.ndarray = None
+    column_density: np.ndarray = None
+
+    fragment_sputter: VMFragmentSputterPolar = None
+    solid_angle_sputter: VMFragmentSputterPolar = None
+
+    volume_density_interpolation: scipy.interpolate.PPoly = None
+    column_density_interpolation: scipy.interpolate.PPoly = None
+
+    collision_sphere_radius: u.Quantity = None
+    max_grid_radius: u.Quantity = None
+    coma_radius: u.Quantity = None
+
+    num_fragments_theory: float = None
+    num_fragments_grid: float = None
+    t_perm_flow: u.Quantity = None
+
+
 class VectorialModel(GasComa):
-    """ Vectorial model for fragments in a coma produced
-         with a dissociative energy kick
+    """
+    Vectorial model for fragments in a coma produced with a dissociative energy
+    kick.
 
-        Parameters
-        ----------
-        base_q : `~astropy.units.Quantity`
-            Base production rate, per time
 
-        parent: `~sbpy.data.Phys`
-            Object with the following physical property fields:
-                * ``tau_T``: total lifetime of the parent molecule
-                * ``tau_d``: photodissociative lifetime of the parent molecule
-                * ``v_outflow``: outflow velocity of the parent molecule
-                * ``sigma``: cross-sectional area of the parent molecule
+    Parameters
+    ----------
+    base_q : `~astropy.units.Quantity`
+        Base production rate, per time
+
+    parent: `~sbpy.data.Phys`
+        Object with the following physical property fields:
+            * ``tau_T``: total lifetime of the parent molecule
+            * ``tau_d``: photodissociative lifetime of the parent molecule
+            * ``v_outflow``: outflow velocity of the parent molecule
+            * ``sigma``: cross-sectional area of the parent molecule
+
+    fragment: `~sbpy.data.Phys`
+        Object with the following physical property fields:
+            * ``tau_T``: total lifetime of the fragment molecule
+            * ``v_photo``: velocity of fragment resulting from
+                photodissociation of the parent
+
+    q_t: callable, optional
+        Calculates the parent production rate as a function of time: ``q_t(t)``.
+        The argument ``t`` is the look-back time as a float in units of seconds.
+        The return value is the production rate in units of inverse seconds.  If
+        provided, this value is added to ``base_q``.
+
+        If no time-dependence function is given, the model will run with steady
+        production at ``base_q`` stretching infinitely far into the past.
+
+    radial_points: int, optional
+        Number of radial grid points the model will use
+
+    radial_substeps: int, optional
+        Number of points along the outflow axis to integrate over
+
+    angular_points: int, optional
+        Number of angular grid points the model will use
+
+    parent_destruction_level: float, optional
+        Model will attempt to track parents until this percentage has
+        dissociated
+
+    fragment_destruction_level: float, optional
+        Model will attempt to track fragments until this percentage has
+        dissociated
+
+    max_fragment_lifetimes: float, optional
+        Fragments traveling through the coma will be ignored if they take longer
+        than this to arrive and contribute to the density at any considered
+        point.
+
+    print_progress: bool, optional
+        Print progress while calculating.
+
+
+    References
+    ----------
+    The density distribution of neutral compounds in cometary atmospheres. I -
+    Models and equations, Festou, M. C. 1981, Astronomy and Astrophysics, vol.
+    95, no. 1, Feb. 1981, p. 69-79.
 
-        fragment: `~sbpy.data.Phys`
-            Object with the following physical property fields:
-                * ``tau_T``: total lifetime of the fragment molecule
-                * ``v_photo``: velocity of fragment resulting from
-                    photodissociation of the parent
-
-        q_t: callable, optional
-            Calculates the parent production rate as a function of time:
-            ``q_t(t)``. The argument ``t`` is the look-back time as a float
-            in units of seconds.  The return value is the production rate in
-            units of inverse seconds.  If provided, this value is added to
-            ``base_q``.
-
-            If no time-dependence function is given, the model will run with
-            steady production at ``base_q`` stretching infinitely far into the
-            past.
-
-        radial_points: int, optional
-            Number of radial grid points the model will use
-
-        radial_substeps: int, optional
-            Number of points along the contributing axis to integrate over
-
-        angular_points: int, optional
-            Number of angular grid points the model will use
-
-        angular_substeps: int, optional
-            Number of angular steps per radial substep to integrate over
-
-        parent_destruction_level: float, optional
-            Model will attempt to track parents until
-            this percentage has dissociated
-
-        fragment_destruction_level: float, optional
-            Model will attempt to track fragments until
-            this percentage has dissociated
-
-        max_fragment_lifetimes: float, optional
-            Fragments traveling through the coma will be ignored if they take
-            longer than this to arrive and contribute to the density at any
-            considered point
-
-        print_progress: bool, optional
-            Print progress percentage while calculating
-
-        References:
-            The density distribution of neutral compounds in cometary
-            atmospheres. I - Models and equations,
-            Festou, M. C. 1981, Astronomy and Astrophysics, vol. 95, no. 1,
-            Feb. 1981, p. 69-79.
     """
-    @bib.cite({'model': '1981A&A....95...69F'})
-    @u.quantity_input(base_q=(u.s ** -1, u.mol / u.s))
-    def __init__(self, base_q, parent, fragment, q_t=None, radial_points=50,
-                 radial_substeps=12, angular_points=30, angular_substeps=7,
-                 parent_destruction_level=0.99,
-                 fragment_destruction_level=0.95,
-                 max_fragment_lifetimes=8.0,
-                 print_progress=False):
-
-        warnings.warn("Literature tests with the Vectorial model are generally"
-                      " in agreement at the 20% level or better.  The cause"
-                      " for the differences with the Festou FORTRAN code are"
-                      " not yet precisely known.  Help testing this feature is"
-                      " appreciated.", TestingNeeded)
 
-        super().__init__(base_q, parent['v_outflow'][0])
+    @bib.cite({"model": "1981A&A....95...69F"})
+    @u.quantity_input(base_q=(u.s**-1, u.mol / u.s))
+    def __init__(
+        self,
+        base_q,
+        parent,
+        fragment,
+        q_t=None,
+        radial_points=50,
+        radial_substeps=80,
+        angular_points=30,
+        parent_destruction_level=0.99,
+        fragment_destruction_level=0.95,
+        max_fragment_lifetimes=8.0,
+        print_progress=False,
+    ):
+        # warnings.warn(
+        #     "Literature tests with the Vectorial model are generally"
+        #     " in agreement at the 20% level or better.  The cause"
+        #     " for the differences with the Festou FORTRAN code are"
+        #     " not yet precisely known.  Help testing this feature is"
+        #     " appreciated.",
+        #     TestingNeeded,
+        # )
+
+        super().__init__(base_q, parent["v_outflow"][0])
 
         # Calculations are done internally in meters and seconds to match the
         # base GasComa class
 
         # Convert to unitless value of production per second
         self.base_q = base_q.to(1 / u.s).value
 
@@ -745,761 +992,843 @@
         if q_t is None:
             self.q_t = self._make_steady_production()
         else:
             self.q_t = q_t
 
         # Copy parent info, stripping astropy units and converting to meters
         # and seconds
-        self.parent = {
-            'tau_T': parent['tau_T'][0].to(u.s).value,
-            'tau_d': parent['tau_d'][0].to(u.s).value,
-            'v_outflow': parent['v_outflow'][0].to(u.m / u.s).value,
-            'sigma': parent['sigma'][0].to(u.m ** 2).value
-        }
+        self.parent = VMParent(
+            tau_T=parent["tau_T"][0].to(u.s).value,
+            tau_d=parent["tau_d"][0].to(u.s).value,
+            v_outflow=parent["v_outflow"][0].to(u.m / u.s).value,
+            sigma=parent["sigma"][0].to(u.m**2).value,
+        )
 
         # Same for the fragment info
-        self.fragment = {
-            'tau_T': fragment['tau_T'][0].to(u.s).value,
-            'v_photo': fragment['v_photo'][0].to(u.m / u.s).value
-        }
+        self.fragment = VMFragment(
+            tau_T=fragment["tau_T"][0].to(u.s).value,
+            v_photo=fragment["v_photo"][0].to(u.m / u.s).value,
+        )
 
         # Grid settings
-        self.radial_points = radial_points
-        self.radial_substeps = radial_substeps
-        self.angular_points = angular_points
-        self.angular_substeps = angular_substeps
-
-        # Helps define cutoff for radial grid at this percentage of parents
-        # lost to decay
-        self.parent_destruction_level = parent_destruction_level
-        # Default here is lower than parents because they are born farther from
-        # nucleus, tracking them too long will stretch the radial grid a bit
-        # too much
-        self.fragment_destruction_level = fragment_destruction_level
-
-        # If a fragment has to travel longer than this many lifetimes to
-        # contribute to the density at a point, ignore it
-        self.max_fragment_lifetimes = max_fragment_lifetimes
+        self.grid = VMGridParams(
+            radial_points=radial_points,
+            radial_substeps=radial_substeps,
+            angular_points=angular_points,
+        )
+
+        self.model_params = VMParams(
+            # Helps define cutoff for radial grid at this percentage of parents
+            # lost to decay
+            parent_destruction_level=parent_destruction_level,
+            # Default here is lower than parents because they are born farther
+            # from nucleus, tracking them too long will stretch the radial grid
+            # a bit too much
+            fragment_destruction_level=fragment_destruction_level,
+            # If a fragment has to travel longer than this many lifetimes to
+            # contribute to the density at a point, ignore it
+            max_fragment_lifetimes=max_fragment_lifetimes,
+        )
 
-        # Print progress during density calculations?
         self.print_progress = print_progress
 
-        """Initialize data structures to hold our calculations"""
-        self.vmodel = {}
+        self.vmr = VMResult()
 
         # Calculate up a few things
         self._setup_calculations()
 
         # Build the radial grid
-        self.vmodel['fast_radial_grid'] = self._make_radial_logspace_grid()
-        self.vmodel['radial_grid'] = self.vmodel['fast_radial_grid'] * (u.m)
+        self.fast_voldens_grid = self._make_radial_logspace_grid()
+        self.vmr.volume_density_grid = self.fast_voldens_grid * (u.m)
 
         # Angular grid
-        self.vmodel['d_alpha'] = self.vmodel[
-            'epsilon_max'] / self.angular_points
+        self.d_alpha = self.epsilon_max / self.grid.angular_points
         # Make array of angles adjusted up away from zero, to keep from
-        # calculating a radial line's contribution to itself
-        self.vmodel['angular_grid'] = np.linspace(
-            0, self.vmodel['epsilon_max'], num=self.angular_points,
-            endpoint=False
+        # encroaching on the outflow axis
+        self.angular_grid = np.linspace(
+            0, self.epsilon_max, num=self.grid.angular_points, endpoint=False
         )
-        # This maps addition over the whole array automatically
-        self.vmodel['angular_grid'] += self.vmodel['d_alpha'] / 2
+        self.angular_grid += self.d_alpha / 2
 
         # Makes a 2d array full of zero values
-        self.vmodel['density_grid'] = np.zeros((self.radial_points,
-                                                self.angular_points))
+        self.fragment_sputter = np.zeros(
+            (self.grid.radial_points, self.grid.angular_points)
+        )
 
         # Do the main computation
         self._compute_fragment_density()
 
-        # Turn our grid into a function of r
-        self._interpolate_radial_density()
+        # Turn our volume density into a function of r
+        self._interpolate_volume_density()
 
         # Get the column density at our grid points and interpolate
         self._compute_column_density()
 
         # Count up the number of fragments in the grid versus theoretical value
-        self.vmodel['num_fragments_theory'] = self.calc_num_fragments_theory()
-        self.vmodel['num_fragments_grid'] = self.calc_num_fragments_grid()
+        self.vmr.num_fragments_theory = self._calc_num_fragments_theory()
+        self.vmr.num_fragments_grid = self._calc_num_fragments_grid()
+
+        # Convert fragment sputters to group of one-dimensional arrays
+        # of the form r_i, theta_i, fragment_density_i
+        sputterlist = []
+        for (i, j), frag_dens in np.ndenumerate(self.fragment_sputter):
+            sputterlist.append(
+                [
+                    self.vmr.volume_density_grid[i].to(u.m).value,
+                    self.angular_grid[j],
+                    frag_dens,
+                ]
+            )
+        sputter = np.array(sputterlist)
+        # fill in the fragment sputter results
+        self.vmr.fragment_sputter = VMFragmentSputterPolar(
+            rs=sputter[:, 0] * u.m,
+            thetas=sputter[:, 1],
+            fragment_density=sputter[:, 2] / u.m**3,
+        )
+        normsputterlist = []
+        for (i, j), norm_dens in np.ndenumerate(self.solid_angle_sputter):
+            normsputterlist.append(
+                [
+                    self.vmr.volume_density_grid[i].to(u.m).value,
+                    self.angular_grid[j],
+                    norm_dens,
+                ]
+            )
+        normsputter = np.array(normsputterlist)
+        self.vmr.solid_angle_sputter = VMFragmentSputterPolar(
+            rs=normsputter[:, 0] * u.m,
+            thetas=normsputter[:, 1],
+            fragment_density=normsputter[:, 2] / u.m**3,
+        )
+
+        if print_progress:
+            print("Vectorial model calculations complete!")
 
     @classmethod
     def binned_production(cls, qs, fragment, parent, ts, **kwargs):
-        """ Alternate constructor for vectorial model
+        """Alternate constructor for vectorial model
+
+
+        Parameters
+        ----------
+        qs : `~astropy.units.Quantity`
+            List of steady production rates, per time, with length equal to that
+            of ``ts``.
+
+        parent: `~sbpy.data.Phys`
+            Same as __init__
+
+        fragment: `~sbpy.data.Phys`
+            Same as __init__
+
+        ts : `~astropy.units.Quantity`
+            List of times corresponding to when the production qs begin, with
+            positive times indicating the past.
+
+        kwargs: variable, optional
+            Any additional parameters in kwargs are passed on to __init__, which
+            are documented above and may be passed in here.
+
+
+        Returns
+        -------
+        VectorialModel
+            Instance of the VectorialModel class
+
+
+        Examples
+        --------
+        This specifies that from 30 days ago to 7 days ago, the production was
+        1.e27, changes to 3.e27 between 7 and 5 days ago, then falls to 2.e27
+        from 5 days ago until now: >>> q_example = [1.e27, 3.e27, 1.e27] *
+        (1/u.s) >>> t_example = [30, 7, 5] * u.day
+
+
+        Notes
+        -----
+        Preserves Festou's original fortran method of describing time dependence
+        in the model - time bins of steady production at specified intervals.
+
+        The base production of the model is taken from the first element in the
+        production array, which assumes the arrays are time-ordered from oldest
+        to most recent.  The base production extends backward in time to
+        infinity, so take care when using this method for time dependence if
+        that is not what is intended.
+
+        """
+
+        return cls(
+            base_q=qs[0],
+            q_t=VectorialModel._make_binned_production(qs, ts),
+            fragment=fragment,
+            parent=parent,
+            **kwargs
+        )
+
+    def _make_binned_production(qs, ts) -> Callable[[np.float64], np.float64]:
+        """Produces a time dependence function out of lists given to
+        binned_production constructor.
+
+
+        Parameters
+        ----------
+        qs : `astropy.units.Quantity`
+            See binned_production for description
+
+        ts : `astropy.units.Quantity`
+            See binned_production for description
+
+
+        Returns
+        -------
+        q_t : function
+            See __init__ for description
+
+
+        Notes
+        -----
+        We create a model-compatible function for time dependence out of the
+        information specified in the arrays qs and ts The resulting function
+        gives a steady specified production within the given time windows.
 
-            Parameters
-            ----------
-            qs : `~astropy.units.Quantity`
-                List of steady production rates, per time, with length equal to
-                that of ``ts``.
-
-            parent: `~sbpy.data.Phys`
-                Same as __init__
-
-            fragment: `~sbpy.data.Phys`
-                Same as __init__
-
-            ts : `~astropy.units.Quantity`
-                List of times corresponding to when the production qs begin,
-                with positive times indicating the past.
-
-            kwargs: variable, optional
-                Any additional parameters in kwargs are passed on to __init__,
-                which are documented above and may be passed in here.
-
-            Returns
-            -------
-            VectorialModel
-                Instance of the VectorialModel class
-
-            Examples
-            --------
-            This specifies that from 30 days ago to 7 days ago, the production
-            was 1.e27, changes to 3.e27 between 7 and 5 days ago, then falls to
-            2.e27 from 5 days ago until now
-            >>> q_example = [1.e27, 3.e27, 1.e27] * (1/u.s)
-            >>> t_example = [30, 7, 5] * u.day
-
-            Notes
-            -----
-            Preserves Festou's original fortran method of describing time
-            dependence in the model - time bins of steady production at
-            specified intervals
-
-            The base production of the model is taken from the first element in
-            the production array, which assumes the arrays are time-ordered
-            from oldest to most recent.  The base production extends backward
-            in time to infinity, so take care when using this method for time
-            dependence if that is not what is intended.
-        """
-        return cls(base_q=qs[0],
-                   q_t=VectorialModel._make_binned_production(qs, ts),
-                   fragment=fragment, parent=parent, **kwargs)
-
-    def _make_binned_production(qs, ts):
-        """ Produces a time dependence function out of lists given to
-            binned_production constructor
-
-            Parameters
-            ----------
-            qs : `astropy.units.Quantity`
-                See binned_production for description
-
-            ts : `astropy.units.Quantity`
-                See binned_production for description
-
-            Returns
-            -------
-            q_t : function
-                See __init__ for description
-
-            Notes
-            -----
-            We create a model-compatible function for time dependence out of
-            the information specified in the arrays qs and ts
-            The resulting function gives a steady specified production within
-            the given time windows
         """
 
-        q_invsecs = qs.to(1 / (u.s)).value
-        t_at_p_secs = ts.to(u.s).value
         base_q = qs[0]
+        q_variations = qs - base_q
+
+        q_invsecs = q_variations.to_value(1 / (u.s))
+        t_at_p_secs = ts.to_value(u.s)
 
         # extend the arrays to simplify our comparisons in binned_q_t
         # last bin stops at observation time, t = 0
         t_at_p_secs = np.append(t_at_p_secs, [0])
         # junk value for production because this is in the future
         q_invsecs = np.append(q_invsecs, [0])
 
+        # this function represents the deviation from base_q at any time t, so
+        # we need to handle times outside of the range specified in 'ts'
         def q_t(t):
             # too long in the past?
-            if t > t_at_p_secs[0] or t < 0:
-                return base_q
+            if t > t_at_p_secs[0]:
+                return 0
             # in the future?
             if t < 0:
                 return 0
 
-            # loop over all elements except the last so we can always look at
-            # [index+1] for the comparison
+            # find which bin the given time falls in, and return the
+            # corresponding production for that interval
             for i in range(len(q_invsecs) - 1):
                 if t < t_at_p_secs[i] and t > t_at_p_secs[i + 1]:
                     return q_invsecs[i]
 
         return q_t
 
-    def _make_steady_production(self):
-        """ Produces a time dependence function that contributes no extra
-            parents at any time
-
-            Notes
-            -----
-            If no q_t is given, we use this as our time dependence as the
-            model needs a q_t to run
+    def _make_steady_production(self) -> Callable[[np.float64], np.float64]:
+        """Produces a time dependence function that contributes no extra
+        parents at any time.
+
+
+        Returns
+        -------
+        q_t : function
+            See __init__ for description
+
+
+        Notes
+        -----
+        If no q_t is given, we use this as our time dependence as the
+        model needs a q_t to run
+
         """
+
         # No additional production at any time
-        def q_t(t):
-            return 0
+        def q_t(_):
+            return 0.0
 
         return q_t
 
-    def _setup_calculations(self):
-        """ Miscellaneus calculations to inform the model later
+    def _setup_calculations(self) -> None:
+        """Miscellaneous calculations to inform the model later.
+
+        Notes
+        -----
+        Calculates the collision sphere radius, coma radius, time to
+        permanent flow regime, the maximum radius our grid could possibly
+        need to extend out to, and the maximum angle that a fragment's
+        trajectory can deviate from its parent's trajectory (which is
+        assumed to be radial).
 
-            Notes
-            -----
-            Calculates the collision sphere radius, coma radius, time to
-            permanent flow regime, the maximum radius our grid could possibly
-            need to extend out to, and the maximum angle that a fragment's
-            trajectory can deviate from its parent's trajectory (which is
-            assumed to be radial)
         """
 
         """
             Calculate collision sphere radius based on the first production
             rate, Eq. (5) in Festou 1981
 
             Note that this is only calculated with the base production rate,
             because it is assumed that the base production rate has had roughly
             enough time to reach a steady state before letting production vary
             with time.
         """
+
+        if self.print_progress:
+            print("Performing setup calculations...")
+
         # This v_therm factor comes from molecular flux of ideal gas moving
         # through a surface, in our case the surface of the collision sphere
         # The gas is collisional inside this sphere and free beyond it, so we
         # can model this as effusion
-        v_therm = self.parent['v_outflow'] * 0.25
+        v_therm = self.parent.v_outflow * 0.25
         q = self.base_q
-        vp = self.parent['v_outflow']
-        vf = self.fragment['v_photo']
+        vp = self.parent.v_outflow
+        vf = self.fragment.v_photo
 
         # Eq. 5 of Festou 1981
-        self.vmodel['collision_sphere_radius'] = (
-            (self.parent['sigma'] * q * v_therm) / (vp * vp)
+        self.vmr.collision_sphere_radius = (
+            (self.parent.sigma * q * v_therm) / (vp * vp)
         ) * u.m
 
-        # Calculates the radius of the coma (parents only), given our input
-        # parameters
+        # Calculates the radius of the coma (defined as the space the parents
+        # occupy)
         # NOTE: Equation (16) of Festou 1981 where alpha is the percent
         # destruction of molecules
-        parent_beta_r = -np.log(1.0 - self.parent_destruction_level)
-        parent_r = parent_beta_r * vp * self.parent['tau_T']
-        self.vmodel['coma_radius'] = parent_r * u.m
+        parent_beta_r = -np.log(1.0 - self.model_params.parent_destruction_level)
+        parent_r = parent_beta_r * vp * self.parent.tau_T
+        self.vmr.coma_radius = parent_r * u.m
 
-        # Calculates the time needed to hit a steady, permanent production of
+        fragment_beta_r = -np.log(1.0 - self.model_params.fragment_destruction_level)
+        # Calculate the time needed to hit a steady, permanent production of
         # fragments
-        fragment_beta_r = -np.log(1.0 - self.fragment_destruction_level)
-
-        perm_flow_radius = (
-            self.vmodel['coma_radius'].value +
-            ((vp + vf) * fragment_beta_r * self.fragment['tau_T'])
+        perm_flow_radius = self.vmr.coma_radius.value + (
+            (vp + vf) * fragment_beta_r * self.fragment.tau_T
         )
 
-        t_secs = (
-            self.vmodel['coma_radius'].value / vp +
-            (perm_flow_radius - self.vmodel['coma_radius'].value)
-            / (vp + vf)
-        )
-        self.vmodel['t_perm_flow'] = (t_secs * u.s).to(u.day)
+        t_secs = self.vmr.coma_radius.value / vp + (
+            perm_flow_radius - self.vmr.coma_radius.value
+        ) / (vp + vf)
+        self.vmr.t_perm_flow = (t_secs * u.s).to(u.day)
 
         # This is the total radial size that parents & fragments occupy, beyond
         # which we assume zero density
-        self.vmodel['max_grid_radius'] = perm_flow_radius * u.m
+        self.vmr.max_grid_radius = perm_flow_radius * u.m
 
         # Two cases for angular range of ejection of fragment based on relative
         # velocities of parent and fragment species
-        if(vf < vp):
-            self.vmodel['epsilon_max'] = np.arcsin(vf / vp)
+        if vf < vp:
+            self.epsilon_max = np.arcsin(vf / vp)
         else:
-            self.vmodel['epsilon_max'] = np.pi
+            self.epsilon_max = np.pi
+
+    def production_at_time(self, t: np.float64) -> np.float64:
+        """Get production rate at time t.
+
+
+        Parameters
+        ----------
+        t : numpy.float64
+            Time in seconds, with positive values representing the past
 
-    def production_at_time(self, t):
-        """ Get production rate at time t
 
-            Parameters
-            ----------
-            t : float
-                Time in seconds, with positive values representing the past
-
-            Returns
-            -------
-            numpy.float64
-                Production rate, unitless, at the specified time
+        Returns
+        -------
+        numpy.float64
+            Production rate, unitless, at the specified time
 
         """
 
         return self.base_q + self.q_t(t)
 
-    def _make_radial_logspace_grid(self):
-        """ Create an appropriate radial grid based on the model parameters
+    def _make_radial_logspace_grid(self) -> np.ndarray:
+        """Create an appropriate radial grid based on the model parameters.
+
+
+        Returns
+        -------
+        ndarray
+            Logarithmically spaced samples of the radial space around the coma,
+            out to a maximum distance.
+
+
+        Notes
+        -----
+        Creates a grid (in meters) with numpy's logspace function that covers
+        the expected radial size, stretching from 2 times the collision sphere
+        radius (near the nucleus be dragons) out to the calculated max.  If we
+        get too close to the nucleus things go very badly so don't do it, dear
+        reader.
 
-            Returns
-            -------
-            ndarray
-                Logarithmically spaced samples of the radial space around the
-                coma, out to a maximum distance
-
-            Notes
-            -----
-            Creates a grid (in meters) with numpy's logspace function that
-            covers the expected radial size, stretching from 2 times the
-            collision sphere radius (near the nucleus be dragons) out to the
-            calculated max.  If we get too close to the nucleus things go very
-            badly so don't do it, dear reader
         """
-        start_power = np.log10(
-            self.vmodel['collision_sphere_radius'].value * 2
-        )
-        end_power = np.log10(self.vmodel['max_grid_radius'].value)
+
+        start_power = np.log10(self.vmr.collision_sphere_radius.value * 2)
+        end_power = np.log10(self.vmr.max_grid_radius.value)
         return np.logspace(
-            start_power, end_power,
-            num=self.radial_points, endpoint=True
+            start_power, end_power, num=self.grid.radial_points, endpoint=True
+        )
+
+    def _outflow_axis_sampling(
+        self, x: np.float64, y: np.float64, theta: np.float64
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """Construct a list of points along the outflow axis, sampled to be
+        more dense around the minimum distance to (x, y).
+
+
+        Parameters
+        ----------
+        x : numpy.float64
+            x-coordinate of the space where we are calculating the fragment
+            density
+
+        y : numpy.float64
+            y-coordinate of the space where we are calculating the fragment
+            density
+
+        theta: numpy.float64
+            polar spherical coordinate of (x, y) to avoid calculating it from
+            (x, y)
+
+
+        Returns
+        -------
+        tuple(numpy.ndarray, numpy.ndarray)
+            Tuple with list of ejection sites in the first index and their
+            extents in the second index
+
+
+        Notes
+        -----
+        Returns list of radial points along outflow axis to sample for fragment
+        ejection, with a list describing the size dr that each ejection point
+        occupies along the outflow axis.
+
+        """
+
+        outflow_axis_edge = self.vmr.coma_radius.value
+
+        # calc angle to edge of the grid, and use it if it's less than
+        # epsilon max.  without this, when epsilon_max approaches pi we
+        # get values of r outside the edge of the grid
+        grid_edge_angle = np.arctan2(x, (y - outflow_axis_edge))
+        if grid_edge_angle < self.epsilon_max:
+            max_subangle = grid_edge_angle
+        else:
+            max_subangle = self.epsilon_max
+
+        # Trace angles from our grid point at x, y and find where dissociations
+        # would have to occur along the outflow axis. This samples shorter
+        # trajectories more finely along the axis, which is necessary because
+        # the exponential decay along their transit means they contribute the
+        # most to the fragment density
+        ces = np.vectorize(lambda epsilon: y - x / np.tan(epsilon))
+
+        # array one element larger than radial_substeps because we will
+        # use the midpoints defined by this array
+        subangles = np.linspace(
+            theta, max_subangle, num=self.grid.radial_substeps + 1, endpoint=True
         )
 
-    def _compute_fragment_density(self):
-        """ Computes the density of fragments as a function of radius
+        # Find where this set of angles intersects the outflow axis
+        ejection_grid = ces(subangles)
+        # Find dr for radial integration
+        drs = np.diff(ejection_grid)
+
+        # This puts the sampling of the ejection sites at the midpoints
+        # of our ejection grid
+        ejection_sites = (ejection_grid[1:] + ejection_grid[:-1]) / 2
+
+        return ejection_sites, drs
+
+    def _fragment_sputter(self, r: np.float64, theta: np.float64) -> np.float64:
+        """Compute the fragment density at (r, theta) in a spherical
+        coordinate system where theta is the polar angle and the parents flow
+        radially outward along the z axis.
+
+
+        Parameters
+        ----------
+        r : numpy.float64
+            radial coordinate in meters where we are calculating the fragment
+            density.
+
+        theta : numpy.float64
+            polar spherical coordinate where we are calculating the fragment
+            density.
+
+
+        Returns
+        -------
+        np.float64
+            Fragment density in 1/m**3, no astropy units attached.
+
+        """
+
+        sputter = 0.0
+        vp = self.parent.v_outflow
+        vf = self.fragment.v_photo
+        p_tau_T = self.parent.tau_T
+        f_tau_T = self.fragment.tau_T
+
+        x = r * np.sin(theta)
+        y = r * np.cos(theta)
+
+        ejection_sites, drs = self._outflow_axis_sampling(x, y, theta)
+
+        # Loop over these ejection sites that contribute to x, y
+        for slice_r, dr in zip(ejection_sites, drs):
+            # Distance from dissociation site to our grid point
+            sep_dist = np.sqrt(x**2 + (slice_r - y) ** 2)
+
+            cos_eject = (y - slice_r) / sep_dist
+            sin_eject = x / sep_dist
+
+            # Parent extinction when traveling along to the
+            # dissociation site
+            p_extinction = np.e ** (-slice_r / (p_tau_T * vp))
+
+            # Calculate sqrt(vR^2 - u^2 sin^2 gamma)
+            v_factor = np.sqrt(vf * vf - (vp * vp) * sin_eject**2)
+
+            # The geometry of the problem can admit one or two solutions for
+            # the velocity of the fragment
+            v_one = vp * cos_eject + v_factor
+            if vf > vp:
+                velocities = [v_one]
+            else:
+                v_two = vp * cos_eject - v_factor
+                velocities = [v_one, v_two]
+
+            # TODO: this shouldn't be necessary if we only pick r, theta inside ejection
+            if v_one == 0.0:
+                continue
+
+            for v in velocities:
+                # Time taken to travel from the dissociation point at v, reject
+                # if the time is too large and fragments have decayed beyond
+                # self.fragment_destruction_level percent
+                t_frag = sep_dist / v
+                if t_frag > self.time_limit:
+                    continue
+
+                # total time between parent emission from nucleus and fragment
+                # arriving at our point of interest, which we then use to look
+                # up Q at that time in the past
+                t_total = (slice_r / vp) + t_frag
+
+                # Division by parent velocity makes this production per
+                # unit distance for radial integration q(r, epsilon)
+                # given by eq. 32, Festou 1981
+                q = self.production_at_time(t_total) / vp
+                q_r_eps = (v**2 * q) / (vf * np.abs(v - vp * cos_eject))
+
+                # Fragment extinction when traveling at speed v from
+                # dissociation site to x, y
+                f_extinction = np.e ** (-t_frag / f_tau_T)
+
+                # differential addition to the density integrating along dr,
+                # similar to eq. (36) Festou 1981
+                n_r = (p_extinction * f_extinction * q_r_eps) / (sep_dist**2 * v)
+
+                sputter += n_r * dr
+
+        return sputter
+
+    def _compute_fragment_density(self) -> None:
+        """Computes the density of fragments as a function of radius.
+
+        Notes
+        -----
+        Computes the density of fragments sputtered around the comet due to an
+        outflow of parents along the z-axis, performing the integration in eq.
+        (36), Festou 1981. The resulting radial fragment density will be in
+        units of 1/(m^3) as we work in m, s, and m/s.
+
+        We then interpolate the fragment density as a function of arbitrary
+        radius.  We use our results to calculate the total number of fragments
+        in the coma for comparison to the theoretical number we expect, to
+        provide the user with a rough idea of how well the chosen radial and
+        angular grid sizes have captured the appropriate amount of particles.
+        Note that some level of disagreement is expected because the
+        parent_destruction_level and fragment_destruction_level parameters cut
+        the grid off before all parents can dissociate, and thus some escape the
+        model and come up missing in the fragment count based on the grid.
 
-            Notes
-            -----
-            Computes the density at different radii and due to each ejection
-            angle, performing the radial integration of eq. (36), Festou 1981
-            with only one fragment velocity.  The resulting units will be in
-            1/(m^3) as we work in m, s, and m/s.
-
-            The density is first found on a radial grid, then interpolated to
-            find density as a function of arbitrary radius.  We use our results
-            from the grid to calculate the total number of fragments in the
-            coma for comparison to the theoretical number we expect, to provide
-            the user with a rough idea of how well the chosen radial and
-            angular grid sizes have captured the appropriate amount of
-            particles.  Note that some level of disagreement is expected
-            because the parent_destruction_level and fragment_destruction_level
-            parameters cut the grid off before all particles can dissociate,
-            and thus some escape the model and come up missing in the fragment
-            count based on the grid.
         """
-        vp = self.parent['v_outflow']
-        vf = self.fragment['v_photo']
+
+        if self.print_progress:
+            print("Starting fragment density computations...")
 
         # Follow fragments until they have been totally destroyed
-        time_limit = self.max_fragment_lifetimes * self.fragment['tau_T']
-        r_coma = self.vmodel['coma_radius'].value
-        r_limit = r_coma
-
-        # temporary radial array for when we loop through 0 to epsilonMax
-        ejection_radii = np.zeros(self.radial_substeps)
-
-        p_tau_T = self.parent['tau_T']
-        f_tau_T = self.fragment['tau_T']
-        p_tau_d = self.parent['tau_d']
+        self.time_limit = self.model_params.max_fragment_lifetimes * self.fragment.tau_T
 
-        # Compute this once ahead of time
         # More factors to fill out integral similar to eq. (36) Festou 1981
         integration_factor = (
-            (1 / (4 * np.pi * p_tau_d)) *
-            self.vmodel['d_alpha'] / (4.0 * np.pi)
+            (1 / (4 * np.pi * self.parent.tau_d)) * self.d_alpha / (4.0 * np.pi)
         )
 
-        # Calculate the density contributions over the volume of the comet
-        # atmosphere due to one ejection axis
-        for j in range(0, self.angular_points):
-            cur_angle = self.vmodel['angular_grid'][j]
-            # Loop through the radial points along this axis
-            for i in range(0, self.radial_points):
-
-                cur_r = self.vmodel['fast_radial_grid'][i]
-                x = cur_r * np.sin(cur_angle)
-                y = cur_r * np.cos(cur_angle)
-
-                # Decide how granular our epsilon should be
-                d_epsilon_steps = len(ejection_radii)
-                d_epsilon = (
-                            (self.vmodel['epsilon_max'] - cur_angle)
-                    / d_epsilon_steps
-                )
-
-                # Maximum radius that contributes to point x,y when there is a
-                # a max ejection angle
-                if(self.vmodel['epsilon_max'] < np.pi):
-                    r_limit = y - (x / np.tan(self.vmodel['epsilon_max']))
-                # Set the last element to be r_coma or the above limit
-                ejection_radii[d_epsilon_steps - 1] = r_limit
-
-                # We already filled out the very last element in the array
-                # above, so it's d_epsilon_steps - 1
-                for dE in range(0, d_epsilon_steps - 1):
-                    ejection_radii[dE] = (
-                        y -
-                        x / np.tan((dE + 1) * d_epsilon + cur_angle)
-                    )
-
-                ejection_radii_start = 0
-                # Number of slices along the contributing axis for each step
-                num_slices = self.angular_substeps
-
-                # Loop over radial chunk that contributes to x,y
-                for ejection_radii_end in ejection_radii:
-
-                    # We are slicing up this axis into pieces
-                    dr = (
-                         (ejection_radii_end - ejection_radii_start) /
-                        num_slices
-                    )
-
-                    # Loop over tiny slices along this chunk
-                    for m in range(0, num_slices):
-
-                        # TODO: We could probably eliminate m by making a
-                        # linear space from ejection_radii_start to
-                        # ejection_radii_end
-
-                        # Current distance along contributing axis
-                        cur_r = (m + 0.5) * dr + ejection_radii_start
-                        # This is the distance from the NP axis point to the
-                        # current point on the ray, squared
-                        sep_dist = np.sqrt(x * x + (cur_r - y) * (cur_r - y))
-
-                        cos_eject = (y - cur_r) / sep_dist
-                        sin_eject = x / sep_dist
-
-                        # Calculate sqrt(vR^2 - u^2 sin^2 gamma)
-                        v_factor = np.sqrt(
-                            vf * vf - (vp * vp) * sin_eject ** 2)
-
-                        # The first (and largest) of the two solutions for the
-                        # velocity when it arrives
-                        v_one = vp * cos_eject + v_factor
-
-                        # Time taken to travel from the dissociation point at
-                        # v1, reject if the time is too large (and all
-                        # fragments have decayed)
-                        t_frag_one = sep_dist / v_one
-                        if t_frag_one > time_limit:
-                            continue
-
-                        # This is the total time between parent emission from
-                        # nucleus and fragment arriving at our point of
-                        # interest, which we then use to look up Q at that time
-                        # in the past
-                        t_total_one = (cur_r / vp) + t_frag_one
-
-                        # Division by parent velocity makes this production per
-                        # unit distance for radial integration q(r, epsilon)
-                        # given by eq. 32, Festou 1981
-                        prod_one = self.production_at_time(t_total_one) / vp
-                        q_r_eps_one = (
-                            (v_one * v_one * prod_one) /
-                            (vf * np.abs(v_one - vp * cos_eject))
-                        )
-
-                        # Parent extinction when traveling along to the
-                        # dissociation site
-                        p_extinction = np.e ** (-cur_r / (p_tau_T * vp))
-                        # Fragment extinction when traveling at speed v1
-                        f_extinction_one = np.e ** (-t_frag_one / f_tau_T)
-
-                        # First differential addition to the density
-                        # integrating along dr, similar to eq. (36) Festou
-                        # 1981, due to the first velocity
-                        n_r_one = (
-                            (p_extinction * f_extinction_one * q_r_eps_one) /
-                            (sep_dist ** 2 * v_one)
-                        )
-
-                        # Add this contribution to the density grid
-                        self.vmodel['density_grid'][i][j] = (
-                            self.vmodel['density_grid'][i][j] +
-                            n_r_one * dr
-                        )
-
-                        # Check if there is a second solution for the velocity
-                        if vf > vp:
-                            continue
-
-                        # Compute the contribution from the second solution for
-                        # v in the same way
-                        v_two = vp * cos_eject - v_factor
-                        t_frag_two = sep_dist / v_two
-                        if t_frag_two > time_limit:
-                            continue
-                        t_total_two = (cur_r / vp) + t_frag_two
-                        prod_two = self.production_at_time(t_total_two) / vp
-                        q_r_eps_two = (
-                            (v_two * v_two * prod_two) /
-                            (vf * np.abs(v_two - vp * cos_eject))
-                        )
-                        f_extinction_two = np.e ** (-t_frag_two / f_tau_T)
-                        n_r_two = (
-                            (p_extinction * f_extinction_two * q_r_eps_two) /
-                            (v_two * sep_dist ** 2)
-                        )
-                        self.vmodel['density_grid'][i][j] = (
-                            self.vmodel['density_grid'][i][j] +
-                            n_r_two * dr
-                        )
-
-                    # Next starting radial point is the current end point
-                    ejection_radii_start = ejection_radii_end
-
-            if(self.print_progress is True):
-                progress_percent = (j + 1) * 100 / self.angular_points
-                print(f'Computing: {progress_percent:3.1f} %', end='\r')
-
-        # Loops automatically over the 2d grid
-        self.vmodel['density_grid'] *= integration_factor
-        # phew
-
-        """
-            Performs angular part of the integration to yield density in m^-3
-            as a function of radius.  Assumes spherical symmetry of parent
-            production.
-
-            Fills vmodel['radial_density'] and vmodel['fast_radial_density']
-            with and without units respectively
-            Fills vmodel['r_dens_interpolation'] with cubic spline
-            interpolation of the radial density, which takes radial coordinate
-            in m and outputs the density at that coord in m^-3, without units
-            attached
-        """
+        # vectorize and apply to each combination of (r, theta)
+        sputter_func = np.vectorize(self._fragment_sputter)
+        rs, thetas = np.meshgrid(
+            self.fast_voldens_grid, self.angular_grid, indexing="ij"
+        )
+        self.fragment_sputter = integration_factor * sputter_func(rs, thetas)
 
         # Make array to hold our data, no units
-        self.vmodel['fast_radial_density'] = np.zeros(self.radial_points)
+        self.fast_voldens = np.zeros(self.grid.radial_points)
 
-        # loop through grid array
-        for i in range(0, self.radial_points):
-            for j in range(0, self.angular_points):
-                # Current angle is theta
-                theta = self.vmodel['angular_grid'][j]
-                # Integration factors from angular part of integral, similar to
-                # eq. (36) Festou 1981
-                dens_contribution = (
-                    2.0 * np.pi * np.sin(theta) *
-                    self.vmodel['density_grid'][i][j]
-                )
-                self.vmodel['fast_radial_density'][i] += dens_contribution
+        # Integration factors from angular part of integral, similar to
+        # eq. (36) Festou 1981
+        # integrate over theta to produce radial fragment volume density
+        # axis = 1 sums over second column, theta
+        # Equivalent to summing over j for sin(theta[j]) *
+        # fragment_sputter[i][j] with numpy magic
+        self.solid_angle_sputter = np.sin(thetas) * self.fragment_sputter
+        self.fast_voldens = 2.0 * np.pi * np.sum(self.solid_angle_sputter, axis=1)
 
         # Tag with proper units
-        self.vmodel['radial_density'] = (
-            self.vmodel['fast_radial_density'] / (u.m ** 3)
-        )
+        self.vmr.volume_density = self.fast_voldens / (u.m**3)
 
-    def _interpolate_radial_density(self):
-        """ Interpolate the radial density.
+    def _interpolate_volume_density(self) -> None:
+        """Interpolate the volume density as a function of radial distance
+        from the nucleus.
 
         Takes our fragment density grid and constructs density as a function of
-        arbitrary radius
+        arbitrary radius.
+
         """
 
         if not scipy:
-            raise RequiredPackageUnavailable('scipy')
+            raise RequiredPackageUnavailable("scipy")
+
+        if self.print_progress:
+            print("Interpolating radial fragment density...")
+
         # Interpolate this radial density grid with a cubic spline for lookup
         # at non-grid radii, input in m, output in 1/m^3
-        self.vmodel['r_dens_interpolation'] = (
-            CubicSpline(self.vmodel['fast_radial_grid'],
-                        self.vmodel['fast_radial_density'],
-                        bc_type='natural')
-        )
-
-    def _column_density_at_rho(self, rho):
-        """ Calculate the column density of fragments at a given impact parameter
-
-            Parameters
-            ----------
-            rho : float
-                Impact parameter of the column density integration, in meters
-
-            Returns
-            -------
-            float
-                Column density at the given impact parameter in m^-2, no
-                astropy units attached
-
-            Notes
-            -----
-            We return zero column density beyond the edge of our grid, so if
-            there is still significant column density near the edge of the grid
-            this can lead to strange graphing results and sharp cutoffs.
+        self.vmr.volume_density_interpolation = CubicSpline(
+            self.fast_voldens_grid, self.fast_voldens, bc_type="natural"
+        )
+
+    def _column_density_at_rho(self, rho: np.float64) -> np.float64:
+        """
+        Calculate the column density of fragments at a given impact parameter.
+
+
+        Parameters
+        ----------
+        rho : np.float64
+            Impact parameter of the column density integration, in meters
+
+
+        Returns
+        -------
+        np.float64
+            Column density at the given impact parameter in m^-2, no
+            astropy units attached
+
+
+        Notes
+        -----
+        We return zero column density beyond a certain distance past the
+        grid edge, which can lead to strange graphing results and sharp
+        cutoffs.
+
         """
 
-        r_max = self.vmodel['max_grid_radius'].value
-        if(rho > r_max):
+        reach_factor = 2.0
+
+        # _volume_density() approximates beyond the edge of the grid, so allow
+        # an arbirtary limit beyond which we just return zero column density
+        r_max = self.vmr.max_grid_radius.value * reach_factor
+
+        if rho > r_max:
             return 0
-        rhosq = rho ** 2
-        z_max = np.sqrt(r_max ** 2 - rhosq)
+
+        rhosq = rho**2
+        z_max = np.sqrt(r_max**2 - rhosq)
 
         def column_density_integrand(z):
-            return self.vmodel['r_dens_interpolation'](np.sqrt(z ** 2 + rhosq))
+            return self._volume_density(np.sqrt(z**2 + rhosq))
 
-        # Romberg is significantly slower for impact parameters near the
-        # nucleus, and becomes much faster at roughly 60 times the collision
-        # sphere radius, after a few tests
-        # The results of both were the same to within .1% or better, generally
-        # TODO: test this for a range of productions to see if this holds
-
-        if rho < (60 * self.vmodel['collision_sphere_radius'].value):
-            c_dens = (
-                quad(column_density_integrand,
-                     -z_max, z_max, limit=3000)
-            )[0]
-        else:
-            c_dens = (
-                2 * romberg(column_density_integrand,
-                            0, z_max, rtol=0.0001, divmax=20)
-            )
+        c_dens = 2 * romberg(column_density_integrand, 0, z_max, rtol=0.0001, divmax=50)
 
         # result is in 1/m^2
         return c_dens
 
-    def _compute_column_density(self):
-        """ Compute the column density on the grid and interpolate the results
+    def _compute_column_density(self) -> None:
+        """Compute the column density on the grid and interpolate the results.
 
-            Computes the fragment column density on a grid and interpolates for
-            fragment column density as a function of arbitrary radius.
+        Notes
+        -----
+        The interpolator returns column density in m^-2, no astropy units
+        attached.
 
-            Notes
-            -----
-            The interpolator returns column density in m^-2, no astropy units
-            attached
         """
+
         if not scipy:
-            raise RequiredPackageUnavailable('scipy')
+            raise RequiredPackageUnavailable("scipy")
+
+        if self.print_progress:
+            print("Computing column densities...")
 
         # make a grid for the column density values
         column_density_grid = self._make_radial_logspace_grid()
-        # vectorize so we can hand the whole grid to our column density
-        # computing function in one line
+        # vectorize so we can hand the whole grid to our function
         cd_vectorized = np.vectorize(self._column_density_at_rho)
         # array now holds corresponding column density values
         column_densities = cd_vectorized(column_density_grid)
 
-        self.vmodel['fast_column_density_grid'] = column_density_grid
-        self.vmodel['column_density_grid'] = column_density_grid * u.m
-        self.vmodel['column_densities'] = column_densities / (u.m ** 2)
+        self.fast_column_density_grid = column_density_grid
+        self.vmr.column_density_grid = column_density_grid * u.m
+        self.vmr.column_density = column_densities / (u.m**2)
         # Interpolation gives column density in m^-2
-        self.vmodel['column_density_interpolation'] = (
-            CubicSpline(
-                column_density_grid,
-                column_densities,
-                bc_type='natural'
-            )
+        self.vmr.column_density_interpolation = CubicSpline(
+            column_density_grid, column_densities, bc_type="natural"
         )
 
-    def calc_num_fragments_theory(self):
-        """ The total number of fragment species we expect in the coma
+    def _calc_num_fragments_theory(self) -> np.float64:
+        """The total number of fragment species we expect in the coma.
+
+        Returns
+        -------
+        np.float64
+            Total number of fragment species we expect in the coma theoretically
+
+        Notes
+        -----
+        Outbursts/time dependent production in general will make this result
+        poor due to the grid being sized to capture a certain fraction of
+        parents/fragments at the oldest (first) production rate.  The farther
+        you get from this base production, the farther the model will deviate
+        from capturing the requested percentage of particles.
+
+        """
 
-            Returns
-            -------
-            float
-                Total number of fragment species we expect in the coma
-                theoretically
-
-            Notes
-            -----
-            This needs to be rewritten to better handle time dependence; the
-            original implementation was designed for abrupt but small parent
-            production changes.
-        """
-
-        # TODO: Re-implement this as differential equations with parent
-        # photodissociation as a source of fragments, and fragment
-        # photodissociation as a sink
-        vp = self.parent['v_outflow']
-        vf = self.fragment['v_photo']
-        p_tau_T = self.parent['tau_T']
-        f_tau_T = self.fragment['tau_T']
-        p_tau_d = self.parent['tau_d']
-        t_perm = self.vmodel['t_perm_flow'].to(u.s).value
+        vp = self.parent.v_outflow
+        vf = self.fragment.v_photo
+        p_tau_T = self.parent.tau_T
+        f_tau_T = self.fragment.tau_T
+        p_tau_d = self.parent.tau_d
+        t_perm = self.vmr.t_perm_flow.to(u.s).value
 
         alpha = f_tau_T * p_tau_T / p_tau_d
 
-        max_r = self.vmodel['max_grid_radius'].value
-        last_density_element = len(self.vmodel['fast_radial_density']) - 1
-        edge_adjust = (
-            (np.pi * max_r * max_r * (vf + vp) *
-             self.vmodel['fast_radial_density'][last_density_element])
-        )
+        max_r = self.vmr.max_grid_radius.value
+        edge_adjust = np.pi * max_r * max_r * (vf + vp) * self.fast_voldens[-1]
+
+        num_time_slices = 1000
 
-        num_time_slices = 10000
         # array starting at tperm (farthest back in time we expect something to
         # hang around), stepped down to zero (when the observation takes place)
-        time_slices = np.linspace(t_perm, 0, num_time_slices, endpoint=False)
+        time_slices = np.linspace(t_perm, 0, num_time_slices, endpoint=True)
 
+        # estimate based on discrete-time source and sink model
         theory_total = 0
-        for i, t in enumerate(time_slices[:-1], start=0):
-            if t > t_perm:
-                t1 = t_perm
-            else:
-                t1 = t
-            t1 /= p_tau_T
-
-            if i != (num_time_slices - 1):
-                t2 = time_slices[i + 1]
-            else:
-                t2 = 0
-            t2 /= p_tau_T
-            mult_factor = -np.e ** (-t1) + np.e ** (-t2)
+        for i, t in enumerate(time_slices[:-1]):
+            extinction_one = t / p_tau_T
+            extinction_two = time_slices[i + 1] / p_tau_T
+            mult_factor = -np.e ** (-extinction_one) + np.e ** (-extinction_two)
             theory_total += self.production_at_time(t) * mult_factor
 
-        theory_total *= alpha
-        theory_total -= edge_adjust
+        return theory_total * alpha - edge_adjust
+
+    def _calc_num_fragments_grid(self) -> np.float64:
+        """Total number of fragments in the coma.
 
-        return theory_total
+        Calculates the total number of fragments by integrating the density grid
+        over its volume
+
+
+        Returns
+        -------
+        np.float64
+            Number of fragments in the coma based on our grid calculations
 
-    def calc_num_fragments_grid(self):
-        """ Total number of fragments in the coma.
 
-            Calculates the total number of fragment species by integrating the
-            density grid over its volume
-
-            Returns
-            -------
-            float
-                Number of fragments in the coma based on our grid calculations
-
-            Notes
-            -----
-            Outbursts/time dependent production in general will make this
-            result poor due to the grid being sized to capture a certain
-            fraction of parents/fragments at the oldest (first) production
-            rate.  The farther you get from this base production, the farther
-            the model will deviate from capturing the requested percentage of
-            particles.
+        Notes
+        -----
+        Outbursts/time dependent production in general will make this result
+        poor due to the grid being sized to capture a certain fraction of
+        parents/fragments at the oldest (first) production rate.  The farther
+        you get from this base production, the farther the model will deviate
+        from capturing the requested percentage of particles.
+
         """
-        max_r = self.vmodel['max_grid_radius'].value
+
+        max_r = self.vmr.max_grid_radius.value
 
         def vol_integrand(r, r_func):
-            return (r_func(r) * r ** 2)
+            return r_func(r) * r**2
 
         r_int = romberg(
-            vol_integrand, 0, max_r,
-            args=(self.vmodel['r_dens_interpolation'], ),
-            rtol=0.0001, divmax=20)
+            vol_integrand,
+            0,
+            max_r,
+            args=(self.vmr.volume_density_interpolation,),
+            rtol=0.0001,
+            divmax=20,
+        )
         return 4 * np.pi * r_int
 
-    def _column_density(self, rho):
-        """ Gives fragment column density at arbitrary impact parameter
+    def _column_density(self, rho) -> np.float64:
+        """Gives fragment column density at arbitrary impact parameter.
+
+        Parameters
+        ----------
+        rho : np.float64
+            Impact parameter, in meters, no astropy units attached.
+
+
+        Returns
+        -------
+        np.float64
+            Fragment column density at given impact parameter, in m^-2, no
+            astropy units.
 
-            Parameters
-            ----------
-            rho : float
-                Impact parameter, in meters, no astropy units attached
-
-            Returns
-            -------
-            float
-                Fragment column density at given impact parameter, in m^-2
         """
-        return self.vmodel['column_density_interpolation'](rho)
 
-    def _volume_density(self, r):
-        """ Gives fragment volume density at arbitrary radius
+        if rho < self.fast_column_density_grid[0]:
+            return self.vmr.column_density[0].value
+        if rho > self.vmr.max_grid_radius.value:
+            return 0
+        return self.vmr.column_density_interpolation(rho)
+
+    def _volume_density(self, r) -> np.float64:
+        """Gives fragment volume density at arbitrary radius.
+
+
+        Parameters
+        ----------
+        r : np.float64
+            Distance from nucleus, in meters, no astropy units attached.
+
+
+        Returns
+        -------
+        np.float64
+            Fragment volume density at specified radius, in m^-3, no astropy
+            units.
+
+
+        Notes
+        -----
+        When asked for a value at a radius smaller than the first grid point, we
+        have two choices: return a value based on the interpolation of the
+        volume density, or return the value of the closest grid point to the
+        nucleus. This function returns the closest grid point to the nucleus,
+        because the model does not say anything about what happens inside the
+        collision sphere - so we approximate by clamping the value as constant.
+        We can't trust the interpolation outside of the grid because the density
+        values can get very large or become negative.
+
+        Outside the radius of the grid, the volume density is approximated with
+        exponential decay based on the total lifetime of the fragment.
 
-            Parameters
-            ----------
-            r : float
-                Distance from nucles, in meters, no astropy units attached
-
-            Returns
-            -------
-            float
-                Fragment volume density at specified radius
         """
-        return self.vmodel['r_dens_interpolation'](r)
+
+        if r < self.fast_voldens_grid[0]:
+            return self.fast_voldens[0]
+        if r > self.vmr.max_grid_radius.value:
+            diff = r - self.vmr.max_grid_radius.value
+            guess = self.fast_voldens[-1] * np.exp(
+                -diff / (self.fragment.tau_T * self.fragment.v_photo)
+            )
+            return guess
+        return self.vmr.volume_density_interpolation(r)
```

### Comparing `sbpy-0.3.0/sbpy/activity/gas/data/__init__.py` & `sbpy-0.4.0/sbpy/activity/gas/data/__init__.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/activity/gas/data/schleicher88.txt` & `sbpy-0.4.0/sbpy/activity/gas/data/schleicher88.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/activity/gas/productionrate.py` & `sbpy-0.4.0/sbpy/activity/gas/productionrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 :author: Giannina Guzman (gguzman2@villanova.edu)
 
 created on June 26, 2019
 """
 
 import tempfile
 import numpy as np
-import astropy
 import astropy.constants as con
 import astropy.units as u
 from astroquery.jplspec import JPLSpec
 from astroquery.lamda import Lamda
 from ...bib import register
 from ...data import Phys
 
 __all__ = ['LTE', 'NonLTE', 'einstein_coeff',
            'intensity_conversion', 'beta_factor', 'total_number',
            'from_Haser']
 
-if astropy.__version__ < '5':
-    __doctest_skip__ = ['LTE.from_Drahus']
+__doctest_requires__ = {
+    "LTE.from_Drahus": ["astropy>=5.0", "astroquery>=0.4.7"],
+    "NonLTE.from_pyradex": ["astroquery>=0.4.7"],
+    "from_Haser": ["astroquery>=0.4.7"],
+}
 
 
 def intensity_conversion(mol_data):
     """
     Returns conversion of the integrated line intensity at 300 K
     (from the JPL molecular spectra catalog) to a chosen temperature
```

### Comparing `sbpy-0.3.0/sbpy/activity/gas/tests/data/CH3OH.csv` & `sbpy-0.4.0/sbpy/activity/gas/tests/data/CH3OH.csv`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/activity/gas/tests/data/HCN.csv` & `sbpy-0.4.0/sbpy/activity/gas/tests/data/HCN.csv`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/activity/gas/tests/data/wm_fortran_test_output.txt` & `sbpy-0.4.0/sbpy/activity/gas/tests/data/wm_fortran_test_output.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/activity/gas/tests/test_core.py` & `sbpy-0.4.0/sbpy/activity/gas/tests/test_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,124 +1,130 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import pytest
 import numpy as np
 import astropy.units as u
 import astropy.constants as const
 from .. import core
-from .. import (photo_lengthscale, photo_timescale, fluorescence_band_strength,
-                VectorialModel, Haser)
+from .. import (
+    photo_lengthscale,
+    photo_timescale,
+    fluorescence_band_strength,
+    VectorialModel,
+    Haser,
+)
 from .... import exceptions as sbe
 from ....data import Phys
 
 
 def test_photo_lengthscale():
-    gamma = photo_lengthscale('OH', 'CS93')
+    gamma = photo_lengthscale("OH", "CS93")
     assert gamma == 1.6e5 * u.km
 
 
 def test_photo_lengthscale_error():
     with pytest.raises(ValueError):
-        photo_lengthscale('asdf')
+        photo_lengthscale("asdf")
 
     with pytest.raises(ValueError):
-        photo_lengthscale('OH', source='asdf')
+        photo_lengthscale("OH", source="asdf")
 
 
 def test_photo_timescale():
-    tau = photo_timescale('CO2', 'CE83')
+    tau = photo_timescale("CO2", "CE83")
     assert tau == 5.0e5 * u.s
 
 
 def test_photo_timescale_error():
     with pytest.raises(ValueError):
-        photo_timescale('asdf')
+        photo_timescale("asdf")
 
     with pytest.raises(ValueError):
-        photo_timescale('OH', source='asdf')
+        photo_timescale("OH", source="asdf")
 
 
-@pytest.mark.parametrize('band, test', (
-    ('OH 0-0', 1.54e-15 * u.erg / u.s),
-    ('OH 1-0', 1.79e-16 * u.erg / u.s),
-    ('OH 1-1', 2.83e-16 * u.erg / u.s),
-    ('OH 2-2', 1.46e-18 * u.erg / u.s),
-    ('OH 0-1', 0.00356 * 1.54e-15 * u.erg / u.s),
-    ('OH 0-2', 0.00021 * 1.54e-15 * u.erg / u.s),
-    ('OH 1-2', 0.00610 * 2.83e-16 * u.erg / u.s),
-    ('OH 2-0', 0.274 * 1.46e-18 * u.erg / u.s),
-    ('OH 2-1', 1.921 * 1.46e-18 * u.erg / u.s),
-))
+@pytest.mark.parametrize(
+    "band, test",
+    (
+        ("OH 0-0", 1.54e-15 * u.erg / u.s),
+        ("OH 1-0", 1.79e-16 * u.erg / u.s),
+        ("OH 1-1", 2.83e-16 * u.erg / u.s),
+        ("OH 2-2", 1.46e-18 * u.erg / u.s),
+        ("OH 0-1", 0.00356 * 1.54e-15 * u.erg / u.s),
+        ("OH 0-2", 0.00021 * 1.54e-15 * u.erg / u.s),
+        ("OH 1-2", 0.00610 * 2.83e-16 * u.erg / u.s),
+        ("OH 2-0", 0.274 * 1.46e-18 * u.erg / u.s),
+        ("OH 2-1", 1.921 * 1.46e-18 * u.erg / u.s),
+    ),
+)
 def test_fluorescence_band_strength_OH_SA88(band, test):
     "Tests values for -1 km/s at 1 au"
-    eph = {
-        'rh': [1, 2] * u.au,
-        'rdot': [-1, -1] * u.km / u.s
-    }
-    LN = fluorescence_band_strength(band, eph, 'SA88').to(test.unit)
+    eph = {"rh": [1, 2] * u.au, "rdot": [-1, -1] * u.km / u.s}
+    LN = fluorescence_band_strength(band, eph, "SA88").to(test.unit)
     assert np.allclose(LN.value, test.value / np.r_[1, 2] ** 2)
 
 
 def test_fluorescence_band_strength_error():
     with pytest.raises(ValueError):
-        fluorescence_band_strength('asdf')
+        fluorescence_band_strength("asdf")
 
     with pytest.raises(ValueError):
-        fluorescence_band_strength('OH 0-0', source='asdf')
+        fluorescence_band_strength("OH 0-0", source="asdf")
 
 
 def test_gascoma_scipy_error(monkeypatch):
-    monkeypatch.setattr(core, 'scipy', None)
+    monkeypatch.setattr(core, "scipy", None)
     test = Haser(1 / u.s, 1 * u.km / u.s, 1e6 * u.km)
     with pytest.raises(sbe.RequiredPackageUnavailable):
         test._integrate_volume_density(1e5)
 
     with pytest.raises(sbe.RequiredPackageUnavailable):
         aper = core.CircularAperture(1000 * u.km)
         test._integrate_column_density(aper)
 
 
 class TestHaser:
-
     def test_volume_density(self):
         """Test a set of dummy values."""
         Q = 1e28 / u.s
         v = 1 * u.km / u.s
         parent = 1e4 * u.km
         daughter = 1e5 * u.km
         r = np.logspace(1, 7) * u.km
         n = Haser(Q, v, parent, daughter).volume_density(r)
-        rel = (daughter / (parent - daughter)
-               * (np.exp(-r / parent) - np.exp(-r / daughter)))
+        rel = (
+            daughter
+            / (parent - daughter)
+            * (np.exp(-r / parent) - np.exp(-r / daughter))
+        )
         # test radial profile
-        assert np.allclose((n / n[0]).value,
-                           (rel / rel[0] * (r[0] / r) ** 2).value)
+        assert np.allclose((n / n[0]).value, (rel / rel[0] * (r[0] / r) ** 2).value)
 
         # test parent-only coma near nucleus against that expected for
         # a long-lived species; will be close, but not exact
         n = Haser(Q, v, parent).volume_density(10 * u.km)
         assert np.isclose(
             n.decompose().value,
             (Q / v / 4 / np.pi / (10 * u.km) ** 2).decompose().value,
-            rtol=0.001)
+            rtol=0.001,
+        )
 
     def test_column_density_small_aperture(self):
         """Test column density for aperture << lengthscale.
 
         Should be within 1% of ideal value.
 
         """
         Q = 1e28 / u.s
         v = 1 * u.km / u.s
         rho = 1 * u.km
         parent = 1e4 * u.km
         N_avg = 2 * Haser(Q, v, parent).column_density(rho)
         ideal = Q / v / 2 / rho
-        assert np.isclose(N_avg.decompose().value, ideal.decompose().value,
-                          rtol=0.001)
+        assert np.isclose(N_avg.decompose().value, ideal.decompose().value, rtol=0.001)
 
     def test_column_density_small_angular_aperture(self):
         """Test column density for angular aperture << lengthscale.
 
         Regression test for PR#243.
 
         Should be within 1% of ideal value.
@@ -126,32 +132,30 @@
         """
         Q = 1e28 / u.s
         v = 1 * u.km / u.s
         rho = 0.001 * u.arcsec
         eph = dict(delta=1 * u.au)
         parent = 1e4 * u.km
         N_avg = 2 * Haser(Q, v, parent).column_density(rho, eph)
-        rho_km = (rho * eph['delta'] * 725.24 * u.km / u.arcsec / u.au
-                  ).to('km')
+        rho_km = (rho * eph["delta"] * 725.24 * u.km / u.arcsec / u.au).to("km")
         ideal = Q / v / 2 / rho_km
-        assert np.isclose(N_avg.to_value('1/m2'),
-                          ideal.to_value('1/m2'), rtol=0.001)
+        assert np.isclose(N_avg.to_value("1/m2"), ideal.to_value("1/m2"), rtol=0.001)
 
     def test_column_density(self):
         """
         Test column density for aperture = lengthscale.
 
         """
         Q = 1e28 / u.s
         v = 1 * u.km / u.s
         rho = 1000 * u.km
         parent = 1000 * u.km
         coma = Haser(Q, v, parent)
         N_avg = coma.column_density(rho)
-        integral = coma._integrate_volume_density(rho.to('m').value)[0]
+        integral = coma._integrate_volume_density(rho.to("m").value)[0]
         assert np.isclose(N_avg.decompose().value, integral)
 
     def test_total_number_large_aperture(self):
         """Test column density for aperture >> lengthscale."""
         Q = 1 / u.s
         v = 1 * u.km / u.s
         rho = 1000 * u.km
@@ -172,15 +176,15 @@
         Q = 1e25 / u.s
         v = 1 * u.km / u.s
         parent = 24000 * u.km
         daughter = 160000 * u.km
         ap = core.CircularAperture(1 * u.arcsec).as_length(1 * u.au)
         coma = Haser(Q, v, parent, daughter)
         N = coma.total_number(ap)
-        assert np.isclose(N, 5.238964562688742e+26)
+        assert np.isclose(N, 5.238964562688742e26)
 
     def test_total_number_rho_AC75(self):
         """Reproduce A'Hearn and Cowan 1975
 
         Assumed 1 km/s.
 
         N(C2) = 10**(12.9300 + log10(L) + 2 * log10(rh))
@@ -225,38 +229,38 @@
         # ]
 
         # Computed by sbpy.  0.893 C2 and C3 matches are not great,
         # the rest are OK:
         tab = [
             [1.773, 40272, 4.603e30, 0.000000, 0.000000, 26.16, 0.000, 0.00],
             [1.053, 43451, 3.229e31, 1.354e31, 9.527e30, 26.98, 26.52, 26.5],
-            [0.893, 39084, 4.097e31, 1.273e31, 2.875e31, 27.12, 26.54, 27.0]
+            [0.893, 39084, 4.097e31, 1.273e31, 2.875e31, 27.12, 26.54, 27.0],
         ]
 
         for rh, rho, NC2, NCN, NC3, QC2, QCN, QC3 in tab:
             if NC2 > 0:
                 parent = 1.0e4 * u.km
                 daughter = 6.61e4 * u.km
-                Q = 10 ** QC2 / u.s
+                Q = 10**QC2 / u.s
                 coma = Haser(Q, 1 * u.km / u.s, parent, daughter)
                 N = coma.total_number(rho * u.km)
                 assert np.isclose(NC2, N, rtol=0.01)
 
             if NCN > 0:
                 parent = 1.3e4 * u.km
                 daughter = 1.48e5 * u.km
-                Q = 10 ** QCN / u.s
+                Q = 10**QCN / u.s
                 coma = Haser(Q, 1 * u.km / u.s, parent, daughter)
                 N = coma.total_number(rho * u.km)
                 assert np.isclose(NCN, N, rtol=0.01)
 
             if NC3 > 0:
                 parent = 0 * u.km
                 daughter = 4.0e4 * u.km
-                Q = 10 ** QC3 / u.s
+                Q = 10**QC3 / u.s
                 coma = Haser(Q, 1 * u.km / u.s, parent, daughter)
                 N = coma.total_number(rho * u.km)
                 assert np.isclose(NC3, N, rtol=0.01)
 
     def test_circular_integration_0step(self):
         """Compare total number and integrated column density for circle.
 
@@ -299,18 +303,16 @@
 
         Q = 1 / u.s
         v = 1 * u.km / u.s
         aper = core.AnnularAperture((1000, 2000) * u.km)
         parent = 10 * u.km
         N = Haser(Q, v, parent).total_number(aper)
 
-        N1 = Haser(Q, v, parent).total_number(
-            core.CircularAperture(aper.dim[0]))
-        N2 = Haser(Q, v, parent).total_number(
-            core.CircularAperture(aper.dim[1]))
+        N1 = Haser(Q, v, parent).total_number(core.CircularAperture(aper.dim[0]))
+        N2 = Haser(Q, v, parent).total_number(core.CircularAperture(aper.dim[1]))
 
         assert np.allclose(N, N2 - N1)
 
     def test_total_number_rectangular_ap(self):
         """
 
         compare with:
@@ -336,15 +338,15 @@
         Q = 5.8e23 / u.s
         v = 1 * u.km / u.s
         aper = core.RectangularAperture([5000, 3300] * u.km)
 
         coma = Haser(Q, v, parent, daughter)
         N = coma.total_number(aper)
 
-        assert np.isclose(N, 3.449607967230623e+26)
+        assert np.isclose(N, 3.449607967230623e26)
 
     def test_total_number_gaussian_ap(self):
         """
 
         Compare with:
 
         import astropy.units as u
@@ -367,159 +369,322 @@
         parent = 1.4e4 * u.km
         Q = 5.8e23 / u.s
         aper = core.GaussianAperture(1e4 * u.km)
 
         coma = Haser(Q, 1 * u.km / u.s, parent)
         N = coma.total_number(aper)
 
-        assert np.isclose(N, 5.146824269306973e+27, rtol=0.005)
+        assert np.isclose(N, 5.146824269306973e27, rtol=0.005)
 
     def test_missing_scipy(self, monkeypatch):
-        monkeypatch.setattr(core, 'scipy', None)
+        monkeypatch.setattr(core, "scipy", None)
         test = Haser(1 / u.s, 1 * u.km / u.s, 1e6 * u.km)
         with pytest.raises(sbe.RequiredPackageUnavailable):
             test._iK0(1)
         with pytest.raises(sbe.RequiredPackageUnavailable):
             test._K1(1)
 
 
 class TestVectorialModel:
+    def test_small_vphoto(self):
+        """
+        The other test using water as parent and hydroxyl as fragment have a
+        v_photo > v_outflow, but the model has a slightly different case for
+        v_photo < v_outflow
+        """
+
+        # Across python, fortran, and rust models, we get very very close to
+        # this number of fragments
+        num_fragments_grid = 1.2162140e33
+
+        base_q = 1.0e28 * 1 / u.s
+
+        # Parent molecule is H2O
+        parent = Phys.from_dict(
+            {
+                "tau_T": 86430 * u.s,
+                "tau_d": 101730 * u.s,
+                "v_outflow": 1 * u.km / u.s,
+                "sigma": 3e-16 * u.cm**2,
+            }
+        )
+        # Fragment molecule is OH, but v_photo is modified to be smaller than
+        # v_outflow
+        fragment = Phys.from_dict(
+            {"tau_T": photo_timescale("OH") * 0.93, "v_photo": 0.5 * u.km / u.s}
+        )
+
+        coma = VectorialModel(
+            base_q=base_q, parent=parent, fragment=fragment
+        )
+
+        assert np.isclose(
+            coma.vmr.num_fragments_grid, num_fragments_grid, rtol=0.02
+        )
+
+    def test_time_dependent_function(self):
+        """
+        Test handing off a time dependence to the model with zero additional
+        time-dependent production from q_t: results should match a model with
+        steady production specified by base_q
+        Also uses a model with print_progress=true to avoid the code coverage
+        tests being polluted with trivial branches about the model
+        conditionally printing
+        """
+        def q_t(t):
+            # for all times, return zero additional production
+            return t * 0
+
+        base_q = 1.0e28 * 1 / u.s
+
+        # Parent molecule is H2O
+        parent = Phys.from_dict(
+            {
+                "tau_T": 86430 * u.s,
+                "tau_d": 101730 * u.s,
+                "v_outflow": 1 * u.km / u.s,
+                "sigma": 3e-16 * u.cm**2,
+            }
+        )
+        # Fragment molecule is OH
+        fragment = Phys.from_dict(
+            {"tau_T": photo_timescale("OH") * 0.93, "v_photo": 1.05 * u.km / u.s}
+        )
+
+        coma_steady = VectorialModel(
+            base_q=base_q, parent=parent, fragment=fragment
+        )
+
+        coma_q_t = VectorialModel(
+            base_q=base_q, parent=parent, fragment=fragment, q_t=q_t,
+            print_progress=True
+        )
+
+        assert np.isclose(
+            coma_steady.vmr.num_fragments_grid, coma_q_t.vmr.num_fragments_grid, rtol=0.02
+        )
+
+    def test_binned_production_one_element_list(self):
+        """
+        Initialize a comet with the fortran-version style of specifying time
+        dependent production and make it essentially steady production, and
+        test against a comet with the same steady production but initialized
+        differently
+        This also tests the model dealing with times in the past farther back
+        than is specified in the variation list 'ts': it extends the oldest
+        production value (here, 1.0e28) back infinitely into the past
+        """
+        # production from 1 day ago until the present,
+        ts = [1] * u.day
+        # is a steady value of 1e28
+        qs = [1.0e28] / u.s
+
+        base_q = 1.0e28 * 1 / u.s
+
+        # Parent molecule is H2O
+        parent = Phys.from_dict(
+            {
+                "tau_T": 86430 * u.s,
+                "tau_d": 101730 * u.s,
+                "v_outflow": 1 * u.km / u.s,
+                "sigma": 3e-16 * u.cm**2,
+            }
+        )
+        # Fragment molecule is OH
+        fragment = Phys.from_dict(
+            {"tau_T": photo_timescale("OH") * 0.93, "v_photo": 1.05 * u.km / u.s}
+        )
+
+        coma_binned = VectorialModel.binned_production(
+            qs=qs, ts=ts, parent=parent, fragment=fragment
+        )
+
+        coma_steady = VectorialModel(
+            base_q=base_q, parent=parent, fragment=fragment
+        )
+
+        assert np.isclose(
+            coma_steady.vmr.num_fragments_grid, coma_binned.vmr.num_fragments_grid, rtol=0.02
+        )
+
+    def test_binned_production_multi_element_list(self):
+        """
+        Initialize a comet with the fortran-version style of specifying time
+        dependent production and make it steady production, then test against a
+        comet with the same steady production but initialized differently
+        """
+        # Specify that at multiple points in time,
+        ts = [60, 50, 40, 30, 20, 10] * u.day
+        # production is a steady value of 1e28
+        qs = [1.0e28, 1.0e28, 1.0e28, 1.0e28, 1.0e28, 1.0e28] / u.s
+
+        base_q = 1.0e28 * 1 / u.s
+
+        # Parent molecule is H2O
+        parent = Phys.from_dict(
+            {
+                "tau_T": 86430 * u.s,
+                "tau_d": 101730 * u.s,
+                "v_outflow": 1 * u.km / u.s,
+                "sigma": 3e-16 * u.cm**2,
+            }
+        )
+        # Fragment molecule is OH
+        fragment = Phys.from_dict(
+            {"tau_T": photo_timescale("OH") * 0.93, "v_photo": 1.05 * u.km / u.s}
+        )
+
+        coma_binned = VectorialModel.binned_production(
+            qs=qs, ts=ts, parent=parent, fragment=fragment
+        )
+
+        coma_steady = VectorialModel(
+            base_q=base_q, parent=parent, fragment=fragment
+        )
+
+        assert np.isclose(
+            coma_steady.vmr.num_fragments_grid, coma_binned.vmr.num_fragments_grid, rtol=0.02
+        )
 
     def test_grid_count(self):
         """
-            Compute theoretical number of fragments vs. integrated value from
-            grid. This is currently only a good estimate for steady production
-            due to our method for determining the theoretical count of
-            fragments
+        Compute theoretical number of fragments vs. integrated value from
+        grid. This is currently only a good estimate for steady production
+        due to our method for determining the theoretical count of
+        fragments
         """
 
-        base_q = 1.e28 * 1 / u.s
+        base_q = 1.0e28 * 1 / u.s
 
         # Parent molecule is H2O
-        parent = Phys.from_dict({
-            'tau_T': 86430 * u.s,
-            'tau_d': 101730 * u.s,
-            'v_outflow': 1 * u.km / u.s,
-            'sigma': 3e-16 * u.cm ** 2
-        })
+        parent = Phys.from_dict(
+            {
+                "tau_T": 86430 * u.s,
+                "tau_d": 101730 * u.s,
+                "v_outflow": 1 * u.km / u.s,
+                "sigma": 3e-16 * u.cm**2,
+            }
+        )
         # Fragment molecule is OH
-        fragment = Phys.from_dict({
-            'tau_T': photo_timescale('OH') * 0.93,
-            'v_photo': 1.05 * u.km / u.s
-        })
-
-        coma = VectorialModel(base_q=base_q,
-                              parent=parent,
-                              fragment=fragment)
-
-        fragment_theory = coma.vmodel['num_fragments_theory']
-        fragment_grid = coma.vmodel['num_fragments_grid']
-        assert np.isclose(fragment_theory, fragment_grid, rtol=0.02)
+        fragment = Phys.from_dict(
+            {"tau_T": photo_timescale("OH") * 0.93, "v_photo": 1.05 * u.km / u.s}
+        )
+
+        coma = VectorialModel(base_q=base_q, parent=parent, fragment=fragment)
+
+        assert np.isclose(
+            coma.vmr.num_fragments_theory, coma.vmr.num_fragments_grid, rtol=0.02
+        )
 
     def test_total_number_large_aperture(self):
         """
-            Compare theoretical number of fragments vs. integration of column
-            density over a large aperture
+        Compare theoretical number of fragments vs. integration of column
+        density over a large aperture
         """
 
         base_q = 1e28 * 1 / u.s
 
         # Parent molecule is H2O
-        parent = Phys.from_dict({
-            'tau_T': 86430 * u.s,
-            'tau_d': 101730 * u.s,
-            'v_outflow': 1 * u.km / u.s,
-            'sigma': 3e-16 * u.cm ** 2
-        })
+        parent = Phys.from_dict(
+            {
+                "tau_T": 86430 * u.s,
+                "tau_d": 101730 * u.s,
+                "v_outflow": 1 * u.km / u.s,
+                "sigma": 3e-16 * u.cm**2,
+            }
+        )
         # Fragment molecule is OH
-        fragment = Phys.from_dict({
-            'tau_T': photo_timescale('OH') * 0.93,
-            'v_photo': 1.05 * u.km / u.s
-        })
-
-        coma = VectorialModel(base_q=base_q,
-                              parent=parent,
-                              fragment=fragment)
-
-        fragment_theory = coma.vmodel['num_fragments_theory']
-        ap = core.CircularAperture(coma.vmodel['max_grid_radius'])
-        assert np.isclose(fragment_theory, coma.total_number(ap), rtol=0.02)
+        fragment = Phys.from_dict(
+            {"tau_T": photo_timescale("OH") * 0.93, "v_photo": 1.05 * u.km / u.s}
+        )
+
+        coma = VectorialModel(base_q=base_q, parent=parent, fragment=fragment)
+
+        ap = core.CircularAperture(coma.vmr.max_grid_radius)
+        assert np.isclose(
+            coma.vmr.num_fragments_theory, coma.total_number(ap), rtol=0.02
+        )
 
     def test_model_symmetry(self):
         """
-            The symmetry of the model allows the parent production to be
-            treated as an overall scaling factor, and does not affect the
-            features of the calculated densities.
-
-            If we assume an arbitrary fixed count inside an aperture, we can
-            use this to calculate what the production would need to be to
-            produce this count after running the model with a 'dummy' value for
-            the production.
-
-            If we then run another model at this calculated production and use
-            the same aperture, we should recover the number of counts assumed
-            in the paragraph above.  If we do not, we have broken our model
-            somehow and lost the symmetry during our calculations.
+        The symmetry of the model allows the parent production to be
+        treated as an overall scaling factor, and does not affect the
+        features of the calculated densities.
+
+        If we assume an arbitrary fixed count inside an aperture, we can
+        use this to calculate what the production would need to be to
+        produce this count after running the model with a 'dummy' value for
+        the production.
+
+        If we then run another model at this calculated production and use
+        the same aperture, we should recover the number of counts assumed
+        in the paragraph above.  If we do not, we have broken our model
+        somehow and lost the symmetry during our calculations.
         """
 
-        base_production = 1e26
+        base_production = 1e28
 
         # # 100,000 x 100,000 km aperture
-        ap = core.RectangularAperture((1.0e5, 1.0e5) * u.km)
+        ap = core.CircularAperture((1.0e6) * u.km)
         # assumed fragment count inside this aperture
-        assumed_count = 1e30
+        assumed_count = 1e32
 
         # Parent molecule is H2O
-        parent = Phys.from_dict({
-            'tau_T': 86430 * u.s,
-            'tau_d': 101730 * u.s,
-            'v_outflow': 1 * u.km / u.s,
-            'sigma': 3e-16 * u.cm ** 2
-        })
+        parent = Phys.from_dict(
+            {
+                "tau_T": 86430 * u.s,
+                "tau_d": 101730 * u.s,
+                "v_outflow": 1 * u.km / u.s,
+                "sigma": 3e-16 * u.cm**2,
+            }
+        )
         # Fragment molecule is OH
-        fragment = Phys.from_dict({
-            'tau_T': photo_timescale('OH') * 0.93,
-            'v_photo': 1.05 * u.km / u.s
-        })
-
-        coma = VectorialModel(base_q=base_production * (1 / u.s),
-                              parent=parent,
-                              fragment=fragment)
-        # mgr = coma.vmodel['max_grid_radius']
-        # ap = core.RectangularAperture((mgr, mgr))
+        fragment = Phys.from_dict(
+            {"tau_T": photo_timescale("OH") * 0.93, "v_photo": 1.05 * u.km / u.s}
+        )
+
+        coma = VectorialModel(
+            base_q=base_production * (1 / u.s), parent=parent, fragment=fragment
+        )
+
         model_count = coma.total_number(ap)
         calculated_q = (assumed_count / model_count) * base_production
-        print("Calculated: ", calculated_q)
 
-        # Parent molecule is H2O
-        parent_check = Phys.from_dict({
-            'tau_T': 86430 * u.s,
-            'tau_d': 101730 * u.s,
-            'v_outflow': 1 * u.km / u.s,
-            'sigma': 3e-16 * u.cm ** 2
-        })
-        # Fragment molecule is OH
-        fragment_check = Phys.from_dict({
-            'tau_T': photo_timescale('OH') * 0.93,
-            'v_photo': 1.05 * u.km / u.s
-        })
-        coma_check = VectorialModel(base_q=calculated_q * (1 / u.s),
-                                    parent=parent_check,
-                                    fragment=fragment_check)
+        # # Parent molecule is H2O
+        # parent_check = Phys.from_dict({
+        #     'tau_T': 86430 * u.s,
+        #     'tau_d': 101730 * u.s,
+        #     'v_outflow': 1 * u.km / u.s,
+        #     'sigma': 3e-16 * u.cm ** 2
+        # })
+        # # Fragment molecule is OH
+        # fragment_check = Phys.from_dict({
+        #     'tau_T': photo_timescale('OH') * 0.93,
+        #     'v_photo': 1.05 * u.km / u.s
+        # })
+        # coma_check = VectorialModel(base_q=calculated_q * (1 / u.s),
+        #                             parent=parent_check,
+        #                             fragment=fragment_check)
+        coma_check = VectorialModel(
+            base_q=calculated_q * (1 / u.s), parent=parent, fragment=fragment
+        )
         count_check = coma_check.total_number(ap)
-        print("Count/assumed: ", count_check / assumed_count)
+
         assert np.isclose(count_check, assumed_count, rtol=0.001)
 
-    @pytest.mark.parametrize("rh,delta,flux,g,Q", (
-        [1.2912, 0.7410, 337e-14, 2.33e-4, 1.451e28],
-        [1.2949, 0.7651, 280e-14, 2.60e-4, 1.228e28],
-        [1.3089, 0.8083, 480e-14, 3.36e-4, 1.967e28],
-        [1.3200, 0.8353, 522e-14, 3.73e-4, 2.025e28],
-        [1.3366, 0.8720, 560e-14, 4.03e-4, 2.035e28],
-    ))
+    @pytest.mark.parametrize(
+        "rh,delta,flux,g,Q",
+        (
+            [1.2912, 0.7410, 337e-14, 2.33e-4, 1.451e28],
+            [1.2949, 0.7651, 280e-14, 2.60e-4, 1.228e28],
+            [1.3089, 0.8083, 480e-14, 3.36e-4, 1.967e28],
+            [1.3200, 0.8353, 522e-14, 3.73e-4, 2.025e28],
+            [1.3366, 0.8720, 560e-14, 4.03e-4, 2.035e28],
+        ),
+    )
     def test_festou92(self, rh, delta, flux, g, Q):
         """Compare to Festou et al. 1992 production rates of comet 6P/d'Arrest.
 
         Festou et al. 1992. The Gas Production Rate of Periodic Comet d'Arrest.
         Asteroids, Comets, Meteors 1991, 177.
 
         https://ui.adsabs.harvard.edu/abs/1992acm..proc..177F/abstract
@@ -530,34 +695,34 @@
         observation: using 2.025 instead of 3.025.
 
         """
 
         # add units
         rh = rh * u.au
         delta = delta * u.au
-        flux = flux * u.erg / u.s / u.cm ** 2
+        flux = flux * u.erg / u.s / u.cm**2
         g = g / u.s
         Q = Q / u.s
 
         # OH (0-0) luminosity per molecule
         L_N = g / (rh / u.au) ** 2 * const.h * const.c / (3086 * u.AA)
 
         # Parent molecule is H2O
-        parent = Phys.from_dict({
-            'tau_T': 65000 * (rh / u.au) ** 2 * u.s,
-            'tau_d': 72500 * (rh / u.au) ** 2 * u.s,
-            'v_outflow': 0.85 * u.km / u.s,
-            'sigma': 3e-16 * u.cm ** 2,
-
-        })
+        parent = Phys.from_dict(
+            {
+                "tau_T": 65000 * (rh / u.au) ** 2 * u.s,
+                "tau_d": 72500 * (rh / u.au) ** 2 * u.s,
+                "v_outflow": 0.85 * u.km / u.s,
+                "sigma": 3e-16 * u.cm**2,
+            }
+        )
         # Fragment molecule is OH
-        fragment = Phys.from_dict({
-            'tau_T': 160000 * (rh / u.au) ** 2 * u.s,
-            'v_photo': 1.05 * u.km / u.s
-        })
+        fragment = Phys.from_dict(
+            {"tau_T": 160000 * (rh / u.au) ** 2 * u.s, "v_photo": 1.05 * u.km / u.s}
+        )
 
         # https://pds.nasa.gov/ds-view/pds/viewInstrumentProfile.jsp?INSTRUMENT_ID=LWP&INSTRUMENT_HOST_ID=IUE
         # Large-Aperture Length(arcsec)   22.51+/-0.40
         # Large-Aperture Width(arcsec)     9.91+/-0.17
         #
         # 10x20 quoted by Festou et al.
         # effective circle is 8.0 radius
@@ -566,126 +731,86 @@
         # However, vectorial fortran code has 9.1x15.3 hard coded into it.
         lwp = core.RectangularAperture((9.1, 15.3) * u.arcsec)
 
         Q0 = 1e28 / u.s
         coma = VectorialModel(base_q=Q0, parent=parent, fragment=fragment)
         N0 = coma.total_number(lwp, eph=delta)
 
-        Q_model = (Q0 * flux / (L_N * N0) * 4 * np.pi * delta ** 2).to(Q.unit)
+        Q_model = (Q0 * flux / (L_N * N0) * 4 * np.pi * delta**2).to(Q.unit)
 
         # absolute tolerance: Table 2 has 3 significant figures
         #
         # relative tolerance: actual agreement is 14%, future updates should
         # improve this or else explain the difference
         atol = 1.01 * 10 ** (np.floor(np.log10(Q0.value)) - 2) * Q.unit
         assert u.allclose(Q, Q_model, atol=atol, rtol=0.14)
 
-    @pytest.mark.parametrize("rh,delta,N,Q", (
-        [1.8662, 0.9683, 0.2424e32, 1.048e29],
-        [0.8855, 0.9906, 3.819e32, 5.548e29],
-        [0.9787, 0.8337, 1.63e32, 3.69e29],
-        [1.0467, 0.7219, 0.8703e32, 2.813e29],
-        [1.9059, 1.4031, 1.07e32, 2.76e29],
-        [2.0715, 1.7930, 1.01e32, 1.88e29]
-    ))
+    @pytest.mark.parametrize(
+        "rh,delta,N,Q",
+        (
+            [1.8662, 0.9683, 0.2424e32, 1.048e29],
+            [0.8855, 0.9906, 3.819e32, 5.548e29],
+            [0.9787, 0.8337, 1.63e32, 3.69e29],
+            [1.0467, 0.7219, 0.8703e32, 2.813e29],
+            [1.9059, 1.4031, 1.07e32, 2.76e29],
+            [2.0715, 1.7930, 1.01e32, 1.88e29],
+        ),
+    )
     def test_combi93(self, rh, delta, N, Q):
         """Compare to results of Combi et al. 1993.
 
-        Combi et al. 1993 compared a Monte Carlo approach to the Vectorial model
-        for OH.  They find best agreement between the two models near 1 au,
-        likely due to the assumption that the water outflow speed is constant in
-        the VM runs, but the MC model only has 1 km/s speeds near 1 au.
+        Combi et al. 1993 compared a Monte Carlo approach to the Vectorial
+        model for OH.  They find best agreement between the two models near 1
+        au, likely due to the assumption that the water outflow speed is
+        constant in the VM runs, but the MC model only has 1 km/s speeds near 1
+        au.
 
         """
 
         # assign units
         rh = rh * u.au
         delta = delta * u.au
         Q = Q / u.s  # Vectorial model run by Roettger
         aper = core.RectangularAperture((10, 15) * u.arcsec)
 
         # Parent molecule is H2O
-        parent = Phys.from_dict({
-            'tau_T': 8.2e4 * 0.88 * (rh / u.au) ** 2 * u.s,
-            'tau_d': 8.2e4 * (rh / u.au) ** 2 * u.s,
-            'v_outflow': 1 * u.km / u.s,
-            'sigma': 3e-16 * u.cm ** 2,
-        })
+        parent = Phys.from_dict(
+            {
+                "tau_T": 8.2e4 * 0.88 * (rh / u.au) ** 2 * u.s,
+                "tau_d": 8.2e4 * (rh / u.au) ** 2 * u.s,
+                "v_outflow": 1 * u.km / u.s,
+                "sigma": 3e-16 * u.cm**2,
+            }
+        )
 
         # Fragment molecule is OH
-        fragment = Phys.from_dict({
-            'tau_T': 2.0e5 * (rh / u.au) ** 2 * u.s,
-            'v_photo': 1.05 * u.km / u.s
-        })
-
-        Q0 = 2e29 / u.s
-        coma = VectorialModel(base_q=Q0, parent=parent, fragment=fragment)
-        N0 = coma.total_number(aper, eph=delta)
-
-        Q_model = (Q0 * N / N0).to(Q.unit)
-        assert u.allclose(Q, Q_model, rtol=0.13)
-
-    @pytest.mark.parametrize("rh,delta,N,Q", (
-        [1.8662, 0.9683, 0.2424e32, 1.048e29],
-        [0.8855, 0.9906, 3.819e32, 5.548e29],
-        [0.9787, 0.8337, 1.63e32, 3.69e29],
-        [1.0467, 0.7219, 0.8703e32, 2.813e29],
-        [1.9059, 1.4031, 1.07e32, 2.76e29],
-        [2.0715, 1.7930, 1.01e32, 1.88e29]
-    ))
-    def test_combi93(self, rh, delta, N, Q):
-        """Compare to results of Combi et al. 1993.
-
-        Combi et al. 1993 compared a Monte Carlo approach to the Vectorial model
-        for OH.  They find best agreement between the two models near 1 au,
-        likely due to the assumption that the water outflow speed is constant in
-        the VM runs, but the MC model only has 1 km/s speeds near 1 au.
-
-        """
-
-        # assign units
-        rh = rh * u.au
-        delta = delta * u.au
-        Q = Q / u.s  # Vectorial model run by Roettger
-        aper = core.RectangularAperture((10, 15) * u.arcsec)
-
-        # Parent molecule is H2O
-        parent = Phys.from_dict({
-            'tau_T': 8.2e4 * 0.88 * (rh / u.au) ** 2 * u.s,
-            'tau_d': 8.2e4 * (rh / u.au) ** 2 * u.s,
-            'v_outflow': 1 * u.km / u.s,
-            'sigma': 3e-16 * u.cm ** 2,
-        })
-
-        # Fragment molecule is OH
-        fragment = Phys.from_dict({
-            'tau_T': 2.0e5 * (rh / u.au) ** 2 * u.s,
-            'v_photo': 1.05 * u.km / u.s
-        })
+        fragment = Phys.from_dict(
+            {"tau_T": 2.0e5 * (rh / u.au) ** 2 * u.s, "v_photo": 1.05 * u.km / u.s}
+        )
 
         Q0 = 2e29 / u.s
         coma = VectorialModel(base_q=Q0, parent=parent, fragment=fragment)
         N0 = coma.total_number(aper, eph=delta)
 
         Q_model = (Q0 * N / N0).to(Q.unit)
         assert u.allclose(Q, Q_model, rtol=0.13)
 
     def test_vm_fortran(self):
         """Compare to results from vm.f.
 
         vm.f shared with MSK by Joel Parker.  Comments:
 
             WRITTEN BY M. C. FESTOU
-            (Minor modifications were made by MF on 8 Nov. 1988 on the Tempe version)
-            Some unused variables removed on 6 June 1995 in Baltimore when adapting
-            the code to run on a unix machine. A little bit of additional trimming
-            on 27 June 1995. New printing formats.
-            Few printing format changes made on 27 Sept. 96.
-            Formula on the collision radius added on 1 April 1997.
-            Modification in sub GAUSS (NP and coeff.) and in sub APP on 22-24/4/1997.
+            (Minor modifications were made by MF on 8 Nov. 1988 on the Tempe
+            version) Some unused variables removed on 6 June 1995 in Baltimore
+            when adapting the code to run on a unix machine. A little bit of
+            additional trimming on 27 June 1995. New printing formats.  Few
+            printing format changes made on 27 Sept. 96.  Formula on the
+            collision radius added on 1 April 1997.  Modification in sub GAUSS
+            (NP and coeff.) and in sub APP on 22-24/4/1997.
 
         Input fparam.dat:
 
             Wirtanen (HST-FOS slit)
             2.46900010       1.51400006
                     1
             9.99999988E+26   100.000000
@@ -719,53 +844,58 @@
             95.0000000
             1.28999996       3.66000009
 
         Results: see wm_fortran_test_output.txt in data directory.
 
         """
 
-        eph = {'rh': 2.469 * u.au, 'delta': 1.514 * u.au}
+        eph = {"rh": 2.469 * u.au, "delta": 1.514 * u.au}
 
         # Parent molecule is H2O
-        parent = Phys.from_dict({
-            'tau_T': 86430 * (eph['rh'] / u.au) ** 2 * u.s,
-            'tau_d': 101730 * (eph['rh'] / u.au) ** 2 * u.s,
-            'v_outflow': 0.514 * u.km / u.s,
-            'sigma': 3e-16 * u.cm ** 2,
-
-        })
+        parent = Phys.from_dict(
+            {
+                "tau_T": 86430 * (eph["rh"] / u.au) ** 2 * u.s,
+                "tau_d": 101730 * (eph["rh"] / u.au) ** 2 * u.s,
+                "v_outflow": 0.514 * u.km / u.s,
+                "sigma": 3e-16 * u.cm**2,
+            }
+        )
         # Fragment molecule is OH
-        fragment = Phys.from_dict({
-            'tau_T': 129000 * (eph['rh'] / u.au) ** 2 * u.s,
-            'v_photo': 1.05 * u.km / u.s
-        })
+        fragment = Phys.from_dict(
+            {
+                "tau_T": 129000 * (eph["rh"] / u.au) ** 2 * u.s,
+                "v_photo": 1.05 * u.km / u.s,
+            }
+        )
 
         # test values are copy-pasted from wm.f output
-        collision_sphere_radius = 0.14E+07 * u.cm
+        collision_sphere_radius = 0.14e07 * u.cm
         collision_sphere_radius_atol = 0.011e7 * u.cm
-        N_fragments_theory = 0.668E+33
-        N_fragments_theory_atol = 0.0011e33
-        N_fragments = 0.657E+33
-        N_fragments_atol = 0.0011e33
+        N_fragments_theory = 0.668e33
+        # N_fragments_theory_atol = 0.0011e33
+        N_fragments_theory_rtol = 0.001
+        N_fragments = 0.657e33
+        # N_fragments_atol = 0.0011e33
+        N_fragments_rtol = 0.003
 
-        fragment_volume_density = '''
+        fragment_volume_density = """
 0.97E+03  0.43E+03    0.68E+04  0.59E+02    0.13E+05  0.31E+02    0.18E+05  0.21E+02
 0.24E+05  0.15E+02    0.31E+05  0.11E+02    0.43E+05  0.79E+01    0.54E+05  0.59E+01
 0.66E+05  0.46E+01    0.78E+05  0.38E+01    0.90E+05  0.31E+01    0.11E+06  0.24E+01
 0.13E+06  0.19E+01    0.14E+06  0.16E+01    0.16E+06  0.13E+01    0.18E+06  0.11E+01
 0.21E+06  0.87E+00    0.24E+06  0.69E+00    0.27E+06  0.56E+00    0.30E+06  0.46E+00
 0.33E+06  0.38E+00    0.37E+06  0.29E+00    0.42E+06  0.23E+00    0.47E+06  0.18E+00
 0.51E+06  0.14E+00    0.56E+06  0.11E+00    0.63E+06  0.85E-01    0.70E+06  0.65E-01
 0.77E+06  0.50E-01    0.84E+06  0.39E-01    0.92E+06  0.30E-01    0.10E+07  0.21E-01
 0.11E+07  0.16E-01    0.12E+07  0.12E-01    0.13E+07  0.86E-02    0.14E+07  0.64E-02
 0.16E+07  0.44E-02    0.17E+07  0.31E-02    0.19E+07  0.23E-02    0.20E+07  0.17E-02
 0.22E+07  0.12E-02    0.24E+07  0.78E-03    0.27E+07  0.51E-03    0.29E+07  0.34E-03
 0.31E+07  0.23E-03    0.34E+07  0.15E-03    0.37E+07  0.90E-04    0.41E+07  0.53E-04
-0.44E+07  0.32E-04    0.48E+07  0.20E-04'''
-        fragment_column_density = '''
+0.44E+07  0.32E-04    0.48E+07  0.20E-04"""
+        fragment_column_density = """
 0.970E+03   4.77E+11    1.088E+03   4.69E+11    1.221E+03   4.61E+11    1.370E+03   4.53E+11
 1.537E+03   4.44E+11    1.724E+03   4.34E+11    1.935E+03   4.22E+11    2.171E+03   4.15E+11
 2.436E+03   4.00E+11    2.733E+03   3.85E+11    3.066E+03   3.74E+11    3.441E+03   3.67E+11
 3.860E+03   3.57E+11    4.332E+03   3.47E+11    4.860E+03   3.36E+11    5.453E+03   3.27E+11
 6.118E+03   3.18E+11    6.865E+03   3.08E+11    7.703E+03   2.99E+11    8.643E+03   2.89E+11
 9.697E+03   2.79E+11    1.088E+04   2.70E+11    1.221E+04   2.61E+11    1.370E+04   2.51E+11
 1.537E+04   2.42E+11    1.724E+04   2.32E+11    1.935E+04   2.23E+11    2.171E+04   2.13E+11
@@ -776,45 +906,50 @@
 1.537E+05   6.89E+10    1.724E+05   6.21E+10    1.935E+05   5.56E+10    2.171E+05   4.95E+10
 2.436E+05   4.37E+10    2.733E+05   3.83E+10    3.066E+05   3.32E+10    3.441E+05   2.86E+10
 3.860E+05   2.43E+10    4.332E+05   2.05E+10    4.860E+05   1.71E+10    5.453E+05   1.40E+10
 6.118E+05   1.14E+10    6.865E+05   9.11E+09    7.703E+05   7.18E+09    8.643E+05   5.57E+09
 9.697E+05   4.25E+09    1.088E+06   3.19E+09    1.221E+06   2.34E+09    1.370E+06   1.68E+09
 1.537E+06   1.19E+09    1.724E+06   8.29E+08    1.935E+06   5.67E+08    2.171E+06   3.78E+08
 2.436E+06   2.45E+08    2.733E+06   1.54E+08    3.066E+06   9.34E+07    3.441E+06   5.39E+07
-'''
+"""
 
         # convert strings to arrays
-        x = np.fromstring(fragment_volume_density, sep=' ')
+        x = np.fromstring(fragment_volume_density, sep=" ")
         n0_rho = x[::2] * u.km
-        n0 = x[1::2] / u.cm ** 3
+        n0 = x[1::2] / u.cm**3
         # absolute tolerance: 2 significant figures
         n0_atol = 1.1 * 10 ** (np.floor(np.log10(n0.value)) - 1) * n0.unit
         n0_atol_revised = n0_atol * 7
 
-        x = np.fromstring(fragment_column_density, sep=' ')
+        x = np.fromstring(fragment_column_density, sep=" ")
         sigma0_rho = x[::2] * u.km
-        sigma0 = x[1::2] / u.cm ** 2
+        sigma0 = x[1::2] / u.cm**2
         # absolute tolerance: 3 significant figures
-        sigma0_atol = (1.1 * 10 ** (np.floor(np.log10(sigma0.value)) - 2)
-                       * sigma0.unit)
+        sigma0_atol = 1.1 * 10 ** (np.floor(np.log10(sigma0.value)) - 2) * sigma0.unit
         sigma0_atol_revised = sigma0_atol * 40
 
         # evaluate the model
         Q0 = 1e27 / u.s
         coma = VectorialModel(base_q=Q0, parent=parent, fragment=fragment)
-        n = coma.volume_density(n0_rho)
-        sigma = coma.column_density(sigma0_rho)
+        n = [coma.volume_density(r) for r in n0_rho]
+        sigma = [coma.column_density(r) for r in sigma0_rho]
 
         # compare results
-        assert u.isclose(coma.vmodel['collision_sphere_radius'],
-                         collision_sphere_radius,
-                         atol=collision_sphere_radius_atol)
+        assert u.isclose(
+            coma.vmr.collision_sphere_radius,
+            collision_sphere_radius,
+            atol=collision_sphere_radius_atol,
+        )
 
-        assert np.isclose(coma.calc_num_fragments_theory(),
-                          N_fragments_theory, atol=N_fragments_theory_atol)
+        assert np.isclose(
+            coma.vmr.num_fragments_theory,
+            N_fragments_theory,
+            rtol=N_fragments_theory_rtol,
+        )
 
-        assert np.isclose(coma.calc_num_fragments_grid(),
-                          N_fragments, atol=N_fragments_atol)
+        assert np.isclose(
+            coma.vmr.num_fragments_grid, N_fragments, rtol=N_fragments_rtol
+        )
 
         assert u.allclose(n, n0, atol=n0_atol_revised)
 
         assert u.allclose(sigma, sigma0, atol=sigma0_atol_revised)
```

### Comparing `sbpy-0.3.0/sbpy/activity/gas/tests/test_data.py` & `sbpy-0.4.0/sbpy/activity/gas/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/activity/gas/tests/test_prodrate.py` & `sbpy-0.4.0/sbpy/activity/gas/tests/test_prodrate.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/activity/gas/tests/test_prodrate_remote.py` & `sbpy-0.4.0/sbpy/activity/gas/tests/test_prodrate_remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 import numpy as np
 import astropy.units as u
 from astropy.time import Time
-from astropy.tests.helper import remote_data
 from astropy.table import Table
 from astroquery.lamda import Lamda
 from astroquery.jplspec import JPLSpec
 import pytest
 
 try:
     import pyradex
@@ -60,16 +59,17 @@
 
 
 def data_path(filename):
     data_dir = os.path.join(os.path.dirname(__file__), 'data')
     return os.path.join(data_dir, filename)
 
 
-@remote_data
+@pytest.mark.remote_data
 def test_remote_prodrate_simple_hcn():
+    pytest.importorskip("astroquery", minversion="0.4.7")
 
     hcn = Table.read(data_path('HCN.csv'), format="ascii.csv")
 
     temp_estimate = 47. * u.K
     target = '103P'
     vgas = 0.8 * u.km / u.s
     aper = 30 * u.m  # The aperture for telescope used (Drahus et al. 2012)
@@ -105,16 +105,17 @@
     np.testing.assert_almost_equal(q_pred, q_found, decimal=1.3)
 
     err = abs((np.array(q_pred) - np.array(q_found)) / np.array(q_pred) * 100)
 
     assert np.all(err < 0.2345)
 
 
-@remote_data
+@pytest.mark.remote_data
 def test_remote_prodrate_simple_ch3oh():
+    pytest.importorskip("astroquery", minversion="0.4.7")
 
     ch3oh = Table.read(data_path('CH3OH.csv'), format="ascii.csv")
     temp_estimate = 47. * u.K
     target = '103P'
     vgas = 0.8 * u.km / u.s
     aper = 30 * u.m  # The aperture for telescope used (Drahus et al. 2012)
     b = 1.13  # Value taken from (Drahus et al. 2012)
@@ -150,16 +151,17 @@
 
     assert np.all(err < 0.35)
 
 
 # Issue #296
 # MSK: disabling test as CO and HCN are no longer present in LAMDA database(?)
 @pytest.mark.skip
-@remote_data
+@pytest.mark.remote_data
 def test_einstein():
+    pytest.importorskip("astroquery", minversion="0.4.7")
 
     transition_freq_list = [(1611.7935180 * u.GHz).to('MHz'),
                             (177.26111120 * u.GHz).to('MHz')]
     mol_tag_list = [28001, 27001]
     temp_estimate = 300. * u.K
 
     result = []
@@ -200,16 +202,17 @@
 
     err = (abs((np.array(catalog_result) - np.array(result)) /
                np.array(catalog_result) * 100))
 
     assert np.all(err < 23.5)
 
 
-@remote_data
+@pytest.mark.remote_data
 def test_Haser_prodrate():
+    pytest.importorskip("astroquery", minversion="0.4.7")
 
     co = Table.read(data_path('CO.csv'), format="ascii.csv")
 
     lte = LTE()
     Q_estimate = 2.8*10**(28) / u.s
     transition_freq = (230.53799 * u.GHz).to('MHz')
     aper = 10 * u.m
@@ -262,16 +265,18 @@
 Tested: locally, needs pyradex to be installed
 Status: Passed
 See https://github.com/keflavich/pyradex for installment
 '''
 
 
 @pytest.mark.skipif('pyradex is None')
-@remote_data
+@pytest.mark.remote_data
 def test_Haser_pyradex():
+    pytest.importorskip("astroquery", minversion="0.4.7")
+
     co = Table.read(data_path('CO.csv'), format="ascii.csv")
 
     nonlte = NonLTE()
     lte = LTE()
     Q_estimate = 2.8*10**(28) / u.s
     transition_freq = (230.53799 * u.GHz).to('MHz')
     aper = 10 * u.m
@@ -315,48 +320,50 @@
     q_pred = list(co['log(Q)'])
 
     err = abs((np.array(q_pred) - np.array(q_found)) / np.array(q_pred) * 100)
 
     assert np.all(err < 0.35)
 
 
-@remote_data
+@pytest.mark.remote_data
 def test_intensity_conversion():
     # test untested case for intensity conversion function
+    pytest.importorskip("astroquery", minversion="0.4.7")
 
     temp_estimate = 47. * u.K
     # vgas = 0.8 * u.km / u.s
     mol_tag = 27001
     transition_freq = (265.886434 * u.GHz).to('MHz')
     mol_data = Phys.from_jplspec(temp_estimate, transition_freq, mol_tag)
     mol_data['eup_J'] = 3.52359898e-20 * u.J
     mol_data['elo_J'] = 1.76181853e-20 * u.J
     intl = intensity_conversion(mol_data)
 
     assert np.isclose(intl.value, 6.186509000388917e-11)
 
 
-@remote_data
+@pytest.mark.remote_data
 def test_einsteincoeff_case():
     # test untested case for einstein coefficient
+    pytest.importorskip("astroquery", minversion="0.4.7")
 
     temp_estimate = 47. * u.K
     # vgas = 0.8 * u.km / u.s
     mol_tag = 27001
     transition_freq = (265.886434 * u.GHz).to('MHz')
     mol_data = Phys.from_jplspec(temp_estimate, transition_freq, mol_tag)
     mol_data['t_freq'] = 2658864.34 * u.MHz
     intl = intensity_conversion(mol_data)
     mol_data.apply([intl.value] * intl.unit, name='intl')
     au = einstein_coeff(mol_data)
 
     assert np.isclose(round(au.value, 4), 0.0086)
 
 
-@remote_data
+@pytest.mark.remote_data
 def test_betafactor_case():
     # test untested case for beta beta_factor
 
     r = 1.06077567 * u.AU
     delta = 0.14633757 * u.AU
     quanteph = [r, delta]
     nameseph = ['r', 'delta']
@@ -377,16 +384,18 @@
 Tested: locally, needs pyradex to be installed
 Status: Passed
 See https://github.com/keflavich/pyradex for installment
 '''
 
 
 @pytest.mark.skipif('pyradex is None')
-@remote_data
+@pytest.mark.remote_data
 def test_pyradex_case():
+    pytest.importorskip("astroquery", minversion="0.4.7")
+
     transition_freq = (177.196 * u.GHz).to(u.MHz)
     mol_tag = 29002
     cdensity_guess = (1.89*10.**(14) / (u.cm * u.cm))
     temp_estimate = 20. * u.K
     temp_back = 2.8 * u.K
 
     mol_data = Phys.from_jplspec(temp_estimate, transition_freq, mol_tag)
@@ -398,16 +407,17 @@
     cdensity = nonLTE.from_pyradex(1.234 * u.K * u.km / u.s, mol_data,
                                    iter=100, collider_density={'H2': 900})
 
     assert np.isclose(cdensity.value[0], 1.134e14)
 
 
 @pytest.mark.skipif('pyradex is None')
-@remote_data
+@pytest.mark.remote_data
 def test_Haser_prodrate_pyradex(mock_nonlte):
+    pytest.importorskip("astroquery", minversion="0.4.7")
 
     co = Table.read(data_path('CO.csv'), format="ascii.csv")
 
     nonlte = NonLTE()
     lte = LTE()
     Q_estimate = 2.8*10**(28) / u.s
     transition_freq = (230.53799 * u.GHz).to('MHz')
@@ -452,16 +462,17 @@
     q_pred = list(co['log(Q)'])
 
     err = abs((np.array(q_pred) - np.array(q_found)) / np.array(q_pred) * 100)
 
     assert np.all(err < 0.35)
 
 
-@remote_data
+@pytest.mark.remote_data
 def test_pyradex_cdensity(mock_nonlte):
+    pytest.importorskip("astroquery", minversion="0.4.7")
 
     transition_freq = (177.196 * u.GHz).to(u.MHz)
     mol_tag = 29002
     cdensity_guess = (1.89*10.**(14) / (u.cm * u.cm))
     temp_estimate = 20. * u.K
     temp_back = 2.8 * u.K
```

### Comparing `sbpy-0.3.0/sbpy/activity/tests/test_core.py` & `sbpy-0.4.0/sbpy/activity/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/activity/tests/test_dust.py` & `sbpy-0.4.0/sbpy/activity/tests/test_dust.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/bib/core.py` & `sbpy-0.4.0/sbpy/bib/core.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/bib/tests/test_bib.py` & `sbpy-0.4.0/sbpy/bib/tests/test_bib.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/calib/__init__.py` & `sbpy-0.4.0/sbpy/calib/__init__.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/calib/core.py` & `sbpy-0.4.0/sbpy/calib/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,30 +12,29 @@
     'UndefinedSourceError'
 ]
 
 __doctest_requires__ = {
     'SpectralStandard': ['synphot'],
     'solar_spectrum': ['synphot'],
     'vega_spectrum': ['synphot'],
-    'Sun': ['synphot'],
-    'Vega': ['synphot'],
+    'Sun': ['synphot', 'astropy>=5.3'],
+    'Vega': ['synphot', 'astropy>=5.3'],
 }
 
 import os
 from abc import ABC
 from warnings import warn
 from functools import wraps
 import inspect
 import json
 
 import numpy as np
 from astropy.utils.state import ScienceState
 from astropy.utils.data import get_pkg_data_filename
-from astropy.table import Table, QTable
-from astropy.io import ascii
+from astropy.table import Table
 import astropy.units as u
 
 from ..spectroscopy.sources import SpectralSource, SynphotRequired
 from ..exceptions import SbpyException, OptionalPackageUnavailable
 from .. import bib
 from . import solar_sources, vega_sources
 
@@ -631,15 +630,15 @@
     >>> wave = np.logspace(-1, 2, 300) * u.um
     >>> fluxd = B(wave) * np.pi * u.sr
     >>> sun = Sun.from_array(wave, fluxd, description='5770 K blackbody Sun')
 
     Interpolate to / evaluate at 0.62 μm:
 
     >>> print(sun(0.62 * u.um))                # doctest: +FLOAT_CMP
-    1611.7080046473307 W / (m2 um)
+    1611.7080046473307 W / (um m2)
 
     Observe as through a spectrometer:
 
     >>> import numpy as np
     >>> import astropy.units as u
     >>> sun = Sun.from_default()
     >>> wave = np.linspace(1, 2.5) * u.um
@@ -647,15 +646,15 @@
 
     Observe as through a filter, integrating with the bandpass transmission:
 
     >>> from sbpy.photometry import bandpass
     >>> sun = Sun.from_default()
     >>> v = bandpass('Johnson V')
     >>> print(sun.observe(v))                  # doctest: +FLOAT_CMP
-    1839.93273227  W / (m2 um)
+    1839.93273227  W / (um m2)
 
     Observe through a filter, using `sbpy`'s filter calibration system:
 
     >>> from sbpy.calib import solar_fluxd
     >>> import sbpy.units as sbu
     >>> solar_fluxd.set({
     ...     'V': -26.76 * sbu.VEGAmag,
@@ -709,15 +708,15 @@
     >>> vega = Vega.from_default()               # doctest: +IGNORE_OUTPUT
 
     Create Vega from a file:
     >>> vega = Vega.from_file('filename')        # doctest: +SKIP
 
     Evaluate Vega at 1 μm (interpolation):
     >>> print(vega(1 * u.um))                    # doctest: +FLOAT_CMP
-    6.326492514857613e-09 W / (m2 um)
+    6.326492514857613e-09 W / (um m2)
 
     Observe Vega through as if through a spectrometer:
     >>> import numpy as np
     >>> wave = np.linspace(0.4, 0.6) * u.um
     >>> spec = vega.observe(wave)
 
     Observe Vega through a filter:
```

### Comparing `sbpy-0.3.0/sbpy/calib/data/alpha_lyr_stis_008-edit.fits` & `sbpy-0.4.0/sbpy/calib/data/alpha_lyr_stis_008-edit.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/calib/data/e490-00a_2014_hires.csv` & `sbpy-0.4.0/sbpy/calib/data/e490-00a_2014_hires.csv`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/calib/data/e490-00a_2014_lores.csv` & `sbpy-0.4.0/sbpy/calib/data/e490-00a_2014_lores.csv`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/calib/data/e490-00a_2014_table3.txt` & `sbpy-0.4.0/sbpy/calib/data/e490-00a_2014_table3.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/calib/data/e490-00a_2014_table4.txt` & `sbpy-0.4.0/sbpy/calib/data/e490-00a_2014_table4.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/calib/data/solar-photometry-willmer2018.json` & `sbpy-0.4.0/sbpy/calib/data/solar-photometry-willmer2018.json`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/calib/data/vega-photometry-willmer2018.json` & `sbpy-0.4.0/sbpy/calib/data/vega-photometry-willmer2018.json`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/calib/solar_sources.py` & `sbpy-0.4.0/sbpy/calib/solar_sources.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,30 +28,41 @@
         'bibcode': 'doi:10.1520/E0490'
     }
 
     E490_2014LR = {
         'filename': 'e490-00a_2014_hires.csv',
         'wave_unit': 'um',
         'flux_unit': 'W/(m2 um)',
-        'description': 'E490-00a (2014) low resolution reference solar spectrum (Table 4)',
+        'description': ('E490-00a (2014) low resolution reference solar '
+                        'spectrum (Table 4)'),
         'bibcode': 'doi:10.1520/E0490'
     }
 
     Kurucz1993 = {
-        'filename': 'ftp://ftp.stsci.edu/cdbs/grid/k93models/standards/sun_kurucz93.fits',
+        'filename': ('https://archive.stsci.edu/hlsps/reference-atlases/cdbs/'
+                     'grid/k93models/standards/sun_kurucz93.fits'),
         'description': 'Kurucz (1993) model, scaled by Colina et al. (1996)',
         'bibcode': '1993KurCD..13.....K'
     }
 
     Castelli1996 = {
-        'filename': 'ftp://ftp.stsci.edu/cdbs/grid/k93models/standards/sun_castelli.fits',
-        'description': 'Castelli model, scaled and presented by Colina et al. (1996)',
+        'filename': ('https://archive.stsci.edu/hlsps/reference-atlases/cdbs/'
+                     'grid/k93models/standards/sun_castelli.fits'),
+        'description': ('Castelli model, scaled and presented by Colina et '
+                        'al. (1996)'),
         'bibcode': '1996AJ....112..307C'
     }
 
+    calspec = {
+        "filename": ("https://archive.stsci.edu/hlsps/reference-atlases/cdbs/"
+                     "current_calspec/sun_mod_001.fits"),
+        "description": "R=5000, created by R. Bohlin from Kurucz Special Model",
+        "bibcode": "2014PASP..126..711B"
+    }
+
 
 class SolarPhotometry:
     """Built-in solar photometry.
 
     Format:
         {
             'filename': 'solar-photometry-willmer2018.json',
```

### Comparing `sbpy-0.3.0/sbpy/calib/tests/test_core.py` & `sbpy-0.4.0/sbpy/calib/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/calib/tests/test_sun.py` & `sbpy-0.4.0/sbpy/calib/tests/test_sun.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,196 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import inspect
 import pytest
 import numpy as np
 import astropy.units as u
-from astropy.tests.helper import remote_data
 from ...units import JMmag, VEGAmag
 from ...photometry import bandpass
 from .. import *
 
 try:
     import scipy
+
     HAS_SCIPY = True
 except ImportError:
     HAS_SCIPY = False
 
 
 class TestSun:
     def test___repr__(self):
-        with solar_spectrum.set('E490_2014LR'):
-            assert (repr(Sun.from_default()) ==
-                    ('<Sun: E490-00a (2014) low resolution reference '
-                     'solar spectrum (Table 4)>'))
+        with solar_spectrum.set("E490_2014LR"):
+            assert repr(Sun.from_default()) == (
+                "<Sun: E490-00a (2014) low resolution reference "
+                "solar spectrum (Table 4)>"
+            )
 
         sun = Sun.from_array([1, 2] * u.um, [1, 2] * u.Jy)
-        assert repr(sun) == '<Sun>'
+        assert repr(sun) == "<Sun>"
 
     def test_from_builtin(self):
-        sun = Sun.from_builtin('E490_2014LR')
-        assert sun.description == solar_sources.SolarSpectra.E490_2014LR['description']
+        sun = Sun.from_builtin("E490_2014LR")
+        assert (
+            sun.description
+            == solar_sources.SolarSpectra.E490_2014LR["description"]
+        )
 
     def test_from_builtin_unknown(self):
         with pytest.raises(UndefinedSourceError):
-            Sun.from_builtin('not a solar spectrum')
+            Sun.from_builtin("not a solar spectrum")
 
     def test_from_default(self):
-        with solar_spectrum.set('E490_2014LR'):
+        with solar_spectrum.set("E490_2014LR"):
             sun = Sun.from_default()
-            assert sun.description == solar_sources.SolarSpectra.E490_2014LR['description']
+            assert (
+                sun.description
+                == solar_sources.SolarSpectra.E490_2014LR["description"]
+            )
 
     def test_call_single_wavelength(self):
-        with solar_spectrum.set('E490_2014'):
+        with solar_spectrum.set("E490_2014"):
             sun = solar_spectrum.get()
             f = sun(0.5555 * u.um)
             assert np.isclose(f.value, 1897)
 
     def test_call_single_frequency(self):
-        with solar_spectrum.set('E490_2014'):
+        with solar_spectrum.set("E490_2014"):
             sun = solar_spectrum.get()
             f = sun(3e14 * u.Hz)
-            assert np.isclose(f.value, 2.49484251e+14)
+            assert np.isclose(f.value, 2.49484251e14)
 
-    @pytest.mark.skipif('not HAS_SCIPY')
+    @pytest.mark.skipif("not HAS_SCIPY")
     def test_sun_observe_wavelength_array(self):
         from scipy.integrate import trapz
 
-        unit = 'W/(m2 um)'
+        unit = "W/(m2 um)"
 
         # compare Sun's rebinning with an integration over the spectrum
-        sun = Sun.from_builtin('E490_2014')
+        sun = Sun.from_builtin("E490_2014")
 
-        wave0 = sun.wave.to('um').value
+        wave0 = sun.wave.to("um").value
         fluxd0 = sun.fluxd.to(unit).value
 
         wave = np.linspace(0.35, 0.55, 6)
 
         d = np.diff(wave)[0] / 2
         left_bins = wave - d
         right_bins = wave + d
 
         fluxd1 = np.zeros(len(wave))
         for i in range(len(wave)):
             j = (wave0 >= left_bins[i]) * (wave0 <= right_bins[i])
-            fluxd1[i] = (trapz(fluxd0[j] * wave0[j], wave0[j]) /
-                         trapz(wave0[j], wave0[j]))
+            fluxd1[i] = trapz(fluxd0[j] * wave0[j], wave0[j]) / trapz(
+                wave0[j], wave0[j]
+            )
 
         fluxd2 = sun.observe(wave * u.um, unit=unit).value
 
         assert np.allclose(fluxd1, fluxd2, rtol=0.005)
 
     def test_filt_units(self):
         """Colina et al. V=-26.75 mag, for zero-point flux density
-           36.7e-10 ergs/s/cm2/Å.
+        36.7e-10 ergs/s/cm2/Å.
         """
-        sun = Sun.from_builtin('E490_2014')
-        V = bandpass('johnson v')
-        weff, fluxd = sun.observe_bandpass(V, unit='erg/(s cm2 AA)')
+        sun = Sun.from_builtin("E490_2014")
+        V = bandpass("johnson v")
+        weff, fluxd = sun.observe_bandpass(V, unit="erg/(s cm2 AA)")
         assert np.isclose(weff.value, 5502, rtol=0.001)
         assert np.isclose(fluxd.value, 183.94, rtol=0.0003)
 
     def test_filt_vegamag(self):
         """Colina et al. V=-26.75 mag (Johnson-Morgan system)
 
         Not obvious we are using the same filter profile, but 0.006 mag
         agreement is good.
 
         """
-        sun = Sun.from_builtin('E490_2014')
-        V = bandpass('johnson v')
+        sun = Sun.from_builtin("E490_2014")
+        V = bandpass("johnson v")
         fluxd = sun.observe(V, unit=JMmag)
         assert np.isclose(fluxd.value, -26.75, atol=0.006)
 
     def test_filt_abmag(self):
         """Willmer 2018 V=-26.77.
 
         Willmer uses Haberreiter et al. 2017 solar spectrum in the
         optical.
 
         """
-        sun = Sun.from_builtin('E490_2014')
-        V = bandpass('johnson v')
+        sun = Sun.from_builtin("E490_2014")
+        V = bandpass("johnson v")
         fluxd = sun.observe(V, unit=u.ABmag)
         assert np.isclose(fluxd.value, -26.77, atol=0.007)
 
     def test_filt_stmag(self):
         """Willmer 2018, V=-26.76
 
         Willmer uses Haberreiter et al. 2017 solar spectrum in the
         optical.
 
         """
-        sun = Sun.from_builtin('E490_2014')
-        V = bandpass('johnson v')
+        sun = Sun.from_builtin("E490_2014")
+        V = bandpass("johnson v")
         fluxd = sun.observe(V, unit=u.STmag)
         assert np.isclose(fluxd.value, -26.76, atol=0.003)
 
     def test_filt_solar_fluxd(self):
-        with solar_fluxd.set({'V': -26.76 * VEGAmag}):
+        with solar_fluxd.set({"V": -26.76 * VEGAmag}):
             sun = Sun(None)
-            fluxd = sun.observe('V', unit=VEGAmag)
+            fluxd = sun.observe("V", unit=VEGAmag)
         assert np.isclose(fluxd.value, -26.76)
 
     def test_meta(self):
-        sun = Sun.from_builtin('E490_2014')
+        sun = Sun.from_builtin("E490_2014")
         assert sun.meta is None
 
-    @pytest.mark.skipif('True')
-    @remote_data
+    @pytest.mark.remote_data
     def test_kurucz_nan_error(self):
         """sbpy#113
 
         Using Haberreiter et al. 2017 solar spectrum: -26.77.
 
         NaNs in Kurucz file should not affect this calculation.
 
         """
-        sun = Sun.from_builtin('Kurucz1993')
-        V = bandpass('johnson v')
+        sun = Sun.from_builtin("Kurucz1993")
+        V = bandpass("johnson v")
         fluxd = sun.observe(V, unit=u.ABmag)
         assert np.isclose(fluxd.value, -26.77, atol=0.005)
 
+    @pytest.mark.remote_data
+    def test_castelli96(self):
+        """Verify Castelli1996 calibration.
+
+        According to the FITS header:
+
+        HISTORY   Created Thu 15:49:31 16-Nov-95
+        COMMENT   solar model spectrum calculated by F. Castelli.
+        COMMENT   Absolute flux normalized to a V flux of 184.2 ergs/s/cm^2/A
+        COMMENT   For more details see Colina, Bohlin & Castelli 1996
+                  CAL/SCS-008
+
+        2022-06-05: sbpy calculates 184.5 ergs/s/cm^2/A; agreement within 0.2%
+        """
+
+        sun = Sun.from_builtin("Castelli1996")
+        V = bandpass("johnson v")
+        fluxd = sun.observe(V, unit="erg/(s cm2 AA)")
+        assert np.isclose(fluxd.value, 184.2, rtol=0.002)
+
+    @pytest.mark.remote_data
+    def test_calspec(self):
+        """Verify CALSPEC solar model calibration."""
+
+        sun = Sun.from_builtin("calspec")
+        V = bandpass("johnson v")
+        fluxd = sun.observe(V, unit=VEGAmag)
+        assert np.isclose(fluxd.value, -26.75, rtol=0.002)
+
     def test_show_builtin(self, capsys):
         Sun.show_builtin()
         captured = capsys.readouterr()
         sources = inspect.getmembers(
-            Sun._sources, lambda v: isinstance(v, dict))
+            Sun._sources, lambda v: isinstance(v, dict)
+        )
         for k, v in sources:
             assert k in captured.out
```

### Comparing `sbpy-0.3.0/sbpy/calib/tests/test_vega.py` & `sbpy-0.4.0/sbpy/calib/tests/test_vega.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 import inspect
 import pytest
 import numpy as np
 import astropy.units as u
-from astropy.tests.helper import remote_data
 from ... import units as sbu
 from ...photometry import bandpass
 from .. import core
 from .. import *
 
 try:
     import scipy
```

### Comparing `sbpy-0.3.0/sbpy/calib/vega_sources.py` & `sbpy-0.4.0/sbpy/calib/vega_sources.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/conftest.py` & `sbpy-0.4.0/sbpy/conftest.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/data/__init__.py` & `sbpy-0.4.0/sbpy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/data/core.py` & `sbpy-0.4.0/sbpy/data/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 =====================
 sbpy.data core module
 =====================
 
 created on June 22, 2017
 """
 
+from collections.abc import Mapping
 from copy import deepcopy
 from numpy import ndarray, array, hstack, iterable
-from astropy.table import QTable, Column
+from astropy.table import QTable, Table, Column, Row, vstack
 from astropy.time import Time
 from astropy.coordinates import Angle
 import astropy.units as u
 
 from . import Conf
 from ..exceptions import SbpyException, SbpyWarning
 
@@ -639,45 +640,61 @@
             self = self._convert_columns(ident)
             ident = self._translate_columns(ident)[0]
             return self.table[ident]
 
         # return as new instance of this class for all other identifiers
         return self.from_table(self.table[ident])
 
-    def __setitem__(self, *args):
+    def __setitem__(self, ident, val):
         """Refer cls.__setitem__ to self._table"""
-        self.table.__setitem__(*args)
+        # `astropy.table.Table.__setitem__` only allows to set a single
+        # column.  Only this case is checked here for alternative column
+        # name.  All other cases are directly passed to `table.__setitem__`.
+        if isinstance(ident, str) and ident in self:
+            ident = self._translate_columns(ident)[0]
+        self.table.__setitem__(ident, val)
+
+    def __contains__(self, value):
+        """To support `in` operator that allows for alternative names"""
+        if (value in self.table.colnames) or \
+            (value in sum([Conf.fieldnames[Conf.fieldname_idx.get(x, slice(0))]
+                           for x in self.table.colnames], [])):
+            return True
+        else:
+            return False
 
-    def _translate_columns(self, target_colnames):
+    def _translate_columns(self, target_colnames, ignore_missing=False):
         """Translate target_colnames to the corresponding column names
         present in this object's table. Returns a list of actual column
         names present in this object that corresponds to target_colnames
-        (order is preserved). Raises KeyError if not all columns are
-        present or one or more columns could not be translated.
+        (order is preserved). If `ignore_missing == False` (default),
+        raises a `KeyError` if a match cannot be found for an input column
+        name (neither in this object nor defined in `Conf.fieldnames`).
+        If `ignore_missing == True`, then the problemtic column name will
+        be silently carried over and returned.
         """
 
         if not isinstance(target_colnames, (list, ndarray, tuple)):
             target_colnames = [target_colnames]
 
         translated_colnames = deepcopy(target_colnames)
         for idx, colname in enumerate(target_colnames):
-            # colname is already a column name in self.table
-            if colname in self.field_names:
-                continue
-            # colname is an alternative column name
-            elif colname in sum(Conf.fieldnames, []):
-                for alt in Conf.fieldnames[Conf.fieldname_idx[colname]]:
-                    # translation available for colname
+            if colname not in self.field_names:
+                # colname not already in self.table
+                for alt in Conf.fieldnames[
+                            Conf.fieldname_idx.get(colname, slice(0))]:
+                    # defined in `Conf.fieldnames`
                     if alt in self.field_names:
                         translated_colnames[idx] = alt
                         break
-            # colname is unknown, raise a KeyError
-            else:
-                raise KeyError('field {:s} not available.'.format(
-                    colname))
+                else:
+                    # undefined colname
+                    if not ignore_missing:
+                        raise KeyError('field "{:s}" not available.'.format(
+                            colname))
 
         return translated_colnames
 
     def _convert_columns(self, target_colnames):
         """Convert target_colnames, if necessary. Converted columns will be
         added as columns to ``self`` using the field names provided in
         target_colnames. No error is returned by this function if a
@@ -917,7 +934,120 @@
                 # allow plain columns for dimensionless units
                 if not valid and not (
                     self[test_field].unit is None
                     and dim.unit == u.dimensionless_unscaled
                 ):
                     raise FieldError('Field {} does not have units of {}'
                                      .format(test_field, str(dim.unit)))
+
+    def add_row(self, vals, names=None, units=None):
+        """Add a new row to the end of DataClass.
+
+        This is similar to `astropy.table.Table.add_row`, but allows for
+        a set of different columns in the new row from the original DataClass
+        object.  It also allows for aliases of column names.
+
+        Parameters
+        ----------
+        vals : `~astropy.table.Row`, tuple, list, dict
+            Row to be added
+        names : iterable of strings, optional
+            The names of columns if not implicitly specified in ``vals``.
+            Takes precedence over the column names in ``vals`` if any.
+        units : str or list-like, optional
+            Unit labels (as provided by `~astropy.units.Unit`) in which
+            the data provided in ``rows`` will be stored in the underlying
+            table. If None, the units as provided by ``rows``
+            are used. If the units provided in ``units`` differ from those
+            used in ``rows``, ``rows`` will be transformed to the units
+            provided in ``units``. Must have the same length as ``names``
+            and the individual data rows in ``rows``. Default: None
+
+        Notes
+        -----
+        If a time is included in ``vals``, it can either be an explicit
+        `~astropy.time.Time` object, or a number, `~astropy.units.Quantity`
+        object, or string that can be inferred to be a time by the existing
+        column of the same name or by its position in the sequence.  In
+        this case, the type of time values must be valid to initialize
+        an `~astropy.time.Time` object with format='jd' or 'isot', and
+        the scale of time is default to the scale of the corresponding
+        existing column of time.
+
+        Examples
+        --------
+        >>> import astropy.units as u
+        >>> from sbpy.data import DataClass
+        >>>
+        >>> data = DataClass.from_dict(
+        ...         {'rh': [1, 2, 3] * u.au, 'delta': [1, 2, 3] * u.au})
+        >>> row = {'rh': 4 * u.au, 'delta': 4 * u.au, 'phase': 15 * u.deg}
+        >>> data.add_row(row)
+        """
+        if isinstance(vals, Row):
+            vals = DataClass.from_table(vals)
+        else:
+            if isinstance(vals, Mapping):
+                keys_list = list(vals.keys())
+                vals_list = [vals[k] for k in keys_list]
+                vals = vals_list
+                if names is None:
+                    names = keys_list
+            else:
+                # assume it's an iterable that can be taken as columns
+                if names is None:
+                    # if names of columns are not specified, default to the
+                    # existing names and orders
+                    names = self.field_names
+            # check if any astropy Time columns
+            for i, k in enumerate(names):
+                if k in self and isinstance(self[k], Time):
+                    vals[i] = Time(vals[i], scale=self[k].scale,
+                                   format='isot' if isinstance(vals[i], str)
+                                   else 'jd')
+            vals = DataClass.from_rows(vals, names, units=units)
+        self.vstack(vals)
+
+    def vstack(self, data, **kwargs):
+        """Stack another DataClass object to the end of DataClass
+
+        Similar to `~astropy.table.Table.vstack`, the DataClass object
+        to be stacked doesn't have to have the same set of columns as
+        the existing object.  The `join_type` keyword parameter will be
+        used to decide how to process the different sets of columns.
+
+        Joining will be in-place.
+
+        Parameters
+        ----------
+        data : `~sbpy.data.DataClass`, dict, `~astropy.table.Table`
+            Object to be joined with the current object
+        kwargs : dict
+            Keyword parameters accepted by `~astropy.table.Table.vstack`.
+
+        Examples
+        --------
+        >>> import astropy.units as u
+        >>> from sbpy.data import DataClass
+        >>>
+        >>> data1 = DataClass.from_dict(
+        ...         {'rh': [1, 2, 3] * u.au, 'delta': [1, 2, 3] * u.au})
+        >>> data2 = DataClass.from_dict(
+        ...         {'rh': [4, 5] * u.au, 'phase': [15, 15] * u.deg})
+        >>> data1.vstack(data2)
+        """
+        # check and process input data
+        if isinstance(data, dict):
+            data = DataClass.from_dict(data)
+        elif isinstance(data, Table):
+            data = DataClass.from_table(data)
+        if not isinstance(data, DataClass):
+            raise ValueError('DataClass, dict, or astorpy.table.Table are '
+                             'expected, but {} is received.'.
+                             format(type(data)))
+
+        # adjust input column names for alises
+        alt = self._translate_columns(data.field_names, ignore_missing=True)
+        data.table.rename_columns(data.field_names, alt)
+
+        # join with the input table
+        self.table = vstack([self.table, data.table], **kwargs)
```

### Comparing `sbpy-0.3.0/sbpy/data/decorators.py` & `sbpy-0.4.0/sbpy/data/decorators.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/data/dimensions.py` & `sbpy-0.4.0/sbpy/data/dimensions.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/data/ephem.py` & `sbpy-0.4.0/sbpy/data/ephem.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,16 @@
             of queried parameters.
 
         Examples
         --------
         >>> from sbpy.data import Ephem
         >>> from astropy.time import Time
         >>> epoch = Time('2018-05-14', scale='utc')
-        >>> eph = Ephem.from_horizons('ceres', epochs=epoch) # doctest: +SKIP
+        >>> eph = Ephem.from_horizons('ceres', epochs=epoch)
+        ...         # doctest: +REMOTE_DATA
 
         """
 
         # modify epoch input to make it work with astroquery.jplhorizons
         # maybe this stuff should really go into that module....
         _epochs = None  # avoid modifying epochs in-place
         _sorted = False
@@ -531,15 +532,16 @@
             of queried parameters.
 
         Examples
         --------
         >>> from sbpy.data import Ephem
         >>> from astropy.time import Time
         >>> epoch = Time('2018-05-14', scale='utc')
-        >>> eph = Ephem.from_horizons('ceres', epochs=epoch) # doctest: +SKIP
+        >>> eph = Ephem.from_horizons('ceres', epochs=epoch)
+        ...         # doctest: +REMOTE_DATA
         """
 
         _epochs = None  # avoid modifying epochs in-place
 
         # format _epoch for astroquery.imcce.Miriade
         if epochs is None:
             _epochs = {'start': Time.now().utc.jd}
@@ -732,15 +734,15 @@
            1 Ceres  2458529.066966272 ...  1.2522500440509399e-05 70.30569661787204
            1 Ceres 2458529.1086329385 ...  1.4101698473351076e-05 70.31515536712485
            1 Ceres 2458529.1502996054 ...  1.4771304981564537e-05  70.3246138990413
            1 Ceres  2458529.191966272 ...   1.448582020449618e-05 70.33407221340468
            1 Ceres 2458529.2336329385 ...   1.326517587380005e-05 70.34353031031534
            1 Ceres 2458529.2752996054 ...  1.1193369555934085e-05 70.35298818987367        """
 
-        if not pyoorb:
+        if pyoorb is None:
             raise RequiredPackageUnavailable('pyoorb')
 
         # create a copy of orbit
         orb = Orbit.from_table(orbit.table)
 
         if epochs is None:
             epochs = Time.now()
```

### Comparing `sbpy-0.3.0/sbpy/data/fieldnames.rst` & `sbpy-0.4.0/sbpy/data/fieldnames.rst`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/data/names.py` & `sbpy-0.4.0/sbpy/data/names.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 Class for dealing with object naming conventions.
 
 created on August 28, 2017
 
 """
 
+import re
 from ..exceptions import SbpyException
 
 __all__ = ['Names', 'TargetNameParseError', 'natural_sort_key']
 
 
 def natural_sort_key(s):
     """List sort keys considering strings of numbers as integers.
@@ -43,15 +44,14 @@
     ...           '2P/Encke']
     >>> sorted(comets)
     ['101P/Chernykh', '10P/Tempel 2', '2P/Encke', '9P/Tempel 1']
     >>> sorted(comets, key=natural_sort_key)
     ['2P/Encke', '9P/Tempel 1', '10P/Tempel 2', '101P/Chernykh']
 
     """
-    import re
     keys = tuple()
     for k in re.split('([0-9]+)', str(s)):
         keys += (int(k) if k.isdigit() else k,)
     return keys
 
 
 class TargetNameParseError(SbpyException):
@@ -303,28 +303,28 @@
         |C/2013 US10                   |      | C  |        | 2013 US10|                        |
         +------------------------------+------+----+--------+----------+------------------------+
         |C/2015 V2 (Johnson)           |      | C  |        | 2015 V2  |Johnson                 |
         +------------------------------+------+----+--------+----------+------------------------+
 
         """
 
-        import re
-
         # define comet matching pattern
         pat = ('^(([1-9][0-9]*[PDCX]'
                '(-[A-Z]{1,2})?)|[PDCX]/)'  # type/number/fragm [0,1,2]
                '|([-]?[0-9]{3,4}[ _][A-Z]{1,2}[0-9]{0,3}(-[1-9A-Z]{0,2})?)'
                # designation [3,4]
-               '|((([dvA-Z][a-z\']? ?[A-Za-z\-]*)[ -]?[A-Z]?[1-9]*[a-z]*)'
+               r'|((([dvA-Z][a-z\']? ?[A-Za-z\-]*)[ -]?[A-Z]?[1-9]*[a-z]*)'
                '( [1-9A-Z]{1,2})*)'  # name [5,6]
                )
 
         # regex patterns that will be rejected
-        rej_pat = ('(([1-9][0-9]*[pdcxai]\b)'  # small-caps comet number
-                   '|([pdcxai]/))'  # small-caps comet type
+        rej_pat = ('^(([1-9][0-9]*[pdcxiaCXIA]\b)'
+                   # numbered with lower case, X, C, I, or A
+                   '|([pdcxaiAI]/))'
+                   # temporary designation with lower case, I, or A
                    )
 
         raw = s.translate(str.maketrans('()', '  ')).strip()
 
         # reject rej_pat patterns
         rej = re.findall(rej_pat, raw)
 
@@ -338,15 +338,15 @@
 
         if len(m) > 0:
             for el in m:
                 # type & number & fragment
                 if len(el[0]) > 0:
                     typnumber = el[0].replace('/', '')
                     try:
-                        r['type'] = re.findall('[PDCXAI]', typnumber)[0]
+                        r['type'] = re.findall('[PDCX]', typnumber)[0]
                     except IndexError:
                         pass
                     try:
                         r['number'] = int(re.findall('[0-9]*', typnumber)[0])
                     except (IndexError, ValueError):
                         pass
                     try:
@@ -445,18 +445,19 @@
         +----------------------------------+----------+------+-----------------+
         |K07Tf8A                           |2007 TA418|      |                 |
         +----------------------------------+----------+------+-----------------+
         |G3693                             |          |163693|                 |
         +----------------------------------+----------+------+-----------------+
         |1A                                |1A        |      |                 |
         +----------------------------------+----------+------+-----------------+
+        |A/2018 V3                         |2018 V3   |      |                 |
+        +----------------------------------+----------+------+-----------------+
 
-        """
 
-        import re
+        """
 
         pat = ('(([1A][8-9][0-9]{2}[ _][A-Z]{2}[0-9]{0,3}|'
                '20[0-9]{2}[ _][A-Z]{2}[0-9]{0,3})'
                # designation [0,1]
                '|([1-9][0-9]{3}[ _](P-L|T-[1-3])))'
                # Palomar-Leiden  [0,2,3]
                '|([IJKL][0-9]{2}[A-Z][0-9a-z][0-9][A-Z]'
@@ -471,22 +472,24 @@
                "|['`]?[A-Z][A-Z]*['`]?[a-z][a-z]*['`]?[^0-9]*"
                "[ -]?[A-Z]?[a-z]*[^0-9]*)"
                # name [6]
                '|((^|\b)[1-9][0-9]*(\b|$| |_))'
                # number [7,8]
                '|^(([1-9][0-9]*A))'
                # comet-style designations: 1A [10]
+               '|^A/([12][0-9][0-9][0-9] [A-Z][0-9]+)'
+               # asteroids with cometary orbits [12]
                )
 
         # regex patterns that will be rejected
-        rej_pat = ('([1-2][0-9]{0,3}[ _][A-Z][0-9]*(\b|$))'
-                   # comet desig
-                   '|([1-9][0-9]*[PDCXAI]\b)'
-                   # comet number
-                   '|([PDCXAI]/)'
+        rej_pat = ('([CPXDI]/[1-2][0-9]{0,3}[ _][A-Z][0-9]*(\b|$))'
+                   # comet or interstellar desig
+                   '|([1-9][0-9]*[PDCXI]\b)'
+                   # comet or interstellar number
+                   '|([PDCXI]/)'
                    # comet type
                    '|([1-2][0-9]{0,3}[ _][a-z]{2}[0-9]{0,3})'
                    )
 
         raw = s.translate(str.maketrans('()_', '   ')).strip()
 
         # reject rej_pat patterns
@@ -523,14 +526,16 @@
                 # name
                 elif len(el[6]) > 0:
                     if len(el[6].strip()) > 1:
                         r['name'] = el[6].strip()
                 # comet-style designation
                 elif len(el[10]) > 0:
                     r['desig'] = el[10].strip()
+                elif len(el[12]) > 0:
+                    r['desig'] = el[12].strip()
 
         if len(r) == 0:
             raise TargetNameParseError(('{} does not appear to be an '
                                         'asteroid name'.format(s)))
         else:
             return r
```

### Comparing `sbpy-0.3.0/sbpy/data/obs.py` & `sbpy-0.4.0/sbpy/data/obs.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         queried from the selected service.
 
         Parameters
         ----------
         service : str, optional
             Service from which to acquire data: ``'jplhorizons'``,
             ``'mpc'``, or ``'miriade'``, corresponding to the
-            `JPL Horizons system <https://ssd.jpl.nasa.gov/horizons.cgi>`_
+            `JPL Horizons system <https://ssd.jpl.nasa.gov/horizons/>`_
             (using `~sbpy.data.Ephem.from_horizons`),
             the `Minor Planet Center ephemeris service
             <https://minorplanetcenter.net/iau/MPEph/MPEph.html>`_
             (using `~sbpy.data.Ephem.from_mpc`), and
             the `IMCCE Miriade service
             <http://vo.imcce.fr/webservices/miriade/>`_
             (using `~sbpy.data.from_miriade`). Default:
```

### Comparing `sbpy-0.3.0/sbpy/data/orbit.py` & `sbpy-0.4.0/sbpy/data/orbit.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 ======================
 
 Class for querying, manipulating, integrating, and fitting orbital elements.
 
 created on June 04, 2017
 """
 import os
+import itertools
 import numpy as np
 from numpy import array, ndarray, double, arange
 from astropy.time import Time
 from astropy.table import vstack, QTable
 from astroquery.jplhorizons import Horizons
 from astroquery.mpc import MPC
 import astropy.units as u
 from warnings import warn
 
 try:
     import pyoorb
 except ImportError:
     pyoorb = None
 
-from ..bib import cite
+from ..bib import cite, register
 from ..exceptions import RequiredPackageUnavailable, SbpyException
 from . import Conf, DataClass, QueryError, TimeScaleWarning
 
 try:
     import pyoorb
 except ImportError:
     pyoorb = None
@@ -52,15 +53,15 @@
     @classmethod
     @cite({'data source': '1996DPS....28.2504G'})
     @cite({'software: astroquery': '2019AJ....157...98G'})
     def from_horizons(cls, targetids, id_type='smallbody',
                       epochs=None, center='500@10',
                       **kwargs):
         """Load target orbital elements from
-        `JPL Horizons <https://ssd.jpl.nasa.gov/horizons.cgi>`_ using
+        `JPL Horizons <https://ssd.jpl.nasa.gov/horizons/>`_ using
         `astroquery.jplhorizons.HorizonsClass.elements`
 
         Parameters
         ----------
         targetids : str or iterable of str
             Target identifier, i.e., a number, name, designation, or JPL
             Horizons record number, for one or more targets.
@@ -97,15 +98,15 @@
             Arguments that will be provided to
             `astroquery.jplhorizons.HorizonsClass.elements`.
 
         Notes
         -----
         * For detailed explanations of the queried fields, refer to
           `astroquery.jplhorizons.HorizonsClass.elements` and the
-          `JPL Horizons documentation <https://ssd.jpl.nasa.gov/?horizons_doc>`_.
+          `JPL Horizons documentation <https://ssd.jpl.nasa.gov/horizons/manual.html>`_.
         * By default, elements are provided in the J2000.0 reference
           system and relative to the ecliptic and mean equinox of the
           reference epoch. Different settings can be chosen using
           additional keyword arguments as used by
           `astroquery.jplhorizons.HorizonsClass.elements`.
 
         Returns
@@ -697,30 +698,200 @@
 
         for colname in self.field_names:
             if (colname in default_units.keys() and
                 not isinstance(self[colname],
                                (u.Quantity, u.CompositeUnit))):
                 self[colname].unit = default_units[colname]
 
-        ooepoch = [epochs.tt.mjd, Conf.oorb_timeScales['TT']]
+        # epochs may be a scalar value, but we need an interable
+        mjd = epochs.tt.mjd.reshape(epochs.size)
+        ooepoch = np.array(
+            list(itertools.zip_longest(mjd, [3])), dtype=np.double, order="F"
+        )
 
         # convert epochs to TT and MJD
         in_orbits = Orbit.from_table(self.table)
         in_orbits['epoch'] = in_orbits['epoch'].tt
 
         oo_orbits, err = pyoorb.pyoorb.oorb_propagation(
             in_orbits=in_orbits._to_oo(),
             in_epoch=ooepoch,
             in_dynmodel=dynmodel)
+        print(oo_orbits, err)
 
         if err != 0:
             OpenOrbError('pyoorb failed with error code {:d}'.format(err))
 
         orbits = Orbit._from_oo_propagatation(oo_orbits, orbittype, timescale)
 
         # replace id column with actual target names from original orbits
         orbits.table.replace_column('id', self.table['targetname'])
 
         orbits.meta['orbit_type'] = orbittype
         orbits.table.remove_column('epoch_scale'),
 
         return orbits
+
+    @cite({'method': '1997Icar..127...13L'})
+    def tisserand(self, planet='599', epoch=None):
+        """Tisserand parameter with respect to a planet
+
+
+        Parameters
+        ----------
+        planet : str, `~Orbit` object, or sequence of str, optional
+            Planet(s) against which the Tisserand parameter is calculated.
+            If `str`, then the orbital elements of the planet will be
+            automaticallyl pulled from JPL Horizons. If `self` and/or
+            `planet` contains more than one object, then `numpy` broadcasting
+            rules apply.  Default is Jupiter.
+        epoch : `~astropy.time.Time`, optional
+            The epoch of planet orbit if pulled from JPL Horizons.  This
+            parameter will be passed to `~sbpy.data.Orbit.from_horizons`.
+            If the planet orbit is passed directly, then this parameter
+            has no effect.
+
+        Returns
+        -------
+        u.Quantity
+            The Tisserand parameter(s)
+
+
+        References
+        ----------
+        Levison, H. F., Duncan, M. J. 1997, Icarus 127, 13
+
+
+        Examples
+        --------
+        >>> from sbpy.data import Orbit
+        >>> comets = Orbit.from_horizons(['252P', 'P/2016 BA14'],
+        ...     id_type='designation', closest_apparition=True)
+        ...     # doctest: +REMOTE_DATA
+        >>> T_J = comets.tisserand() # doctest: +REMOTE_DATA
+        >>>
+        >>> halley = Orbit.from_horizons('1P', id_type='designation',
+        ...     closest_apparition=True) # doctest: +REMOTE_DATA
+        >>> T = halley.tisserand(['599', '699', '799', '899']) # doctest: +REMOTE_DATA
+        """
+
+        if isinstance(planet, str) \
+            or (hasattr(planet, '__iter__')
+                and np.all([isinstance(x, str) for x in planet])):
+            planet = Orbit.from_horizons(planet, id_type=None, epochs=epoch)
+
+        a_p = planet['a']
+        t = a_p / self['a'] + 2 * np.cos(self['i']) * \
+            np.sqrt((1 - self['e']**2) * self['a'] / a_p)
+        t = u.Quantity(t)
+        if len(t) == 1:
+            t = t[0]
+        return t
+
+    def D_criterion(self, obj, version='sh'):
+        """Evaluate orbit similarity D-criterion
+
+        Three different versions of D-criterion are defined and often compared
+        to each other, includingthe Southworth-Hawkins function [SH63]_,
+        Drummond function [D81]_, and the hybrid version [J93]_.  See review by
+        [W19]_.
+
+        Parameters
+        ----------
+        obj : `~Orbit` object
+            Object(s) against which to calculate D-criterion
+        version : ['sh', 'd', 'h'], optional
+            Select the versions of D-criterion formula.  Case insensitive.
+            'sh' : Southworth-Hawkins function
+            'd' : Drummond function
+            'h' : Hybrid function
+            See references for the details of each version.
+
+
+        Returns
+        -------
+        float or numpy.ndarray
+
+
+        References
+        ----------
+        .. [SH63] `Southwarth, R. B., & Hawkins, G. S. 1963, SCoA, 7, 261
+           <https://ui.adsabs.harvard.edu/abs/1963SCoA....7..261S/abstract>`_
+
+        .. [D81] `Drummond, J. D. 1981, Icarus 45, 545
+           <https://ui.adsabs.harvard.edu/abs/1981Icar...45..545D/abstract>`_
+
+        .. [J93] `Jopek, T. J. 1993, Icarus 106, 603
+           <https://ui.adsabs.harvard.edu/abs/1993Icar..106..603J/abstract>`_
+
+        .. [W19] `Williams, I. P., Jopek, T. J., Rudawska, R., Tóth, J.,
+           Kornoš, L. 2019, In: Ryabova, G. O., Asher, D. J., Compbell-Brown
+           M. D., eds.), Cambridge, UK: Cambridge University Press, 210-234.
+           <https://ui.adsabs.harvard.edu/abs/2019msme.book..210W/abstract>`_
+
+
+        Examples
+        --------
+        >>> from sbpy.data import Orbit
+        >>> comets = Orbit.from_horizons(['252P', 'P/2016 BA14'],
+        ...     id_type='designation', closest_apparition=True)
+        ...     # doctest: +REMOTE_DATA
+        >>> # Southworth & Hawkins function
+        >>> D_SH = comets[0].D_criterion(comets[1]) # doctest: +REMOTE_DATA
+        >>> # Drummond function
+        >>> D_D = comets[0].D_criterion(comets[1], version='d') # doctest: +REMOTE_DATA
+        >>> # hybrid function
+        >>> D_H = comets[0].D_criterion(comets[1], version='h') # doctest: +REMOTE_DATA
+        """
+
+        if version.lower() not in ['sh', 'd', 'h']:
+            raise ValueError("version should be one of ['sh', 'd', 'h'] (case "
+                             "insensitive, {} received".format(version))
+
+        diff_e = obj['e'] - self['e']
+        sum_e = obj['e'] + self['e']
+        diff_q = obj['q'].to_value(u.au) - self['q'].to_value(u.au)
+        sum_q = obj['q'].to_value(u.au) + self['q'].to_value(u.au)
+        diff_i = obj['i'] - self['i']
+        sum_i = obj['i'] + self['i']
+        diff_omega = obj['Omega'] - self['Omega']
+        diff_w = obj['w'] - self['w']
+
+        # sin(I_AB / 2)**2
+        sin_i2 = np.sin(diff_i / 2)**2 \
+            + np.sin(self['i']) * np.sin(obj['i']) * np.sin(diff_omega / 2)**2
+
+        if version.lower() == 'd':
+            # Drummond function
+            register(self.D_criterion, {'method': '1981Icar...45..545D'})
+            i_ba = np.arcsin(np.sqrt(sin_i2)) * 2
+            beta = [np.arcsin(np.sin(o['i']) * np.sin(o['w']))
+                    for o in [obj, self]]
+            lamb = [o['Omega'] + np.arctan(np.cos(o['i']) * np.tan(o['w']))
+                    + (np.cos(o['w']) < 0).astype(int) * np.pi * u.rad
+                    for o in [obj, self]]
+            theta_ba = np.arccos(np.sin(beta[0]) * np.sin(beta[1])
+                                 + np.cos(beta[0]) * np.cos(beta[1])
+                                 * np.cos(lamb[1] - lamb[0]))
+            d2 = (diff_e / sum_e)**2 + (diff_q / sum_q)**2 \
+                + (i_ba / (np.pi * u.rad))**2 \
+                + (sum_e * theta_ba / (2 * np.pi * u.rad))**2
+        else:
+            cos_i2 = np.sqrt(1 - sin_i2)
+            sign = (abs(diff_omega) <= 180 * u.deg).astype(int) * 2 - 1
+            pi_ba = diff_w + 2 * sign * np.arcsin(
+                np.cos(sum_i / 2) * np.sin(diff_omega / 2) / cos_i2)
+
+            if version.lower() == 'sh':
+                # Southworth-Hawkins function
+                register(self.D_criterion, {'method': '1963SCoA....7..261S'})
+                d2 = diff_e**2 + diff_q**2 + 4 * sin_i2 \
+                    + (sum_e * np.sin(pi_ba / 2))**2
+            else:
+                # hybrid function
+                register(self.D_criterion, {'method': '1993Icar..106..603J'})
+                d2 = diff_e**2 + (diff_q / sum_q)**2 + 4 * sin_i2 \
+                    + (sum_e * np.sin(pi_ba / 2))**2
+        d = np.sqrt(u.Quantity(d2))
+        if len(d) == 1:
+            d = d[0]
+        return d
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sbpy-0.3.0/sbpy/data/phys.py` & `sbpy-0.4.0/sbpy/data/phys.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,16 @@
 
                 # identify units
                 if isinstance(val, u.Quantity):
                     columnunits[key].add(val.unit)
                 elif isinstance(val, u.CompositeUnit):
                     for unit in val.bases:
                         columnunits[key].add(unit)
-                elif key == 'H':
-                    # fix for astroquery <0.4.2
+                elif key in ['H', 'M1', 'M2', 'M1_sig', 'M2_sig']:
+                    # fix for lack of units from SBDB via astroquery
                     columnunits[key].add(u.mag)
 
             alldata.append(data)
 
         # re-assemble data on a per-column basis
         coldata = []
         for col in columnnames:
```

### Comparing `sbpy-0.3.0/sbpy/data/tests/test_dataclass.py` & `sbpy-0.4.0/sbpy/data/tests/test_dataclass.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from collections import OrderedDict
 from sbpy.data import dimensions
 import pytest
 from copy import deepcopy
 import astropy.units as u
 from astropy.coordinates import Angle
-from astropy.table import QTable, Column
+from astropy.table import QTable, Column, Row
 from astropy.time import Time
 from ..core import DataClass, Conf, DataClassError, FieldError
 
 
 def data_path(filename):
     data_dir = os.path.join(os.path.dirname(__file__), 'data')
     return os.path.join(data_dir, filename)
@@ -309,14 +309,22 @@
     assert isinstance(data, DataClass)
 
     # modify existing column using set
     data['z'] = 2
     assert data['z'][1] == 2
     assert isinstance(data, DataClass)
 
+    # modify existing column using alternative name
+    data = DataClass.from_dict(
+        {'rh': [1, 2, 3] * u.au,
+         'delta': [4, 5, 6] * u.au})
+    data['r'] = [7, 8, 9] * u.au
+    assert u.allclose(data['rh'], [7, 8, 9] * u.au)
+    assert set(data.field_names) == {'rh', 'delta'}
+
 
 def test_units():
     """ test units on multi-row tables """
 
     ground_truth = QTable([[1, 2, 3]*u.Unit('m'),
                            [4, 5, 6]*u.m/u.s,
                            ['a', 'b', 'c']],
@@ -406,24 +414,28 @@
                 len(set(sum(Conf.fieldnames, []))))
 
     # revert changes to Conf.fieldnames
     Conf.fieldnames = storage[0]
     Conf.fieldname_idx = storage[1]
 
 
-def test_translate_columns(monkeypatch):
-    """test function that translates column names"""
+def test_translate_columns_and_contains(monkeypatch):
+    """test function that translates column names and the `in` operator"""
 
     new_fieldnames_info = [
         {
             'fieldnames': ['zz', 'aa'],
             'dimension': dimensions.length
+        },
+        {
+            'fieldnames': ['yy', 'dd'],
+            'dimension': dimensions.time
         }
     ]
-    new_fieldnames = [['zz', 'aa']]
+    new_fieldnames = [['zz', 'aa'], ['yy', 'dd']]
     new_fieldname_idx = {}
     for idx, field in enumerate(new_fieldnames):
         for alt in field:
             new_fieldname_idx[alt] = idx
     monkeypatch.setattr(Conf, "fieldnames_info", new_fieldnames_info)
     monkeypatch.setattr(Conf, "fieldnames", new_fieldnames)
     monkeypatch.setattr(Conf, "fieldname_idx", new_fieldname_idx)
@@ -433,15 +445,25 @@
                      ('bb', [4, 5, 6]*u.m/u.s),
                      ('cc', ['a', 'b', 'c']))))
 
     assert tab._translate_columns(['aa', 'bb', 'cc']) == ['aa', 'bb', 'cc']
     assert tab._translate_columns(['zz', 'bb', 'cc']) == ['aa', 'bb', 'cc']
 
     with pytest.raises(KeyError):
-        tab._translate_columns(['x'])
+        tab._translate_columns(['x'])  # undefined column name
+        tab._translate_columns(['dd'])  # defined column name but not in table
+
+    trans = tab._translate_columns(['x', 'dd'], ignore_missing=True)
+    assert trans == ['x', 'dd']
+
+    assert 'aa' in tab
+    assert 'bb' in tab
+    assert 'zz' in tab
+    assert 'x' not in tab  # undefined column name
+    assert 'dd' not in tab  # defined column name but no in table
 
 
 def test_indexing():
     """make sure that indexing functionality is not compromised through
     column name translation"""
 
     tab = DataClass.from_dict(
@@ -546,21 +568,24 @@
 def test_io():
     """test file writing and reading capabilities"""
     tab = DataClass.from_dict(OrderedDict([('aa', [1, 2, 3]*u.m),
                                            ('bb', [4, 5, 6]),
                                            ('cc', [7, 8, 9]*u.kg)]))
     tab.meta['test'] = 'stuff'
 
-    tab.to_file('dataclass_table.fits', format='fits', overwrite=True)
+    try:
+        tab.to_file('dataclass_table.fits', format='fits', overwrite=True)
 
-    tab2 = DataClass.from_file('dataclass_table.fits', format='fits')
+        tab2 = DataClass.from_file('dataclass_table.fits', format='fits')
 
-    assert all(tab.table == tab2.table)
-    assert tab.meta == {key.lower(): val.lower()
-                        for key, val in tab2.meta.items()}
+        assert all(tab.table == tab2.table)
+        assert tab.meta == {key.lower(): val.lower()
+                            for key, val in tab2.meta.items()}
+    finally:
+        os.unlink("dataclass_table.fits")
 
 
 def test_apply():
     """test DataClass.apply"""
     tab = DataClass.from_columns([[2451223, 2451224, 2451226]*u.d,
                                   [120.1, 121.3, 124.9]*u.deg,
                                   [12.4, 12.2, 10.8]*u.deg],
@@ -576,7 +601,122 @@
                                  names=('JD', 'RA', 'DEC'))
     tab.apply([12.1, 12.5, 12.6]*u.mag, name='V')
 
     assert len(tab) == 3
 
     with pytest.raises(DataClassError):
         tab.apply([12.1, 12.5, 12.6, 99]*u.mag, name='V')  # wrong size
+
+
+def test_add_row():
+    """test DataClass.add_row"""
+    tab = DataClass.from_columns([Time([2451223, 2451224, 2451226],
+                                       format='jd'),
+                                  [120.1, 121.3, 124.9]*u.deg,
+                                  [12.4, 12.2, 10.8]*u.deg],
+                                 names=('JD', 'RA', 'DEC'))
+    # add astropy Row
+    r = tab.table[0]
+    assert isinstance(r, Row)
+    tab.add_row(r)
+    assert len(tab) == 4
+    assert tab.table[-1] == r
+
+    # add a dict
+    r = {'JD': 2451228 * u.d, 'RA': 130 * u.deg, 'DEC': 8 * u.deg}
+    tab.add_row(r)
+    assert len(tab) == 5
+    assert all(tab[-1]['JD'] == Time(r['JD'], format='jd'))
+    for k in ['RA', 'DEC']:
+        assert u.isclose(tab[-1][k], r[k])
+
+    # add an iterable that matches the existing columns
+    r = [2451130 * u.d, 135 * u.deg, 6 * u.deg]
+    tab.add_row(r)
+    assert len(tab) == 6
+    assert all(tab[-1]['JD'] == Time(r[0], format='jd'))
+    for i, k in enumerate(tab.field_names[1:]):
+        assert u.isclose(tab[-1][k], r[i+1])
+
+    # add an iterable with specified column names
+    r = [2451132 * u.d, 140 * u.deg, 3 * u.au]
+    n = ['JD', 'RA', 'rh']  # with a new column and missing an existing column
+    tab.add_row(r, n)
+    assert len(tab) == 7
+    assert set(tab.field_names) == {'JD', 'RA', 'DEC', 'rh'}
+    assert all(tab[-1]['JD'] == Time(r[0], format='jd'))
+    for i, k in enumerate(n[1:]):
+        assert u.isclose(tab[-1][k], r[i+1])
+
+    # time represented by a string
+    r = ['1998-11-18', 120 * u.deg, 3 * u.au]
+    n = ['JD', 'RA', 'rh']
+    tab.add_row(r, n)
+    assert len(tab) == 8
+    assert all(tab[-1]['JD'] == r[0])
+
+    # specify different names from the Mapping object
+    r = {'JD': 2451228 * u.d, 'RA': 130 * u.deg, 'DEC': 8 * u.deg}
+    n = ['JD', 'RA', 'phase']
+    tab.add_row(r, n)
+    assert len(tab) == 9
+    assert set(tab.field_names) == {'JD', 'RA', 'DEC', 'rh', 'phase'}
+    assert u.isclose(tab[-1]['phase'], r['DEC'])
+
+
+def test_vstack():
+    """test DataClass.vstack"""
+    tab = DataClass.from_columns([[2451223, 2451224, 2451226]*u.d,
+                                  [120.1, 121.3, 124.9]*u.deg,
+                                  [12.4, 12.2, 10.8]*u.deg],
+                                 names=('JD', 'RA', 'DEC'))
+
+    # join a DataClass, same columns
+    assert isinstance(tab, DataClass)
+    tab.vstack(tab)
+    assert len(tab) == 6
+    assert set(tab.field_names) == {'JD', 'RA', 'DEC'}
+    assert all(tab.table[:3] == tab.table[-3:])
+
+    # join a Table
+    delta_tab = tab.table
+    assert isinstance(delta_tab, QTable)
+    tab.vstack(delta_tab)
+    assert len(tab) == 12
+    assert set(tab.field_names) == {'JD', 'RA', 'DEC'}
+    assert all(tab.table[:6] == tab.table[-6:])
+
+    # join a dict
+    delta_tab = dict(tab.table)
+    assert isinstance(delta_tab, dict)
+    tab.vstack(dict(delta_tab))
+    assert len(tab) == 24
+    assert set(tab.field_names) == {'JD', 'RA', 'DEC'}
+    assert all(tab.table[:6] == tab.table[-6:])
+
+    # join an unrecoganized object
+    with pytest.raises(ValueError):
+        tab.vstack([1, 2, 3])
+
+    # join a table with different sets of columns
+    tab = DataClass.from_columns([[2451223, 2451224, 2451226]*u.d,
+                                  [120.1, 121.3, 124.9]*u.deg,
+                                  [12.4, 12.2, 10.8]*u.deg],
+                                 names=('JD', 'RA', 'DEC'))
+    subtab = QTable([[1, 2, 3] * u.au,
+                     [1, 2, 3] * u.au,
+                     [20, 30, 40] * u.deg],
+                    names=('r', 'delta', 'DEC'))
+    field0 = tab.field_names
+    tab.vstack(subtab)
+    assert len(tab) == 6
+    assert set(field0).union(set(subtab.colnames)) == set(tab.field_names)
+
+    # join a table that has a column using alternative names
+    subtab = QTable([[4, 5] * u.au,
+                     [10, 20] * u.deg],
+                    names=('rh', 'phase'))
+    field0 = tab.field_names
+    tab.vstack(subtab)
+    assert len(tab) == 8
+    assert 'rh' not in tab.table.colnames
+    assert set(field0).union({'phase'}) == set(tab.field_names)
```

### Comparing `sbpy-0.3.0/sbpy/data/tests/test_decorators.py` & `sbpy-0.4.0/sbpy/data/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/data/tests/test_ephem.py` & `sbpy-0.4.0/sbpy/data/tests/test_ephem.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/data/tests/test_ephem_remote.py` & `sbpy-0.4.0/sbpy/data/tests/test_ephem_remote.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/data/tests/test_names.py` & `sbpy-0.4.0/sbpy/data/tests/test_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
                                'desig': '1973 QO1'},
     "361267 `I`iwi (2006 SV395)": {'number': 361267, 'name':
                                    '`I`iwi', 'desig': '2006 SV395'},
     "374710 `O`o (2006 RJ110)": {'number': 374710, 'name':
                                  '`O`o', 'desig': '2006 RJ110'},
     "(20123) A900 MA": {'number': 20123, 'desig': '1900 MA'},
     "1A": {'desig': '1A'},
+    "A/2018 V3": {'desig': '2018 V3'}
 }
 
 
 def test_natural_sort_key():
     items = ['1A10', '1A2', 'B3', 'B20', 'C', '4D', 'CE24', 'CC3D', 0]
     items = sorted(items, key=natural_sort_key)
     test = [0, '1A2', '1A10', '4D', 'B3', 'B20', 'C', 'CC3D', 'CE24']
@@ -88,17 +89,16 @@
 
 def test_asteroid_or_comet():
     """Test target name identification."""
     for comet in comets:
         assert Names.asteroid_or_comet(comet) == 'comet', \
             'failed for {}'.format(comet)
     for asteroid in asteroids:
-        if asteroid != '2017 U1':
-            assert Names.asteroid_or_comet(asteroid) == 'asteroid', \
-                'failed for {}'.format(asteroid)
+        assert Names.asteroid_or_comet(asteroid) == 'asteroid', \
+            'failed for {}'.format(asteroid)
 
 
 def test_from_packed():
     """Test packed numbers and designations.
 
     Test values from https://www.minorplanetcenter.net/iau/info/PackedDes.html
```

### Comparing `sbpy-0.3.0/sbpy/data/tests/test_obs_remote.py` & `sbpy-0.4.0/sbpy/data/tests/test_obs_remote.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/data/tests/test_orbit_remote.py` & `sbpy-0.4.0/sbpy/data/tests/test_orbit_remote.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                   'stop': Time('2018-01-05', format='iso'),
                   'number': 10}
         data = Orbit.from_horizons('Ceres', epochs=epochs)
         assert len(data.table) == 10
 
     def test_mult_epochs(self):
         # discrete epochs - astropy.time.Time objects
-        epochs = Time(['2018-01-02', '2018-01-05'], format='iso')
+        epochs = Time(['2018-01-02', '2018-01-05'], format='iso', scale='tdb')
         data = Orbit.from_horizons('Ceres', epochs=epochs)
         assert len(data.table) == 2
 
     def test_mult_objects(self):
         # query two objects
         data = Orbit.from_horizons(['Ceres', 'Pallas'])
         assert len(data.table) == 2
@@ -177,17 +177,37 @@
         """ test oo_propagate method"""
 
         orbit = Orbit.from_horizons('Ceres')
         epoch = Time(Time.now().jd + 100, format='jd', scale='utc')
 
         future_orbit = Orbit.from_horizons('Ceres',
                                            epochs=Time(epoch, format='jd',
-                                                       scale='utc'))
+                                                       scale='utc').tdb)
 
         oo_orbit = orbit.oo_propagate(epoch)
 
         elements = ['a', 'e', 'i', 'Omega', 'w', 'M']
         assert all([u.isclose(oo_orbit[k][0], future_orbit[k][0])
-                   for k in elements])
+                    for k in elements])
         assert u.isclose(oo_orbit['epoch'][0].utc.jd,
                          future_orbit['epoch'][0].utc.jd)
         assert oo_orbit['epoch'].scale == 'utc'
+
+
+@pytest.mark.remote_data
+class TestTisserand:
+    def test_tisserand(self):
+        """Test against JPL values for -0.605 using epoch JD = 2449400.5
+        elements.
+        """
+        epoch = Time(2449400.5, format='jd', scale='tdb')
+        halley = Orbit.from_horizons('1P', id_type='designation',
+                                     closest_apparition=True, epochs=epoch)
+        jupiter = Orbit.from_horizons(599, id_type=None, epochs=epoch)
+        assert u.isclose(halley.tisserand(jupiter), -0.60495016)
+
+        chariklo = Orbit.from_horizons('chariklo', id_type='name',
+                                       closest_apparition=True, epochs=epoch)
+        assert u.allclose(chariklo.tisserand(['599', '699', '799', '899'],
+                                             epoch=epoch),
+                          [3.47740968, 2.92990768, 2.85749431, 3.22074493],
+                          atol=1e-5)
```

### Comparing `sbpy-0.3.0/sbpy/exceptions.py` & `sbpy-0.4.0/sbpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/ginga_plugins/CometaryEnhancements.py` & `sbpy-0.4.0/sbpy/ginga_plugins/CometaryEnhancements.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/ginga_plugins/__init__.py` & `sbpy-0.4.0/sbpy/ginga_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/imageanalysis/core.py` & `sbpy-0.4.0/sbpy/imageanalysis/core.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/imageanalysis/tests/test_utils.py` & `sbpy-0.4.0/sbpy/imageanalysis/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/imageanalysis/utils.py` & `sbpy-0.4.0/sbpy/imageanalysis/utils.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/obsutil/core.py` & `sbpy-0.4.0/sbpy/obsutil/core.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/bandpass.py` & `sbpy-0.4.0/sbpy/photometry/bandpass.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/2mass-h-rsr.txt` & `sbpy-0.4.0/sbpy/photometry/data/2mass-h-rsr.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/2mass-j-rsr.txt` & `sbpy-0.4.0/sbpy/photometry/data/2mass-j-rsr.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/2mass-ks-rsr.txt` & `sbpy-0.4.0/sbpy/photometry/data/2mass-ks-rsr.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/README` & `sbpy-0.4.0/sbpy/photometry/data/README`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/WISE-RSR-W1.EE.txt` & `sbpy-0.4.0/sbpy/photometry/data/WISE-RSR-W1.EE.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/WISE-RSR-W2.EE.txt` & `sbpy-0.4.0/sbpy/photometry/data/WISE-RSR-W2.EE.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/WISE-RSR-W3.EE.txt` & `sbpy-0.4.0/sbpy/photometry/data/WISE-RSR-W3.EE.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/WISE-RSR-W4.EE.txt` & `sbpy-0.4.0/sbpy/photometry/data/WISE-RSR-W4.EE.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/atlas-c.txt` & `sbpy-0.4.0/sbpy/photometry/data/atlas-c.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/atlas-o.txt` & `sbpy-0.4.0/sbpy/photometry/data/atlas-o.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/cousins_i_004_syn.fits` & `sbpy-0.4.0/sbpy/photometry/data/cousins_i_004_syn.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/cousins_r_004_syn.fits` & `sbpy-0.4.0/sbpy/photometry/data/cousins_r_004_syn.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/johnson_b_004_syn.fits` & `sbpy-0.4.0/sbpy/photometry/data/johnson_b_004_syn.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/johnson_u_004_syn.fits` & `sbpy-0.4.0/sbpy/photometry/data/johnson_u_004_syn.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/johnson_v_004_syn.fits` & `sbpy-0.4.0/sbpy/photometry/data/johnson_v_004_syn.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/ps1-gp1.txt` & `sbpy-0.4.0/sbpy/photometry/data/ps1-gp1.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/ps1-ip1.txt` & `sbpy-0.4.0/sbpy/photometry/data/ps1-ip1.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/ps1-rp1.txt` & `sbpy-0.4.0/sbpy/photometry/data/ps1-rp1.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/ps1-wp1.txt` & `sbpy-0.4.0/sbpy/photometry/data/ps1-wp1.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/ps1-yp1.txt` & `sbpy-0.4.0/sbpy/photometry/data/ps1-yp1.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/ps1-zp1.txt` & `sbpy-0.4.0/sbpy/photometry/data/ps1-zp1.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/sdss-g.fits` & `sbpy-0.4.0/sbpy/photometry/data/sdss-g.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/sdss-i.fits` & `sbpy-0.4.0/sbpy/photometry/data/sdss-i.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/sdss-r.fits` & `sbpy-0.4.0/sbpy/photometry/data/sdss-r.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/sdss-u.fits` & `sbpy-0.4.0/sbpy/photometry/data/sdss-u.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/sdss-z.fits` & `sbpy-0.4.0/sbpy/photometry/data/sdss-z.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/wfc3_uvis_f438w_004_syn.fits` & `sbpy-0.4.0/sbpy/photometry/data/wfc3_uvis_f438w_004_syn.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/data/wfc3_uvis_f606w_004_syn.fits` & `sbpy-0.4.0/sbpy/photometry/data/wfc3_uvis_f606w_004_syn.fits`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/tests/test_bandpass.py` & `sbpy-0.4.0/sbpy/photometry/tests/test_bandpass.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/photometry/tests/test_core.py` & `sbpy-0.4.0/sbpy/photometry/tests/test_iau.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,168 +1,38 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import numpy as np
 import pytest
 from astropy import units as u
 from astropy.modeling import Parameter
+from astropy.modeling.fitting import SLSQPLSQFitter
 from ...calib import solar_fluxd
-from ..core import *
 from ...data import Ephem, Phys
+from ..core import InvalidPhaseFunctionWarning
+from ..iau import HG, HG12, HG1G2, HG12_Pen16, _check_bounds
 
 
 def setup_module(module):
     module.solar_fluxd_default = solar_fluxd.get()
     solar_fluxd.set({'V': -26.77 * u.mag})
 
 
 def teardown_module(module):
     solar_fluxd.set(module.solar_fluxd_default)
 
 
-class TestDiskIntegratedPhaseFunc():
-    def test__unit(self):
-        class TestClass(DiskIntegratedPhaseFunc):
-            p = Parameter(default=1.)
-
-            @staticmethod
-            def evaluate(a, p):
-                return a * p
-
-        temp = TestClass()
-        with pytest.raises(ValueError):
-            temp._check_unit()
-
-    def test_ref_phasefunc(self):
-        class ExpPhase(DiskIntegratedPhaseFunc):
-            _unit = 'ref'
-            p = Parameter(default=0.1 / u.sr)
-            nu = Parameter(default=0.1 / u.rad)
-
-            @staticmethod
-            def evaluate(a, p, nu):
-                return p * np.exp(-nu * a)
-
-        exp_phase = ExpPhase()
-        pha_test = np.linspace(0, 120, 10) * u.deg
-        ref_test = [0.1, 0.09769976, 0.09545244, 0.0932568, 0.09111168,
-                    0.08901589, 0.08696831, 0.08496784, 0.08301337,
-                    0.08110387] / u.sr
-        ref = exp_phase(pha_test)
-        assert np.allclose(ref.value, ref_test.value)
-        assert ref.unit == ref_test.unit
-        ref_n_test = [1.01760649, 0.99419913, 0.97133019, 0.94898729,
-                      0.92715833, 0.90583148, 0.88499521, 0.86463822,
-                      0.84474949, 0.82531824]
-        ref_n = exp_phase.to_ref(pha_test, normalized=10 * u.deg)
-        assert np.allclose(ref_n, ref_n_test)
-
-        with pytest.raises(ValueError):
-            mag = exp_phase.to_mag(1 * u.rad)
-        with pytest.raises(ValueError):
-            mag = exp_phase.to_mag(1 * u.rad, unit=u.mag)
-        exp_phase.radius = 100 * u.km
-        with pytest.raises(ValueError):
-            mag = exp_phase.to_mag(1 * u.rad, unit=u.mag)
-        exp_phase.wfb = 'V'
-        mag = exp_phase.to_mag(pha_test, unit=u.mag)
-        mag_test = [5.36175238, 5.38701861, 5.41228484, 5.43755106,
-                    5.46281729, 5.48808352, 5.51334975, 5.53861598, 5.56388221,
-                    5.58914844] * u.mag
-        assert np.allclose(mag.value, mag_test.value)
-        assert mag.unit == mag_test.unit
-
-        eph_dict = {'alpha': pha_test,
-                    'r': np.repeat(0.8 * u.au, 10),
-                    'delta': np.repeat(0.5 * u.au, 10)}
-        eph_test = Ephem.from_dict(eph_dict)
-        ref1 = exp_phase.to_ref(eph_test)
-        assert np.allclose(ref1.value, ref_test.value)
-
-
-class TestLinear():
-    def test_init(self):
-        linphase = LinearPhaseFunc(5 * u.mag, 0.04 * u.mag/u.deg,
-                                   radius=300 * u.km, wfb='V')
-        assert np.isclose(linphase.H.value, 5)
-        assert linphase.H.unit == u.mag
-        assert np.isclose(linphase.S.value, 0.04)
-        assert linphase.S.unit == u.mag/u.deg
-        assert linphase.radius == 300 * u.km
-        assert linphase.wfb == 'V'
-
-    def test_to_mag(self):
-        linphase = LinearPhaseFunc(5 * u.mag, 0.04 * u.mag/u.deg,
-                                   radius=300 * u.km)
-        pha_test = np.linspace(0, np.pi, 10) * u.rad
-        mag_test = [5., 5.8, 6.6, 7.4, 8.2, 9., 9.8, 10.6, 11.4, 12.2] * u.mag
-        eph = linphase.to_mag(pha_test, append_results=True)
-        assert np.allclose(eph['mag'].value, mag_test.value)
-        assert eph['mag'].unit == mag_test.unit
-        assert np.allclose(eph['alpha'].value, pha_test.value)
-        assert eph['alpha'].unit == pha_test.unit
-        assert set(eph.field_names) == {'alpha', 'mag'}
-        eph = linphase.to_mag(eph, append_results=True)
-        assert set(eph.field_names) == {'alpha', 'mag', 'mag1'}
-
-    def test_to_ref(self):
-        linphase = LinearPhaseFunc(5 * u.mag, 0.04 * u.mag/u.deg,
-                                   radius=300 * u.km, wfb='V')
-        pha_test = np.linspace(0, 180, 10) * u.deg
-        eph = linphase.to_ref(pha_test, append_results=True)
-        ref_test = [1.55045242e-02, 7.42093183e-03, 3.55188129e-03,
-                    1.70003727e-03, 8.13688994e-04, 3.89456039e-04,
-                    1.86405380e-04, 8.92192241e-05, 4.27030055e-05,
-                    2.04389434e-05] / u.sr
-        ref_norm_test = np.array(
-            [1., 0.47863009, 0.22908677, 0.10964782, 0.05248075,
-             0.02511886, 0.01202264, 0.0057544, 0.00275423,
-             0.00131826]) * u.dimensionless_unscaled
-        assert u.allclose(eph['ref'], ref_test)
-        assert u.allclose(eph['alpha'], pha_test)
-        assert set(eph.field_names) == {'alpha', 'ref'}
-        eph_norm = linphase.to_ref(pha_test, normalized=0 * u.deg,
-                                   append_results=True)
-        assert u.allclose(eph_norm['ref'], ref_norm_test)
-        assert u.allclose(eph_norm['alpha'], pha_test)
-        assert set(eph_norm.field_names) == {'alpha', 'ref'}
-        eph = linphase.to_ref(eph, append_results=True)
-        assert set(eph.field_names) == {'alpha', 'ref', 'ref1'}
-        # test exception
-        linphase = LinearPhaseFunc(5 * u.mag, 0.04 * u.mag/u.deg,
-                                   radius=300 * u.km)
-        with pytest.raises(ValueError):
-            linphase.to_ref(10 * u.deg)
-
-    def test_props(self):
-        linphase = LinearPhaseFunc(5 * u.mag, 2.29 * u.mag/u.rad,
-                                   radius=300 * u.km, wfb='V')
-        assert np.isclose(linphase.geomalb, 0.0487089)
-        assert np.isclose(linphase.bondalb, 0.01790315)
-        assert np.isclose(linphase.phaseint, 0.36755394203990327)
-
-    def test__distance_module(self):
-        r = [0.5, 1, 1.2, 2] * u.au
-        delta = [0.3, 1, 1, 2] * u.au
-        m = LinearPhaseFunc(5 * u.mag, 0.04 * u.mag / u.deg)
-        module_test = [0.0225, 1., 1.44, 16.]
-        module = m._distance_module(Ephem.from_dict({'r': r, 'delta': delta}))
-        assert np.allclose(module, module_test)
-
-    def test_fit(self):
-        pha = np.linspace(0, 60, 100) * u.deg
-        mag = LinearPhaseFunc(5 * u.mag, 0.04 * u.mag/u.deg)(pha) + \
-            (np.random.rand(100)*0.2-0.1) * u.mag
-        from astropy.modeling.fitting import LevMarLSQFitter
-        fitter = LevMarLSQFitter()
-        m0 = LinearPhaseFunc(3 * u.mag, 0.02 * u.mag/u.deg)
-        m = fitter(m0, pha, mag)
-        assert isinstance(m, LinearPhaseFunc)
-
-    def test_fit_deriv(self):
-        assert np.allclose(LinearPhaseFunc.fit_deriv(1, 1, 2), [1, 1])
+def test__check_bounds():
+    with pytest.warns(Warning):
+        _check_bounds(1, [2, 3], Warning)
+        _check_bounds(5, [2, 3], Warning)
+        _check_bounds(np.array([1, 2, 2.5]), [2, 3], Warning)
+    with pytest.raises(Exception):
+        _check_bounds(1, [2, 3], Exception)
+    _check_bounds(2.5, [2, 3], Exception)
+    _check_bounds(np.array([2.1, 2.2, 3]), [2, 3], Exception)
 
 
 class TestHG:
     def test_init(self):
         # initialize with numbers
         ceres = HG(3.34 * u.mag, 0.12, radius=480 * u.km, wfb='V')
         assert u.isclose(ceres.radius, 480 * u.km)
@@ -247,49 +117,48 @@
                94.73684211, 101.05263158, 107.36842105, 113.68421053,
                120.] * u.deg
         data = [3.14451639, 4.06262914, 4.1154297, 4.54870242, 4.42265052,
                 4.71990531, 5.1628504, 5.16098737, 5.20971821, 5.3032115,
                 5.52976173, 5.64255607, 5.84536878, 6.13724017, 6.33675472,
                 6.63099954, 7.2461781, 7.32734464, 8.00147425,
                 8.40595306] * u.mag
-        from astropy.modeling.fitting import LevMarLSQFitter
-        fitter = LevMarLSQFitter()
+        fitter = SLSQPLSQFitter()
         # test fit with one column
         m = HG.from_obs({'alpha': pha, 'mag': data}, fitter)
         assert isinstance(m, HG)
         assert isinstance(m.H, Parameter) & np.isclose(
-            m.H.value, 3.436677) & (m.H.unit == u.mag)
+            m.H.value, 3.43668488) & (m.H.unit == u.mag)
         assert isinstance(m.G, Parameter) & np.isclose(
-            m.G.value, 0.1857588) & (m.G.unit == u.dimensionless_unscaled)
+            m.G.value, 0.18576227) & (m.G.unit == u.dimensionless_unscaled)
         # test fit with one column and `init` parameters
         m = HG.from_obs({'alpha': pha, 'mag': data}, fitter, init=[3, 0.1])
         assert isinstance(m, HG)
         assert isinstance(m.H, Parameter) & np.isclose(
-            m.H.value, 3.4366849) & (m.H.unit == u.mag)
+            m.H.value, 3.43674827) & (m.H.unit == u.mag)
         assert isinstance(m.G, Parameter) & np.isclose(
-            m.G.value, 0.18576319) & (m.G.unit == u.dimensionless_unscaled)
+            m.G.value, 0.18580637) & (m.G.unit == u.dimensionless_unscaled)
         # test fit with more than one column
         m = HG.from_obs({'alpha': pha, 'mag': data, 'mag1': data,
                          'mag2': data}, fitter, fields=['mag', 'mag1', 'mag2'])
         assert isinstance(m, HG)
         assert isinstance(m.H, Parameter) & np.allclose(
-            m.H.value, [3.436677]*3) & (m.H.unit == u.mag)
+            m.H.value, [3.43668488]*3) & (m.H.unit == u.mag)
         assert isinstance(m.G, Parameter) & np.allclose(
-            m.G.value, [0.1857588]*3) & (m.G.unit == u.dimensionless_unscaled)
+            m.G.value, [0.18576227]*3) & (m.G.unit == u.dimensionless_unscaled)
         assert 'fields' in m.meta
         assert m.meta['fields'] == ['mag', 'mag1', 'mag2']
         # test fit with more than one column with `init` parameters
         m = HG.from_obs({'alpha': pha, 'mag': data, 'mag1': data,
                          'mag2': data}, fitter, fields=['mag', 'mag1', 'mag2'],
                         init=[[3., 3., 3.], [0.1, 0.1, 0.1]])
         assert isinstance(m, HG)
         assert isinstance(m.H, Parameter) & np.allclose(
-            m.H.value, [3.4366849]*3) & (m.H.unit == u.mag)
+            m.H.value, [3.43674827]*3) & (m.H.unit == u.mag)
         assert isinstance(m.G, Parameter) & np.allclose(
-            m.G.value, [0.18576319]*3) & (m.G.unit == u.dimensionless_unscaled)
+            m.G.value, [0.18580637]*3) & (m.G.unit == u.dimensionless_unscaled)
         assert 'fields' in m.meta
         assert m.meta['fields'] == ['mag', 'mag1', 'mag2']
 
     def test_to_mag(self):
         ceres = HG(3.34 * u.mag, 0.12, radius=480 * u.km, wfb='V')
         eph_dict = {'alpha': np.linspace(0, np.pi*0.9, 10) * u.rad,
                     'r': np.repeat(2.7*u.au, 10),
@@ -339,15 +208,15 @@
         assert set(eph4.field_names) == {'alpha', 'ref'}
         assert u.allclose(eph3['ref'], ref1_test)
         assert u.allclose(eph4['ref'], ref2_norm_test)
         ref5 = ceres.to_ref(pha_test)
         assert u.allclose(ref5, ref1_test)
 
     def test_g_validate(self):
-        with pytest.warns(NonmonotonicPhaseFunctionWarning):
+        with pytest.warns(InvalidPhaseFunctionWarning):
             m = HG(0, 1.2)
 
     def test_hgphi_exception(self):
         with pytest.raises(ValueError):
             tmp = HG._hgphi(0, 0)
         with pytest.raises(ValueError):
             tmp = HG._hgphi(0, 3)
@@ -421,24 +290,23 @@
                94.73684211, 101.05263158, 107.36842105, 113.68421053,
                120.] * u.deg
         data = [7.14679706, 7.32220201, 7.85637226, 7.98824651, 8.2029765,
                 8.27574759, 8.49437766, 9.05650671, 8.79649221, 9.33071561,
                 9.24703668, 9.49069761, 9.57246629, 10.12429626, 10.14465944,
                 10.51021594, 10.63215313, 11.15570421, 11.44890748,
                 11.43888611] * u.mag
-        from astropy.modeling.fitting import LevMarLSQFitter
-        fitter = LevMarLSQFitter()
+        fitter = SLSQPLSQFitter()
         m = HG1G2.from_obs({'alpha': pha, 'mag': data}, fitter)
         assert isinstance(m, HG1G2)
         assert isinstance(m.H, Parameter) & np.isclose(
-            m.H.value, 7.1167) & (m.H.unit == u.mag)
+            m.H.value, 7.11670348) & (m.H.unit == u.mag)
         assert isinstance(m.G1, Parameter) & np.isclose(
-            m.G1.value, 0.63922) & (m.G1.unit == u.dimensionless_unscaled)
+            m.G1.value, 0.63922934) & (m.G1.unit == u.dimensionless_unscaled)
         assert isinstance(m.G2, Parameter) & np.isclose(
-            m.G2.value, 0.17262569) & (m.G2.unit == u.dimensionless_unscaled)
+            m.G2.value, 0.17261464) & (m.G2.unit == u.dimensionless_unscaled)
 
     def test_to_mag(self):
         themis = HG1G2(7.063 * u.mag, 0.62, 0.14, radius=100 * u.km, wfb='V')
         pha_test = np.linspace(0, np.pi, 10)*u.rad
         mag_test = [7.063, 8.07436233, 8.68048572, 9.29834638, 9.96574599,
                     10.72080704, 11.52317465, 12.15094612, 18.65369516,
                     18.65389398] * u.mag
@@ -450,15 +318,15 @@
         ref_test = [2.08689669e-02, 8.22159390e-03, 4.70442623e-03,
                     2.66294623e-03, 1.44013284e-03, 7.18419542e-04,
                     3.43108196e-04, 1.92452033e-04, 4.82195204e-07,
                     4.82106912e-07] / u.sr
         assert u.allclose(themis.to_ref(pha_test), ref_test)
 
     def test_g1g2_validator(self):
-        with pytest.warns(NonmonotonicPhaseFunctionWarning):
+        with pytest.warns(InvalidPhaseFunctionWarning):
             m = HG1G2(0, -0.2, 0.5)
             m = HG1G2(0, 0.5, -0.2)
             m = HG1G2(0, 0.6, 0.6)
 
 
 class TestHG12:
     def test_init(self):
@@ -521,22 +389,21 @@
                94.73684211, 101.05263158, 107.36842105, 113.68421053,
                120.] * u.deg
         data = [6.95036472, 7.71609702, 8.04175457, 7.88226545, 8.28192813,
                 8.50954834, 8.36880691, 8.73216696, 8.90742914, 9.05696656,
                 9.20869753, 9.52578025, 9.8427691, 9.91588852, 10.3636637,
                 10.26459992, 10.79316978, 10.79202241, 11.36950747,
                 11.61018708] * u.mag
-        from astropy.modeling.fitting import LevMarLSQFitter
-        fitter = LevMarLSQFitter()
+        fitter = SLSQPLSQFitter()
         m = HG12.from_obs({'alpha': pha, 'mag': data}, fitter)
         assert isinstance(m, HG12)
         assert isinstance(m.H, Parameter) & np.isclose(
-            m.H.value, 7.13939) & (m.H.unit == u.mag)
+            m.H.value, 7.13938908) & (m.H.unit == u.mag)
         assert isinstance(m.G12, Parameter) & np.isclose(
-            m.G12.value, 0.44872) & (m.G12.unit == u.dimensionless_unscaled)
+            m.G12.value, 0.448715) & (m.G12.unit == u.dimensionless_unscaled)
 
     def test_to_mag(self):
         pha_test = np.linspace(0, np.pi, 10) * u.rad
         mag_test = [7.121, 8.07252953, 8.67890827, 9.2993879, 9.96817595,
                     10.72086969, 11.51208664, 12.12722017, 18.70628001,
                     18.70647883] * u.mag
         themis = HG12(7.121 * u.mag, 0.68)
@@ -548,15 +415,15 @@
                     2.66039298e-03, 1.43691333e-03, 7.18378086e-04,
                     3.46630119e-04, 1.96703860e-04, 4.59397839e-07,
                     4.59313722e-07] / u.sr
         themis = HG12(7.121 * u.mag, 0.68, radius=100 * u.km, wfb='V')
         assert u.allclose(themis.to_ref(pha_test), ref_test)
 
     def test_g_validator(self):
-        with pytest.warns(NonmonotonicPhaseFunctionWarning):
+        with pytest.warns(InvalidPhaseFunctionWarning):
             m = HG12(0, -0.71)
             m = HG12(0, 1.31)
 
     def test_G1_G2(self):
         themis = HG12(7.121 * u.mag, 0.68, radius=100 * u.km, wfb='V')
         assert np.isclose(themis._G1, 0.669592)
         assert np.isclose(themis._G2, 0.1407)
@@ -615,22 +482,21 @@
                94.73684211, 101.05263158, 107.36842105, 113.68421053,
                120.] * u.deg
         data = [7.15663893, 7.4389134, 8.00006177, 7.9044872, 8.16865497,
                 8.51010016, 8.63386712, 8.65893367, 8.84895152, 9.24495642,
                 9.16195702, 9.54770054, 9.60599559, 10.06129054, 10.22544773,
                 10.49122575, 10.78544483, 11.12145723, 11.18055954,
                 11.40468613] * u.mag
-        from astropy.modeling.fitting import LevMarLSQFitter
-        fitter = LevMarLSQFitter()
+        fitter = SLSQPLSQFitter()
         m = HG12_Pen16.from_obs({'alpha': pha, 'mag': data}, fitter)
         assert isinstance(m, HG12_Pen16)
         assert isinstance(m.H, Parameter) & np.isclose(
-            m.H.value, 7.038705) & (m.H.unit == u.mag)
+            m.H.value, 7.03870429) & (m.H.unit == u.mag)
         assert isinstance(m.G12, Parameter) & np.isclose(
-            m.G12.value, 0.681691) & (m.G12.unit == u.dimensionless_unscaled)
+            m.G12.value, 0.68169538) & (m.G12.unit == u.dimensionless_unscaled)
 
     def test_to_mag(self):
         pha_test = np.linspace(0, np.pi, 10) * u.rad
         mag_test = [7.121, 8.12425116, 8.71866169, 9.32576929, 9.98752147,
                     10.7522335, 11.60154855, 12.28573613, 18.49298496,
                     18.49318378] * u.mag
         themis = HG12_Pen16(7.121 * u.mag, 0.68)
@@ -642,10 +508,10 @@
                     2.59652934e-03, 1.41153731e-03, 6.97923066e-04,
                     3.19213708e-04, 1.69983395e-04, 5.59122499e-07,
                     5.59020121e-07] / u.sr
         themis = HG12_Pen16(7.121 * u.mag, 0.68, radius=100 * u.km, wfb='V')
         assert u.allclose(themis.to_ref(pha_test), ref_test)
 
     def test_g_validator(self):
-        with pytest.warns(NonmonotonicPhaseFunctionWarning):
+        with pytest.warns(InvalidPhaseFunctionWarning):
             m = HG12(0, -0.71)
             m = HG12(0, 1.31)
```

### Comparing `sbpy-0.3.0/sbpy/shape/core.py` & `sbpy-0.4.0/sbpy/shape/core.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/spectroscopy/core.py` & `sbpy-0.4.0/sbpy/spectroscopy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 except ImportError:
     class SpectralElement:
         pass
 
 
 __all__ = ['Spectrum', 'SpectralModel', 'SpectralGradient']
 
+__doctest_requires__ = {
+    "SpectralGradient": ["astropy>=5.3"],
+    "SpectralGradient.from_color": ["astropy>=5.3"],
+    "SpectralGradient.renormalize": ["astropy>=5.3"],
+}
+
 
 class SpectralGradient(u.SpecificTypeQuantity):
     r"""Convert between magnitude and spectral gradient.
 
     ``SpectralGradient`` is a `~astropy.units.Quantity` object with
     units of percent change per wavelength.
 
@@ -70,25 +76,25 @@
 
     Examples
     --------
     >>> import astropy.units as u
     >>> from sbpy.units import hundred_nm
     >>> S = SpectralGradient(10 * u.percent / hundred_nm, wave0=5500 * u.AA)
     >>> print(S)
-    10.0 % / 100 nm
+    10.0 % / (100 nm)
 
     >>> from sbpy.units import VEGAmag
     >>> from sbpy.photometry import bandpass
     >>> V = bandpass('Johnson V')
     >>> R = bandpass('Cousins R')
     >>> VmR = 15.8 * VEGAmag - 15.3 * VEGAmag
     >>> VmR_sun = 0.37 * u.mag
     >>> S = SpectralGradient.from_color((V, R), VmR - VmR_sun)
     >>> print(S)    # doctest: +FLOAT_CMP
-    12.29185986266534 % / 100 nm
+    12.29185986266534 % / (100 nm)
 
 
     References
     ----------
     .. [ADT84] A'Hearn, Dwek & Tokunaga 1984. Infrared Photometry of
         Comet Bowell and Other Comets. ApJ 282, 803-806.
 
@@ -174,15 +180,15 @@
 
         Examples
         --------
         >>> import astropy.units as u
         >>> w = [0.4719, 0.6185] * u.um
         >>> S = SpectralGradient.from_color(w, 0.10 * u.mag)
         >>> print(S)                            # doctest: +FLOAT_CMP
-        6.27819572 % / 100 nm
+        6.27819572 % / (100 nm)
 
         """
         from ..units import hundred_nm
 
         lambda_eff = SpectralGradient._lambda_eff(wfb)
 
         try:
@@ -283,15 +289,15 @@
         >>> import astropy.units as u
         >>> from sbpy.spectroscopy import SpectralGradient
         >>> from sbpy.units import hundred_nm
         >>> S1 = SpectralGradient(10 * u.percent / hundred_nm,
         ...                      wave0=0.55 * u.um)
         >>> S2 = S1.renormalize(3.6 * u.um)
         >>> print(S2.renormalize(3.6 * u.um))    # doctest: +FLOAT_CMP
-        2.469135802469136 % / 100 nm
+        2.469135802469136 % / (100 nm)
         >>> print(S2.wave0)
         3.6 um
         """
 
         if self.wave0 is None:
             raise ValueError('wave0 attribute must be defined.')
```

### Comparing `sbpy-0.3.0/sbpy/spectroscopy/sources.py` & `sbpy-0.4.0/sbpy/spectroscopy/sources.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/spectroscopy/tests/test_sources.py` & `sbpy-0.4.0/sbpy/spectroscopy/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/spectroscopy/tests/test_specgrad.py` & `sbpy-0.4.0/sbpy/spectroscopy/tests/test_specgrad.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/tests/coveragerc` & `sbpy-0.4.0/sbpy/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/thermal/core.py` & `sbpy-0.4.0/sbpy/thermal/core.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/units/core.py` & `sbpy-0.4.0/sbpy/units/core.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/units/tests/data/hi05070405_9000036-avg-spec.txt` & `sbpy-0.4.0/sbpy/units/tests/data/hi05070405_9000036-avg-spec.txt`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/units/tests/data/hi05070405_9000036-avg-spec_ref.pdf` & `sbpy-0.4.0/sbpy/units/tests/data/hi05070405_9000036-avg-spec_ref.pdf`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy/units/tests/test_core.py` & `sbpy-0.4.0/sbpy/units/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/sbpy.egg-info/PKG-INFO` & `sbpy-0.4.0/sbpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: sbpy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python module for small-body planetary astronomy
 Home-page: https://sbpy.org
 Author: sbpy team
 Author-email: msk@astro.umd.edu
 License: BSD 3-Clause
 Keywords: astronomy,astrophysics,planetary,asteroid,comet,space,science
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.rst
 
-.. image:: https://github.com/NASA-Planetary-Science/sbpy/raw/master/logo/sbpy_logo_short.png
+.. image:: https://github.com/NASA-Planetary-Science/sbpy/raw/main/logo/sbpy_logo_short.png
     :width: 400px
     :align: center	    
     :alt: sbpy	     
 	  
        
 sbpy is an `Astropy <https://www.astropy.org/>`_ affiliated package for small-body
 planetary astronomy.
@@ -42,15 +41,15 @@
     :target: https://sbpy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation status
 
 .. image:: https://joss.theoj.org/papers/10.21105/joss.01426/status.svg
     :target: https://doi.org/10.21105/joss.01426
     :alt: JOSS documentation
 
-.. image:: https://codecov.io/gh/NASA-Planetary-Science/sbpy/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/NASA-Planetary-Science/sbpy/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/NASA-Planetary-Science/sbpy
     :alt: codecov status
 	  
 
 Overview
 --------
 
@@ -81,14 +80,12 @@
 
 sbpy is still under development, with v1.0 scheduled for delivery in 2024. For an overview on the status of individual features see the `Status Page <https://sbpy.readthedocs.io/en/latest/status.html>`_.
 
 
 Acknowledgements
 ----------------
 
-`sbpy` is supported by NASA PDART Grant No. 80NSSC18K0987.
+`sbpy` support provided by NASA PDART Grant Nos. 80NSSC18K0987 and 80NSSC22K0143.
 
 If you use `sbpy` in your work, please acknowledge it by citing
 
     `Mommert, Kelley, de-Val Borro, Li et al., (2019). sbpy: A Python module for small-body planetary astronomy. Journal of Open Source Software, 4(38), 1426 <https://joss.theoj.org/papers/8b8e7bb15fb4a14f80f2afd06b6ce060>`_
-
-
```

### Comparing `sbpy-0.3.0/sbpy.egg-info/SOURCES.txt` & `sbpy-0.4.0/sbpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 .gitignore
+.readthedocs.yaml
 CHANGES.rst
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE.rst
 MANIFEST.in
 README.rst
 pep8speaks.yml
 pip-requirements
 pyproject.toml
-readthedocs.yml
 setup.cfg
 setup.py
 tox.ini
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/issue-report.md
 .github/workflows/ci_cron_weekly.yml
 .github/workflows/ci_tests.yml
@@ -155,14 +155,15 @@
 sbpy/imageanalysis/tests/__init__.py
 sbpy/imageanalysis/tests/test_utils.py
 sbpy/obsutil/__init__.py
 sbpy/obsutil/core.py
 sbpy/photometry/__init__.py
 sbpy/photometry/bandpass.py
 sbpy/photometry/core.py
+sbpy/photometry/iau.py
 sbpy/photometry/data/2mass-h-rsr.txt
 sbpy/photometry/data/2mass-j-rsr.txt
 sbpy/photometry/data/2mass-ks-rsr.txt
 sbpy/photometry/data/README
 sbpy/photometry/data/WISE-RSR-W1.EE.txt
 sbpy/photometry/data/WISE-RSR-W2.EE.txt
 sbpy/photometry/data/WISE-RSR-W3.EE.txt
@@ -186,14 +187,15 @@
 sbpy/photometry/data/sdss-u.fits
 sbpy/photometry/data/sdss-z.fits
 sbpy/photometry/data/wfc3_uvis_f438w_004_syn.fits
 sbpy/photometry/data/wfc3_uvis_f606w_004_syn.fits
 sbpy/photometry/tests/__init__.py
 sbpy/photometry/tests/test_bandpass.py
 sbpy/photometry/tests/test_core.py
+sbpy/photometry/tests/test_iau.py
 sbpy/shape/__init__.py
 sbpy/shape/core.py
 sbpy/spectroscopy/__init__.py
 sbpy/spectroscopy/core.py
 sbpy/spectroscopy/sources.py
 sbpy/spectroscopy/tests/__init__.py
 sbpy/spectroscopy/tests/test_sources.py
```

### Comparing `sbpy-0.3.0/setup.cfg` & `sbpy-0.4.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [metadata]
 name = sbpy
 package_name = sbpy
 author = sbpy team
 author_email = msk@astro.umd.edu
 license = BSD 3-Clause
-license_file = LICENSE.rst
+license_files = 
+	LICENSE.rst
 url = https://sbpy.org
 description = Python module for small-body planetary astronomy
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 edit_on_github = False
 github_project = NASA-Planetary-Science/sbpy
 keywords = astronomy, astrophysics, planetary, asteroid, comet, space, science
@@ -19,89 +20,64 @@
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 packages = find:
 zip_save = False
-python_requires = >=3.7
+python_requires = >=3.8
 setup_requires = setuptools_scm
 install_requires = 
-	numpy>=1.17.0
-	astropy>=4.0
+	numpy>=1.18.0
+	astropy>=4.3
 	ads>=0.12
-	synphot>=1.0
+	synphot>=1.1.1
 	astroquery>=0.4.5
 include_package_data = True
 
 [options.extras_require]
 all = 
-	scipy
+	scipy>=1.3
 	ginga
 	photutils
 	pyyaml
 test = 
-	pytest>=4.6
+	pytest>=7.0
 	pytest-astropy
-	pytest-doctestplus
+	pytest-doctestplus>=0.10
 	pytest-remotedata
 	pytest-xdist
 	coverage
 docs = 
-	sphinx-astropy>=1.3
-	pytest
-	matplotlib>=3.0
+	pytest>=7.0
+	matplotlib>=3.1
+	sphinx-astropy>=1.3,!=1.9.0
 
 [options.package_data]
 * = *.fits *.csv *.txt
 
 [options.entry_points]
 ginga.rv.plugins = 
 	cometaryenhancements = sbpy.ginga_plugins:setup_cometaryenhancements
 
 [tool:pytest]
-minversion = 4.6
+minversion = 7.0
 testpaths = "sbpy" "docs"
 norecursedirs = 
 	"docs[\/]_build"
 	"docs[\/]generated"
 astropy_header = true
 doctest_plus = enabled
 text_file_format = rst
-addopts = --doctest-rst --doctest-plus --ignore=compile_fieldnames.py
 remote_data_strict = true
+addopts = --doctest-rst --ignore=compile_fieldnames.py --color=yes
+xfail_strict = true
 doctest_norecursedirs = 
 	*/setup_package.py
-
-[coverage:run]
-omit = 
-	sbpy/_astropy_init*
-	sbpy/conftest.py
-	sbpy/*setup_package*
-	sbpy/tests/*
-	sbpy/*/tests/*
-	sbpy/*/*/tests/*
-	sbpy/extern/*
-	sbpy/version*
-	*/sbpy/_astropy_init*
-	*/sbpy/conftest.py
-	*/sbpy/*setup_package*
-	*/sbpy/tests/*
-	*/sbpy/*/tests/*
-	*/sbpy/*/*/tests/*
-	*/sbpy/extern/*
-	*/sbpy/version*
-
-[coverage:report]
-exclude_lines = 
-	pragma: no cover
-	except ImportError
-	raise AssertionError
-	raise NotImplementedError
-	def main\(.*\):
-	pragma: py{ignore_python_version}
-	def _ipython_key_completions_
+filterwarnings = 
+	ignore:numpy\.ufunc size changed:RuntimeWarning
+	ignore:numpy\.ndarray size changed:RuntimeWarning
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sbpy-0.3.0/setup.py` & `sbpy-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/tox.ini` & `sbpy-0.4.0/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 [tox]
 envlist =
-    py{37,38,39,dev}-test{,-alldeps,-oldestdeps,-devdeps,-numpy117,-numpy118,-numpy119}{,-cov}
+    py{38,39,310,311,dev}-test{,-alldeps,-oldestdeps,-devdeps,-numpy118,-numpy119,-numpy120,-numpy121,-numpy122,-numpy123}{,-cov}
     build_docs
     linkcheck
     codestyle
 requires =
     setuptools >= 30.3.0
     pip >= 19.3.1
     tox-pypi-filter >= 0.12
 isolated_build = true
 
 [testenv]
 
-# The following option combined with the use of the tox-pypi-filter above allows
-# project-wide pinning of dependencies, e.g. if new versions of pytest do not
-# work correctly with pytest-astropy plugins. Most of the time the pinnings file
-# should be empty.
-pypi_filter = https://raw.githubusercontent.com/astropy/ci-helpers/master/pip_pinnings.txt
-
 # Pass through the following environemnt variables which are needed for the CI
-passenv = HOME WINDIR LC_ALL LC_CTYPE CC CI TEST_READ_HUGE_FILE FC_GFORTRAN
+passenv = HOME,WINDIR,LC_ALL,LC_CTYPE,CC,CI,TEST_READ_HUGE_FILE,FC_GFORTRAN,ADS_DEV_KEY
 
 # For coverage, we need to pass extra options to the C compiler
 setenv =
     cov: CFLAGS = --coverage -fno-inline-functions -O0
     image: MPLFLAGS = --mpl
     !image: MPLFLAGS =
 
@@ -41,60 +35,63 @@
 #
 description =
     run tests
     alldeps: with all optional dependencies
     devdeps: with the latest developer version of key dependencies
     oldestdeps: with the oldest supported version of key dependencies
     cov: and test coverage
-    numpy117: with numpy 1.17.*
     numpy118: with numpy 1.18.*
-    numpy119: with numpy 1.18.*
+    numpy119: with numpy 1.19.*
+    numpy120: with numpy 1.20.*
+    numpy121: with numpy 1.21.*
+    numpy122: with numpy 1.22.*
+    numpy123: with numpy 1.23.*
     image: with image tests
     mpldev: with the latest developer version of matplotlib
     double: twice in a row to check for global state changes
 
 deps =
-    # avoid pickling error with astropy 5 + astroquery 0.4.5; remove when astroquery 0.4.6 is released
-    test: git+https://github.com/astropy/astroquery.git#egg=astroquery
-
-    numpy117: numpy==1.17.*
     numpy118: numpy==1.18.*
     numpy119: numpy==1.19.*
+    numpy120: numpy==1.20.*
+    numpy121: numpy==1.21.*
+    numpy122: numpy==1.22.*
+    numpy123: numpy==1.23.*
 
     image: pytest-mpl
 
-    # pytest-openfiles pinned because of https://github.com/astropy/astropy/issues/10160 (takes too long)
-    alldeps: pytest-openfiles==0.4.0
-    alldeps: git+https://github.com/mkelley/pyoorb-experiment.git@sbpy-testing#egg=pyoorb
+    alldeps,oldestdeps,devdeps: git+https://github.com/mkelley/pyoorb-experiment.git@sbpy-testing#egg=pyoorb
 
     # The oldestdeps factor is intended to be used to install the oldest versions of all
     # dependencies that have a minimum version.
-    oldestdeps: numpy==1.17.*
-    oldestdeps: matplotlib==3.0.*
+    oldestdeps: numpy==1.18.*
+    oldestdeps: matplotlib==3.1.*
     oldestdeps: scipy==1.3.*
-    oldestdeps: synphot==1.0.*
-    oldestdeps: astropy==4.0.*
+    oldestdeps: synphot==1.1.*
+    oldestdeps: astropy==4.3.*
     oldestdeps: ads==0.12.*
 
     # The devdeps factor is intended to be used to install the latest developer version
     # of key dependencies.
-    devdeps: git+https://github.com/numpy/numpy.git#egg=numpy
+    devdeps: numpy>=0.0.dev0
+    devdeps: scipy>=0.0.dev0
     devdeps: git+https://github.com/astropy/astropy.git#egg=astropy
     devdeps: git+https://github.com/astropy/astroquery.git#egg=astroquery
-    devdeps,mpldev: git+https://github.com/matplotlib/matplotlib.git#egg=matplotlib
+    devdeps,mpldev: matplotlib>=0.0.dev0
 
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
-    test
+    test: test
     alldeps: all
 
 commands =
     pip freeze
     !cov: pytest --pyargs sbpy {toxinidir}/docs {env:MPLFLAGS} {posargs}
     cov: pytest --pyargs sbpy  {env:MPLFLAGS} --cov sbpy --cov-config={toxinidir}/setup.cfg {posargs}
+    cov: coverage xml -o {toxinidir}/coverage.xml
 
 [testenv:build_docs]
 changedir = docs
 description = invoke sphinx-build to build the HTML docs
 extras = docs
 commands =
     pip freeze
```

### Comparing `sbpy-0.3.0/website/public/css/style.css` & `sbpy-0.4.0/website/public/css/style.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,643 +1,745 @@
 /* https://meyerweb.com/eric/tools/css/reset/
    v2.0 | 20110126
    License: none (public domain)
 */
 
-html, body, div, span, applet, object, iframe,
-h1, h2, h3, h4, h5, h6, p, blockquote, pre,
-a, abbr, acronym, address, big, cite, code,
-del, dfn, em, img, ins, kbd, q, s, samp,
-small, strike, strong, tt, var,
-b, u, i, center,
-dl, dt, dd, ol, ul, li,
-fieldset, form, label, legend,
-table, caption, tbody, tfoot, thead, tr, th, td,
-article, aside, canvas, details, embed,
-figure, figcaption, footer, header, hgroup,
-menu, nav, output, ruby, section, summary,
-time, mark, audio, video {
+html,
+body,
+div,
+span,
+applet,
+object,
+iframe,
+h1,
+h2,
+h3,
+h4,
+h5,
+h6,
+p,
+blockquote,
+pre,
+a,
+abbr,
+acronym,
+address,
+big,
+cite,
+code,
+del,
+dfn,
+em,
+img,
+ins,
+kbd,
+q,
+s,
+samp,
+small,
+strike,
+strong,
+tt,
+var,
+b,
+u,
+i,
+center,
+dl,
+dt,
+dd,
+ol,
+ul,
+li,
+fieldset,
+form,
+label,
+legend,
+table,
+caption,
+tbody,
+tfoot,
+thead,
+tr,
+th,
+td,
+article,
+aside,
+canvas,
+details,
+embed,
+figure,
+figcaption,
+footer,
+header,
+hgroup,
+menu,
+nav,
+output,
+ruby,
+section,
+summary,
+time,
+mark,
+audio,
+video {
 	margin: 0;
 	padding: 0;
 	border: 0;
 	font-size: 100%;
 	font: inherit;
 	vertical-align: baseline;
 }
 
 /* HTML5 display-role reset for older browsers */
-article, aside, details, figcaption, figure,
-footer, header, hgroup, menu, nav, section {
+article,
+aside,
+details,
+figcaption,
+figure,
+footer,
+header,
+hgroup,
+menu,
+nav,
+section {
 	display: block;
 }
+
 .footer {
 	color: black;
 	background-color: #f5f5f5;
 	position: relative;
 }
+
 .footer-text {
-        width: 100%;
+	width: 100%;
 	text-align: center;
 	padding: 12px 12px;
 }
+
 .footer-text a:hover {
 	color: #FF851B;
 }
+
 .footer-stamp {
 	position: absolute;
 	top: 20px;
 	right: 10px;
 }
+
 @media (max-width: 710px) {
-  .footer-text {
-	width: 40%;
-	padding: 12px 6px;
-  }
+	.footer-text {
+		width: 40%;
+		padding: 12px 6px;
+	}
 }
+
 @media (max-width: 593px) {
-  .footer-text {
-	width: 90%;
-	padding: 12px 12px;
-  }
-  .footer-stamp {
-	position: static;
-	margin: 13px;
-  }
+	.footer-text {
+		width: 90%;
+		padding: 12px 12px;
+	}
+
+	.footer-stamp {
+		position: static;
+		margin: 13px;
+	}
 }
+
 body {
 	line-height: 1;
 }
-ol, ul {
+
+ol,
+ul {
 	list-style: none;
 }
-blockquote, q {
+
+blockquote,
+q {
 	quotes: none;
 }
-blockquote:before, blockquote:after,
-q:before, q:after {
+
+blockquote:before,
+blockquote:after,
+q:before,
+q:after {
 	content: '';
 	content: none;
 }
+
 table {
 	border-collapse: collapse;
 	border-spacing: 0;
 }
 
-body{
+body {
 	line-height: 1.25em;
 	font-size: 14px;
-	color:#333;
+	color: #333;
 	font-family: 'Open Sans', sans-serif;
 }
 
 code {
 	font-family: monospace;
 }
 
 #index {
-        background-color:#F5F5F5;
+	/* background-color: #F5F5F5; */
 }
 
-#wrapper{
-	margin:0 auto;
-	max-width:960px;
-	padding:0 10px;
-	min-width: 320px; /* min-width of whole site */
+#wrapper {
+	margin: 0 auto;
+	max-width: 960px;
+	padding: 0 10px;
+	min-width: 320px;
+	/* min-width of whole site */
 }
 
-a{
+a {
 	color: #FF5000;
 	text-decoration: none;
 }
-a, svg{
+
+a,
+svg {
 	-webkit-transition: all 0.3s ease;
 	-moz-transition: all 0.3s ease;
 	-o-transition: all 0.3s ease;
 	-ms-transition: all 0.3s ease;
 	transition: all 0.3s ease;
 }
 
-a:hover{
-	color:#333;
+a:hover {
+	color: #333;
 }
 
-h1{
+h1 {
 	font-size: 24px;
 	margin-top: 10px;
 	margin-bottom: 20px;
 }
 
-h2{
+h2 {
 	font-size: 20px;
 	margin-bottom: 10px;
 }
 
-h3{
+h3 {
 	font-size: 16px;
 	margin: 20px 0px 10px 0px;
 
 }
 
-p{
+p {
 	margin-bottom: 10px;
 	margin-top: 10px;
 	line-height: 1.5em;
 }
 
-strong{
+strong {
 	font-weight: bold;
 
 }
 
-section{
+section {
 	border-bottom: 1px #efefef solid;
 	padding: 30px 0 30px;
 	clear: both;
 }
 
-section:first-of-type{
-	margin-top:42px;
+section:first-of-type {
+	margin-top: 42px;
 }
 
-section:last-of-type{
+section:last-of-type {
 	border-bottom: 0px;
 }
 
-section *:last-child{
+section *:last-child {
 	margin-bottom: 0px;
 }
 
-ul li{
+ul li {
 	list-style-type: square;
 	list-style-position: outside;
-	list-style-color:  #FF5000;
+	list-style-color: #FF5000;
 	line-height: 1.5em;
-	margin-bottom:0.5em;
+	margin-bottom: 0.5em;
 	margin-left: 30px;
 }
 
-ul li:last-child{
+ul li:last-child {
 	margin-bottom: 0px;
 }
 
-cite{
+cite {
 	font-family: monospace;
 }
 
-code{
-	/* background-color: #f5f5f5; */
-	/* border: 1px solid #ddd; */
-	/* padding: 5px; */
-        margin-left: 20px;
-        color: #999;
+pre {
+	background-color: #f5f5f5;
+	border: 1px solid #ccc;
+	padding: 10px;
+	color: black;
 	font-family: Courier New, monospace;
-	/* webkit-border-radius: 3px; */
-	/* -moz-border-radius: 3px; */
-	/* border-radius: 3px; */
+	border-radius: 3px;
 	margin-bottom: 5px;
 }
 
-.button{
+.button {
 	padding: 8px;
 	display: inline-block;
-	background-image: -webkit-gradient(
-	linear,
-	left top,
-	left bottom,
-	color-stop(0, #FC9468),
-	color-stop(0.89, #FF5100)
-	);
+	background-image: -webkit-gradient(linear,
+			left top,
+			left bottom,
+			color-stop(0, #FC9468),
+			color-stop(0.89, #FF5100));
 	background-image: -o-linear-gradient(bottom, #FC9468 0%, #FF5100 89%);
 	background-image: -moz-linear-gradient(bottom, #FC9468 0%, #FF5100 89%);
 	background-image: -webkit-linear-gradient(bottom, #FC9468 0%, #FF5100 89%);
 	background-image: -ms-linear-gradient(bottom, #FC9468 0%, #FF5100 89%);
 	background-image: linear-gradient(to bottom, #FC9468 0%, #FF5100 89%);
-        border-radius: 3px;
+	border-radius: 3px;
 }
 
-a.button, .button a{
+a.button,
+.button a {
 	color: white;
 }
 
 
-p .button{
-	padding-top:0px;
-	padding-bottom:0px;
-	padding-right:4px;
-	padding-left:4px;
+p .button {
+	padding-top: 0px;
+	padding-bottom: 0px;
+	padding-right: 4px;
+	padding-left: 4px;
 }
 
-.button:hover{
+.button:hover {
 	cursor: pointer;
-	background-image: -webkit-gradient(
-		linear,
-		left top,
-		left bottom,
-		color-stop(0, #FFA47D),
-		color-stop(1, #FF7D45)
-	);
+	background-image: -webkit-gradient(linear,
+			left top,
+			left bottom,
+			color-stop(0, #FFA47D),
+			color-stop(1, #FF7D45));
 	background-image: -o-linear-gradient(bottom, #FFA47D 0%, #FF7D45 100%);
 	background-image: -moz-linear-gradient(bottom, #FFA47D 0%, #FF7D45 100%);
 	background-image: -webkit-linear-gradient(bottom, #FFA47D 0%, #FF7D45 100%);
 	background-image: -ms-linear-gradient(bottom, #FFA47D 0%, #FF7D45 100%);
 	background-image: linear-gradient(to bottom, #FFA47D 0%, #FF7D45 100%);
 }
 
 hr {
-    border: none;
-    height: 1px;
-    /* Set the hr color */
-    color: #333; /* old IE */
-    background-color: grey; /* Modern Browsers */
+	border: none;
+	height: 1px;
+	/* Set the hr color */
+	color: #333;
+	/* old IE */
+	background-color: grey;
+	/* Modern Browsers */
 }
 
-.right{
+.right {
 	float: right;
 }
 
 /* nav */
-nav{
+nav {
 	line-height: 42px;
-	position:absolute;
-	left:0px;
-	top:0px;
-	width:100%;
-	background-image: -webkit-gradient(linear,left top,left bottom,color-stop(0, #222222),color-stop(0.89, #333333));
+	position: absolute;
+	left: 0px;
+	top: 0px;
+	width: 100%;
+	background-image: -webkit-gradient(linear, left top, left bottom, color-stop(0, #222222), color-stop(0.89, #333333));
 	background-image: -o-linear-gradient(bottom, #222222 0%, #333333 89%);
 	background-image: -moz-linear-gradient(bottom, #222222 0%, #333333 89%);
 	background-image: -webkit-linear-gradient(bottom, #222222 0%, #333333 89%);
 	background-image: -ms-linear-gradient(bottom, #222222 0%, #333333 89%);
 	background-image: linear-gradient(to bottom, #222222 0%, #333333 89%);
 }
 
-nav > *{
-	display:inline-block;
-	vertical-align:top;
+nav>* {
+	display: inline-block;
+	vertical-align: top;
 }
 
-nav img{
+nav img {
 	float: left;
 	margin-left: 20px;
 	margin-top: 5px;
 }
 
-nav ul{
-	max-width:960px;
-	margin:0 auto;
+nav ul {
+	max-width: 960px;
+	margin: 0 auto;
 }
 
-nav ul li{
-	display:inline;
+nav ul li {
+	display: inline;
 	list-style: none;
 	margin: 10px;
 }
 
 
-nav li a, nav li a:link{
-	color:white;
+nav li a,
+nav li a:link {
+	color: white;
 }
-nav li a:hover{
-	color:#FF5000;
+
+nav li a:hover {
+	color: #FF5000;
 }
 
-nav li a.active{
-	color:#FF5000;
+nav li a.active {
+	color: #FF5000;
 }
 
-nav .pull-right{
+nav .pull-right {
 	float: right;
-	margin-right:10px;
+	margin-right: 10px;
 }
 
-.search input{
+.search input {
 	margin-top: 4px;
 	width: 180px;
 	height: 18px;
 	border: 1px solid #ccc;
 	-webkit-border-radius: 3px;
 	-moz-border-radius: 3px;
 	border-radius: 3px;
 	background-color: #ffffff;
 	font-size: 13px;
 	line-height: 18px;
 	padding-left: 5px;
 }
 
 #mobile-header {
-    display: none;
+	display: none;
 }
 
-@media only screen and (max-width: 370px){
-	.search{
+@media only screen and (max-width: 370px) {
+	.search {
 		display: none;
 	}
 }
 
 
 /*hero*/
 
-section#hero{
+section#hero {
 	text-align: center;
-	position:absolute;
-	left:0px;
-	top:0;
-	width:100%;
-        border-bottom: 10px;
+	position: absolute;
+	left: 0px;
+	top: 0;
+	width: 100%;
+	border-bottom: 10px;
+	z-index: -1;
 }
 
-section#hero p{
+section#hero p {
 	max-width: 600px;
 	margin: 10px auto 20px auto;
 
 }
 
-section#hero img{
+section#hero img {
 	display: inline;
-	margin:20px 0px;
-	max-width:90%;
+	margin: 20px 0px;
+	max-width: 90%;
 }
 
-section#hero div#documentation{
-	color:white;
+section#hero div#documentation {
+	color: white;
 	display: inline-block;
 	position: relative;
 }
 
-section#hero div#documentation span{
+section#hero div#documentation span {
 	font-size: 10px;
-	padding:10px 20px 6px 20px;
+	padding: 10px 20px 6px 20px;
 }
 
-section#hero div#documentation a{
+section#hero div#documentation a {
 	color: white;
-	text-align:center;
+	text-align: center;
 }
 
-section#hero div#documentation ul{
+section#hero div#documentation ul {
 	border-top: white 2px solid;
 	text-align: left;
 	position: absolute;
-	left: 179px; top: 33px;
+	left: 179px;
+	top: 33px;
 	display: none;
 	background-color: #FF5000;
 	width: 107px;
 	font-size: 12px;
-	z-index:1;
+	z-index: 1;
 }
 
-section#hero div#documentation ul li{
+section#hero div#documentation ul li {
 	border-top: white 1px solid;
 	padding: 5px 5px;
 	list-style: none;
 	margin: 0px;
 }
-section#hero div#documentation ul li:hover{
+
+section#hero div#documentation ul li:hover {
 	background-color: #ffa077;
 	cursor: pointer;
 }
 
 section#hero div#documentation ul li a {
-  display: block;
-  text-decoration: none;
+	display: block;
+	text-decoration: none;
 }
 
 /*Front Page*/
 
-section.whatsnew{
-	margin-top:350px;
-	border:1px #E8E8E8 solid;
-	border-right-style:none;
-	border-left-style:none;
-	border-padding=1px;
+section.whatsnew {
+	margin-top: 350px;
+	border: 1px #E8E8E8 solid;
+	border-right-style: none;
+	border-left-style: none;
+	border-spacing: 1px;
 	padding-top: 15px;
 	padding-bottom: 15px;
 }
 
-section.whatsnew .version{
-	color:grey;
+section.whatsnew .version {
+	color: grey;
 	font-size: 12px;
-	margin-top:6px;
-	margin-bottom:0px;
+	margin-top: 6px;
+	margin-bottom: 0px;
 }
 
-.whatsnew{
+.whatsnew {
 	font-size: 24px;
 	text-align: center;
 }
 
 /*Installation Instructions*/
 
 /*section.install{
 	margin-top:380px;
 }*/
 
 /*section.install div{
 	margin-top: 30px;
 }*/
 
-section.install .button.download{
+section.install .button.download {
 	padding: 5px 5px;
 }
 
-section.install ul li{
+section.install ul li {
 	list-style: none;
 	margin-left: 0px;
 }
 
-section.install ul li a{
-        background: #fff;
+section.install ul li a {
+	background: #fff;
 	border: 1px #FFE1D6 solid;
 	padding: 10px;
 	float: left;
 	margin: 0px 5px -1px 5px;
-	height:20px;
+	height: 20px;
 	line-height: 20px;
-        border-radius: 3px 3px 0px 0px;
+	border-radius: 3px 3px 0px 0px;
 }
-section.install ul li a.right{
+
+section.install ul li a.right {
 	float: right;
 }
 
 
 /* Make tweaks here to accomodate additional tabs */
 @media all and (max-width: 630px) {
-	section.install ul li a{
-		padding:10px 2px;
-		font-size:12px;
+	section.install ul li a {
+		padding: 10px 2px;
+		font-size: 12px;
 	}
 }
 
 @media all and (max-width: 420px) {
 
-	section.install ul li a{
+	section.install ul li a {
 		padding: 10px 15px;
 	}
 
-	section.install ul li a span{
+	section.install ul li a span {
 		display: none;
 	}
 }
+
 /* end changes */
 
 
-section.install ul li:first-child a{
+section.install ul li:first-child a {
 	margin-left: 0px;
 }
 
-section.install div h3{
+section.install div h3 {
 	color: black;
 	margin-top: 0px;
 }
 
 
 
 
 /*Affiliated*/
 
-.featured{
-	background-color:#fdfdfd;
+.featured {
+	background-color: #fdfdfd;
 }
 
-.featured div{
+.featured div {
 	clear: both;
 	padding: 20px 0px;
 }
 
-.featured div:first-of-type{
+.featured div:first-of-type {
 	padding-top: 5px;
 }
 
-.featured div h3{
-	color:black;
+.featured div h3 {
+	color: black;
 	margin-bottom: 10px;
 	padding-bottom: 10px;
 	border-bottom: 1px solid #FFE1D6;
 }
 
-.featured img{
-	float: left+;
-	margin-right:10px;
+.featured img {
+	float: left;
+	margin-right: 10px;
 }
 
-table{
+table {
 	margin: 20px 0px;
-	word-break:overflow-wrap;
+	word-break: overflow-wrap;
 }
 
 
 
-thead{
+thead {
 	text-align: left;
 	font-weight: bold;
-	border-bottom: 1px solid rgba(128,128,128,0.2);
+	border-bottom: 1px solid rgba(128, 128, 128, 0.2);
 }
 
 
 
-td{
-	padding:12px 5px;
+td {
+	padding: 12px 5px;
 	font-size: 100%;
 	line-height: 1.3em;
 }
 
 
 td:first-child {
-    font-weight: bold;
-  }
+	font-weight: bold;
+}
 
 /* Create gray border after every 3rd row to visually separate packages */
 table tr.border-top {
-    border-top: 1px solid rgba(128,128,128,0.2);
+	border-top: 1px solid rgba(128, 128, 128, 0.2);
 }
 
 
 /* About */
 
-p.citation{
+p.citation {
 	margin: 10px 40px;
 }
 
-ul.team{
-	-moz-column-count:5; /* Firefox */
-	-webkit-column-count:5; /* Safari and Chrome */
-	column-count:5;
+ul.team {
+	-moz-column-count: 5;
+	/* Firefox */
+	-webkit-column-count: 5;
+	/* Safari and Chrome */
+	column-count: 5;
 }
 
-@media only screen and (max-width: 920px){
-	ul.team{
-		-moz-column-count:2; /* Firefox */
-		-webkit-column-count:2; /* Safari and Chrome */
-		column-count:2;
+@media only screen and (max-width: 920px) {
+	ul.team {
+		-moz-column-count: 2;
+		/* Firefox */
+		-webkit-column-count: 2;
+		/* Safari and Chrome */
+		column-count: 2;
 	}
 }
 
-ul.team li, ul.coordinators li{
-	margin-bottom:0px;
+ul.team li,
+ul.coordinators li {
+	margin-bottom: 0px;
 }
 
 p.centered {
 	text-align: center
 }
 
 .center {
-    text-align: center;
-    color: red;
+	text-align: center;
+	color: red;
 }
 
 .dropdown {
-    position: relative;
-    display: inline-block;
+	position: relative;
+	display: inline-block;
 }
 
 .dropdown-content {
-    display: none;
-    position: absolute;
-    background-color: DimGray;
-    min-width: 160px;
-    width: 100%;
-    height: 100%
-    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
-    padding: 0px 16px;
-    z-index: 1;
+	display: none;
+	position: absolute;
+	background-color: DimGray;
+	min-width: 160px;
+	width: 100%;
+	height: 100%;
+	box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
+	padding: 0px 16px;
+	z-index: 1;
 }
 
 .dropdown:hover .dropdown-content {
-    display: block;
+	display: block;
 }
 
 .dropdown-content a {
-display: block;
+	display: block;
 }
 
 .dropdown-content a:hover {
-color: white;
+	color: white;
 }
 
 .dropdown a:hover {
-color: #FF5000;
+	color: #FF5000;
 }
 
 .dropdown z:hover {
-color: #FF5000;
-width: 10;
-display: none;
+	color: #FF5000;
+	width: 10;
+	display: none;
 }
 
 .dropdown z {
-color: white;
+	color: white;
 }
 
 .dropdown:after {
-    content: "";
-    position: absolute;
-    right: -13px;
-    top: 9px;
-    width: 0;
-    height: 0;
-    border-left: 5px solid transparent;
-    border-right: 5px solid transparent;
-    border-top: 5px solid white;
+	content: "";
+	position: absolute;
+	right: -13px;
+	top: 9px;
+	width: 0;
+	height: 0;
+	border-left: 5px solid transparent;
+	border-right: 5px solid transparent;
+	border-top: 5px solid white;
 }
 
 #roles-table td {
 	padding: 7px 5px;
-}
+}
```

### Comparing `sbpy-0.3.0/website/public/images/NASA_logo.svg` & `sbpy-0.4.0/website/public/images/NASA_logo.svg`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/website/public/images/sbpy_logo_full.png` & `sbpy-0.4.0/website/public/images/sbpy_logo_full.png`

 * *Files identical despite different names*

### Comparing `sbpy-0.3.0/website/public/index.html` & `sbpy-0.4.0/website/public/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -20,26 +20,17 @@
   <div id="wrapper">
     <nav>
       <div id="navigation">
         <ul>
           <li>
             <a href="index.html"><strong>sbpy</strong></a>
           </li>
-          <li>
-            <div class="dropdown">
-              <a>About</a>
-              <div class="dropdown-content">
-                <ul>
-                  <li><a href="https://sbpy.readthedocs.io/en/latest/about.html">About sbpy</a></li>
-                  <li><a href="https://astropy.org">Aboout Astropy</a></li>
-                </ul>
-              </div>
-            </div>
-          </li>
+          <li><a href="https://sbpy.readthedocs.io/en/latest/about.html">About</a></li>
           <li><a href="https://sbpy.readthedocs.io/en/latest/index.html">Documentation</a></li>
+          <li><a href="https://github.com/NASA-Planetary-Science/sbpy/discussions">Help</a></li>
           <li><a href="https://github.com/NASA-Planetary-Science/sbpy-tutorial">Tutorials</a></li>
           <li><a href="https://sbpy.readthedocs.io/en/latest/development/index.html">Contributing</a></li>
           <li><a href="https://github.com/NASA-Planetary-Science/sbpy">GitHub</a></li>
 
           <li><a href="team.html">Team</a></li>
         </ul>
       </div>
@@ -65,47 +56,71 @@
           src="https://github.com/NASA-Planetary-Science/sbpy/workflows/CI/badge.svg" /></a>
       <a class="reference external image-reference" href="https://sbpy.readthedocs.io/en/latest/?badge=latest">
         <img alt="Documentation Status" src="https://readthedocs.org/projects/sbpy/badge/?version=latest" /></a>
       <a class="reference external image-reference"
         href="https://joss.theoj.org/papers/8b8e7bb15fb4a14f80f2afd06b6ce060#">
         <img alt="JOSS Publication" src="https://joss.theoj.org/papers/10.21105/joss.01426/status.svg"></a>
       <a class="reference external image-reference" href="https://codecov.io/gh/NASA-Planetary-Science/sbpy">
-        <img src="https://codecov.io/gh/NASA-Planetary-Science/sbpy/branch/master/graph/badge.svg">
+        <img src="https://codecov.io/gh/NASA-Planetary-Science/sbpy/branch/main/graph/badge.svg">
       </a>
 
-      <p class="version">Current Version: 0.1.1</p>
+      <p class="version">Current Version: 0.3</p>
 
     </section>
 
     <section class="install">
       <h1>Installation</h1>
-      <p>We recommend
-        installing <a href="https://www.anaconda.com/download/">Anaconda
-          Python 3</a> before installing sbpy using:
-      <p><code>pip install git+https://github.com/NASA-Planetary-Science/sbpy.git</code></p>
+      <p>sbpy is a Python package, installable with pip:</p>
+      <p>
+      <pre>pip install sbpy</pre>
+      </p>
+      <p>Or with <a href="https://www.anaconda.com/">Anaconda</a> via the <a
+          href="https://conda-forge.org/">conda-forge</a> channel</a>:
+      <p>
+      <pre>conda install sbpy --channel=conda-forge</pre>
+      </p>
       <a class="button" href="https://sbpy.readthedocs.io/en/latest/install.html" target="_blank">Detailed Installation
         Instructions</a>
     </section>
 
     <section class="whatsnext">
       <h1>Learn sbpy</h1>
       <p>Explore sbpy using tutorial notebooks that showcase its functionality using real-life science applications or
         browse its documentation.</p>
       <a class="button" href="https://github.com/NASA-Planetary-Science/sbpy-tutorial" target="_blank">Tutorial
         Notebooks</a>
       <a class="button" href="https://sbpy.readthedocs.io/en/latest/" target="_blank">Documentation</a>
     </section>
 
     <section class="whatsnext">
-      <h1>Report bugs and Contribute</h1>
-      <p>Please report what you believe is a bug or a mistake using the github issue tracker. If you have an idea for
-        how to improve sbpy, or would like to contribute code directly, please check out the contribution guidelines.
+      <h1>Get help</h1>
+      <p>Questions about sbpy or how to use sbpy modules can be posted at <a
+          href="https://github.com/NASA-Planetary-Science/sbpy/discussions">sbpy
+          Discussions</a>, hosted on GitHub. Help about using astropy and affiliated
+        packages (including sbpy) can also be found on <a href="https://www.astropy.org/help.html">Astropy's help
+          page</a>. You can
+        also find sbpy developers on the Astropy slack workspace in the #sbpy
+        channel (see <a href="https://www.astropy.org/help.html">Astropy's help
+          page</a> for connection details).
+      </p>
+      <a class="button" href="https://github.com/NASA-Planetary-Science/sbpy/discussions" target="_blank">sbpy
+        Discussions</a>
+      <a class="button" href="https://www.astropy.org/help.html" target="_blank">Astropy help</a>
+    </section>
+
+    <section class="whatsnext">
+      <h1>Report bugs and contribute</h1>
+      <p>Please report what you believe is a bug or a mistake using <a
+          href="https://github.com/NASA-Planetary-Science/sbpy/issues">sbpy's issue
+          tracker</a>. If you have an idea for how to improve sbpy, or would like to
+        contribute code directly, please check out the <a
+          href="https://sbpy.readthedocs.io/en/latest/development/">contribution guidelines</a>.
       </p>
       <a class="button" href="https://github.com/NASA-Planetary-Science/sbpy/issues" target="_blank">Report issues</a>
-      <a class="button" href="https://sbpy.readthedocs.io/en/latest/development/index.html" target="_blank">Contribution
+      <a class="button" href="https://sbpy.readthedocs.io/en/latest/development/" target="_blank">Contribution
         Guidelines</a>
     </section>
 
     <section class="whatsnext">
       <h1>Acknowledge sbpy</h1>
       <p>If you use sbpy in your work, we would appreciate if you could acknowledge its use by citing</p>
       <p><code>Mommert, Kelley, de Val-Borro, Li et al. (2019), Journal of Open Source Software, 4(38), 1426</code></p>
@@ -121,15 +136,15 @@
           the <a href="https://www.astropy.org/code_of_conduct.html">Astropy
             Code of Conduct</a>.</p>
         <p>
         <figure style="display: inline-block; vertical-align: middle">
           <img src="images/NASA_logo.svg" height="40px">
           <figcaption>Partner</figcaption>
         </figure>
-        sbpy is supported by NASA PDART Grant No. 80NSSC18K0987.</p>
+        sbpy support provided by NASA PDART Grant Nos. 80NSSC18K0987, 80NSSC22K0143.</p>
       </div>
     </div>
   </div>
 
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -2,45 +2,54 @@
 
 
 
 
 
     * sbpy
     * About
-          o About_sbpy
-          o Aboout_Astropy
     * Documentation
+    * Help
     * Tutorials
     * Contributing
     * GitHub
     * Team
 [q                   ]
   [sbpy - A Python Module for Small-Body Planetary Astronomy]
 sbpy is an Astropy affiliated package for asteroid and comet researchers.
 [GitHub_testing_status] [Documentation_Status] [JOSS_Publication] [https://
-codecov.io/gh/NASA-Planetary-Science/sbpy/branch/master/graph/badge.svg]
-Current Version: 0.1.1
+codecov.io/gh/NASA-Planetary-Science/sbpy/branch/main/graph/badge.svg]
+Current Version: 0.3
 
 ****** Installation ******
-We recommend installing Anaconda_Python_3 before installing sbpy using:
-pip install git+https://github.com/NASA-Planetary-Science/sbpy.git
+sbpy is a Python package, installable with pip:
+pip install sbpy
+Or with Anaconda via the conda-forge channel
+:
+conda install sbpy --channel=conda-forge
 Detailed_Installation_Instructions
 ****** Learn sbpy ******
 Explore sbpy using tutorial notebooks that showcase its functionality using
 real-life science applications or browse its documentation.
 Tutorial_Notebooks Documentation
-****** Report bugs and Contribute ******
-Please report what you believe is a bug or a mistake using the github issue
+****** Get help ******
+Questions about sbpy or how to use sbpy modules can be posted at sbpy
+Discussions, hosted on GitHub. Help about using astropy and affiliated packages
+(including sbpy) can also be found on Astropy's_help_page. You can also find
+sbpy developers on the Astropy slack workspace in the #sbpy channel (see
+Astropy's_help_page for connection details).
+sbpy_Discussions Astropy_help
+****** Report bugs and contribute ******
+Please report what you believe is a bug or a mistake using sbpy's_issue
 tracker. If you have an idea for how to improve sbpy, or would like to
-contribute code directly, please check out the contribution guidelines.
+contribute code directly, please check out the contribution_guidelines.
 Report_issues Contribution_Guidelines
 ****** Acknowledge sbpy ******
 If you use sbpy in your work, we would appreciate if you could acknowledge its
 use by citing
 Mommert, Kelley, de Val-Borro, Li et al. (2019), Journal of Open Source
 Software, 4(38), 1426
 sbpy_JOSS_Publication
 ===============================================================================
 sbpy is an Astropy affiliated package and as such committed to the Astropy_Code
 of_Conduct.
- [images/NASA_logo.svg] Partner  sbpy is supported by NASA PDART Grant No.
-80NSSC18K0987.
+ [images/NASA_logo.svg] Partner  sbpy support provided by NASA PDART Grant Nos.
+80NSSC18K0987, 80NSSC22K0143.
```

