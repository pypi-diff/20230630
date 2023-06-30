# Comparing `tmp/exposan-1.2.5.tar.gz` & `tmp/exposan-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exposan-1.2.5.tar", last modified: Tue Jan 31 23:15:47 2023, max compression
+gzip compressed data, was "exposan-1.3.0.tar", last modified: Fri Jun 30 20:45:29 2023, max compression
```

## Comparing `exposan-1.2.5.tar` & `exposan-1.3.0.tar`

### file list

```diff
@@ -1,141 +1,147 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:47.026826 exposan-1.2.5/
--rw-rw-rw-   0        0        0     5385 2022-10-08 14:24:51.000000 exposan-1.2.5/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0      227 2022-10-08 14:24:51.000000 exposan-1.2.5/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1937 2022-10-08 14:24:51.000000 exposan-1.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0      726 2022-10-08 14:24:51.000000 exposan-1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6248 2023-01-31 23:15:47.026826 exposan-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4947 2022-12-08 03:41:14.000000 exposan-1.2.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.879989 exposan-1.2.5/exposan/
--rw-rw-rw-   0        0        0      640 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.901506 exposan-1.2.5/exposan/adm/
--rw-rw-rw-   0        0        0     2190 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/adm/README.rst
--rw-rw-rw-   0        0        0     1708 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/adm/__init__.py
--rw-rw-rw-   0        0        0     5095 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/adm/analyses.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.901506 exposan-1.2.5/exposan/adm/data/
--rw-rw-rw-   0        0        0     1362 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/adm/data/_adm1.tsv
--rw-rw-rw-   0        0        0    37114 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/adm/data/stoichio.xlsx
--rw-rw-rw-   0        0        0     2853 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/adm/model.py
--rw-rw-rw-   0        0        0     4913 2022-12-08 03:41:14.000000 exposan-1.2.5/exposan/adm/system.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.905529 exposan-1.2.5/exposan/asm/
--rw-rw-rw-   0        0        0     1518 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/asm/README.rst
--rw-rw-rw-   0        0        0     2228 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/asm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.905529 exposan-1.2.5/exposan/asm/data/
--rw-rw-rw-   0        0        0      788 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/asm/data/_asm1.tsv
--rw-rw-rw-   0        0        0     7588 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/asm/systems.py
--rw-rw-rw-   0        0        0     7028 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/asm/validation.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.913148 exposan-1.2.5/exposan/biogenic_refinery/
--rw-rw-rw-   0        0        0     7422 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/biogenic_refinery/README.rst
--rw-rw-rw-   0        0        0    22979 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/biogenic_refinery/__init__.py
--rw-rw-rw-   0        0        0     5652 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/biogenic_refinery/_components.py
--rw-rw-rw-   0        0        0    12884 2022-12-08 03:41:14.000000 exposan-1.2.5/exposan/biogenic_refinery/country_specific.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.914154 exposan-1.2.5/exposan/biogenic_refinery/data/
--rw-rw-rw-   0        0        0      586 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/biogenic_refinery/data/impact_indicators.csv
--rw-rw-rw-   0        0        0    22078 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/biogenic_refinery/data/impact_items.xlsx
--rw-rw-rw-   0        0        0    46976 2022-12-08 03:41:14.000000 exposan-1.2.5/exposan/biogenic_refinery/models.py
--rw-rw-rw-   0        0        0    24902 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/biogenic_refinery/systems.py
--rw-rw-rw-   0        0        0     1333 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/biogenic_refinery/uncertainty.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.919076 exposan-1.2.5/exposan/bsm1/
--rw-rw-rw-   0        0        0    10334 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bsm1/README.rst
--rw-rw-rw-   0        0        0     2004 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/bsm1/__init__.py
--rw-rw-rw-   0        0        0    18470 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bsm1/analyses.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.919076 exposan-1.2.5/exposan/bsm1/data/
--rw-rw-rw-   0        0        0      788 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bsm1/data/_asm1.tsv
--rw-rw-rw-   0        0        0    18455 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bsm1/data/initial_conditions.xlsx
--rw-rw-rw-   0        0        0   205750 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bsm1/data/matlab_exported_data.xlsx
--rw-rw-rw-   0        0        0    12349 2023-01-23 17:32:59.000000 exposan-1.2.5/exposan/bsm1/model.py
--rw-rw-rw-   0        0        0     7192 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/bsm1/system.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.929379 exposan-1.2.5/exposan/bwaise/
--rw-rw-rw-   0        0        0    10923 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bwaise/README.rst
--rw-rw-rw-   0        0        0    15472 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/bwaise/__init__.py
--rw-rw-rw-   0        0        0     5302 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bwaise/_components.py
--rw-rw-rw-   0        0        0    13681 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bwaise/_lca_data.py
--rw-rw-rw-   0        0        0    22122 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bwaise/analyses.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.931384 exposan-1.2.5/exposan/bwaise/data/
--rw-rw-rw-   0        0        0    24099 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bwaise/data/LCA ReCiPe Damage to Points Unit Conversion.xlsx
--rw-rw-rw-   0        0        0    14499 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bwaise/data/cf_dct.pckl
--rw-rw-rw-   0        0        0     1472 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bwaise/data/indicators_new.tsv
--rw-rw-rw-   0        0        0     1187 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bwaise/data/indicators_original.tsv
--rw-rw-rw-   0        0        0    11285 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bwaise/data/items_original.xlsx
--rw-rw-rw-   0        0        0    38545 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bwaise/models.py
--rw-rw-rw-   0        0        0     7926 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bwaise/stats_demo.py
--rw-rw-rw-   0        0        0    21744 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/bwaise/systems.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.935412 exposan-1.2.5/exposan/cas/
--rw-rw-rw-   0        0        0      597 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/cas/README.rst
--rw-rw-rw-   0        0        0     1929 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/cas/__init__.py
--rw-rw-rw-   0        0        0     1810 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/cas/_components.py
--rw-rw-rw-   0        0        0     3044 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/cas/system.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.935412 exposan-1.2.5/exposan/eco_san/
--rw-rw-rw-   0        0        0     6061 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/eco_san/README.rst
--rw-rw-rw-   0        0        0     7954 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/eco_san/__init__.py
--rw-rw-rw-   0        0        0     1275 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/eco_san/_components.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.939419 exposan-1.2.5/exposan/eco_san/data/
--rw-rw-rw-   0        0        0     1187 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/eco_san/data/impact_indicators.tsv
--rw-rw-rw-   0        0        0    12445 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/eco_san/data/impact_items.xlsx
--rw-rw-rw-   0        0        0    17043 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/eco_san/systems.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.944455 exposan-1.2.5/exposan/htl/
--rw-rw-rw-   0        0        0     3935 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/htl/__init__.py
--rw-rw-rw-   0        0        0    19398 2023-01-31 21:22:43.000000 exposan-1.2.5/exposan/htl/_components.py
--rw-rw-rw-   0        0        0     3407 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/htl/_process_settings.py
--rw-rw-rw-   0        0        0    22683 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/htl/_sanunits.py
--rw-rw-rw-   0        0        0    11557 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/htl/_tea.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.947477 exposan-1.2.5/exposan/htl/data/
--rw-rw-rw-   0        0        0      998 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/htl/data/impact_indicators.csv
--rw-rw-rw-   0        0        0    46881 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/htl/data/impact_items.xlsx
--rw-rw-rw-   0        0        0    50404 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/htl/models.py
--rw-rw-rw-   0        0        0    24367 2023-01-31 21:11:31.000000 exposan-1.2.5/exposan/htl/systems.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.947477 exposan-1.2.5/exposan/interface/
--rw-rw-rw-   0        0        0     1886 2023-01-25 01:11:15.000000 exposan-1.2.5/exposan/interface/README.rst
--rw-rw-rw-   0        0        0     1499 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/interface/__init__.py
--rw-rw-rw-   0        0        0     3965 2023-01-24 15:07:42.000000 exposan-1.2.5/exposan/interface/system.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.954362 exposan-1.2.5/exposan/metab_mock/
--rw-rw-rw-   0        0        0     1026 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/_milestone_analysis.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.976927 exposan-1.2.5/exposan/metab_mock/data/
--rw-rw-rw-   0        0        0    24157 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/data/CFs.xlsx
--rw-rw-rw-   0        0        0    17562 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/data/HDPE_pipe_chart.xlsx
--rw-rw-rw-   0        0        0     9538 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/data/TRACI_indicators.xlsx
--rw-rw-rw-   0        0        0    64306 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/data/_impact_items.xlsx
--rw-rw-rw-   0        0        0    10229 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/data/stainless_steel_pipe_chart.xlsx
--rw-rw-rw-   0        0        0     2626 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/hrt_test.py
--rw-rw-rw-   0        0        0     6425 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/lca.py
--rw-rw-rw-   0        0        0      468 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/models.py
--rw-rw-rw-   0        0        0    12142 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/systems.py
--rw-rw-rw-   0        0        0    40717 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/units.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:47.005673 exposan-1.2.5/exposan/metab_mock/utils/
--rw-rw-rw-   0        0        0      321 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/utils/__init__.py
--rw-rw-rw-   0        0        0     4057 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/utils/dm_lci.py
--rw-rw-rw-   0        0        0     8579 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/utils/encap_lci.py
--rw-rw-rw-   0        0        0     2844 2023-01-31 22:29:34.000000 exposan-1.2.5/exposan/metab_mock/utils/er_lci.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:47.018528 exposan-1.2.5/exposan/new_generator/
--rw-rw-rw-   0        0        0     9442 2023-01-27 17:53:59.000000 exposan-1.2.5/exposan/new_generator/README.rst
--rw-rw-rw-   0        0        0    16490 2022-12-04 15:43:22.000000 exposan-1.2.5/exposan/new_generator/__init__.py
--rw-rw-rw-   0        0        0     1859 2022-12-04 15:43:22.000000 exposan-1.2.5/exposan/new_generator/_components.py
--rw-rw-rw-   0        0        0     1205 2022-12-04 15:43:22.000000 exposan-1.2.5/exposan/new_generator/analysis.py
--rw-rw-rw-   0        0        0    10223 2022-12-04 15:43:22.000000 exposan-1.2.5/exposan/new_generator/country_specific.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:47.018528 exposan-1.2.5/exposan/new_generator/data/
--rw-rw-rw-   0        0        0      586 2022-12-04 15:43:22.000000 exposan-1.2.5/exposan/new_generator/data/impact_indicators.csv
--rw-rw-rw-   0        0        0    28614 2022-12-04 15:43:22.000000 exposan-1.2.5/exposan/new_generator/data/impact_items.xlsx
--rw-rw-rw-   0        0        0    37028 2022-12-04 15:43:22.000000 exposan-1.2.5/exposan/new_generator/models.py
--rw-rw-rw-   0        0        0    14994 2023-01-27 17:59:31.000000 exposan-1.2.5/exposan/new_generator/systems.py
--rw-rw-rw-   0        0        0     1168 2022-12-04 15:43:22.000000 exposan-1.2.5/exposan/new_generator/uncertainty.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:47.026826 exposan-1.2.5/exposan/reclaimer/
--rw-rw-rw-   0        0        0     7598 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/reclaimer/README.rst
--rw-rw-rw-   0        0        0    15800 2023-01-23 17:29:31.000000 exposan-1.2.5/exposan/reclaimer/__init__.py
--rw-rw-rw-   0        0        0     2842 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/reclaimer/_components.py
--rw-rw-rw-   0        0        0     9375 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/reclaimer/country_specific.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:47.026826 exposan-1.2.5/exposan/reclaimer/data/
--rw-rw-rw-   0        0        0      586 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/reclaimer/data/impact_indicators.csv
--rw-rw-rw-   0        0        0    21977 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/reclaimer/data/impact_items.xlsx
--rw-rw-rw-   0        0        0    34303 2022-12-08 03:41:14.000000 exposan-1.2.5/exposan/reclaimer/models.py
--rw-rw-rw-   0        0        0    18132 2022-12-28 22:37:10.000000 exposan-1.2.5/exposan/reclaimer/systems.py
--rw-rw-rw-   0        0        0     1165 2022-10-08 14:24:51.000000 exposan-1.2.5/exposan/reclaimer/uncertainty.py
--rw-rw-rw-   0        0        0    21800 2022-12-08 03:41:14.000000 exposan-1.2.5/exposan/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:15:46.894204 exposan-1.2.5/exposan.egg-info/
--rw-rw-rw-   0        0        0     6248 2023-01-31 23:15:46.000000 exposan-1.2.5/exposan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3522 2023-01-31 23:15:46.000000 exposan-1.2.5/exposan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 23:15:46.000000 exposan-1.2.5/exposan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-01-31 23:15:46.000000 exposan-1.2.5/exposan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-01-31 23:15:46.000000 exposan-1.2.5/exposan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      657 2023-01-27 18:01:27.000000 exposan-1.2.5/pytest.ini
--rw-rw-rw-   0        0        0       42 2023-01-31 23:15:47.026826 exposan-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2681 2023-01-31 23:12:40.000000 exposan-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:29.491557 exposan-1.3.0/
+-rw-rw-rw-   0        0        0     5385 2022-10-08 14:24:51.000000 exposan-1.3.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0      227 2022-10-08 14:24:51.000000 exposan-1.3.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1937 2022-10-08 14:24:51.000000 exposan-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      726 2022-10-08 14:24:51.000000 exposan-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6248 2023-06-30 20:45:29.488323 exposan-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4947 2022-12-08 03:41:14.000000 exposan-1.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.430344 exposan-1.3.0/exposan/
+-rw-rw-rw-   0        0        0      640 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.487422 exposan-1.3.0/exposan/adm/
+-rw-rw-rw-   0        0        0     2190 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/adm/README.rst
+-rw-rw-rw-   0        0        0     1708 2023-02-04 00:06:58.000000 exposan-1.3.0/exposan/adm/__init__.py
+-rw-rw-rw-   0        0        0     5095 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/adm/analyses.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.516124 exposan-1.3.0/exposan/adm/data/
+-rw-rw-rw-   0        0        0     1362 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/adm/data/_adm1.tsv
+-rw-rw-rw-   0        0        0    37114 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/adm/data/stoichio.xlsx
+-rw-rw-rw-   0        0        0     2853 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/adm/model.py
+-rw-rw-rw-   0        0        0     4913 2022-12-08 03:41:14.000000 exposan-1.3.0/exposan/adm/system.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.532486 exposan-1.3.0/exposan/asm/
+-rw-rw-rw-   0        0        0     1518 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/asm/README.rst
+-rw-rw-rw-   0        0        0     2228 2023-02-04 00:06:58.000000 exposan-1.3.0/exposan/asm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.536010 exposan-1.3.0/exposan/asm/data/
+-rw-rw-rw-   0        0        0      788 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/asm/data/_asm1.tsv
+-rw-rw-rw-   0        0        0     7588 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/asm/systems.py
+-rw-rw-rw-   0        0        0     7028 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/asm/validation.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.564175 exposan-1.3.0/exposan/biogenic_refinery/
+-rw-rw-rw-   0        0        0     7422 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/biogenic_refinery/README.rst
+-rw-rw-rw-   0        0        0    22979 2023-03-03 20:42:22.000000 exposan-1.3.0/exposan/biogenic_refinery/__init__.py
+-rw-rw-rw-   0        0        0     5652 2023-03-03 20:42:22.000000 exposan-1.3.0/exposan/biogenic_refinery/_components.py
+-rw-rw-rw-   0        0        0    12884 2022-12-08 03:41:14.000000 exposan-1.3.0/exposan/biogenic_refinery/country_specific.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.568222 exposan-1.3.0/exposan/biogenic_refinery/data/
+-rw-rw-rw-   0        0        0      586 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/biogenic_refinery/data/impact_indicators.csv
+-rw-rw-rw-   0        0        0    22078 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/biogenic_refinery/data/impact_items.xlsx
+-rw-rw-rw-   0        0        0    46976 2023-03-03 20:42:22.000000 exposan-1.3.0/exposan/biogenic_refinery/models.py
+-rw-rw-rw-   0        0        0    24902 2023-03-03 20:42:22.000000 exposan-1.3.0/exposan/biogenic_refinery/systems.py
+-rw-rw-rw-   0        0        0     1333 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/biogenic_refinery/uncertainty.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.593060 exposan-1.3.0/exposan/bsm1/
+-rw-rw-rw-   0        0        0    10334 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bsm1/README.rst
+-rw-rw-rw-   0        0        0     2004 2023-02-04 00:06:58.000000 exposan-1.3.0/exposan/bsm1/__init__.py
+-rw-rw-rw-   0        0        0    18470 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bsm1/analyses.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.616879 exposan-1.3.0/exposan/bsm1/data/
+-rw-rw-rw-   0        0        0      788 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bsm1/data/_asm1.tsv
+-rw-rw-rw-   0        0        0    18455 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bsm1/data/initial_conditions.xlsx
+-rw-rw-rw-   0        0        0   205750 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bsm1/data/matlab_exported_data.xlsx
+-rw-rw-rw-   0        0        0    12349 2023-06-30 20:31:25.000000 exposan-1.3.0/exposan/bsm1/model.py
+-rw-rw-rw-   0        0        0     7192 2023-02-04 00:06:58.000000 exposan-1.3.0/exposan/bsm1/system.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.674459 exposan-1.3.0/exposan/bwaise/
+-rw-rw-rw-   0        0        0    10923 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bwaise/README.rst
+-rw-rw-rw-   0        0        0    15472 2023-02-04 00:06:58.000000 exposan-1.3.0/exposan/bwaise/__init__.py
+-rw-rw-rw-   0        0        0     5302 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bwaise/_components.py
+-rw-rw-rw-   0        0        0    13681 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bwaise/_lca_data.py
+-rw-rw-rw-   0        0        0    22122 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bwaise/analyses.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.723971 exposan-1.3.0/exposan/bwaise/data/
+-rw-rw-rw-   0        0        0    24099 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bwaise/data/LCA ReCiPe Damage to Points Unit Conversion.xlsx
+-rw-rw-rw-   0        0        0    14499 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bwaise/data/cf_dct.pckl
+-rw-rw-rw-   0        0        0     1472 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bwaise/data/indicators_new.tsv
+-rw-rw-rw-   0        0        0     1187 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bwaise/data/indicators_original.tsv
+-rw-rw-rw-   0        0        0    11285 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bwaise/data/items_original.xlsx
+-rw-rw-rw-   0        0        0    38545 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bwaise/models.py
+-rw-rw-rw-   0        0        0     7926 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bwaise/stats_demo.py
+-rw-rw-rw-   0        0        0    21744 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/bwaise/systems.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.745753 exposan-1.3.0/exposan/cas/
+-rw-rw-rw-   0        0        0      597 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/cas/README.rst
+-rw-rw-rw-   0        0        0     1929 2023-02-04 00:06:58.000000 exposan-1.3.0/exposan/cas/__init__.py
+-rw-rw-rw-   0        0        0     1810 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/cas/_components.py
+-rw-rw-rw-   0        0        0     3044 2023-01-23 17:29:31.000000 exposan-1.3.0/exposan/cas/system.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.777618 exposan-1.3.0/exposan/eco_san/
+-rw-rw-rw-   0        0        0     6061 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/eco_san/README.rst
+-rw-rw-rw-   0        0        0     7954 2023-02-04 00:06:58.000000 exposan-1.3.0/exposan/eco_san/__init__.py
+-rw-rw-rw-   0        0        0     1275 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/eco_san/_components.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.785659 exposan-1.3.0/exposan/eco_san/data/
+-rw-rw-rw-   0        0        0     1187 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/eco_san/data/impact_indicators.tsv
+-rw-rw-rw-   0        0        0    12445 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/eco_san/data/impact_items.xlsx
+-rw-rw-rw-   0        0        0    17043 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/eco_san/systems.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.825693 exposan-1.3.0/exposan/htl/
+-rw-rw-rw-   0        0        0     3993 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/htl/__init__.py
+-rw-rw-rw-   0        0        0    19398 2023-01-31 21:22:43.000000 exposan-1.3.0/exposan/htl/_components.py
+-rw-rw-rw-   0        0        0     3407 2023-02-04 00:06:58.000000 exposan-1.3.0/exposan/htl/_process_settings.py
+-rw-rw-rw-   0        0        0    22698 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/htl/_sanunits.py
+-rw-rw-rw-   0        0        0    11557 2023-02-04 00:06:58.000000 exposan-1.3.0/exposan/htl/_tea.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.858274 exposan-1.3.0/exposan/htl/data/
+-rw-rw-rw-   0        0        0      998 2023-01-23 17:29:31.000000 exposan-1.3.0/exposan/htl/data/impact_indicators.csv
+-rw-rw-rw-   0        0        0    47603 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/htl/data/impact_items.xlsx
+-rw-rw-rw-   0        0        0      165 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/htl/data/~$impact_items.xlsx
+-rw-rw-rw-   0        0        0    60791 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/htl/models.py
+-rw-rw-rw-   0        0        0    25641 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/htl/systems.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.895937 exposan-1.3.0/exposan/interface/
+-rw-rw-rw-   0        0        0     1886 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/interface/README.rst
+-rw-rw-rw-   0        0        0     1499 2023-02-04 00:06:58.000000 exposan-1.3.0/exposan/interface/__init__.py
+-rw-rw-rw-   0        0        0     3965 2023-03-14 13:50:46.000000 exposan-1.3.0/exposan/interface/system.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:29.116511 exposan-1.3.0/exposan/metab_mock/
+-rw-rw-rw-   0        0        0     1097 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/metab_mock/__init__.py
+-rw-rw-rw-   0        0        0     4934 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/metab_mock/_milestone_analysis.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:29.186069 exposan-1.3.0/exposan/metab_mock/data/
+-rw-rw-rw-   0        0        0    25454 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/metab_mock/data/CFs.xlsx
+-rw-rw-rw-   0        0        0    17562 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/metab_mock/data/HDPE_pipe_chart.xlsx
+-rw-rw-rw-   0        0        0    10229 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/metab_mock/data/stainless_steel_pipe_chart.xlsx
+-rw-rw-rw-   0        0        0     2626 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/metab_mock/hrt_test.py
+-rw-rw-rw-   0        0        0      744 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/metab_mock/init_cond_test.py
+-rw-rw-rw-   0        0        0     2878 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/metab_mock/process.py
+-rw-rw-rw-   0        0        0    12838 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/metab_mock/systems.py
+-rw-rw-rw-   0        0        0    23768 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/metab_mock/test_biofilm.py
+-rw-rw-rw-   0        0        0    13642 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/metab_mock/units.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:29.358004 exposan-1.3.0/exposan/new_generator/
+-rw-rw-rw-   0        0        0     9442 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/new_generator/README.rst
+-rw-rw-rw-   0        0        0    16490 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/new_generator/__init__.py
+-rw-rw-rw-   0        0        0     1859 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/new_generator/_components.py
+-rw-rw-rw-   0        0        0     1205 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/new_generator/analysis.py
+-rw-rw-rw-   0        0        0    10223 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/new_generator/country_specific.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:29.406796 exposan-1.3.0/exposan/new_generator/data/
+-rw-rw-rw-   0        0        0      586 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/new_generator/data/impact_indicators.csv
+-rw-rw-rw-   0        0        0    28614 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/new_generator/data/impact_items.xlsx
+-rw-rw-rw-   0        0        0    37028 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/new_generator/models.py
+-rw-rw-rw-   0        0        0    14994 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/new_generator/systems.py
+-rw-rw-rw-   0        0        0     1168 2023-06-11 13:36:53.000000 exposan-1.3.0/exposan/new_generator/uncertainty.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:29.445880 exposan-1.3.0/exposan/reclaimer/
+-rw-rw-rw-   0        0        0     7598 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/reclaimer/README.rst
+-rw-rw-rw-   0        0        0    15800 2023-02-04 00:06:58.000000 exposan-1.3.0/exposan/reclaimer/__init__.py
+-rw-rw-rw-   0        0        0     2842 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/reclaimer/_components.py
+-rw-rw-rw-   0        0        0     9375 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/reclaimer/country_specific.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:29.448495 exposan-1.3.0/exposan/reclaimer/data/
+-rw-rw-rw-   0        0        0      586 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/reclaimer/data/impact_indicators.csv
+-rw-rw-rw-   0        0        0    21977 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/reclaimer/data/impact_items.xlsx
+-rw-rw-rw-   0        0        0    34303 2022-12-08 03:41:14.000000 exposan-1.3.0/exposan/reclaimer/models.py
+-rw-rw-rw-   0        0        0    18132 2022-12-28 22:37:10.000000 exposan-1.3.0/exposan/reclaimer/systems.py
+-rw-rw-rw-   0        0        0     1165 2022-10-08 14:24:51.000000 exposan-1.3.0/exposan/reclaimer/uncertainty.py
+-rw-rw-rw-   0        0        0    21800 2022-12-08 03:41:14.000000 exposan-1.3.0/exposan/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:28.463598 exposan-1.3.0/exposan.egg-info/
+-rw-rw-rw-   0        0        0     6248 2023-06-30 20:45:28.000000 exposan-1.3.0/exposan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3586 2023-06-30 20:45:28.000000 exposan-1.3.0/exposan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 20:45:28.000000 exposan-1.3.0/exposan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 20:45:28.000000 exposan-1.3.0/exposan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-30 20:45:28.000000 exposan-1.3.0/exposan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      698 2023-06-11 13:36:53.000000 exposan-1.3.0/pytest.ini
+-rw-rw-rw-   0        0        0       42 2023-06-30 20:45:29.492575 exposan-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2681 2023-06-30 20:43:54.000000 exposan-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:45:29.483962 exposan-1.3.0/tests/
+-rw-rw-rw-   0        0        0     2025 2023-02-04 00:06:58.000000 exposan-1.3.0/tests/test_adm.py
+-rw-rw-rw-   0        0        0     1675 2023-01-23 17:29:31.000000 exposan-1.3.0/tests/test_asm.py
+-rw-rw-rw-   0        0        0     2641 2023-06-11 13:36:53.000000 exposan-1.3.0/tests/test_biogenic_refinery.py
+-rw-rw-rw-   0        0        0     1785 2023-02-04 00:06:58.000000 exposan-1.3.0/tests/test_bsm1.py
+-rw-rw-rw-   0        0        0     1208 2023-06-11 13:36:53.000000 exposan-1.3.0/tests/test_bwaise.py
+-rw-rw-rw-   0        0        0      514 2023-01-23 17:29:31.000000 exposan-1.3.0/tests/test_cas.py
+-rw-rw-rw-   0        0        0     1207 2023-06-11 13:36:53.000000 exposan-1.3.0/tests/test_eco_san.py
+-rw-rw-rw-   0        0        0     1403 2023-06-11 13:45:47.000000 exposan-1.3.0/tests/test_htl.py
+-rw-rw-rw-   0        0        0     1246 2023-06-14 15:15:54.000000 exposan-1.3.0/tests/test_interface.py
+-rw-rw-rw-   0        0        0     2666 2023-06-11 13:36:53.000000 exposan-1.3.0/tests/test_reclaimer.py
```

### Comparing `exposan-1.2.5/CODE_OF_CONDUCT.md` & `exposan-1.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/LICENSE.txt` & `exposan-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/MANIFEST.in` & `exposan-1.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/PKG-INFO` & `exposan-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exposan
-Version: 1.2.5
+Version: 1.3.0
 Summary: Exposition of sanitation and resource recovery systems
 Home-page: https://github.com/QSD-Group/EXPOsan
 Author: Quantitative Sustainable Design Group
 Author-email: quantitative.sustainable.design@gmail.com
 License: UIUC
 Project-URL: Homepage, https://qsdsan.com
 Project-URL: Documentation, https://qsdsan.readthedocs.io
