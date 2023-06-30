# Comparing `tmp/pdstools-3.1.8.tar.gz` & `tmp/pdstools-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdstools-3.1.8.tar", last modified: Mon May 15 13:40:59 2023, max compression
+gzip compressed data, was "pdstools-3.1.9.tar", last modified: Fri May 19 15:41:18 2023, max compression
```

## Comparing `pdstools-3.1.8.tar` & `pdstools-3.1.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.787946 pdstools-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 13:40:47.000000 pdstools-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-15 13:40:59.787946 pdstools-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-15 13:40:47.000000 pdstools-3.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.779945 pdstools-3.1.8/pdstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-15 13:40:59.000000 pdstools-3.1.8/pdstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-15 13:40:59.000000 pdstools-3.1.8/pdstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:40:59.000000 pdstools-3.1.8/pdstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 13:40:59.000000 pdstools-3.1.8/pdstools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-15 13:40:59.000000 pdstools-3.1.8/pdstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 13:40:59.000000 pdstools-3.1.8/pdstools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-15 13:40:47.000000 pdstools-3.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.775946 pdstools-3.1.8/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.779945 pdstools-3.1.8/python/pdstools/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.779945 pdstools-3.1.8/python/pdstools/adm/
--rw-r--r--   0 runner    (1001) docker     (123)    56265 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/adm/ADMDatamart.py
--rw-r--r--   0 runner    (1001) docker     (123)    40060 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/adm/ADMTrees.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/adm/Tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.779945 pdstools-3.1.8/python/pdstools/app/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/app/Home.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/app/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.779945 pdstools-3.1.8/python/pdstools/app/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/app/pages/Health Check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.779945 pdstools-3.1.8/python/pdstools/ih/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/ih/IHAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/ih/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/ih/legacy_IH.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.783946 pdstools-3.1.8/python/pdstools/pega_io/
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/pega_io/API.py
--rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/pega_io/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/pega_io/S3.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/pega_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.783946 pdstools-3.1.8/python/pdstools/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/plots/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/plots/plots_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.783946 pdstools-3.1.8/python/pdstools/reports/
--rw-r--r--   0 runner    (1001) docker     (123)    39159 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/reports/HealthCheck.qmd
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/reports/HealthCheckModel.qmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.787946 pdstools-3.1.8/python/pdstools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/cdh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17946 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/hds_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/pega_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/polars_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/show_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/streamlit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/table_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.787946 pdstools-3.1.8/python/pdstools/valuefinder/
--rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/valuefinder/ValueFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/valuefinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:40:59.787946 pdstools-3.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.858224 pdstools-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 15:41:09.000000 pdstools-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-19 15:41:18.858224 pdstools-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-19 15:41:09.000000 pdstools-3.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/pdstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-19 15:41:18.000000 pdstools-3.1.9/pdstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-19 15:41:18.000000 pdstools-3.1.9/pdstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:41:18.000000 pdstools-3.1.9/pdstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 15:41:18.000000 pdstools-3.1.9/pdstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-19 15:41:18.000000 pdstools-3.1.9/pdstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 15:41:18.000000 pdstools-3.1.9/pdstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-19 15:41:09.000000 pdstools-3.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.850224 pdstools-3.1.9/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/adm/
+-rw-r--r--   0 runner    (1001) docker     (123)    56340 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/adm/ADMDatamart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40060 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/adm/ADMTrees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/adm/Tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/app/Home.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/app/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/app/pages/Health Check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/ih/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/ih/IHAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/ih/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/ih/legacy_IH.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/pega_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/pega_io/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/pega_io/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/pega_io/S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/pega_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50996 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/plots/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/plots/plots_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    40080 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/reports/HealthCheck.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/reports/HealthCheckModel.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.858224 pdstools-3.1.9/python/pdstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/cdh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/hds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/pega_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/polars_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/streamlit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/table_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.858224 pdstools-3.1.9/python/pdstools/valuefinder/
+-rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/valuefinder/ValueFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/valuefinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 15:41:18.858224 pdstools-3.1.9/setup.cfg
```

### Comparing `pdstools-3.1.8/LICENSE` & `pdstools-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/PKG-INFO` & `pdstools-3.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.8
+Version: 3.1.9
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.8 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.9 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.1.8/README.md` & `pdstools-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/pdstools.egg-info/PKG-INFO` & `pdstools-3.1.9/pdstools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.8
+Version: 3.1.9
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.8 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.9 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.1.8/pdstools.egg-info/SOURCES.txt` & `pdstools-3.1.9/pdstools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/pyproject.toml` & `pdstools-3.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -29,33 +29,34 @@
     "pds",
     "pdstools",
     "cdhtools",
     "datascientist",
     "tools",
 ]
 dependencies = [
-        "plotly>=5.5.0",
+        "pandas>=1.5.3",
+        "plotly>=5.14.1",
         "requests",
         "pydot",
-        "polars>=0.17.3",
+        "polars>=0.17.14",
         "pyarrow",
         "tqdm",
         "pyyaml",
         "aioboto3>=11.0"
     ]
 requires-python = ">=3.8"
 
 [tool.setuptools.dynamic]
 version = {attr="pdstools.__version__"}
 
 [project.optional-dependencies]
 docs = ['sphinx','furo','sphinx-autoapi','nbsphinx','sphinx-copybutton','myst-parser']
