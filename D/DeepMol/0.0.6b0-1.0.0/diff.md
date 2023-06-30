# Comparing `tmp/DeepMol-0.0.6b0.tar.gz` & `tmp/DeepMol-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepMol-0.0.6b0.tar", last modified: Fri Mar 17 23:40:35 2023, max compression
+gzip compressed data, was "DeepMol-1.0.0.tar", last modified: Fri Jun 30 14:52:19 2023, max compression
```

## Comparing `DeepMol-0.0.6b0.tar` & `DeepMol-1.0.0.tar`

### file list

```diff
@@ -1,96 +1,135 @@
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.686054 DeepMol-0.0.6b0/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1359 2022-06-02 17:02:23.000000 DeepMol-0.0.6b0/LICENSE
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)       30 2023-02-09 09:55:08.000000 DeepMol-0.0.6b0/MANIFEST.in
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1491 2023-03-17 23:40:35.686054 DeepMol-0.0.6b0/PKG-INFO
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    16641 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/README.md
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1066 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/extra-requirements.txt
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      529 2022-11-12 16:26:57.000000 DeepMol-0.0.6b0/pyproject.toml
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      990 2023-03-17 23:40:35.686054 DeepMol-0.0.6b0/setup.cfg
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1091 2023-02-09 09:55:08.000000 DeepMol-0.0.6b0/setup.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.682053 DeepMol-0.0.6b0/src/
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.682053 DeepMol-0.0.6b0/src/DeepMol.egg-info/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1491 2023-03-17 23:40:35.000000 DeepMol-0.0.6b0/src/DeepMol.egg-info/PKG-INFO
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     2746 2023-03-17 23:40:35.000000 DeepMol-0.0.6b0/src/DeepMol.egg-info/SOURCES.txt
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)       58 2023-03-17 23:40:35.000000 DeepMol-0.0.6b0/src/DeepMol.egg-info/dependency_links.txt
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)        1 2022-12-29 11:04:42.000000 DeepMol-0.0.6b0/src/DeepMol.egg-info/not-zip-safe
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1988 2023-03-17 23:40:35.000000 DeepMol-0.0.6b0/src/DeepMol.egg-info/requires.txt
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)        8 2023-03-17 23:40:35.000000 DeepMol-0.0.6b0/src/DeepMol.egg-info/top_level.txt
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.682053 DeepMol-0.0.6b0/src/deepmol/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)        0 2022-11-12 16:26:57.000000 DeepMol-0.0.6b0/src/deepmol/__init__.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.682053 DeepMol-0.0.6b0/src/deepmol/compound_featurization/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1074 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/compound_featurization/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     3635 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/compound_featurization/_utils.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     4239 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/compound_featurization/base_featurizer.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    20108 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/compound_featurization/deepchem_featurizers.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1364 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/compound_featurization/mixed_descriptors.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     4383 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/compound_featurization/mol2vec.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    32735 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/compound_featurization/rdkit_descriptors.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    14636 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/compound_featurization/rdkit_fingerprints.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     2718 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/compound_featurization/similarity_matrix.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.682053 DeepMol-0.0.6b0/src/deepmol/datasets/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)       45 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/datasets/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1841 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/datasets/_utils.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    31927 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/datasets/datasets.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.682053 DeepMol-0.0.6b0/src/deepmol/evaluator/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)       33 2022-11-16 14:07:13.000000 DeepMol-0.0.6b0/src/deepmol/evaluator/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     3868 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/evaluator/evaluator.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.682053 DeepMol-0.0.6b0/src/deepmol/feature_importance/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)       36 2022-11-12 16:26:58.000000 DeepMol-0.0.6b0/src/deepmol/feature_importance/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     6600 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/feature_importance/shap_values.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.682053 DeepMol-0.0.6b0/src/deepmol/feature_selection/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      116 2022-11-16 14:07:13.000000 DeepMol-0.0.6b0/src/deepmol/feature_selection/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    17295 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/feature_selection/base_feature_selector.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.682053 DeepMol-0.0.6b0/src/deepmol/imbalanced_learn/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      115 2022-11-16 14:07:13.000000 DeepMol-0.0.6b0/src/deepmol/imbalanced_learn/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    20445 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/imbalanced_learn/imbalanced_learn.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.682053 DeepMol-0.0.6b0/src/deepmol/loaders/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)       42 2022-11-12 16:26:58.000000 DeepMol-0.0.6b0/src/deepmol/loaders/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1514 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/loaders/_utils.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     8369 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/loaders/loaders.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.682053 DeepMol-0.0.6b0/src/deepmol/loggers/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)       27 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/loggers/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     6544 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/loggers/logger.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.682053 DeepMol-0.0.6b0/src/deepmol/metrics/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)       28 2022-11-12 16:26:58.000000 DeepMol-0.0.6b0/src/deepmol/metrics/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     4225 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/metrics/metrics.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1712 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/metrics/metrics_functions.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.686054 DeepMol-0.0.6b0/src/deepmol/models/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      187 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/models/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      637 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/models/_utils.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     9119 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/models/base_models.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    10630 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/models/deepchem_models.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     5886 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/models/ensembles.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     7479 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/models/keras_models.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     5934 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/models/models.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     6484 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/models/sklearn_models.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.686054 DeepMol-0.0.6b0/src/deepmol/parallelism/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/parallelism/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     3163 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/parallelism/multiprocessing.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.686054 DeepMol-0.0.6b0/src/deepmol/parameter_optimization/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      102 2023-02-09 09:55:18.000000 DeepMol-0.0.6b0/src/deepmol/parameter_optimization/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1959 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/parameter_optimization/_utils.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     8811 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/parameter_optimization/deepchem_hyperparameter_optimization.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    17694 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/parameter_optimization/hyperparameter_optimization.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.686054 DeepMol-0.0.6b0/src/deepmol/scalers/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      202 2022-11-16 14:07:13.000000 DeepMol-0.0.6b0/src/deepmol/scalers/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     4053 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/scalers/base_scaler.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    29992 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/scalers/sklearn_scalers.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.686054 DeepMol-0.0.6b0/src/deepmol/splitters/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      128 2022-11-16 14:07:13.000000 DeepMol-0.0.6b0/src/deepmol/splitters/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     5033 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/splitters/_utils.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    33660 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/splitters/splitters.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.686054 DeepMol-0.0.6b0/src/deepmol/standardizer/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      212 2022-11-16 14:07:13.000000 DeepMol-0.0.6b0/src/deepmol/standardizer/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     7296 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/standardizer/_utils.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      621 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/standardizer/basic_standardizer.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      745 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/standardizer/chembl_standardizer.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     1112 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/standardizer/custom_standardizer.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     2500 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/standardizer/molecular_standardizer.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.686054 DeepMol-0.0.6b0/src/deepmol/unsupervised/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)       91 2022-11-16 14:07:13.000000 DeepMol-0.0.6b0/src/deepmol/unsupervised/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    25809 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/unsupervised/base_unsupervised.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)     4122 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/unsupervised/umap.py
-drwxrwxr-x   0 joao-correia  (1000) joao-correia  (1000)        0 2023-03-17 23:40:35.686054 DeepMol-0.0.6b0/src/deepmol/utils/
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)        0 2022-11-12 16:26:58.000000 DeepMol-0.0.6b0/src/deepmol/utils/__init__.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)      566 2022-11-16 14:07:13.000000 DeepMol-0.0.6b0/src/deepmol/utils/errors.py
--rw-rw-r--   0 joao-correia  (1000) joao-correia  (1000)    25553 2023-03-17 23:35:27.000000 DeepMol-0.0.6b0/src/deepmol/utils/utils.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.775853 DeepMol-1.0.0/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1359 2023-02-22 10:26:07.000000 DeepMol-1.0.0/LICENSE
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)       30 2023-02-22 10:26:07.000000 DeepMol-1.0.0/MANIFEST.in
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1661 2023-06-30 14:52:19.775853 DeepMol-1.0.0/PKG-INFO
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    25482 2023-06-30 14:50:02.000000 DeepMol-1.0.0/README.md
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1426 2023-06-30 14:50:02.000000 DeepMol-1.0.0/extra-requirements.txt
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      529 2023-02-22 10:26:07.000000 DeepMol-1.0.0/pyproject.toml
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1069 2023-06-30 14:52:19.775853 DeepMol-1.0.0/setup.cfg
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1091 2023-02-22 10:26:07.000000 DeepMol-1.0.0/setup.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.767853 DeepMol-1.0.0/src/
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.767853 DeepMol-1.0.0/src/DeepMol.egg-info/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1661 2023-06-30 14:52:19.000000 DeepMol-1.0.0/src/DeepMol.egg-info/PKG-INFO
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     4342 2023-06-30 14:52:19.000000 DeepMol-1.0.0/src/DeepMol.egg-info/SOURCES.txt
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)       58 2023-06-30 14:52:19.000000 DeepMol-1.0.0/src/DeepMol.egg-info/dependency_links.txt
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)        1 2023-06-30 14:14:08.000000 DeepMol-1.0.0/src/DeepMol.egg-info/not-zip-safe
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     2698 2023-06-30 14:52:19.000000 DeepMol-1.0.0/src/DeepMol.egg-info/requires.txt
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)        8 2023-06-30 14:52:19.000000 DeepMol-1.0.0/src/DeepMol.egg-info/top_level.txt
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.767853 DeepMol-1.0.0/src/deepmol/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)       25 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/__init__.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.767853 DeepMol-1.0.0/src/deepmol/base/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      147 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/base/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      255 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/base/_serializer.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1464 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/base/estimator.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     4128 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/base/predictor.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     3666 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/base/transformer.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/compound_featurization/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1187 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/compound_featurization/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     8385 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/compound_featurization/_constants.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     6310 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/compound_featurization/_utils.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     4977 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/compound_featurization/base_featurizer.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    29392 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/compound_featurization/deepchem_featurizers.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1369 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/compound_featurization/mixed_descriptors.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     4383 2023-03-09 10:23:07.000000 DeepMol-1.0.0/src/deepmol/compound_featurization/mol2vec.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     6465 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/compound_featurization/one_hot_encoder.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    33131 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/compound_featurization/rdkit_descriptors.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    28322 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/compound_featurization/rdkit_fingerprints.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     3797 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/compound_featurization/similarity_matrix.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/datasets/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)       45 2023-03-09 10:23:07.000000 DeepMol-1.0.0/src/deepmol/datasets/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1841 2023-03-09 10:23:07.000000 DeepMol-1.0.0/src/deepmol/datasets/_utils.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    34595 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/datasets/datasets.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/evaluator/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)       33 2023-02-22 10:26:08.000000 DeepMol-1.0.0/src/deepmol/evaluator/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     3868 2023-03-15 15:35:06.000000 DeepMol-1.0.0/src/deepmol/evaluator/evaluator.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/feature_importance/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)       36 2023-02-22 10:26:08.000000 DeepMol-1.0.0/src/deepmol/feature_importance/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     2820 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/feature_importance/_utils.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    12680 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/feature_importance/shap_values.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/feature_selection/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      116 2023-02-22 10:26:08.000000 DeepMol-1.0.0/src/deepmol/feature_selection/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    15244 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/feature_selection/base_feature_selector.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/imbalanced_learn/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      115 2023-02-22 10:26:08.000000 DeepMol-1.0.0/src/deepmol/imbalanced_learn/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1922 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/imbalanced_learn/_utils.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    25897 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/imbalanced_learn/imbalanced_learn.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/loaders/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)       42 2023-02-22 10:26:08.000000 DeepMol-1.0.0/src/deepmol/loaders/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1514 2023-02-27 10:08:46.000000 DeepMol-1.0.0/src/deepmol/loaders/_utils.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     8369 2023-03-09 10:23:07.000000 DeepMol-1.0.0/src/deepmol/loaders/loaders.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/loggers/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)       27 2023-03-09 10:23:07.000000 DeepMol-1.0.0/src/deepmol/loggers/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     6774 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/loggers/logger.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/metrics/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)       28 2023-02-22 10:26:08.000000 DeepMol-1.0.0/src/deepmol/metrics/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     4486 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/metrics/metrics.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1712 2023-02-28 17:05:11.000000 DeepMol-1.0.0/src/deepmol/metrics/metrics_functions.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/models/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      187 2023-03-09 10:23:07.000000 DeepMol-1.0.0/src/deepmol/models/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     6724 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/models/_utils.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     9142 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/models/base_models.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    29034 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/models/deepchem_model_builders.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    15938 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/models/deepchem_models.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     5836 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/models/ensembles.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    21908 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/models/keras_model_builders.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     9835 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/models/keras_models.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     6431 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/models/models.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    89977 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/models/sklearn_model_builders.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     8453 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/models/sklearn_models.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/parallelism/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)        0 2023-02-23 10:57:44.000000 DeepMol-1.0.0/src/deepmol/parallelism/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     3163 2023-02-28 17:05:11.000000 DeepMol-1.0.0/src/deepmol/parallelism/multiprocessing.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/parameter_optimization/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      102 2023-02-22 10:26:08.000000 DeepMol-1.0.0/src/deepmol/parameter_optimization/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1959 2023-03-14 08:50:09.000000 DeepMol-1.0.0/src/deepmol/parameter_optimization/_utils.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     3549 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/parameter_optimization/base_hyperparameter_optimization.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     9283 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/parameter_optimization/deepchem_hyperparameter_optimization.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    14071 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/parameter_optimization/hyperparameter_optimization.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.771854 DeepMol-1.0.0/src/deepmol/pipeline/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)       31 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      693 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline/_utils.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    12836 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline/pipeline.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.775853 DeepMol-1.0.0/src/deepmol/pipeline_optimization/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)       56 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline_optimization/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    34225 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline_optimization/_deepchem_models_objectives.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     5429 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline_optimization/_feature_selector_objectives.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     2635 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline_optimization/_featurizer_objectives.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    22379 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline_optimization/_keras_model_objectives.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     4978 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline_optimization/_scaler_objectives.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    58937 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline_optimization/_sklearn_model_objectives.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1227 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline_optimization/_standardizer_objectives.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    19089 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline_optimization/_utils.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     3680 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline_optimization/objective_wrapper.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     6778 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/pipeline_optimization/pipeline_optimization.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.775853 DeepMol-1.0.0/src/deepmol/scalers/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      202 2023-02-22 10:26:08.000000 DeepMol-1.0.0/src/deepmol/scalers/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     2845 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/scalers/base_scaler.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    11705 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/scalers/sklearn_scalers.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.775853 DeepMol-1.0.0/src/deepmol/splitters/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      189 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/splitters/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     5033 2023-03-09 10:23:07.000000 DeepMol-1.0.0/src/deepmol/splitters/_utils.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     3611 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/splitters/multitask_splitter.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    33744 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/splitters/splitters.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.775853 DeepMol-1.0.0/src/deepmol/standardizer/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      212 2023-02-22 10:26:08.000000 DeepMol-1.0.0/src/deepmol/standardizer/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     7296 2023-03-09 10:23:07.000000 DeepMol-1.0.0/src/deepmol/standardizer/_utils.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      621 2023-02-27 10:08:46.000000 DeepMol-1.0.0/src/deepmol/standardizer/basic_standardizer.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      745 2023-02-27 10:08:46.000000 DeepMol-1.0.0/src/deepmol/standardizer/chembl_standardizer.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     1112 2023-02-27 10:08:46.000000 DeepMol-1.0.0/src/deepmol/standardizer/custom_standardizer.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     3458 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/standardizer/molecular_standardizer.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.775853 DeepMol-1.0.0/src/deepmol/tokenizers/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      154 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/tokenizers/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      442 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/tokenizers/_utils.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     3294 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/tokenizers/atom_level_smiles_tokenizer.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     4857 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/tokenizers/kmer_smiles_tokenizer.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     2115 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/tokenizers/tokenizer.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.775853 DeepMol-1.0.0/src/deepmol/unsupervised/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)       91 2023-02-22 10:26:08.000000 DeepMol-1.0.0/src/deepmol/unsupervised/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)    28452 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/unsupervised/base_unsupervised.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     4761 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/unsupervised/umap.py
+drwxrwxr-x   0 bisbii    (1000) bisbii    (1000)        0 2023-06-30 14:52:19.775853 DeepMol-1.0.0/src/deepmol/utils/
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)        0 2023-02-22 10:26:08.000000 DeepMol-1.0.0/src/deepmol/utils/__init__.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      180 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/utils/cached_properties.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     2578 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/utils/decorators.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)      566 2023-02-22 10:26:08.000000 DeepMol-1.0.0/src/deepmol/utils/errors.py
+-rw-rw-r--   0 bisbii    (1000) bisbii    (1000)     5448 2023-06-30 14:50:02.000000 DeepMol-1.0.0/src/deepmol/utils/utils.py
```

### Comparing `DeepMol-0.0.6b0/LICENSE` & `DeepMol-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/PKG-INFO` & `DeepMol-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepMol
-Version: 0.0.6b0
+Version: 1.0.0
 Summary: DeepMol: a python-based machine and deep learning framework for drug discovery
 Author: DeepMol Team
 License: BSD 2-Clause License
 Keywords: machine-learning,deep-learning,cheminformatics,drug-discovery
 Platform: unix
 Platform: linux
 Platform: osx
@@ -13,40 +13,46 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
+Provides-Extra: test
+Provides-Extra: preprocessing
 Provides-Extra: deep_learning
 Provides-Extra: rdkit-pypi
-Provides-Extra: preprocessing
 Provides-Extra: machine_learning
-Provides-Extra: test
 Provides-Extra: smilespe
 Provides-Extra: seaborn
 Provides-Extra: joblib
 Provides-Extra: pillow
 Provides-Extra: h5py
+Provides-Extra: cached_property
+Provides-Extra: numpy
+Provides-Extra: dill
 Provides-Extra: shap
 Provides-Extra: gensim
 Provides-Extra: imblearn
 Provides-Extra: umap-learn
 Provides-Extra: kneed
 Provides-Extra: kaleido
 Provides-Extra: plotly
 Provides-Extra: chembl_structure_pipeline
 Provides-Extra: torch
-Provides-Extra: torchvision
-Provides-Extra: torchaudio
 Provides-Extra: dgl
+Provides-Extra: dgllife
 Provides-Extra: deepchem
+Provides-Extra: torch_geometric
 Provides-Extra: tensorflow
+Provides-Extra: tensorflow-probability
 Provides-Extra: boruta
 Provides-Extra: scikit-learn
+Provides-Extra: optuna
+Provides-Extra: scikit-multilearn
 Provides-Extra: pytest
 Provides-Extra: pytest-cov
 Provides-Extra: mypy
 Provides-Extra: flake8
 Provides-Extra: tox
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `DeepMol-0.0.6b0/README.md` & `DeepMol-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,31 +4,36 @@
 DeepMol is a Python-based machine and deep learning framework for drug discovery. 
 It offers a variety of functionalities that enable a smoother approach to many 
 drug discovery and chemoinformatics problems. It uses Tensorflow, Keras, 
 Scikit-learn and DeepChem to build custom ML and DL models or 
 make use of pre-built ones. It uses the RDKit framework to perform 
 operations on molecular data.
 
+More detailed and comprehensive documentation in [DeepMol readthedocs](https://deepmol.readthedocs.io/en/latest/).
+
 ### Table of contents:
 
 - [Requirements](#requirements)
 - [Installation](#installation)
     - [Pip](#pip)
     - [Manually](#manually)
 - [Getting Started](#getting-started)
     - [Load dataset from csv](#load-a-dataset-from-a-csv)
+    - [Load dataset from sdf](#load-a-dataset-from-a-sdf)
     - [Compound Standardization](#compound-standardization)
     - [Compound Featurization](#compound-featurization)
     - [Feature Selection](#feature-selection)
     - [Unsupervised Exploration](#unsupervised-exploration)
     - [Data Split](#data-split)
     - [Build, train and evaluate a model](#build-train-and-evaluate-a-model)
     - [Hyperparameter Optimization](#hyperparameter-optimization)
     - [Feature Importance (Shap Values)](#feature-importance-shap-values)
     - [Unbalanced Datasets](#unbalanced-datasets)
+    - [Pipelines](#pipeline)
+    - [Pipeline Optimization](#pipeline-optimization)
 - [About Us](#about-us)
 - [Citing DeepMol](#citing-deepmol)
   - [Related Publications](#publications-using-deepmol)
 - [License](#licensing)
 
 
 ## Requirements
@@ -114,19 +119,14 @@
 
 The DeepMol framework is still under development, and it is currently at a 
 pre-release version. New models and features will be added in the future.
 
 
 ### Load a dataset from a CSV
 
-For now, it is only possible to load data directly from CSV files. Modules to 
-load data from different file types and sources will be implemented in the 
-future. These include JSON, SDF and FASTA files and directly from our 
-databases.
-
 To load data from a CSV it's only required to provide the math and molecules 
 field name. Optionally, it is also possible to provide a field with some ids, 
 the labels fields, features fields, features to keep (useful for instance 
 to select only the features kept after feature selection) and the number of 
 samples to load (by default loads the entire dataset).
 
 ```python