```

### Comparing `exposan-1.2.5/README.rst` & `exposan-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/__init__.py` & `exposan-1.3.0/exposan/__init__.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/adm/README.rst` & `exposan-1.3.0/exposan/adm/README.rst`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/adm/__init__.py` & `exposan-1.3.0/exposan/adm/__init__.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/adm/analyses.py` & `exposan-1.3.0/exposan/adm/analyses.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/adm/data/_adm1.tsv` & `exposan-1.3.0/exposan/adm/data/_adm1.tsv`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/adm/data/stoichio.xlsx` & `exposan-1.3.0/exposan/adm/data/stoichio.xlsx`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/adm/model.py` & `exposan-1.3.0/exposan/adm/model.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/adm/system.py` & `exposan-1.3.0/exposan/adm/system.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/asm/README.rst` & `exposan-1.3.0/exposan/asm/README.rst`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/asm/__init__.py` & `exposan-1.3.0/exposan/asm/__init__.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/asm/data/_asm1.tsv` & `exposan-1.3.0/exposan/asm/data/_asm1.tsv`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/asm/systems.py` & `exposan-1.3.0/exposan/asm/systems.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/asm/validation.py` & `exposan-1.3.0/exposan/asm/validation.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/biogenic_refinery/README.rst` & `exposan-1.3.0/exposan/biogenic_refinery/README.rst`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/biogenic_refinery/__init__.py` & `exposan-1.3.0/exposan/biogenic_refinery/__init__.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/biogenic_refinery/_components.py` & `exposan-1.3.0/exposan/biogenic_refinery/_components.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/biogenic_refinery/country_specific.py` & `exposan-1.3.0/exposan/biogenic_refinery/country_specific.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/biogenic_refinery/data/impact_indicators.csv` & `exposan-1.3.0/exposan/biogenic_refinery/data/impact_indicators.csv`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/biogenic_refinery/data/impact_items.xlsx` & `exposan-1.3.0/exposan/biogenic_refinery/data/impact_items.xlsx`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/biogenic_refinery/models.py` & `exposan-1.3.0/exposan/biogenic_refinery/models.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/biogenic_refinery/systems.py` & `exposan-1.3.0/exposan/biogenic_refinery/systems.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/biogenic_refinery/uncertainty.py` & `exposan-1.3.0/exposan/biogenic_refinery/uncertainty.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bsm1/README.rst` & `exposan-1.3.0/exposan/bsm1/README.rst`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bsm1/__init__.py` & `exposan-1.3.0/exposan/bsm1/__init__.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bsm1/analyses.py` & `exposan-1.3.0/exposan/bsm1/analyses.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bsm1/data/_asm1.tsv` & `exposan-1.3.0/exposan/bsm1/data/_asm1.tsv`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bsm1/data/initial_conditions.xlsx` & `exposan-1.3.0/exposan/bsm1/data/initial_conditions.xlsx`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bsm1/data/matlab_exported_data.xlsx` & `exposan-1.3.0/exposan/bsm1/data/matlab_exported_data.xlsx`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bsm1/model.py` & `exposan-1.3.0/exposan/bsm1/model.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bsm1/system.py` & `exposan-1.3.0/exposan/bsm1/system.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/README.rst` & `exposan-1.3.0/exposan/bwaise/README.rst`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/__init__.py` & `exposan-1.3.0/exposan/bwaise/__init__.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/_components.py` & `exposan-1.3.0/exposan/bwaise/_components.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/_lca_data.py` & `exposan-1.3.0/exposan/bwaise/_lca_data.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/analyses.py` & `exposan-1.3.0/exposan/bwaise/analyses.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/data/LCA ReCiPe Damage to Points Unit Conversion.xlsx` & `exposan-1.3.0/exposan/bwaise/data/LCA ReCiPe Damage to Points Unit Conversion.xlsx`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/data/cf_dct.pckl` & `exposan-1.3.0/exposan/bwaise/data/cf_dct.pckl`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/data/indicators_new.tsv` & `exposan-1.3.0/exposan/bwaise/data/indicators_new.tsv`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/data/indicators_original.tsv` & `exposan-1.3.0/exposan/bwaise/data/indicators_original.tsv`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/data/items_original.xlsx` & `exposan-1.3.0/exposan/bwaise/data/items_original.xlsx`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/models.py` & `exposan-1.3.0/exposan/bwaise/models.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/stats_demo.py` & `exposan-1.3.0/exposan/bwaise/stats_demo.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/bwaise/systems.py` & `exposan-1.3.0/exposan/bwaise/systems.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/cas/README.rst` & `exposan-1.3.0/exposan/cas/README.rst`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/cas/__init__.py` & `exposan-1.3.0/exposan/cas/__init__.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/cas/_components.py` & `exposan-1.3.0/exposan/cas/_components.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/cas/system.py` & `exposan-1.3.0/exposan/cas/system.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/eco_san/README.rst` & `exposan-1.3.0/exposan/eco_san/README.rst`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/eco_san/__init__.py` & `exposan-1.3.0/exposan/eco_san/__init__.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/eco_san/_components.py` & `exposan-1.3.0/exposan/eco_san/_components.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/eco_san/data/impact_indicators.tsv` & `exposan-1.3.0/exposan/eco_san/data/impact_indicators.tsv`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/eco_san/data/impact_items.xlsx` & `exposan-1.3.0/exposan/eco_san/data/impact_items.xlsx`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/eco_san/systems.py` & `exposan-1.3.0/exposan/eco_san/systems.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/htl/__init__.py` & `exposan-1.3.0/exposan/htl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 Please refer to https://github.com/QSD-Group/EXPOsan/blob/main/LICENSE.txt
 for license details.
 '''
 
 import os, pandas as pd, qsdsan as qs
 from qsdsan.utils import auom
 from exposan.utils import _init_modules
+from datetime import date
 
 htl_path = os.path.dirname(__file__)
 module = os.path.split(htl_path)[-1]
 data_path, results_path = _init_modules(module, include_data_path=True)
 
 _kg_to_g = auom('kg').conversion_factor('g')
 _m3perh_to_MGD = auom('m3/h').conversion_factor('MGD')
@@ -74,15 +75,15 @@
         
 from . import models
 from .models import *
 
 def simulate_and_save(model,
                       resample=True, samples_kwargs={'N':1000, 'rule':'L', 'seed':None},
                       include_spearman=True, spearman_kwargs={'nan_policy': 'omit'},
-                      export_results=True, path='',):
+                      export_results=True, path='',notes=''):
     if resample:
         kwargs = {'N':1000, 'rule':'L', 'seed':None}
         kwargs.update(samples_kwargs)
         samples = model.sample(**kwargs)
         model.load_samples(samples)
     model.evaluate()
     idx = len(model.parameters)
@@ -93,15 +94,15 @@
         kwargs = {'nan_policy': 'omit'}
         kwargs.update(spearman_kwargs)
         r_df, p_df = qs.stats.get_correlations(model, kind='Spearman', **kwargs)
 
     if export_results:
         ID = model.system.flowsheet.ID
         N = model.table.shape[0]
-        path = path or os.path.join(results_path, f'_{ID}_{N}.xlsx')
+        path = path or os.path.join(results_path, f'{date.today()}__{ID}_{N}_{notes}.xlsx')
         with pd.ExcelWriter(path) as writer:
             parameters.to_excel(writer, sheet_name='Parameters')
             results.to_excel(writer, sheet_name='Results')
             percentiles.to_excel(writer, sheet_name='Percentiles')
             if include_spearman:
                 r_df.to_excel(writer, sheet_name='Spearman_r')
                 p_df.to_excel(writer, sheet_name='Spearman_p')
```

### Comparing `exposan-1.2.5/exposan/htl/_components.py` & `exposan-1.3.0/exposan/htl/_components.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/htl/_process_settings.py` & `exposan-1.3.0/exposan/htl/_process_settings.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/htl/_sanunits.py` & `exposan-1.3.0/exposan/htl/_sanunits.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,27 +97,28 @@
         
         SanUnit.__init__(self, ID, ins, outs, thermo, init_with)
         self.ww_2_dry_sludge = ww_2_dry_sludge
         self.sludge_moisture = sludge_moisture
         self.sludge_dw_ash = sludge_dw_ash
         self.sludge_afdw_lipid = sludge_afdw_lipid
         self.sludge_afdw_protein = sludge_afdw_protein
-        self.sludge_afdw_carbo = round(1 - sludge_afdw_protein - sludge_afdw_lipid, 5)
         self.lipid_2_C = lipid_2_C
         self.protein_2_C = protein_2_C
         self.carbo_2_C = carbo_2_C
         self.C_2_H = C_2_H
         self.protein_2_N = protein_2_N
         self.N_2_P = N_2_P
         self.operation_hours = operation_hours
     
     def _run(self):
         
         ww = self.ins[0]
         sludge, treated = self.outs
+
+        self.sludge_afdw_carbo = round(1 - self.sludge_afdw_protein - self.sludge_afdw_lipid, 5)   
         
         if self.sludge_dw_ash >= 1:
             raise Exception ('ash can not be larger than or equal to 1')
         
         if self.sludge_afdw_protein + self.sludge_afdw_lipid > 1:
             raise Exception ('protein and lipid exceed 1')
```

### Comparing `exposan-1.2.5/exposan/htl/_tea.py` & `exposan-1.3.0/exposan/htl/_tea.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/htl/data/impact_indicators.csv` & `exposan-1.3.0/exposan/htl/data/impact_indicators.csv`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/htl/models.py` & `exposan-1.3.0/exposan/htl/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,24 +15,25 @@
 '''
 
 import qsdsan as qs
 from chaospy import distributions as shape
 from qsdsan.utils import DictAttrSetter
 
 from exposan.htl import (
-    _kg_to_g,
     _m3perh_to_MGD,
     _MJ_to_MMBTU,
     _MMgal_to_L,
     create_system,
     )
 
 __all__ = ('create_model',)
 