-app = ['streamlit>=1.20', 'quarto', 'papermill', 'itables', 'pandas>=1.5.3', 'jinja2>=3.1', 'xlsxwriter>=3.0']
+app = ['streamlit>=1.20', 'quarto', 'papermill', 'itables', 'jinja2>=3.1', 'xlsxwriter>=3.0']
 
 [project.urls]
 "Homepage" = "https://github.com/pegasystems/pega-datascientist-tools"
 "Bug Tracker" = "https://github.com/pegasystems/pega-datascientist-tools/issues"
 "Wiki" = "https://github.com/pegasystems/pega-datascientist-tools/wiki"
 "Docs" = "https://pegasystems.github.io/pega-datascientist-tools/"
 
 [project.scripts]
-pdstools = 'pdstools.app.cli:main'
+pdstools = 'pdstools.app.cli:main'
```

### Comparing `pdstools-3.1.8/python/pdstools/__init__.py` & `pdstools-3.1.9/python/pdstools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python pdstools"""
 
-__version__ = "3.1.8"
+__version__ = "3.1.9"
 
 from polars import enable_string_cache
 
 enable_string_cache(True)
 
 import sys
 from pathlib import Path
```

### Comparing `pdstools-3.1.8/python/pdstools/adm/ADMDatamart.py` & `pdstools-3.1.9/python/pdstools/adm/ADMDatamart.py`

 * *Files 0% similar despite different names*

```diff
@@ -1329,23 +1329,24 @@
 
         Returns
         -------
         str:
             The full path to the generated Health Check file.
         """
 
-        def delete_temp_files(working_dir, files):
+        def delete_temp_files(working_dir, files, del_log=True):
             temp_files = files + (
                 "params.yaml",
                 "HealthCheck.qmd",
                 "HealthCheck.ipynb",
                 "HealthCheckModel.qmd",
                 "HealthCheckModel.ipynb",
-                "log.txt",
             )
+            if del_log:
+                temp_files += tuple(["log.txt"])
             for f in temp_files:
                 try:
                     os.remove(f"{working_dir}/{f}")
                 except:
                     pass
 
         working_dir, output_location = Path(working_dir), Path(output_location)
@@ -1380,19 +1381,19 @@
         }
 
         with open(f"{working_dir}/params.yaml", "w") as f:
             yaml.dump(params, f)
 
         bashCommand = f"quarto render {healthcheck_file} --to {output_type} --output {output_filename} --execute-params params.yaml"
         if not verbose:
-            stdout, stderr = subprocess.DEVNULL, subprocess.STDOUT
+            stdout, stderr = subprocess.DEVNULL, None
         else:
             print("Set verbose=False to hide output.")
             print("Running:", bashCommand)
