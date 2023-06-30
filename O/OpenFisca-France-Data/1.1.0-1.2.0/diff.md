# Comparing `tmp/OpenFisca-France-Data-1.1.0.tar.gz` & `tmp/OpenFisca-France-Data-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-France-Data-1.1.0.tar", last modified: Tue Jun 27 09:25:34 2023, max compression
+gzip compressed data, was "OpenFisca-France-Data-1.2.0.tar", last modified: Fri Jun 30 14:24:02 2023, max compression
```

## Comparing `OpenFisca-France-Data-1.1.0.tar` & `OpenFisca-France-Data-1.2.0.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.033478 OpenFisca-France-Data-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)    10500 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11506 2023-06-27 09:25:34.000000 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4093 2023-06-27 09:25:34.000000 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 09:25:34.000000 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-06-27 09:25:34.000000 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-06-27 09:25:34.000000 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-06-27 09:25:34.000000 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11506 2023-06-27 09:25:34.033478 OpenFisca-France-Data-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10702 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/openfisca_france_data/
--rw-r--r--   0 runner    (1001) docker     (122)     7557 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2998 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/zone_apl/
--rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/base_survey.py
--rw-r--r--   0 runner    (1001) docker     (122)    21046 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/common.py
--rw-r--r--   0 runner    (1001) docker     (122)    23221 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/comparator.py
--rw-r--r--   0 runner    (1001) docker     (122)      996 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.021478 OpenFisca-France-Data-1.1.0/openfisca_france_data/dads/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/openfisca_france_data/dads/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/dads/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/
--rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/run_all.py
--rw-r--r--   0 runner    (1001) docker     (122)     8932 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (122)    21783 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11919 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
--rw-r--r--   0 runner    (1001) docker     (122)    26165 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (122)    13995 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
--rw-r--r--   0 runner    (1001) docker     (122)    36615 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
--rw-r--r--   0 runner    (1001) docker     (122)     8399 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
--rw-r--r--   0 runner    (1001) docker     (122)    13216 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py
--rw-r--r--   0 runner    (1001) docker     (122)     1536 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/old/
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/old/aggregates.py
--rw-r--r--   0 runner    (1001) docker     (122)    19211 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/old/datatable.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4388 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)     7108 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)     6660 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15394 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (122)    25444 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
--rw-r--r--   0 runner    (1001) docker     (122)    45059 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
--rw-r--r--   0 runner    (1001) docker     (122)    35127 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
--rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/test_case_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.021478 OpenFisca-France-Data-1.1.0/openfisca_france_data/felin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/felin/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/felin/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      541 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/calage.py
--rw-r--r--   0 runner    (1001) docker     (122)    11373 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/id_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/survey_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/reforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12440 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/reforms/inversion_directe_salaires.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/scripts/build_input_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/smic.py
--rw-r--r--   0 runner    (1001) docker     (122)     7052 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)    15060 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-06-27 09:25:34.033478 OpenFisca-France-Data-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.033478 OpenFisca-France-Data-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.021478 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.033478 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/
--rw-r--r--   0 runner    (1001) docker     (122)     2466 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_af.py
--rw-r--r--   0 runner    (1001) docker     (122)     8242 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_al.py
--rw-r--r--   0 runner    (1001) docker     (122)    10685 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_impot_revenu.py
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_inflation.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_input_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_pivot_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_rebuild_input_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_salaire_imposable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.033478 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/unit/
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/unit/test_get_survey_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/test_fake_survey_simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/test_get_baremes_salarie.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.681681 OpenFisca-France-Data-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    10720 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.661681 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11506 2023-06-30 14:24:02.000000 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4093 2023-06-30 14:24:02.000000 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 14:24:02.000000 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-06-30 14:24:02.000000 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-06-30 14:24:02.000000 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-06-30 14:24:02.000000 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11506 2023-06-30 14:24:02.681681 OpenFisca-France-Data-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10702 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.661681 OpenFisca-France-Data-1.2.0/openfisca_france_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     7682 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4356 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.665681 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.665681 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.665681 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/base_survey.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21046 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23193 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      996 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.657681 OpenFisca-France-Data-1.2.0/openfisca_france_data/dads/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.665681 OpenFisca-France-Data-1.2.0/openfisca_france_data/dads/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/dads/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.665681 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.669681 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8932 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21783 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11919 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26165 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13995 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36615 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8399 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13216 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1536 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.669681 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/old/
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/old/aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19211 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/old/datatable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.669681 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7108 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.673681 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)     6660 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15394 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25444 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45059 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35127 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/test_case_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.657681 OpenFisca-France-Data-1.2.0/openfisca_france_data/felin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.673681 OpenFisca-France-Data-1.2.0/openfisca_france_data/felin/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/felin/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.673681 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      541 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/calage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11373 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/id_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/survey_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.673681 OpenFisca-France-Data-1.2.0/openfisca_france_data/reforms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12440 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/reforms/inversion_directe_salaires.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.677681 OpenFisca-France-Data-1.2.0/openfisca_france_data/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/scripts/build_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/smic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7052 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15060 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-06-30 14:24:02.681681 OpenFisca-France-Data-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.677681 OpenFisca-France-Data-1.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.657681 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.681681 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)     2466 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_af.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8456 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_al.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10685 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_impot_revenu.py
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_input_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_pivot_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_rebuild_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_salaire_imposable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.681681 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/unit/test_get_survey_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/test_fake_survey_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/test_get_baremes_salarie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/test_misc.py
```

### Comparing `OpenFisca-France-Data-1.1.0/CHANGELOG.md` & `OpenFisca-France-Data-1.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Changelog
 