@@ -145,24 +145,47 @@
 
 # print shape of the dataset (molecules, X, y)
 dataset.get_shape()
 
 ((1000,), None, (1000,))
 ```
 
+### Load a dataset from a SDF
+
+If you want to load a dataset from a SDF file with 3D structures, it is only required to provide
+the path to the file. Optionally, it is also possible to provide a field with some ids,
+the labels fields.
+
+```python
+from deepmol.loaders import SDFLoader
+
+# load a dataset from a SDF (required fields: dataset_path)
+loader = SDFLoader(dataset_path='../../data/train_dataset.sdf',
+                   id_field='ids',
+                   labels_fields=['y'],
+                   shard_size=1000,
+                   mode='auto')
+dataset = loader.create_dataset()
+dataset.get_shape()
+
+((1000,), None, (1000,))
+```
+
 ### Compound Standardization
 
 It is possible to standardize the loaded molecules using three option. Using
 a basic standardizer that only does sanitization (Kekulize, check valencies, 
 set aromaticity, conjugation and hybridization). A more complex standardizer can
 be customized by choosing or not to perform specific tasks such as sanitization, 
 remove isotope information, neutralize charges, remove stereochemistry and remove
 smaller fragments. Another possibility is to use the ChEMBL Standardizer.
 
 ```python
+from deepmol.standardizer import BasicStandardizer, CustomStandardizer, ChEMBLStandardizer 
+
 # Option 1: Basic Standardizer
 standardizer = BasicStandardizer().standardize(dataset)
 
 # Option 2: Custom Standardizer
 heavy_standardisation = {
     'REMOVE_ISOTOPE': True,
     'NEUTRALISE_CHARGE': True,
@@ -184,15 +207,15 @@
 Mol2Vec can also be computed. More complex molecular embeddings like the 
 Seq2Seq and transformer-based are in  development and will be added soon.
 
 ```python
 from deepmol.compound_featurization import MorganFingerprint
 
 # Compute morgan fingerprints for molecules in the previous loaded dataset
-MorganFingerprint(radius=2, size=1024).featurize(dataset)
+MorganFingerprint(radius=2, size=1024).featurize(dataset, inplace=True)
 # view the computed features (dataset.X)
 dataset.X
 ```
 
 
 ```python
 #print shape of the dataset to see difference in the X shape
@@ -208,15 +231,15 @@
 KBest, Percentile, Recursive Feature Elimination and selecting features based on 
 importance weights.
 
 ```python
 from deepmol.feature_selection import LowVarianceFS
 
 # Feature Selection to remove features with low variance across molecules
-LowVarianceFS(0.15).select_features(dataset)
+LowVarianceFS(0.15).select_features(dataset, inplace=True)
 
 # print shape of the dataset to see difference in the X shape (fewer features)
 dataset.get_shape()
 
 ((1000,), (1000, 35), (1000,))
 ```
 
@@ -225,15 +248,15 @@
 It is possible to do unsupervised exploration of the datasets using PCA, tSNE,
 KMeans and UMAP.
 
 ```python
 from deepmol.unsupervised import UMAP
 
 ump = UMAP()
-umap_df = ump.run_unsupervised(dataset)
+umap_df = ump.run(dataset)
 ump.plot(umap_df.X, path='umap_output.png')
 ```
 
 ![umap_output](docs/imgs/umap_output.png)
 
 ### Data Split
 
@@ -267,15 +290,15 @@
 implemented allowing evaluation of the models under a common workspace.
 
 #### Scikit-Learn model example
 
 Models can be imported from scikit-learn and wrapped using the SKlearnModel
 module.
 
-Check this **[jupyter notebook](examples/notebooks/RandomForestTest.ipynb)** for a complete example!
+Check this **[jupyter notebook](examples/workshop_bod/featurization.ipynb)** for a complete example!
 
 ```python
 from sklearn.ensemble import RandomForestClassifier
 from deepmol.models.sklearn_models import SklearnModel
 
 # Scikit-Learn Random Forest
 rf = RandomForestClassifier()
@@ -284,19 +307,18 @@
 # model training
 model.fit(train_dataset)
 
 from deepmol.metrics.metrics import Metric
 from deepmol.metrics.metrics_functions import roc_auc_score
 
 # cross validate model on the full dataset
-model.cross_validate(dataset, Metric(roc_auc_score), folds=3)
+best_model, train_score_best_model, test_score_best_model, \
+            train_scores, test_scores, average_train_score, average_test_score = model.cross_validate(dataset, Metric(roc_auc_score), folds=3)
 ```
 
-![cross_validation_output](docs/imgs/cross_validation_output.png)
-
 ```python
 from sklearn.metrics import precision_score, accuracy_score, confusion_matrix, classification_report
 
 #evaluate the model using different metrics
 metrics = [Metric(roc_auc_score), Metric(precision_score), Metric(accuracy_score), Metric(confusion_matrix), 
            Metric(classification_report)]
 
@@ -307,23 +329,31 @@
 # evaluate the model on training data
 print('Validation Dataset: ')
 valid_score = model.evaluate(valid_dataset, metrics)
 
 # evaluate the model on training data
 print('Test Dataset: ')
 test_score = model.evaluate(test_dataset, metrics)
+model.save('my_model')
 ```
 
 ![evaluate_output](docs/imgs/evaluate_output.png)
 
+Loading and saving models was never so easy!
+
+```python
+model = SklearnModel.load('my_model')
+model.evaluate(test_dataset, metrics)
+```
+
 #### Keras model example
 
 Example of how to build and wrap a keras model using the KerasModel module.
 
-Check this **[jupyter notebook](examples/notebooks/test_keras.ipynb)** for a complete example!
+Check this **[jupyter notebook](examples/workshop_bod/models.ipynb)** for a complete example!
 
 ```python
 from tensorflow.keras.models import Sequential
 from tensorflow.keras.layers import Dense, Dropout
 from deepmol.metrics.metrics import Metric
 
 input_dim = train_dataset.X.shape[1]
@@ -356,22 +386,30 @@
            Metric(precision_score),
            Metric(accuracy_score),
            Metric(confusion_matrix),
            Metric(classification_report)]
 
 print('Training set score:', model.evaluate(train_dataset, metrics))
 print('Test set score:', model.evaluate(test_dataset, metrics))
+
+model.save('my_model')
 ```
 
+Loading and saving models was never so easy!
+
+```python
+model = KerasModel.load('my_model')
+model.evaluate(test_dataset, metrics)
+```
 
 #### DeepChem model example
 
 Using DeepChem models:
 
-Check this **[jupyter notebook](examples/notebooks/deepchem_test.ipynb)** for a complete example!
+Check this **[jupyter notebook](examples/workshop_bod/models.ipynb)** for a complete example!
 
 ```python
 from deepmol.compound_featurization import WeaveFeat
 from deepchem.models import MPNNModel
 from deepmol.models.deepchem_models import DeepChemModel
 from deepmol.metrics.metrics import Metric
 from deepmol.splitters.splitters import SingletaskStratifiedSplitter
@@ -389,119 +427,293 @@
 # Evaluation
 metrics = [Metric(roc_auc_score), Metric(precision_score), Metric(accuracy_score)]
 print('Training Dataset: ')
 train_score = model_mpnn.evaluate(train_dataset, metrics)
 print('Valid Dataset: ')
 valid_score = model_mpnn.evaluate(valid_dataset, metrics)
 print('Test Dataset: ')
-test_score = model_mpnn.evaluate(test_dataset, metrics)    
+test_score = model_mpnn.evaluate(test_dataset, metrics)
+model_mpnn.save("my_model")
+```
+Loading and saving models was never so easy!
+
+```python
+model = DeepChemModel.load('my_model')
+model.evaluate(test_dataset, metrics)
 ```
 
+
 ### Hyperparameter Optimization
 
 Grid and randomized hyperparameter optimization is provided using cross-validation
-or a held-out validation set.
+or a held-out validation set. For a more detailed example check this 
+**[jupyter notebook](examples/workshop_bod/hyperparameter_optimization.ipynb)**.
 
 ```python
-from deepmol.parameter_optimization.hyperparameter_optimization import HyperparameterOptimizerValidation,
-
-HyperparameterOptimizerCV
-
-# Hyperparameter Optimization (using the above created keras model)
-optimizer = HyperparameterOptimizerValidation(create_model)
-
-params_dict = {'optimizer': ['adam', 'rmsprop'],
-               'dropout': [0.2, 0.4, 0.5]}
+from deepmol.parameter_optimization.hyperparameter_optimization import HyperparameterOptimizerValidation
 
-best_model, best_hyperparams, all_results = optimizer.hyperparameter_search(params_dict, train_dataset,
-                                                                            valid_dataset, Metric(roc_auc_score))
+from tensorflow.keras.optimizers import Adam
+from tensorflow.keras.layers import Dropout
+from tensorflow import keras
+from tensorflow.keras import layers
+
+def create_model(input_dim, optimizer='adam', dropout=0.5):
+    # create model
+    inputs = layers.Input(shape=input_dim)
+
+    # Define the shared layers
+    shared_layer_1 = layers.Dense(64, activation="relu")
+    dropout_1 = Dropout(dropout)
+    shared_layer_2 = layers.Dense(32, activation="relu")
+
+    # Define the shared layers for the inputs
+    x = shared_layer_1(inputs)
+    x = dropout_1(x)
+    x = shared_layer_2(x)
+
+    task_output = layers.Dense(1, activation="sigmoid")(x)
+
+    # Define the model that outputs the predictions for each task
+    model = keras.Model(inputs=inputs, outputs=task_output)
+    # Compile the model with different loss functions and metrics for each task
+    model.compile(
+        optimizer=optimizer, loss="binary_crossentropy", metrics=["accuracy"]
+    )
+    return model
+
+optimizer = HyperparameterOptimizerValidation(create_model,
+                                              metric=Metric(accuracy_score),
+                                              maximize_metric=True,
+                                              n_iter_search=2,
+                                              params_dict=params_dict_dense,
+                                              model_type="keras")
+params_dict_dense = {
+                   "input_dim": [train_dataset.X.shape[1]],
+                   "dropout": [0.5, 0.6, 0.7],
+                   "optimizer": [Adam]
+                   }
 
-print(best_hyperparams)
-print(best_model)
+best_dnn, best_hyperparams, all_results = optimizer.fit(train_dataset=train_dataset,
+                                                        valid_dataset=valid_dataset)
 
 # Evaluate model
 best_model.evaluate(test_dataset, metrics)
 ```
 
 ### Feature Importance (Shap Values)
 
 Explain the output of a machine learning model can be done using SHAP (SHapley 
-Additive exPlanations) package. The features that most influenced (positively or
+Additive exPlanations) package. For a more detailed description you can check out this **[jupyter notebook](examples/workshop_bod/model_explainability.ipynb)**.
+The features that most influenced (positively or
 negatively) a certain prediction can be calculated and visualized in different 
 ways:
 
 ```python
 from deepmol.feature_importance import ShapValues
 
-shap_calc = ShapValues(test_dataset, model)
-shap_calc.computePermutationShap()
+# compute shap values
+shap_calc = ShapValues()
+shap_calc.fit(train_dataset, model)
+shap_calc.beeswarm_plot()
 ```
 
 ![calc_shap_output](docs/imgs/calc_shap_output.png)
 
 ```python
-shap_calc.plotSampleExplanation(index=1, plot_type='waterfall')
+shap_calc.sample_explanation_plot(index=1, plot_type='waterfall')
 ```
 
 ![sample_explanation_output](docs/imgs/sample_explanation_output.png)
 
 ```python
-shap_calc.plotFeatureExplanation(index=115)
+shap_calc.feature_explanation_plot(1)
 ```
 
 ![feature_explanation_output](docs/imgs/feature_explanation_output.png)
 
 #### Draw relevant features
 
 It is possible to plot the ON bits (or some of them) in a molecule for MACCS Keys,
 Morgan and RDK Fingeprints. IT is also possible to draw those bits on the 
 respective molecule. This can be allied with the Shap Values calculation to 
 highlight the zone of the molecule that most contributed to a certain prediction,
 for instance, the substructure in the molecule that most contributed to its 
 classification as an active or inactive molecule against a receptor.
 
 ```python
-from deepmol.utils.utils import draw_MACCS_Pattern
+from deepmol.compound_featurization import MACCSkeysFingerprint
 
 patt_number = 54
 mol_number = 1
 
 prediction = model.predict(test_dataset)[mol_number]
 actual_value = test_dataset.y[mol_number]
 print('Prediction: ', prediction)
 print('Actual Value: ', actual_value)
 smi = test_dataset.mols[mol_number]
 
-draw_MACCS_Pattern(smi, patt_number)
+maccs_keys = MACCSkeysFingerprint()
+
+maccs_keys.draw_bit(smi, patt_number)
 ```
 
 ![draw_maccs_output](docs/imgs/draw_maccs_output.png)
 
 
 ### Unbalanced Datasets
 
 Multiple methods to deal with unbalanced datasets can be used to do oversampling,
 under-sampling or a mixture of both (Random, SMOTE, SMOTEENN, SMOTETomek and 
-ClusterCentroids).
+ClusterCentroids). For a more detailed example check this **[jupyter notebook](examples/workshop_bod/imbalanced_learn.ipynb)**.
 
 ```python
 from deepmol.imbalanced_learn.imbalanced_learn import SMOTEENN
 
 train_dataset = SMOTEENN().sample(train_dataset)
 ```
 
 
-## About Us
+### Pipeline
+
+DeepMol provides a pipeline to perform almost all the steps above in a sequence without
+having to worry about the details of each step. The pipeline can be used to perform
+a prediction pipeline (last step is a data predictor) or a data transformation pipeline
+(all steps are data transformers). Transformers must implement the _fit and _transform
+methods and predictors must implement the _fit and _predict methods.
+
+```python
+from deepmol.loaders import CSVLoader
+from tensorflow.keras import Sequential
+from tensorflow.keras.layers import Dense
+from deepmol.models import KerasModel
+from deepmol.standardizer import BasicStandardizer
+from deepmol.compound_featurization import MorganFingerprint
+from deepmol.scalers import StandardScaler
+from deepmol.feature_selection import KbestFS
+from deepmol.pipeline import Pipeline
+from deepmol.metrics import Metric
+from sklearn.metrics import accuracy_score
+
+loader_train = CSVLoader('data_train_path.csv',
+                         smiles_field='Smiles',
+                         labels_fields=['Class'])
+train_dataset = loader_train.create_dataset(sep=";")
+
+loader_test = CSVLoader('data_test_path.csv',
+                        smiles_field='Smiles',
+                        labels_fields=['Class'])
+test_dataset = loader_train.create_dataset(sep=";")
+        
+def basic_classification_model_builder(input_shape):
+  model = Sequential()
+  model.add(Dense(10, input_shape=input_shape, activation='relu'))
+  model.add(Dense(1, activation='sigmoid'))
+  model.compile(loss='binary_crossentropy', optimizer='adam', metrics=['accuracy'])
+  return model
+
+keras_model = KerasModel(model_builder=basic_classification_model_builder, epochs=2, input_shape=(1024,))
+        
+steps = [('standardizer', BasicStandardizer()),
+         ('featurizer', MorganFingerprint(size=1024)),
+         ('scaler', StandardScaler()),
+         ('feature_selector', KbestFS(k=10)),
+         ('model', keras_model)]
+
+pipeline = Pipeline(steps=steps, path='test_pipeline/')
+
+pipeline.fit_transform(train_dataset)
+
+predictions = pipeline.predict(test_dataset)
+pipeline.evaluate(test_dataset, [Metric(accuracy_score)])
+
+# save pipeline
+pipeline.save()
+
+# load pipeline
+pipeline = Pipeline.load('test_pipeline/')
+``` 
+
+### Pipeline optimization
+```python
+from sklearn.ensemble import RandomForestClassifier
+from sklearn.metrics import accuracy_score
+from sklearn.svm import SVC
+
+from deepmol.loaders import CSVLoader
+from deepmol.metrics import Metric
+from deepmol.models import SklearnModel
+from deepmol.pipeline_optimization import PipelineOptimization
+from deepmol.splitters import RandomSplitter
+
+# DEFINE THE OBJECTIVE FUNCTION
+def objective(trial):
+    model = trial.suggest_categorical('model', ['RandomForestClassifier', 'SVC'])
+    if model == 'RandomForestClassifier':
+        n_estimators = trial.suggest_int('model__n_estimators', 10, 100, step=10)
+        model = RandomForestClassifier(n_estimators=n_estimators)
+    elif model == 'SVC':
+        kernel = trial.suggest_categorical('model__kernel', ['linear', 'poly', 'rbf', 'sigmoid'])
+        model = SVC(kernel=kernel)
+    model = SklearnModel(model=model, model_dir='model')
+    steps = [('model', model)]
+    return steps
+ 
+# LOAD THE DATA   
+loader = CSVLoader('data_path...',
+                   smiles_field='mols',
+                   id_field='ids',
+                   labels_fields=['y'],
+                   features_fields=['f1', 'f2', 'f3', '...'],
+                   mode='classification')
+dataset_descriptors = loader.create_dataset(sep=",")
+   
+# OPTIMIZE THE PIPELINE 
+po = PipelineOptimization(direction='maximize', study_name='test_predictor_pipeline')
+metric = Metric(accuracy_score)
+train, test = RandomSplitter().train_test_split(dataset_descriptors, seed=123)
+po.optimize(train_dataset=train, test_dataset=test, objective_steps=objective, 
+            metric=metric, n_trials=5, save_top_n=3)
+```
+
+### About Us
 
 DeepMol is managed by a team of contributors from the BioSystems group 
 at the Centre of Biological Engineering, University of Minho.
 
 This research was financed by Portuguese Funds through FCT – Fundação para 
 a Ciência e a Tecnologia.
 
+#### Contributors
+
+João Correia - PhD student at the University of Minho (UMinho) and 
+researcher at the Centre of Biological Engineering (CEB), Braga, Portugal. João Correia is a PhD student in 
+Bioinformatics currently working with machine learning methods applied to the discovery of new chemical compounds 
+and reactions. [GitHub](https://github.com/jcorreia11), [LinkedIn](https://www.linkedin.com/in/joaocorreia95/), 
+[Research Gate](https://www.researchgate.net/profile/Joao-Correia-70)
+
+João Capela - PhD student at the University of Minho (UMinho) and 
+researcher at the Centre of Biological Engineering (CEB), Braga, Portugal. João Capela is a 
+PhD student in Bioinformatics currently working with machine learning methods to expose plant secondary metabolism.
+[GitHub](https://github.com/jcapels), [LinkedIn](https://www.linkedin.com/in/joaocapels/), 
+[ResearchGate](https://www.researchgate.net/profile/Joao-Capela-4)
+
+Vitor Pereira - Postdoctoral researcher at the University of Minho (UMinho) and Centre of Biological Engineering (CEB),
+Braga, Portugal. Vitor Pereira is a postdoctoral researcher in Bioinformatics currently working with machine learning
+to produce new chemical compounds and proteins. 
+[GitHub](https://github.com/vmspereira), [LinkedIn](https://www.linkedin.com/in/v%C3%ADtor-s%C3%A1-pereira/),
+[ResearchGate](https://www.researchgate.net/profile/Vitor-Pereira-9)
+
+Miguel Rocha - Associate Professor in Artificial Intelligence and Bioinformatics, 
+being the founder of the MSc in Bioinformatics (2007) and its current Director. 
+He is currently the CSO of OmniumAI. He has 20 years of experience in applying AI and data science 
+technologies to biological and biomedical data, both in academic (with numerous publications) 
+and in industry scenarios.
+[GitHub](https://github.com/miguelfrocha), [LinkedIn](https://www.linkedin.com/in/miguelprocha/),
+[ResearchGate](https://www.researchgate.net/profile/Miguel-Rocha-16)
+
 ## Citing DeepMol
 
 Manuscript under preparation.
 
 ### Publications using DeepMol
 
 Baptista D., Correia J., Pereira B., Rocha M. (2022) "A Comparison of Different Compound Representations for Drug Sensitivity Prediction". In: Rocha M., Fdez-Riverola F., Mohamad M.S., Casado-Vara R. (eds) Practical Applications of Computational Biology & Bioinformatics, 15th International Conference (PACBB 2021). PACBB 2021. Lecture Notes in Networks and Systems, vol 325. Springer, Cham. https://doi.org/10.1007/978-3-030-86258-9_15
```