-            stdout, stderr = subprocess.PIPE, None
+            stdout, stderr = subprocess.PIPE, subprocess.STDOUT
         if kwargs.get("output_to_file", False):
             with open(f"{working_dir}/log.txt", "w") as outfile:
                 process = subprocess.Popen(
                     bashCommand.split(), stdout=outfile, stderr=stderr, cwd=working_dir
                 )
                 process.communicate()
 
@@ -1402,15 +1403,15 @@
             )
             process.communicate()
         if not os.path.exists(working_dir / output_filename):
             msg = "Error when generating healthcheck."
             if not verbose and not kwargs.get("output_to_file", False):
                 msg += "Set 'verbose' to True to see the full output"
             if delete_temp_files:
-                delete_temp_files(working_dir, files)
+                delete_temp_files(working_dir, files, del_log=False)
             raise ValueError(msg)
 
         filename = f"{output_location}/{output_filename}"
 
         if output_location != working_dir:
             if os.path.isfile(filename):
                 counter = 1
```

### Comparing `pdstools-3.1.8/python/pdstools/adm/ADMTrees.py` & `pdstools-3.1.9/python/pdstools/adm/ADMTrees.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/adm/Tables.py` & `pdstools-3.1.9/python/pdstools/adm/Tables.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/app/cli.py` & `pdstools-3.1.9/python/pdstools/app/cli.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/app/pages/Health Check.py` & `pdstools-3.1.9/python/pdstools/app/pages/Health Check.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from pathlib import Path
 
 import streamlit as st
+import traceback
 from pdstools.utils import streamlit_utils
 
 intro, imports, filters, report = st.tabs(
     [
         "Introduction",
         "Data import",
         "Data filters",
@@ -52,15 +53,15 @@
 
     opts = {}
     with st.expander("Configure advanced options"):
         col1, col2 = st.columns([4, 7])
         with col1:
             opts["extract_keys"] = st.checkbox(
                 "Extract additional keys",
-                False,
+                True,
                 help="""By default, ADM has a few "Context Keys" it uses to 
                 distinguish between models, such as Issue, Group, Channel, or Name. 
                 However, if you've setup custom context keys that are not part of a regular 
                 CDH setup, they are embedded in the "pyName" column. Setting this checkbox
                 tells us to try to extract these keys into separate columns.""",
             )
         with col2:
@@ -130,62 +131,80 @@
                         output_type=output_type,
                         working_dir=working_dir,
                         output_location=working_dir,
                         delete_temp_files=delete_temp_files,
                         include_tables=include_tables,
                         output_to_file=True,
                         modelData_only=st.session_state["modelhc"],
+                        verbose=True,
                     )
                 )
                 if os.path.isfile(outfile):
                     file = open(outfile, "rb")
+
+                st.session_state["run"][st.session_state["runID"]] = {
+                    "name": outfile,
+                    "file": file,
+                }
+
+                if not include_tables:
+                    tablename = Path(outfile).name.rsplit(".", 1)[0] + "_Tables.xlsx"
+                    tables = (
+                        st.session_state["dm"]
+                        .applyGlobalQuery(st.session_state["filters"])
+                        .exportTables(tablename)
+                    )
+                    st.session_state["run"][st.session_state["runID"]][
+                        "tables"
+                    ] = tablename
+                    st.session_state["run"][st.session_state["runID"]][
+                        "tablefile"
+                    ] = open(tables, "rb")
+
+                if len(st.session_state["run"][st.session_state["runID"]]) == 0:
+                    st.stop()
+
+                col1, col2 = st.columns([1, 1])
+                with col1:
+                    if "file" in st.session_state["run"][st.session_state["runID"]]:
+                        btn = st.download_button(
+                            label="Download Health Check",
+                            data=st.session_state["run"][st.session_state["runID"]][
+                                "file"
+                            ],
+                            file_name=Path(
+                                st.session_state["run"][st.session_state["runID"]][
+                                    "name"
+                                ]
+                            ).name,
+                        )
+                        if (
+                            "tables"
+                            in st.session_state["run"][st.session_state["runID"]]
+                        ):
+                            with col2:
+                                btn = st.download_button(
+                                    label="Download additional tables",
+                                    data=st.session_state["run"][
+                                        st.session_state["runID"]
+                                    ]["tablefile"],
+                                    file_name=st.session_state["run"][
+                                        st.session_state["runID"]
+                                    ]["tables"],
+                                )
+
             except Exception as e:
                 st.error(f"""Error occured when generating healthcheck: {e}""")