-def create_model(system=None, exclude_sludge_compositions=False, key_metrics_only=False):
+def create_model(system=None, exclude_sludge_compositions=False,
+                 include_HTL_yield_as_metrics=True, include_other_metrics=True,
+                 include_other_CFs_as_metrics=True, include_check=True):
     '''
     Create a model based on the given system
     (or create the system based on the given configuration).
     
     Parameters
     ----------
     system : obj or str
@@ -813,34 +814,35 @@
             kind='isolated',
             units='$/kg',
             baseline=38.79,
             distribution=dist)
     def set_HT_HC_catalyst_price(i):
         CoMo_alumina_HT.price=CoMo_alumina_HC.price=i
         
-    FuelMixer = unit.FuelMixer
+    gasoline = stream.gasoline
     dist = shape.Triangle(0.7085,0.9388,1.4493)
     @param(name='gasoline price',
             element='TEA',
             kind='isolated',
             units='$/kg',
             baseline=0.9388,
             distribution=dist)
     def set_gasoline_price(i):
-        FuelMixer.gasoline_price=i
-        
+        gasoline.price=i
+    
+    diesel = stream.diesel
     dist = shape.Triangle(0.7458,0.9722,1.6579)
     @param(name='diesel price',
             element='TEA',
             kind='isolated',
             units='$/kg',
             baseline=0.9722,
             distribution=dist)
     def set_diesel_price(i):
-        FuelMixer.diesel_price=i
+        diesel.price=i
         
     # dist = shape.Uniform(-0.0605,-0.0495)
     # @param(name='residual disposal',
     #         element='TEA',
     #         kind='isolated',
     #         units='$/kg',
     #         baseline=-0.055,
@@ -859,14 +861,15 @@
     def set_electrivity_price(i):
         qs.PowerUtility.price=i
     
     # =========================================================================
     # LCA (unifrom ± 10%)
     # =========================================================================
     # don't get joint distribution for multiple times, since the baselines for LCA will change.
+    qs.ImpactItem.get_all_items().pop('waste_sludge_item')
     for item in qs.ImpactItem.get_all_items().keys():
         for CF in qs.ImpactIndicator.get_all_indicators().keys():
             abs_small = 0.9*qs.ImpactItem.get_item(item).CFs[CF]
             abs_large = 1.1*qs.ImpactItem.get_item(item).CFs[CF]
             dist = shape.Uniform(min(abs_small,abs_large),max(abs_small,abs_large))
             @param(name=f'{item}_{CF}',
                    setter=DictAttrSetter(qs.ImpactItem.get_item(item), 'CFs', CF),
@@ -880,15 +883,15 @@
     
     # =========================================================================
     # metrics
     # =========================================================================
 
     metric = model.metric
     
-    if not key_metrics_only: # all metrics
+    if include_other_metrics: # all metrics
         # Element metrics
         @metric(name='sludge_C',units='kg/hr',element='Sankey')
         def get_sludge_C():
             return WWTP.sludge_C
         
         @metric(name='sludge_N',units='kg/hr',element='Sankey')
         def get_sludge_N():
@@ -956,15 +959,14 @@
             return sum(mass*[cmp.i_C for cmp in cmps])
         
         @metric(name='HT_gas_N',units='kg/hr',element='Sankey')
         def get_HT_gas_N():
             mass = F2.outs[0].mass + D1.outs[0].mass
             return sum(mass*[cmp.i_N for cmp in cmps])
     
-        
         @metric(name='HT_ww_C',units='kg/hr',element='Sankey')
         def get_HT_ww_C():
             mass = sum((i.outs[0].mass for i in (D1, D2, D3, F2)), D3.outs[1].mass)
             return HTL.biocrude_C - sum(mass*[cmp.i_C for cmp in cmps])
         
         @metric(name='HT_ww_N',units='kg/hr',element='Sankey')
         def get_HT_ww_N():
@@ -1112,31 +1114,44 @@
         SluC, P1 = unit.SluC, unit.P1
         @metric(name='HTL_CAPEX',units='$',element='TEA')
         def get_HTL_CAPEX():
             return sum(i.installed_cost for i in (SluC, P1, H1, HTL))
         
         SP1, H2SO4_Tank = unit.SP1, unit.H2SO4_Tank
         if AcidEx:
-            def get_Phosphorus_CAPEX():
-                return (AcidEx.installed_cost +
-                        StruPre.installed_cost +
-                        H2SO4_Tank.installed_cost*SP1.outs[0].F_mass/SP1.F_mass_out)
+            if SP1.F_mass_out != 0:
+                def get_Phosphorus_CAPEX():
+                    return (AcidEx.installed_cost +
+                            StruPre.installed_cost +
+                            H2SO4_Tank.installed_cost*SP1.outs[0].F_mass/SP1.F_mass_out)
+            else:
+                def get_Phosphorus_CAPEX():
+                    return 0
         else:
-            def get_Phosphorus_CAPEX():
-                return (StruPre.installed_cost +
-                        H2SO4_Tank.installed_cost*SP1.outs[0].F_mass/SP1.F_mass_out)
+            if SP1.F_mass_out != 0:
+                def get_Phosphorus_CAPEX():
+                    return (StruPre.installed_cost +
+                            H2SO4_Tank.installed_cost*SP1.outs[0].F_mass/SP1.F_mass_out)
+            else:
+                def get_Phosphorus_CAPEX():
+                    return 0
         model.metric(getter=get_Phosphorus_CAPEX, name='Phosphorus_CAPEX',units='$',element='TEA')
         
         @metric(name='CHG_CAPEX',units='$',element='TEA')
         def get_CHG_CAPEX():
             return CHG.installed_cost + F1.installed_cost
         
-        @metric(name='Nitrogen_CAPEX',units='$',element='TEA')
-        def get_Nitrogen_CAPEX():
-            return MemDis.installed_cost+H2SO4_Tank.installed_cost*SP1.outs[1].F_mass/SP1.F_mass_out
+        if SP1.F_mass_out != 0:
+            def get_Nitrogen_CAPEX():
+                return MemDis.installed_cost+H2SO4_Tank.installed_cost*SP1.outs[1].F_mass/SP1.F_mass_out
+        else:
+            def get_Nitrogen_CAPEX():
+                return 0
+        model.metric(getter=get_Nitrogen_CAPEX, name='Nitrogen_CAPEX',units='$',element='TEA')
+        
         
         HT_HC_units = (unit.P2, HT, unit.H2, F2, unit.H3, D1, D2, D3, unit.P3, HC,
                        unit.H4, F3, D4, unit.H5, unit.H6, unit.GasolineTank, unit.DieselTank)
         @metric(name='HT_HC_CAPEX',units='$',element='TEA')
         def get_HT_HC_CAPEX():
             return sum(i.installed_cost for i in HT_HC_units)
         
@@ -1228,18 +1243,18 @@
         
         # LCA metrics
         lca = sys.LCA
         @metric(name='construction_GWP',units='kg CO2 eq',element='LCA')
         def get_construction_GWP():
             return lca.get_construction_impacts()['GlobalWarming']
         
-        fuel = stream.fuel
+        diesel = stream.diesel
         @metric(name='stream_GWP',units='kg CO2 eq',element='LCA')
         def get_stream_GWP():
-            return lca.get_stream_impacts(exclude=(fuel,))['GlobalWarming']
+            return lca.get_stream_impacts()['GlobalWarming']
         
         @metric(name='other_GWP',units='kg CO2 eq',element='LCA')
         def get_other_GWP():
             return lca.get_other_impacts()['GlobalWarming']
         
         @metric(name='HTL_constrution_GWP',units='kg CO2 eq',element='LCA')
         def get_HTL_constrution_GWP():
@@ -1283,15 +1298,15 @@
         def get_CHG_stream_GWP():
             table_stream = lca.get_impact_table('Stream')['GlobalWarming [kg CO2-eq]']
             return table_stream['CHG_catalyst_out']
         
         @metric(name='HT_HC_stream_GWP',units='kg CO2 eq',element='LCA')
         def get_HT_HC_stream_GWP():
             table_stream = lca.get_impact_table('Stream')['GlobalWarming [kg CO2-eq]']
-            return table_stream['H2']+table_stream['HT_catalyst_out']+table_stream['HC_catalyst_out']
+            return table_stream['H2']+table_stream['HT_catalyst_out']+table_stream['HC_catalyst_out']+table_stream['gasoline']+table_stream['diesel']
         
         @metric(name='nutrient_stream_GWP',units='kg CO2 eq',element='LCA')
         def get_nutrient_stream_GWP():
             table_stream = lca.get_impact_table('Stream')['GlobalWarming [kg CO2-eq]']
             return table_stream['H2SO4']+table_stream['MgCl2']+table_stream['MgO']+table_stream['struvite']+\
                    table_stream['NH4Cl']+table_stream['Membrane_in']+table_stream['NaOH']+table_stream['ammonium_sulfate']
                    
@@ -1357,32 +1372,218 @@
             table_other = lca.get_impact_table('Other')['GlobalWarming [kg CO2-eq]']
             return table_other['Electricity [kWh]']
         
         @metric(name='cooling_GWP',units='kg CO2 eq',element='LCA')
         def get_cooling_GWP():
             table_other = lca.get_impact_table('Other')['GlobalWarming [kg CO2-eq]']
             return table_other['Cooling [MJ]']
+        
+        @metric(name='HTL_cooling_percentage',units='-',element='utilities')
+        def get_HTL_cooling_percentage():
+            HTL_cool=0
+            for i in range(len(unit.HTL.heat_utilities)):
+                if unit.HTL.heat_utilities[i].duty < 0:
+                    HTL_cool+=unit.HTL.heat_utilities[i].duty
+                    
+            sys_cool=0
+            for i in range(len(sys.heat_utilities)):
+                if sys.heat_utilities[i].duty < 0:
+                    sys_cool+=sys.heat_utilities[i].duty
+                    
+            HXN_cool=0
+            for i in range(len(unit.HXN.heat_utilities)):
+                if unit.HXN.heat_utilities[i].duty > 0:
+                    HXN_cool+=unit.HXN.heat_utilities[i].duty
+            
+            return HTL_cool/(sys_cool-HXN_cool)
+        
+        @metric(name='CHG_cooling_percentage',units='-',element='utilities')
+        def get_CHG_cooling_percentage():
+            CHG_cool=0
+            for i in range(len(unit.CHG.heat_utilities)):
+                if unit.CHG.heat_utilities[i].duty < 0:
+                    CHG_cool+=unit.CHG.heat_utilities[i].duty
+                    
+            sys_cool=0
+            for i in range(len(sys.heat_utilities)):
+                if sys.heat_utilities[i].duty < 0:
+                    sys_cool+=sys.heat_utilities[i].duty
+                    
+            HXN_cool=0
+            for i in range(len(unit.HXN.heat_utilities)):
+                if unit.HXN.heat_utilities[i].duty > 0:
+                    HXN_cool+=unit.HXN.heat_utilities[i].duty
+            
+            return CHG_cool/(sys_cool-HXN_cool)
+        
+        @metric(name='HTL_heating_percentage',units='-',element='utilities')
+        def get_HTL_heating_percentage():
+            HTL_heat=0
+            for i in range(len(unit.H1.heat_utilities)):
+                if unit.H1.heat_utilities[i].duty > 0:
+                    HTL_heat+=unit.H1.heat_utilities[i].duty
+                    
+            sys_heat=0
+            for i in range(len(sys.heat_utilities)):
+                if sys.heat_utilities[i].duty > 0:
+                    sys_heat+=sys.heat_utilities[i].duty
+                    
+            HXN_heat=0
+            for i in range(len(unit.HXN.heat_utilities)):
+                if unit.HXN.heat_utilities[i].duty < 0:
+                    HXN_heat+=unit.HXN.heat_utilities[i].duty
+                    
+            CHP_heat=0
+            for i in range(len(unit.CHP.heat_utilities)):
+                if unit.CHP.heat_utilities[i].duty < 0:
+                    CHP_heat+=unit.CHP.heat_utilities[i].duty
+            
+            return HTL_heat/(sys_heat-HXN_heat-CHP_heat)
+        
+        @metric(name='CHG_heating_percentage',units='-',element='utilities')
+        def get_CHG_heating_percentage():
+            CHG_heat=0
+            for i in range(len(unit.CHG.heat_utilities)):
+                if unit.CHG.heat_utilities[i].duty > 0:
+                    CHG_heat+=unit.CHG.heat_utilities[i].duty
+                    
+            sys_heat=0
+            for i in range(len(sys.heat_utilities)):
+                if sys.heat_utilities[i].duty > 0:
+                    sys_heat+=sys.heat_utilities[i].duty
+                    
+            HXN_heat=0
+            for i in range(len(unit.HXN.heat_utilities)):
+                if unit.HXN.heat_utilities[i].duty < 0:
+                    HXN_heat+=unit.HXN.heat_utilities[i].duty
+                    
+            CHP_heat=0
+            for i in range(len(unit.CHP.heat_utilities)):
+                if unit.CHP.heat_utilities[i].duty < 0:
+                    CHP_heat+=unit.CHP.heat_utilities[i].duty
+            
+            return CHG_heat/(sys_heat-HXN_heat-CHP_heat)
+        
+        @metric(name='HXN_heat_offset',units='-',element='utilities')
+        def get_HXN_heat_offset():
+            return 1-unit.HXN.actual_heat_util_load/unit.HXN.original_heat_util_load
+        
+        @metric(name='HXN_cool_offset',units='-',element='utilities')
+        def get_HXN_cool_offset():
+            return 1-unit.HXN.actual_cool_util_load/unit.HXN.original_cool_util_load
 
     else:
-        fuel = stream.fuel
+        diesel = stream.diesel
         lca = sys.LCA
-    
+        HTL = unit.HTL
+        
+    if include_HTL_yield_as_metrics:
+        @metric(name='HTL_biocrude_yield',units='-',element='HTL')
+        def get_HTL_biocrude_yield():
+            return HTL.biocrude_yield
+        
+        @metric(name='HTL_aqueous_yield',units='-',element='HTL')
+        def get_HTL_aqueous_yield():
+            return HTL.aqueous_yield
+        
+        @metric(name='HTL_biochar_yield',units='-',element='HTL')
+        def get_HTL_biochar_yield():
+            return HTL.biochar_yield
+        
+        @metric(name='HTL_gasyield',units='-',element='HTL')
+        def get_HTL_gas_yield():
+            return HTL.gas_yield
+        
     # Key metrics
-    @metric(name='MFSP',units='$/gal diesel',element='TEA')
-    def get_MFSP():
-        return tea.solve_price(fuel)*FuelMixer.diesel_gal_2_kg
+    @metric(name='MDSP',units='$/gal diesel',element='TEA')
+    def get_MDSP():
+        diesel_gal_2_kg=3.220628346
+        return tea.solve_price(diesel)*diesel_gal_2_kg
     
     raw_wastewater = stream.raw_wastewater
     @metric(name='sludge_management_price',units='$/ton dry sludge',element='TEA')
     def get_sludge_treatment_price():
         return -tea.solve_price(raw_wastewater)*_MMgal_to_L/WWTP.ww_2_dry_sludge
     
-    @metric(name='GWP_diesel',units='g CO2/MMBTU diesel',element='LCA')
-    def get_LCA_diesel():
-        return lca.get_total_impacts(exclude=(fuel,))['GlobalWarming']/fuel.F_mass/sys.operating_hours/lca.lifetime*_kg_to_g/45.5/_MJ_to_MMBTU
-    # diesel: 45.5 MJ/kg
+    @metric(name='GWP_diesel',units='kg CO2/MMBTU diesel',element='LCA')
+    def get_GWP_diesel():
+        return lca.get_total_impacts(exclude=(diesel,))['GlobalWarming']/diesel.F_mass/sys.operating_hours/lca.lifetime/45.6/_MJ_to_MMBTU
+    # gasoline : 46.4 MJ/kg
+    # diesel: 45.6 MJ/kg
     
     @metric(name='GWP_sludge',units='kg CO2/ton dry sludge',element='LCA')
-    def get_LCA_sludge():
-        return lca.get_total_impacts()['GlobalWarming']/raw_wastewater.F_vol/_m3perh_to_MGD/WWTP.ww_2_dry_sludge/(sys.operating_hours/24)/lca.lifetime
+    def get_GWP_sludge():
+        return lca.get_total_impacts(exclude=(raw_wastewater,))['GlobalWarming']/raw_wastewater.F_vol/_m3perh_to_MGD/WWTP.ww_2_dry_sludge/(sys.operating_hours/24)/lca.lifetime
+    
+    if include_other_CFs_as_metrics:
+    
+        @metric(name='OzoneDepletion_diesel',units='kg CFC-11-eq/MMBTU diesel',element='LCA')
+        def get_OZP_diesel():
+            return lca.get_total_impacts(exclude=(diesel,))['OzoneDepletion']/diesel.F_mass/sys.operating_hours/lca.lifetime/45.6/_MJ_to_MMBTU
+
+        @metric(name='OzoneDepletion_sludge',units='kg CFC-11-eq/ton dry sludge',element='LCA')
+        def get_OZP_sludge():
+            return lca.get_total_impacts()['OzoneDepletion']/raw_wastewater.F_vol/_m3perh_to_MGD/WWTP.ww_2_dry_sludge/(sys.operating_hours/24)/lca.lifetime
+    
+        @metric(name='Carcinogenics_diesel',units='kg benzene-eq/MMBTU diesel',element='LCA')
+        def get_CAR_diesel():
+            return lca.get_total_impacts(exclude=(diesel,))['Carcinogenics']/diesel.F_mass/sys.operating_hours/lca.lifetime/45.6/_MJ_to_MMBTU
+
+        @metric(name='Carcinogenics_sludge',units='kg benzene-eq/ton dry sludge',element='LCA')
+        def get_CAR_sludge():
+            return lca.get_total_impacts()['Carcinogenics']/raw_wastewater.F_vol/_m3perh_to_MGD/WWTP.ww_2_dry_sludge/(sys.operating_hours/24)/lca.lifetime
+    
+        @metric(name='Acidification_diesel',units='moles of H+-eq/MMBTU diesel',element='LCA')
+        def get_ACD_diesel():
+            return lca.get_total_impacts(exclude=(diesel,))['Acidification']/diesel.F_mass/sys.operating_hours/lca.lifetime/45.6/_MJ_to_MMBTU
+
+        @metric(name='Acidification_sludge',units='moles of H+-eq/ton dry sludge',element='LCA')
+        def get_ACD_sludge():
+            return lca.get_total_impacts()['Acidification']/raw_wastewater.F_vol/_m3perh_to_MGD/WWTP.ww_2_dry_sludge/(sys.operating_hours/24)/lca.lifetime
+    
+        @metric(name='RespiratoryEffects_diesel',units='kg PM2.5-eq/MMBTU diesel',element='LCA')
+        def get_RES_diesel():
+            return lca.get_total_impacts(exclude=(diesel,))['RespiratoryEffects']/diesel.F_mass/sys.operating_hours/lca.lifetime/45.6/_MJ_to_MMBTU
+
+        @metric(name='RespiratoryEffects_sludge',units='kg PM2.5-eq/ton dry sludge',element='LCA')
+        def get_RES_sludge():
+            return lca.get_total_impacts()['RespiratoryEffects']/raw_wastewater.F_vol/_m3perh_to_MGD/WWTP.ww_2_dry_sludge/(sys.operating_hours/24)/lca.lifetime
+    
+        @metric(name='Eutrophication_diesel',units='kg N/MMBTU diesel',element='LCA')
+        def get_EUT_diesel():
+            return lca.get_total_impacts(exclude=(diesel,))['Eutrophication']/diesel.F_mass/sys.operating_hours/lca.lifetime/45.6/_MJ_to_MMBTU
+
+        @metric(name='Eutrophication_sludge',units='kg N/ton dry sludge',element='LCA')
+        def get_EUT_sludge():
+            return lca.get_total_impacts()['Eutrophication']/raw_wastewater.F_vol/_m3perh_to_MGD/WWTP.ww_2_dry_sludge/(sys.operating_hours/24)/lca.lifetime
+    
+        @metric(name='PhotochemicalOxidation_diesel',units='kg NOx-eq/MMBTU diesel',element='LCA')
+        def get_PHO_diesel():
+            return lca.get_total_impacts(exclude=(diesel,))['PhotochemicalOxidation']/diesel.F_mass/sys.operating_hours/lca.lifetime/45.6/_MJ_to_MMBTU
+
+        @metric(name='PhotochemicalOxidation_sludge',units='kg NOx-eq/ton dry sludge',element='LCA')
+        def get_PHO_sludge():
+            return lca.get_total_impacts()['PhotochemicalOxidation']/raw_wastewater.F_vol/_m3perh_to_MGD/WWTP.ww_2_dry_sludge/(sys.operating_hours/24)/lca.lifetime
+    
+        @metric(name='Ecotoxicity_diesel',units='kg 2,4-D-eq/MMBTU diesel',element='LCA')
+        def get_ECO_diesel():
+            return lca.get_total_impacts(exclude=(diesel,))['Ecotoxicity']/diesel.F_mass/sys.operating_hours/lca.lifetime/45.6/_MJ_to_MMBTU
+
+        @metric(name='Ecotoxicity_sludge',units='kg 2,4-D-eq/ton dry sludge',element='LCA')
+        def get_ECO_sludge():
+            return lca.get_total_impacts()['Ecotoxicity']/raw_wastewater.F_vol/_m3perh_to_MGD/WWTP.ww_2_dry_sludge/(sys.operating_hours/24)/lca.lifetime
+    
+        @metric(name='NonCarcinogenics_diesel',units='kg toluene-eq/MMBTU diesel',element='LCA')
+        def get_NCA_diesel():
+            return lca.get_total_impacts(exclude=(diesel,))['NonCarcinogenics']/diesel.F_mass/sys.operating_hours/lca.lifetime/45.6/_MJ_to_MMBTU
+
+        @metric(name='NonCarcinogenics_sludge',units='kg toluene-eq/ton dry sludge',element='LCA')
+        def get_NCA_sludge():
+            return lca.get_total_impacts()['NonCarcinogenics']/raw_wastewater.F_vol/_m3perh_to_MGD/WWTP.ww_2_dry_sludge/(sys.operating_hours/24)/lca.lifetime
+        
+    if include_check:
+        
+        @metric(name='sludge_afdw_carbohydrate',units='-',element='test')
+        def get_sludge_afdw_carbohydrate():
+            return unit.WWTP.sludge_afdw_carbo
     
     return model
```

### Comparing `exposan-1.2.5/exposan/htl/systems.py` & `exposan-1.3.0/exposan/htl/systems.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,19 @@
 from qsdsan.utils import clear_lca_registries
 from exposan.htl import (
     _load_components,
     _load_process_settings,
     create_tea,
     )
 from exposan.htl import _sanunits as su
+from biosteam import settings
 
 __all__ = ('create_system',)
 
-def create_system(configuration='baseline'):
+def create_system(configuration='baseline', waste_price=0, waste_GWP=0):
     configuration = configuration or 'baseline'
     if configuration not in ('baseline', 'no_P', 'PSA'):
         raise ValueError('`configuration` can only be "baseline", '
                          '"no_P" (without acid extraction and P recovery), '
                          'or "PSA" (with H2 recovery through pressure swing adsorption), '
                          f'not "{configuration}".')
     flowsheet_ID = f'htl_{configuration}'
@@ -64,29 +65,32 @@
     _load_process_settings()
     
     # Construction here, StreamImpactItem after TEA
     folder = os.path.dirname(__file__)
     qs.ImpactIndicator.load_from_file(os.path.join(folder, 'data/impact_indicators.csv'))
     qs.ImpactItem.load_from_file(os.path.join(folder, 'data/impact_items.xlsx'))
     
-    raw_wastewater = qs.Stream('raw_wastewater', H2O=100, units='MGD', T=25+273.15)
+    
+    raw_wastewater = qs.WasteStream('raw_wastewater', H2O=100, units='MGD', T=25+273.15)
     # Jones baseline: 1276.6 MGD, 1.066e-4 $/kg ww
     # set H2O equal to the total raw wastewater into the WWTP
     
     # =============================================================================
     # pretreatment (Area 000)
     # =============================================================================
                 
     WWTP = su.WWTP('S000', ins=raw_wastewater, outs=('sludge','treated_water'),
                    ww_2_dry_sludge=0.94,
                    # how much metric ton/day sludge can be produced by 1 MGD of ww
                    sludge_moisture=0.99, sludge_dw_ash=0.257, 
                    sludge_afdw_lipid=0.204, sludge_afdw_protein=0.463, operation_hours=7920)
     WWTP.register_alias('WWTP')
     
+    raw_wastewater.price = -WWTP.ww_2_dry_sludge*waste_price/3.79/(10**6)
+    
     SluC = qsu.SludgeCentrifuge('A000', ins=WWTP-0,
                             outs=('supernatant','compressed_sludge'),
                             init_with='Stream',
                             solids=('Sludge_lipid','Sludge_protein',
                                     'Sludge_carbo','Sludge_ash'),
                             sludge_moisture=0.8)
     SluC.register_alias('SluC')
@@ -156,15 +160,15 @@
     CHG.ins[1].price = 134.53
     CHG.register_alias('CHG')
     
     V1 = IsenthalpicValve('A240', ins=CHG-0, outs='depressed_cooled_CHG', P=50*6894.76, vle=True)
     V1.register_alias('V1')
     
     F1 = qsu.Flash('A250', ins=V1-0, outs=('CHG_fuel_gas','N_riched_aqueous'),
-                     T=60+273.15, P=50*6894.76)
+                     T=60+273.15, P=50*6894.76, thermo=settings.thermo.ideal())
     F1.register_alias('F1')
     
     MemDis = qsu.MembraneDistillation('A260', ins=(F1-1, SP1-1, 'NaOH', 'Membrane_in'),
                                   outs=('ammonium_sulfate','MemDis_ww', 'Membrane_out','solution'), init_with='WasteStream')
     MemDis.ins[2].price = 0.5256
     MemDis.outs[0].price = 0.3236
     MemDis.register_alias('MemDis')
@@ -198,17 +202,18 @@
     
     V2 = IsenthalpicValve('A320', ins=HT-0, outs='depressed_HT', P=717.4*6894.76, vle=True)
     V2.register_alias('V2')
     
     H2 = qsu.HXutility('A330', ins=V2-0, outs='cooled_HT', T=60+273.15,
                         init_with='Stream', rigorous=True)
     H2.register_alias('H2')
-    
+
+
     F2 = qsu.Flash('A340', ins=H2-0, outs=('HT_fuel_gas','HT_aqueous'), T=43+273.15,
-               P=717.4*6894.76) # outflow P
+               P=717.4*6894.76, thermo=settings.thermo.ideal()) # outflow P
     F2.register_alias('F2')
     
     V3 = IsenthalpicValve('A350', ins=F2-1, outs='depressed_flash_effluent', P=55*6894.76, vle=True)
     V3.register_alias('V3')
     
     SP2 = qsu.Splitter('S310', ins=V3-0, outs=('HT_ww','HT_oil'),
                         split={'H2O':1}, init_with='Stream')
@@ -303,42 +308,41 @@
     PC4 = qsu.PhaseChanger('S550', ins=HT-1, outs='HT_catalyst_out', phase='s')
     PC4.register_alias('PC4')
     
     PC5 = qsu.PhaseChanger('S560', ins=HC-1, outs='HC_catalyst_out', phase='s')
     PC5.register_alias('PC5')
     
     GasolineTank = qsu.StorageTank('T500', ins=PC1-0, outs=('gasoline'),
-                                    tau=3*24, init_with='Stream', vessel_material='Carbon steel')
+                                    tau=3*24, init_with='WasteStream', vessel_material='Carbon steel')
     # store for 3 days based on Jones 2014
     GasolineTank.register_alias('GasolineTank')
     
+    GasolineTank.outs[0].price = 0.9388
+    
     DieselTank = qsu.StorageTank('T510', ins=PC2-0, outs=('diesel'),
-                                  tau=3*24, init_with='Stream', vessel_material='Carbon steel')
+                                  tau=3*24, init_with='WasteStream', vessel_material='Carbon steel')
     # store for 3 days based on Jones 2014
     DieselTank.register_alias('DieselTank')
     
-    FuelMixer = su.FuelMixer('S570', ins=(GasolineTank-0, DieselTank-0),
-                             outs='fuel', target='diesel')
-    # integrate gasoline and diesel based on their LHV for MFSP calculation
-    FuelMixer.register_alias('FuelMixer')
+    DieselTank.outs[0].price = 0.9722
     
     GasMixer = qsu.Mixer('S580', ins=(HTL-3, F1-0, F2-0, D1-0, F3-0),
                           outs=('fuel_gas'), init_with='Stream')
     GasMixer.register_alias('GasMixer')
     
     WWmixer = su.WWmixer('S590', ins=(SluC-0, MemDis-1, SP2-0),
                         outs='wastewater', init_with='Stream')
     # effluent of WWmixer goes back to WWTP
     WWmixer.register_alias('WWmixer')
     
     # =============================================================================
     # facilities
     # =============================================================================
     
-    qsu.HeatExchangerNetwork('HXN')
+    qsu.HeatExchangerNetwork('HXN', force_ideal_thermo=True)
     
     CHP = qsu.CombinedHeatPower('CHP', include_construction=True,
                                 ins=(GasMixer-0, 'natural_gas', 'air'),
                   outs=('emission','solid_ash'), init_with='WasteStream',
                   supplement_power_utility=False)
     CHP.ins[1].price = 0.1685
     
@@ -346,14 +350,28 @@
         f'sys_{configuration}',
         units=list(flowsheet.unit), 
         operating_hours=WWTP.operation_hours, # 7920 hr Jones
         )
     sys.register_alias('sys')
 
     ##### Add stream impact items #####
+
+    # add impact for waste sludge
+    qs.StreamImpactItem(ID='waste_sludge_item',
+                        linked_stream=stream.raw_wastewater,
+                        Acidification=0,
+                        Ecotoxicity=0,
+                        Eutrophication=0,
+                        GlobalWarming=-WWTP.ww_2_dry_sludge*waste_GWP/3.79/(10**6),
+                        OzoneDepletion=0,
+                        PhotochemicalOxidation=0,
+                        Carcinogenics=0,
+                        NonCarcinogenics=0,
+                        RespiratoryEffects=0)
+    
     # Biocrude upgrading
     qs.StreamImpactItem(ID='H2_item',
                         linked_stream=stream.H2,
                         Acidification=0.81014,
                         Ecotoxicity=0.42747,
                         Eutrophication=0.0029415,
                         GlobalWarming=1.5624,
@@ -509,17 +527,30 @@
                         GlobalWarming=-1.2499,
                         OzoneDepletion=-6.12E-08,
                         PhotochemicalOxidation=-0.0044519,
                         Carcinogenics=-0.036742,
                         NonCarcinogenics=-62.932,
                         RespiratoryEffects=-0.0031315)
     
+    # Gasoline (naphtha)
+    qs.StreamImpactItem(ID='gasoline_item',
+                        linked_stream=stream.gasoline,
+                        Acidification=-0.21813,
+                        Ecotoxicity=-0.15887,
+                        Eutrophication=-0.0010594,
+                        GlobalWarming=-0.36865,
+                        OzoneDepletion=-6.4977E-07,
+                        PhotochemicalOxidation=-0.00182,
+                        Carcinogenics=-0.00053932,
+                        NonCarcinogenics=-2.2524,
+                        RespiratoryEffects=-0.0009461)
+    
     # Diesel
     qs.StreamImpactItem(ID='diesel_item',
-                        linked_stream=stream.fuel,
+                        linked_stream=stream.diesel,
                         Acidification=-0.25164,
                         Ecotoxicity=-0.18748,
                         Eutrophication=-0.0010547,
                         GlobalWarming=-0.47694,
                         OzoneDepletion=-6.42E-07,
                         PhotochemicalOxidation=-0.0019456,
                         Carcinogenics=-0.00069252,
```

### Comparing `exposan-1.2.5/exposan/interface/README.rst` & `exposan-1.3.0/exposan/interface/README.rst`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/interface/__init__.py` & `exposan-1.3.0/exposan/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/interface/system.py` & `exposan-1.3.0/exposan/interface/system.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/metab_mock/__init__.py` & `exposan-1.3.0/exposan/metab_mock/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,34 +8,40 @@
 
 This module is under the University of Illinois/NCSA Open Source License.
 Please refer to https://github.com/QSD-Group/EXPOsan/blob/main/LICENSE.txt
 for license details.
 '''
 
 import os