### Comparing `DeepMol-0.0.6b0/extra-requirements.txt` & `DeepMol-1.0.0/extra-requirements.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 rdkit-pypi==2022.9.3: preprocessing, deep_learning, machine_learning, test
 smilespe==0.0.3: preprocessing, deep_learning, machine_learning, test
 seaborn==0.12.0: preprocessing, deep_learning, machine_learning, test
 joblib==1.1.1: preprocessing, deep_learning, machine_learning, test
 pillow==8.4.0: preprocessing, deep_learning, machine_learning, test
 h5py==3.7.0: preprocessing, deep_learning, machine_learning, test
+cached_property==1.5.2: preprocessing, deep_learning, machine_learning, test
+numpy==1.23.5: preprocessing, deep_learning, machine_learning, test
+dill==0.3.6: preprocessing, deep_learning, machine_learning, test
 shap==0.41.0: deep_learning, machine_learning
 gensim==4.2.0: preprocessing
 imblearn: preprocessing
 umap-learn==0.5.1: machine_learning
 kneed==0.8.2: machine_learning
 kaleido==0.2.1: machine_learning
 plotly==5.13.1: machine_learning
 chembl_structure_pipeline==1.1.0: preprocessing
-torch==1.12.1: deep_learning
-torchvision==0.13.1: deep_learning
-torchaudio==0.12.1: deep_learning
+torch==2.0.0: deep_learning
 dgl==0.9.1: deep_learning
-deepchem==2.5.0: deep_learning
-tensorflow==2.10.0: deep_learning
+dgllife==0.3.2: deep_learning
+deepchem==2.7.1: deep_learning
+torch_geometric==2.3.1: deep_learning
+tensorflow==2.12.0: deep_learning
+tensorflow-probability==0.20.1: deep_learning
 boruta==0.3: preprocessing
 scikit-learn==1.2.0: machine_learning, deep_learning
+optuna==3.1.1: machine_learning, deep_learning
+scikit-multilearn==0.2.0: machine_learning, deep_learning
 pytest>=7.1.1: test
 pytest-cov>=3.0.0: test
 mypy>=0.942: test
 flake8>=4.0.1: test
 tox>=3.25.0: test
```

### Comparing `DeepMol-0.0.6b0/pyproject.toml` & `DeepMol-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/setup.cfg` & `DeepMol-1.0.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = DeepMol
-version = 0.0.6-beta
+version = 1.0.0
 description = DeepMol: a python-based machine and deep learning framework for drug discovery
 keywords = machine-learning, deep-learning, cheminformatics, drug-discovery
 author = DeepMol Team
 license = BSD 2-Clause License
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
@@ -20,14 +20,19 @@
 	=src
 packages = find_namespace:
 python_requires = >=3.7
 zip_safe = False
 include_package_data = True
 install_requires = 
 	rdkit-pypi==2022.9.3
+	cached_property==1.5.2
+	seaborn==0.12.0
+	joblib==1.1.1
+	pillow==8.4.0
+	h5py==3.7.0
 dependency_links = [
 	'git+https://github.com/samoturk/mol2vec#egg=mol2vec'
 	]
 
 [options.packages.find]
 where = src
```

### Comparing `DeepMol-0.0.6b0/setup.py` & `DeepMol-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/DeepMol.egg-info/PKG-INFO` & `DeepMol-1.0.0/src/DeepMol.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepMol
-Version: 0.0.6b0
+Version: 1.0.0
 Summary: DeepMol: a python-based machine and deep learning framework for drug discovery
 Author: DeepMol Team
 License: BSD 2-Clause License
 Keywords: machine-learning,deep-learning,cheminformatics,drug-discovery
 Platform: unix
 Platform: linux
 Platform: osx
@@ -13,40 +13,46 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
+Provides-Extra: test
+Provides-Extra: preprocessing
 Provides-Extra: deep_learning
 Provides-Extra: rdkit-pypi
-Provides-Extra: preprocessing
 Provides-Extra: machine_learning
-Provides-Extra: test
 Provides-Extra: smilespe
 Provides-Extra: seaborn
 Provides-Extra: joblib
 Provides-Extra: pillow
 Provides-Extra: h5py
+Provides-Extra: cached_property
+Provides-Extra: numpy
+Provides-Extra: dill
 Provides-Extra: shap
 Provides-Extra: gensim
 Provides-Extra: imblearn
 Provides-Extra: umap-learn
 Provides-Extra: kneed
 Provides-Extra: kaleido
 Provides-Extra: plotly
 Provides-Extra: chembl_structure_pipeline
 Provides-Extra: torch
-Provides-Extra: torchvision
-Provides-Extra: torchaudio
 Provides-Extra: dgl
+Provides-Extra: dgllife
 Provides-Extra: deepchem
+Provides-Extra: torch_geometric
 Provides-Extra: tensorflow
+Provides-Extra: tensorflow-probability
 Provides-Extra: boruta
 Provides-Extra: scikit-learn