-# 1.1.0 [#225](https://github.com/openfisca/openfisca-france-data/pull/225)
+# 1.2.0 [#226](https://github.com/openfisca/openfisca-france-data/pull/226)
+* Technical changes
+- Adapte le comparator pour permettre de changer les agrégats cibles.
+- Ajoute les agrégats de la note de validation d'INES
 
+# 1.1.0 [#225](https://github.com/openfisca/openfisca-france-data/pull/225)
 
 * Technical changes
 - Ajoute des variables concernant le calcul des aides au logement, des non salariés et du handicap dans le builder de openfisca-france-data
 
-
-
 # 1.0.0 [#224](https://github.com/openfisca/openfisca-france-data/pull/224)
 
 * Breaking changes
 - dans model/common.py/salaire_brut:
   - Retire rev_microsocial
 
 - Détails
```

### Comparing `OpenFisca-France-Data-1.1.0/CONTRIBUTING.md` & `OpenFisca-France-Data-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/LICENSE` & `OpenFisca-France-Data-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/PKG-INFO` & `OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 1.1.0
+Version: 1.2.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/SOURCES.txt` & `OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/PKG-INFO` & `OpenFisca-France-Data-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 1.1.0
+Version: 1.2.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-France-Data-1.1.0/README.md` & `OpenFisca-France-Data-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/__init__.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,57 +148,61 @@
 openfisca_france_tax_benefit_system = openfisca_france.FranceTaxBenefitSystem()
 # The existence of either CountryTaxBenefitSystem or country_tax_benefit_system is mandatory
 france_data_tax_benefit_system = openfisca_france_data(openfisca_france_tax_benefit_system)
 
 CountryTaxBenefitSystem = lambda: france_data_tax_benefit_system  # noqa analysis:ignore
 
 AGGREGATES_DEFAULT_VARS = [
-    'cotisations_non_contributives',
+    "cotisation_salariales",
+    #"cotisations_employeur",
+    "cotisation_non_salarie",
     "salaire_brut",
     "retraite_brute",
     "chomage_brut",
     "salaire_imposable",
     "retraite_imposable",
     "chomage_imposable",
     "csg_salaire",
     "csg_non_salarie",
     "csg_remplacement",
     "csg_revenus_capital",
     'csg',
     'crds',
     'impot_revenu',
-    "taxe_habitation",
-    'ppe',
-    'ppe_brute',
+    'irpp',
+    'prelevement_forfaitaire_unique_ir',
+    'prelevement_forfaitaire_liberatoire',
+    'taxe_habitation',
+    #'ppe',
+    #'ppe_brute',
     'af',
     'af_base',
     'af_majoration',
     'af_allocation_forfaitaire',
     'cf',
     'paje_base',
     'paje_naissance',
-    'paje_clca',
+    'paje_prepare',
     'paje_cmg',
     'ars',
-    'aeeh',
+    #'aeeh',
     'asf',
     'aspa',
-    # 'minimum_vieillesse',
     'aah',
     'caah',
     'rsa',
-    'rsa_activite',
-    'aefa',
-    'api',
-    # 'majo_rsa',
-    'psa',
+    'ppa',
+    #'aefa',
+    #'api',
+    #'psa',
     'aides_logement',
     'alf',
     'als',
     'apl',
+    #'garantie_jeunes'
     ]
 #  ajouter csgd pour le calcul des agrégats erfs
 #  ajouter rmi pour le calcul des agrégats erfs
 
 
 COUNTRY_DIR = os.path.dirname(os.path.abspath(__file__))
 DATA_DIR = os.path.join(
```

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/aggregates.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/aggregates.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import collections
-from datetime import datetime
 import logging
-import os
+import json
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import pkg_resources
 
 
@@ -28,53 +27,84 @@
         ('actual_beneficiaries', "Bénéficiaires\nréels\n(milliers)"),
         ('amount_absolute_difference', "Diff. absolue\nDépenses\n(millions d'€)"),
         ('beneficiaries_absolute_difference', "Diff absolue\nBénéficiaires\n(milliers)"),
         ('amount_relative_difference', "Diff. relative\nDépenses"),
         ('beneficiaries_relative_difference', "Diff. relative\nBénéficiaires"),
         ))
     aggregate_variables = AGGREGATES_DEFAULT_VARS
+    target_source = None
+
+    def __init__(self, survey_scenario = None, target_source = None):
+        super().__init__(survey_scenario = survey_scenario)
+        self.target_source = target_source
 
     def load_actual_data(self, year = None):
+        target_source = self.target_source
+        assert target_source in ["ines", "taxipp"], "les options possible pour source_cible sont ines ou taxipp"
         assert year is not None
-        taxipp_aggregates_file = Path(
-            pkg_resources.get_distribution("openfisca-france-data").location,
-            "openfisca_france_data",
-            "assets",
-            "agregats_tests_taxipp_2_0.xlsx"
-            )
-        df = (
-            pd.read_excel(
-                taxipp_aggregates_file,
-                # "https://gitlab.com/ipp/partage-public-ipp/taxipp/-/blob/master/simulation/assets/agregats_tests_taxipp_2_0.xlsx",
-                # engine = 'openpyxl'
+
+        if target_source == "taxipp":
+            taxipp_aggregates_file = Path(
+                pkg_resources.get_distribution("openfisca-france_data").location,
+                "openfisca_france_data",
+                "assets",
+                "aggregats",
+                "taxipp",
+                "agregats_tests_taxipp_2_0.xlsx"
+                )
+            df = (
+                pd.read_excel(
+                    taxipp_aggregates_file,
+                    # "https://gitlab.com/ipp/partage-public-ipp/taxipp/-/blob/master/simulation/assets/agregats_tests_taxipp_2_0.xlsx",
+                    # engine = 'openpyxl'
+                    )
+                .rename(columns = str.lower)
+                .rename(columns = {"unnamed: 0": "description"})
+                .dropna(subset = ["annee 2019", "annee 2018", "annee 2017", "annee 2016"], how = "all")
+                )
+            if f"annee {year}" not in df:
+                return
+
+            df = (
+                df[["variable_openfisca", f"annee {year}"]]
+                .dropna()
+                .rename(columns = {
+                    "variable_openfisca": "variable",
+                    f"annee {year}": year,
+                    })
                 )
-            .rename(columns = str.lower)
-            .rename(columns = {"unnamed: 0": "description"})
-            .dropna(subset = ["annee 2019", "annee 2018", "annee 2017", "annee 2016"], how = "all")
-            )
-        if f"annee {year}" not in df:
-            return
-
-        df = (
-            df[["variable_openfisca", f"annee {year}"]]
-            .dropna()
-            .rename(columns = {
-                "variable_openfisca": "variable",
-                f"annee {year}": year,
-                })
-            )
-
-        beneficiaries = (
-            df.loc[df.variable.str.startswith("nombre")]
-            .set_index("variable")
-            .rename(index = lambda x : x.replace("nombre_", ""))
-            .rename(columns = {year: "actual_beneficiaries"})
-            ) / self.beneficiaries_unit
-
-        amounts = (
-            df.loc[~df.variable.str.startswith("nombre")]
-            .set_index("variable")
-            .rename(columns = {year: "actual_amount"})
-            ) / self.amount_unit
 
-        result = amounts.merge(beneficiaries, on = "variable", how = "outer").drop("PAS SIMULE")
+            beneficiaries = (
+                df.loc[df.variable.str.startswith("nombre")]
+                .set_index("variable")
+                .rename(index = lambda x : x.replace("nombre_", ""))
+                .rename(columns = {year: "actual_beneficiaries"})
+                ) / self.beneficiaries_unit
+
+            amounts = (
+                df.loc[~df.variable.str.startswith("nombre")]
+                .set_index("variable")
+                .rename(columns = {year: "actual_amount"})
+                ) / self.amount_unit
+
+            result = amounts.merge(beneficiaries, on = "variable", how = "outer").drop("PAS SIMULE")
+
+        elif target_source == "ines":
+            ines_aggregates_file = Path(
+                pkg_resources.get_distribution("openfisca-france_data").location,
+                "openfisca_france_data",
+                "assets",
+                "aggregats",
+                "ines",
+                f"ines_{year}.json"
+                )
+
+            with open(ines_aggregates_file, 'r') as f:
+                data = json.load(f)
+
+            result = pd.DataFrame(data['data']).drop('notes', axis = 1)
+            result['actual_beneficiaries'] = result. actual_beneficiaries / self.beneficiaries_unit
+            result['actual_amount'] = result. actual_amount / self.amount_unit
+
+            result = result[["variable","actual_amount","actual_beneficiaries"]].set_index("variable")
+
         return result
```

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/base_survey.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/base_survey.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/common.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/common.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/comparator.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/comparator.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,14 +300,15 @@
 
 class AbstractComparator(object):
     name = None
     default_target_variables = None
     filter_expr_by_label = None
     period = None
     messages = list()
+    survey_name = None
 
     def get_name(self):
         return self.name + "_" + str(self.period)
 
     def get_test_dataframes(self, rebuild = False, noindivs = None):
         start_time = datetime.datetime.now()
         if not rebuild:
@@ -429,16 +430,15 @@
 
         except Exception as error:
             if debug:
                 print(error)
                 pdb.post_mortem(sys.exc_info()[2])
             raise error
 
-    def compute_divergence(self, input_dataframe_by_entity, target_dataframe_by_entity, figures_directory,
-            target_variables = None, period = None, summary = False):
+    def compute_divergence(self, input_dataframe_by_entity, target_dataframe_by_entity, figures_directory, target_variables = None, period = None, summary = False):
         """
         Compare openfisca-france-data computation with data targets.
 
         Args:
             input_dataframe_by_period (dict): Input data
             target_dataframe_by_period (dict): Targets to macth
             figures_directory (path): Where to store the figures
@@ -453,16 +453,15 @@
         data = (
             dict(input_dataframe_by_entity = input_dataframe_by_entity)
             if input_dataframe_by_entity is not None
             else None
             )
 
         survey_scenario = self.get_survey_scenario(
-            data = data,
-            survey_name = f'openfisca_erfs_fpr_{period}'
+            data = data
             )
 
         tax_benefit_system = survey_scenario.tax_benefit_system
         markdown_section_by_variable = dict()
         markdown_summary_section_by_variable = dict()
         stats_by_variable = dict()
         result_by_variable = dict()
@@ -558,15 +557,16 @@
                 )
             data_frame.drop(data_frame.index[~selection], inplace = True)
             obs_after = data_frame.noind.nunique()
             log_message = f"Applying filter '{label}': dropping {obs_before - obs_after}, keeping {obs_after} observations."
             log.info(log_message)
             self.messages.append(log_message + "\n")
 
-    def get_survey_scenario(self, data = None, survey_name = None):
+    def get_survey_scenario(self, data = None):
+        survey_name = self.survey_name
         return get_survey_scenario(
             year = str(self.period),
             data = data,
             survey_name = f'openfisca_erfs_fpr_{self.period}' if survey_name is None else survey_name,
             )
 
     def _load_test_dataframes(self, noindivs = None, idents = None):
```

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/config.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/config.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/__init__.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/__init__.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/base.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/base.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/run_all.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/run_all.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/old/aggregates.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/old/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/old/datatable.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/old/datatable.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/scenario.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/comparison.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/comparison.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,32 @@
 
 openfisca_by_erfs_fpr_variables = {
     "chomage_i": "chomage_imposable",
     "ident": "idmen_original",
     "noindiv": "noindiv",
     "rag_i": "rag",
     "retraites_i": "retraite_imposable",  # TODO: CHECk
-    "rev_fonciers_bruts": "f4ba",
+    #"rev_fonciers_bruts": "f4ba",
     "ric_i": "ric",
     "rnc_i": "rnc",
     "salaires_i": "salaire_imposable",
     "logt": "statut_occupation_logement",
     "rev_fonciers_bruts": "revenu_categoriel_foncier_menage",
     "rev_valeurs_mobilieres_bruts": "revenus_capitaux_prelevement_forfaitaire_unique_ir_menage",
     "rev_financier_prelev_lib_imputes": "rev_financier_prelev_lib_imputes_menage",
+    "ppa": "ppa_menage",
+    "nivviem": "niveau_de_vie",
+    "prest_fam_autres": "prestations_familiales_autres_menage",
+    "prest_fam_petite_enfance": "paje_menage",
+    "prest_logement": "aides_logement_menage",
+    "prest_precarite_rsa": "rsa_menage",
+    "prest_precarite_hand": "aah_menage",
+    "prest_precarite_vieil": 'aspa_menage',
+    "revdispm": "revenu_disponible",
+    "nb_uci": "unites_consommation",
     }
 
 
 class ErfsFprtoInputComparator(AbstractComparator):
     name = "erfs_fpr"
     period = None
     default_target_variables = [
```

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/scenario.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/test_case_creation.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/test_case_creation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/model/base.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/model/base.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/model/calage.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/model/calage.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/model/common.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/model/common.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/model/id_variables.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/model/id_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/model/survey_variables.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/model/survey_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/reforms/inversion_directe_salaires.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/reforms/inversion_directe_salaires.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/scripts/build_input_data.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/scripts/build_input_data.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/smic.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/smic.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/surveys.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/openfisca_france_data/utils.py` & `OpenFisca-France-Data-1.2.0/openfisca_france_data/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/setup.cfg` & `OpenFisca-France-Data-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/setup.py` & `OpenFisca-France-Data-1.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name = "OpenFisca-France-Data",
-    version = "1.1.0",
+    version = "1.2.0",
     description = "OpenFisca-France-Data module to work with French survey data",
     long_description = long_description,
     long_description_content_type="text/markdown",
     author = "OpenFisca Team",
     author_email = "contact@openfisca.fr",
     url = "https://github.com/openfisca/openfisca-france-data",
     license = "http://www.fsf.org/licensing/licenses/agpl-3.0.html",
```

### Comparing `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_af.py` & `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_af.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_aggregates.py` & `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_aggregates.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,30 +34,31 @@
         year = year,
         rebuild_input_data = rebuild_input_data,
         use_marginal_tax_rate = use_marginal_tax_rate,
         variation_factor = variation_factor,
         varying_variable = varying_variable,
         survey_name = survey_name,
         )
-    aggregates = Aggregates(survey_scenario = survey_scenario)
+    aggregates_taxipp = Aggregates(survey_scenario = survey_scenario, target_source = 'taxipp')
+    aggregates_ines = Aggregates(survey_scenario = survey_scenario, target_source = 'ines')
 
     if False:
         mtr_rd = survey_scenario.compute_marginal_tax_rate(target_variable = 'revenu_disponible', period = year, use_baseline = True)
         print("Rev Disp: Mean = {}; Zero = {}; Positive = {}; Total = {};".format(mtr_rd.mean(), sum(mtr_rd == 0), sum(mtr_rd > 0), mtr_rd.size))
         np.quantile(mtr_rd, q = np.arange(0, 1.1, .1))
 
         vv1 = survey_scenario.simulation.calculate_add('salaire_de_base', period = year)
         vv2 = survey_scenario._modified_simulation.calculate_add('salaire_de_base', period = year)
 
         tv1 = survey_scenario.simulation.calculate_add('revenu_disponible', period = year)
         tv2 = survey_scenario._modified_simulation.calculate_add('revenu_disponible', period = year)
 
         np.quantile(mtr_rd, q = np.arange(0, 1.1, .1))
 
-    return survey_scenario, aggregates
+    return survey_scenario, aggregates_taxipp.get_data_frame(), aggregates_ines.get_data_frame()
 
 
 def test_erfs_fpr_aggregates_reform():
     """Tests aggregates value with data.
 
     :param year: year of data and simulation to test agregates
     :param reform: optional argument, put an openfisca_france.refoms object, default None
@@ -107,25 +108,27 @@
         except KeyError:
             years = [year]
             log.warning(f"Key 'erfs_fpr' not found in {configfile}, switching back to year {year}")
     else:
         years = [year]
 
     for year in years:
-        survey_scenario, aggregates = test_erfs_fpr_survey_simulation_aggregates(
+        survey_scenario, aggregates_taxipp, aggregates_ines = test_erfs_fpr_survey_simulation_aggregates(
             year = year,
             rebuild_input_data = False,
             use_marginal_tax_rate = True,
             variation_factor = relative_variation,
             varying_variable = varying_variable
             )
 
-        aggregates.to_csv(f'aggregates_erfs_fpr_{year}.csv')
-        print(aggregates.to_markdown())
-        aggregates.to_html(f'aggregates_erfs_fpr_{year}.html')
+        df = pd.concat({
+            "taxipp": aggregates_taxipp,
+            "ines": aggregates_ines,
+            })
+        df.to_csv(f'aggregates_erfs_fpr_{year}.csv')
 
         continue
         survey_scenario._set_used_as_input_variables_by_entity()
 
         mtr_rd = survey_scenario.compute_marginal_tax_rate(target_variable = target_variable, period = year, use_baseline = True)
         print("Rev Disp: Mean = {}; Zero = {}; Positive = {}; Total = {};".format(mtr_rd.mean(), sum(mtr_rd == 0), sum(mtr_rd > 0), mtr_rd.size))
         gc.collect()
```

### Comparing `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_al.py` & `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_al.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py` & `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_impot_revenu.py` & `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_impot_revenu.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_inflation.py` & `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_inflation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_input_variables.py` & `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_input_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_pivot_table.py` & `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_pivot_table.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_rebuild_input_data.py` & `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_rebuild_input_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import logging
-import numpy as np
-
 
 from openfisca_france_data import base_survey
 from openfisca_france_data.erfs_fpr.get_survey_scenario import get_survey_scenario
-from openfisca_france_data.aggregates import FranceAggregates as Aggregates
-
 
 log = logging.getLogger(__name__)
 
 
 def test_rebuild_input_data(year = 2014):
 
     tax_benefit_system = base_survey.france_data_tax_benefit_system
```

### Comparing `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_rsa.py` & `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_rsa.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_salaire_imposable.py` & `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_salaire_imposable.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/unit/test_get_survey_scenario.py` & `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/unit/test_get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/test_aggregate.py` & `OpenFisca-France-Data-1.2.0/tests/test_aggregate.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 
 @pytest.mark.skip(
     reason = "FileNotFoundError: [Errno 2] No such file or directory: '/opt/hostedtoolcache/Python/3.9.9/x64/lib/python3.9/site-packages/openfisca_france_data/assets/agregats_tests_taxipp_2_0.xlsx'",
     )
 def test_erfs_survey_simulation(survey_scenario, fake_input_data, year: int = 2009):
     # On ititialise le survey scenario
-    survey_scenario = survey_scenario(year)
+    survey_scenario = ErfsFprSurveyScenario.create(year)
 
     # On charge les données
     input_data = fake_input_data(year)
 
     # On initialise le survey scenario
     survey_scenario.init_from_data(data = dict(input_data_frame = input_data))
 
     # On calcule les agrégats
-    aggregates = Aggregates(survey_scenario = survey_scenario)
+    aggregates = Aggregates(survey_scenario = survey_scenario, target_source = 'taxipp')
     aggregates.compute_aggregates(use_baseline = False)
     return aggregates.base_data_frame
 
 
 @pytest.mark.skip(
     reason = "FileNotFoundError: [Errno 2] No such file or directory: '/opt/hostedtoolcache/Python/3.9.9/x64/lib/python3.9/site-packages/openfisca_france_data/assets/agregats_tests_taxipp_2_0.xlsx'",
     )
@@ -38,10 +38,10 @@
         )
     # On charge les données
     input_data = fake_input_data(year)
 
     # On initialise le survey scenario
     survey_scenario.init_from_data(data = dict(input_data_frame = input_data))
 
-    aggregates = Aggregates(survey_scenario = survey_scenario)
+    aggregates = Aggregates(survey_scenario = survey_scenario, target_source = 'taxipp')
     base_data_frame = aggregates.compute_aggregates()
     return aggregates, base_data_frame
```

### Comparing `OpenFisca-France-Data-1.1.0/tests/test_calibration.py` & `OpenFisca-France-Data-1.2.0/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/test_fake_survey_simulation.py` & `OpenFisca-France-Data-1.2.0/tests/test_fake_survey_simulation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/test_get_baremes_salarie.py` & `OpenFisca-France-Data-1.2.0/tests/test_get_baremes_salarie.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.1.0/tests/test_misc.py` & `OpenFisca-France-Data-1.2.0/tests/test_misc.py`

 * *Files identical despite different names*