+
 folder = os.path.dirname(__file__)
 data_path = os.path.join(folder, 'data')
 results_path = os.path.join(folder, 'results')
 figures_path = os.path.join(folder, 'figures')
 # To save simulation results and generated figures
 if not os.path.isdir(results_path): os.mkdir(results_path)
 if not os.path.isdir(figures_path): os.mkdir(figures_path)
-del os
+
+_impact_item_loaded = False
+from exposan.metab import load_lca_data
+
+from . import process
+from .process import *
 
 from . import units
 from .units import *
 
 from . import systems
 from .systems import *
 
-# from . import models
-# from .models import *
 
 __all__ = (
     'folder',
     'data_path',
     'results_path',
     'figures_path',
+    *process.__all__,
     *units.__all__,
     *systems.__all__,
-    # *models.__all__,
-	)
+	)
+
+
```

### Comparing `exposan-1.2.5/exposan/metab_mock/_milestone_analysis.py` & `exposan-1.3.0/exposan/metab_mock/_milestone_analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,68 +6,76 @@
     
     Joy Zhang <joycheung1994@gmail.com>
 
 This module is under the University of Illinois/NCSA Open Source License.
 Please refer to https://github.com/QSD-Group/EXPOsan/blob/main/LICENSE.txt
 for license details.
 '''
-from qsdsan import ImpactIndicator as IInd, ImpactItem as IItm, TEA, LCA, PowerUtility
-from qsdsan.utils import ospath, auom
-from exposan.metab_mock import create_systems, data_path, results_path
+from qsdsan import ImpactIndicator as IInd, ImpactItem as IItm, \
+    StreamImpactItem as SIItm, \
+    TEA, LCA, PowerUtility
+from qsdsan.utils import ospath
+from exposan.metab_mock import create_systems, data_path, results_path, DegassingMembrane
 import pandas as pd
 
 IInd.load_from_file(ospath.join(data_path, 'TRACI_indicators.xlsx'), sheet=0)
 IItm.load_from_file(ospath.join(data_path, '_impact_items.xlsx'))
-fugitive_ch4 = IItm(ID='fugitive_ch4', functional_unit='kg', 
-                    GWP100=28, MIR=0.0143794871794872)
+IItm('Stainless_steel', source='stainless_steel')
+bg_offset_CFs = IItm.get_item('biogas_offset').CFs
+NaOCl_item = IItm.get_item('NaOCl')
+citric_acid_item = IItm.get_item('citric_acid')
 
 #%%
 irr = 0.1
-# p_treatment = 0.28 # assume USD/kg COD centralized treatment
-p_ng = 0.688 # USD/therm of natural gas
+# p_ng = 0.65165 # USD/therm of natural gas charged to the brewery in 2016 (including tax and delivery etc.)
+# p_ng = 0.85*auom('kJ').conversion_factor('therm') # [USD/kJ] 5.47 2021USD/Mcf vs. 4.19 2016USD/Mcf
 op_hr = 365*24
 get = getattr
-PowerUtility.price = 0.0913
+PowerUtility.price = 0.0913 # 2021$ for minnesota area
 
 def run_tea_lca(sys, save_report=True, info='', lt=30):
     sys.simulate(state_reset_hook='reset_cache', t_span=(0, 400), method='BDF')
     F = sys.flowsheet
     inf = get(F.stream, f'BreweryWW_{F.ID}')
     eff = get(F.stream, f'Effluent_{F.ID}')
     cmps = eff.components
+    KJ_per_kg = cmps.i_mass/cmps.chem_MW*cmps.LHV
+    for ws in sys.products:
+        if ws.phase == 'l':
+            SIItm(ID=f'{ws.ID}_fugitive_ch4', linked_stream=ws, 
+                  flow_getter=lambda s: s.imass['S_ch4']*cmps.S_ch4.i_mass,
+                  GWP100=28, MIR=0.0143794871794872)
+        elif ws.phase == 'g':
+            fget = lambda s: -sum(s.mass*KJ_per_kg)*1e-3/39
+            SIItm(ID=f'{ws.ID}_NG_offset', linked_stream=ws, functional_unit='m3',
+                  flow_getter=fget, # m3/hr natural-gas-equivalent
+                  **bg_offset_CFs)
+    for u in sys.units:
+        if isinstance(u, DegassingMembrane):
+            SIItm(linked_stream=u.NaOCl, **NaOCl_item.CFs)
+            SIItm(linked_stream=u.citric_acid, **citric_acid_item.CFs)
     
     # Operation items
-    fug_ch4 = eff.imass['S_ch4']*cmps.S_ch4.i_mass # kg/h
-    kW = sys.power_utility.consumption
-    duties = [hu.duty for hu in sys.heat_utilities]
-    heat = sum(d for d in duties if d > 0)
-    cool = sum(d for d in duties if d < 0)
-    MJ_per_hr = (heat + cool * 0.2)*1e-3 # assume 20% efficiency in recoverying heat from R1 eff (i.e., R2 inf)
-    offset = sum(sum(bg.mass*cmps.i_mass/cmps.chem_MW*cmps.LHV) \
-               for bg in sys.products if bg.phase == 'g') # kJ/hr
-    V_offset = offset * 1e-3 / 39      # m3/hr natural-gas-equivalent
+    kWh = lambda lca: lca.system.power_utility.rate*lca.lifetime_hr
+    def MJ(lca):
+        sys = lca.system
+        duties = [hu.duty for hu in sys.heat_utilities]
+        MJ_per_hr = sum(d for d in duties if d > 0)*1e-3
+        return MJ_per_hr*lca.lifetime_hr
     
     rCOD = inf.composite('COD', flow=True) - eff.composite('COD', flow=True)  # kgCOD/hr
 
-    tea = TEA(
-        sys, discount_rate=irr, lifetime=lt, simulate_system=False, 
-        system_add_OPEX=dict(
-            # COD_discharge_reduction = -rCOD*p_treatment*op_hr,
-            NG_purchase_reduction = -auom('kJ').convert(offset,'therm')*p_ng*op_hr,
-            )
-        )
+    tea = TEA(sys, discount_rate=irr, lifetime=lt, simulate_system=False, CEPCI=708)
     levelized_cost = -tea.annualized_NPV/(rCOD * op_hr *1e-3)
     print(f'{sys.ID} TEA: ${round(levelized_cost, 1)}/ton rCOD')
     
     lca = LCA(
         sys, lifetime=lt, simulate_system=False,
-        electricity = (kW*lt*op_hr, 'kWh'),
-        heat_onsite = (MJ_per_hr*lt*op_hr, 'MJ'),
-        fugitive_ch4 = (fug_ch4*lt*op_hr, 'kg'),
-        biogas_offset = (-V_offset*lt*op_hr, 'm3')
+        electricity = kWh,
+        heat_onsite = MJ
         )
     
     gwp = lca.get_total_impacts()['GWP100']
     gwp_per_rcod = gwp/(rCOD * op_hr * lt *1e-3)
     print(f'{sys.ID} LCA: {round(gwp_per_rcod, 1)} kg CO2eq/ton rCOD')
     
     if save_report:
@@ -90,27 +98,29 @@
                 rs = u.results()
                 rs.index.names = ['l0', 'l1']
                 rs.join(pd.DataFrame.from_dict({'lifetime': u.lifetime}),
                         on='l1')
                 rs.to_excel(writer, sheet_name=u.ID)
         lca.save_report(ospath.join(results_path, f'{F.ID}_{info}_lca.xlsx'))
     
-    # return sys
+    return sys
 
 #%%
 if __name__ == '__main__':
-    save = True
-    # save = False
-    info = '35C_20yr_1yr'
-    lt = 20
-    sysA, sysB = create_systems(which=('A', 'B'))
-    print(info)
-    run_tea_lca(sysA, save, info, lt)
-    run_tea_lca(sysB, save, info, lt)
-    # systems = create_systems(which=('C', 'D'))
-    # for sys in systems:
-    #     u = sys.units[0]
-    #     for tau in (1, 2, 4, 8):
-    #         u.V_liq = tau*5
-    #         u.V_gas = tau*5/10
-    #         info = f'HRT{tau}'
-    #         run_tea_lca(sys, save, info, lt)
+    # save = True
+    save = False
+    info = '35C_30yr_1yr'
+    lt = 30
+    # sysA, sysB = create_systems(which=('A', 'B'))
+    # print(info)
+    # sysA = run_tea_lca(sysA, save, info, lt)
+    # run_tea_lca(sysB, save, info, lt)
+    systems = create_systems(which=('C',))
+    for sys in systems:
+        u = sys.units[0]
+        # for tau in (1, 2):
+        tau = 2
+        u.V_liq = tau*5
+        u.V_gas = tau*5/10
+        info = f'HRT{tau}'
+        # IItm.clear_registry()
+        run_tea_lca(sys, save, info, lt)
```

### Comparing `exposan-1.2.5/exposan/metab_mock/data/HDPE_pipe_chart.xlsx` & `exposan-1.3.0/exposan/metab_mock/data/HDPE_pipe_chart.xlsx`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/metab_mock/data/stainless_steel_pipe_chart.xlsx` & `exposan-1.3.0/exposan/metab_mock/data/stainless_steel_pipe_chart.xlsx`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/metab_mock/hrt_test.py` & `exposan-1.3.0/exposan/metab_mock/hrt_test.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/metab_mock/systems.py` & `exposan-1.3.0/exposan/metab_mock/systems.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,34 @@
 
 This module is under the University of Illinois/NCSA Open Source License.
 Please refer to https://github.com/QSD-Group/EXPOsan/blob/main/LICENSE.txt
 for license details.
 '''
 
 import numpy as np, qsdsan as qs
