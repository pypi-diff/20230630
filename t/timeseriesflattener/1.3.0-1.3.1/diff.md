# Comparing `tmp/timeseriesflattener-1.3.0.tar.gz` & `tmp/timeseriesflattener-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-1.3.0.tar", last modified: Thu Jun 29 09:14:50 2023, max compression
+gzip compressed data, was "timeseriesflattener-1.3.1.tar", last modified: Fri Jun 30 08:23:44 2023, max compression
```

## Comparing `timeseriesflattener-1.3.0.tar` & `timeseriesflattener-1.3.1.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.402251 timeseriesflattener-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      738 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.366249 timeseriesflattener-1.3.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.362249 timeseriesflattener-1.3.0/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.366249 timeseriesflattener-1.3.0/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.366249 timeseriesflattener-1.3.0/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      948 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)      252 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.370249 timeseriesflattener-1.3.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     2083 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/cruft.yml
--rw-r--r--   0 root         (0) root         (0)      849 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      868 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     2446 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     2891 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     3056 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2871 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      644 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     1286 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    56049 2023-06-29 09:14:38.000000 timeseriesflattener-1.3.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1087 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/Makefile
--rw-r--r--   0 root         (0) root         (0)    11520 2023-06-29 09:14:50.402251 timeseriesflattener-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9122 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1763 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.370249 timeseriesflattener-1.3.0/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.370249 timeseriesflattener-1.3.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   811066 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)     4211 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)     5280 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      312 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/timeseriesflattener.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.374249 timeseriesflattener-1.3.0/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   118804 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    50220 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    72388 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/03_text.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.374249 timeseriesflattener-1.3.0/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      370 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)    49714 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.374249 timeseriesflattener-1.3.0/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4298 2023-06-29 09:14:38.000000 timeseriesflattener-1.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 09:14:50.402251 timeseriesflattener-1.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.378250 timeseriesflattener-1.3.0/src/
--rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.378250 timeseriesflattener-1.3.0/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      309 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     5559 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/column_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.378250 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6308 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.382250 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_specs/
--rw-r--r--   0 root         (0) root         (0)     7039 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_specs/group_specs.py
--rw-r--r--   0 root         (0) root         (0)     8488 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_specs/single_specs.py
--rw-r--r--   0 root         (0) root         (0)    36395 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2271 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/logger.py
--rw-r--r--   0 root         (0) root         (0)     7704 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/misc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.382250 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     3008 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.382250 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8082 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2700 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     2279 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.362249 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.362249 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.382250 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1505 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.386250 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1869 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.398251 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      812 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   248865 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     1392 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.398251 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.398251 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3425 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.398251 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16237 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.402251 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18309 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2688 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2328 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     8190 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/text_embedding_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.402251 timeseriesflattener-1.3.0/src/timeseriesflattener/utils/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/utils/pydantic_basemodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.378250 timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11520 2023-06-29 09:14:50.000000 timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5042 2023-06-29 09:14:50.000000 timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 09:14:50.000000 timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      716 2023-06-29 09:14:50.000000 timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-29 09:14:50.000000 timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9390 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.724664 timeseriesflattener-1.3.1/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.676664 timeseriesflattener-1.3.1/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.668664 timeseriesflattener-1.3.1/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.676664 timeseriesflattener-1.3.1/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.676664 timeseriesflattener-1.3.1/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      948 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)      252 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.680664 timeseriesflattener-1.3.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      868 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    56250 2023-06-30 08:23:32.000000 timeseriesflattener-1.3.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11520 2023-06-30 08:23:44.724664 timeseriesflattener-1.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9122 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.684664 timeseriesflattener-1.3.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.684664 timeseriesflattener-1.3.1/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   811066 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      312 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/timeseriesflattener.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.684664 timeseriesflattener-1.3.1/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   118804 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    50220 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    72388 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/03_text.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.688664 timeseriesflattener-1.3.1/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      370 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.688664 timeseriesflattener-1.3.1/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4298 2023-06-30 08:23:32.000000 timeseriesflattener-1.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 08:23:44.724664 timeseriesflattener-1.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.688664 timeseriesflattener-1.3.1/src/
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.692664 timeseriesflattener-1.3.1/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      309 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     5559 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/column_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.696664 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.696664 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)     7090 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_specs/group_specs.py
+-rw-r--r--   0 root         (0) root         (0)     8488 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_specs/single_specs.py
+-rw-r--r--   0 root         (0) root         (0)    36395 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7704 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/misc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.696664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     3008 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.696664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8082 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2700 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.672664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.672664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.700664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.700664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.720664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      812 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   248865 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.720664 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.720664 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.720664 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16237 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.724664 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18309 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     8190 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/text_embedding_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.724664 timeseriesflattener-1.3.1/src/timeseriesflattener/utils/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/utils/pydantic_basemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.692664 timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11520 2023-06-30 08:23:44.000000 timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-06-30 08:23:44.000000 timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 08:23:44.000000 timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-30 08:23:44.000000 timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-30 08:23:44.000000 timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9390 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/tasks.py
```

### Comparing `timeseriesflattener-1.3.0/.cruft.json` & `timeseriesflattener-1.3.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/actions/test/action.yml` & `timeseriesflattener-1.3.1/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-1.3.1/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/dependabot.yml` & `timeseriesflattener-1.3.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/recommended_repo_setup.md` & `timeseriesflattener-1.3.1/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/workflows/check_for_rej.yml` & `timeseriesflattener-1.3.1/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/workflows/cruft.yml` & `timeseriesflattener-1.3.1/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-1.3.1/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/workflows/documentation.yml` & `timeseriesflattener-1.3.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-1.3.1/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-1.3.1/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/workflows/pre-commit.yml` & `timeseriesflattener-1.3.1/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/workflows/stalebot.yml` & `timeseriesflattener-1.3.1/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.github/workflows/static_type_checks.yml` & `timeseriesflattener-1.3.1/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.gitignore` & `timeseriesflattener-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.pre-commit-config.yaml` & `timeseriesflattener-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/.zenodo.json` & `timeseriesflattener-1.3.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/CHANGELOG.md` & `timeseriesflattener-1.3.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.1 (2023-06-30)
+
+### Fix
+
+* Create combinations not working for ([`8c3c343`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/8c3c34314cf4f6e304d8f64c7118f57fa1ca1498))
+
 ## v1.3.0 (2023-06-29)
 
 ### Feature
 
 * Add types to aggregation functions ([`560539f`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/560539f2d1871043024539f863fc755cb101c28e))
 
 ## v1.2.1 (2023-06-20)