+                traceback_str = traceback.format_exc()
+                with open(working_dir / "log.txt", "a") as f:
+                    f.write(traceback_str)
                 with open(working_dir / "log.txt", "rb") as f:
                     btn = st.download_button(
                         label="Download error log",
                         data=f,
                         file_name="errorlog.txt",
                     )
-            st.session_state["run"][st.session_state["runID"]] = {
-                "name": outfile,
-                "file": file,
-            }
-
-            if not include_tables:
-                tablename = Path(outfile).name.rsplit(".", 1)[0] + "_Tables.xlsx"
-                tables = (
-                    st.session_state["dm"]
-                    .applyGlobalQuery(st.session_state["filters"])
-                    .exportTables(tablename)
-                )
-                st.session_state["run"][st.session_state["runID"]]["tables"] = tablename
-                st.session_state["run"][st.session_state["runID"]]["tablefile"] = open(
-                    tables, "rb"
-                )
-
-    print(st.session_state["run"])
-
-    if len(st.session_state["run"][st.session_state["runID"]]) == 0:
-        st.stop()
-
-    col1, col2 = st.columns([1, 1])
-    with col1:
-        if "file" in st.session_state["run"][st.session_state["runID"]]:
-            btn = st.download_button(
-                label="Download Health Check",
-                data=st.session_state["run"][st.session_state["runID"]]["file"],
-                file_name=Path(
-                    st.session_state["run"][st.session_state["runID"]]["name"]
-                ).name,
-            )
-            if "tables" in st.session_state["run"][st.session_state["runID"]]:
-                with col2:
-                    btn = st.download_button(
-                        label="Download additional tables",
-                        data=st.session_state["run"][st.session_state["runID"]][
-                            "tablefile"
-                        ],
-                        file_name=st.session_state["run"][st.session_state["runID"]][
-                            "tables"
-                        ],
-                    )
+                
+                for filename in os.listdir(working_dir):
+                    file_path = os.path.join(working_dir, filename)
+                    if os.path.isfile(file_path):
+                        os.remove(file_path)
```

### Comparing `pdstools-3.1.8/python/pdstools/ih/IHAnalysis.py` & `pdstools-3.1.9/python/pdstools/ih/IHAnalysis.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/ih/legacy_IH.py` & `pdstools-3.1.9/python/pdstools/ih/legacy_IH.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import pandas as pd
-import json
 import matplotlib.pyplot as plt
 import seaborn as sns
 import numpy as np
-from datetime import date, timedelta, datetime
+from datetime import timedelta
 import itertools
-import pytest
 
 
 def initial_prep(df, referenceTime="pxOutcomeTime"):
     for i in df.columns:
         if "time" in str(i).lower():
             df[i] = pd.to_datetime(df[i])
     df["Date"] = df[referenceTime].dt.strftime("%Y-%m-%d")
```

### Comparing `pdstools-3.1.8/python/pdstools/pega_io/API.py` & `pdstools-3.1.9/python/pdstools/pega_io/API.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/pega_io/File.py` & `pdstools-3.1.9/python/pdstools/pega_io/File.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/pega_io/S3.py` & `pdstools-3.1.9/python/pdstools/pega_io/S3.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/plots/plot_base.py` & `pdstools-3.1.9/python/pdstools/plots/plot_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Optional, Union, Dict, List, Any
-import pandas as pd
 import polars as pl
 from .plots_plotly import ADMVisualisations as plotly
 from ..utils.cdh_utils import (
     weighed_performance_polars,
     weighed_average_polars,
 )
 from ..utils.errors import NotApplicableError