-from qsdsan import processes as pc, WasteStream, System
-from qsdsan.utils import ospath, ExogenousDynamicVariable as EDV
+from qsdsan import (
+    processes as pc, 
+    WasteStream, System, TEA, LCA, PowerUtility,
+    ImpactItem as IItm, 
+    StreamImpactItem as SIItm,
+    )
+from qsdsan.utils import ExogenousDynamicVariable as EDV
 from exposan.metab_mock import (
+    _impact_item_loaded,
+    load_lca_data,
     rhos_adm1_ph_ctrl,
+    METAB_AnCSTR as AB
+    )
+from exposan.metab import (
     DegassingMembrane as DM, 
-    METAB_AnCSTR as AB,
     IronSpongeTreatment as IST,
     DoubleMembraneGasHolder as GH,
+    add_strm_iitm, add_TEA_LCA
     )
 
-folder = ospath.dirname(__file__)
-
 __all__ = (
     'create_systems', 
     'default_inf_concs',
     'default_R1_init_conds',
     'default_R2_init_conds',
     'default_R_init_conds',
     'R1_ss_conds',
@@ -47,14 +55,18 @@
 ph1 = 5.8
 
 T2 = 273.15+25    
 Vl2 = 75*scale
 Vg2 = 5*(scale**0.5)
 ph2 = 7.2
 
+T3 = T2
+Vl3 = 5*scale
+Vg3 = 0.556*(scale**0.5)
+
 bl = 1   # yr, bead lifetime
 # bl = 10
 
 Temp1 = EDV('T1', function=lambda t: T1)
 Temp2 = EDV('T2', function=lambda t: T2)
 pH1 = EDV('pH1', function=lambda t: ph1)
 pH2 = EDV('pH2', function=lambda t: ph2)
@@ -165,21 +177,21 @@
  'S_IC': 846.4879614661522,
  'S_IN': 222.13725282096297,
  'S_I': 110.71467278942289,
  'X_c': 107.43132381172228,
  'X_ch': 1.2600235711799973,
  'X_pr': 1.3804329631122664,
  'X_li': 1.7696259648387357,
- 'X_su': 732.9760678333023,
- 'X_aa': 224.81751931525334,
- 'X_fa': 126.7301174776879,
- 'X_c4': 227.8726398428066,
- 'X_pro': 140.2738127019708,
- 'X_ac': 669.4626559278454,
- 'X_h2': 245.67774602566578,
+ 'X_su': 732.9760678333023*5,
+ 'X_aa': 224.81751931525334*5,
+ 'X_fa': 126.7301174776879*5,
+ 'X_c4': 227.8726398428066*5,
+ 'X_pro': 140.2738127019708*5,
+ 'X_ac': 669.4626559278454*5,
+ 'X_h2': 245.67774602566578*5,
  'X_I': 206.42934561053158,
  'S_cat': 40.0,
  'S_an': 20.0,
  }
 
 R1_ss_conds = {
     'S_su': 0.0145871088552909*1e3,
@@ -232,19 +244,21 @@
     'X_pro': 0.0503466475437059*1e3,
     'X_ac': 1.1653549028287*1e3,
     'X_h2': 0.4352809013846*1e3,
     'X_I': 0.196117291164614*1e3
     }
 
 #%% Systems