```

### Comparing `timeseriesflattener-1.3.0/CODE_OF_CONDUCT.md` & `timeseriesflattener-1.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/CONTRIBUTING.md` & `timeseriesflattener-1.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/LICENSE` & `timeseriesflattener-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/PKG-INFO` & `timeseriesflattener-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.3.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.3.1 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-1.3.0/README.md` & `timeseriesflattener-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/citation.cff` & `timeseriesflattener-1.3.1/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/Makefile` & `timeseriesflattener-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/_static/favicon.ico` & `timeseriesflattener-1.3.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/_static/icon.png` & `timeseriesflattener-1.3.1/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/_static/icon_dark.png` & `timeseriesflattener-1.3.1/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/_static/terminology_figure.png` & `timeseriesflattener-1.3.1/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/conf.py` & `timeseriesflattener-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/faq.rst` & `timeseriesflattener-1.3.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/index.rst` & `timeseriesflattener-1.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-1.3.1/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-1.3.1/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/tutorials/03_text.ipynb` & `timeseriesflattener-1.3.1/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/tutorials/img/term_a.png` & `timeseriesflattener-1.3.1/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/tutorials/img/term_b.png` & `timeseriesflattener-1.3.1/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/tutorials/img/term_c.png` & `timeseriesflattener-1.3.1/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/docs/tutorials/img/term_d.png` & `timeseriesflattener-1.3.1/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/icon.png` & `timeseriesflattener-1.3.1/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/paper/paper.bib` & `timeseriesflattener-1.3.1/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/paper/paper.md` & `timeseriesflattener-1.3.1/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/pyproject.toml` & `timeseriesflattener-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "1.3.0"
+version = "1.3.1"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"}, {name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com"}, {name = "Kenneth Enevoldsen"}, {name = "Martin Bernstorff", email = "martinbernstorff@gmail.com"}]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.8",
```

### Comparing `timeseriesflattener-1.3.0/src/conftest.py` & `timeseriesflattener-1.3.1/src/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/aggregation_fns.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/column_handler.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/column_handler.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/feature_cache/cache_to_disk.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/feature_specs/group_specs.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/feature_specs/group_specs.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,19 +89,20 @@
         combination_dict = create_feature_combinations_from_dict(
             dictionary=self.__dict__,
         )
 
         return [
             OutcomeSpec(
                 prefix=d["prefix"],  # type: ignore
-                timeseries_df=d["values_pairs"].df,  # type: ignore
-                feature_base_name=d["values_pairs"].base_feature_name,  # type: ignore
+                timeseries_df=d["named_dataframes"].df,  # type: ignore
+                feature_base_name=d["named_dataframes"].name,  # type: ignore
                 lookahead_days=d["lookahead_days"],  # type: ignore
                 aggregation_fn=d["aggregation_fns"],  # type: ignore
                 fallback=d["fallback"],  # type: ignore
+                incident=d["incident"],  # type: ignore
             )
             for d in combination_dict
         ]
 
 
 class TextPredictorGroupSpec(BaseModel):
     """A group of text predictor specifications. See PredictorGroupSpec and TextPredictorSpec for more details."""
```

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/feature_specs/single_specs.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/feature_specs/single_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/flattened_dataset.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/flattened_ds_validator.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/logger.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/misc_utils.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/misc_utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/utils.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/text_embedding_functions.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/text_embedding_functions.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener/utils/pydantic_basemodel.py` & `timeseriesflattener-1.3.1/src/timeseriesflattener/utils/pydantic_basemodel.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.3.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.3.1 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.0/tasks.py` & `timeseriesflattener-1.3.1/tasks.py`

 * *Files identical despite different names*