```

### Comparing `pdstools-3.1.8/python/pdstools/plots/plots_plotly.py` & `pdstools-3.1.9/python/pdstools/plots/plots_plotly.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/reports/HealthCheck.qmd` & `pdstools-3.1.9/python/pdstools/reports/HealthCheck.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
    return display(Markdown(d))
 import sys
 sys.path.append('..')
 from pdstools import datasets, ADMDatamart
 from pdstools import cdh_utils
 from pdstools import defaultPredictorCategorization
 from plotly.offline import iplot
-from itables import show
+from itables import show, JavascriptFunction
 import plotly.express as px
 import plotly.graph_objs as go
 import polars as pl
 import pandas as pd
 import numpy as np
 from pdstools.utils import pega_template 
 import math
@@ -438,19 +438,42 @@
 - Predictors that consistently perform poorly could potentially be removed.
 - Be sure to check for data problems
 - Note we advise to be careful with predictor removal. Only remove if there is clearly no future value to other propositions as well or if there is always a related predictor that performs better.
 
 ```{python}
 # weighted performance
 if include_tables:
-    bad_predictors = datamart.bad_predictors.to_pandas(use_pyarrow_extension_array=False)
+    responses_column_index = datamart.bad_predictors.columns.index("Response Count")
+    bad_predictors = datamart.bad_predictors.to_pandas(
+        use_pyarrow_extension_array=False
+    )
+
+    show(
+        bad_predictors,
+        scrollX=True,
+        columnDefs=[
+            {
+                "className": "dt-left",
+                "targets": [responses_column_index],
+                "createdCell": JavascriptFunction(
+                    """
+function (td, cellData, rowData, row, col) {
+    if (cellData < 200) {
+        $(td).css('color', 'red')
+    }
+}
+"""
+                ),
+            }
+        ],
+    )
+
 
-    show(bad_predictors, scrollX=True)
 else:
-    print('Please refer to the `bad_predictors` tab in the included Excel file.')
+    print("Please refer to the `bad_predictors` tab in the included Excel file.")
 ```
 
 ## Number of Active and Inactive Predictors
 Showing the number of active and inactive predictors per model.
 
 ### Guidance
 - We expect a fewModels that have never been used
@@ -898,13 +921,30 @@
 # Appendix - all the models
 
 A list of all the models is written to a file so a script can iterate over all models and generate off-line model reports for each of them.
 
 Generally you will want to apply some filtering, or do this for specific models only. This can be accomplished in either this script here, or by editing the generated file.
 ```{python}
 if include_tables:
+    responses_column_index = datamart.appendix.columns.index("Responses")
     appendix = datamart.appendix.to_pandas(use_pyarrow_extension_array=True)
-    show(appendix)
+    show(
+        appendix,
+        columnDefs=[
+            {
+                "targets": [responses_column_index],
+                "createdCell": JavascriptFunction(
+                    """
+function (td, cellData, rowData, row, col) {
+    if (cellData < 200) {
+        $(td).css('color', 'red')
+    }
+}
+"""
+                ),
+            }
+        ],
+    )
 else:
-    print('Please refer to the `appendix` tab in the included Excel file.')
+    print("Please refer to the `appendix` tab in the included Excel file.")
 
 ```