+if not _impact_item_loaded: load_lca_data()
 
-def create_systems(flowsheet_A=None, flowsheet_B=None, flowsheet_C=None, flowsheet_D=None,
+def create_systems(lifetime=30, discount_rate=0.1, electric_price=0.0913,
+                   flowsheet_A=None, flowsheet_B=None, flowsheet_C=None, flowsheet_D=None,
                    inf_concs={}, R1_init_conds={}, R2_init_conds={}, R_init_conds={}, 
                    which=None, selective=False):
-    
+    PowerUtility.price = electric_price
     which = which or ('A', 'B', 'C', 'D')
     if isinstance(which, str): which = (which,)
     
     if selective: 
         R1_retain = fermenters
         R2_retain = methanogens
     else: R1_retain = R2_retain = biomass_IDs
@@ -289,15 +303,16 @@
                  F_BM_default=1)
     
         R1A.set_init_conc(**R1_init_conds)
         R2A.set_init_conc(**R2_init_conds)
     
         sysA = System('sysA', path=(R1A, R2A))
         sysA.set_dynamic_tracker(R1A, R2A, bg1A, bg2A, effA)
-        
+        add_strm_iitm(sysA)
+        add_TEA_LCA(sysA, discount_rate, lifetime)
         systems.append(sysA)
         
     if 'B' in which:
         flowsheet_B = flowsheet_B or qs.Flowsheet('B')
         qs.main_flowsheet.set_flowsheet(flowsheet_B)
         
         infB = brewery_ww.copy('BreweryWW_B')