+Provides-Extra: optuna
+Provides-Extra: scikit-multilearn
 Provides-Extra: pytest
 Provides-Extra: pytest-cov
 Provides-Extra: mypy
 Provides-Extra: flake8
 Provides-Extra: tox
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `DeepMol-0.0.6b0/src/DeepMol.egg-info/requires.txt` & `DeepMol-1.0.0/src/DeepMol.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,92 @@
 rdkit-pypi==2022.9.3
+cached_property==1.5.2
+seaborn==0.12.0
+joblib==1.1.1
+pillow==8.4.0
+h5py==3.7.0
 
 [all]
+seaborn==0.12.0
+mypy>=0.942
+optuna==3.1.1
 rdkit-pypi==2022.9.3
-kneed==0.8.2
-joblib==1.1.1
+torch==2.0.0
+scikit-multilearn==0.2.0
+deepchem==2.7.1
+dgl==0.9.1
 boruta==0.3
-h5py==3.7.0
-torchvision==0.13.1
+joblib==1.1.1
+cached_property==1.5.2
+plotly==5.13.1
+chembl_structure_pipeline==1.1.0
+gensim==4.2.0
+kneed==0.8.2
 shap==0.41.0
-imblearn
 flake8>=4.0.1
-chembl_structure_pipeline==1.1.0
-smilespe==0.0.3
-scikit-learn==1.2.0
-torchaudio==0.12.1
-kaleido==0.2.1
-tox>=3.25.0
+pillow==8.4.0
 pytest-cov>=3.0.0
 pytest>=7.1.1
-dgl==0.9.1
 umap-learn==0.5.1
-seaborn==0.12.0
-mypy>=0.942
-deepchem==2.5.0
-gensim==4.2.0
-plotly==5.13.1
-pillow==8.4.0
-tensorflow==2.10.0
-torch==1.12.1
+tox>=3.25.0
+dill==0.3.6
+torch_geometric==2.3.1
+tensorflow-probability==0.20.1
+smilespe==0.0.3
+tensorflow==2.12.0
+imblearn
+numpy==1.23.5
+h5py==3.7.0
+dgllife==0.3.2
+scikit-learn==1.2.0
+kaleido==0.2.1
 
 [boruta]
 boruta==0.3
 
+[cached_property]
+cached_property==1.5.2
+
 [chembl_structure_pipeline]
 chembl_structure_pipeline==1.1.0
 
 [deep_learning]
+seaborn==0.12.0
+optuna==3.1.1
 rdkit-pypi==2022.9.3
+torch==2.0.0
+scikit-multilearn==0.2.0
+deepchem==2.7.1
 dgl==0.9.1
 joblib==1.1.1
-seaborn==0.12.0
-h5py==3.7.0
+cached_property==1.5.2
+shap==0.41.0
 pillow==8.4.0
+dill==0.3.6
+torch_geometric==2.3.1
+tensorflow-probability==0.20.1
 smilespe==0.0.3
-tensorflow==2.10.0
+tensorflow==2.12.0
+numpy==1.23.5
+h5py==3.7.0
+dgllife==0.3.2
 scikit-learn==1.2.0
-torchvision==0.13.1
-torchaudio==0.12.1
-deepchem==2.5.0
-torch==1.12.1
-shap==0.41.0
 
 [deepchem]
-deepchem==2.5.0
+deepchem==2.7.1
 
 [dgl]
 dgl==0.9.1
 
+[dgllife]
+dgllife==0.3.2
+
+[dill]
+dill==0.3.6
+
 [flake8]
 flake8>=4.0.1
 
 [gensim]
 gensim==4.2.0
 
 [h5py]
@@ -75,92 +101,112 @@
 [kaleido]
 kaleido==0.2.1
 
 [kneed]
 kneed==0.8.2
 
 [machine_learning]
+seaborn==0.12.0
+joblib==1.1.1
+kaleido==0.2.1
 plotly==5.13.1
+optuna==3.1.1
 rdkit-pypi==2022.9.3
+scikit-multilearn==0.2.0
 umap-learn==0.5.1
-joblib==1.1.1
+smilespe==0.0.3
 kneed==0.8.2
-seaborn==0.12.0
+shap==0.41.0
+dill==0.3.6
+scikit-learn==1.2.0
+numpy==1.23.5
 h5py==3.7.0
 pillow==8.4.0
-smilespe==0.0.3
-scikit-learn==1.2.0
-kaleido==0.2.1
-shap==0.41.0
+cached_property==1.5.2
 
 [mypy]
 mypy>=0.942
 
+[numpy]
+numpy==1.23.5
+
+[optuna]
+optuna==3.1.1
+
 [pillow]
 pillow==8.4.0
 
 [plotly]
 plotly==5.13.1
 
 [preprocessing]
-imblearn
-rdkit-pypi==2022.9.3
-joblib==1.1.1
-boruta==0.3
 seaborn==0.12.0
+joblib==1.1.1
 chembl_structure_pipeline==1.1.0
+gensim==4.2.0
+rdkit-pypi==2022.9.3
+smilespe==0.0.3
+dill==0.3.6
+boruta==0.3
+imblearn
+numpy==1.23.5
 h5py==3.7.0
 pillow==8.4.0
-smilespe==0.0.3
-gensim==4.2.0
+cached_property==1.5.2
 
 [pytest]
 pytest>=7.1.1
 
 [pytest-cov]
 pytest-cov>=3.0.0
 
 [rdkit-pypi]
 rdkit-pypi==2022.9.3
 
 [scikit-learn]
 scikit-learn==1.2.0
 
+[scikit-multilearn]
+scikit-multilearn==0.2.0
+
 [seaborn]
 seaborn==0.12.0
 
 [shap]
 shap==0.41.0
 
 [smilespe]
 smilespe==0.0.3
 
 [tensorflow]
-tensorflow==2.10.0
+tensorflow==2.12.0
+
+[tensorflow-probability]
+tensorflow-probability==0.20.1
 
 [test]
+seaborn==0.12.0
+mypy>=0.942
+joblib==1.1.1
 pytest>=7.1.1
 rdkit-pypi==2022.9.3
-joblib==1.1.1
+smilespe==0.0.3
+tox>=3.25.0
+dill==0.3.6
 flake8>=4.0.1
-seaborn==0.12.0
+numpy==1.23.5
 h5py==3.7.0
 pillow==8.4.0
-smilespe==0.0.3
-mypy>=0.942
-tox>=3.25.0
+cached_property==1.5.2
 pytest-cov>=3.0.0
 
 [torch]
-torch==1.12.1
-
-[torchaudio]
-torchaudio==0.12.1
+torch==2.0.0
 
-[torchvision]
-torchvision==0.13.1
+[torch_geometric]
+torch_geometric==2.3.1
 
 [tox]
 tox>=3.25.0
 
 [umap-learn]
 umap-learn==0.5.1
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/compound_featurization/__init__.py` & `DeepMol-1.0.0/src/deepmol/compound_featurization/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 try:
     from .mol2vec import Mol2Vec
 except ImportError:
     warnings.warn("Mol2Vec not available. Please install it to use it.")
 
 try:
     from .deepchem_featurizers import WeaveFeat, CoulombFeat, CoulombEigFeat, ConvMolFeat, MolGraphConvFeat, \
-        SmileImageFeat, SmilesSeqFeat, MolGanFeat
+        SmileImageFeat, SmilesSeqFeat, MolGanFeat, PagtnMolGraphFeat, DagTransformer, DMPNNFeat, MATFeat, RawFeat
 except ImportError:
     warnings.warn("DeepChem not available. Please install it to use it.")
 
+from .one_hot_encoder import SmilesOneHotEncoder
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/compound_featurization/base_featurizer.py` & `DeepMol-1.0.0/src/deepmol/compound_featurization/base_featurizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from abc import ABC, abstractmethod
 from typing import Tuple
 
 import numpy as np
 from rdkit.Chem import Mol, MolToSmiles
 
+from deepmol.base import Transformer
 from deepmol.datasets import Dataset
 from deepmol.loggers.logger import Logger
 from deepmol.parallelism.multiprocessing import JoblibMultiprocessing
-from deepmol.scalers import BaseScaler
+from deepmol.utils.decorators import modify_object_inplace_decorator
 from deepmol.utils.errors import PreConditionViolationException
 from deepmol.utils.utils import canonicalize_mol_object
 
 
-class MolecularFeaturizer(ABC):
+class MolecularFeaturizer(ABC, Transformer):
     """
     Abstract class for calculating a set of features for a molecule.
     A `MolecularFeaturizer` uses SMILES strings or RDKit molecule objects to represent molecules.
 
     Subclasses need to implement the _featurize method for calculating features for a single molecule.
     """
 
@@ -25,14 +26,15 @@
         Initializes the featurizer.
 
         Parameters
         ----------
         n_jobs: int
             The number of jobs to run in parallel in the featurization.
         """
+        super().__init__()
         self.n_jobs = n_jobs
         self.feature_names = None
         self.logger = Logger()
 
     def _featurize_mol(self, mol: Mol) -> Tuple[np.ndarray, bool]:
         """
         Calculate features for a single molecule.
@@ -58,38 +60,32 @@
             exit(1)
 
         except Exception as e:
             if mol is not None:
                 smiles = MolToSmiles(mol)
             else:
                 smiles = None
-            self.logger = Logger()
             self.logger.error(f"Failed to featurize {smiles}. Appending empty array")
             self.logger.error("Exception message: {}".format(e))
             remove_mol = True
             return np.array([]), remove_mol
 
+    @modify_object_inplace_decorator
     def featurize(self,
                   dataset: Dataset,
-                  scaler: BaseScaler = None,
-                  path_to_save_scaler: str = None,
                   remove_nans_axis: int = 0
                   ) -> Dataset:
 
         """
         Calculate features for molecules.
 
         Parameters
         ----------
         dataset: Dataset
             The dataset containing the molecules to featurize in dataset.mols.
-        scaler: BaseScaler
-            The scaler to use for scaling the generated features.
-        path_to_save_scaler: str
-            The path to save the scaler to.
         remove_nans_axis: int
             The axis to remove NaNs from. If None, no NaNs are removed.
 
         Returns
         -------
         dataset: Dataset
           The input Dataset containing a featurized representation of the molecules in Dataset.X.
@@ -98,35 +94,62 @@
 
         multiprocessing_cls = JoblibMultiprocessing(process=self._featurize_mol, n_jobs=self.n_jobs)
         features = multiprocessing_cls.run(molecules)
 
         features, remove_mols = zip(*features)
 
         remove_mols_list = np.array(remove_mols)
-        dataset.remove_elements(dataset.ids[remove_mols_list])
+        dataset.remove_elements(dataset.ids[remove_mols_list], inplace=True)
 
         features = np.array(features)
         features = features[~remove_mols_list]
 
         if (isinstance(features[0], np.ndarray) and len(features[0].shape) == 2) or not isinstance(features[0],
                                                                                                    np.ndarray):
             pass
         else:
             features = np.vstack(features)
+
+        dataset.clear_cached_properties()
         dataset._X = features
         dataset.feature_names = self.feature_names
 
-        dataset.remove_nan(remove_nans_axis)
-
-        if scaler and path_to_save_scaler:
-            # transform data
-            scaler.fit_transform(dataset)
-            scaler.save(path_to_save_scaler)
-
-        elif scaler:
-            scaler.transform(dataset)
-
+        dataset.remove_nan(remove_nans_axis, inplace=True)
         return dataset
 
     @abstractmethod
     def _featurize(self, mol: Mol):
         raise NotImplementedError
+
+    def _transform(self, dataset: Dataset) -> Dataset:
+        """
+        Calculate features for molecules. This method is called by the transform method of the Transformer class.
+        To be used by pipeline.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            The dataset containing the molecules to featurize in dataset.mols.
+
+        Returns
+        -------
+        dataset: Dataset
+            The input Dataset containing a featurized representation of the molecules in Dataset.X.
+        """
+        return self.featurize(dataset)
+
+    def _fit(self, dataset: Dataset) -> 'MolecularFeaturizer':
+        """
+        Fit the featurizer. This method is called by the fit method of the Transformer class.
+        To be used by pipeline.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            The dataset containing the molecules to featurize in dataset.mols.
+
+        Returns
+        -------
+        self: MolecularFeaturizer
+            The fitted featurizer.
+        """
+        return self
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/compound_featurization/mixed_descriptors.py` & `DeepMol-1.0.0/src/deepmol/compound_featurization/mixed_descriptors.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         Parameters
         ----------
         featurizers: Iterable[MolecularFeaturizer]
             Iterable of featurizer to use to create features.
         """
         super().__init__(**kwargs)
         self.featurizers = featurizers
-        self.feature_names = [name for featurizer in featurizers for name in featurizer.feature_names]
+        self.feature_names = [name for featurizer in self.featurizers for name in featurizer.feature_names]
 
     def _featurize(self, mol: Mol):
         """
         Featurization with mix of featurizers.
 
         Parameters
         ----------
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/compound_featurization/mol2vec.py` & `DeepMol-1.0.0/src/deepmol/compound_featurization/mol2vec.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/compound_featurization/rdkit_descriptors.py` & `DeepMol-1.0.0/src/deepmol/compound_featurization/rdkit_descriptors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import inspect
 import sys
 import traceback
 import warnings
+from abc import ABC
 from typing import Union, List
 
 import numpy as np
 from rdkit import Chem
 from rdkit.Chem import Mol, AllChem, MolFromSmiles, Descriptors, rdMolDescriptors
+from rdkit.Chem.GraphDescriptors import Ipc
 from rdkit.Chem.rdForceFieldHelpers import UFFOptimizeMoleculeConfs
 from rdkit.ML.Descriptors import MoleculeDescriptors
 
 from deepmol.compound_featurization import MolecularFeaturizer
 from deepmol.datasets import Dataset
 from deepmol.loggers.logger import Logger
 from deepmol.utils.errors import PreConditionViolationException
@@ -385,15 +387,16 @@
     for i in range(mol_set.shape[0]):
         printProgressBar(i, mol_set.shape[0])
         try:
             signal.alarm(timeout_per_molecule)
             m2 = generate_conformers(generator, mol_set[i], etkg_version, optimization_mode)
             signal.alarm(0)
             label = dataset.y[i]
-            m2.SetProp("_Class", "%f" % label)
+            for j, class_name in enumerate(dataset.label_names):
+                m2.SetProp(class_name, "%f" % label[j])
             if dataset.ids is not None and dataset.ids.size > 0:
                 mol_id = dataset.ids[i]
                 m2.SetProp("_ID", f"{mol_id}")
             writer.write(m2)
             final_set_with_conformations.append(m2)
         except:
             logger.info("Timeout for molecule %d" % i)
@@ -424,23 +427,30 @@
             Mol object from rdkit.
 
         Returns
         -------
         all_descriptors: np.ndarray
             Array with all 2D descriptors from rdkit.
         """
-        calc = MoleculeDescriptors.MolecularDescriptorCalculator([x[0] for x in Descriptors._descList])
-
-        descriptors = calc.CalcDescriptors(mol)
+        calc = MoleculeDescriptors.MolecularDescriptorCalculator(self.feature_names)
+        # Deal with very large/inf values of the Ipc descriptor (https://github.com/rdkit/rdkit/issues/1527)
+        # find position of Ipc
+        pos = self.feature_names.index("Ipc")
+        # calculate AvgIpc
+        avg_ipc = Ipc(mol, avg=1)
+
+        descriptors = list(calc.CalcDescriptors(mol))
+        # replace Ipc with AvgIpc
+        descriptors[pos] = avg_ipc
         assert not np.isnan(np.sum(descriptors))
         descriptors = np.array(descriptors, dtype=np.float32)
         return descriptors
 
 
-class ThreeDimensionDescriptor(MolecularFeaturizer):
+class ThreeDimensionDescriptor(MolecularFeaturizer, ABC):
     """
     Class to generate three-dimensional descriptors.
     """
 
     def __init__(self, mandatory_generation_of_conformers: bool, **kwargs):
         """
         Initialize the class.
@@ -503,17 +513,14 @@
         fp = self.descriptor_function(mol)
         if any([isinstance(fp, fp_type) for fp_type in [str, int, np.float32, float, np.int64]]):
             fp = [fp]
 
         fp = np.asarray(fp, dtype=np.float32)
         return fp
 
-    def _featurize(self, mol: Mol):
-        raise NotImplementedError
-
 
 class All3DDescriptors(MolecularFeaturizer):
     """
     Class to generate all three-dimensional descriptors.
     """
 
     def __init__(self, mandatory_generation_of_conformers=True):
@@ -648,15 +655,15 @@
         Parameters
         ----------
         mandatory_generation_of_conformers: bool
             If True, the conformers are generated and optimized before the descriptors are calculated.
         """
         super().__init__(mandatory_generation_of_conformers)
         self.descriptor_function = rdMolDescriptors.CalcPBF
-        self.feature_names = ['PBF']
+        self.feature_names = self.feature_names = ['PBF']
 
     def _featurize(self, mol: Mol) -> np.ndarray:
         """
         Radial distribution function descriptors calculation.
 
         Parameters
         ----------
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/compound_featurization/similarity_matrix.py` & `DeepMol-1.0.0/src/deepmol/compound_featurization/similarity_matrix.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 from typing import Tuple
 
 import numpy as np
 
+from deepmol.base import Transformer
 from deepmol.compound_featurization._utils import calc_morgan_fingerprints, calc_similarity
 from deepmol.datasets import Dataset
 from deepmol.parallelism.multiprocessing import JoblibMultiprocessing
+from deepmol.utils.decorators import modify_object_inplace_decorator
 
 
-class TanimotoSimilarityMatrix:
+class TanimotoSimilarityMatrix(Transformer):
+    """
+    Class to calculate Tanimoto similarity matrix for a dataset.
+
+    The similarity matrix is calculated using Morgan fingerprints.
+    """
 
     def __init__(self, n_molecules: int, n_jobs: int = -1) -> None:
         """
         Initialize a MACCSkeysFingerprint object.
 
         Parameters
         ----------
         n_molecules: int
             Number of molecules in the dataset.
         n_jobs: int
             Number of jobs to run in parallel.
         """
+        super().__init__()
+        self.n_molecules = n_molecules
         self.n_jobs = n_jobs
-        self.feature_names = [f"tanimoto_{i}" for i in range(n_molecules)]
+        self.feature_names = [f"tanimoto_{i}" for i in range(self.n_molecules)]
         self.fps = None
 
     def _calc_similarity(self, i, j) -> Tuple[int, int, float]:
         """
         Calculates the Tanimoto similarity between two fingerprints.
 
         Parameters
@@ -42,14 +51,15 @@
         j: int
             Index of the second fingerprint
         similarity: float
             Tanimoto similarity between the two fingerprints
         """
         return calc_similarity(i, j, self.fps)
 
+    @modify_object_inplace_decorator
     def featurize(self,
                   dataset: Dataset,
                   **kwargs
                   ) -> Dataset:
         """
         Calculate Tanimoto similarities between all pairs of molecules in the dataset.
 
@@ -79,7 +89,39 @@
             similarity_matrix[j, i] = similarity
 
         features = np.array(similarity_matrix, dtype=object)
 
         dataset._X = features
         dataset.feature_names = self.feature_names
         return dataset
+
+    def _fit(self, dataset: Dataset) -> 'TanimotoSimilarityMatrix':
+        """
+        Fit the featurizer to a dataset.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            The dataset to fit the featurizer to.
+
+        Returns
+        -------
+        self: Mol2Vec
+            The fitted featurizer.
+        """
+        return self
+
+    def _transform(self, dataset: Dataset) -> Dataset:
+        """
+        Transform a dataset.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            The dataset to transform.
+
+        Returns
+        -------
+        dataset: Dataset
+            The transformed dataset.
+        """
+        return self.featurize(dataset)
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/datasets/_utils.py` & `DeepMol-1.0.0/src/deepmol/datasets/_utils.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/datasets/datasets.py` & `DeepMol-1.0.0/src/deepmol/datasets/datasets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 import uuid
 import warnings
 from abc import ABC, abstractmethod
+from copy import deepcopy
 from typing import Union, List, Tuple
 
 import numpy as np
 import pandas as pd
 from rdkit.Chem import Mol
 
 from deepmol.loggers.logger import Logger
 from deepmol.datasets._utils import merge_arrays, merge_arrays_of_arrays
+from deepmol.utils.cached_properties import deepmol_cached_property
+from deepmol.utils.decorators import inplace_decorator
 from deepmol.utils.utils import smiles_to_mol, mol_to_smiles
 
 
 class Dataset(ABC):
-
     """
     Abstract base class for datasets
     Subclasses need to implement their own methods based on this class.
 
     """
 
     def __init__(self):
         self.logger = Logger()
 
+    def clear_cached_properties(self):
+        """
+        Clears the cached properties of the class.
+        """
+        for name in dir(type(self)):
+            if isinstance(getattr(type(self), name), deepmol_cached_property):
+                vars(self).pop(name, None)
+
     @abstractmethod
     def __len__(self) -> int:
         """
         Get the length of the dataset.
         It returns the number of molecules in the dataset.
         """
 
@@ -84,26 +94,14 @@
 
         Returns
         -------
         X: np.ndarray
             The features in the dataset.
         """
 
-    @X.setter
-    @abstractmethod
-    def X(self, value: Union[List, np.ndarray]) -> None:
-        """
-        Set the features in the dataset.
-
-        Parameters
-        ----------
-        value: Union[List, np.ndarray]
-            The features to set in the dataset.
-        """
-
     @property
     @abstractmethod
     def y(self) -> np.ndarray:
         """
         Get the labels in the dataset.
 
         Returns
@@ -274,15 +272,15 @@
         Parameters
         ----------
         indexes: List[int]
             The indexes of the elements to remove.
         """
 
     @abstractmethod
-    def select_features_by_index(self, indexes: List[int]) -> None:
+    def select_features_by_index(self, indexes: List[int]) -> 'Dataset':
         """
         Select the features from the dataset.
         Parameters
         ----------
         indexes: List[int]
             The indexes of the features to select.
         """
@@ -366,15 +364,16 @@
         super().__init__()
         self._smiles = np.array(smiles)
         self._ids = np.array([str(i) for i in ids]) if ids is not None \
             else np.array([str(uuid.uuid4().hex) for _ in range(len(smiles))])
         self._X = np.array(X) if X is not None else None
         self._y = np.array(y) if y is not None else None
         self._mols = np.array(mols) if mols is not None else np.array([smiles_to_mol(s) for s in self._smiles])
-        self.remove_elements([self._ids[i] for i, m in enumerate(self._mols) if m is None])
+        invalid = [self._ids[i] for i, m in enumerate(self._mols) if m is None]
+        self.remove_elements(invalid, inplace=True)
         self._feature_names = np.array(feature_names) if feature_names is not None else None
         self._label_names = np.array(label_names) if label_names is not None else None
         self._validate_params()
         self._n_tasks = len(self._label_names) if self._label_names is not None else 0
         self._mode = mode if mode != 'auto' else self._infer_mode()
         self.logger = Logger()
 
@@ -475,36 +474,46 @@
         super().__init__()
         self._smiles = np.array(smiles)
         self._ids = np.array([str(uuid.uuid4().hex) for _ in range(len(smiles))])
         self._X = None
         self._y = None
         self._n_tasks = None
         self._mols = np.array([smiles_to_mol(s) for s in self._smiles])
-        self.remove_elements([self._ids[i] for i, m in enumerate(self._mols) if m is None])
+        self.remove_elements([self._ids[i] for i, m in enumerate(self._mols) if m is None], inplace=True)
         self._feature_names = None
         self._label_names = None
         self.mode = None
 
-    def _infer_mode(self) -> Union[str, None]:
+    def _infer_mode(self) -> Union[str, None, List[str]]:
         """
         Infers the mode of the dataset.
 
         Returns
         -------
         str
             The inferred mode.
         """
         if self._y is None:
             return None
         if len(self._y.shape) > 1:
             self.logger.info("Assuming multitask since y has more than one dimension. If otherwise, explicitly set the "
                              "mode to 'classification' or 'regression'!")
-            return 'multitask'
-        classes = np.unique(self.y)
-        if len(classes) > 10:
+            labels_per_task = []
+            for label in range(self._y.shape[1]):
+                label_i = self._y[:, label]
+                classes = np.all(np.isclose(label_i, np.round(label_i), equal_nan=True))
+                if classes:
+                    labels_per_task.append('classification')
+                else:
+                    labels_per_task.append('regression')
+
+            return labels_per_task
+
+        classes = np.all(np.isclose(self.y, np.round(self.y), equal_nan=True))
+        if not classes:
             self.logger.info("Assuming regression since there are more than 10 unique y values. If otherwise, "
                              "explicitly set the mode to 'classification'!")
             return 'regression'
         else:
             self.logger.info("Assuming classification since there are less than 10 unique y values. If otherwise, "
                              "explicitly set the mode to 'regression'!")
             return 'classification'
@@ -564,17 +573,22 @@
             Feature names of the molecules.
         """
         if self._X is None:
             raise ValueError('The features must be set before setting the feature names.')
         if len(self._X.shape) == 1:
             if len(feature_names) != 1:
                 raise ValueError('The number of feature names must be equal to the number of features.')
-        else:
+        elif len(self._X.shape) == 2:
             if len(feature_names) != len(self._X[0]):
                 raise ValueError('The number of feature names must be equal to the number of features.')
+        elif len(self._X.shape) == 3:
+            if len(feature_names) != len(self._X[0][0]):
+                raise ValueError('The number of feature names must be equal to the number of features.')
+        else:
+            raise ValueError('The number of dimensions of X must be 1, 2 or 3.')
         if len(feature_names) != len(set(feature_names)):
             raise ValueError('The feature names must be unique.')
         self._feature_names = np.array([str(fn) for fn in feature_names])
 
     @property
     def label_names(self) -> np.ndarray:
         """
@@ -603,15 +617,15 @@
         else:
             if len(label_names) != len(self._y[0]):
                 raise ValueError('The number of label names must be equal to the number of labels.')
         if len(label_names) != len(set(label_names)):
             raise ValueError('The label names must be unique.')
         self._label_names = np.array([str(ln) for ln in label_names])
 
-    @property
+    @deepmol_cached_property
     def X(self) -> np.ndarray:
         """
         Get the features of the molecules in the dataset.
         Returns
         -------
         np.ndarray
             Features of the molecules in the dataset.
@@ -684,16 +698,21 @@
         Set the mode of the dataset.
 
         Parameters
         ----------
         mode: str
             The mode of the dataset.
         """
-        if mode not in ['classification', 'regression', None]:
-            raise ValueError('The mode must be either "classification" or "regression".')
+        if not isinstance(mode, list):
+            if mode not in ['classification', 'regression', None]:
+                raise ValueError('The mode must be either "classification" or "regression".')
+        else:
+            for m in mode:
+                if m not in ['classification', 'regression', None]:
+                    raise ValueError('The mode must be either "classification" or "regression".')
         self._mode = mode
 
     def get_shape(self) -> Tuple[Tuple, Union[Tuple, None], Union[Tuple, None]]:
         """
         Get the shape of the dataset.
         Returns three tuples, giving the shape of the smiles, X and y arrays.
 
@@ -710,106 +729,134 @@
         self.logger.info(f'Mols_shape: {smiles_shape}')
         x_shape = self._X.shape if self._X is not None else None
         self.logger.info(f'Features_shape: {x_shape}')
         y_shape = self._y.shape if self._y is not None else None
         self.logger.info(f'Labels_shape: {y_shape}')
         return smiles_shape, x_shape, y_shape
 
+    @inplace_decorator
     def remove_duplicates(self) -> None:
         """
         Remove molecules with duplicated features from the dataset.
+
+        Parameters
+        ----------
+        inplace: bool, optional (default False)
+            If True, the dataset will be modified in place.
         """
         if self._X is not None:
             if np.isnan(np.stack(self._X)).any():
                 warnings.warn('The dataset contains NaNs. Molecules with NaNs will be ignored.')
             unique, index = np.unique(self.X, return_index=True, axis=0)
             ids = self.ids[index]
-            self.select(ids, axis=0)
+            self.select(ids, axis=0, inplace=True)
 
+    @inplace_decorator
     def remove_elements(self, ids: List[str]) -> None:
         """
         Remove elements with specific IDs from the dataset.
         Parameters
         ----------
         ids: List[str]
             IDs of the elements to remove.
+        inplace: bool, optional (default False)
+            If True, the dataset will be modified in place.
         """
         if len(ids) != 0:
             all_indexes = self.ids
             indexes_to_keep = list(set(all_indexes) - set(ids))
-            self.select(indexes_to_keep)
+            self.select(indexes_to_keep, inplace=True)
 
+    @inplace_decorator
     def remove_elements_by_index(self, indexes: List[int]) -> None:
         """
         Remove elements with specific indexes from the dataset.
         Parameters
         ----------
         indexes: List[int]
             Indexes of the elements to remove.
+        inplace: bool, optional (default False)
+            If True, the dataset will be modified in place.
         """
         if len(indexes) > 0:
             indexes = self._ids[indexes]
-            self.remove_elements(indexes)
+            self.remove_elements(indexes, inplace=True)
 
-    def select_features_by_index(self, indexes: List[int]) -> None:
+    @inplace_decorator
+    def select_features_by_index(self, indexes: List[int]) -> 'SmilesDataset':
         """
         Select features with specific indexes from the dataset
         Parameters
         ----------
         indexes: List[int]
             The indexes of the features to select from the dataset.
+        inplace: bool, optional (default False)
+            If True, the dataset will be modified in place.
         """
         if len(indexes) != 0:
-            self.select(indexes, axis=1)
+            self.select(indexes, axis=1, inplace=True)
+            self.clear_cached_properties()
+            return self
+        else:
+            raise ValueError('The list of indexes is empty.')
 
+    @inplace_decorator
     def select_features_by_name(self, names: List[str]) -> None:
         """
         Select features with specific names from the dataset
         Parameters
         ----------
         names: List[str]
             The names of the features to select from the dataset.
+        inplace: bool, optional (default False)
+            If True, the dataset will be modified in place.
         """
         if len(names) != 0:
             # Get the indexes of the features to select
             indexes = [i for i, name in enumerate(self._feature_names) if name in names]
-            self.select(indexes, axis=1)
+            self.select(indexes, axis=1, inplace=True)
+            self.clear_cached_properties()
 
+    @inplace_decorator
     def remove_nan(self, axis: int = 0) -> None:
         """
         Remove samples with at least one NaN in the features (when axis = 0)
         Or remove samples with all features with NaNs and the features with at least one NaN (axis = 1)
         Parameters
         ----------
         axis: int
             The axis to remove the NaNs from.
+        inplace: bool, optional (default False)
+            If True, the dataset will be modified in place.
         """
         if self._X is None or len(self._X.shape) == 0:
             return
         if axis == 0:
             if len(self._X.shape) == 1:
                 indexes = np.where(pd.isna(self._X))[0]
             else:
                 indexes = np.where(pd.isna(self._X).any(axis=1))[0]
             # rows with at least one NaN
-            self.remove_elements_by_index(indexes)
+            self.remove_elements_by_index(indexes, inplace=True)
         elif axis == 1:
             if len(self._X.shape) == 1:
                 indexes = np.where(np.isnan(self._X))[0]
-                self.remove_elements_by_index(indexes)
+                self.remove_elements_by_index(indexes, inplace=True)
             else:
                 # rows with all NaNs
                 indexes = np.where(np.isnan(self._X).all(axis=1))[0]
-                self.remove_elements_by_index(indexes)
+                self.remove_elements_by_index(indexes, inplace=True)
                 # columns with at least one NaN
                 columns = list(set(np.where(np.isnan(self._X).any(axis=0))[0]))
                 self._X = np.delete(self._X, columns, axis=1)
                 if len(self._X.shape) <= 2:  # feature names in datasets with more than two dimensions not supported
                     feature_names_to_delete = [self._feature_names[i] for i in columns]
                     self._feature_names = [name for name in self._feature_names if name not in feature_names_to_delete]
+
+                self.clear_cached_properties()
         else:
             raise ValueError('The axis must be 0 or 1.')
 
     def select_to_split(self, indexes: Union[np.ndarray, List[int]]) -> 'SmilesDataset':
         """
         Select elements with specific indexes to split the dataset
         Parameters
@@ -827,25 +874,28 @@
         y = self._y[indexes] if self._y is not None else None
         ids = self._ids[indexes]
         feature_names = self._feature_names
         label_names = self._label_names
         mode = self._mode
         return SmilesDataset(smiles, mols, ids, X, feature_names, y, label_names, mode)
 
+    @inplace_decorator
     def select(self, ids: Union[List[str], List[int]], axis: int = 0) -> None:
         """
         Creates a new sub dataset of self from a selection of indexes.
 
         Parameters
         ----------
         ids: Union[List[str], List[int]]
           List of ids/indexes to select.IDs of the compounds in case axis = 0,
           indexes of the columns in case axis = 1.
         axis: int
             Axis to select along. 0 selects along the first axis, 1 selects along the second axis.
+        inplace: bool, optional (default False)
+            If True, the dataset will be modified in place.
         """
         if axis == 0:
             ids_to_delete = sorted(list(set(self._ids) - set(ids)))
             raw_indexes = [i for i, mol_index in enumerate(self._ids) if mol_index in ids_to_delete]
             for idx in raw_indexes:
                 self.logger.error(f"Molecule with smiles: {self._smiles[idx]} removed from dataset.")
             self._smiles = np.delete(self._smiles, raw_indexes, axis)
@@ -925,21 +975,24 @@
         if self._X is not None:
             columns_names = self._feature_names
             df_x = pd.DataFrame(self._X, columns=columns_names)
             df = pd.concat([df, df_x], axis=1)
 
         df.to_csv(path, index=False)
 
+    @inplace_decorator
     def load_features(self, path: str, **kwargs) -> None:
         """
         Load features from a csv file.
         Parameters
         ----------
         path: str
             Path to the csv file.
+        inplace: bool, optional (default False)
+            If True, the dataset will be modified in place.
         kwargs:
             Keyword arguments to pass to pandas.read_csv.
         """
         df = pd.read_csv(path, **kwargs)
         self._X = df.to_numpy()
 
     def save_features(self, path: str = 'features.csv') -> None:
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/evaluator/evaluator.py` & `DeepMol-1.0.0/src/deepmol/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/feature_selection/base_feature_selector.py` & `DeepMol-1.0.0/src/deepmol/feature_selection/base_feature_selector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,94 @@
-from abc import ABC, abstractmethod
-from typing import Union, Iterable, List
+from abc import ABC
+from typing import Union, Iterable
 
 import numpy as np
 from boruta import BorutaPy
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
-from sklearn.feature_selection import VarianceThreshold, chi2, SelectKBest, SelectPercentile, RFECV, SelectFromModel
+from sklearn.feature_selection import VarianceThreshold, SelectKBest, SelectPercentile, RFECV, SelectFromModel, \
+    f_classif
 
+from deepmol.base import Transformer
 from deepmol.datasets import Dataset
+from deepmol.utils.decorators import modify_object_inplace_decorator
 
 
-class BaseFeatureSelector(ABC):
+class BaseFeatureSelector(ABC, Transformer):
     """
     Abstract class for feature selection.
     A `BaseFeatureSelector` uses features present in a Dataset object to select the most important ones.
     FeatureSelectors which are subclasses of this class should always operate over Dataset Objects.
-
-    Subclasses need to implement the _select_features method for performing feature selection.
     """
 
-    def __init__(self):
+    def __init__(self, feature_selector):
         """
         Initialize the feature selector.
         """
         if self.__class__ == BaseFeatureSelector:
             raise Exception('Abstract class BaseFeatureSelector should not be instantiated')
+        super().__init__()
+        self.feature_selector = feature_selector
+        self.features_to_keep = None
 
-    def select_features(self, dataset: Dataset):
+    @modify_object_inplace_decorator
+    def select_features(self, dataset: Dataset) -> Dataset:
         """
         Perform feature selection for the molecules present in the dataset.
 
         Parameters
         ----------
         dataset: Dataset
             Dataset to perform feature selection on
+        inplace: bool
+            Whether to perform the feature selection in the received dataset or not.
 
         Returns
         -------
         dataset: Dataset
           Dataset containing the selected features and indexes of the features kept as 'self.features2keep'.
         """
-        features_to_keep = self._select_features(dataset)
-        dataset.select_features_by_index(list(features_to_keep))
-        return dataset
+        return self.fit_transform(dataset)
 
-    @abstractmethod
-    def _select_features(self, dataset: Dataset) -> np.ndarray:
+    def _transform(self, dataset: Dataset) -> Dataset:
         """
         Perform feature selection for the molecules present in the dataset.
 
         Parameters
         ----------
         dataset: Dataset
             Dataset to perform feature selection on
 
         Returns
         -------
-        features_to_keep: np.ndarray
-            Array containing the indexes of the features to keep.
+        dataset: Dataset
+          Dataset containing the selected features and indexes of the features kept as 'self.features2keep'.
+        """
+        if self.features_to_keep is not None:
+            dataset = dataset.select_features_by_index(list(self.features_to_keep))
+        return dataset
+
+    def _fit(self, dataset: Dataset) -> 'BaseFeatureSelector':
+        """
+        Fits the feature selector to a dataset of molecules.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            Dataset of molecules.
+
+        Returns
+        -------
+        self: BaseFeatureSelector
+            The fitted feature selector.
         """
+        x = np.stack(dataset.X, axis=0)
+        y = np.array(dataset.y)
+        fs = self.feature_selector.fit(x, y)
+        self.features_to_keep = fs.get_support(indices=True)
+        return self
 
 
 class LowVarianceFS(BaseFeatureSelector):
     """
     Class for Low Variance feature selection.
     Feature selector that removes all features with low-variance.
     """
@@ -71,123 +98,60 @@
         Initialize this Feature Selector
 
         Parameters
         ----------
         threshold: float
             Features with a training-set variance lower than this threshold will be removed.
         """
-        super().__init__()
         self.param = threshold
-
-    def _select_features(self, dataset: Dataset) -> np.ndarray:
-        """
-        Returns features and indexes of features to keep.
-
-        Parameters
-        ----------
-        dataset: Dataset
-            Dataset to perform feature selection on
-
-        Returns
-        -------
-        features_to_keep: np.ndarray
-            Array containing the indexes of the features to keep.
-        """
-        fs = np.stack(dataset.X, axis=0)
-        vt = VarianceThreshold(threshold=self.param)
-        vt.fit_transform(fs)
-        return vt.get_support(indices=True)
+        super().__init__(VarianceThreshold(threshold=threshold))
 
 
 class KbestFS(BaseFeatureSelector):
     """
     Class for K best feature selection.
 
     Select features according to the k-highest scores.
     """
 
-    def __init__(self, k: int = 10, score_func: callable = chi2):
+    def __init__(self, k: int = 10, score_func: callable = f_classif):
         """
         Initialize this KbestFS Feature Selector.
 
         Parameters
         ----------
         k: int
             Number of top features to select.
         score_func: callable
             Function taking two arrays X and y, and returning a pair of arrays (scores, pvalues) or a single array with
             scores.
         """
-        super().__init__()
-        self.k = k
-        self.score_func = score_func
-
-    def _select_features(self, dataset: Dataset) -> np.ndarray:
-        """
-        Returns features and indexes of features to keep.
-
-        Parameters
-        ----------
-        dataset: Dataset
-            Dataset to perform feature selection on
-
-        Returns
-        -------
-        features_to_keep: np.ndarray
-            Array containing the indexes of the features to keep.
-        """
-        fs = np.stack(dataset.X, axis=0)
-        y = dataset.y
-        kb = SelectKBest(self.score_func, k=self.k)
-        kb.fit_transform(fs, y)
-        return kb.get_support(indices=True)
+        super().__init__(SelectKBest(score_func=score_func, k=k))
 
 
 class PercentilFS(BaseFeatureSelector):
     """
     Class for percentil feature selection.
 
     Select features according to a percentile of the highest scores.
     """
 
-    def __init__(self, percentil: int = 10, score_func: callable = chi2):
+    def __init__(self, percentil: int = 10, score_func: callable = f_classif):
         """
         Initialize the PercentilFS Feature Selector.
 
         Parameters
         ----------
         percentil: int
             Percent of features to keep.
         score_func: callable
             Function taking two arrays X and y, and returning a pair of arrays (scores, pvalues) or a single array with
             scores.
         """
-        super().__init__()
-        self.percentil = percentil
-        self.score_func = score_func
-
-    def _select_features(self, dataset: Dataset) -> np.ndarray:
-        """
-        Returns features and indexes of features to keep.
-
-        Parameters
-        ----------
-        dataset: Dataset
-            Dataset to perform feature selection on
-
-        Returns
-        -------
-        features_to_keep: np.ndarray
-            Array containing the indexes of the features to keep.
-        """
-        fs = np.stack(dataset.X, axis=0)
-        y = dataset.y
-        sp = SelectPercentile(self.score_func, percentile=self.percentil)
-        sp.fit_transform(fs, y)
-        return sp.get_support(indices=True)
+        super().__init__(SelectPercentile(score_func=score_func, percentile=percentil))
 
 
 # TODO: takes too long to run, check if its normal or a code problem
 class RFECVFS(BaseFeatureSelector):
     """
     Class for RFECV feature selection.
 
@@ -229,49 +193,24 @@
             scorer(estimator, X, y).
         verbose: in
             Controls verbosity of output.
         n_jobs: int
             Number of cores to run in parallel while fitting across folds. None means 1 unless in a
             joblib.parallel_backend context. -1 means using all processors.
         """
-        super().__init__()
         if estimator is None:
-            self.estimator = RandomForestClassifier(n_jobs=n_jobs)
-        else:
-            self.estimator = estimator
-        self.step = step
-        self.min_features_to_select = min_features_to_select
-        self.cv = cv
-        self.scoring = scoring
-        self.verbose = verbose
-
-    def _select_features(self, dataset: Dataset) -> np.ndarray:
-        """
-        Returns features and indexes of features to keep.
-
-        Parameters
-        ----------
-        dataset: Dataset
-            Dataset to perform feature selection on
+            estimator = RandomForestClassifier(n_jobs=n_jobs)
 
-        Returns
-        -------
-        features_to_keep: np.ndarray
-            Array containing the indexes of the features to keep.
-        """
-        fs = np.stack(dataset.X, axis=0)
-        y = dataset.y
-        rfe = RFECV(self.estimator,
-                    step=self.step,
-                    cv=self.cv,
-                    min_features_to_select=self.min_features_to_select,
-                    scoring=self.scoring,
-                    verbose=self.verbose)
-        rfe.fit_transform(fs, y)
-        return rfe.get_support(indices=True)
+        rfe = RFECV(estimator=estimator,
+                    step=step,
+                    cv=cv,
+                    min_features_to_select=min_features_to_select,
+                    scoring=scoring,
+                    verbose=verbose)
+        super().__init__(rfe)
 
 
 class SelectFromModelFS(BaseFeatureSelector):
     """
     Class for Select From Model feature selection.
 
     Meta-transformer for selecting features based on importance weights.
@@ -279,15 +218,14 @@
 
     def __init__(self,
                  estimator: callable = None,
                  threshold: Union[str, float] = None,
                  prefit: bool = False,
                  norm_order: int = 1,
                  max_features: int = None):
-
         """
         Initialize this SelectFromModelFS Feature Selector.
 
         Parameters
         ----------
         estimator: callable
             The base estimator from which the transformer is built. This can be both a fitted (if prefit is set to True)
@@ -306,47 +244,22 @@
             to do feature selection.
         norm_order: int
             Order of the norm used to filter the vectors of coefficients below threshold in the case where the
             coef_ attribute of the estimator is of dimension 2.
         max_features: int
             The maximum number of features to select. To only select based on max_features, set threshold=-np.inf
         """
-        super().__init__()
         if estimator is None:
-            self.estimator = RandomForestClassifier(n_jobs=-1)
-        else:
-            self.estimator = estimator
-        self.threshold = threshold
-        self.prefit = prefit
-        self.norm_order = norm_order
-        self.max_features = max_features
-
-    def _select_features(self, dataset: Dataset) -> np.ndarray:
-        """
-        Returns features and indexes of features to keep.
-
-        Parameters
-        ----------
-        dataset: Dataset
-            Dataset to perform feature selection on
-
-        Returns
-        -------
-        features_to_keep: np.ndarray
-            Array containing the indexes of the features to keep.
-        """
-        fs = np.stack(dataset.X, axis=0)
-        y = dataset.y
-        sfm = SelectFromModel(self.estimator,
-                              threshold=self.threshold,
-                              prefit=self.prefit,
-                              norm_order=self.norm_order,
-                              max_features=self.max_features)
-        sfm.fit_transform(fs, y)
-        return sfm.get_support(indices=True)
+            estimator = RandomForestClassifier(n_jobs=-1)
+        sfm = SelectFromModel(estimator=estimator,
+                              threshold=threshold,
+                              prefit=prefit,
+                              norm_order=norm_order,
+                              max_features=max_features)
+        super().__init__(sfm)
 
 
 class BorutaAlgorithm(BaseFeatureSelector):
     """
     Class for Boruta feature selection.
 
     Boruta is an all-relevant feature selection method. It is based on the idea that all features are relevant until
@@ -399,59 +312,75 @@
             Random state to use.
         verbose: int
             Controls verbosity of output.
             - 0: no output
             - 1: displays iteration number
             - 2: which features have been selected already
         """
-        super().__init__()
         self.support_weak = support_weak
         if estimator is None:
             if task == "classification":
-                self.estimator = RandomForestClassifier(
+                estimator = RandomForestClassifier(
                     n_jobs=-1,
                     max_depth=5
                 )
             elif task == "regression":
-                self.estimator = RandomForestRegressor(
+                estimator = RandomForestRegressor(
                     n_jobs=-1,
                     max_depth=5
                 )
-        else:
-            self.estimator = estimator
 
-        self.boruta = BorutaPy(
-            self.estimator,
+        boruta = BorutaPy(
+            estimator,
             n_estimators,
             perc,
             alpha,
             two_step,
             max_iter,
             random_state,
             verbose
         )
+        super().__init__(boruta)
 
-    def _select_features(self, dataset: Dataset) -> np.ndarray:
+    def _fit(self, dataset: Dataset) -> 'BorutaAlgorithm':
         """
-        Returns features and indexes of features to keep.
+        Fit the Boruta Algorithm.
 
         Parameters
         ----------
         dataset: Dataset
-            Dataset to perform feature selection on
+            Dataset to fit
 
         Returns
         -------
-        features_to_keep: np.ndarray
-            Array containing the indexes of the features to keep.
+        self: BorutaAlgorithm
+            The fitted BorutaAlgorithm
         """
         fs = np.stack(dataset.X, axis=0)
         y = dataset.y
-        self.boruta.fit(fs, y)
-        self.boruta.transform(fs, weak=self.support_weak)
-        support = [i for i, boolean in enumerate(self.boruta.support_) if boolean]
+        self.feature_selector.fit(fs, y)
+        return self
+
+    def _transform(self, dataset: Dataset) -> Dataset:
+        """
+        Transform the dataset using the selected features.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            Dataset to transform
+
+        Returns
+        -------
+        transformed_dataset: Dataset
+            Transformed dataset
+        """
+        fs = np.stack(dataset.X, axis=0)
+        self.feature_selector.transform(fs, weak=self.support_weak)
+        support = [i for i, boolean in enumerate(self.feature_selector.support_) if boolean]
         if self.support_weak:
-            weak_support = [i for i, boolean in enumerate(self.boruta.support_weak_) if boolean]
+            weak_support = [i for i, boolean in enumerate(self.feature_selector.support_weak_) if boolean]
             features_to_keep = list(set.union(set(support), set(weak_support)))
         else:
             features_to_keep = support
-        return np.array(features_to_keep)
+        dataset.select_features_by_index(list(features_to_keep))
+        return dataset
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/loaders/_utils.py` & `DeepMol-1.0.0/src/deepmol/loaders/_utils.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/loaders/loaders.py` & `DeepMol-1.0.0/src/deepmol/loaders/loaders.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/loggers/logger.py` & `DeepMol-1.0.0/src/deepmol/loggers/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,23 +84,25 @@
             self.logger.setLevel(self.level)
         self.create_handlers()
 
     def create_handlers(self):
         """
         Creates the handlers for the logger.
         """
-        self.logger = logging.getLogger(self.file_path)
 
-        self.console_handler = logging.StreamHandler(sys.stdout)
-        self.console_handler.setFormatter(self.formatter)
-        self.file_handler = TimedRotatingFileHandler(self.file_path, when='midnight')
-        self.file_handler.setFormatter(self.formatter)
-        self.logger.addHandler(self.file_handler)
-        self.logger.addHandler(self.console_handler)
-        self.logger.setLevel(self.level)
+        if not self.logger:
+            self.logger = logging.getLogger(self.file_path)
+            self.console_handler = logging.StreamHandler(sys.stdout)
+            self.console_handler.setFormatter(self.formatter)
+            self.file_handler = TimedRotatingFileHandler(self.file_path, when='midnight')
+            self.file_handler.setFormatter(self.formatter)
+            if not self.logger.hasHandlers():
+                self.logger.addHandler(self.file_handler)
+                self.logger.addHandler(self.console_handler)
+            self.logger.setLevel(self.level)
 
     def set_file_path(self, file_path: str):
         """
         Sets the file path of the logger.
 
         Parameters
         ----------
@@ -209,23 +211,27 @@
         Returns
         -------
         d: dict
             The state of the logger.
         """
         d = self.__dict__.copy()
         d['logger'] = d['logger'].name
-        d['console_handler'] = d['console_handler'].name
-        d['file_handler'] = d['file_handler'].name
+        if 'console_handler' in d:
+            d['console_handler'] = 'console_handler'
+        if 'file_handler' in d:
+            d['file_handler'] = 'file_handler'
 
         return d
 
     def __setstate__(self, d: dict):
         """
         Sets the state of the logger.
 
         Parameters
         ----------
         d: dict
             The dictionary to set the state of the logger.
 
         """
+
+        d['logger'] = logging.getLogger(d['file_path'])
         self.__dict__.update(d)
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/metrics/metrics.py` & `DeepMol-1.0.0/src/deepmol/metrics/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,11 +116,16 @@
         metric_value: float
             The computed value of the metric.
         """
         # deal with metrics that require 0 or 1 values not probabilities
         try:
             metric_value = self.metric(y_true, y_pred, **kwargs)
         except ValueError as e:
-            # round values in y_ped to 0 or 1
-            y_pred_rounded = np.round(y_pred)
-            metric_value = self.metric(y_true, y_pred_rounded, **kwargs)
+            try:
+                # round values in y_ped to 0 or 1
+                y_pred_rounded = np.round(y_pred)
+                metric_value = self.metric(y_true, y_pred_rounded, **kwargs)
+            except ValueError as e:
+                # transform y_pred [[0, 1], [1, 0]] to [1, 0]
+                y_pred_single = np.argmax(y_pred, axis=1)
+                metric_value = self.metric(y_true, y_pred_single, **kwargs)
         return metric_value
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/metrics/metrics_functions.py` & `DeepMol-1.0.0/src/deepmol/metrics/metrics_functions.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/models/base_models.py` & `DeepMol-1.0.0/src/deepmol/models/base_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from keras.dtensor.optimizers import Adadelta, RMSprop
 from keras.layers import BatchNormalization, GaussianNoise
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.svm import SVC
 from tensorflow.keras import Sequential, regularizers
 from tensorflow.keras.layers import Dense, Dropout, Reshape, Conv1D, Flatten
 from tensorflow.keras import layers
+import tensorflow as tf
 
 
 # TODO: add more pre-defined models
 
 
 def rf_model_builder(n_estimators: int = 100,
                      max_features: Union[int, float, str] = 'auto',
@@ -242,8 +243,7 @@
     metrics = {task_names[i]: metrics[i] for i in range(len(task_names))}
     # Compile the model with different loss functions and metrics for each task
     model.compile(
         optimizer=keras.optimizers.Adam(learning_rate=0.001),
         loss=losses,
         metrics=metrics)
     return model
-
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/models/ensembles.py` & `DeepMol-1.0.0/src/deepmol/models/ensembles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from abc import ABC, abstractmethod
 from typing import List
 
 import numpy as np
 
+from deepmol.base import Predictor
 from deepmol.datasets import Dataset
 from deepmol.evaluator.evaluator import Evaluator
 from deepmol.metrics.metrics import Metric
 from deepmol.models.models import Model
 
 
-class Ensemble(ABC):
+class Ensemble(ABC, Predictor):
     """
     Abstract class for ensembles of models.
     """
 
     def __init__(self, models: List[Model]):
         """
         Initializes an ensemble of models.
 
         Parameters
         ----------
         models: List[Model]
             List of models to be used in the ensemble.
         """
+        super().__init__()
         self.models = models
 
     def fit(self, dataset: Dataset):
         """
         Fits the models to the specified dataset.
         """
         for model in self.models:
@@ -62,17 +64,15 @@
         multitask_scores: dict
             Dictionary mapping names of metrics to metric scores.
         all_task_scores: dict, optional
             If `per_task_metrics == True` is passed as a keyword argument, then returns a second dictionary of scores
             for each task separately.
         """
         evaluator = Evaluator(self, dataset)
-        return evaluator.compute_model_performance(metrics,
-                                                   per_task_metrics=per_task_metrics,
-                                                   n_classes=n_classes)
+        return evaluator.compute_model_performance(metrics, per_task_metrics=per_task_metrics)
 
 
 class VotingClassifier(Ensemble):
     """
     VotingClassifier Ensemble.
     It uses a voting strategy to predict the labels of a dataset.
     """
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/models/keras_models.py` & `DeepMol-1.0.0/src/deepmol/models/sklearn_models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,101 +1,96 @@
-from deepmol.models.models import Model
-from deepmol.models.sklearn_models import SklearnModel
-from deepmol.metrics.metrics import Metric
-from deepmol.splitters.splitters import RandomSplitter, SingletaskStratifiedSplitter
-from typing import Sequence
+import os
+
 import numpy as np
+from sklearn.base import BaseEstimator
+
+from deepmol.models._utils import save_to_disk, _get_splitter, load_from_disk
+from deepmol.models.models import Model
 from deepmol.datasets import Dataset
-from keras.wrappers.scikit_learn import KerasClassifier, KerasRegressor
+from deepmol.splitters.splitters import Splitter
+from deepmol.metrics.metrics import Metric
+
 from sklearn.base import clone
 
+from deepmol.utils.utils import normalize_labels_shape
 
-# Only for sequential single input models
-class KerasModel(Model):
+
+class SklearnModel(Model):
     """
-    Wrapper class that wraps keras models.
-    The `KerasModel` class provides a wrapper around keras models that allows this models to be trained on `Dataset`
-    objects.
+    Wrapper class that wraps scikit-learn models.
+    The `SklearnModel` class provides a wrapper around scikit-learn models that allows scikit-learn models to be
+    trained on `Dataset` objects and evaluated with the metrics in Metrics.
     """
 
-    def __init__(self,
-                 model_builder: callable,
-                 mode: str = 'classification',
-                 model_dir: str = None,
-                 loss: str = 'binary_crossentropy',
-                 optimizer: str = 'adam',
-                 learning_rate: float = 0.001,
-                 epochs: int = 150,
-                 batch_size: int = 10,
-                 verbose: int = 0,
-                 **kwargs) -> None:
+    def __init__(self, model: BaseEstimator, mode: str = None, model_dir: str = None, **kwargs):
         """
-        Initializes a `KerasModel` object.
+        Initializes a `SklearnModel` object.
 
         Parameters
         ----------
-        model_builder: callable
-            A function that builds a keras model.
+        model: BaseEstimator
+          The model instance which inherits a scikit-learn `BaseEstimator` Class.
         mode: str
-            The mode of the model. Can be either 'classification' or 'regression'.
+            'classification' or 'regression'
         model_dir: str
-            The directory to save the model to.
-        loss: str
-            The loss function to use.
-        optimizer: str
-            The optimizer to use.
-        learning_rate: float
-            The learning rate to use.
-        epochs: int
-            The number of epochs to train for.
-        batch_size: int
-            The batch size to use.
-        verbose: int
-            The verbosity of the model.
+          If specified the model will be stored in this directory. Else, a temporary directory will be used.
+        kwargs: dict
+            Additional keyword arguments.
         """
-        super().__init__(model_builder, model_dir, **kwargs)
+        super().__init__(model, model_dir, **kwargs)
         self.mode = mode
-        self.loss = loss
-        self.optimizer = optimizer
-        self.learning_rate = learning_rate
-        self.model_type = 'keras'
-        self.batch_size = batch_size
-        self.epochs = epochs
-        self.model_builder = model_builder
-        self.verbose = verbose
-
-        if mode == 'classification':
-            self.model = KerasClassifier(build_fn=model_builder, epochs=epochs, batch_size=batch_size,
-                                         verbose=verbose, **kwargs)
-        elif mode == 'regression':
-            self.model = KerasRegressor(build_fn=model_builder, nb_epoch=epochs, batch_size=batch_size, verbose=verbose,
-                                        **kwargs)
-        else:
-            self.model = model_builder
+        self.parameters_to_save = {'mode': self.mode}
 
-    def fit(self, dataset: Dataset, **kwargs) -> None:
+    @property
+    def model_type(self):
         """
-        Fits keras model to data.
+        Returns the type of the model.
+        """
+        return 'sklearn'
+
+    def fit_on_batch(self, dataset: Dataset) -> None:
+        """
+        Fits model on batch of data.
+
+        Parameters
+        ----------
+        dataset: Dataset
+          Dataset to train on.
+        """
+
+    def get_task_type(self) -> str:
+        """
+        Returns the task type of the model.
+        """
+
+    def get_num_tasks(self) -> int:
+        """
+        Returns the number of tasks.
+        """
+
+    def _fit(self, dataset: Dataset) -> None:
+        """
+        Fits scikit-learn model to data.
 
         Parameters
         ----------
         dataset: Dataset
             The `Dataset` to train this model on.
-        kwargs:
-            Additional arguments to pass to `fit` method of the keras model.
+
+        Returns
+        -------
+        BaseEstimator
+            The trained scikit-learn model.
         """
-        if self.mode != dataset.mode:
-            raise ValueError('Dataset mode does not match model mode.')
-        features = dataset.X.astype('float32')
-        if len(dataset.label_names) == 1:
-            y = np.squeeze(dataset.y)
-        else:
-            targets = [dataset.y[:, i] for i in range(len(dataset.label_names))]
-            y = {f"{dataset.label_names[i]}": targets[i] for i in range(len(dataset.label_names))}
-        self.model.fit(features, y, **kwargs)
+        if self.mode is not None and self.mode != dataset.mode:
+            raise ValueError(f'The mode of the dataset must match the mode of the model. '
+                             f'Got {dataset.mode} for dataset and {self.mode} for model.')
+        features = dataset.X
+        y = np.squeeze(dataset.y)
+        return self.model.fit(features, y)
 
     def predict(self, dataset: Dataset) -> np.ndarray:
         """
         Makes predictions on dataset.
 
         Parameters
         ----------
@@ -104,116 +99,163 @@
 
         Returns
         -------
         np.ndarray
           The value is a return value of `predict_proba` or `predict` method of the scikit-learn model. If the
           scikit-learn model has both methods, the value is always a return value of `predict_proba`.
         """
-        try:
-            return self.model.predict_proba(dataset.X.astype('float32'))
-        except AttributeError:
-            self.logger.info(str(self.model))
-            self.logger.info(str(type(self.model)))
-            return self.model.predict(dataset.X.astype('float32'))
+        predictions = self.model.predict(dataset.X)
+
+        if not dataset.y.shape == np.array(predictions).shape:
+            predictions = normalize_labels_shape(predictions, dataset.n_tasks)
+
+        return predictions
 
-    def predict_on_batch(self, X: Dataset) -> np.ndarray:
+    def predict_proba(self, dataset: Dataset) -> np.ndarray:
+        """
+        Makes predictions on dataset.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            Dataset to make prediction on.
+
+        Returns
+        -------
+        np.ndarray
+        """
+        predictions = self.model.predict_proba(dataset.X)
+
+        if not dataset.y.shape == np.array(predictions).shape:
+            predictions = normalize_labels_shape(predictions, dataset.n_tasks)
+
+        return predictions
+
+    def predict_on_batch(self, dataset: Dataset) -> np.ndarray:
         """
         Makes predictions on batch of data.
 
         Parameters
         ----------
-        X: Dataset
+        dataset: Dataset
           Dataset to make prediction on.
 
         Returns
         -------
         np.ndarray
             numpy array of predictions.
         """
-        return super(KerasModel, self).predict(X)
+        return super(SklearnModel, self).predict(dataset)
 
-    def fit_on_batch(self, X: Sequence, y: Sequence):
-        """
-        Fits model on batch of data.
+    def save(self, folder_path: str = None):
         """
+        Saves scikit-learn model to disk using joblib, numpy or pickle.
+        Supported extensions: .joblib, .pkl, .npy
 
-    def reload(self) -> None:
-        """
-        Reloads the model from disk.
+        Parameters
+        ----------
+        folder_path: str
+            Folder path to save model to.
         """
+        if folder_path is None:
+            model_path = self.get_model_filename(self.model_dir)
+        else:
+            if "." in folder_path:
+                raise ValueError("folder_path should be a folder, not a file")
+            os.makedirs(folder_path, exist_ok=True)
+            model_path = self.get_model_filename(folder_path)
+
+        save_to_disk(self.model, model_path)
+
+        # change file path to keep the extension but add _params
+        parameters_file_path = model_path.split('.')[0] + '_params.' + model_path.split('.')[1]
+        save_to_disk(self.parameters_to_save, parameters_file_path)
 
-    def save(self) -> None:
-        """
-        Saves the model to disk.
+    @classmethod
+    def load(cls, folder_path: str, **kwargs) -> 'SklearnModel':
         """
+        Loads scikit-learn model from joblib or pickle file on disk.
+        Supported extensions: .joblib, .pkl
 
-    def get_task_type(self) -> str:
-        """
-        Returns the task type of the model.
-        """
+        Parameters
+        ----------
+        folder_path: str
+            Path to model file.
 
-    def get_num_tasks(self) -> int:
-        """
-        Returns the number of tasks of the model.
+        Returns
+        -------
+        SklearnModel
+            The loaded scikit-learn model.
         """
+        if "." in folder_path:
+            raise ValueError("model_path should be a folder, not a file")
+        model_path = cls.get_model_filename(folder_path)
+        model = load_from_disk(model_path)
+        # change file path to keep the extension but add _params
+        parameters_file_path = model_path.split('.')[0] + '_params.' + model_path.split('.')[1]
+        params = load_from_disk(parameters_file_path)
+        instance = cls(model=model, model_dir=model_path, **params)
+        return instance
 
     def cross_validate(self,
                        dataset: Dataset,
                        metric: Metric,
+                       splitter: Splitter = None,
                        folds: int = 3):
         """
-        Cross validates the model on a dataset.
+        Performs cross-validation on a dataset.
 
         Parameters
         ----------
         dataset: Dataset
-            The `Dataset` to cross validate on.
+            Dataset to perform cross-validation on.
         metric: Metric
-            The metric to use for cross validation.
+            Metric to evaluate model performance.
+        splitter: Splitter
+            Splitter to use for cross-validation.
         folds: int
-            The number of folds to use for cross validation.
+            Number of folds to use for cross-validation.
 
         Returns
         -------
         Tuple[SKlearnModel, float, float, List[float], List[float], float, float]
             The first element is the best model, the second is the train score of the best model, the third is the train
             score of the best model, the fourth is the test scores of all models, the fifth is the average train scores
             of all folds and the sixth is the average test score of all folds.
         """
-        # TODO: add option to choose between splitters
-        splitter = None
-        if dataset.mode == 'classification':
-            splitter = SingletaskStratifiedSplitter()
-        if dataset.mode == 'regression':
-            splitter = RandomSplitter()
-
-        assert splitter is not None
+        if splitter is None:
+            splitter = _get_splitter(dataset)
 
         datasets = splitter.k_fold_split(dataset, folds)
 
         train_scores = []
         train_score_best_model = 0
         avg_train_score = 0
 
         test_scores = []
         test_score_best_model = 0
         avg_test_score = 0
         best_model = None
+        split = 1
+
+        print("Computing K-fold cross validation")
         for train_ds, test_ds in datasets:
+            split += 1
             dummy_model = clone(SklearnModel(model=self.model))
 
             dummy_model.fit(train_ds)
 
-            train_score = dummy_model.evaluate(train_ds, metric)
+            train_score = dummy_model.evaluate(train_ds, [metric])[0]
             train_scores.append(train_score[metric.name])
             avg_train_score += train_score[metric.name]
 
-            test_score = dummy_model.evaluate(test_ds, metric)
+            test_score = dummy_model.evaluate(test_ds, [metric])[0]
             test_scores.append(test_score[metric.name])
             avg_test_score += test_score[metric.name]
 
             if test_score[metric.name] > test_score_best_model:
                 test_score_best_model = test_score[metric.name]
                 train_score_best_model = train_score[metric.name]
                 best_model = dummy_model
 
-        return best_model, train_score_best_model, test_score_best_model, train_scores, test_scores, avg_train_score / folds, avg_test_score / folds
+        return best_model, train_score_best_model, test_score_best_model, \
+            train_scores, test_scores, avg_train_score / folds, avg_test_score / folds
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/models/models.py` & `DeepMol-1.0.0/src/deepmol/models/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import os
 import shutil
 import tempfile
-from typing import List, Sequence, Union, Tuple, Dict
+from abc import ABC
+from typing import List, Union, Tuple, Dict
 import numpy as np
+
+from deepmol.base import Predictor
 from deepmol.datasets import Dataset
 from deepmol.evaluator.evaluator import Evaluator
 from deepmol.loggers.logger import Logger
 from deepmol.metrics.metrics import Metric
 
 from sklearn.base import BaseEstimator
 
 
-class Model(BaseEstimator):
+class Model(BaseEstimator, Predictor, ABC):
     """
     Abstract base class for ML/DL models.
     """
 
     def __init__(self, model: BaseEstimator = None, model_dir: str = None, **kwargs) -> None:
         """
         Abstract class for all models.
@@ -30,61 +33,76 @@
             directory.
         """
         if self.__class__.__name__ == "Model":
             raise ValueError(
                 "This constructor is for an abstract class and should never be called directly. Can only call from "
                 "subclass constructors.")
 
+        super().__init__()
+
         self.model_dir_is_temp = False
 
         if model_dir is not None:
             if not os.path.exists(model_dir):
                 os.makedirs(model_dir)
         else:
             model_dir = tempfile.mkdtemp()
             self.model_dir_is_temp = True
 
-        self.model_dir = model_dir
+        self._model_dir = model_dir
         self.model = model
         self.model_class = model.__class__
 
         self.logger = Logger()
 
     def __del__(self):
         """
         Delete model directory if it was created by this object.
         """
         if 'model_dir_is_temp' in dir(self) and self.model_dir_is_temp:
             shutil.rmtree(self.model_dir)
 
-    def fit_on_batch(self, X: Sequence, y: Sequence):
+    def fit_on_batch(self, dataset: Dataset) -> None:
         """
         Perform a single step of training.
 
         Parameters
         ----------
-        X: np.ndarray
-            the inputs for the batch
-        y: np.ndarray
-            the labels for the batch
+        dataset: Dataset
+            Dataset object.
         """
 
-    def predict_on_batch(self, X: Sequence):
+    def predict_on_batch(self, dataset: Dataset) -> np.ndarray:
         """
         Makes predictions on given batch of new data.
 
         Parameters
         ----------
-        X: np.ndarray
-            array of features
-        """
+        dataset: Dataset
+            Dataset object.
 
-    def reload(self) -> None:
+        Returns
+        -------
+        np.ndarray
+            Predicted values.
+        """
+    @classmethod
+    def load(cls, folder_path: str) -> 'Model':
         """
         Reload trained model from disk.
+
+        Parameters
+        ----------
+        folder_path: str
+            Path to folder where model is stored.
+
+        Returns
+        -------
+        Model
+            Model object.
         """
 
     @staticmethod
     def get_model_filename(model_dir: str) -> str:
         """
         Given model directory, obtain filename for the model itself.
 
@@ -94,15 +112,15 @@
             Path to directory where model is stored.
 
         Returns
         -------
         str
             Path to model file.
         """
-        return os.path.join(model_dir, "model.joblib")
+        return os.path.join(model_dir, "model.pkl")
 
     @staticmethod
     def get_params_filename(model_dir: str) -> str:
         """
         Given model directory, obtain filename for the model itself.
 
         Parameters
@@ -113,29 +131,23 @@
         Returns
         -------
         str
             Path to file where model parameters are stored.
         """
         return os.path.join(model_dir, "model_params.joblib")
 
-    def save(self) -> None:
+    def save(self, file_path: str = None) -> None:
         """
         Function for saving models.
         Each subclass is responsible for overriding this method.
-        """
-        ("Each class model must implement its own save method.")
-
-    def fit(self, dataset: Dataset):
-        """
-        Fits a model on data in a Dataset object.
 
         Parameters
         ----------
-        dataset: Dataset
-            the Dataset to train on
+        file_path: str
+            Path to file where model should be saved.
         """
 
     def predict(self, dataset: Dataset) -> np.ndarray:
         """
         Uses self to make predictions on provided Dataset object.
 
         Parameters
@@ -155,15 +167,27 @@
             # Discard any padded predictions
             y_pred_batch = y_pred_batch[:n_samples]
             y_preds.append(y_pred_batch)
         y_pred = np.concatenate(y_preds)
         return y_pred
 
     def predict_proba(self, dataset: Dataset) -> np.ndarray:
+        """
+        Uses self to make predictions on provided Dataset object.
 
+        Parameters
+        ----------
+        dataset: Dataset
+            Dataset to make prediction on
+
+        Returns
+        -------
+        np.ndarray
+            A numpy array of predictions.
+        """
         y_pred = self.model.predict_proba(dataset.X)
         return y_pred
 
     def evaluate(self,
                  dataset: Dataset,
                  metrics: Union[List[Metric], Metric],
                  per_task_metrics: bool = False) -> Tuple[Dict, Union[None, Dict]]:
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/models/sklearn_models.py` & `DeepMol-1.0.0/src/deepmol/compound_featurization/_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,193 +1,245 @@
-from typing import Sequence
+from typing import List, Dict, Tuple
 
 import numpy as np
-from sklearn.base import BaseEstimator
+from IPython.core.display import SVG
+from deepchem.utils import ConformerGenerator
+from rdkit import DataStructs, Chem
+from rdkit.Chem import Mol, AllChem, rdDepictor
+from rdkit.Chem.Draw import rdMolDraw2D
 
-from deepmol.models._utils import save_to_disk
-from deepmol.models.models import Model
-from deepmol.datasets import Dataset
-from deepmol.splitters.splitters import RandomSplitter, SingletaskStratifiedSplitter
-from deepmol.metrics.metrics import Metric
-
-from deepmol.utils.utils import load_from_disk
-
-from sklearn.base import clone
-
-
-class SklearnModel(Model):
-    """
-    Wrapper class that wraps scikit-learn models.
-    The `SklearnModel` class provides a wrapper around scikit-learn models that allows scikit-learn models to be
-    trained on `Dataset` objects and evaluated with the metrics in Metrics.
-    """
-
-    def __init__(self, model: BaseEstimator, mode: str = None, model_dir: str = None, **kwargs):
-        """
-        Initializes a `SklearnModel` object.
-
-        Parameters
-        ----------
-        model: BaseEstimator
-          The model instance which inherits a scikit-learn `BaseEstimator` Class.
-        mode: str
-            'classification' or 'regression'
-        model_dir: str
-          If specified the model will be stored in this directory. Else, a temporary directory will be used.
-        kwargs: dict
-            Additional keyword arguments.
-        """
-        super().__init__(model, model_dir, **kwargs)
-        self.mode = mode
-        self.model_type = 'sklearn'
-
-    def fit_on_batch(self, X: Sequence, y: Sequence):
-        """
-        Fits model on batch of data.
-        """
-
-    def get_task_type(self) -> str:
-        """
-        Returns the task type of the model.
-        """
-
-    def get_num_tasks(self) -> int:
-        """
-        Returns the number of tasks.
-        """
-
-    def fit(self, dataset: Dataset) -> None:
-        """
-        Fits scikit-learn model to data.
-
-        Parameters
-        ----------
-        dataset: Dataset
-            The `Dataset` to train this model on.
-
-        Returns
-        -------
-        BaseEstimator
-            The trained scikit-learn model.
-        """
-        if self.mode is not None and self.mode != dataset.mode:
-            raise ValueError(f'The mode of the dataset must match the mode of the model. '
-                             f'Got {dataset.mode} for dataset and {self.mode} for model.')
-        features = dataset.X
-        y = np.squeeze(dataset.y)
-        return self.model.fit(features, y)
-
-    def predict(self, dataset: Dataset) -> np.ndarray:
-        """
-        Makes predictions on dataset.
-
-        Parameters
-        ----------
-        dataset: Dataset
-          Dataset to make prediction on.
-
-        Returns
-        -------
-        np.ndarray
-          The value is a return value of `predict_proba` or `predict` method of the scikit-learn model. If the
-          scikit-learn model has both methods, the value is always a return value of `predict_proba`.
-        """
+from deepmol.loggers import Logger
+
+
+def find_maximum_number_atoms(molecules: List[Mol]) -> int:
+    """
+    Finds maximum number of atoms within a set of molecules
+
+    Parameters
+    ----------
+    molecules: List[Mol]
+        List of rdkit mol objects
+
+    Returns
+    -------
+    best: int
+        Maximum number of atoms in a molecule in the list.
+    """
+    best = 0
+    for i, mol in enumerate(molecules):
+        atoms = mol.GetNumAtoms()
+        if atoms > best:
+            best = atoms
+    return best
+
+
+def get_conformers(molecules: List[Mol], generator: ConformerGenerator) -> List[Mol]:
+    """
+    Gets conformers for molecules with a specific generator
+
+    Parameters
+    ----------
+    molecules: List[Mol]
+        List of rdkit mol objects
+    generator: ConformerGenerator
+        DeepChem conformer generator.
+
+    Returns
+    -------
+    new_conformations: List[Mol]
+        List of rdkit mol objects with conformers.
+    """
+    new_conformations = []
+    for i, mol in enumerate(molecules):
+        try:
+            conf = generator.generate_conformers(mol)
+            new_conformations.append(conf)
+        except Exception as e:
+            logger = Logger()
+            logger.error(f"Could not generate conformers for molecule {i} with error {e}")
+            new_conformations.append([])
+    return new_conformations
+
+
+def get_dictionary_from_smiles(smiles: List[str], max_len: int) -> Dict[str, int]:
+    """
+    Dictionary of character to index mapping
+    Adapted from deepchem.
+
+    Parameters
+    ----------
+    smiles: List[str]
+        List of SMILES string
+    max_len: int
+        Maximum length of SMILES string
+
+    Returns
+    -------
+    dictionary: Dict[str, int]
+        Dictionary of character to index mapping
+    """
+
+    pad_token = "<pad>"
+    out_of_vocab_token = "<unk>"
+
+    char_set = set()
+    for smile in smiles:
+        if len(smile) <= max_len:
+            char_set.update(set(smile))
+
+    unique_char_list = list(char_set) + [pad_token, out_of_vocab_token]
+    dictionary = {letter: idx for idx, letter in enumerate(unique_char_list)}
+    return dictionary
+
+
+def calc_morgan_fingerprints(mols: np.ndarray, **kwargs) -> List[np.ndarray]:
+    """
+    Calculates Morgan fingerprints for a array of molecules.
+
+    Parameters
+    ----------
+    mols: np.ndarray
+        Array of rdkit mol objects
+    kwargs:
+        Keyword arguments for the Morgan fingerprint calculation.
+
+    Returns
+    -------
+    fps: List[np.ndarray]
+        List of Morgan fingerprints
+    """
+    if "radius" not in kwargs:
+        kwargs["radius"] = 2
+    if "nBits" not in kwargs:
+        kwargs["nBits"] = 1024
+    fps = [AllChem.GetMorganFingerprintAsBitVect(m, **kwargs) for m in mols]
+    return fps
+
+
+def calc_similarity(first_fp_idx: int, second_fp_idx: int, fps: List[np.ndarray]) -> Tuple[int, int, float]:
+    """
+    Calculates the Tanimoto similarity between two fingerprints.
+
+    Parameters
+    ----------
+    first_fp_idx: int
+        Index of the first fingerprint
+    second_fp_idx: int
+        Index of the second fingerprint
+    fps: List[np.ndarray]
+        List of Morgan fingerprints
+
+    Returns
+    -------
+    i: int
+        Index of the first fingerprint
+    j: int
+        Index of the second fingerprint
+    similarity: float
+        Tanimoto similarity between the two fingerprints
+    """
+    return first_fp_idx, second_fp_idx, DataStructs.TanimotoSimilarity(fps[first_fp_idx], fps[second_fp_idx])
+
+
+def prepare_mol(mol: Mol, kekulize: bool):
+    """
+    Prepare a molecule for drawing.
+
+    Parameters
+    ----------
+    mol: Mol
+        Molecule to prepare.
+    kekulize: bool
+        If True, the molecule is kekulized.
+
+    Returns
+    -------
+    mc: Mol
+        Prepared molecule.
+    """
+    mc = Chem.Mol(mol.ToBinary())
+    if kekulize:
         try:
-            return self.model.predict_proba(dataset.X)
-        except AttributeError:
-            return self.model.predict(dataset.X)
-
-    def predict_on_batch(self, dataset: Dataset) -> np.ndarray:
-        """
-        Makes predictions on batch of data.
-
-        Parameters
-        ----------
-        dataset: Dataset
-          Dataset to make prediction on.
-
-        Returns
-        -------
-        np.ndarray
-            numpy array of predictions.
-        """
-        return super(SklearnModel, self).predict(dataset)
-
-    def save(self):
-        """
-        Saves scikit-learn model to disk using joblib.
-        """
-        save_to_disk(self.model, self.get_model_filename(self.model_dir))
-
-    def reload(self):
-        """
-        Loads scikit-learn model from joblib file on disk.
-        """
-        self.model = load_from_disk(self.get_model_filename(self.model_dir))
-
-    def cross_validate(self,
-                       dataset: Dataset,
-                       metric: Metric,
-                       folds: int = 3):
-        """
-        Performs cross-validation on a dataset.
-
-        Parameters
-        ----------
-        dataset: Dataset
-            Dataset to perform cross-validation on.
-        metric: Metric
-            Metric to evaluate model performance.
-        folds: int
-            Number of folds to use for cross-validation.
-
-        Returns
-        -------
-        Tuple[SKlearnModel, float, float, List[float], List[float], float, float]
-            The first element is the best model, the second is the train score of the best model, the third is the train
-            score of the best model, the fourth is the test scores of all models, the fifth is the average train scores
-            of all folds and the sixth is the average test score of all folds.
-        """
-        # TODO: add option to choose between splitters
-        if dataset.mode == 'classification':
-            splitter = SingletaskStratifiedSplitter()
-            datasets = splitter.k_fold_split(dataset, folds)
-        elif dataset.mode == 'regression':
-            splitter = RandomSplitter()
-            datasets = splitter.k_fold_split(dataset, folds)
-        else:
-            try:
-                splitter = SingletaskStratifiedSplitter()
-                datasets = splitter.k_fold_split(dataset, folds)
-            except Exception as e:
-                splitter = RandomSplitter()
-                datasets = splitter.k_fold_split(dataset, folds)
-
-        train_scores = []
-        train_score_best_model = 0
-        avg_train_score = 0
-
-        test_scores = []
-        test_score_best_model = 0
-        avg_test_score = 0
-        best_model = None
-        split = 1
-        for train_ds, test_ds in datasets:
-            split += 1
-            dummy_model = clone(SklearnModel(model=self.model))
-
-            dummy_model.fit(train_ds)
-
-            train_score = dummy_model.evaluate(train_ds, metric)[0]
-            train_scores.append(train_score[metric.name])
-            avg_train_score += train_score[metric.name]
-
-            test_score = dummy_model.evaluate(test_ds, metric)[0]
-            test_scores.append(test_score[metric.name])
-            avg_test_score += test_score[metric.name]
-
-            if test_score[metric.name] > test_score_best_model:
-                test_score_best_model = test_score[metric.name]
-                train_score_best_model = train_score[metric.name]
-                best_model = dummy_model
+            Chem.Kekulize(mc)
+        except:
+            mc = Chem.Mol(mol.ToBinary())
+    if not mc.GetNumConformers():
+        rdDepictor.Compute2DCoords(mc)
+    return mc
+
+
+def mol_to_svg(mol: Mol, molSize: Tuple[int, int] = (450, 200), kekulize: bool = True, drawer: object = None, **kwargs):
+    """
+    Convert a molecule to SVG.
+
+    Parameters
+    ----------
+    mol: Mol
+        Molecule to convert.
+    molSize: Tuple[int, int]
+        Size of the molecule.
+    kekulize: bool
+        If True, the molecule is kekulized.
+    drawer: object
+        Object to draw the molecule.
+    **kwargs:
+        Additional arguments for the drawer.
+
+    Returns
+    -------
+    SVG
+        The molecule in SVG format.
+    """
+    mc = prepare_mol(mol, kekulize)
+    if drawer is None:
+        drawer = rdMolDraw2D.MolDraw2DSVG(molSize[0], molSize[1])
+    drawer.DrawMolecule(mc, **kwargs)
+    drawer.FinishDrawing()
+    svg = drawer.GetDrawingText()
+    return SVG(svg.replace('svg:', ''))
+
+
+def svg_text_to_file(svg_text: str, file_name: str):
+    """
+    Save a SVG text to a file.
 
-        return best_model, train_score_best_model, test_score_best_model, train_scores, test_scores, avg_train_score / folds, avg_test_score / folds
+    Parameters
+    ----------
+    svg_text: str
+        SVG text to save.
+    file_name: str
+        Name of the file to save.
+    """
+    with open(file_name, 'w') as f:
+        f.write(svg_text)
+
+
+def get_substructure_depiction(mol: Mol, atomID: int, radius: int, molSize: Tuple[int, int] = (450, 200)):
+    """
+    Get a depiction of a substructure.
+
+    Parameters
+    ----------
+    mol: Mol
+        Molecule to draw.
+    atomID: int
+        ID of the atom to highlight.
+    radius: int
+        Radius of the substructure.
+    molSize: Tuple[int, int]
+        Size of the molecule.
+
+    Returns
+    -------
+    SVG
+        The molecule in SVG format.
+    """
+    if radius > 0:
+        env = Chem.FindAtomEnvironmentOfRadiusN(mol, radius, atomID)
+        atomsToUse = []
+        for b in env:
+            atomsToUse.append(mol.GetBondWithIdx(b).GetBeginAtomIdx())
+            atomsToUse.append(mol.GetBondWithIdx(b).GetEndAtomIdx())
+        atomsToUse = list(set(atomsToUse))
+    else:
+        atomsToUse = [atomID]
+    return mol_to_svg(mol, molSize=molSize, highlightAtoms=atomsToUse, highlightAtomColors={atomID: (0.3, 0.3, 1)})
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/parallelism/multiprocessing.py` & `DeepMol-1.0.0/src/deepmol/parallelism/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/parameter_optimization/_utils.py` & `DeepMol-1.0.0/src/deepmol/parameter_optimization/_utils.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/parameter_optimization/deepchem_hyperparameter_optimization.py` & `DeepMol-1.0.0/src/deepmol/parameter_optimization/deepchem_hyperparameter_optimization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-"""Hyperparameter Optimization Classes for DeepchemModel models"""
 from collections import defaultdict
 from typing import Union, List
 
 import numpy as np
 from sklearn.model_selection import ParameterGrid, ParameterSampler
 
 from deepmol.datasets import Dataset
 from deepmol.metrics import Metric
+from deepmol.parameter_optimization.base_hyperparameter_optimization import HyperparameterOptimizer
 from deepmol.splitters import SingletaskStratifiedSplitter, RandomSplitter
 
 
 # TODO: it would probably be better if we tried to create a scikit-learn wrapper for DeepchemModel models,
 #  similar to KerasRegressor and KerasClassifier (not sure it would work though)
-class DeepchemBaseSearchCV(object):
+class DeepchemBaseSearchCV(HyperparameterOptimizer):
     """
     Base class for hyperparameter search with cross-validation for DeepChemModels.
     """
 
-    def __init__(self,
-                 model_build_fn: callable,
-                 param_grid: Union[dict, ParameterGrid, ParameterSampler],
-                 scoring: Union[Metric, List[Metric]],
-                 maximize: bool,
+    def __init__(self, model_builder: callable,
+                 params_dict: Union[dict, ParameterGrid, ParameterSampler],
+                 metric: Union[Metric, List[Metric]],
+                 maximize_metric: bool,
                  refit: bool,
                  cv: int,
                  mode: str,
                  random_state: int = None,
-                 return_train_score: bool = False):
+                 return_train_score: bool = False, **kwargs):
         """
         Initialize the hyperparameter search.
 
         Parameters
         ----------
         model_build_fn: callable
             A function that builds a DeepchemModel model.
@@ -47,58 +46,58 @@
         mode: str
             The mode of the model. Can be 'classification' or 'regression'.
         random_state: int
             The random state to use for the cross-validation.
         return_train_score: bool
             If True, return the training scores.
         """
-        self.build_fn = model_build_fn
-        self.param_grid = param_grid
-        self.metric = scoring
-        self.maximize = maximize
+        super().__init__(model_builder, "deepchem", params_dict, metric, maximize_metric, **kwargs)
+        self.metric = metric
         self.mode = mode
         self.refit = refit
         self.cv = cv
         self.random_state = random_state
         self.return_train_score = return_train_score
 
         self.best_score_ = None
         self.best_params_ = {}
         self.best_estimator_ = None
         self.cv_results_ = None
 
-    def fit(self, dataset: Dataset):
+    def fit(self, train_dataset: Dataset, validation_dataset: Dataset = None):
         """
         Run hyperparameter search with cross-validation.
 
         Parameters
         ----------
-        dataset: Dataset
+        train_dataset: Dataset
             The dataset to use for the hyperparameter search.
+        validation_dataset: Dataset
+            The dataset to use for validation. If None, use the training dataset.
         """
-        if self.mode != dataset.mode:
+        if self.mode != train_dataset.mode:
             raise ValueError(f'The mode of the model and the dataset must be the same. Got {self.mode} and '
-                             f'{dataset.mode} respectively.')
+                             f'{train_dataset.mode} respectively.')
         results_dict = defaultdict(list)
 
         # split dataset into folds
-        if dataset.mode == 'classification':
+        if train_dataset.mode == 'classification':
             splitter = SingletaskStratifiedSplitter()
         else:
             splitter = RandomSplitter()
 
-        datasets = splitter.k_fold_split(dataset, k=self.cv, seed=self.random_state)
-        for param_combination in self.param_grid:
+        datasets = splitter.k_fold_split(train_dataset, k=self.cv, seed=self.random_state)
+        for param_combination in self.params_dict:
             results_dict['params'].append(param_combination)
 
             # Cross-validation:
             train_scores = []
             test_scores = []
             for train_dataset, test_dataset in datasets:
-                model = self.build_fn(**param_combination)  # creates a new DeepchemModel
+                model = self.model_builder(**param_combination)  # creates a new DeepchemModel
                 model.fit(train_dataset)
                 train_score, _ = model.evaluate(train_dataset, [self.metric])
                 train_scores.append(train_score[self.metric.name])
                 test_score, _ = model.evaluate(test_dataset, [self.metric])
                 test_scores.append(test_score[self.metric.name])
 
             results_dict['mean_train_score'].append(np.mean(train_scores))
@@ -108,112 +107,119 @@
             results_dict['std_test_score'].append(np.std(test_scores))
             for i, (train_score, test_score) in enumerate(zip(train_scores, test_scores)):
                 train_key = 'split%s_train_score' % str(i)
                 test_key = 'split%s_test_score' % str(i)
                 results_dict[train_key].append(train_score)
                 results_dict[test_key].append(test_score)
 
-            if self.maximize:
+            if self.maximize_metric:
                 if (self.best_score_ is None) or (mean_test_score > self.best_score_):
                     self.best_score_ = mean_test_score
                     self.best_params_ = param_combination
             else:
                 if (self.best_score_ is None) or (mean_test_score < self.best_score_):
                     self.best_score_ = mean_test_score
                     self.best_params_ = param_combination
 
         self.cv_results_ = results_dict
-        self.best_estimator_ = self.build_fn(**self.best_params_)
+        self.best_estimator_ = self.model_builder(**self.best_params_)
 
         if self.refit:
-            self.best_estimator_.fit(dataset)
+            self.best_estimator_.fit(train_dataset)
+
+        return self.best_estimator_, self.best_params_, self.cv_results_
 
 
 class DeepchemGridSearchCV(DeepchemBaseSearchCV):
     """
     Hyperparameter search with cross-validation for DeepChemModels using a grid search.
     """
 
     def __init__(self,
-                 model_build_fn: callable,
-                 param_grid: Union[dict, ParameterGrid],
-                 scoring: Union[Metric, List[Metric]],
-                 maximize: bool,
+                 model_builder: callable,
+                 params_dict: Union[dict, ParameterGrid],
+                 metric: Union[Metric, List[Metric]],
+                 maximize_metric: bool,
                  refit: bool,
                  cv: int,
                  mode: str,
                  random_state: int = None,
                  return_train_score: bool = False):
         """
         Initialize the hyperparameter search.
 
         Parameters
         ----------
-        model_build_fn: callable
+        model_builder: callable
             A function that builds a DeepchemModel model.
-        param_grid: Union[dict, ParameterGrid]
+        params_dict: Union[dict, ParameterGrid]
             The hyperparameter grid to search.
-        scoring: Union[Metric, List[Metric]]
+        metric: Union[Metric, List[Metric]]
             The metric to use for scoring.
-        maximize: bool
+        maximize_metric: bool
             If True, maximize the metric. If False, minimize the metric.
         refit: bool
             If True, refit the best model on the whole dataset.
         cv: int
             The number of folds for cross-validation.
         mode: str
             The mode of the model. Can be 'classification' or 'regression'.
         random_state: int
             The random state to use for the cross-validation.
         return_train_score: bool
             If True, return the training scores.
         """
-        self.param_grid = ParameterGrid(param_grid)
-        super().__init__(model_build_fn=model_build_fn, param_grid=self.param_grid, scoring=scoring, maximize=maximize,
-                         refit=refit, cv=cv, mode=mode, random_state=random_state, return_train_score=return_train_score)
+        self.param_grid = ParameterGrid(params_dict)
+        super().__init__(model_builder=model_builder, params_dict=self.param_grid, metric=metric,
+                         maximize_metric=maximize_metric,
+                         refit=refit, cv=cv,
+                         mode=mode, random_state=random_state,
+                         return_train_score=return_train_score)
 
 
 class DeepchemRandomSearchCV(DeepchemBaseSearchCV):
     """
     Hyperparameter search with cross-validation for DeepChemModels using a random search.
     """
 
     def __init__(self,
-                 model_build_fn: callable,
-                 param_distributions: Union[dict, ParameterSampler],
-                 scoring: Union[Metric, List[Metric]],
-                 maximize: bool,
+                 model_builder: callable,
+                 params_dict: Union[dict, ParameterSampler],
+                 metric: Union[Metric, List[Metric]],
+                 maximize_metric: bool,
                  refit: bool,
                  cv: int,
                  mode: str,
                  random_state: int = None,
                  return_train_score: bool = False,
                  n_iter: int = 20):
         """
         Initialize the hyperparameter search.
 
         Parameters
         ----------
-        model_build_fn: callable
+        model_builder: callable
             A function that builds a DeepchemModel model.
-        param_distributions: Union[dict, ParameterSampler]
+        param_grid: Union[dict, ParameterSampler]
             The hyperparameter sampler to search.
-        scoring: Union[Metric, List[Metric]]
+        metric: Union[Metric, List[Metric]]
             The metrics to use for scoring.
-        maximize: bool
+        maximize_metric: bool
             If True, maximize the metric. If False, minimize the metric.
         refit: bool
             If True, refit the best model on the whole dataset.
         cv: int
             The number of folds for cross-validation.
         mode: str
             The mode of the model. Can be 'classification' or 'regression'.
         random_state: int
             The random state to use for the cross-validation.
         return_train_score: bool
             If True, return the training scores.
         n_iter: int
             The number of iterations to perform.
         """
-        self.param_grid = ParameterSampler(param_distributions, n_iter, random_state=random_state)
-        super().__init__(model_build_fn=model_build_fn, param_grid=self.param_grid, scoring=scoring, maximize=maximize,
-                         refit=refit, cv=cv, mode=mode, random_state=random_state, return_train_score=return_train_score)
+        self.param_grid = ParameterSampler(params_dict, n_iter, random_state=random_state)
+        super().__init__(model_builder=model_builder, params_dict=self.param_grid, metric=metric,
+                         maximize_metric=maximize_metric,
+                         refit=refit, cv=cv, mode=mode,
+                         random_state=random_state, return_train_score=return_train_score)
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/scalers/base_scaler.py` & `DeepMol-1.0.0/src/deepmol/scalers/base_scaler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,152 +1,113 @@
-from abc import ABC, abstractmethod
+from abc import ABC
 
 import joblib
-import numpy as np
 
+from deepmol.base import Transformer
 from deepmol.datasets import Dataset
+from deepmol.utils.decorators import modify_object_inplace_decorator
 
 
-class BaseScaler(ABC):
+class BaseScaler(ABC, Transformer):
     """
     Abstract class for all scalers. It is used to define the interface for all scalers.
     """
 
-    def __init__(self) -> None:
+    def __init__(self, scaler, columns: list = None) -> None:
         """
         Constructor for the BaseScaler class.
         """
         if self.__class__ == BaseScaler:
             raise Exception('Abstract class BaseScaler should not be instantiated')
+        super().__init__()
+        self._scaler_object = scaler
+        self.columns = columns
 
     @property
-    @abstractmethod
-    def scaler_object(self) -> object:
+    def scaler_object(self):
         """
         Returns the scaler object.
 
         Returns
         -------
-        object
+        object:
             The scaler object.
         """
+        return self._scaler_object
 
     @scaler_object.setter
-    @abstractmethod
-    def scaler_object(self, value: object) -> None:
+    def scaler_object(self, value: object):
         """
         Sets the scaler object.
 
+        Parameters
+        ----------
         value: object
             The scaler object.
         """
+        self._scaler_object = value
 
     def save(self, file_path: str) -> None:
         """
         Saves the scaler object to a file.
 
         file_path: str
             The path to the file where the scaler object will be saved.
         """
-        joblib.dump(self.scaler_object, file_path)
+        joblib.dump(self._scaler_object, file_path)
 
-    @abstractmethod
-    def load(self, file_path: str) -> object:
+    def load(self, file_path: str) -> 'BaseScaler':
         """
         Loads the scaler object from a file.
 
         file_path: str
             The path to the file where the scaler object is saved.
 
         Returns
         -------
         object
             The scaler object.
         """
+        self._scaler_object = joblib.load(file_path)
+        return self
 
-    def fit_transform(self, dataset: Dataset, columns: list = None) -> None:
+    @modify_object_inplace_decorator
+    def scale(self, dataset: Dataset) -> Dataset:
         """
-        Fits and transforms the dataset.
+        Scales the dataset.
 
         dataset: Dataset
-            The dataset to be fitted and transformed.
-        columns: list
-            The columns to be fitted and transformed.
-        """
-        if not columns:
-            columns = [i for i in range(dataset.X.shape[1])]
-        try:
-            res = self._fit_transform(dataset.X[:, columns])
-            # TODO: due to X being a property, the "set" method must choose so that it could behave as a numpy array
-            dataset.X[:, columns] = res
-        except Exception as e:
-            raise Exception(f"It was not possible to scale the data. Error: {e}")
-
-    @abstractmethod
-    def _fit_transform(self, X: np.ndarray) -> None:
+            The dataset to be scaled.
         """
-        Fits and transforms the dataset.
+        return self.fit_transform(dataset)
 
-        X: np.ndarray
-            The dataset to be fitted and transformed.
+    def _fit(self, dataset: Dataset) -> 'BaseScaler':
         """
+        Fits the scaler with the dataset.
 
-    def fit(self, dataset: Dataset, columns: list = None) -> None:
-        """
-        Fits the dataset.
-
+        Parameters
+        ----------
         dataset: Dataset
             The dataset to be fitted.
-        columns: list
-            The columns to be fitted.
-        """
-        if not columns:
-            columns = [i for i in range(dataset.X.shape[1])]
-        try:
-            self._fit(dataset.X[:, columns])
 
-        except:
-            raise Exception("It was not possible to scale the data")
-
-    @abstractmethod
-    def _fit(self, X: np.ndarray) -> None:
-        """
-        Fits the dataset.
-
-        X: np.ndarray
-            The dataset to be fitted.
+        Returns
+        -------
+        BaseScaler
+            The fitted scaler.
         """
+        if not self.columns:
+            self.columns = [i for i in range(dataset.X.shape[1])]
+        x = dataset.X[:, self.columns]
+        self._scaler_object.fit(x)
+        return self
 
-    def transform(self, dataset: Dataset, columns: list = None) -> None:
+    def _transform(self, dataset: Dataset) -> Dataset:
         """
         Transforms the dataset.
 
         dataset: Dataset
             The dataset to be transformed.
-        columns: list
-            The columns to be transformed.
-        """
-        if not columns:
-            columns = [i for i in range(dataset.X.shape[1])]
-        try:
-            res = self._transform(dataset.X[:, columns])
-            dataset.X[:, columns] = res
-
-        except:
-            raise Exception("It was not possible to scale the data")
-
-    def _transform(self, X: np.ndarray) -> None:
-        """
-        Transforms the dataset.
-
-        X: np.ndarray
-            The dataset to be transformed.
-        """
-
-    # TODO: figure out the better way of wrapping this method, as it intends to fit the dataset in batches
-    def partial_fit(self, dataset: Dataset) -> None:
-        """
-        Partially fits the dataset.
-
-        dataset: Dataset
-            The dataset to be partially fitted.
         """
+        x = dataset.X[:, self.columns]
+        res = self._scaler_object.transform(x)
+        dataset.X[:, self.columns] = res
+        return dataset
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/splitters/_utils.py` & `DeepMol-1.0.0/src/deepmol/splitters/_utils.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/splitters/splitters.py` & `DeepMol-1.0.0/src/deepmol/splitters/splitters.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,22 +330,24 @@
             np.random.seed(seed)
 
         train_idx = np.array([])
         valid_idx = np.array([])
         test_idx = np.array([])
 
         # divide idx by y value
-        classes = np.unique(dataset.y)
+
         if not force_split:
             # check if regression or classification (assume regression if there are more than 10 unique y values)
-            if len(classes) > 10:
+            classes = np.all(np.isclose(dataset.y, np.round(dataset.y), equal_nan=True))
+            if not classes:
                 raise ValueError("Cannot stratify by regression labels. Use other splitter instead. "
                                  "If you want to force the split, set force_split=True.")
         remaining_idx = []
         idx_by_class = {}
+        classes = np.unique(dataset.y)
         for c in classes:
             idx_by_class[c] = np.where(dataset.y == c)[0]
             np.random.shuffle(idx_by_class[c])
             train_stop = int(frac_train * len(idx_by_class[c]))
             valid_stop = int(train_stop + (frac_valid * len(idx_by_class[c])))
             test_stop = int(valid_stop + (frac_test * len(idx_by_class[c])))
             train_idx = np.hstack([train_idx, idx_by_class[c][:train_stop]])
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/standardizer/_utils.py` & `DeepMol-1.0.0/src/deepmol/standardizer/_utils.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/standardizer/basic_standardizer.py` & `DeepMol-1.0.0/src/deepmol/standardizer/basic_standardizer.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/standardizer/chembl_standardizer.py` & `DeepMol-1.0.0/src/deepmol/standardizer/chembl_standardizer.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/standardizer/custom_standardizer.py` & `DeepMol-1.0.0/src/deepmol/standardizer/custom_standardizer.py`

 * *Files identical despite different names*