```

### Comparing `pdstools-3.1.8/python/pdstools/reports/HealthCheckModel.qmd` & `pdstools-3.1.9/python/pdstools/reports/HealthCheckModel.qmd`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/utils/cdh_utils.py` & `pdstools-3.1.9/python/pdstools/utils/cdh_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/utils/datasets.py` & `pdstools-3.1.9/python/pdstools/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/utils/hds_utils.py` & `pdstools-3.1.9/python/pdstools/utils/hds_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         def sample_it(s: pl.Series) -> pl.Series:
             out = pl.Series(
                 values=np.random.binomial(
                     1, self.config.sample_percentage_schema_inferencing, s.len()
                 ),
                 dtype=pl.Boolean,
             )
-            if out.len() < 50:
+            if out.len() < 500:
                 out = pl.Series(values=[True] * out.len(), dtype=pl.Boolean)
             return out
 
         df_ = (
             df.lazy()
             .with_columns(pl.first().map(sample_it).alias("_sample"))
             .filter(pl.col("_sample"))
@@ -426,14 +426,18 @@
         column_mapping = {
             **predictors,
             **context_keys,
             **ih_predictors,
             **special_predictors,
             **outcome_column,
         }
+        if "filename" in symbolic_predictors_to_mask:
+            symbolic_predictors_to_mask.remove("filename")
+        if "filename" in column_mapping:
+            _ = column_mapping.pop("filename", None)
 
         return symbolic_predictors_to_mask, numeric_predictors_to_mask, column_mapping
 
     def getHasher(
         self,
         cols,
         algorithm="xxhash",
@@ -466,29 +470,31 @@
         """Anonymize the dataset."""
 
         def to_hash(cols, **kwargs):
             hasher = self.getHasher(cols, **kwargs)
             return (
                 pl.when(
                     (pl.col(cols).is_not_null())
-                    & (pl.col(cols) != "")
-                    & (pl.col(cols).is_in(["true", "false"]).is_not())
+                    & (pl.col(cols).cast(pl.Utf8) != pl.lit(""))
+                    & (pl.col(cols).cast(pl.Utf8).is_in(["true", "false"]).is_not())
                 )
                 .then(hasher)
                 .otherwise(pl.col(cols))
             )
 
         def to_normalize(cols):
             return (pl.col(cols) - pl.col(cols).min()) / (
                 pl.col(cols).max() - pl.col(cols).min()
             )
 
         def to_boolean(col, positives):
             return (
-                pl.when(pl.col(col).is_in(positives)).then(True).otherwise(False)
+                pl.when(pl.col(col).cast(pl.Utf8).is_in(positives))
+                .then(True)
+                .otherwise(False)
             ).alias(col)
 
         df = self.df.with_columns(
             pl.col(self.numeric_predictors_to_mask)
             .map_dict({"": None}, default=pl.first())
             .cast(pl.Float64)
         ).with_columns(
```

### Comparing `pdstools-3.1.8/python/pdstools/utils/pega_template.py` & `pdstools-3.1.9/python/pdstools/utils/pega_template.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/utils/polars_ext.py` & `pdstools-3.1.9/python/pdstools/utils/polars_ext.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/utils/show_versions.py` & `pdstools-3.1.9/python/pdstools/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/utils/streamlit_utils.py` & `pdstools-3.1.9/python/pdstools/utils/streamlit_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     you can import the data simply by pointing the app to the directory
     where the original files are located, and we can find it automatically."""
     )
     dir = st.text_input(
         "The folder of the Model Snapshot and Predictor Binning files:",
         placeholder="/Users/Downloads",
     )
+    import_strategy = "eager" if opts["extract_keys"] else "lazy"
     if dir != "":
         try:
             model_matches = pega_io.get_latest_file(dir, target="modelData")
         except FileNotFoundError:
             st.error(f"**Directory not found:** {dir}")
             st.stop()
         except NotADirectoryError:
@@ -137,25 +138,25 @@
             )
             model_analysis = st.checkbox("Only run model-based Health Check")
             if model_analysis:
                 st.session_state["dm"] = cachedDatamart(
                     path=dir,
                     model_filename=Path(model_matches).name,
                     predictor_filename=None,
-                    import_strategy="lazy",
+                    import_strategy=import_strategy,
                     **opts,
                 )
                 st.session_state["modelhc"] = True
 
         else:
             st.session_state["dm"] = cachedDatamart(
                 path=dir,
                 model_filename=Path(model_matches).name,
                 predictor_filename=Path(predictor_matches).name,
-                import_strategy="lazy",
+                import_strategy=import_strategy,
                 **opts,
             )
 
 
 def filter_dataframe(df: pl.LazyFrame, schema: Optional[dict] = None) -> pl.LazyFrame:
     """
     Adds a UI on top of a dataframe to let viewers filter columns
```

### Comparing `pdstools-3.1.8/python/pdstools/utils/table_definitions.py` & `pdstools-3.1.9/python/pdstools/utils/table_definitions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.8/python/pdstools/valuefinder/ValueFinder.py` & `pdstools-3.1.9/python/pdstools/valuefinder/ValueFinder.py`

 * *Files identical despite different names*