@@ -324,37 +339,40 @@
                   F_BM_default=1)
     
         R1B.set_init_conc(**R1_init_conds)
         R2B.set_init_conc(**R2_init_conds)
         
         sysB = System('sysB', path=(R1B, R2B, DM2B))
         sysB.set_dynamic_tracker(R1B, R2B, bg1B, bgh2B, bgm2B, effB)
-        
+        add_strm_iitm(sysB)
+        add_TEA_LCA(sysB, discount_rate, lifetime)
         systems.append(sysB)
     
     if 'C' in which:
         flowsheet_C = flowsheet_C or qs.Flowsheet('C')
         qs.main_flowsheet.set_flowsheet(flowsheet_C)
         
         infC = brewery_ww.copy('BreweryWW_C')
         effC = WasteStream('Effluent_C', T=T2)
         bgC = WasteStream('Biogas_C', phase='g')
 
         ISTC = IST(ID='ISTC')
         GHC = GH(ID='GHC')
         
         RC = AB('RC', ins=infC, outs=(bgC, effC), 
-                V_liq=Vl2, V_gas=Vg2, T=T2, model=adm1,
+                V_liq=Vl3, V_gas=Vg3, T=T3, model=adm1,
                 retain_cmps=biomass_IDs, bead_lifetime=bl,
                 equipment=[ISTC, GHC],
                 F_BM_default=1)        
         RC.set_init_conc(**R_init_conds)
     
         sysC = System('sysC', path=(RC,))
         sysC.set_dynamic_tracker(RC, bgC, effC)