### Comparing `DeepMol-0.0.6b0/src/deepmol/unsupervised/base_unsupervised.py` & `DeepMol-1.0.0/src/deepmol/unsupervised/base_unsupervised.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,76 @@
 from abc import abstractmethod, ABC
+from typing import Tuple
 
-from deepmol.datasets import Dataset, SmilesDataset
+from deepmol.base import Transformer
+from deepmol.datasets import Dataset
 
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import plotly.express as px
 from kneed import KneeLocator
 
 from sklearn import cluster, decomposition, manifold
 
 from deepmol.loggers.logger import Logger
+from deepmol.utils.decorators import modify_object_inplace_decorator
 
 
-class UnsupervisedLearn(ABC):
+class UnsupervisedLearn(ABC, Transformer):
     """
     Class for unsupervised learning.
 
     A UnsupervisedLearn sampler receives a Dataset object and performs unsupervised learning.
 
     Subclasses need to implement a _unsupervised method to perform unsupervised learning.
     """
 
     def __init__(self):
         """
         Initialize the UnsupervisedLearn object.
         """
         self.logger = Logger()
+        super().__init__()
 
-    def run_unsupervised(self, dataset: Dataset, **kwargs) -> SmilesDataset:
+    @modify_object_inplace_decorator
+    def run(self, dataset: Dataset, **kwargs) -> Dataset:
         """
         Run unsupervised learning.
 
         Parameters
         ----------
         dataset: Dataset
             The dataset to perform unsupervised learning.
         kwargs:
             Additional arguments to pass to the _run_unsupervised method.
 
         Returns
         -------
-        df: SmilesDataset
+        df: Dataset
             The dataset with the unsupervised features in dataset.X.
         """