+        add_strm_iitm(sysC)
+        add_TEA_LCA(sysC, discount_rate, lifetime)
         systems.append(sysC)
         
     if 'D' in which:
         flowsheet_D = flowsheet_D or qs.Flowsheet('D')
         qs.main_flowsheet.set_flowsheet(flowsheet_D)
         
         infD = brewery_ww.copy('BreweryWW_D')
@@ -362,31 +380,33 @@
         bghD = WasteStream('Biogas_hsp_D', phase='g')
         bgmD = WasteStream('Biogas_mem_D', phase='g')
 
         ISTD = IST(ID='ISTD')
         GHD = GH(ID='GHD')
         
         RD = AB('RD', ins=infD, outs=(bghD, ''), 
-                V_liq=Vl2, V_gas=Vg2, T=T2, model=adm1,
+                V_liq=Vl3, V_gas=Vg3, T=T3, model=adm1,
                 retain_cmps=biomass_IDs, bead_lifetime=bl,
                 equipment=[ISTD, GHD],
                 F_BM_default=1)
         DMD = DM('DMD', ins=RD-1, outs=(bgmD, effD),
                   F_BM_default=1)
         RD.set_init_conc(**R_init_conds)
     
         sysD = System('sysD', path=(RD, DMD))
         sysD.set_dynamic_tracker(RD, bghD, bgmD, effD)
+        add_strm_iitm(sysD)
+        add_TEA_LCA(sysD, discount_rate, lifetime)
         systems.append(sysD)
     
     return systems
 
 #%%
 if __name__ == '__main__':
     systems = create_systems()
     for sys in systems:
         sys.simulate(
-            t_span=(0,200),
+            t_span=(0,400),
             state_reset_hook='reset_cache',
             method='BDF'
             )
         sys.diagram()
```

### Comparing `exposan-1.2.5/exposan/new_generator/README.rst` & `exposan-1.3.0/exposan/new_generator/README.rst`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/new_generator/__init__.py` & `exposan-1.3.0/exposan/new_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/new_generator/_components.py` & `exposan-1.3.0/exposan/new_generator/_components.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/new_generator/analysis.py` & `exposan-1.3.0/exposan/new_generator/analysis.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/new_generator/country_specific.py` & `exposan-1.3.0/exposan/new_generator/country_specific.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/new_generator/data/impact_indicators.csv` & `exposan-1.3.0/exposan/new_generator/data/impact_indicators.csv`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/new_generator/data/impact_items.xlsx` & `exposan-1.3.0/exposan/new_generator/data/impact_items.xlsx`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/new_generator/models.py` & `exposan-1.3.0/exposan/new_generator/models.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/new_generator/systems.py` & `exposan-1.3.0/exposan/new_generator/systems.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/new_generator/uncertainty.py` & `exposan-1.3.0/exposan/new_generator/uncertainty.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/reclaimer/README.rst` & `exposan-1.3.0/exposan/reclaimer/README.rst`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/reclaimer/__init__.py` & `exposan-1.3.0/exposan/reclaimer/__init__.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/reclaimer/_components.py` & `exposan-1.3.0/exposan/reclaimer/_components.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/reclaimer/country_specific.py` & `exposan-1.3.0/exposan/reclaimer/country_specific.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/reclaimer/data/impact_indicators.csv` & `exposan-1.3.0/exposan/reclaimer/data/impact_indicators.csv`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/reclaimer/data/impact_items.xlsx` & `exposan-1.3.0/exposan/reclaimer/data/impact_items.xlsx`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/reclaimer/models.py` & `exposan-1.3.0/exposan/reclaimer/models.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/reclaimer/systems.py` & `exposan-1.3.0/exposan/reclaimer/systems.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/reclaimer/uncertainty.py` & `exposan-1.3.0/exposan/reclaimer/uncertainty.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan/utils.py` & `exposan-1.3.0/exposan/utils.py`

 * *Files identical despite different names*

### Comparing `exposan-1.2.5/exposan.egg-info/PKG-INFO` & `exposan-1.3.0/exposan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exposan
-Version: 1.2.5
+Version: 1.3.0
 Summary: Exposition of sanitation and resource recovery systems
 Home-page: https://github.com/QSD-Group/EXPOsan
 Author: Quantitative Sustainable Design Group
 Author-email: quantitative.sustainable.design@gmail.com
 License: UIUC
 Project-URL: Homepage, https://qsdsan.com
 Project-URL: Documentation, https://qsdsan.readthedocs.io
```

### Comparing `exposan-1.2.5/exposan.egg-info/SOURCES.txt` & `exposan-1.3.0/exposan.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -69,33 +69,29 @@
 exposan/htl/_process_settings.py
 exposan/htl/_sanunits.py
 exposan/htl/_tea.py
 exposan/htl/models.py
 exposan/htl/systems.py
 exposan/htl/data/impact_indicators.csv
 exposan/htl/data/impact_items.xlsx
+exposan/htl/data/~$impact_items.xlsx
 exposan/interface/README.rst
 exposan/interface/__init__.py
 exposan/interface/system.py
 exposan/metab_mock/__init__.py
 exposan/metab_mock/_milestone_analysis.py
 exposan/metab_mock/hrt_test.py
-exposan/metab_mock/lca.py
-exposan/metab_mock/models.py
+exposan/metab_mock/init_cond_test.py
+exposan/metab_mock/process.py
 exposan/metab_mock/systems.py
+exposan/metab_mock/test_biofilm.py
 exposan/metab_mock/units.py
 exposan/metab_mock/data/CFs.xlsx
 exposan/metab_mock/data/HDPE_pipe_chart.xlsx
-exposan/metab_mock/data/TRACI_indicators.xlsx
-exposan/metab_mock/data/_impact_items.xlsx
 exposan/metab_mock/data/stainless_steel_pipe_chart.xlsx
-exposan/metab_mock/utils/__init__.py
-exposan/metab_mock/utils/dm_lci.py
-exposan/metab_mock/utils/encap_lci.py
-exposan/metab_mock/utils/er_lci.py
 exposan/new_generator/README.rst
 exposan/new_generator/__init__.py
 exposan/new_generator/_components.py
 exposan/new_generator/analysis.py
 exposan/new_generator/country_specific.py
 exposan/new_generator/models.py
 exposan/new_generator/systems.py
@@ -106,8 +102,18 @@
 exposan/reclaimer/__init__.py
 exposan/reclaimer/_components.py
 exposan/reclaimer/country_specific.py
 exposan/reclaimer/models.py
 exposan/reclaimer/systems.py
 exposan/reclaimer/uncertainty.py
 exposan/reclaimer/data/impact_indicators.csv
-exposan/reclaimer/data/impact_items.xlsx
+exposan/reclaimer/data/impact_items.xlsx
+tests/test_adm.py
+tests/test_asm.py
+tests/test_biogenic_refinery.py
+tests/test_bsm1.py
+tests/test_bwaise.py
+tests/test_cas.py
+tests/test_eco_san.py
+tests/test_htl.py
+tests/test_interface.py
+tests/test_reclaimer.py
```

### Comparing `exposan-1.2.5/pytest.ini` & `exposan-1.3.0/pytest.ini`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 	--doctest-continue-on-failure
 	--ignore='setup.py'
 	--ignore='exposan/bwaise/stats_demo.py'
 	--ignore='exposan/bsm1/profile.py'
 	--ignore='exposan/bsm1/test.py'
 	--ignore-glob='exposan/bwaise/comparison/**'
 	--ignore-glob='exposan/htl/analyses/**'
+	--ignore-glob='exposan/metab/utils/**'
 	--ignore-glob='exposan/metab_mock/**'
 	--ignore-glob='exposan/new_generator/**'
 norecursedirs = 
 	build
 	dist
 	.egg-info
 	.cache
```

### Comparing `exposan-1.2.5/setup.py` & `exposan-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 '''
 
 from setuptools import setup
 
 setup(
     name='exposan',
     packages=['exposan'],
-    version='1.2.5',
+    version='1.3.0',
     license='UIUC',
     author='Quantitative Sustainable Design Group',
     author_email='quantitative.sustainable.design@gmail.com',
     description='Exposition of sanitation and resource recovery systems',
     long_description=open('README.rst', encoding='utf-8').read(),
     url='https://github.com/QSD-Group/EXPOsan',
     project_urls={
         'Homepage': 'https://qsdsan.com',
         'Documentation': 'https://qsdsan.readthedocs.io',
         'Repository': 'https://github.com/QSD-Group/EXPOsan',
     },
-    install_requires=['qsdsan>=1.2.5',],
+    install_requires=['qsdsan>=1.3.0',],
     package_data=
         {'exposan': [
             'adm/*',
             'adm/data/*',
             'asm/*',
             'asm/data/*',
             'biogenic_refinery/*',
```