-        df = self._run_unsupervised(dataset=dataset, **kwargs)
-        return df
+        dataset._X, dataset.feature_names = self._run_unsupervised(dataset=dataset, **kwargs)
+        return dataset
 
     @abstractmethod
-    def _run_unsupervised(self, dataset: Dataset, **kwargs) -> SmilesDataset:
+    def _run_unsupervised(self, dataset: Dataset, **kwargs) -> Dataset:
         """
         Run unsupervised learning.
 
         Parameters
         ----------
         dataset: Dataset
             The dataset to perform unsupervised learning.
         kwargs:
             Additional arguments to pass to the _unsupervised method.
 
         Returns
         -------
-        x: SmilesDataset
+        x: Dataset
             The dataset with the unsupervised features in dataset.X.
         """
 
     @abstractmethod
     def plot(self, x_new: np.ndarray, path: str = None, **kwargs) -> None:
         """
         Plot the results of unsupervised learning.
@@ -139,41 +144,36 @@
                 Only used by randomized SVD solver when svd_solver == 'randomized'.
             power_iteration_normalizer: str
                 Power iteration normalizer for randomized SVD solver. Available options are ‘auto’, ‘QR’, ‘LU’, ‘none’.
         """
         super().__init__()
         self.pca = decomposition.PCA(**kwargs)
 
-    def _run_unsupervised(self, dataset: Dataset, **kwargs) -> SmilesDataset:
+    def _run_unsupervised(self, dataset: Dataset, **kwargs) -> Tuple[np.ndarray, np.ndarray]:
         """
         Fit the model with X and apply the dimensionality reduction on X.
 
         Parameters
         ----------
         dataset: Dataset
             The dataset to perform unsupervised learning.
         kwargs:
             Additional arguments to pass to the _unsupervised method.
 
         Returns
         -------
-        df: SmilesDataset
-            The dataset with the unsupervised features in dataset.X.
+        x_new: np.ndarray
+            Transformed values.
+        feature_names: np.ndarray
+            The names of the features.
         """
         self.dataset = dataset
         x_new = self.pca.fit_transform(dataset.X)
-        feature_names = [f'PCA_{i}' for i in range(x_new.shape[1])]
-        return SmilesDataset(smiles=dataset.smiles,
-                             mols=dataset.mols,
-                             X=x_new,
-                             y=dataset.y,
-                             ids=dataset.ids,
-                             feature_names=feature_names,
-                             label_names=dataset.label_names,
-                             mode=dataset.mode)
+        feature_names = np.array([f'PCA_{i}' for i in range(x_new.shape[1])])
+        return x_new, feature_names
 
     def plot(self, x_new: np.ndarray, path: str = None, **kwargs) -> None:
         """
         Plot the results of unsupervised learning (PCA).
 
         X_new : ndarray of shape (n_samples, n_components)
             Transformed values.
@@ -230,14 +230,49 @@
                       y=exp_var_cumul,
                       labels={"x": "# Components", "y": "Explained Variance"},
                       **kwargs)
         fig.show()
         if path is not None:
             fig.write_image(path)
 
+    def _fit(self, dataset: Dataset) -> 'PCA':
+        """
+        Fit the model with dataset.X.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            The dataset to perform unsupervised learning.
+
+        Returns
+        -------
+        self: PCA
+            The fitted model.
+        """
+        self.pca.fit(dataset.X)
+        return self
+
+    def _transform(self, dataset: Dataset) -> Dataset:
+        """
+        Apply dimensionality reduction on dataset.X.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            The dataset to perform unsupervised learning.
+
+        Returns
+        -------
+        dataset: Dataset
+            The transformed dataset.
+        """
+        dataset._X = self.pca.transform(dataset.X)
+        dataset.feature_names = np.array([f'PCA_{i}' for i in range(dataset.X.shape[1])])
+        return dataset
+
 
 class TSNE(UnsupervisedLearn):
     """
     Class to perform t-distributed Stochastic Neighbor Embedding (TSNE).
 
     Wrapper around scikit-learn TSNE
     (https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html#sklearn.manifold.TSNE)
@@ -322,39 +357,34 @@
                 metric="precomputed" or (metric="euclidean" and method="exact"). None means 1 unless in a
                 joblib.parallel_backend context. -1 means using all processors.
 
         """
         super().__init__()
         self.tsne = manifold.TSNE(**kwargs)
 
-    def _run_unsupervised(self, dataset: Dataset, **kwargs) -> SmilesDataset:
+    def _run_unsupervised(self, dataset: Dataset, **kwargs) -> Tuple[np.ndarray, np.ndarray]:
         """
         Fit X into an embedded space and return that transformed output.
 
         Parameters
         ----------
         dataset: Dataset
             Dataset to be transformed.
 
         Returns
         -------
-        SmilesDataset
-            Transformed dataset.
+        x_new: np.ndarray
+            The transformed output.
+        feature_names: np.ndarray
+            The feature names.
         """
         self.dataset = dataset
         x_new = self.tsne.fit_transform(dataset.X)
-        feature_names = [f"tsne_{i}" for i in range(x_new.shape[1])]
-        return SmilesDataset(smiles=dataset.smiles,
-                             mols=dataset.mols,
-                             X=x_new,
-                             y=dataset.y,
-                             ids=dataset.ids,
-                             feature_names=feature_names,
-                             label_names=dataset.label_names,
-                             mode=dataset.mode)
+        feature_names = np.array([f"tsne_{i}" for i in range(x_new.shape[1])])
+        return x_new, feature_names
 
     def plot(self, x_new: np.ndarray, path: str = None, **kwargs) -> None:
         self.logger.info(f'{x_new.shape[1]} Components t-SNE: ')
 
         if self.dataset.mode == 'classification':
             y = [str(i) for i in self.dataset.y]
         else:
@@ -371,14 +401,49 @@
                                     labels={'color': self.dataset.label_names[0]},
                                     **kwargs)
             fig.update_traces(diagonal_visible=False)
         fig.show()
         if path:
             fig.write_image(path)
 
+    def _fit(self, dataset: Dataset) -> 'TSNE':
+        """
+        Fit the model with dataset.X.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            The dataset to perform unsupervised learning.
+
+        Returns
+        -------
+        self: TSNE
+            The fitted model.
+        """
+        self.tsne.fit(dataset.X)
+        return self
+
+    def _transform(self, dataset: Dataset) -> Dataset:
+        """
+        Apply dimensionality reduction on dataset.X.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            The dataset to perform unsupervised learning.
+
+        Returns
+        -------
+        dataset: Dataset
+            The transformed dataset.
+        """
+        dataset._X = self.tsne.fit_transform(dataset.X)
+        dataset.feature_names = np.array([f"tsne_{i}" for i in range(dataset.X.shape[1])])
+        return dataset
+
 
 class KMeans(UnsupervisedLearn):
     """Class to perform K-Means clustering.
 
     Wrapper around scikit-learn K-Means.
     (https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html#sklearn.cluster.KMeans)
 
@@ -425,58 +490,70 @@
                 is False.
             algorithm: str {"lloyd", "elkan", "auto", "full"}
                 K-means algorithm to use. The classical EM-style algorithm is `"lloyd"`. The “elkan” variation is more
                 efficient on data with well-defined clusters, by using the triangle inequality. However, it’s more memory
                 intensive due to the allocation of an extra array of shape (n_samples, n_clusters).
         """
         super().__init__()
+        self.k_means = None
         self.kwargs = kwargs
 
-    def _run_unsupervised(self, dataset: Dataset, **kwargs) -> SmilesDataset:
+    def _get_kmeans_instance(self, dataset: Dataset, **kwargs) -> None:
+        """
+        Return the KMeans instance.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            Dataset to cluster.
+        kwargs:
+            Additional keyword arguments to pass to the elbow method.
+        """
+        if 'n_clusters' not in self.kwargs or self.kwargs['n_clusters'] == 'elbow':
+            self.kwargs['n_clusters'] = 'elbow'
+            self.logger.info('Using elbow method to determine number of clusters.')
+            n_clusters = self._elbow(dataset, **kwargs)
+            self.kwargs['n_clusters'] = n_clusters
+
+        self.k_means = cluster.KMeans(**self.kwargs)
+
+    def _run_unsupervised(self, dataset: Dataset, **kwargs) -> Tuple[np.ndarray, np.ndarray]:
         """
         Compute cluster centers and predict cluster index for each sample.
 
         Parameters
         ----------
         dataset: Dataset
             Dataset to cluster.
         kwargs:
             Additional keyword arguments to pass to the elbow method.
 
         Returns
         -------
-        SmilesDataset
-            Transformed dataset.
+        x_new: np.ndarray
+            The transformed output.
+        feature_names: np.ndarray
+            The feature names.
         """
         self.dataset = dataset
 
-        if 'n_clusters' not in self.kwargs or self.kwargs['n_clusters'] == 'elbow':
-            self.kwargs['n_clusters'] = 'elbow'
-            self.logger.info('Using elbow method to determine number of clusters.')
-            n_clusters = self._elbow(**kwargs)
-            self.kwargs['n_clusters'] = n_clusters
+        self._get_kmeans_instance(dataset, **kwargs)
 
-        self.k_means = cluster.KMeans(**self.kwargs)
         x_new = self.k_means.fit_transform(dataset.X)
-        feature_names = [f"cluster_{i}" for i in range(x_new.shape[1])]
-        return SmilesDataset(smiles=dataset.smiles,
-                             mols=dataset.mols,
-                             X=x_new,
-                             y=dataset.y,
-                             ids=dataset.ids,
-                             feature_names=feature_names,
-                             label_names=dataset.label_names,
-                             mode=dataset.mode)
+        feature_names = np.array([f"cluster_{i}" for i in range(x_new.shape[1])])
+        return x_new, feature_names
 
-    def _elbow(self, **kwargs):
+    def _elbow(self, dataset: Dataset, **kwargs):
         """
         Determine the optimal number of clusters using the elbow method.
 
         Parameters
         ----------
+        dataset: Dataset
+            Dataset to cluster.
         kwargs:
             Additional keyword arguments to pass to the elbow method.
             kwargs include:
                 path: str
                     Path to save the elbow method graph. By default, the graph is not saved.
                 S: float
                     The sensitivity of the elbow method. By default, S = 0.1.
@@ -501,15 +578,15 @@
         # kwargs without n_clusters
         k_means_kwargs = self.kwargs.copy()
         k_means_kwargs.pop('n_clusters')
         wcss = []
         for i in range(1, 11):
             kmeans_elbow = cluster.KMeans(n_clusters=i,
                                           **k_means_kwargs)
-            kmeans_elbow.fit(self.dataset.X)
+            kmeans_elbow.fit(dataset.X)
             wcss.append(kmeans_elbow.inertia_)
         plt.plot(range(1, 11), wcss)
         plt.title('The Elbow Method Graph')
         plt.xlabel('Number of clusters')
         plt.ylabel('WCSS')
         plt.show()
         if 'path' in kwargs:
@@ -547,7 +624,44 @@
         else:
             fig = px.scatter_matrix(x_new, color=[str(kl) for kl in self.k_means.labels_],
                                     dimensions=range(x_new.shape[1]), labels={'color': 'cluster'}, **kwargs)
             fig.update_traces(diagonal_visible=False)
         fig.show()
         if path:
             fig.write_image(path)
+
+    def _fit(self, dataset: Dataset) -> 'KMeans':
+        """
+        Fit the model with dataset.X.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            The dataset to perform unsupervised learning.
+
+        Returns
+        -------
+        self: KMeans
+            The fitted model.
+        """
+        # Using fit does not allow to pass additional arguments to the elbow method
+        self._get_kmeans_instance(dataset)
+        self.k_means.fit(dataset.X)
+        return self
+
+    def _transform(self, dataset: Dataset) -> Dataset:
+        """
+        Apply dimensionality reduction on dataset.X.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            The dataset to perform unsupervised learning.
+
+        Returns
+        -------
+        dataset: Dataset
+            The transformed dataset.
+        """
+        dataset._X = self.k_means.transform(dataset.X)
+        dataset.feature_names = np.array([f"cluster_{i}" for i in range(dataset.X.shape[1])])
+        return dataset
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/unsupervised/umap.py` & `DeepMol-1.0.0/src/deepmol/unsupervised/umap.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from typing import Tuple
+
 import numpy as np
 import umap
 
-from deepmol.datasets import Dataset, SmilesDataset
+from deepmol.datasets import Dataset
 from deepmol.unsupervised.base_unsupervised import UnsupervisedLearn
 import plotly.express as px
 
 
 class UMAP(UnsupervisedLearn):
     """
     Class to perform Uniform Manifold Approximation and Projection (UMAP).
@@ -41,41 +43,36 @@
         """
         super().__init__()
         if parametric:
             self.umap = umap.parametric_umap.ParametricUMAP(**kwargs)
         else:
             self.umap = umap.UMAP(**kwargs)
 
-    def _run_unsupervised(self, dataset: Dataset, **kwargs) -> SmilesDataset:
+    def _run_unsupervised(self, dataset: Dataset, **kwargs) -> Tuple[np.ndarray, np.ndarray]:
         """
         Compute cluster centers and predict cluster index for each sample.
 
         Parameters
         ----------
         dataset : Dataset
             The dataset to run the unsupervised learning on.
         kwargs:
             Additional keyword arguments for the UMAP class.
 
         Returns
         -------
-        SmilesDataset
-            The dataset with the new features.
+        x_new : np.ndarray
+            The new features.
+        feature_names : np.ndarray
+            The names of the new features.
         """
         self.dataset = dataset
         x_new = self.umap.fit_transform(dataset.X)
-        feature_names = [f'UMAP_{i}' for i in range(x_new.shape[1])]
-        return SmilesDataset(smiles=dataset.smiles,
-                             mols=dataset.mols,
-                             X=x_new,
-                             y=dataset.y,
-                             ids=dataset.ids,
-                             feature_names=feature_names,
-                             label_names=dataset.label_names,
-                             mode=dataset.mode)
+        feature_names = np.array([f'UMAP_{i}' for i in range(x_new.shape[1])])
+        return x_new, feature_names
 
     def plot(self, x_new: np.ndarray, path: str = None, **kwargs) -> None:
         """
         Plot the UMAP embedding.
 
         Parameters
         ----------
@@ -91,23 +88,58 @@
         if self.dataset.mode == 'classification':
             y = [str(i) for i in self.dataset.y]
         else:
             y = self.dataset.y
 
         if x_new.shape[1] == 2:
             fig = px.scatter(x_new, x=0, y=1, color=y,
-                             labels={'0': 'PC 1', '1': 'PC 2', 'color': self.dataset.label_names[0]}, **kwargs)
+                             labels={'0': 'UMAP 1', '1': 'UMAP 2', 'color': self.dataset.label_names[0]}, **kwargs)
         elif x_new.shape[1] == 3:
             fig = px.scatter_3d(x_new, x=0, y=1, z=2, color=y,
-                                labels={'0': 'PC 1', '1': 'PC 2', '2': 'PC 3', 'color': self.dataset.label_names[0]})
+                                labels={'0': 'UMAP 1', '1': 'UMAP 2', '2': 'UMAP 3', 'color': self.dataset.label_names[0]})
         else:
             labels = {str(i): f"UMAP {i + 1}" for i in range(x_new.shape[1])}
             labels['color'] = self.dataset.label_names[0]
             fig = px.scatter_matrix(x_new,
                                     color=y,
                                     dimensions=range(x_new.shape[1]),
                                     labels=labels,
                                     **kwargs)
             fig.update_traces(diagonal_visible=False)
         fig.show()
         if path is not None:
             fig.write_image(path)
+
+    def _fit(self, dataset: Dataset) -> 'UMAP':
+        """
+        Fit the model with dataset.X.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            The dataset to perform unsupervised learning.
+
+        Returns
+        -------
+        self: TSNE
+            The fitted model.
+        """
+        self.umap.fit(dataset.X)
+        return self
+
+    def _transform(self, dataset: Dataset) -> Dataset:
+        """
+        Apply dimensionality reduction on dataset.X.
+
+        Parameters
+        ----------
+        dataset: Dataset
+            The dataset to perform unsupervised learning.
+
+        Returns
+        -------
+        dataset: Dataset
+            The transformed dataset.
+        """
+        dataset._X = self.umap.transform(dataset.X)
+        dataset.feature_names = np.array([f'UMAP_{i}' for i in range(dataset.X.shape[1])])
+        return dataset
```

### Comparing `DeepMol-0.0.6b0/src/deepmol/utils/errors.py` & `DeepMol-1.0.0/src/deepmol/utils/errors.py`

 * *Files identical despite different names*

