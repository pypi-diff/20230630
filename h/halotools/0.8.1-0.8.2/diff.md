# Comparing `tmp/halotools-0.8.1.tar.gz` & `tmp/halotools-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halotools-0.8.1.tar", last modified: Wed Sep 28 17:03:32 2022, max compression
+gzip compressed data, was "halotools-0.8.2.tar", last modified: Fri Jun 30 17:51:15 2023, max compression
```

## Comparing `halotools-0.8.1.tar` & `halotools-0.8.2.tar`

### file list

```diff
@@ -1,845 +1,849 @@
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.514685 halotools-0.8.1/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:31.994487 halotools-0.8.1/.github/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.038037 halotools-0.8.1/.github/workflows/
--rw-r--r--   0 aphearin   (501) staff       (20)     1480 2022-09-23 19:40:55.000000 halotools-0.8.1/.github/workflows/ci_tests.yml
--rw-r--r--   0 aphearin   (501) staff       (20)      852 2022-09-25 19:14:09.000000 halotools-0.8.1/.github/workflows/wheels.yml
--rw-r--r--   0 aphearin   (501) staff       (20)      683 2022-09-25 14:53:47.000000 halotools-0.8.1/.gitignore
--rw-r--r--   0 aphearin   (501) staff       (20)      228 2022-09-23 19:40:55.000000 halotools-0.8.1/.readthedocs.yml
--rw-r--r--   0 aphearin   (501) staff       (20)     9632 2022-09-28 17:00:07.000000 halotools-0.8.1/CHANGES.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      305 2022-09-27 18:06:44.000000 halotools-0.8.1/MANIFEST.in
--rw-r--r--   0 aphearin   (501) staff       (20)     9799 2022-09-28 17:03:32.514963 halotools-0.8.1/PKG-INFO
--rw-r--r--   0 aphearin   (501) staff       (20)     9372 2022-09-27 17:51:03.000000 halotools-0.8.1/README.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.038996 halotools-0.8.1/cextern/
--rw-r--r--   0 aphearin   (501) staff       (20)      299 2020-08-05 18:14:21.000000 halotools-0.8.1/cextern/README.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.053364 halotools-0.8.1/docs/
--rw-r--r--   0 aphearin   (501) staff       (20)     4724 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/Makefile
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.074779 halotools-0.8.1/docs/_static/
--rw-r--r--   0 aphearin   (501) staff       (20)    16687 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/bijective_distribution_matching_demo.png
--rw-r--r--   0 aphearin   (501) staff       (20)    44595 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/cam_example_assembias_clf.png
--rw-r--r--   0 aphearin   (501) staff       (20)    12849 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/cam_example_bulge_disk_ratio.png
--rw-r--r--   0 aphearin   (501) staff       (20)    15023 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/cam_example_complex_sfr.png
--rw-r--r--   0 aphearin   (501) staff       (20)    15931 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/cam_example_complex_sfr_dmdt_correlation.png
--rw-r--r--   0 aphearin   (501) staff       (20)    12004 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/cam_example_complex_sfr_recovery.png
--rw-r--r--   0 aphearin   (501) staff       (20)    32174 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/color_correlation_pdf.png
--rw-r--r--   0 aphearin   (501) staff       (20)   154081 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/dm-splatting-large.png
--rw-r--r--   0 aphearin   (501) staff       (20)    15955 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/fuzzy_binning_example.png
--rw-r--r--   0 aphearin   (501) staff       (20)      104 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/halotools.css
--rw-r--r--   0 aphearin   (501) staff       (20)    12194 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/matched_distributions.png
--rw-r--r--   0 aphearin   (501) staff       (20)     6699 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/monte_carlo_example.png
--rw-r--r--   0 aphearin   (501) staff       (20)    46403 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/monte_carlo_example2.png
--rw-r--r--   0 aphearin   (501) staff       (20)    28645 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/noisy_percentile_demo.png
--rw-r--r--   0 aphearin   (501) staff       (20)    34365 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/quenching_gradient_model_clustering.png
--rw-r--r--   0 aphearin   (501) staff       (20)    32129 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/quenching_gradient_models.png
--rw-r--r--   0 aphearin   (501) staff       (20)    15404 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_static/spin_percentile.png
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:31.995236 halotools-0.8.1/docs/_templates/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.078632 halotools-0.8.1/docs/_templates/autosummary/
--rw-r--r--   0 aphearin   (501) staff       (20)      250 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      251 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      252 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/_templates/autosummary/module.rst
--rw-r--r--   0 aphearin   (501) staff       (20)       90 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/changelog.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     5042 2022-09-25 14:53:47.000000 halotools-0.8.1/docs/conf.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.079192 halotools-0.8.1/docs/full_ref_api/
--rw-r--r--   0 aphearin   (501) staff       (20)      587 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/full_ref_api/halotools_full_api.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.085267 halotools-0.8.1/docs/function_usage/
--rw-r--r--   0 aphearin   (501) staff       (20)      216 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/function_usage/abundance_matching.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      412 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/function_usage/empirical_model_factory_functions.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      578 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/function_usage/hod_occupation_functions.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     2033 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/function_usage/index.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     1308 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/function_usage/mock_observables_functions.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      856 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/function_usage/phase_space_models_functions.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      452 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/function_usage/processing_simulation_data.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     1093 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/function_usage/utility_functions.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     1469 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/index.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     8696 2022-09-27 17:51:03.000000 halotools-0.8.1/docs/install.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     1346 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/installation_troubleshooting.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     1317 2022-09-23 19:40:55.000000 halotools-0.8.1/docs/installing_halotools_with_virtualenv.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     4513 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/make.bat
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:31.997125 halotools-0.8.1/docs/notebooks/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.088666 halotools-0.8.1/docs/notebooks/cam_modeling/
--rw-r--r--   0 aphearin   (501) staff       (20)    59110 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/cam_modeling/cam_complex_sfr_tutorial.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    64871 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/cam_modeling/cam_decorated_clf.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    33338 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/cam_modeling/cam_disk_bulge_ratios_demo.ipynb
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:31.996441 halotools-0.8.1/docs/notebooks/galcat_analysis/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.101284 halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/
--rw-r--r--   0 aphearin   (501) staff       (20)   132493 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial
--rw-r--r--   0 aphearin   (501) staff       (20)    81382 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial1.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)     9983 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial10.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    41554 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial2.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    50743 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial3.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    59196 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial4.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    11038 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial5.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    26854 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial6.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    59055 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial7.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    39567 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial8.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)   319967 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial9.ipynb
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.104616 halotools-0.8.1/docs/notebooks/galcat_analysis/intermediate_examples/
--rw-r--r--   0 aphearin   (501) staff       (20)    14432 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/intermediate_examples/galaxy_catalog_intermediate_analysis_tutorial1.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)   136855 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/galcat_analysis/intermediate_examples/quenching_gradient_tutorial.ipynb
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:31.996667 halotools-0.8.1/docs/notebooks/halocat_analysis/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.107413 halotools-0.8.1/docs/notebooks/halocat_analysis/basic_examples/
--rw-r--r--   0 aphearin   (501) staff       (20)    20171 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial1.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    68521 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial2.ipynb
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.112661 halotools-0.8.1/docs/notebooks/hod_modeling/
--rw-r--r--   0 aphearin   (501) staff       (20)    17926 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/hod_modeling/hod_modeling_tutorial1.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    14511 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/hod_modeling/hod_modeling_tutorial2.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)     5749 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/hod_modeling/hod_modeling_tutorial3.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    30300 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/hod_modeling/hod_modeling_tutorial4.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    49309 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/hod_modeling/hod_modeling_tutorial5.ipynb
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.116821 halotools-0.8.1/docs/notebooks/subhalo_modeling/
--rw-r--r--   0 aphearin   (501) staff       (20)     9010 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial1.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    52926 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial2.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)     5822 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial3.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    37815 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial4.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    51211 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial5.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)     4996 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/overview.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.118563 halotools-0.8.1/docs/quickstart_and_tutorials/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.122817 halotools-0.8.1/docs/quickstart_and_tutorials/development/
--rw-r--r--   0 aphearin   (501) staff       (20)      412 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/development/bug_reports.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     3027 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/development/citing_halotools.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      972 2022-09-23 19:40:55.000000 halotools-0.8.1/docs/quickstart_and_tutorials/development/contributors.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      429 2022-09-25 19:14:09.000000 halotools-0.8.1/docs/quickstart_and_tutorials/development/getting_started.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      357 2022-09-23 19:40:55.000000 halotools-0.8.1/docs/quickstart_and_tutorials/development/index.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    11937 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/getting_started_overview.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     2046 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/index.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.123607 halotools-0.8.1/docs/quickstart_and_tutorials/managing_catalogs/
--rw-r--r--   0 aphearin   (501) staff       (20)     4780 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/managing_catalogs/supported_sim_list.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.125182 halotools-0.8.1/docs/quickstart_and_tutorials/mock_observations/
--rw-r--r--   0 aphearin   (501) staff       (20)     5414 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/mock_observations/calculating_counts_in_cells.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     5657 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/mock_observations/mock_obs_pos_formatting.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.127010 halotools-0.8.1/docs/quickstart_and_tutorials/quickstart_guides/
--rw-r--r--   0 aphearin   (501) staff       (20)     6594 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/quickstart_guides/halo_catalog_analysis_quickstart.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     2174 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/quickstart_guides/working_with_alternative_catalogs.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     4966 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/quickstart_guides/working_with_halotools_provided_catalogs.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.130126 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.000122 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.130667 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.133957 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.145555 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/
--rw-r--r--   0 aphearin   (501) staff       (20)    35707 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/angular_crosscorr.png
--rw-r--r--   0 aphearin   (501) staff       (20)     4759 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial2.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     7072 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial3.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     4494 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial4.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     9603 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial9.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    37960 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/gg_lensing_tutorial3.png
--rw-r--r--   0 aphearin   (501) staff       (20)    68942 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/mock_fullsky.png
--rw-r--r--   0 aphearin   (501) staff       (20)    15719 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/mock_octant.png
--rw-r--r--   0 aphearin   (501) staff       (20)    33076 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/one_two_halo_clustering.png
--rw-r--r--   0 aphearin   (501) staff       (20)    21885 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/output_9_1.png
--rw-r--r--   0 aphearin   (501) staff       (20)    21171 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/random_vs_analytic.png
--rw-r--r--   0 aphearin   (501) staff       (20)    48225 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/wp_red_blue_cross.png
--rw-r--r--   0 aphearin   (501) staff       (20)    43021 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/wp_tutorial4.png
--rw-r--r--   0 aphearin   (501) staff       (20)    14277 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/wtheta1.png
--rw-r--r--   0 aphearin   (501) staff       (20)     2217 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/crossmatching_galaxy_catalogs.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     9422 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial1.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.146779 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/group_identification/
--rw-r--r--   0 aphearin   (501) staff       (20)     9277 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/group_identification/galaxy_catalog_analysis_tutorial5.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     9795 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/group_identification/group_richness_vs_group_cenmass.png
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.147447 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/isolation_criteria/
--rw-r--r--   0 aphearin   (501) staff       (20)     6496 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/isolation_criteria/galaxy_catalog_analysis_tutorial10.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    14222 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/output_18_1.png
--rw-r--r--   0 aphearin   (501) staff       (20)    26171 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/output_23_1.png
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.150138 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/
--rw-r--r--   0 aphearin   (501) staff       (20)    18722 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/cluster_bcg_infall_velocity.png
--rw-r--r--   0 aphearin   (501) staff       (20)    30240 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/cluster_dispersion_profile.png
--rw-r--r--   0 aphearin   (501) staff       (20)     4898 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/galaxy_catalog_analysis_tutorial6.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     4786 2022-09-17 13:29:45.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/galaxy_catalog_analysis_tutorial7.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.151651 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/void_stats/
--rw-r--r--   0 aphearin   (501) staff       (20)     4124 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/void_stats/galaxy_catalog_analysis_tutorial8.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    18713 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/void_stats/vpf_upf_tutorial.png
--rw-r--r--   0 aphearin   (501) staff       (20)     2842 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/index.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:31.999787 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/intermediate_examples/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.152844 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/intermediate_examples/isolation_criteria/
--rw-r--r--   0 aphearin   (501) staff       (20)    11442 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/intermediate_examples/isolation_criteria/galaxy_catalog_intermediate_analysis_tutorial1.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.155085 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.157725 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.158990 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/figs/
--rw-r--r--   0 aphearin   (501) staff       (20)    19523 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/figs/radial_profile_halocat_tutorial_fig1.png
--rw-r--r--   0 aphearin   (501) staff       (20)    23205 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/figs/radial_profile_halocat_tutorial_fig2.png
--rw-r--r--   0 aphearin   (501) staff       (20)     5950 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial1.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     6486 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial2.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     9024 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/nsub_vs_hostmass.png
--rw-r--r--   0 aphearin   (501) staff       (20)     4140 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/crossmatching_halo_catalogs.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     1536 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/index.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     4584 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/rockstar_subhalo_nomenclature.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    81243 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/subhalo_membership.png
--rw-r--r--   0 aphearin   (501) staff       (20)     5783 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/merger_tree_analysis_example.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.161978 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/
--rw-r--r--   0 aphearin   (501) staff       (20)      827 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/altering_param_dict.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.164800 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/
--rw-r--r--   0 aphearin   (501) staff       (20)     3637 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_complex_sfr.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     4139 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_decorated_clf.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     3520 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_disk_bulge_ratios.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     2180 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_quenching_gradients.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     7131 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_tutorial.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.165393 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.171760 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/
--rw-r--r--   0 aphearin   (501) staff       (20)      710 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial0.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     9555 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial1.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     6646 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial2.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    10285 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial3.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    10856 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial4.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     7554 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial5.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     6902 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/writing_your_own_hod_occupation_component.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      261 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/writing_your_own_hod_profile_component.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     3412 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/zheng07_using_cenocc_model_tutorial.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     1921 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/index.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.175492 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/
--rw-r--r--   0 aphearin   (501) staff       (20)      741 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial0.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     8148 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial1.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     5335 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial2.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     9051 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial3.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    10729 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial4.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     7056 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial5.rst
--rw-r--r--   0 aphearin   (501) staff       (20)   131548 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/halotools_design.png
--rw-r--r--   0 aphearin   (501) staff       (20)     3529 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/index.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.181669 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/
--rw-r--r--   0 aphearin   (501) staff       (20)      482 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/abundance_matching_composite_model.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     6845 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/behroozi10_composite_model.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     7468 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/cacciato09_composite_model.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     8057 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/hearin15_composite_model.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     4259 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/index.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     7617 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/leauthaud11_composite_model.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      787 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/preloaded_models_list.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     6181 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/tinker13_composite_model.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     8034 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/zheng07_composite_model.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     8093 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/zu_mandelbaum15_composite_model.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     7458 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/zu_mandelbaum16_composite_model.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     8838 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/reducing_and_caching_a_new_rockstar_catalog.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     4447 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/user_supplied_halo_catalogs.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     3451 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/working_with_alternative_particle_data.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.182775 halotools-0.8.1/docs/source_notes/
--rw-r--r--   0 aphearin   (501) staff       (20)     3769 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/convert_tutorials.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.004144 halotools-0.8.1/docs/source_notes/empirical_models/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.183553 halotools-0.8.1/docs/source_notes/empirical_models/assembias_models/
--rw-r--r--   0 aphearin   (501) staff       (20)      211 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/empirical_models/assembias_models/heaviside_assembias_source_code_notes.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.189741 halotools-0.8.1/docs/source_notes/empirical_models/factories/
--rw-r--r--   0 aphearin   (501) staff       (20)    21897 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/empirical_models/factories/hod_mock_factory_source_notes.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    12746 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/empirical_models/factories/hod_model_factory_source_notes.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      882 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/empirical_models/factories/index.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    16187 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/empirical_models/factories/model_factory_composite_sequence_mechanisms.rst
--rw-r--r--   0 aphearin   (501) staff       (20)   165846 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/empirical_models/factories/np_repeat_tutorial.png
--rw-r--r--   0 aphearin   (501) staff       (20)     5532 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/empirical_models/factories/subhalo_mock_factory_source_notes.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    12008 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/empirical_models/factories/subhalo_model_factory_source_notes.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.192361 halotools-0.8.1/docs/source_notes/empirical_models/phase_space_models/
--rw-r--r--   0 aphearin   (501) staff       (20)     2770 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/empirical_models/phase_space_models/jeans_equation_derivations.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      943 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/empirical_models/phase_space_models/monte_carlo_galprof_source_notes.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    22266 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/empirical_models/phase_space_models/nfw_profile_source_notes.rst
--rw-r--r--   0 aphearin   (501) staff       (20)    15674 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/empirical_models/phase_space_models/profile_template_source_notes.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     1135 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/index.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.193162 halotools-0.8.1/docs/source_notes/mock_observables/
--rw-r--r--   0 aphearin   (501) staff       (20)     4354 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/source_notes/mock_observables/zspace_distortions.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.004948 halotools-0.8.1/docs/usage_tutorials/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.193722 halotools-0.8.1/docs/usage_tutorials/cache_management/
--rw-r--r--   0 aphearin   (501) staff       (20)     4365 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/usage_tutorials/cache_management/relocating_simulation_data.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.005371 halotools-0.8.1/docs/usage_tutorials/empirical_models/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.194270 halotools-0.8.1/docs/usage_tutorials/empirical_models/assembias_models/
--rw-r--r--   0 aphearin   (501) staff       (20)     4783 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/usage_tutorials/empirical_models/assembias_models/heaviside_assembias_tutorial.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.194772 halotools-0.8.1/docs/usage_tutorials/empirical_models/subhalo_phase_space/
--rw-r--r--   0 aphearin   (501) staff       (20)    10877 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/usage_tutorials/empirical_models/subhalo_phase_space/subhalo_phase_space_tutorial.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      452 2022-09-23 19:40:55.000000 halotools-0.8.1/docs/whats_new.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.197699 halotools-0.8.1/docs/whats_new_history/
--rw-r--r--   0 aphearin   (501) staff       (20)     6992 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/whats_new_history/whats_new_0.5.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     2136 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/whats_new_history/whats_new_0.6.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     2086 2020-08-05 18:14:21.000000 halotools-0.8.1/docs/whats_new_history/whats_new_0.7.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      457 2022-09-23 19:40:55.000000 halotools-0.8.1/docs/whats_new_history/whats_new_0.8.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      337 2022-09-23 19:40:55.000000 halotools-0.8.1/docs/whats_new_history/whats_new_v0x_history.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.202126 halotools-0.8.1/halotools/
--rw-r--r--   0 aphearin   (501) staff       (20)      427 2022-09-15 17:03:51.000000 halotools-0.8.1/halotools/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)      356 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/_astropy_init.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2720 2022-09-28 17:03:31.000000 halotools-0.8.1/halotools/_compiler.c
--rw-r--r--   0 aphearin   (501) staff       (20)     1081 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/conftest.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1681 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/custom_exceptions.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.205297 halotools-0.8.1/halotools/data/
--rw-r--r--   0 aphearin   (501) staff       (20)      200 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/data/README.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.207623 halotools-0.8.1/halotools/empirical_models/
--rw-r--r--   0 aphearin   (501) staff       (20)      510 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.210412 halotools-0.8.1/halotools/empirical_models/abunmatch/
--rw-r--r--   0 aphearin   (501) staff       (20)      175 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6484 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/bin_free_cam.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8805 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/conditional_abunmatch_bin_based.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.212365 halotools-0.8.1/halotools/empirical_models/abunmatch/engines/
--rw-r--r--   0 aphearin   (501) staff       (20)       79 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/engines/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    12050 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/engines/bin_free_cam_kernel.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)      901 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/engines/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7869 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/noisy_percentile.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.216699 halotools-0.8.1/halotools/empirical_models/abunmatch/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1326 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/tests/naive_python_cam.py
--rw-r--r--   0 aphearin   (501) staff       (20)    17601 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/tests/test_bin_free_cam.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1595 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/tests/test_conditional_abunmatch.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1168 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/tests/test_noisy_percentile.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4440 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/tests/test_pure_python.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3974 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/tests/test_sample2_window_function.py
--rw-r--r--   0 aphearin   (501) staff       (20)      163 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/abunmatch/tests/test_single_unit.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.217893 halotools-0.8.1/halotools/empirical_models/assembias_models/
--rw-r--r--   0 aphearin   (501) staff       (20)       35 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/assembias_models/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    24275 2022-09-25 18:24:15.000000 halotools-0.8.1/halotools/empirical_models/assembias_models/heaviside_assembias.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.219799 halotools-0.8.1/halotools/empirical_models/assembias_models/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/assembias_models/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3589 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/assembias_models/tests/test_assembias.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.222187 halotools-0.8.1/halotools/empirical_models/component_model_templates/
--rw-r--r--   0 aphearin   (501) staff       (20)      116 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/component_model_templates/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    14084 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/component_model_templates/binary_galprop_models.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8107 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/component_model_templates/prim_galprop_model.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6792 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/component_model_templates/scatter_models.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.224296 halotools-0.8.1/halotools/empirical_models/component_model_templates/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/component_model_templates/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3129 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/component_model_templates/tests/test_binary_galprop_models.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3708 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/component_model_templates/tests/test_prim_galprop_model.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9015 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/component_model_templates/tests/test_scatter_models.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.224813 halotools-0.8.1/halotools/empirical_models/composite_models/
--rw-r--r--   0 aphearin   (501) staff       (20)      307 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.229334 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/
--rw-r--r--   0 aphearin   (501) staff       (20)      186 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4363 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/cacciato09.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5274 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/hearin15.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4450 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/leauthaud11.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.231491 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1491 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/tests/test_tinker13.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4088 2021-03-06 19:16:34.000000 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/tests/test_zheng07.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2608 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/tests/test_zu_mandelbaum16.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5470 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/tinker13.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5150 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/zheng07.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5435 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/zu_mandelbaum15.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6105 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/zu_mandelbaum16.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.232608 halotools-0.8.1/halotools/empirical_models/composite_models/sfr_models/
--rw-r--r--   0 aphearin   (501) staff       (20)       31 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/sfr_models/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3881 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/sfr_models/smhm_binary_sfr.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.233701 halotools-0.8.1/halotools/empirical_models/composite_models/smhm_models/
--rw-r--r--   0 aphearin   (501) staff       (20)       26 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/smhm_models/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3166 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/smhm_models/behroozi10.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.234744 halotools-0.8.1/halotools/empirical_models/composite_models/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3384 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/composite_models/tests/test_preloaded_models.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.242570 halotools-0.8.1/halotools/empirical_models/factories/
--rw-r--r--   0 aphearin   (501) staff       (20)      401 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/factories/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    24290 2021-03-06 19:16:34.000000 halotools-0.8.1/halotools/empirical_models/factories/hod_mock_factory.py
--rw-r--r--   0 aphearin   (501) staff       (20)    60636 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/factories/hod_model_factory.py
--rw-r--r--   0 aphearin   (501) staff       (20)    24512 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/factories/mock_factory_template.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2561 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/factories/mock_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)    34549 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/factories/model_factory_template.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13000 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/factories/prebuilt_model_factory.py
--rw-r--r--   0 aphearin   (501) staff       (20)    11211 2021-03-06 19:16:34.000000 halotools-0.8.1/halotools/empirical_models/factories/subhalo_mock_factory.py
--rw-r--r--   0 aphearin   (501) staff       (20)    45481 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/factories/subhalo_model_factory.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.248811 halotools-0.8.1/halotools/empirical_models/factories/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)       74 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/factories/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2107 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/factories/tests/test_clf_support.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4388 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/factories/tests/test_hod_factory.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9495 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/factories/tests/test_hod_mock_factory.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9593 2021-03-06 19:16:34.000000 halotools-0.8.1/halotools/empirical_models/factories/tests/test_hod_model_factory.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1023 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/factories/tests/test_mock_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1458 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/factories/tests/test_prebuilt_hod_model_factory.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2654 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/factories/tests/test_prebuilt_subhalo_model_factory.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8936 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/factories/tests/test_subhalo_model_factory.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3051 2021-03-06 19:16:34.000000 halotools-0.8.1/halotools/empirical_models/model_defaults.py
--rw-r--r--   0 aphearin   (501) staff       (20)    15586 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/model_helpers.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.255551 halotools-0.8.1/halotools/empirical_models/occupation_models/
--rw-r--r--   0 aphearin   (501) staff       (20)      227 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/__init__.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)    27900 2020-10-26 13:55:24.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/cacciato09_components.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.257199 halotools-0.8.1/halotools/empirical_models/occupation_models/engines/
--rw-r--r--   0 aphearin   (501) staff       (20)      296 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/engines/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4921 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/engines/cacciato09_sats_mc_prim_galprop_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)      920 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/engines/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)    19151 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/leauthaud11_components.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9722 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/occupation_model_template.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.261601 halotools-0.8.1/halotools/empirical_models/occupation_models/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/tests/__init__.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)    16108 2020-10-26 13:55:24.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_cacciato09_clf.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4872 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_leauthaud11_hod.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6051 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_occupation_component.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2749 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_tinker13.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7802 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_zheng07_centrals.py
--rw-r--r--   0 aphearin   (501) staff       (20)    11023 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_zheng07_satellites.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7768 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_zu_mandelbaum15_components.py
--rw-r--r--   0 aphearin   (501) staff       (20)    28194 2020-10-22 19:43:27.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/tinker13_components.py
--rw-r--r--   0 aphearin   (501) staff       (20)    32599 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/zheng07_components.py
--rw-r--r--   0 aphearin   (501) staff       (20)    12637 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/occupation_models/zu_mandelbaum15_components.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.262153 halotools-0.8.1/halotools/empirical_models/phase_space_models/
--rw-r--r--   0 aphearin   (501) staff       (20)       67 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.265021 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/
--rw-r--r--   0 aphearin   (501) staff       (20)      196 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.267084 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/centrals/
--rw-r--r--   0 aphearin   (501) staff       (20)       95 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/centrals/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.268623 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/centrals/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/centrals/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)      252 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/centrals/tests/test_trivial_phase_space.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1690 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/centrals/tests/test_trivial_profile.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2293 2020-10-22 19:43:27.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/centrals/trivial_phase_space.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4007 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/centrals/trivial_profile.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7479 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/halo_boundary_functions.py
--rw-r--r--   0 aphearin   (501) staff       (20)    28598 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/monte_carlo_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)    17446 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/profile_model_template.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.269162 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/
--rw-r--r--   0 aphearin   (501) staff       (20)       19 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.274125 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/
--rw-r--r--   0 aphearin   (501) staff       (20)      198 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    20411 2020-10-22 19:43:27.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/biased_nfw_phase_space.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.276494 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/
--rw-r--r--   0 aphearin   (501) staff       (20)      108 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1307 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/direct_from_halo_catalog.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1139 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/dutton_maccio14.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.277410 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1978 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/tests/test_conc_mass.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.280325 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/
--rw-r--r--   0 aphearin   (501) staff       (20)      533 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2448 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/biased_isotropic_velocity.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4201 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/mass_profile.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4562 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/mc_generate_nfw_radial_positions.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.283400 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.287052 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/
--rw-r--r--   0 aphearin   (501) staff       (20)      285 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/README.md
--rw-r--r--   0 aphearin   (501) staff       (20)    25000 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_c10.dat
--rw-r--r--   0 aphearin   (501) staff       (20)    25000 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_c5.dat
--rw-r--r--   0 aphearin   (501) staff       (20)     4800 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_ch10_cg5.dat
--rw-r--r--   0 aphearin   (501) staff       (20)     4800 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_ch5_cg10.dat
--rw-r--r--   0 aphearin   (501) staff       (20)        8 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1873 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/test_biased_isotropic_velocity.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1329 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/test_mc_generate_nfw_radial_positions.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1157 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/test_unbiased_isotropic_velocity.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1931 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/unbiased_isotropic_velocity.py
--rw-r--r--   0 aphearin   (501) staff       (20)    38761 2021-10-08 17:47:05.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/nfw_phase_space.py
--rw-r--r--   0 aphearin   (501) staff       (20)    24226 2021-03-06 19:16:34.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/nfw_profile.py
--rw-r--r--   0 aphearin   (501) staff       (20)    11700 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/sfr_biased_nfw_phase_space.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.287710 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.291864 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1203 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_consistency.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6762 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_consistency_mockpop.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3304 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_initialization.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2156 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_phase_space.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4584 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_phase_space_argument_handling.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5679 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_conc_gal_bias_behavior.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7641 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_mockpop.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.292904 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_conc_mass_inheritance/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_conc_mass_inheritance/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3375 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_conc_mass_inheritance/test_direct_from_halo_catalog.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.296169 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2019 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3928 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_argument_handling.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3455 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_functions.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1371 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_initialization.py
--rw-r--r--   0 aphearin   (501) staff       (20)    11333 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_monte_carlo.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.297876 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_profile/
--rw-r--r--   0 aphearin   (501) staff       (20)      153 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_profile/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1968 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_profile/test_colossus_consistency.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13287 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_profile/test_nfw_profile.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.298764 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4399 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/tests/test_halo_boundary_functions.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.301301 halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/
--rw-r--r--   0 aphearin   (501) staff       (20)      137 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    17503 2022-06-11 20:01:23.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/subhalo_phase_space.py
--rw-r--r--   0 aphearin   (501) staff       (20)    23321 2022-06-11 20:01:23.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/subhalo_selection_kernel.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.303678 halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2358 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/test_composite_model.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7617 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/test_subhalo_phase_space.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8463 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/test_subhalo_selection_kernel.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.305473 halotools-0.8.1/halotools/empirical_models/sfr_models/
--rw-r--r--   0 aphearin   (501) staff       (20)       66 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/sfr_models/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4250 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/sfr_models/halo_mass_quenching.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.306892 halotools-0.8.1/halotools/empirical_models/sfr_models/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/sfr_models/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1308 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/sfr_models/tests/test_halo_mass_quenching.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2419 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/sfr_models/tests/test_zu_mandelbaum16.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6066 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/sfr_models/zu_mandelbaum16.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.309660 halotools-0.8.1/halotools/empirical_models/smhm_models/
--rw-r--r--   0 aphearin   (501) staff       (20)      229 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/smhm_models/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9986 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/smhm_models/behroozi10.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5444 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/smhm_models/moster13.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2315 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/smhm_models/smhm_helpers.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.312148 halotools-0.8.1/halotools/empirical_models/smhm_models/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/smhm_models/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4945 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/smhm_models/tests/test_behroozi10.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4019 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/smhm_models/tests/test_moster13.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1615 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/smhm_models/tests/test_redshift_defensiveness.py
--rw-r--r--   0 aphearin   (501) staff       (20)      313 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/smhm_models/tests/test_zu_mandelbaum15.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7083 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/empirical_models/smhm_models/zu_mandelbaum15.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.313240 halotools-0.8.1/halotools/empirical_models/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)      153 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5307 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/empirical_models/tests/test_model_helpers.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.313773 halotools-0.8.1/halotools/extern/
--rw-r--r--   0 aphearin   (501) staff       (20)       72 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/extern/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.317885 halotools-0.8.1/halotools/mock_observables/
--rw-r--r--   0 aphearin   (501) staff       (20)      849 2021-08-04 18:44:34.000000 halotools-0.8.1/halotools/mock_observables/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    19580 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/catalog_analysis_helpers.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.318936 halotools-0.8.1/halotools/mock_observables/counts_in_cells/
--rw-r--r--   0 aphearin   (501) staff       (20)       61 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/counts_in_cells/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    14228 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/counts_in_cells/counts_in_cylinders.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.320619 halotools-0.8.1/halotools/mock_observables/counts_in_cells/engines/
--rw-r--r--   0 aphearin   (501) staff       (20)      267 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/counts_in_cells/engines/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.321162 halotools-0.8.1/halotools/mock_observables/counts_in_cells/engines/conditions/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/counts_in_cells/engines/conditions/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)      456 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/counts_in_cells/engines/conditions/conditions.pxd
--rw-r--r--   0 aphearin   (501) staff       (20)     2100 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/counts_in_cells/engines/conditions/conditions.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)    12742 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/counts_in_cells/engines/counts_in_cylinders_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)      908 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/mock_observables/counts_in_cells/engines/setup_package.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.322546 halotools-0.8.1/halotools/mock_observables/counts_in_cells/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/counts_in_cells/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2571 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/counts_in_cells/tests/pure_python_counts_in_cells.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13360 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/counts_in_cells/tests/test_counts_in_cylinders.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.323596 halotools-0.8.1/halotools/mock_observables/group_identification/
--rw-r--r--   0 aphearin   (501) staff       (20)      191 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/group_identification/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13492 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/group_identification/fof_groups.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.324829 halotools-0.8.1/halotools/mock_observables/group_identification/test_groups/
--rw-r--r--   0 aphearin   (501) staff       (20)      205 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/group_identification/test_groups/__init__.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)     2311 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/group_identification/test_groups/test_fof_groups.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.328554 halotools-0.8.1/halotools/mock_observables/isolation_functions/
--rw-r--r--   0 aphearin   (501) staff       (20)      506 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13584 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/conditional_cylindrical_isolation.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13009 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/conditional_spherical_isolation.py
--rw-r--r--   0 aphearin   (501) staff       (20)    11135 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/cylindrical_isolation.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.332834 halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/
--rw-r--r--   0 aphearin   (501) staff       (20)      607 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9509 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/cylindrical_isolation_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)      445 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/isolation_criteria_marking_functions.pxd
--rw-r--r--   0 aphearin   (501) staff       (20)     1385 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/isolation_criteria_marking_functions.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)    11583 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/marked_cylindrical_isolation_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)    11081 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/marked_spherical_isolation_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     1094 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9018 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/spherical_isolation_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     5590 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/isolation_functions_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9971 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/spherical_isolation.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.337340 halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1478 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/pure_python_isolation.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3526 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_brute_force_comparisons.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9198 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_conditional_cylindrical_isolation.py
--rw-r--r--   0 aphearin   (501) staff       (20)    21026 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_conditional_spherical_isolation.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5385 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_cylindrical_isolation.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2679 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_isolation_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1824 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_pure_python_isolation.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5633 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_spherical_isolation.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.338850 halotools-0.8.1/halotools/mock_observables/large_scale_density/
--rw-r--r--   0 aphearin   (501) staff       (20)      185 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/large_scale_density/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6628 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/large_scale_density/large_scale_density_spherical_annulus.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6216 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/large_scale_density/large_scale_density_spherical_volume.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.340244 halotools-0.8.1/halotools/mock_observables/large_scale_density/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/large_scale_density/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3256 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/large_scale_density/tests/test_large_scale_density_spherical_annulus.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2647 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/large_scale_density/tests/test_large_scale_density_spherical_volume.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6694 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/mock_observables_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3013 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/mock_survey.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6753 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/occupation_stats.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.351089 halotools-0.8.1/halotools/mock_observables/pair_counters/
--rw-r--r--   0 aphearin   (501) staff       (20)      781 2021-08-13 17:49:56.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.359996 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/
--rw-r--r--   0 aphearin   (501) staff       (20)     2133 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/README.md
--rw-r--r--   0 aphearin   (501) staff       (20)      811 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)      816 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/distances.pxd
--rw-r--r--   0 aphearin   (501) staff       (20)     3646 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/distances.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     7833 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_3d_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)    11213 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_jackknife_3d_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)    11852 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_jackknife_xy_z_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     8787 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_per_object_3d_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     8231 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_projected_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)    10212 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_s_mu_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     8487 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_xy_z_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     8295 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/pairwise_distance_3d_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     8935 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/pairwise_distance_xy_z_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)    13828 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/pairwise_distances.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     1247 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)    11358 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/weighted_npairs_s_mu_engine.pyx
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.366489 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/
--rw-r--r--   0 aphearin   (501) staff       (20)     3008 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/README.md
--rw-r--r--   0 aphearin   (501) staff       (20)      321 2021-08-13 17:49:56.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9850 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/conditional_pairwise_distances.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)      183 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/custom_marking_func.pxd
--rw-r--r--   0 aphearin   (501) staff       (20)      416 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/custom_marking_func.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)      189 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/custom_weighting_func.pxd
--rw-r--r--   0 aphearin   (501) staff       (20)      488 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/custom_weighting_func.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     1182 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/distances.pxd
--rw-r--r--   0 aphearin   (501) staff       (20)     3646 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/distances.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     9944 2021-08-13 17:49:56.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/marked_npairs_3d_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)    10460 2021-08-13 17:49:56.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/marked_npairs_xy_z_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)      827 2021-08-13 17:49:56.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/marking_functions.pxd
--rw-r--r--   0 aphearin   (501) staff       (20)     3080 2021-08-13 17:49:56.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/marking_functions.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     1008 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13365 2021-08-13 17:49:56.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_npairs_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7252 2021-08-13 17:49:56.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/marked_npairs_xy_z.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8827 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/mesh_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8739 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)    11157 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_jackknife_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)    11074 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_jackknife_xy_z.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6291 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_per_object_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9470 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_projected.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9326 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_s_mu.py
--rw-r--r--   0 aphearin   (501) staff       (20)    10379 2021-08-13 17:49:56.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_xy_z.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)    21710 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/pairs.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9618 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/pairwise_distance_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9780 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/pairwise_distance_xy_z.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13939 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/rectangular_mesh.py
--rw-r--r--   0 aphearin   (501) staff       (20)    11177 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/rectangular_mesh_2d.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.378648 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/
--rw-r--r--   0 aphearin   (501) staff       (20)      173 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2993 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/pure_python_distance_matrix.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1416 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/pure_python_npairs_per_object_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)    15923 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_marked_npairs_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)    18473 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_marked_npairs_xy_z.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2433 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_mesh_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2303 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_non_cubic_volumes.py
--rw-r--r--   0 aphearin   (501) staff       (20)    12676 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9727 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_jackknife_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)    11051 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_jackknife_xy_z.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3784 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_per_object_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)    14582 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_projected.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)     5991 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_s_mu.py
--rw-r--r--   0 aphearin   (501) staff       (20)    12993 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_xy_z.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)    10246 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_pairwise_distance_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7251 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_rectangular_mesh.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4060 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_weighted_npairs_s_mu.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3399 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_wnpairs_pure_python.py
--rw-r--r--   0 aphearin   (501) staff       (20)    10567 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pair_counters/weighted_npairs_s_mu.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.383756 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/
--rw-r--r--   0 aphearin   (501) staff       (20)      616 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.389126 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/
--rw-r--r--   0 aphearin   (501) staff       (20)      300 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9790 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/mean_radial_velocity_vs_r_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)    10019 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/radial_pvd_vs_r_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     1083 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)    10176 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/velocity_marked_npairs_3d_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)    10797 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/velocity_marked_npairs_xy_z_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)      842 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/velocity_marking_functions.pxd
--rw-r--r--   0 aphearin   (501) staff       (20)     8848 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/velocity_marking_functions.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)    10350 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/los_pvd_vs_rp.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9274 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/mean_los_velocity_vs_rp.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13065 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/mean_radial_velocity_vs_r.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4894 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/pairwise_velocities_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)    10461 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/radial_pvd_vs_r.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.395429 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2048 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/pure_python_mean_radial_velocity_vs_r.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8008 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_los_pvd_vs_rp.py
--rw-r--r--   0 aphearin   (501) staff       (20)    19225 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_mean_los_velocity_vs_rp.py
--rw-r--r--   0 aphearin   (501) staff       (20)    30303 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_mean_radial_velocity_vs_r.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6745 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_pairwise_velocity_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3816 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_pairwise_velocity_stats.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3195 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_pure_python_mean_radial_velocity_vs_r.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8682 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_radial_pvd_vs_r.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3329 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_velocity_marked_npairs_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13354 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/velocity_marked_npairs_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8874 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/pairwise_velocities/velocity_marked_npairs_xy_z.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.397407 halotools-0.8.1/halotools/mock_observables/radial_profiles/
--rw-r--r--   0 aphearin   (501) staff       (20)      198 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/radial_profiles/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.399255 halotools-0.8.1/halotools/mock_observables/radial_profiles/engines/
--rw-r--r--   0 aphearin   (501) staff       (20)       71 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/radial_profiles/engines/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9453 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/radial_profiles/engines/radial_profile_3d_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)      906 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/mock_observables/radial_profiles/engines/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13080 2021-08-04 18:44:34.000000 halotools-0.8.1/halotools/mock_observables/radial_profiles/radial_profile_3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4311 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/radial_profiles/radial_profiles_helpers.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.400295 halotools-0.8.1/halotools/mock_observables/radial_profiles/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/radial_profiles/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    16289 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/radial_profiles/tests/test_radial_profile_3d.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.404595 halotools-0.8.1/halotools/mock_observables/surface_density/
--rw-r--r--   0 aphearin   (501) staff       (20)      111 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.407814 halotools-0.8.1/halotools/mock_observables/surface_density/engines/
--rw-r--r--   0 aphearin   (501) staff       (20)      460 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/engines/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7544 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/engines/mean_delta_sigma_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     8824 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/engines/mean_ds_one_two_halo_decomp_halo_id_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     9511 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/engines/mean_ds_one_two_halo_decomp_rhalo_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)      997 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/mock_observables/surface_density/engines/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7601 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/engines/weighted_npairs_per_object_xy_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)     6584 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/engines/weighted_npairs_xy_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)    11566 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/mass_in_cylinders.py
--rw-r--r--   0 aphearin   (501) staff       (20)    15380 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/mean_delta_sigma.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2152 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/surface_density.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2614 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/surface_density_helpers.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.412927 halotools-0.8.1/halotools/mock_observables/surface_density/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1119 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/tests/pure_python_weighted_npairs_per_object_xy.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1293 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/tests/pure_python_weighted_npairs_xy.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4510 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_mass_in_cylinders.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3218 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_mean_delta_sigma.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1075 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_pure_python_weighted_npairs_xy.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2767 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_surface_density.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1563 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_surface_density_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4094 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_weighted_npairs_per_object_xy.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7323 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_weighted_npairs_xy.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6591 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/weighted_npairs_per_object_xy.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8669 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/surface_density/weighted_npairs_xy.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.414530 halotools-0.8.1/halotools/mock_observables/tensor_calculations/
--rw-r--r--   0 aphearin   (501) staff       (20)      179 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tensor_calculations/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.416095 halotools-0.8.1/halotools/mock_observables/tensor_calculations/engines/
--rw-r--r--   0 aphearin   (501) staff       (20)      155 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tensor_calculations/engines/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    10131 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tensor_calculations/engines/inertia_tensor_3d_engine.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)      904 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/mock_observables/tensor_calculations/engines/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8846 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tensor_calculations/inertia_tensor.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3777 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tensor_calculations/tensor_derived_quantities.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.417612 halotools-0.8.1/halotools/mock_observables/tensor_calculations/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)       83 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tensor_calculations/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6477 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tensor_calculations/tests/test_inertia_tensor.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3665 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tensor_calculations/tests/test_tensor_derived_quantities.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.420511 halotools-0.8.1/halotools/mock_observables/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5681 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tests/cf_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13358 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tests/test_catalog_analysis_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5276 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/tests/test_mock_observables_helpers.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)     1008 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tests/test_mock_survey.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3038 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/tests/test_occupation_stats.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.431945 halotools-0.8.1/halotools/mock_observables/two_point_clustering/
--rw-r--r--   0 aphearin   (501) staff       (20)     1055 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    12986 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/angular_tpcf.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3208 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/clustering_helpers.py
--rw-r--r--   0 aphearin   (501) staff       (20)    23103 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/marked_tpcf.py
--rw-r--r--   0 aphearin   (501) staff       (20)    17324 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/rp_pi_tpcf.py
--rw-r--r--   0 aphearin   (501) staff       (20)    20886 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/rp_pi_tpcf_jackknife.py
--rw-r--r--   0 aphearin   (501) staff       (20)    18908 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/s_mu_tpcf.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.442269 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2538 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/locate_external_unit_testing_data.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4088 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_angular_tpcf.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2231 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_clustering_helpers.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)    10223 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_marked_tpcf.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)     4003 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_rp_pi_tpcf.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8912 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_rp_pi_tpcf_jackknife.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)     2904 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_s_mu_tpcf.py
--rw-r--r--   0 aphearin   (501) staff       (20)    25238 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_tpcf.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1972 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_tpcf_estimators.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4369 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_tpcf_jackknife.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1510 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_tpcf_multipole.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)     9821 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_tpcf_one_two_halo.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)     4975 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_wp.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4221 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_wp_jackknife.py
--rw-r--r--   0 aphearin   (501) staff       (20)    19660 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tpcf.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5988 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tpcf_estimators.py
--rw-r--r--   0 aphearin   (501) staff       (20)    19869 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tpcf_jackknife.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2855 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tpcf_multipole.py
--rw-r--r--   0 aphearin   (501) staff       (20)    20404 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/tpcf_one_two_halo_decomp.py
--rw-r--r--   0 aphearin   (501) staff       (20)    10516 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/wp.py
--rw-r--r--   0 aphearin   (501) staff       (20)    19645 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/two_point_clustering/wp_jackknife.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.443403 halotools-0.8.1/halotools/mock_observables/velocity_decomposition/
--rw-r--r--   0 aphearin   (501) staff       (20)       89 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/velocity_decomposition/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8429 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/velocity_decomposition/radial_velocity_decomposition.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.444318 halotools-0.8.1/halotools/mock_observables/velocity_decomposition/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/velocity_decomposition/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7169 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/velocity_decomposition/tests/test_radial_velocity.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.446430 halotools-0.8.1/halotools/mock_observables/void_statistics/
--rw-r--r--   0 aphearin   (501) staff       (20)      229 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/void_statistics/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.448261 halotools-0.8.1/halotools/mock_observables/void_statistics/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/mock_observables/void_statistics/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6704 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/void_statistics/tests/test_underdensity_prob_func.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4375 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/void_statistics/tests/test_void_prob_func.py
--rw-r--r--   0 aphearin   (501) staff       (20)    10220 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/void_statistics/underdensity_prob_func.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9081 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/mock_observables/void_statistics/void_prob_func.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.460776 halotools-0.8.1/halotools/sim_manager/
--rw-r--r--   0 aphearin   (501) staff       (20)     1068 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    27209 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/cached_halo_catalog.py
--rw-r--r--   0 aphearin   (501) staff       (20)    45654 2022-09-28 16:33:58.000000 halotools-0.8.1/halotools/sim_manager/download_manager.py
--rw-r--r--   0 aphearin   (501) staff       (20)    11257 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/fake_sim.py
--rw-r--r--   0 aphearin   (501) staff       (20)    15326 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/halo_table_cache.py
--rw-r--r--   0 aphearin   (501) staff       (20)    15142 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/halo_table_cache_log_entry.py
--rw-r--r--   0 aphearin   (501) staff       (20)    14017 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/ptcl_table_cache.py
--rw-r--r--   0 aphearin   (501) staff       (20)    12036 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/ptcl_table_cache_log_entry.py
--rw-r--r--   0 aphearin   (501) staff       (20)    36766 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/rockstar_hlist_reader.py
--rw-r--r--   0 aphearin   (501) staff       (20)        8 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/sim_manager/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2193 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/sim_defaults.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6053 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/sim_manager/supported_sims.py
--rw-r--r--   0 aphearin   (501) staff       (20)    26344 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/sim_manager/tabular_ascii_reader.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.472099 halotools-0.8.1/halotools/sim_manager/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)      246 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.472668 halotools-0.8.1/halotools/sim_manager/tests/data/
--rw-r--r--   0 aphearin   (501) staff       (20)   299010 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/data/dummy_halocat_0.07812.list
--rw-r--r--   0 aphearin   (501) staff       (20)     1574 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/helper_functions.py
--rw-r--r--   0 aphearin   (501) staff       (20)    21319 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/sim_manager/tests/test_cached_halo_catalog.py
--rw-r--r--   0 aphearin   (501) staff       (20)    20010 2022-09-28 16:33:58.000000 halotools-0.8.1/halotools/sim_manager/tests/test_download_manager.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2773 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/test_fake_sim.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8454 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/test_halo_table_cache.py
--rw-r--r--   0 aphearin   (501) staff       (20)    15559 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/test_halo_table_cache_log_entry.py
--rw-r--r--   0 aphearin   (501) staff       (20)      983 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/test_load_default_halocat.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9640 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/test_ptcl_table_cache.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9557 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/test_ptcl_table_cache_log_entry.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13793 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/test_rockstar_hlist_reader.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3370 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/test_supported_sims.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8947 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/test_tabular_ascii_reader.py
--rw-r--r--   0 aphearin   (501) staff       (20)    19164 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/sim_manager/tests/test_user_supplied_halo_catalog.py
--rw-r--r--   0 aphearin   (501) staff       (20)    10670 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/tests/test_user_supplied_ptcl_catalog.py
--rw-r--r--   0 aphearin   (501) staff       (20)    19796 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/user_supplied_halo_catalog.py
--rw-r--r--   0 aphearin   (501) staff       (20)    13168 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/sim_manager/user_supplied_ptcl_catalog.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.479366 halotools-0.8.1/halotools/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)      121 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)      768 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/tests/coveragerc
--rw-r--r--   0 aphearin   (501) staff       (20)       57 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/tests/ddc.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.481425 halotools-0.8.1/halotools/tests/docs_code_block_tests/
--rw-r--r--   0 aphearin   (501) staff       (20)      256 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/tests/docs_code_block_tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    17744 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/tests/docs_code_block_tests/test_hod_model_factory_tutorial.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2093 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/tests/docs_code_block_tests/test_preloaded_mockpop.py
--rw-r--r--   0 aphearin   (501) staff       (20)        8 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/tests/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2499 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/tests/test_amurrica.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2172 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/tests/test_seed.py
--rw-r--r--   0 aphearin   (501) staff       (20)      336 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/tests/test_subpkg_imports.py
--rw-r--r--   0 aphearin   (501) staff       (20)      243 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/tests/usa.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.494574 halotools-0.8.1/halotools/utils/
--rw-r--r--   0 aphearin   (501) staff       (20)      692 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    14043 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/array_indexing_manipulations.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5919 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/array_utils.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5606 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/conditional_percentile.py
--rw-r--r--   0 aphearin   (501) staff       (20)     8476 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/crossmatch.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5671 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/distribution_matching.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.496295 halotools-0.8.1/halotools/utils/engines/
--rw-r--r--   0 aphearin   (501) staff       (20)       68 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/engines/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3989 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/engines/conditional_rank_kernel.pyx
--rw-r--r--   0 aphearin   (501) staff       (20)      905 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/utils/engines/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7275 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/group_member_generator.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9346 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/inverse_transformation_sampling.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1693 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/io_utils.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1582 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/load_umachine_binaries.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4642 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/mcrotations.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5420 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/probabilistic_binning.py
--rw-r--r--   0 aphearin   (501) staff       (20)      394 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/python_string_comparisons.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4895 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/rotations2d.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9228 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/rotations3d.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2679 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/spherical_geometry.py
--rw-r--r--   0 aphearin   (501) staff       (20)    15237 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/table_utils.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.507980 halotools-0.8.1/halotools/utils/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)      334 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/__init__.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.508527 halotools-0.8.1/halotools/utils/tests/data/
--rw-r--r--   0 aphearin   (501) staff       (20)       55 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/data/dummy_ascii.dat
--rw-r--r--   0 aphearin   (501) staff       (20)        8 2022-09-25 14:53:47.000000 halotools-0.8.1/halotools/utils/tests/setup_package.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2133 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/tests/test_2d_rotations.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3986 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/tests/test_3d_rotations.py
--rw-r--r--   0 aphearin   (501) staff       (20)    14233 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/test_array_indexing_manipulations.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1969 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/test_array_utils.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1680 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/test_compute_richness.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4997 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/test_conditional_percentile.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3786 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/test_crossmatch.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2385 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/test_distribution_matching.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7617 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/test_group_member_generator.py
--rw-r--r--   0 aphearin   (501) staff       (20)      238 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/test_io_utils.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3423 2020-12-11 16:11:40.000000 halotools-0.8.1/halotools/utils/tests/test_its.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1066 2020-10-22 19:43:27.000000 halotools-0.8.1/halotools/utils/tests/test_mcrotations.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3024 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/test_probabilistic_binning.py
--rw-r--r--   0 aphearin   (501) staff       (20)      233 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/test_python_string_comparisons.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1068 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/tests/test_rotate_vector_collection.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6447 2020-08-05 18:14:21.000000 halotools-0.8.1/halotools/utils/tests/test_table_utils.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4727 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/tests/test_value_added_halo_table_functions.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4504 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/tests/test_vector_utilities.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7248 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/value_added_halo_table_functions.py
--rw-r--r--   0 aphearin   (501) staff       (20)     9573 2022-09-23 19:40:55.000000 halotools-0.8.1/halotools/utils/vector_utilities.py
--rw-r--r--   0 aphearin   (501) staff       (20)      337 2022-09-28 17:03:31.000000 halotools-0.8.1/halotools/version.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.204913 halotools-0.8.1/halotools.egg-info/
--rw-r--r--   0 aphearin   (501) staff       (20)     9799 2022-09-28 17:03:31.000000 halotools-0.8.1/halotools.egg-info/PKG-INFO
--rw-r--r--   0 aphearin   (501) staff       (20)    50767 2022-09-28 17:03:31.000000 halotools-0.8.1/halotools.egg-info/SOURCES.txt
--rw-r--r--   0 aphearin   (501) staff       (20)        1 2022-09-28 17:03:31.000000 halotools-0.8.1/halotools.egg-info/dependency_links.txt
--rw-r--r--   0 aphearin   (501) staff       (20)       82 2022-09-28 17:03:31.000000 halotools-0.8.1/halotools.egg-info/entry_points.txt
--rw-r--r--   0 aphearin   (501) staff       (20)        1 2022-09-28 17:03:31.000000 halotools-0.8.1/halotools.egg-info/not-zip-safe
--rw-r--r--   0 aphearin   (501) staff       (20)      114 2022-09-28 17:03:31.000000 halotools-0.8.1/halotools.egg-info/requires.txt
--rw-r--r--   0 aphearin   (501) staff       (20)       10 2022-09-28 17:03:31.000000 halotools-0.8.1/halotools.egg-info/top_level.txt
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.509657 halotools-0.8.1/licenses/
--rw-r--r--   0 aphearin   (501) staff       (20)     1780 2022-09-23 19:40:55.000000 halotools-0.8.1/licenses/LICENSE.rst
--rw-r--r--   0 aphearin   (501) staff       (20)       87 2020-08-05 18:14:21.000000 halotools-0.8.1/licenses/README.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      244 2022-09-25 18:24:15.000000 halotools-0.8.1/pyproject.toml
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2022-09-28 17:03:32.514164 halotools-0.8.1/scripts/
--rw-r--r--   0 aphearin   (501) staff       (20)       87 2020-08-05 18:14:21.000000 halotools-0.8.1/scripts/README.rst
--rwxr-xr-x   0 aphearin   (501) staff       (20)     7286 2020-10-22 19:43:27.000000 halotools-0.8.1/scripts/convert_documentation_tutorials.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)     8172 2022-09-28 12:20:27.000000 halotools-0.8.1/scripts/download_additional_halocat.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)     5317 2020-08-05 18:14:21.000000 halotools-0.8.1/scripts/download_initial_halocat.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)     8840 2022-09-28 12:20:27.000000 halotools-0.8.1/scripts/rebuild_halo_table_cache_log.py
--rwxr-xr-x   0 aphearin   (501) staff       (20)     7469 2022-09-28 12:20:27.000000 halotools-0.8.1/scripts/rebuild_ptcl_table_cache_log.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1749 2022-09-28 17:03:32.516187 halotools-0.8.1/setup.cfg
--rwxr-xr-x   0 aphearin   (501) staff       (20)     2264 2022-09-28 12:20:27.000000 halotools-0.8.1/setup.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2354 2022-09-25 14:53:47.000000 halotools-0.8.1/tox.ini
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.737925 halotools-0.8.2/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.651034 halotools-0.8.2/.github/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.661198 halotools-0.8.2/.github/workflows/
+-rw-r--r--   0 aphearin   (501) staff       (20)     1480 2022-09-23 19:40:55.000000 halotools-0.8.2/.github/workflows/ci_tests.yml
+-rw-r--r--   0 aphearin   (501) staff       (20)      852 2023-06-30 17:38:52.000000 halotools-0.8.2/.github/workflows/wheels.yml
+-rw-r--r--   0 aphearin   (501) staff       (20)      683 2022-09-25 14:53:47.000000 halotools-0.8.2/.gitignore
+-rw-r--r--   0 aphearin   (501) staff       (20)      228 2022-09-23 19:40:55.000000 halotools-0.8.2/.readthedocs.yml
+-rw-r--r--   0 aphearin   (501) staff       (20)    10016 2023-06-30 17:39:30.000000 halotools-0.8.2/CHANGES.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      305 2022-09-27 18:06:44.000000 halotools-0.8.2/MANIFEST.in
+-rw-r--r--   0 aphearin   (501) staff       (20)     9824 2023-06-30 17:51:15.738031 halotools-0.8.2/PKG-INFO
+-rw-r--r--   0 aphearin   (501) staff       (20)     9397 2023-05-26 00:48:02.000000 halotools-0.8.2/README.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.661316 halotools-0.8.2/cextern/
+-rw-r--r--   0 aphearin   (501) staff       (20)      299 2020-08-05 18:14:21.000000 halotools-0.8.2/cextern/README.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.662284 halotools-0.8.2/docs/
+-rw-r--r--   0 aphearin   (501) staff       (20)     4724 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/Makefile
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.664381 halotools-0.8.2/docs/_static/
+-rw-r--r--   0 aphearin   (501) staff       (20)    16687 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/bijective_distribution_matching_demo.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    44595 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/cam_example_assembias_clf.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    12849 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/cam_example_bulge_disk_ratio.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    15023 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/cam_example_complex_sfr.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    15931 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/cam_example_complex_sfr_dmdt_correlation.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    12004 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/cam_example_complex_sfr_recovery.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    32174 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/color_correlation_pdf.png
+-rw-r--r--   0 aphearin   (501) staff       (20)   154081 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/dm-splatting-large.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    15955 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/fuzzy_binning_example.png
+-rw-r--r--   0 aphearin   (501) staff       (20)      104 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/halotools.css
+-rw-r--r--   0 aphearin   (501) staff       (20)    12194 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/matched_distributions.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    36072 2022-10-18 22:33:34.000000 halotools-0.8.2/docs/_static/mbk10_nsat_up0_behavior.png
+-rw-r--r--   0 aphearin   (501) staff       (20)     6699 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/monte_carlo_example.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    46403 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/monte_carlo_example2.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    28645 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/noisy_percentile_demo.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    32894 2022-10-18 22:33:34.000000 halotools-0.8.2/docs/_static/non_poisson_mc_realization.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    34365 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/quenching_gradient_model_clustering.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    32129 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/quenching_gradient_models.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    15404 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_static/spin_percentile.png
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.651302 halotools-0.8.2/docs/_templates/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.664672 halotools-0.8.2/docs/_templates/autosummary/
+-rw-r--r--   0 aphearin   (501) staff       (20)      250 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      251 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      252 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)       90 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/changelog.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     5042 2022-09-25 14:53:47.000000 halotools-0.8.2/docs/conf.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.664795 halotools-0.8.2/docs/full_ref_api/
+-rw-r--r--   0 aphearin   (501) staff       (20)      587 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/full_ref_api/halotools_full_api.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.665629 halotools-0.8.2/docs/function_usage/
+-rw-r--r--   0 aphearin   (501) staff       (20)      216 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/function_usage/abundance_matching.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      412 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/function_usage/empirical_model_factory_functions.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      578 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/function_usage/hod_occupation_functions.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     2033 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/function_usage/index.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1308 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/function_usage/mock_observables_functions.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      856 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/function_usage/phase_space_models_functions.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      452 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/function_usage/processing_simulation_data.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1093 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/function_usage/utility_functions.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1469 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/index.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     8696 2022-09-27 17:51:03.000000 halotools-0.8.2/docs/install.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1346 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/installation_troubleshooting.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1317 2022-09-23 19:40:55.000000 halotools-0.8.2/docs/installing_halotools_with_virtualenv.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     4513 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/make.bat
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.651970 halotools-0.8.2/docs/notebooks/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.666003 halotools-0.8.2/docs/notebooks/cam_modeling/
+-rw-r--r--   0 aphearin   (501) staff       (20)    59110 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/cam_modeling/cam_complex_sfr_tutorial.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    64871 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/cam_modeling/cam_decorated_clf.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    33338 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/cam_modeling/cam_disk_bulge_ratios_demo.ipynb
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.651712 halotools-0.8.2/docs/notebooks/galcat_analysis/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.667396 halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/
+-rw-r--r--   0 aphearin   (501) staff       (20)   132493 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial
+-rw-r--r--   0 aphearin   (501) staff       (20)    81382 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial1.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)     9983 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial10.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    41554 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial2.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    50743 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial3.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    59196 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial4.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    11038 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial5.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    26854 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial6.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    59055 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial7.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    39567 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial8.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)   319967 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial9.ipynb
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.667755 halotools-0.8.2/docs/notebooks/galcat_analysis/intermediate_examples/
+-rw-r--r--   0 aphearin   (501) staff       (20)    14432 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/intermediate_examples/galaxy_catalog_intermediate_analysis_tutorial1.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)   136855 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/galcat_analysis/intermediate_examples/quenching_gradient_tutorial.ipynb
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.651829 halotools-0.8.2/docs/notebooks/halocat_analysis/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.668054 halotools-0.8.2/docs/notebooks/halocat_analysis/basic_examples/
+-rw-r--r--   0 aphearin   (501) staff       (20)    20171 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial1.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    68521 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial2.ipynb
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.668690 halotools-0.8.2/docs/notebooks/hod_modeling/
+-rw-r--r--   0 aphearin   (501) staff       (20)    17926 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/hod_modeling/hod_modeling_tutorial1.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    14511 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/hod_modeling/hod_modeling_tutorial2.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)     5749 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/hod_modeling/hod_modeling_tutorial3.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    30300 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/hod_modeling/hod_modeling_tutorial4.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    49309 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/hod_modeling/hod_modeling_tutorial5.ipynb
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.669422 halotools-0.8.2/docs/notebooks/subhalo_modeling/
+-rw-r--r--   0 aphearin   (501) staff       (20)     9010 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial1.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    52926 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial2.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)     5822 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial3.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    37815 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial4.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    51211 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial5.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)     4996 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/overview.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.669724 halotools-0.8.2/docs/quickstart_and_tutorials/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.670321 halotools-0.8.2/docs/quickstart_and_tutorials/development/
+-rw-r--r--   0 aphearin   (501) staff       (20)      412 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/development/bug_reports.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     3027 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/development/citing_halotools.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      972 2022-09-23 19:40:55.000000 halotools-0.8.2/docs/quickstart_and_tutorials/development/contributors.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      429 2022-09-25 19:14:09.000000 halotools-0.8.2/docs/quickstart_and_tutorials/development/getting_started.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      357 2022-09-23 19:40:55.000000 halotools-0.8.2/docs/quickstart_and_tutorials/development/index.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    11937 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/getting_started_overview.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     2046 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/index.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.670452 halotools-0.8.2/docs/quickstart_and_tutorials/managing_catalogs/
+-rw-r--r--   0 aphearin   (501) staff       (20)     4780 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/managing_catalogs/supported_sim_list.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.670703 halotools-0.8.2/docs/quickstart_and_tutorials/mock_observations/
+-rw-r--r--   0 aphearin   (501) staff       (20)     5414 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/mock_observations/calculating_counts_in_cells.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     5657 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/mock_observations/mock_obs_pos_formatting.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.671079 halotools-0.8.2/docs/quickstart_and_tutorials/quickstart_guides/
+-rw-r--r--   0 aphearin   (501) staff       (20)     6594 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/quickstart_guides/halo_catalog_analysis_quickstart.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     2174 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/quickstart_guides/working_with_alternative_catalogs.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     4966 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/quickstart_guides/working_with_halotools_provided_catalogs.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.671588 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.653124 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.671713 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.672242 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.674311 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/
+-rw-r--r--   0 aphearin   (501) staff       (20)    35707 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/angular_crosscorr.png
+-rw-r--r--   0 aphearin   (501) staff       (20)     4759 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial2.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     7072 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial3.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     4494 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial4.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     9603 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial9.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    37960 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/gg_lensing_tutorial3.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    68942 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/mock_fullsky.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    15719 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/mock_octant.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    33076 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/one_two_halo_clustering.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    21885 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/output_9_1.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    21171 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/random_vs_analytic.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    48225 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/wp_red_blue_cross.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    43021 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/wp_tutorial4.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    14277 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/wtheta1.png
+-rw-r--r--   0 aphearin   (501) staff       (20)     2217 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/crossmatching_galaxy_catalogs.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     9422 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial1.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.674593 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/group_identification/
+-rw-r--r--   0 aphearin   (501) staff       (20)     9277 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/group_identification/galaxy_catalog_analysis_tutorial5.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     9795 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/group_identification/group_richness_vs_group_cenmass.png
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.674740 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/isolation_criteria/
+-rw-r--r--   0 aphearin   (501) staff       (20)     6496 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/isolation_criteria/galaxy_catalog_analysis_tutorial10.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    14222 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/output_18_1.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    26171 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/output_23_1.png
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.675322 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/
+-rw-r--r--   0 aphearin   (501) staff       (20)    18722 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/cluster_bcg_infall_velocity.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    30240 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/cluster_dispersion_profile.png
+-rw-r--r--   0 aphearin   (501) staff       (20)     4898 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/galaxy_catalog_analysis_tutorial6.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     4786 2022-09-17 13:29:45.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/galaxy_catalog_analysis_tutorial7.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.675601 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/void_stats/
+-rw-r--r--   0 aphearin   (501) staff       (20)     4124 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/void_stats/galaxy_catalog_analysis_tutorial8.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    18713 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/void_stats/vpf_upf_tutorial.png
+-rw-r--r--   0 aphearin   (501) staff       (20)     2842 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/index.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.653061 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/intermediate_examples/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.675763 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/intermediate_examples/isolation_criteria/
+-rw-r--r--   0 aphearin   (501) staff       (20)    11442 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/intermediate_examples/isolation_criteria/galaxy_catalog_intermediate_analysis_tutorial1.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.676232 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.676601 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.676838 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/figs/
+-rw-r--r--   0 aphearin   (501) staff       (20)    19523 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/figs/radial_profile_halocat_tutorial_fig1.png
+-rw-r--r--   0 aphearin   (501) staff       (20)    23205 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/figs/radial_profile_halocat_tutorial_fig2.png
+-rw-r--r--   0 aphearin   (501) staff       (20)     5950 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial1.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     6486 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial2.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     9024 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/nsub_vs_hostmass.png
+-rw-r--r--   0 aphearin   (501) staff       (20)     4140 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/crossmatching_halo_catalogs.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1536 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/index.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     4584 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/rockstar_subhalo_nomenclature.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    81243 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/subhalo_membership.png
+-rw-r--r--   0 aphearin   (501) staff       (20)     5783 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/merger_tree_analysis_example.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.677230 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/
+-rw-r--r--   0 aphearin   (501) staff       (20)      827 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/altering_param_dict.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.677764 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/
+-rw-r--r--   0 aphearin   (501) staff       (20)     3637 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_complex_sfr.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     4139 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_decorated_clf.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     3520 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_disk_bulge_ratios.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     2180 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_quenching_gradients.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     7131 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_tutorial.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.677882 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.678842 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/
+-rw-r--r--   0 aphearin   (501) staff       (20)      710 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial0.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     9555 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial1.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     6646 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial2.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    10285 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial3.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    10856 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial4.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     7554 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial5.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     6902 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/writing_your_own_hod_occupation_component.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      261 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/writing_your_own_hod_profile_component.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     3412 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/zheng07_using_cenocc_model_tutorial.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1921 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/index.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.679539 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/
+-rw-r--r--   0 aphearin   (501) staff       (20)      741 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial0.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     8148 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial1.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     5335 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial2.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     9051 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial3.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    10729 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial4.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     7056 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial5.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)   131548 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/halotools_design.png
+-rw-r--r--   0 aphearin   (501) staff       (20)     3529 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/index.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.680733 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)      482 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/abundance_matching_composite_model.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     6845 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/behroozi10_composite_model.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     7468 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/cacciato09_composite_model.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     8057 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/hearin15_composite_model.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     4259 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/index.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     7617 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/leauthaud11_composite_model.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      787 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/preloaded_models_list.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     6181 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/tinker13_composite_model.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     8034 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/zheng07_composite_model.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     8093 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/zu_mandelbaum15_composite_model.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     7458 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/zu_mandelbaum16_composite_model.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     8838 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/reducing_and_caching_a_new_rockstar_catalog.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     4447 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/user_supplied_halo_catalogs.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     3451 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/working_with_alternative_particle_data.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.680936 halotools-0.8.2/docs/source_notes/
+-rw-r--r--   0 aphearin   (501) staff       (20)     3769 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/convert_tutorials.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.653890 halotools-0.8.2/docs/source_notes/empirical_models/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.681037 halotools-0.8.2/docs/source_notes/empirical_models/assembias_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)      211 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/empirical_models/assembias_models/heaviside_assembias_source_code_notes.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.681852 halotools-0.8.2/docs/source_notes/empirical_models/factories/
+-rw-r--r--   0 aphearin   (501) staff       (20)    21897 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/empirical_models/factories/hod_mock_factory_source_notes.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    12746 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/empirical_models/factories/hod_model_factory_source_notes.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      882 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/empirical_models/factories/index.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    16187 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/empirical_models/factories/model_factory_composite_sequence_mechanisms.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)   165846 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/empirical_models/factories/np_repeat_tutorial.png
+-rw-r--r--   0 aphearin   (501) staff       (20)     5532 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/empirical_models/factories/subhalo_mock_factory_source_notes.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    12008 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/empirical_models/factories/subhalo_model_factory_source_notes.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.682261 halotools-0.8.2/docs/source_notes/empirical_models/phase_space_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)     2770 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/empirical_models/phase_space_models/jeans_equation_derivations.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      943 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/empirical_models/phase_space_models/monte_carlo_galprof_source_notes.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    22266 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/empirical_models/phase_space_models/nfw_profile_source_notes.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)    15674 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/empirical_models/phase_space_models/profile_template_source_notes.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1135 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/index.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.682366 halotools-0.8.2/docs/source_notes/mock_observables/
+-rw-r--r--   0 aphearin   (501) staff       (20)     4354 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/source_notes/mock_observables/zspace_distortions.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.654107 halotools-0.8.2/docs/usage_tutorials/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.682497 halotools-0.8.2/docs/usage_tutorials/cache_management/
+-rw-r--r--   0 aphearin   (501) staff       (20)     4365 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/usage_tutorials/cache_management/relocating_simulation_data.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.654197 halotools-0.8.2/docs/usage_tutorials/empirical_models/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.682631 halotools-0.8.2/docs/usage_tutorials/empirical_models/assembias_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)     4783 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/usage_tutorials/empirical_models/assembias_models/heaviside_assembias_tutorial.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.682753 halotools-0.8.2/docs/usage_tutorials/empirical_models/subhalo_phase_space/
+-rw-r--r--   0 aphearin   (501) staff       (20)    10877 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/usage_tutorials/empirical_models/subhalo_phase_space/subhalo_phase_space_tutorial.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      452 2022-09-23 19:40:55.000000 halotools-0.8.2/docs/whats_new.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.683337 halotools-0.8.2/docs/whats_new_history/
+-rw-r--r--   0 aphearin   (501) staff       (20)     6992 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/whats_new_history/whats_new_0.5.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     2136 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/whats_new_history/whats_new_0.6.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     2086 2020-08-05 18:14:21.000000 halotools-0.8.2/docs/whats_new_history/whats_new_0.7.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      457 2022-09-23 19:40:55.000000 halotools-0.8.2/docs/whats_new_history/whats_new_0.8.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      337 2022-09-23 19:40:55.000000 halotools-0.8.2/docs/whats_new_history/whats_new_v0x_history.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.683937 halotools-0.8.2/halotools/
+-rw-r--r--   0 aphearin   (501) staff       (20)      427 2022-09-15 17:03:51.000000 halotools-0.8.2/halotools/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      356 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/_astropy_init.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2720 2023-06-30 17:51:15.000000 halotools-0.8.2/halotools/_compiler.c
+-rw-r--r--   0 aphearin   (501) staff       (20)     1081 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/conftest.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1681 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/custom_exceptions.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.684719 halotools-0.8.2/halotools/data/
+-rw-r--r--   0 aphearin   (501) staff       (20)      200 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/data/README.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.685010 halotools-0.8.2/halotools/empirical_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)      510 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/empirical_models/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.685413 halotools-0.8.2/halotools/empirical_models/abunmatch/
+-rw-r--r--   0 aphearin   (501) staff       (20)      175 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6484 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/bin_free_cam.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8805 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/conditional_abunmatch_bin_based.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.685715 halotools-0.8.2/halotools/empirical_models/abunmatch/engines/
+-rw-r--r--   0 aphearin   (501) staff       (20)       79 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/engines/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    12050 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/engines/bin_free_cam_kernel.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)      901 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/engines/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7869 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/noisy_percentile.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.686563 halotools-0.8.2/halotools/empirical_models/abunmatch/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1326 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/tests/naive_python_cam.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    17601 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/tests/test_bin_free_cam.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1595 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/tests/test_conditional_abunmatch.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1168 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/tests/test_noisy_percentile.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4440 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/tests/test_pure_python.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3974 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/tests/test_sample2_window_function.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      163 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/abunmatch/tests/test_single_unit.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.686772 halotools-0.8.2/halotools/empirical_models/assembias_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)       35 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/assembias_models/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    24275 2022-09-25 18:24:15.000000 halotools-0.8.2/halotools/empirical_models/assembias_models/heaviside_assembias.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.686982 halotools-0.8.2/halotools/empirical_models/assembias_models/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/assembias_models/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3589 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/assembias_models/tests/test_assembias.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.687384 halotools-0.8.2/halotools/empirical_models/component_model_templates/
+-rw-r--r--   0 aphearin   (501) staff       (20)      116 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/component_model_templates/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    14084 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/component_model_templates/binary_galprop_models.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8107 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/component_model_templates/prim_galprop_model.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6792 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/component_model_templates/scatter_models.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.687755 halotools-0.8.2/halotools/empirical_models/component_model_templates/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/component_model_templates/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3129 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/component_model_templates/tests/test_binary_galprop_models.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3708 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/component_model_templates/tests/test_prim_galprop_model.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9015 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/component_model_templates/tests/test_scatter_models.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.687856 halotools-0.8.2/halotools/empirical_models/composite_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)      307 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.688658 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)      186 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4363 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/cacciato09.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5274 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/hearin15.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4450 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/leauthaud11.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.689079 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1491 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/tests/test_tinker13.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4088 2021-03-06 19:16:34.000000 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/tests/test_zheng07.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2608 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/tests/test_zu_mandelbaum16.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5470 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/tinker13.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5150 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/zheng07.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5435 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/zu_mandelbaum15.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6105 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/zu_mandelbaum16.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.689301 halotools-0.8.2/halotools/empirical_models/composite_models/sfr_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)       31 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/sfr_models/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3881 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/sfr_models/smhm_binary_sfr.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.689514 halotools-0.8.2/halotools/empirical_models/composite_models/smhm_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)       26 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/smhm_models/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3166 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/smhm_models/behroozi10.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.689723 halotools-0.8.2/halotools/empirical_models/composite_models/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3384 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/composite_models/tests/test_preloaded_models.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.690772 halotools-0.8.2/halotools/empirical_models/factories/
+-rw-r--r--   0 aphearin   (501) staff       (20)      401 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/factories/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    24290 2021-03-06 19:16:34.000000 halotools-0.8.2/halotools/empirical_models/factories/hod_mock_factory.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    60636 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/factories/hod_model_factory.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    24512 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/factories/mock_factory_template.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2561 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/factories/mock_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    34549 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/factories/model_factory_template.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13000 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/factories/prebuilt_model_factory.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    11211 2021-03-06 19:16:34.000000 halotools-0.8.2/halotools/empirical_models/factories/subhalo_mock_factory.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    45481 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/factories/subhalo_model_factory.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.691799 halotools-0.8.2/halotools/empirical_models/factories/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)       74 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/factories/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2107 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/factories/tests/test_clf_support.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4388 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/factories/tests/test_hod_factory.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9388 2023-06-30 17:38:52.000000 halotools-0.8.2/halotools/empirical_models/factories/tests/test_hod_mock_factory.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9593 2021-03-06 19:16:34.000000 halotools-0.8.2/halotools/empirical_models/factories/tests/test_hod_model_factory.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1023 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/factories/tests/test_mock_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1458 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/factories/tests/test_prebuilt_hod_model_factory.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2654 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/factories/tests/test_prebuilt_subhalo_model_factory.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8936 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/factories/tests/test_subhalo_model_factory.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3051 2021-03-06 19:16:34.000000 halotools-0.8.2/halotools/empirical_models/model_defaults.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    15586 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/model_helpers.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.692772 halotools-0.8.2/halotools/empirical_models/occupation_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)      265 2022-10-18 22:33:34.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/__init__.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)    28359 2022-10-18 22:33:34.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/cacciato09_components.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.693123 halotools-0.8.2/halotools/empirical_models/occupation_models/engines/
+-rw-r--r--   0 aphearin   (501) staff       (20)      296 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/engines/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4921 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/engines/cacciato09_sats_mc_prim_galprop_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)      920 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/engines/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    33060 2023-06-29 23:56:11.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/leauthaud11_components.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    14058 2022-10-18 22:33:34.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/negative_binomial_sats.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9722 2022-10-07 22:20:51.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/occupation_model_template.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.694175 halotools-0.8.2/halotools/empirical_models/occupation_models/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/tests/__init__.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)    16108 2020-10-26 13:55:24.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_cacciato09_clf.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4925 2023-06-29 23:56:11.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_leauthaud11_hod.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4057 2022-10-18 22:33:34.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_negative_binomial_sats.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6051 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_occupation_component.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2749 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_tinker13.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7802 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_zheng07_centrals.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    11034 2023-02-09 21:46:23.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_zheng07_satellites.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7768 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_zu_mandelbaum15_components.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    28929 2022-10-18 22:33:34.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/tinker13_components.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    33452 2022-10-18 22:33:34.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/zheng07_components.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    12633 2022-10-18 22:33:34.000000 halotools-0.8.2/halotools/empirical_models/occupation_models/zu_mandelbaum15_components.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.694270 halotools-0.8.2/halotools/empirical_models/phase_space_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)       67 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.694682 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)      196 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.694997 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/centrals/
+-rw-r--r--   0 aphearin   (501) staff       (20)       95 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/centrals/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.695349 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/centrals/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/centrals/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      252 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/centrals/tests/test_trivial_phase_space.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1690 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/centrals/tests/test_trivial_profile.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2293 2020-10-22 19:43:27.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/centrals/trivial_phase_space.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4007 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/centrals/trivial_profile.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7479 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/halo_boundary_functions.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    28598 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/monte_carlo_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    17446 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/profile_model_template.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.695469 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/
+-rw-r--r--   0 aphearin   (501) staff       (20)       19 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.696128 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/
+-rw-r--r--   0 aphearin   (501) staff       (20)      198 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    20395 2023-06-29 23:56:11.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/biased_nfw_phase_space.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.696505 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/
+-rw-r--r--   0 aphearin   (501) staff       (20)      108 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1350 2023-06-29 23:56:11.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/direct_from_halo_catalog.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1138 2023-06-29 23:56:11.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/dutton_maccio14.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.696743 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1978 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/tests/test_conc_mass.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.697385 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/
+-rw-r--r--   0 aphearin   (501) staff       (20)      542 2023-06-29 23:56:11.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2584 2023-06-29 23:56:11.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/biased_isotropic_velocity.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4222 2023-06-29 23:56:11.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/mass_profile.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4583 2023-06-29 23:56:11.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/mc_generate_nfw_radial_positions.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.698023 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.698742 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/
+-rw-r--r--   0 aphearin   (501) staff       (20)      285 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/README.md
+-rw-r--r--   0 aphearin   (501) staff       (20)    25000 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_c10.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)    25000 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_c5.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)     4800 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_ch10_cg5.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)     4800 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_ch5_cg10.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)        8 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1873 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/test_biased_isotropic_velocity.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1329 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/test_mc_generate_nfw_radial_positions.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1157 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/test_unbiased_isotropic_velocity.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1977 2023-06-29 23:56:11.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/unbiased_isotropic_velocity.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    39060 2023-06-30 13:33:08.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/nfw_phase_space.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    24220 2023-06-29 23:56:11.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/nfw_profile.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    11962 2023-06-29 23:56:11.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/sfr_biased_nfw_phase_space.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.698876 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.699892 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1203 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_consistency.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6762 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_consistency_mockpop.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3304 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_initialization.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2156 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_phase_space.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4584 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_phase_space_argument_handling.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5679 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_conc_gal_bias_behavior.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7641 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_mockpop.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.700147 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_conc_mass_inheritance/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_conc_mass_inheritance/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3375 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_conc_mass_inheritance/test_direct_from_halo_catalog.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.700826 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2019 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3928 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_argument_handling.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3455 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_functions.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1371 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_initialization.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    11333 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_monte_carlo.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.701164 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_profile/
+-rw-r--r--   0 aphearin   (501) staff       (20)      153 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_profile/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1968 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_profile/test_colossus_consistency.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13287 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_profile/test_nfw_profile.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.701374 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4399 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/tests/test_halo_boundary_functions.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.701711 halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)      137 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    17503 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/subhalo_phase_space.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    23321 2022-06-11 20:01:23.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/subhalo_selection_kernel.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.702167 halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2358 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/test_composite_model.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7617 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/test_subhalo_phase_space.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8463 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/test_subhalo_selection_kernel.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.702493 halotools-0.8.2/halotools/empirical_models/sfr_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)       66 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/sfr_models/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4250 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/sfr_models/halo_mass_quenching.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.702805 halotools-0.8.2/halotools/empirical_models/sfr_models/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/sfr_models/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1308 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/sfr_models/tests/test_halo_mass_quenching.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2419 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/sfr_models/tests/test_zu_mandelbaum16.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6066 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/sfr_models/zu_mandelbaum16.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.703322 halotools-0.8.2/halotools/empirical_models/smhm_models/
+-rw-r--r--   0 aphearin   (501) staff       (20)      229 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/smhm_models/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9986 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/smhm_models/behroozi10.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5444 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/smhm_models/moster13.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2315 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/smhm_models/smhm_helpers.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.703886 halotools-0.8.2/halotools/empirical_models/smhm_models/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/smhm_models/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4945 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/smhm_models/tests/test_behroozi10.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4019 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/smhm_models/tests/test_moster13.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1615 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/smhm_models/tests/test_redshift_defensiveness.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      313 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/smhm_models/tests/test_zu_mandelbaum15.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7083 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/empirical_models/smhm_models/zu_mandelbaum15.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.704137 halotools-0.8.2/halotools/empirical_models/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)      153 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5307 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/empirical_models/tests/test_model_helpers.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.704247 halotools-0.8.2/halotools/extern/
+-rw-r--r--   0 aphearin   (501) staff       (20)       72 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/extern/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.704748 halotools-0.8.2/halotools/mock_observables/
+-rw-r--r--   0 aphearin   (501) staff       (20)      849 2021-08-04 18:44:34.000000 halotools-0.8.2/halotools/mock_observables/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    19930 2023-06-30 13:08:32.000000 halotools-0.8.2/halotools/mock_observables/catalog_analysis_helpers.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.704947 halotools-0.8.2/halotools/mock_observables/counts_in_cells/
+-rw-r--r--   0 aphearin   (501) staff       (20)       61 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/counts_in_cells/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    14228 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/counts_in_cells/counts_in_cylinders.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.705293 halotools-0.8.2/halotools/mock_observables/counts_in_cells/engines/
+-rw-r--r--   0 aphearin   (501) staff       (20)      267 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/counts_in_cells/engines/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.705506 halotools-0.8.2/halotools/mock_observables/counts_in_cells/engines/conditions/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/counts_in_cells/engines/conditions/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      456 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/counts_in_cells/engines/conditions/conditions.pxd
+-rw-r--r--   0 aphearin   (501) staff       (20)     2100 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/counts_in_cells/engines/conditions/conditions.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)    12742 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/counts_in_cells/engines/counts_in_cylinders_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)      908 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/mock_observables/counts_in_cells/engines/setup_package.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.705862 halotools-0.8.2/halotools/mock_observables/counts_in_cells/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/counts_in_cells/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2571 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/counts_in_cells/tests/pure_python_counts_in_cells.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13360 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/counts_in_cells/tests/test_counts_in_cylinders.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.706105 halotools-0.8.2/halotools/mock_observables/group_identification/
+-rw-r--r--   0 aphearin   (501) staff       (20)      191 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/group_identification/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13492 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/group_identification/fof_groups.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.706361 halotools-0.8.2/halotools/mock_observables/group_identification/test_groups/
+-rw-r--r--   0 aphearin   (501) staff       (20)      205 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/group_identification/test_groups/__init__.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     2311 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/group_identification/test_groups/test_fof_groups.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.707077 halotools-0.8.2/halotools/mock_observables/isolation_functions/
+-rw-r--r--   0 aphearin   (501) staff       (20)      506 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13584 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/conditional_cylindrical_isolation.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13009 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/conditional_spherical_isolation.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    11135 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/cylindrical_isolation.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.707927 halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/
+-rw-r--r--   0 aphearin   (501) staff       (20)      607 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9509 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/cylindrical_isolation_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)      445 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/isolation_criteria_marking_functions.pxd
+-rw-r--r--   0 aphearin   (501) staff       (20)     1385 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/isolation_criteria_marking_functions.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)    11583 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/marked_cylindrical_isolation_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)    11081 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/marked_spherical_isolation_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     1094 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9018 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/spherical_isolation_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     5590 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/isolation_functions_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9971 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/spherical_isolation.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.708937 halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1478 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/pure_python_isolation.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3526 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_brute_force_comparisons.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9198 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_conditional_cylindrical_isolation.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    21026 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_conditional_spherical_isolation.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5385 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_cylindrical_isolation.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2679 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_isolation_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1824 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_pure_python_isolation.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5633 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_spherical_isolation.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.709303 halotools-0.8.2/halotools/mock_observables/large_scale_density/
+-rw-r--r--   0 aphearin   (501) staff       (20)      185 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/large_scale_density/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6628 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/large_scale_density/large_scale_density_spherical_annulus.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6216 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/large_scale_density/large_scale_density_spherical_volume.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.709605 halotools-0.8.2/halotools/mock_observables/large_scale_density/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/large_scale_density/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3256 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/large_scale_density/tests/test_large_scale_density_spherical_annulus.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2647 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/large_scale_density/tests/test_large_scale_density_spherical_volume.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6694 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/mock_observables_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3013 2023-06-29 23:56:00.000000 halotools-0.8.2/halotools/mock_observables/mock_survey.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6753 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/occupation_stats.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.711449 halotools-0.8.2/halotools/mock_observables/pair_counters/
+-rw-r--r--   0 aphearin   (501) staff       (20)      781 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.713127 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/
+-rw-r--r--   0 aphearin   (501) staff       (20)     2133 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/README.md
+-rw-r--r--   0 aphearin   (501) staff       (20)      811 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      816 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/distances.pxd
+-rw-r--r--   0 aphearin   (501) staff       (20)     3646 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/distances.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     7833 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_3d_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)    11213 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_jackknife_3d_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)    11852 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_jackknife_xy_z_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     8787 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_per_object_3d_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     8231 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_projected_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)    10212 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_s_mu_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     8487 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_xy_z_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     8295 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/pairwise_distance_3d_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     8935 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/pairwise_distance_xy_z_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)    13828 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/pairwise_distances.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     1247 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    11358 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/weighted_npairs_s_mu_engine.pyx
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.714322 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/
+-rw-r--r--   0 aphearin   (501) staff       (20)     3008 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/README.md
+-rw-r--r--   0 aphearin   (501) staff       (20)      321 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9850 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/conditional_pairwise_distances.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)      183 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/custom_marking_func.pxd
+-rw-r--r--   0 aphearin   (501) staff       (20)      416 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/custom_marking_func.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)      189 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/custom_weighting_func.pxd
+-rw-r--r--   0 aphearin   (501) staff       (20)      488 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/custom_weighting_func.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     1182 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/distances.pxd
+-rw-r--r--   0 aphearin   (501) staff       (20)     3646 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/distances.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     9944 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/marked_npairs_3d_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)    10460 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/marked_npairs_xy_z_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)      827 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/marking_functions.pxd
+-rw-r--r--   0 aphearin   (501) staff       (20)     3080 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/marking_functions.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     1008 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13365 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_npairs_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7252 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/marked_npairs_xy_z.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8827 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/mesh_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8739 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    11157 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_jackknife_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    11074 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_jackknife_xy_z.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6291 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_per_object_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9470 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_projected.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9326 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_s_mu.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    10379 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_xy_z.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)    21710 2023-05-26 00:47:53.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/pairs.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9618 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/pairwise_distance_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9780 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/pairwise_distance_xy_z.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13939 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/rectangular_mesh.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    11177 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/rectangular_mesh_2d.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.716279 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/
+-rw-r--r--   0 aphearin   (501) staff       (20)      173 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2993 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/pure_python_distance_matrix.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1416 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/pure_python_npairs_per_object_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    15923 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_marked_npairs_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    18473 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_marked_npairs_xy_z.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2433 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_mesh_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2303 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_non_cubic_volumes.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    12676 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9727 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_jackknife_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    11051 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_jackknife_xy_z.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3784 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_per_object_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    14582 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_projected.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     5991 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_s_mu.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    12993 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_xy_z.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)    10246 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_pairwise_distance_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7251 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_rectangular_mesh.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4060 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_weighted_npairs_s_mu.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3399 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_wnpairs_pure_python.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    10567 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pair_counters/weighted_npairs_s_mu.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.717122 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/
+-rw-r--r--   0 aphearin   (501) staff       (20)      616 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.718058 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/
+-rw-r--r--   0 aphearin   (501) staff       (20)      300 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9790 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/mean_radial_velocity_vs_r_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)    10019 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/radial_pvd_vs_r_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     1083 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    10176 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/velocity_marked_npairs_3d_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)    10797 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/velocity_marked_npairs_xy_z_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)      842 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/velocity_marking_functions.pxd
+-rw-r--r--   0 aphearin   (501) staff       (20)     8848 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/velocity_marking_functions.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)    10350 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/los_pvd_vs_rp.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9274 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/mean_los_velocity_vs_rp.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13065 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/mean_radial_velocity_vs_r.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4894 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/pairwise_velocities_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    10461 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/radial_pvd_vs_r.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.719114 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2048 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/pure_python_mean_radial_velocity_vs_r.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8008 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_los_pvd_vs_rp.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    19225 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_mean_los_velocity_vs_rp.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    30303 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_mean_radial_velocity_vs_r.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6745 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_pairwise_velocity_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3816 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_pairwise_velocity_stats.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3195 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_pure_python_mean_radial_velocity_vs_r.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8682 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_radial_pvd_vs_r.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3329 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_velocity_marked_npairs_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13354 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/velocity_marked_npairs_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8874 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/pairwise_velocities/velocity_marked_npairs_xy_z.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.719406 halotools-0.8.2/halotools/mock_observables/radial_profiles/
+-rw-r--r--   0 aphearin   (501) staff       (20)      198 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/radial_profiles/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.719692 halotools-0.8.2/halotools/mock_observables/radial_profiles/engines/
+-rw-r--r--   0 aphearin   (501) staff       (20)       71 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/radial_profiles/engines/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9453 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/radial_profiles/engines/radial_profile_3d_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)      906 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/mock_observables/radial_profiles/engines/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13080 2021-08-04 18:44:34.000000 halotools-0.8.2/halotools/mock_observables/radial_profiles/radial_profile_3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4311 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/radial_profiles/radial_profiles_helpers.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.719865 halotools-0.8.2/halotools/mock_observables/radial_profiles/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/radial_profiles/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    16289 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/radial_profiles/tests/test_radial_profile_3d.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.720555 halotools-0.8.2/halotools/mock_observables/surface_density/
+-rw-r--r--   0 aphearin   (501) staff       (20)      111 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.721125 halotools-0.8.2/halotools/mock_observables/surface_density/engines/
+-rw-r--r--   0 aphearin   (501) staff       (20)      460 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/engines/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7544 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/engines/mean_delta_sigma_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     8824 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/engines/mean_ds_one_two_halo_decomp_halo_id_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     9511 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/engines/mean_ds_one_two_halo_decomp_rhalo_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)      997 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/mock_observables/surface_density/engines/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7601 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/engines/weighted_npairs_per_object_xy_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)     6584 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/engines/weighted_npairs_xy_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)    11566 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/mass_in_cylinders.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    15380 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/mean_delta_sigma.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2152 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/surface_density.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2614 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/surface_density_helpers.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.722294 halotools-0.8.2/halotools/mock_observables/surface_density/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1119 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/tests/pure_python_weighted_npairs_per_object_xy.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1293 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/tests/pure_python_weighted_npairs_xy.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4510 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_mass_in_cylinders.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3218 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_mean_delta_sigma.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1075 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_pure_python_weighted_npairs_xy.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2767 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_surface_density.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1563 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_surface_density_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4094 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_weighted_npairs_per_object_xy.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7323 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_weighted_npairs_xy.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6591 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/weighted_npairs_per_object_xy.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8669 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/surface_density/weighted_npairs_xy.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.722665 halotools-0.8.2/halotools/mock_observables/tensor_calculations/
+-rw-r--r--   0 aphearin   (501) staff       (20)      179 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/tensor_calculations/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.723034 halotools-0.8.2/halotools/mock_observables/tensor_calculations/engines/
+-rw-r--r--   0 aphearin   (501) staff       (20)      155 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/tensor_calculations/engines/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    10131 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/tensor_calculations/engines/inertia_tensor_3d_engine.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)      904 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/mock_observables/tensor_calculations/engines/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8846 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/tensor_calculations/inertia_tensor.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3777 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/tensor_calculations/tensor_derived_quantities.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.723425 halotools-0.8.2/halotools/mock_observables/tensor_calculations/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)       83 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/tensor_calculations/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6477 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/tensor_calculations/tests/test_inertia_tensor.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3665 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/tensor_calculations/tests/test_tensor_derived_quantities.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.724143 halotools-0.8.2/halotools/mock_observables/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5681 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/tests/cf_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    14145 2023-06-30 13:08:32.000000 halotools-0.8.2/halotools/mock_observables/tests/test_catalog_analysis_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5276 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/tests/test_mock_observables_helpers.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     1008 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/tests/test_mock_survey.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3038 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/tests/test_occupation_stats.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.725952 halotools-0.8.2/halotools/mock_observables/two_point_clustering/
+-rw-r--r--   0 aphearin   (501) staff       (20)     1055 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    12986 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/angular_tpcf.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3208 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/clustering_helpers.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    23103 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/marked_tpcf.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    17324 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/rp_pi_tpcf.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    20886 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/rp_pi_tpcf_jackknife.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    18908 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/s_mu_tpcf.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.727539 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2538 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/locate_external_unit_testing_data.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4088 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_angular_tpcf.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2231 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_clustering_helpers.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)    10223 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_marked_tpcf.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     4003 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_rp_pi_tpcf.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8912 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_rp_pi_tpcf_jackknife.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     2904 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_s_mu_tpcf.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    25238 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_tpcf.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1972 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_tpcf_estimators.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4369 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_tpcf_jackknife.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1510 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_tpcf_multipole.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     9821 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_tpcf_one_two_halo.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     4975 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_wp.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4221 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_wp_jackknife.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    19660 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tpcf.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5988 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tpcf_estimators.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    19869 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tpcf_jackknife.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2855 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tpcf_multipole.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    20404 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/tpcf_one_two_halo_decomp.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    10516 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/wp.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    19645 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/two_point_clustering/wp_jackknife.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.727737 halotools-0.8.2/halotools/mock_observables/velocity_decomposition/
+-rw-r--r--   0 aphearin   (501) staff       (20)       89 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/velocity_decomposition/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8429 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/velocity_decomposition/radial_velocity_decomposition.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.727920 halotools-0.8.2/halotools/mock_observables/velocity_decomposition/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/velocity_decomposition/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7169 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/velocity_decomposition/tests/test_radial_velocity.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.728214 halotools-0.8.2/halotools/mock_observables/void_statistics/
+-rw-r--r--   0 aphearin   (501) staff       (20)      229 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/void_statistics/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.728485 halotools-0.8.2/halotools/mock_observables/void_statistics/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/mock_observables/void_statistics/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6704 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/void_statistics/tests/test_underdensity_prob_func.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4375 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/void_statistics/tests/test_void_prob_func.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    10220 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/void_statistics/underdensity_prob_func.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9081 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/mock_observables/void_statistics/void_prob_func.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.729972 halotools-0.8.2/halotools/sim_manager/
+-rw-r--r--   0 aphearin   (501) staff       (20)     1068 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    27209 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/cached_halo_catalog.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    45654 2022-09-28 16:33:58.000000 halotools-0.8.2/halotools/sim_manager/download_manager.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    11257 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/fake_sim.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    15326 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/halo_table_cache.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    15142 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/halo_table_cache_log_entry.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    14017 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/ptcl_table_cache.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    12036 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/ptcl_table_cache_log_entry.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    36766 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/rockstar_hlist_reader.py
+-rw-r--r--   0 aphearin   (501) staff       (20)        8 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/sim_manager/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2193 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/sim_defaults.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6053 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/sim_manager/supported_sims.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    26344 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/sim_manager/tabular_ascii_reader.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.731444 halotools-0.8.2/halotools/sim_manager/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)      246 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/tests/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.731543 halotools-0.8.2/halotools/sim_manager/tests/data/
+-rw-r--r--   0 aphearin   (501) staff       (20)   299010 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/tests/data/dummy_halocat_0.07812.list
+-rw-r--r--   0 aphearin   (501) staff       (20)     1574 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/tests/helper_functions.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    21316 2023-06-30 17:38:52.000000 halotools-0.8.2/halotools/sim_manager/tests/test_cached_halo_catalog.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    20004 2023-06-30 17:38:52.000000 halotools-0.8.2/halotools/sim_manager/tests/test_download_manager.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2773 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/tests/test_fake_sim.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8454 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/tests/test_halo_table_cache.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    15559 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/tests/test_halo_table_cache_log_entry.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      983 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/tests/test_load_default_halocat.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9640 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/tests/test_ptcl_table_cache.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9557 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/tests/test_ptcl_table_cache_log_entry.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13793 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/tests/test_rockstar_hlist_reader.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3444 2023-06-30 17:38:52.000000 halotools-0.8.2/halotools/sim_manager/tests/test_supported_sims.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8947 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/tests/test_tabular_ascii_reader.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    19164 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/sim_manager/tests/test_user_supplied_halo_catalog.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    10670 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/tests/test_user_supplied_ptcl_catalog.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    19796 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/user_supplied_halo_catalog.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    13168 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/sim_manager/user_supplied_ptcl_catalog.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.732428 halotools-0.8.2/halotools/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)      121 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      768 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/tests/coveragerc
+-rw-r--r--   0 aphearin   (501) staff       (20)       57 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/tests/ddc.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.732737 halotools-0.8.2/halotools/tests/docs_code_block_tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)      256 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/tests/docs_code_block_tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    17744 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/tests/docs_code_block_tests/test_hod_model_factory_tutorial.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2093 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/tests/docs_code_block_tests/test_preloaded_mockpop.py
+-rw-r--r--   0 aphearin   (501) staff       (20)        8 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/tests/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2499 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/tests/test_amurrica.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2172 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/tests/test_seed.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      336 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/tests/test_subpkg_imports.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      243 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/tests/usa.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.734538 halotools-0.8.2/halotools/utils/
+-rw-r--r--   0 aphearin   (501) staff       (20)      692 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/utils/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    14043 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/array_indexing_manipulations.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5919 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/array_utils.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5606 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/conditional_percentile.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     8476 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/utils/crossmatch.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5671 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/distribution_matching.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.734830 halotools-0.8.2/halotools/utils/engines/
+-rw-r--r--   0 aphearin   (501) staff       (20)       68 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/engines/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3989 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/engines/conditional_rank_kernel.pyx
+-rw-r--r--   0 aphearin   (501) staff       (20)      905 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/utils/engines/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7275 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/group_member_generator.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9346 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/inverse_transformation_sampling.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1693 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/utils/io_utils.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1582 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/load_umachine_binaries.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4642 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/utils/mcrotations.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5420 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/probabilistic_binning.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      394 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/python_string_comparisons.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4895 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/utils/rotations2d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9228 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/utils/rotations3d.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2679 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/spherical_geometry.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    15237 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/table_utils.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.736936 halotools-0.8.2/halotools/utils/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)      334 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/__init__.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.737048 halotools-0.8.2/halotools/utils/tests/data/
+-rw-r--r--   0 aphearin   (501) staff       (20)       55 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/data/dummy_ascii.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)        8 2022-09-25 14:53:47.000000 halotools-0.8.2/halotools/utils/tests/setup_package.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2133 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/utils/tests/test_2d_rotations.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3986 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/utils/tests/test_3d_rotations.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    14233 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/test_array_indexing_manipulations.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1969 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/test_array_utils.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1680 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/test_compute_richness.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4997 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/test_conditional_percentile.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3786 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/test_crossmatch.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2385 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/test_distribution_matching.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7617 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/test_group_member_generator.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      238 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/test_io_utils.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3423 2020-12-11 16:11:40.000000 halotools-0.8.2/halotools/utils/tests/test_its.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1066 2020-10-22 19:43:27.000000 halotools-0.8.2/halotools/utils/tests/test_mcrotations.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3024 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/test_probabilistic_binning.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      233 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/test_python_string_comparisons.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1068 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/utils/tests/test_rotate_vector_collection.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6447 2020-08-05 18:14:21.000000 halotools-0.8.2/halotools/utils/tests/test_table_utils.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4727 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/utils/tests/test_value_added_halo_table_functions.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4504 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/utils/tests/test_vector_utilities.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     7248 2022-10-21 16:05:22.000000 halotools-0.8.2/halotools/utils/value_added_halo_table_functions.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     9573 2022-09-23 19:40:55.000000 halotools-0.8.2/halotools/utils/vector_utilities.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      337 2023-06-30 17:51:15.000000 halotools-0.8.2/halotools/version.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.684621 halotools-0.8.2/halotools.egg-info/
+-rw-r--r--   0 aphearin   (501) staff       (20)     9824 2023-06-30 17:51:15.000000 halotools-0.8.2/halotools.egg-info/PKG-INFO
+-rw-r--r--   0 aphearin   (501) staff       (20)    51005 2023-06-30 17:51:15.000000 halotools-0.8.2/halotools.egg-info/SOURCES.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)        1 2023-06-30 17:51:15.000000 halotools-0.8.2/halotools.egg-info/dependency_links.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)       82 2023-06-30 17:51:15.000000 halotools-0.8.2/halotools.egg-info/entry_points.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)        1 2023-06-30 16:52:13.000000 halotools-0.8.2/halotools.egg-info/not-zip-safe
+-rw-r--r--   0 aphearin   (501) staff       (20)      114 2023-06-30 17:51:15.000000 halotools-0.8.2/halotools.egg-info/requires.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)       10 2023-06-30 17:51:15.000000 halotools-0.8.2/halotools.egg-info/top_level.txt
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.737256 halotools-0.8.2/licenses/
+-rw-r--r--   0 aphearin   (501) staff       (20)     1780 2022-09-23 19:40:55.000000 halotools-0.8.2/licenses/LICENSE.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)       87 2020-08-05 18:14:21.000000 halotools-0.8.2/licenses/README.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      244 2022-09-25 18:24:15.000000 halotools-0.8.2/pyproject.toml
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-06-30 17:51:15.737836 halotools-0.8.2/scripts/
+-rw-r--r--   0 aphearin   (501) staff       (20)       87 2020-08-05 18:14:21.000000 halotools-0.8.2/scripts/README.rst
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     7286 2020-10-22 19:43:27.000000 halotools-0.8.2/scripts/convert_documentation_tutorials.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     8172 2022-09-28 12:20:27.000000 halotools-0.8.2/scripts/download_additional_halocat.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     5317 2020-08-05 18:14:21.000000 halotools-0.8.2/scripts/download_initial_halocat.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     8840 2022-09-28 12:20:27.000000 halotools-0.8.2/scripts/rebuild_halo_table_cache_log.py
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     7469 2022-09-28 12:20:27.000000 halotools-0.8.2/scripts/rebuild_ptcl_table_cache_log.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1749 2023-06-30 17:51:15.738446 halotools-0.8.2/setup.cfg
+-rwxr-xr-x   0 aphearin   (501) staff       (20)     2264 2022-09-28 12:20:27.000000 halotools-0.8.2/setup.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2372 2023-06-14 13:29:05.000000 halotools-0.8.2/tox.ini
```

### Comparing `halotools-0.8.1/.github/workflows/ci_tests.yml` & `halotools-0.8.2/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/.github/workflows/wheels.yml` & `halotools-0.8.2/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/.gitignore` & `halotools-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/CHANGES.rst` & `halotools-0.8.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+0.8.2 (2023-06-30)
+------------------
+
+- Add non-Poissonian occupation statistics for satellites (https://github.com/astropy/halotools/pull/1053)
+
+- Fix bug in little h convention in Leauthaud+11 HOD model (https://github.com/astropy/halotools/pull/1063)
+
+- Fix bug in PBC handling of return_xyz_formatted_array convenience function (https://github.com/astropy/halotools/pull/1066)
+
+
 0.8.1 (2022-09-28)
 ------------------
 
 - Include command-line scripts for halo catalog downloads that were omitted from v0.8 release
 
 
 0.8 (2022-09-25)
```

### Comparing `halotools-0.8.1/PKG-INFO` & `halotools-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halotools
-Version: 0.8.1
+Version: 0.8.2
 Summary: Package designed to analyze N-body simulations and constrain models of cosmology and galaxy evolution.
 Home-page: http://astropy.org
 Author: Andrew Hearin
 Author-email: ahearin@anl.gov
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
@@ -161,8 +161,9 @@
            adsurl = {https://ui.adsabs.harvard.edu/abs/2017AJ....154..190H},
           adsnote = {Provided by the SAO/NASA Astrophysics Data System}
     }
 
 License
 -------
 
-Halotools is licensed under a 3-clause BSD style license - see the licenses/LICENSE.rst file.
+Halotools is licensed by Argonne National Lab under a 3-clause BSD style license - see the licenses/LICENSE.rst file.
+
```

### Comparing `halotools-0.8.1/README.rst` & `halotools-0.8.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -146,8 +146,9 @@
            adsurl = {https://ui.adsabs.harvard.edu/abs/2017AJ....154..190H},
           adsnote = {Provided by the SAO/NASA Astrophysics Data System}
     }
 
 License
 -------
 
-Halotools is licensed under a 3-clause BSD style license - see the licenses/LICENSE.rst file.
+Halotools is licensed by Argonne National Lab under a 3-clause BSD style license - see the licenses/LICENSE.rst file.
+
```

### Comparing `halotools-0.8.1/docs/Makefile` & `halotools-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/bijective_distribution_matching_demo.png` & `halotools-0.8.2/docs/_static/bijective_distribution_matching_demo.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/cam_example_assembias_clf.png` & `halotools-0.8.2/docs/_static/cam_example_assembias_clf.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/cam_example_bulge_disk_ratio.png` & `halotools-0.8.2/docs/_static/cam_example_bulge_disk_ratio.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/cam_example_complex_sfr.png` & `halotools-0.8.2/docs/_static/cam_example_complex_sfr.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/cam_example_complex_sfr_dmdt_correlation.png` & `halotools-0.8.2/docs/_static/cam_example_complex_sfr_dmdt_correlation.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/cam_example_complex_sfr_recovery.png` & `halotools-0.8.2/docs/_static/cam_example_complex_sfr_recovery.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/color_correlation_pdf.png` & `halotools-0.8.2/docs/_static/color_correlation_pdf.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/dm-splatting-large.png` & `halotools-0.8.2/docs/_static/dm-splatting-large.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/fuzzy_binning_example.png` & `halotools-0.8.2/docs/_static/fuzzy_binning_example.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/matched_distributions.png` & `halotools-0.8.2/docs/_static/matched_distributions.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/monte_carlo_example.png` & `halotools-0.8.2/docs/_static/monte_carlo_example.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/monte_carlo_example2.png` & `halotools-0.8.2/docs/_static/monte_carlo_example2.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/noisy_percentile_demo.png` & `halotools-0.8.2/docs/_static/noisy_percentile_demo.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/quenching_gradient_model_clustering.png` & `halotools-0.8.2/docs/_static/quenching_gradient_model_clustering.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/quenching_gradient_models.png` & `halotools-0.8.2/docs/_static/quenching_gradient_models.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/_static/spin_percentile.png` & `halotools-0.8.2/docs/_static/spin_percentile.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/conf.py` & `halotools-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/full_ref_api/halotools_full_api.rst` & `halotools-0.8.2/docs/full_ref_api/halotools_full_api.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/function_usage/hod_occupation_functions.rst` & `halotools-0.8.2/docs/function_usage/hod_occupation_functions.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/function_usage/index.rst` & `halotools-0.8.2/docs/function_usage/index.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/function_usage/mock_observables_functions.rst` & `halotools-0.8.2/docs/function_usage/mock_observables_functions.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/function_usage/phase_space_models_functions.rst` & `halotools-0.8.2/docs/function_usage/phase_space_models_functions.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/function_usage/utility_functions.rst` & `halotools-0.8.2/docs/function_usage/utility_functions.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/index.rst` & `halotools-0.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/install.rst` & `halotools-0.8.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/installation_troubleshooting.rst` & `halotools-0.8.2/docs/installation_troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/installing_halotools_with_virtualenv.rst` & `halotools-0.8.2/docs/installing_halotools_with_virtualenv.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/make.bat` & `halotools-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/cam_modeling/cam_complex_sfr_tutorial.ipynb` & `halotools-0.8.2/docs/notebooks/cam_modeling/cam_complex_sfr_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/cam_modeling/cam_decorated_clf.ipynb` & `halotools-0.8.2/docs/notebooks/cam_modeling/cam_decorated_clf.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/cam_modeling/cam_disk_bulge_ratios_demo.ipynb` & `halotools-0.8.2/docs/notebooks/cam_modeling/cam_disk_bulge_ratios_demo.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial` & `halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial1.ipynb` & `halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial1.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial10.ipynb` & `halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial10.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial2.ipynb` & `halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial2.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial3.ipynb` & `halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial3.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial4.ipynb` & `halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial4.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial5.ipynb` & `halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial5.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial6.ipynb` & `halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial6.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial7.ipynb` & `halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial7.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial8.ipynb` & `halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial8.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial9.ipynb` & `halotools-0.8.2/docs/notebooks/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial9.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/intermediate_examples/galaxy_catalog_intermediate_analysis_tutorial1.ipynb` & `halotools-0.8.2/docs/notebooks/galcat_analysis/intermediate_examples/galaxy_catalog_intermediate_analysis_tutorial1.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/galcat_analysis/intermediate_examples/quenching_gradient_tutorial.ipynb` & `halotools-0.8.2/docs/notebooks/galcat_analysis/intermediate_examples/quenching_gradient_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial1.ipynb` & `halotools-0.8.2/docs/notebooks/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial1.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial2.ipynb` & `halotools-0.8.2/docs/notebooks/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial2.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/hod_modeling/hod_modeling_tutorial1.ipynb` & `halotools-0.8.2/docs/notebooks/hod_modeling/hod_modeling_tutorial1.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/hod_modeling/hod_modeling_tutorial2.ipynb` & `halotools-0.8.2/docs/notebooks/hod_modeling/hod_modeling_tutorial2.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/hod_modeling/hod_modeling_tutorial3.ipynb` & `halotools-0.8.2/docs/notebooks/hod_modeling/hod_modeling_tutorial3.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/hod_modeling/hod_modeling_tutorial4.ipynb` & `halotools-0.8.2/docs/notebooks/hod_modeling/hod_modeling_tutorial4.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/hod_modeling/hod_modeling_tutorial5.ipynb` & `halotools-0.8.2/docs/notebooks/hod_modeling/hod_modeling_tutorial5.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial1.ipynb` & `halotools-0.8.2/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial1.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial2.ipynb` & `halotools-0.8.2/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial2.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial3.ipynb` & `halotools-0.8.2/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial3.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial4.ipynb` & `halotools-0.8.2/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial4.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial5.ipynb` & `halotools-0.8.2/docs/notebooks/subhalo_modeling/subhalo_modeling_tutorial5.ipynb`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/overview.rst` & `halotools-0.8.2/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/development/citing_halotools.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/development/citing_halotools.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/development/contributors.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/development/contributors.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/getting_started_overview.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/getting_started_overview.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/index.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/managing_catalogs/supported_sim_list.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/managing_catalogs/supported_sim_list.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/mock_observations/calculating_counts_in_cells.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/mock_observations/calculating_counts_in_cells.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/mock_observations/mock_obs_pos_formatting.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/mock_observations/mock_obs_pos_formatting.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/quickstart_guides/halo_catalog_analysis_quickstart.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/quickstart_guides/halo_catalog_analysis_quickstart.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/quickstart_guides/working_with_alternative_catalogs.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/quickstart_guides/working_with_alternative_catalogs.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/quickstart_guides/working_with_halotools_provided_catalogs.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/quickstart_guides/working_with_halotools_provided_catalogs.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/angular_crosscorr.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/angular_crosscorr.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial2.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial2.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial3.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial3.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial4.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial4.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial9.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/galaxy_catalog_analysis_tutorial9.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/gg_lensing_tutorial3.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/gg_lensing_tutorial3.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/mock_fullsky.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/mock_fullsky.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/mock_octant.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/mock_octant.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/one_two_halo_clustering.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/one_two_halo_clustering.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/output_9_1.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/output_9_1.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/random_vs_analytic.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/random_vs_analytic.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/wp_red_blue_cross.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/wp_red_blue_cross.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/wp_tutorial4.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/wp_tutorial4.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/wtheta1.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/clustering_examples/wtheta1.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/crossmatching_galaxy_catalogs.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/crossmatching_galaxy_catalogs.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial1.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/galaxy_catalog_analysis_tutorial1.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/group_identification/galaxy_catalog_analysis_tutorial5.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/group_identification/galaxy_catalog_analysis_tutorial5.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/group_identification/group_richness_vs_group_cenmass.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/group_identification/group_richness_vs_group_cenmass.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/isolation_criteria/galaxy_catalog_analysis_tutorial10.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/isolation_criteria/galaxy_catalog_analysis_tutorial10.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/output_18_1.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/output_18_1.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/output_23_1.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/output_23_1.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/cluster_bcg_infall_velocity.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/cluster_bcg_infall_velocity.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/cluster_dispersion_profile.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/cluster_dispersion_profile.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/galaxy_catalog_analysis_tutorial6.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/galaxy_catalog_analysis_tutorial6.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/galaxy_catalog_analysis_tutorial7.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/velocity_statistics/galaxy_catalog_analysis_tutorial7.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/void_stats/galaxy_catalog_analysis_tutorial8.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/void_stats/galaxy_catalog_analysis_tutorial8.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/void_stats/vpf_upf_tutorial.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/basic_examples/void_stats/vpf_upf_tutorial.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/index.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/index.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/intermediate_examples/isolation_criteria/galaxy_catalog_intermediate_analysis_tutorial1.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/galcat_analysis/intermediate_examples/isolation_criteria/galaxy_catalog_intermediate_analysis_tutorial1.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/figs/radial_profile_halocat_tutorial_fig1.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/figs/radial_profile_halocat_tutorial_fig1.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/figs/radial_profile_halocat_tutorial_fig2.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/figs/radial_profile_halocat_tutorial_fig2.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial1.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial1.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial2.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/halo_catalog_analysis_tutorial2.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/nsub_vs_hostmass.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/basic_examples/nsub_vs_hostmass.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/crossmatching_halo_catalogs.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/crossmatching_halo_catalogs.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/index.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/index.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/rockstar_subhalo_nomenclature.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/rockstar_subhalo_nomenclature.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/subhalo_membership.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/catalog_analysis/halocat_analysis/subhalo_membership.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/merger_tree_analysis_example.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/merger_tree_analysis_example.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/altering_param_dict.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/altering_param_dict.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_complex_sfr.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_complex_sfr.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_decorated_clf.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_decorated_clf.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_disk_bulge_ratios.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_disk_bulge_ratios.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_quenching_gradients.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_quenching_gradients.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_tutorial.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/cam_tutorial_pages/cam_tutorial.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial0.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial0.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial1.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial1.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial2.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial2.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial3.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial3.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial4.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial4.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial5.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/hod_modeling_tutorial5.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/writing_your_own_hod_occupation_component.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/writing_your_own_hod_occupation_component.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/zheng07_using_cenocc_model_tutorial.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/hod_modeling/zheng07_using_cenocc_model_tutorial.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/index.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/index.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial0.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial0.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial1.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial1.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial2.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial2.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial3.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial3.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial4.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial4.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial5.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/composing_models/subhalo_modeling/subhalo_modeling_tutorial5.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/halotools_design.png` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/halotools_design.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/index.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/index.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/behroozi10_composite_model.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/behroozi10_composite_model.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/cacciato09_composite_model.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/cacciato09_composite_model.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/hearin15_composite_model.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/hearin15_composite_model.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/index.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/index.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/leauthaud11_composite_model.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/leauthaud11_composite_model.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/preloaded_models_list.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/preloaded_models_list.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/tinker13_composite_model.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/tinker13_composite_model.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/zheng07_composite_model.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/zheng07_composite_model.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/zu_mandelbaum15_composite_model.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/zu_mandelbaum15_composite_model.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/zu_mandelbaum16_composite_model.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/model_building/preloaded_models/zu_mandelbaum16_composite_model.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/reducing_and_caching_a_new_rockstar_catalog.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/reducing_and_caching_a_new_rockstar_catalog.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/user_supplied_halo_catalogs.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/user_supplied_halo_catalogs.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/quickstart_and_tutorials/tutorials/working_with_alternative_particle_data.rst` & `halotools-0.8.2/docs/quickstart_and_tutorials/tutorials/working_with_alternative_particle_data.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/convert_tutorials.py` & `halotools-0.8.2/docs/source_notes/convert_tutorials.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/empirical_models/factories/hod_mock_factory_source_notes.rst` & `halotools-0.8.2/docs/source_notes/empirical_models/factories/hod_mock_factory_source_notes.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/empirical_models/factories/hod_model_factory_source_notes.rst` & `halotools-0.8.2/docs/source_notes/empirical_models/factories/hod_model_factory_source_notes.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/empirical_models/factories/index.rst` & `halotools-0.8.2/docs/source_notes/empirical_models/factories/index.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/empirical_models/factories/model_factory_composite_sequence_mechanisms.rst` & `halotools-0.8.2/docs/source_notes/empirical_models/factories/model_factory_composite_sequence_mechanisms.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/empirical_models/factories/np_repeat_tutorial.png` & `halotools-0.8.2/docs/source_notes/empirical_models/factories/np_repeat_tutorial.png`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/empirical_models/factories/subhalo_mock_factory_source_notes.rst` & `halotools-0.8.2/docs/source_notes/empirical_models/factories/subhalo_mock_factory_source_notes.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/empirical_models/factories/subhalo_model_factory_source_notes.rst` & `halotools-0.8.2/docs/source_notes/empirical_models/factories/subhalo_model_factory_source_notes.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/empirical_models/phase_space_models/jeans_equation_derivations.rst` & `halotools-0.8.2/docs/source_notes/empirical_models/phase_space_models/jeans_equation_derivations.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/empirical_models/phase_space_models/monte_carlo_galprof_source_notes.rst` & `halotools-0.8.2/docs/source_notes/empirical_models/phase_space_models/monte_carlo_galprof_source_notes.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/empirical_models/phase_space_models/nfw_profile_source_notes.rst` & `halotools-0.8.2/docs/source_notes/empirical_models/phase_space_models/nfw_profile_source_notes.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/empirical_models/phase_space_models/profile_template_source_notes.rst` & `halotools-0.8.2/docs/source_notes/empirical_models/phase_space_models/profile_template_source_notes.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/index.rst` & `halotools-0.8.2/docs/source_notes/index.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/source_notes/mock_observables/zspace_distortions.rst` & `halotools-0.8.2/docs/source_notes/mock_observables/zspace_distortions.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/usage_tutorials/cache_management/relocating_simulation_data.rst` & `halotools-0.8.2/docs/usage_tutorials/cache_management/relocating_simulation_data.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/usage_tutorials/empirical_models/assembias_models/heaviside_assembias_tutorial.rst` & `halotools-0.8.2/docs/usage_tutorials/empirical_models/assembias_models/heaviside_assembias_tutorial.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/usage_tutorials/empirical_models/subhalo_phase_space/subhalo_phase_space_tutorial.rst` & `halotools-0.8.2/docs/usage_tutorials/empirical_models/subhalo_phase_space/subhalo_phase_space_tutorial.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/whats_new_history/whats_new_0.5.rst` & `halotools-0.8.2/docs/whats_new_history/whats_new_0.5.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/whats_new_history/whats_new_0.6.rst` & `halotools-0.8.2/docs/whats_new_history/whats_new_0.6.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/docs/whats_new_history/whats_new_0.7.rst` & `halotools-0.8.2/docs/whats_new_history/whats_new_0.7.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/_compiler.c` & `halotools-0.8.2/halotools/_compiler.c`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/conftest.py` & `halotools-0.8.2/halotools/conftest.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/custom_exceptions.py` & `halotools-0.8.2/halotools/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/abunmatch/bin_free_cam.py` & `halotools-0.8.2/halotools/empirical_models/abunmatch/bin_free_cam.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/abunmatch/conditional_abunmatch_bin_based.py` & `halotools-0.8.2/halotools/empirical_models/abunmatch/conditional_abunmatch_bin_based.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/abunmatch/engines/bin_free_cam_kernel.pyx` & `halotools-0.8.2/halotools/empirical_models/abunmatch/engines/bin_free_cam_kernel.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/abunmatch/engines/setup_package.py` & `halotools-0.8.2/halotools/empirical_models/abunmatch/engines/setup_package.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/abunmatch/noisy_percentile.py` & `halotools-0.8.2/halotools/empirical_models/abunmatch/noisy_percentile.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/abunmatch/tests/naive_python_cam.py` & `halotools-0.8.2/halotools/empirical_models/abunmatch/tests/naive_python_cam.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/abunmatch/tests/test_bin_free_cam.py` & `halotools-0.8.2/halotools/empirical_models/abunmatch/tests/test_bin_free_cam.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/abunmatch/tests/test_conditional_abunmatch.py` & `halotools-0.8.2/halotools/empirical_models/abunmatch/tests/test_conditional_abunmatch.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/abunmatch/tests/test_noisy_percentile.py` & `halotools-0.8.2/halotools/empirical_models/abunmatch/tests/test_noisy_percentile.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/abunmatch/tests/test_pure_python.py` & `halotools-0.8.2/halotools/empirical_models/abunmatch/tests/test_pure_python.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/abunmatch/tests/test_sample2_window_function.py` & `halotools-0.8.2/halotools/empirical_models/abunmatch/tests/test_sample2_window_function.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/assembias_models/heaviside_assembias.py` & `halotools-0.8.2/halotools/empirical_models/assembias_models/heaviside_assembias.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/assembias_models/tests/test_assembias.py` & `halotools-0.8.2/halotools/empirical_models/assembias_models/tests/test_assembias.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/component_model_templates/binary_galprop_models.py` & `halotools-0.8.2/halotools/empirical_models/component_model_templates/binary_galprop_models.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/component_model_templates/prim_galprop_model.py` & `halotools-0.8.2/halotools/empirical_models/component_model_templates/prim_galprop_model.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/component_model_templates/scatter_models.py` & `halotools-0.8.2/halotools/empirical_models/component_model_templates/scatter_models.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/component_model_templates/tests/test_binary_galprop_models.py` & `halotools-0.8.2/halotools/empirical_models/component_model_templates/tests/test_binary_galprop_models.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/component_model_templates/tests/test_prim_galprop_model.py` & `halotools-0.8.2/halotools/empirical_models/component_model_templates/tests/test_prim_galprop_model.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/component_model_templates/tests/test_scatter_models.py` & `halotools-0.8.2/halotools/empirical_models/component_model_templates/tests/test_scatter_models.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/cacciato09.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/cacciato09.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/hearin15.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/hearin15.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/leauthaud11.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/leauthaud11.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/tests/test_tinker13.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/tests/test_tinker13.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/tests/test_zheng07.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/tests/test_zheng07.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/tests/test_zu_mandelbaum16.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/tests/test_zu_mandelbaum16.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/tinker13.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/tinker13.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/zheng07.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/zheng07.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/zu_mandelbaum15.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/zu_mandelbaum15.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/hod_models/zu_mandelbaum16.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/hod_models/zu_mandelbaum16.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/sfr_models/smhm_binary_sfr.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/sfr_models/smhm_binary_sfr.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/smhm_models/behroozi10.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/smhm_models/behroozi10.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/composite_models/tests/test_preloaded_models.py` & `halotools-0.8.2/halotools/empirical_models/composite_models/tests/test_preloaded_models.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/hod_mock_factory.py` & `halotools-0.8.2/halotools/empirical_models/factories/hod_mock_factory.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/hod_model_factory.py` & `halotools-0.8.2/halotools/empirical_models/factories/hod_model_factory.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/mock_factory_template.py` & `halotools-0.8.2/halotools/empirical_models/factories/mock_factory_template.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/mock_helpers.py` & `halotools-0.8.2/halotools/empirical_models/factories/mock_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/model_factory_template.py` & `halotools-0.8.2/halotools/empirical_models/factories/model_factory_template.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/prebuilt_model_factory.py` & `halotools-0.8.2/halotools/empirical_models/factories/prebuilt_model_factory.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/subhalo_mock_factory.py` & `halotools-0.8.2/halotools/empirical_models/factories/subhalo_mock_factory.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/subhalo_model_factory.py` & `halotools-0.8.2/halotools/empirical_models/factories/subhalo_model_factory.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/tests/test_clf_support.py` & `halotools-0.8.2/halotools/empirical_models/factories/tests/test_clf_support.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/tests/test_hod_factory.py` & `halotools-0.8.2/halotools/empirical_models/factories/tests/test_hod_factory.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/tests/test_hod_mock_factory.py` & `halotools-0.8.2/halotools/empirical_models/factories/tests/test_hod_mock_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 """
 from __future__ import absolute_import, division, print_function
+
+from copy import deepcopy
+
+import numpy as np
 import pytest
 from astropy.config.paths import _find_home
-import numpy as np
-from copy import deepcopy
 
+from ....custom_exceptions import HalotoolsError
+from ....empirical_models import (
+    AssembiasZheng07Cens,
+    AssembiasZheng07Sats,
+    HodModelFactory,
+    NFWPhaseSpace,
+    TrivialPhaseSpace,
+)
 from ....mock_observables import return_xyz_formatted_array, tpcf_one_two_halo_decomp
-
-
-from ....empirical_models import AssembiasZheng07Cens
-from ....empirical_models import TrivialPhaseSpace
-from ....empirical_models import AssembiasZheng07Sats
-from ....empirical_models import NFWPhaseSpace
-from ....empirical_models import HodModelFactory
-
-from ....sim_manager import FakeSim, CachedHaloCatalog
+from ....sim_manager import CachedHaloCatalog, FakeSim
 from ....sim_manager.fake_sim import FakeSimHalosNearBoundaries
 from ..prebuilt_model_factory import PrebuiltHodModelFactory
-from ....custom_exceptions import HalotoolsError
 
 # Determine whether the machine is mine
 # This will be used to select tests whose
 # returned values depend on the configuration
 # of my personal cache directory files
 aph_home = "/Users/aphearin"
 detected_home = _find_home()
@@ -50,15 +51,14 @@
     assert estimated_ngals2 == estimated_ngals
 
     estimated_ngals3 = model.mock.estimate_ngals(seed=fixed_seed + 1)
     assert estimated_ngals3 != estimated_ngals
 
 
 def test_estimate_ngals2():
-
     model = PrebuiltHodModelFactory("tinker13")
     halocat = FakeSim(seed=fixed_seed)
     model.populate_mock(halocat, seed=fixed_seed)
 
     estimated_ngals = model.mock.estimate_ngals(seed=fixed_seed)
     actual_ngals = len(model.mock.galaxy_table)
     assert np.allclose(estimated_ngals, actual_ngals, rtol=0.01)
@@ -231,24 +231,22 @@
         try:
             assert np.allclose(h1[key], h2[key], rtol=0.001)
         except TypeError:
             pass
 
 
 def test_zero_satellite_edge_case():
-
     model = PrebuiltHodModelFactory("zheng07", threshold=-18)
     model.param_dict["logM0"] = 20
 
     halocat = FakeSim()
     model.populate_mock(halocat=halocat)
 
 
 def test_zero_halo_edge_case():
-
     model = PrebuiltHodModelFactory("zheng07", threshold=-18)
     model.param_dict["logM0"] = 20
 
     halocat = FakeSim()
     with pytest.raises(HalotoolsError) as err:
         model.populate_mock(halocat=halocat, Num_ptcl_requirement=1e10)
     substr = "Such a cut is not permissible."
```

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/tests/test_hod_model_factory.py` & `halotools-0.8.2/halotools/empirical_models/factories/tests/test_hod_model_factory.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/tests/test_mock_helpers.py` & `halotools-0.8.2/halotools/empirical_models/factories/tests/test_mock_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/tests/test_prebuilt_hod_model_factory.py` & `halotools-0.8.2/halotools/empirical_models/factories/tests/test_prebuilt_hod_model_factory.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/tests/test_prebuilt_subhalo_model_factory.py` & `halotools-0.8.2/halotools/empirical_models/factories/tests/test_prebuilt_subhalo_model_factory.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/factories/tests/test_subhalo_model_factory.py` & `halotools-0.8.2/halotools/empirical_models/factories/tests/test_subhalo_model_factory.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/model_defaults.py` & `halotools-0.8.2/halotools/empirical_models/model_defaults.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/model_helpers.py` & `halotools-0.8.2/halotools/empirical_models/model_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/cacciato09_components.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/cacciato09_components.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,29 +10,34 @@
 from .occupation_model_template import OccupationComponent
 from .engines import cacciato09_sats_mc_prim_galprop_engine
 
 from .. import custom_incomplete_gamma
 
 from ...custom_exceptions import HalotoolsError
 
-__all__ = ('Cacciato09Cens', 'Cacciato09Sats')
+__all__ = ("Cacciato09Cens", "Cacciato09Sats")
 
 
 class Cacciato09Cens(OccupationComponent):
-    r""" CLF-style model for the central galaxy occupation. Since it is a CLF
+    r"""CLF-style model for the central galaxy occupation. Since it is a CLF
     model, it also assigns a primary galaxy property to galaxies in addition to
     effectively being an HOD model. The primary galaxy property can for example
     be luminosity or stellar mass.
 
     See :ref:`cacciato09_composite_model` for a tutorial on this model.
 
     """
 
-    def __init__(self, threshold=10.0, prim_haloprop_key='halo_m180b',
-                 prim_galprop_key='luminosity', **kwargs):
+    def __init__(
+        self,
+        threshold=10.0,
+        prim_haloprop_key="halo_m180b",
+        prim_galprop_key="luminosity",
+        **kwargs
+    ):
         r"""
         Parameters
         ----------
         threshold : float, optional
             Logarithm of the primary galaxy property threshold. If the primary
             galaxy property is luminosity, it is given in h=1 solar luminosity
             units.
@@ -50,47 +55,52 @@
         >>> cen_model = Cacciato09Cens()
         >>> cen_model = Cacciato09Cens(threshold = 11.25)
         >>> cen_model = Cacciato09Cens(prim_haloprop_key = 'halo_mvir')
 
         """
 
         super(Cacciato09Cens, self).__init__(
-            gal_type='centrals', threshold=threshold,
+            gal_type="centrals",
+            threshold=threshold,
             upper_occupation_bound=1.0,
             prim_haloprop_key=prim_haloprop_key,
-            **kwargs)
+            **kwargs
+        )
 
-        self._mock_generation_calling_sequence = ['mc_occupation',
-                                                  'mc_prim_galprop']
+        self._mock_generation_calling_sequence = ["mc_occupation", "mc_prim_galprop"]
         self.prim_galprop_key = prim_galprop_key
-        self._galprop_dtypes_to_allocate = np.dtype([(prim_galprop_key, 'f8')])
+        self._galprop_dtypes_to_allocate = np.dtype([(prim_galprop_key, "f8")])
         self.param_dict = self.get_published_parameters()
-        self._methods_to_inherit = (['mc_occupation', 'median_prim_galprop',
-                                     'mean_occupation', 'mc_prim_galprop',
-                                     'clf'])
-        self.publications = ['arXiv:0807.4932']
+        self._methods_to_inherit = [
+            "mc_occupation",
+            "median_prim_galprop",
+            "mean_occupation",
+            "mc_prim_galprop",
+            "clf",
+        ]
+        self.publications = ["arXiv:0807.4932"]
 
     def get_published_parameters(self):
-        r""" Return the values of ``self.param_dict`` according to
+        r"""Return the values of ``self.param_dict`` according to
         the best-fit values of the WMAP3 model in Table 3 of arXiv:0807.4932.
         In this analysis, halo masses have been defined using an overdensity of
         180 times the background density of the Universe.
         """
-        param_dict = (
-            {'log_L_0': 9.935,
-             'log_M_1': 11.07,
-             'gamma_1': 3.273,
-             'gamma_2': 0.255,
-             'sigma': 0.143}
-            )
+        param_dict = {
+            "log_L_0": 9.935,
+            "log_M_1": 11.07,
+            "gamma_1": 3.273,
+            "gamma_2": 0.255,
+            "sigma": 0.143,
+        }
 
         return param_dict
 
     def median_prim_galprop(self, **kwargs):
-        r""" Return the median primary galaxy property of a central galaxy as a
+        r"""Return the median primary galaxy property of a central galaxy as a
         function of the input table.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             Array of mass-like variable upon which the calculation is based.
             If ``prim_haloprop`` is not passed, then ``table`` keyword argument
@@ -105,35 +115,37 @@
         -------
         prim_galprop : array_like
             Array containing the median primary galaxy property of the halos
             specified.
         """
 
         # Retrieve the array storing the mass-like variable.
-        if 'table' in list(kwargs.keys()):
-            mass = kwargs['table'][self.prim_haloprop_key]
-        elif 'prim_haloprop' in list(kwargs.keys()):
-            mass = kwargs['prim_haloprop']
+        if "table" in list(kwargs.keys()):
+            mass = kwargs["table"][self.prim_haloprop_key]
+        elif "prim_haloprop" in list(kwargs.keys()):
+            mass = kwargs["prim_haloprop"]
         else:
-            msg = ("\nYou must pass either a ``table`` or ``prim_haloprop`` "
-                   "argument to the ``median_prim_galprop`` function of the "
-                   "``Cacciato09Cens`` class.\n")
+            msg = (
+                "\nYou must pass either a ``table`` or ``prim_haloprop`` "
+                "argument to the ``median_prim_galprop`` function of the "
+                "``Cacciato09Cens`` class.\n"
+            )
             raise HalotoolsError(msg)
 
-        gamma_1 = self.param_dict['gamma_1']
-        gamma_2 = self.param_dict['gamma_2']
-        mass_c = 10**self.param_dict['log_M_1']
-        prim_galprop_c = 10**self.param_dict['log_L_0']
+        gamma_1 = self.param_dict["gamma_1"]
+        gamma_2 = self.param_dict["gamma_2"]
+        mass_c = 10 ** self.param_dict["log_M_1"]
+        prim_galprop_c = 10 ** self.param_dict["log_L_0"]
 
         r = mass / mass_c
 
-        return prim_galprop_c * (r / (1 + r))**gamma_1 * (1 + r)**gamma_2
+        return prim_galprop_c * (r / (1 + r)) ** gamma_1 * (1 + r) ** gamma_2
 
     def clf(self, prim_galprop=1e10, prim_haloprop=1e12):
-        r""" Return the CLF in units of dn/dlogL for the primary halo property
+        r"""Return the CLF in units of dn/dlogL for the primary halo property
         and galaxy property L.
 
         Parameters
         ----------
         prim_haloprop : array_like, optional
             Array of mass-like variable upon which the calculation is based.
 
@@ -151,85 +163,93 @@
             assumed throughout.
         """
 
         prim_galprop = np.atleast_1d(prim_galprop)
         prim_haloprop = np.atleast_1d(prim_haloprop)
 
         if (len(prim_haloprop) > 1) & (len(prim_galprop) > 1):
-            msg = ("If both ``prim_galprop`` and ``prim_haloprop`` are arrays"
-                   "with multiple elements, they must have the same length.\n")
+            msg = (
+                "If both ``prim_galprop`` and ``prim_haloprop`` are arrays"
+                "with multiple elements, they must have the same length.\n"
+            )
             assert len(prim_galprop) == len(prim_haloprop), msg
 
         med_prim_galprop = self.median_prim_galprop(prim_haloprop=prim_haloprop)
 
-        return ((1.0 / (np.sqrt(2.0 * np.pi) * self.param_dict['sigma'])) *
-                np.exp(-(np.log10(prim_galprop / med_prim_galprop))**2 / (2.0 *
-                       self.param_dict['sigma']**2)))
+        return (1.0 / (np.sqrt(2.0 * np.pi) * self.param_dict["sigma"])) * np.exp(
+            -((np.log10(prim_galprop / med_prim_galprop)) ** 2)
+            / (2.0 * self.param_dict["sigma"] ** 2)
+        )
 
     def mean_occupation(self, prim_galprop_min=None, prim_galprop_max=None, **kwargs):
-        r""" Expected number of central galaxies in a halo. Derived from
-        integrating the CLF from the primary galaxy property threshold to
-        infinity.
-
-        Parameters
-        ----------
-        prim_galprop_min : float, optional
-            Lower limit of the CLF integration used to calculate the expected
-            number of central galaxies. If not specified, the lower limit is the
-            threshold.
-       
-       prim_galprop_max : float, optional
-            Upper limit of the CLF integration used to calculate the expected
-            number of central galaxies. If not specified, the upper limit is
-            infinity.
-
-        prim_haloprop : array, optional
-            Array of mass-like variable upon which occupation statistics are
-            based.
-            If ``prim_haloprop`` is not passed, then ``table`` keyword argument
-            must be passed.
-
-        table : object, optional
-            Data table storing halo catalog.
-            If ``table`` is not passed, then ``prim_haloprop`` keyword argument
-            must be passed.
+        r"""Expected number of central galaxies in a halo. Derived from
+         integrating the CLF from the primary galaxy property threshold to
+         infinity.
+
+         Parameters
+         ----------
+         prim_galprop_min : float, optional
+             Lower limit of the CLF integration used to calculate the expected
+             number of central galaxies. If not specified, the lower limit is the
+             threshold.
 
-        Returns
-        -------
-        mean_ncen : array
-            Mean number of central galaxies in halos of the input mass.
+        prim_galprop_max : float, optional
+             Upper limit of the CLF integration used to calculate the expected
+             number of central galaxies. If not specified, the upper limit is
+             infinity.
+
+         prim_haloprop : array, optional
+             Array of mass-like variable upon which occupation statistics are
+             based.
+             If ``prim_haloprop`` is not passed, then ``table`` keyword argument
+             must be passed.
+
+         table : object, optional
+             Data table storing halo catalog.
+             If ``table`` is not passed, then ``prim_haloprop`` keyword argument
+             must be passed.
+
+         Returns
+         -------
+         mean_ncen : array
+             Mean number of central galaxies in halos of the input mass.
         """
 
         if prim_galprop_min is not None:
             prim_galprop_min = prim_galprop_min
         else:
             prim_galprop_min = 10**self.threshold
-        
+
         if prim_galprop_max is not None:
             if prim_galprop_max <= prim_galprop_min:
-                msg = ("\nFor the ``mean_occupation`` function of the "
-                       "``Cacciato09Cens`` class the ``prim_galprop_max`` "
-                       "keyword must be bigger than 10^threshold or "
-                       "``prim_galprop_min`` if provided.\n")
+                msg = (
+                    "\nFor the ``mean_occupation`` function of the "
+                    "``Cacciato09Cens`` class the ``prim_galprop_max`` "
+                    "keyword must be bigger than 10^threshold or "
+                    "``prim_galprop_min`` if provided.\n"
+                )
                 raise HalotoolsError(msg)
 
         log_prim_galprop = np.log10(self.median_prim_galprop(**kwargs))
-        
-        
-        result = (0.5 * erfc((np.log10(prim_galprop_min) - log_prim_galprop) /
-                           (np.sqrt(2.0) * self.param_dict['sigma'])))
-       
+
+        result = 0.5 * erfc(
+            (np.log10(prim_galprop_min) - log_prim_galprop)
+            / (np.sqrt(2.0) * self.param_dict["sigma"])
+        )
+
         if prim_galprop_max is not None:
-            result = (result - 0.5 * erfc((np.log10(prim_galprop_max) - log_prim_galprop) /
-                           (np.sqrt(2.0) * self.param_dict['sigma'])))
-  
+            result = result - 0.5 * erfc(
+                (np.log10(prim_galprop_max) - log_prim_galprop)
+                / (np.sqrt(2.0) * self.param_dict["sigma"])
+            )
+
         return result
 
     def mc_prim_galprop(self, **kwargs):
-        r""" Method to generate Monte Carlo realizations of the primary galaxy
+        r"""Method to generate Monte Carlo realizations of the primary galaxy
         property of galaxies under the constraint that the primary galaxy
         property is above the primary galaxy property threshold.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             Array of mass-like variable upon which the primary galaxy properties
@@ -251,35 +271,38 @@
         mc_prim_galprop : array
             Float array giving the Monte Carlo realization of primary galaxy
             properties of centrals in halos of the given mass. All primary
             galaxy properties returned are above the threshold.
         """
 
         # Retrieve the array storing the mass-like variable.
-        if 'table' in list(kwargs.keys()):
-            mass = kwargs['table'][self.prim_haloprop_key]
-        elif 'prim_haloprop' in list(kwargs.keys()):
-            mass = kwargs['prim_haloprop']
+        if "table" in list(kwargs.keys()):
+            mass = kwargs["table"][self.prim_haloprop_key]
+        elif "prim_haloprop" in list(kwargs.keys()):
+            mass = kwargs["prim_haloprop"]
         else:
-            msg = ("\nYou must pass either a ``table`` or ``prim_haloprop``"
-                   "argument to the ``mc_prim_galprop`` function of the "
-                   "``Cacciato09Cens`` class.\n")
+            msg = (
+                "\nYou must pass either a ``table`` or ``prim_haloprop``"
+                "argument to the ``mc_prim_galprop`` function of the "
+                "``Cacciato09Cens`` class.\n"
+            )
             raise HalotoolsError(msg)
 
         log_median_prim_galprop = np.log10(self.median_prim_galprop(**kwargs))
         mean_occupation = self.mean_occupation(**kwargs)
 
         if np.any(mean_occupation <= 0):
             msg = (
                 "\nOne of the input halos to the ``mc_prim_galprop``  function "
                 "of the ``Cacciato09Cens`` class has (virtually) no expected "
-                "galaxy.\n")
+                "galaxy.\n"
+            )
             raise HalotoolsError(msg)
 
-        seed = kwargs.get('seed', None)
+        seed = kwargs.get("seed", None)
 
         prim_galprop = np.zeros(len(mean_occupation))
 
         with NumpyRNGContext(seed):
 
             # Draw cumulative distribution function (CDF) values for the
             # primary galaxy properties in [0, 1).
@@ -290,39 +313,46 @@
             # for low expected occupations CDF ~ 1 which can lead to numerical
             # problems.
             cdf = mean_occupation * x + (1 - mean_occupation)
             cdfc = mean_occupation * (1 - x)  # 1 - cdf
 
             # Draw primary galaxy properties.
             mask = cdf <= 0.5
-            prim_galprop[mask] = 10**(-erfcinv(2 * cdf[mask]) *
-                                      np.sqrt(2 * self.param_dict['sigma']**2) +
-                                      log_median_prim_galprop[mask])
+            prim_galprop[mask] = 10 ** (
+                -erfcinv(2 * cdf[mask]) * np.sqrt(2 * self.param_dict["sigma"] ** 2)
+                + log_median_prim_galprop[mask]
+            )
             mask = np.logical_not(mask)  # cdf > 0.5
-            prim_galprop[mask] = 10**(erfcinv(2 * cdfc[mask]) *
-                                      np.sqrt(2 * self.param_dict['sigma']**2) +
-                                      log_median_prim_galprop[mask])
+            prim_galprop[mask] = 10 ** (
+                erfcinv(2 * cdfc[mask]) * np.sqrt(2 * self.param_dict["sigma"] ** 2)
+                + log_median_prim_galprop[mask]
+            )
 
-        if 'table' in list(kwargs.keys()):
-            kwargs['table'][self.prim_galprop_key][:] = prim_galprop
+        if "table" in list(kwargs.keys()):
+            kwargs["table"][self.prim_galprop_key][:] = prim_galprop
 
         return prim_galprop
 
 
 class Cacciato09Sats(OccupationComponent):
-    r""" CLF-style model for the satellite galaxy occupation. Since it is a CLF
+    r"""CLF-style model for the satellite galaxy occupation. Since it is a CLF
     model, it also assigns a primary galaxy property to galaxies in addition to
     effectively being an HOD model. The primary galaxy property can for example
     be luminosity or stellar mass.
 
     See :ref:`cacciato09_composite_model` for a tutorial on this model.
     """
 
-    def __init__(self, threshold=10.0, prim_haloprop_key='halo_m180b',
-                 prim_galprop_key='luminosity', **kwargs):
+    def __init__(
+        self,
+        threshold=10.0,
+        prim_haloprop_key="halo_m180b",
+        prim_galprop_key="luminosity",
+        **kwargs
+    ):
         r"""
         Parameters
         ----------
             Logarithm of the primary galaxy property threshold. If the primary
             galaxy property is luminosity, it is given in h=1 solar luminosity
             units.
 
@@ -338,68 +368,77 @@
         --------
         >>> sat_model = Cacciato09Sats()
         >>> sat_model = Cacciato09Sats(threshold = 11.25)
         >>> sat_model = Cacciato09Sats(prim_haloprop_key = 'halo_mvir')
 
         """
         super(Cacciato09Sats, self).__init__(
-            gal_type='satellites', threshold=threshold,
+            gal_type="satellites",
+            threshold=threshold,
             upper_occupation_bound=float("inf"),
             prim_haloprop_key=prim_haloprop_key,
-            **kwargs)
+            **kwargs
+        )
 
-        self._mock_generation_calling_sequence = ['mc_occupation',
-                                                  'mc_prim_galprop']
-        self._galprop_dtypes_to_allocate = np.dtype([(prim_galprop_key, 'f8')])
+        self._mock_generation_calling_sequence = ["mc_occupation", "mc_prim_galprop"]
+        self._galprop_dtypes_to_allocate = np.dtype([(prim_galprop_key, "f8")])
         self.prim_galprop_key = prim_galprop_key
         self.param_dict = self.get_default_parameters()
         self.central_occupation_model = Cacciato09Cens(
-            threshold=threshold, prim_haloprop_key=prim_haloprop_key,
-            prim_galprop_key=prim_galprop_key, **kwargs)
-        self._methods_to_inherit = (
-            ['mc_occupation', 'mean_occupation', 'mc_prim_galprop', 'clf',
-             'phi_sat', 'alpha_sat', 'prim_galprop_cut']
-            )
-        self.publications = ['arXiv:0807.4932']
+            threshold=threshold,
+            prim_haloprop_key=prim_haloprop_key,
+            prim_galprop_key=prim_galprop_key,
+            **kwargs
+        )
+        self._methods_to_inherit = [
+            "mc_occupation",
+            "mean_occupation",
+            "mc_prim_galprop",
+            "clf",
+            "phi_sat",
+            "alpha_sat",
+            "prim_galprop_cut",
+        ]
+        self.publications = ["arXiv:0807.4932"]
 
     def get_default_parameters(self):
-        r""" Return the values of ``self.param_dict`` according to
+        r"""Return the values of ``self.param_dict`` according to
         the best-fit values of the WMAP3 model in Table 3 of arXiv:0807.4932.
         In this analysis, halo masses have been defined using an overdensity of
         180 times the background density of the Universe.
         """
 
-        param_dict = (
-            {'a_1': 0.501,
-             'a_2': 2.106,
-             'log_M_2': 14.28,
-             'b_0': -0.766,
-             'b_1': 1.008,
-             'b_2': -0.094,
-             'delta_1': 0.0,
-             'delta_2': 0.0,
-             'log_L_0': 9.935,
-             'log_M_1': 11.07,
-             'gamma_1': 3.273,
-             'gamma_2': 0.255}
-            )
+        param_dict = {
+            "a_1": 0.501,
+            "a_2": 2.106,
+            "log_M_2": 14.28,
+            "b_0": -0.766,
+            "b_1": 1.008,
+            "b_2": -0.094,
+            "delta_1": 0.0,
+            "delta_2": 0.0,
+            "log_L_0": 9.935,
+            "log_M_1": 11.07,
+            "gamma_1": 3.273,
+            "gamma_2": 0.255,
+        }
 
         return param_dict
 
     def _update_central_params(self):
         r"""
         Private method to update the model parameters.
         """
 
         for key, value in self.param_dict.items():
             if key in self.central_occupation_model.param_dict:
                 self.central_occupation_model.param_dict[key] = value
 
     def phi_sat(self, **kwargs):
-        r""" Return the normalization for the CLF as a function of the input
+        r"""Return the normalization for the CLF as a function of the input
         table. See equation (36) in Cacciato et al. (2009) for details.
         The normalization refers to $\phi_s^\star$.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             Array of mass-like variable upon which the calculation is based.
@@ -415,34 +454,39 @@
         -------
         phi_sat : array_like
             Array containing the CLF normalization values of the halos
             specified.
         """
 
         # Retrieve the array storing the primary galaxy property.
-        if 'table' in list(kwargs.keys()):
-            prim_haloprop = kwargs['table'][self.prim_haloprop_key]
-        elif 'prim_haloprop' in list(kwargs.keys()):
-            prim_haloprop = kwargs['prim_haloprop']
+        if "table" in list(kwargs.keys()):
+            prim_haloprop = kwargs["table"][self.prim_haloprop_key]
+        elif "prim_haloprop" in list(kwargs.keys()):
+            prim_haloprop = kwargs["prim_haloprop"]
         else:
-            msg = ("\nYou must pass either a ``table`` or ``prim_haloprop`` "
-                   "argument to the ``alpha_sat`` function of the "
-                   "``Cacciato09Sats`` class.\n")
+            msg = (
+                "\nYou must pass either a ``table`` or ``prim_haloprop`` "
+                "argument to the ``alpha_sat`` function of the "
+                "``Cacciato09Sats`` class.\n"
+            )
             raise HalotoolsError(msg)
 
-        b_0 = self.param_dict['b_0']
-        b_1 = self.param_dict['b_1']
-        b_2 = self.param_dict['b_2']
+        b_0 = self.param_dict["b_0"]
+        b_1 = self.param_dict["b_1"]
+        b_2 = self.param_dict["b_2"]
         log_prim_haloprop = np.log10(prim_haloprop)
 
-        return 10**(b_0 + b_1 * (log_prim_haloprop - 12.0) + b_2 *
-                    (log_prim_haloprop - 12.0)**2)
+        return 10 ** (
+            b_0
+            + b_1 * (log_prim_haloprop - 12.0)
+            + b_2 * (log_prim_haloprop - 12.0) ** 2
+        )
 
     def alpha_sat(self, **kwargs):
-        r""" Return the power-law slope of the CLF as a function of the input
+        r"""Return the power-law slope of the CLF as a function of the input
         table.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             Array of mass-like variable upon which the calculation is based.
             If ``prim_haloprop`` is not passed, then ``table`` keyword argument
@@ -456,33 +500,36 @@
         Returns
         -------
         alpha_sat : array_like
             Array containing the CLF power-law slopes of the halos specified.
         """
 
         # Retrieve the array storing the mass-like variable.
-        if 'table' in list(kwargs.keys()):
-            mass = kwargs['table'][self.prim_haloprop_key]
-        elif 'prim_haloprop' in list(kwargs.keys()):
-            mass = kwargs['prim_haloprop']
+        if "table" in list(kwargs.keys()):
+            mass = kwargs["table"][self.prim_haloprop_key]
+        elif "prim_haloprop" in list(kwargs.keys()):
+            mass = kwargs["prim_haloprop"]
         else:
-            msg = ("\nYou must pass either a ``table`` or ``prim_haloprop`` "
-                   "argument to the ``alpha_sat`` function of the "
-                   "``Cacciato09Sats`` class.\n")
+            msg = (
+                "\nYou must pass either a ``table`` or ``prim_haloprop`` "
+                "argument to the ``alpha_sat`` function of the "
+                "``Cacciato09Sats`` class.\n"
+            )
             raise HalotoolsError(msg)
 
-        a_1 = self.param_dict['a_1']
-        a_2 = self.param_dict['a_2']
-        log_m_2 = self.param_dict['log_M_2']
-
-        return -2.0 + a_1 * (1.0 - 2.0 / np.pi * np.arctan(a_2 * (np.log10(
-            mass) - log_m_2)))
+        a_1 = self.param_dict["a_1"]
+        a_2 = self.param_dict["a_2"]
+        log_m_2 = self.param_dict["log_M_2"]
+
+        return -2.0 + a_1 * (
+            1.0 - 2.0 / np.pi * np.arctan(a_2 * (np.log10(mass) - log_m_2))
+        )
 
     def prim_galprop_cut(self, **kwargs):
-        r""" Return the cut-off primary galaxy properties of the CLF as a
+        r"""Return the cut-off primary galaxy properties of the CLF as a
         function of the input table. See equation (38) in Cacciato et al. (2009)
         for details. The cut-off primary galaxy property refers to $\L_s^\star$.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             Array of mass-like variable upon which the calculation is based.
@@ -497,31 +544,32 @@
         Returns
         -------
         prim_galprop_cut : array_like
             Array containing the cut-off primary galaxy property of the halos
             specified.
         """
 
-        if not ('table' in list(kwargs.keys()) or 'prim_haloprop'
-                in list(kwargs.keys())):
-            msg = ("\nYou must pass either a ``table`` or ``prim_haloprop`` "
-                   "argument to the ``prim_galprop_cut`` function of the "
-                   "``Cacciato09Sats`` class.\n")
+        if not (
+            "table" in list(kwargs.keys()) or "prim_haloprop" in list(kwargs.keys())
+        ):
+            msg = (
+                "\nYou must pass either a ``table`` or ``prim_haloprop`` "
+                "argument to the ``prim_galprop_cut`` function of the "
+                "``Cacciato09Sats`` class.\n"
+            )
             raise HalotoolsError(msg)
 
         self._update_central_params()
 
-        med_prim_galprop = self.central_occupation_model.median_prim_galprop(
-            **kwargs)
+        med_prim_galprop = self.central_occupation_model.median_prim_galprop(**kwargs)
 
         return med_prim_galprop * 0.562
 
-    def mean_occupation(self, prim_galprop_min=None, prim_galprop_max=None,
-                        **kwargs):
-        r""" Expected number of satellite galaxies in a halo. Derived from
+    def mean_occupation(self, prim_galprop_min=None, prim_galprop_max=None, **kwargs):
+        r"""Expected number of satellite galaxies in a halo. Derived from
         integrating the CLF from the luminosity threshold to infinity.
 
         Parameters
         ----------
         prim_galprop_min : float, optional
             Lower limit of the CLF integration used to calculate the expected
             number of satellite galaxies. If not specified, the lower limit is
@@ -546,56 +594,63 @@
         Returns
         -------
         mean_nsat : array
             Mean number of satellite galaxies in the halo of the input mass.
         """
 
         # Retrieve the array storing the primary halo property.
-        if 'table' in list(kwargs.keys()):
-            prim_haloprop = kwargs['table'][self.prim_haloprop_key]
-        elif 'prim_haloprop' in list(kwargs.keys()):
-            prim_haloprop = kwargs['prim_haloprop']
+        if "table" in list(kwargs.keys()):
+            prim_haloprop = kwargs["table"][self.prim_haloprop_key]
+        elif "prim_haloprop" in list(kwargs.keys()):
+            prim_haloprop = kwargs["prim_haloprop"]
         else:
-            msg = ("\nYou must pass either a ``table`` or ``prim_haloprop`` "
-                   "argument to the ``mean_occupation`` function of the "
-                   "``Cacciato09Sats`` class.\n")
+            msg = (
+                "\nYou must pass either a ``table`` or ``prim_haloprop`` "
+                "argument to the ``mean_occupation`` function of the "
+                "``Cacciato09Sats`` class.\n"
+            )
             raise HalotoolsError(msg)
 
         if prim_galprop_min is not None:
             prim_galprop_min = prim_galprop_min
         else:
             prim_galprop_min = 10**self.threshold
 
         if prim_galprop_max is not None:
             if prim_galprop_max <= prim_galprop_min:
-                msg = ("\nFor the ``mean_occupation`` function of the "
-                       "``Cacciato09Sats`` class the ``prim_galprop_max`` "
-                       "keyword must be bigger than 10^threshold or "
-                       "``prim_galprop_min`` if provided.\n")
+                msg = (
+                    "\nFor the ``mean_occupation`` function of the "
+                    "``Cacciato09Sats`` class the ``prim_galprop_max`` "
+                    "keyword must be bigger than 10^threshold or "
+                    "``prim_galprop_min`` if provided.\n"
+                )
                 raise HalotoolsError(msg)
 
         alpha_sat = self.alpha_sat(prim_haloprop=prim_haloprop)
         prim_galprop_cut = self.prim_galprop_cut(prim_haloprop=prim_haloprop)
         phi_sat = self.phi_sat(prim_haloprop=prim_haloprop)
-        delta = 10**(self.param_dict['delta_1'] + self.param_dict['delta_2'] *
-                     (np.log10(prim_haloprop) - 12))
-
-        result = custom_incomplete_gamma(alpha_sat / 2.0 + 0.5,
-                                         delta * (prim_galprop_min /
-                                                  prim_galprop_cut)**2)
+        delta = 10 ** (
+            self.param_dict["delta_1"]
+            + self.param_dict["delta_2"] * (np.log10(prim_haloprop) - 12)
+        )
+
+        result = custom_incomplete_gamma(
+            alpha_sat / 2.0 + 0.5, delta * (prim_galprop_min / prim_galprop_cut) ** 2
+        )
         if prim_galprop_max is not None:
             result = result - custom_incomplete_gamma(
                 alpha_sat / 2.0 + 0.5,
-                delta * (prim_galprop_max / prim_galprop_cut)**2)
+                delta * (prim_galprop_max / prim_galprop_cut) ** 2,
+            )
 
-        result = result * (phi_sat / 2.0) * delta**(- (alpha_sat + 1.0) / 2.0)
+        result = result * (phi_sat / 2.0) * delta ** (-(alpha_sat + 1.0) / 2.0)
         return result
 
     def clf(self, prim_galprop=1e10, prim_haloprop=1e12):
-        r""" Return the CLF in units of dn/dlogL for the primary halo property
+        r"""Return the CLF in units of dn/dlogL for the primary halo property
         and galaxy property L.
 
         Parameters
         ----------
         prim_haloprop : array_like, optional
             Array of mass-like variable upon which the calculation is based.
 
@@ -613,33 +668,43 @@
             assumed throughout.
         """
 
         prim_galprop = np.atleast_1d(prim_galprop)
         prim_haloprop = np.atleast_1d(prim_haloprop)
 
         try:
-            assert ((len(prim_haloprop) == 1) or (len(prim_galprop) == 1) or
-                    (len(prim_haloprop) == (len(prim_galprop))))
+            assert (
+                (len(prim_haloprop) == 1)
+                or (len(prim_galprop) == 1)
+                or (len(prim_haloprop) == (len(prim_galprop)))
+            )
         except AssertionError:
-            msg = ("If both ``prim_galprop`` and ``prim_haloprop`` are arrays"
-                   " with multiple elements, they must have the same length.\n")
+            msg = (
+                "If both ``prim_galprop`` and ``prim_haloprop`` are arrays"
+                " with multiple elements, they must have the same length.\n"
+            )
             raise HalotoolsError(msg)
 
         phi_sat = self.phi_sat(prim_haloprop=prim_haloprop)
         alpha_sat = self.alpha_sat(prim_haloprop=prim_haloprop)
         prim_galprop_cut = self.prim_galprop_cut(prim_haloprop=prim_haloprop)
-        delta = 10**(self.param_dict['delta_1'] + self.param_dict['delta_2'] *
-                     (np.log10(prim_haloprop) - 12))
-
-        return (phi_sat * (prim_galprop / prim_galprop_cut)**(alpha_sat + 1) *
-                np.exp(-delta * (prim_galprop / prim_galprop_cut)**2) *
-                np.log(10))
+        delta = 10 ** (
+            self.param_dict["delta_1"]
+            + self.param_dict["delta_2"] * (np.log10(prim_haloprop) - 12)
+        )
+
+        return (
+            phi_sat
+            * (prim_galprop / prim_galprop_cut) ** (alpha_sat + 1)
+            * np.exp(-delta * (prim_galprop / prim_galprop_cut) ** 2)
+            * np.log(10)
+        )
 
     def mc_prim_galprop(self, **kwargs):
-        r""" Method to generate Monte Carlo realizations of the primary galaxy
+        r"""Method to generate Monte Carlo realizations of the primary galaxy
         property of galaxies under the constraint that the primary galaxy
         property is above the primary galaxy property threshold.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             Array of mass-like variable upon which the primary galaxy properties
@@ -661,39 +726,47 @@
         mc_prim_galprop : array
             Float array giving the Monte Carlo realization of primary galaxy
             properties of satellites in halos of the given mass. All primary
             galaxy properties returned are above the threshold.
         """
 
         # Retrieve the array storing the mass-like variable.
-        if 'table' in list(kwargs.keys()):
-            mass = kwargs['table'][self.prim_haloprop_key]
-        elif 'prim_haloprop' in list(kwargs.keys()):
-            mass = kwargs['prim_haloprop']
+        if "table" in list(kwargs.keys()):
+            mass = kwargs["table"][self.prim_haloprop_key]
+        elif "prim_haloprop" in list(kwargs.keys()):
+            mass = kwargs["prim_haloprop"]
         else:
-            msg = ("\nYou must pass either a ``table`` or ``prim_haloprop`` "
-                   "argument to the ``mc_prim_galprop`` function of the "
-                   "``Cacciato09Sats`` class.\n")
+            msg = (
+                "\nYou must pass either a ``table`` or ``prim_haloprop`` "
+                "argument to the ``mc_prim_galprop`` function of the "
+                "``Cacciato09Sats`` class.\n"
+            )
             raise HalotoolsError(msg)
 
         alpha_sat = self.alpha_sat(**kwargs)
         prim_galprop_cut = self.prim_galprop_cut(**kwargs)
         prim_galprop = np.zeros(len(mass))
 
         if np.any(alpha_sat > 10):
-            msg = ("\nThe ``mc_prim_galprop`` function of the "
-                   "``Cacciato09Sats`` class does not support models where "
-                   "alpha_sat is bigger than 10.\n")
+            msg = (
+                "\nThe ``mc_prim_galprop`` function of the "
+                "``Cacciato09Sats`` class does not support models where "
+                "alpha_sat is bigger than 10.\n"
+            )
             raise HalotoolsError(msg)
 
-        seed = kwargs.get('seed', None)
+        seed = kwargs.get("seed", None)
         with NumpyRNGContext(seed):
             while np.any(prim_galprop == 0):
                 randoms = np.random.random(size=len(mass) * 2)
                 prim_galprop = cacciato09_sats_mc_prim_galprop_engine(
-                    prim_galprop, randoms, alpha_sat, prim_galprop_cut,
-                    10**self.threshold)
+                    prim_galprop,
+                    randoms,
+                    alpha_sat,
+                    prim_galprop_cut,
+                    10**self.threshold,
+                )
 
-        if 'table' in list(kwargs.keys()):
-            kwargs['table'][self.prim_galprop_key][:] = prim_galprop
+        if "table" in list(kwargs.keys()):
+            kwargs["table"][self.prim_galprop_key][:] = prim_galprop
 
         return prim_galprop
```

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/engines/cacciato09_sats_mc_prim_galprop_engine.pyx` & `halotools-0.8.2/halotools/empirical_models/occupation_models/engines/cacciato09_sats_mc_prim_galprop_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/engines/setup_package.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/engines/setup_package.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/occupation_model_template.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/occupation_model_template.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_cacciato09_clf.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_cacciato09_clf.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_leauthaud11_hod.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_leauthaud11_hod.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """ Module providing unit-testing for the component models in
 `halotools.empirical_models.occupation_components.leauthaud11_components` module"
 """
 import numpy as np
 import pytest
 
-from .. import Leauthaud11Cens, Leauthaud11Sats
+from ..leauthaud11_components import Leauthaud11Cens, Leauthaud11Sats
 
-__all__ = ('test_Leauthaud11Cens', 'test_Leauthaud11Sats')
+__all__ = ("test_Leauthaud11Cens", "test_Leauthaud11Sats")
 
 
 @pytest.mark.installation_test
 def test_Leauthaud11Cens():
-    """ Function to test
+    """Function to test
     `~halotools.empirical_models.Leauthaud11Cens`.
     """
 
     # Verify that the mean and Monte Carlo occupations are both reasonable and in agreement
     # for halos of mass 1e12
     model = Leauthaud11Cens()
     ncen1 = model.mean_occupation(prim_haloprop=5e11)
-    mcocc = model.mc_occupation(prim_haloprop=np.ones(int(1e4))*5e11, seed=43)
+    mcocc = model.mc_occupation(prim_haloprop=np.ones(int(1e4)) * 5e11, seed=43)
 
     # Check that the model behavior is altered in the expected way by changing param_dict values
 
     # Increasing scatter picks up more galaxies in low-mass halos
-    model.param_dict['scatter_model_param1'] *= 1.5
+    model.param_dict["scatter_model_param1"] *= 1.5
     ncen2 = model.mean_occupation(prim_haloprop=5e11)
     assert ncen2 > ncen1
-#
-    model.param_dict['smhm_m1_0'] *= 1.1
+    #
+    model.param_dict["smhm_m1_0"] *= 1.1
     ncen3 = model.mean_occupation(prim_haloprop=5e11)
     assert ncen3 < ncen2
-#
-    model.param_dict['smhm_m1_a'] *= 1.1
+    #
+    model.param_dict["smhm_m1_a"] *= 1.1
     ncen4 = model.mean_occupation(prim_haloprop=5e11)
     assert ncen4 == ncen3
 
     # Check that increasing stellar mass thresholds decreases the mean occupation
     model2 = Leauthaud11Cens(threshold=10.75)
     ncen5 = model2.mean_occupation(prim_haloprop=5e11)
     model3 = Leauthaud11Cens(threshold=11.25)
@@ -44,73 +44,73 @@
     assert ncen6 < ncen5 < ncen1
 
     __ = model2.get_published_parameters()
 
 
 @pytest.mark.installation_test
 def test_Leauthaud11Sats():
-    """ Function to test
+    """Function to test
     `~halotools.empirical_models.Leauthaud11Cens`.
     """
 
     # Verify that the mean and Monte Carlo occupations are both reasonable and in agreement
     # for halos of mass 1e12
     model = Leauthaud11Sats()
-    nsat1 = model.mean_occupation(prim_haloprop=5.e12)
-    mcocc = model.mc_occupation(prim_haloprop=np.ones(int(1e4))*5e12, seed=43)
+    nsat1 = model.mean_occupation(prim_haloprop=5.0e12)
+    mcocc = model.mc_occupation(prim_haloprop=np.ones(int(1e4)) * 5e12, seed=43)
 
     # Check that the model behavior is altered in the expected way by changing param_dict values
-    model.param_dict['alphasat'] *= 1.1
-    nsat2 = model.mean_occupation(prim_haloprop=5.e12)
+    model.param_dict["alphasat"] *= 1.1
+    nsat2 = model.mean_occupation(prim_haloprop=5.0e12)
     assert nsat2 < nsat1
 
     # Msat := Bsat(mhalo_thresh/1e12)**betasat
     # since mhalo_thresh(logM*=10.5) > 1e12, increasing betasat should increase Msat
     msat1 = np.copy(model._msat)
-    model.param_dict['betasat'] *= 1.1
+    model.param_dict["betasat"] *= 1.1
     model._update_satellite_params()
     msat2 = np.copy(model._msat)
     assert msat2 > msat1
 
     # Msat := Bsat(mhalo_thresh/1e12)**betasat
     # Increasing Bsat should increase Msat regardless of mass
     model._update_satellite_params()
     msat1 = np.copy(model._msat)
-    model.param_dict['bsat'] *= 1.1
+    model.param_dict["bsat"] *= 1.1
     model._update_satellite_params()
     msat2 = np.copy(model._msat)
     assert msat2 > msat1
-#
+    #
     # Mcut := Bcut(mhalo_thresh/1e12)**betacut
     # Default value of betacut is -0.13 for default threshold of 10.5
     # since mhalo_thresh(logM*=10.5) > 1e12, increasing betacut should increase Mcut
-    model.param_dict['betacut'] = -0.13
+    model.param_dict["betacut"] = -0.13
     model._update_satellite_params()
     mcut1 = np.copy(model._mcut)
-    model.param_dict['betacut'] = -0.1
+    model.param_dict["betacut"] = -0.1
     model._update_satellite_params()
     mcut2 = np.copy(model._mcut)
     assert mcut2 > mcut1
-# #
+    # #
     # Mcut := Bcut(mhalo_thresh/1e12)**betacut
     # Increasing Bcut should increase Mcut regardless of mass
     model._update_satellite_params()
     mcut1 = np.copy(model._mcut)
-    model.param_dict['bcut'] *= 1.1
+    model.param_dict["bcut"] *= 1.1
     model._update_satellite_params()
     mcut2 = np.copy(model._mcut)
     assert mcut2 > mcut1
-# #
-#
+    # #
+    #
     # Check that modulate_with_cenocc strictly decreases the mean occupations
     model2a = Leauthaud11Sats(modulate_with_cenocc=False)
     model2b = Leauthaud11Sats(modulate_with_cenocc=True)
-    nsat2a = model2a.mean_occupation(prim_haloprop=5.e12)
-    nsat2b = model2b.mean_occupation(prim_haloprop=5.e12)
-    assert model2b.central_occupation_model.mean_occupation(prim_haloprop=5.e12) < 1
+    nsat2a = model2a.mean_occupation(prim_haloprop=5.0e12)
+    nsat2b = model2b.mean_occupation(prim_haloprop=5.0e12)
+    assert model2b.central_occupation_model.mean_occupation(prim_haloprop=5.0e12) < 1
     assert nsat2b < nsat2a
 
     # Check that increasing stellar mass thresholds decreases the mean occupation
     model10 = Leauthaud11Sats(threshold=10)
     model105 = Leauthaud11Sats(threshold=10.5)
     model11 = Leauthaud11Sats(threshold=11)
     nsat10 = model10.mean_occupation(prim_haloprop=1e13)
```

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_occupation_component.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_occupation_component.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_tinker13.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_tinker13.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_zheng07_centrals.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_zheng07_centrals.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_zheng07_satellites.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_zheng07_satellites.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
     fracdiff_highmass = (
         model4.mean_occupation(prim_haloprop=highmass)
         - default_model.mean_occupation(prim_haloprop=highmass)
     ) / default_model.mean_occupation(prim_haloprop=highmass)
     assert fracdiff_highmass < 0
 
     # The fractional change due to alterations of logM1 should be identical at all mass
-    assert fracdiff_highmass == fracdiff_midmass
+    assert np.allclose(fracdiff_highmass, fracdiff_midmass)
 
 
 def test_raises_correct_exception():
     default_model = Zheng07Sats()
     with pytest.raises(HalotoolsError) as err:
         _ = default_model.mean_occupation(x=4)
     substr = "You must pass either a ``table`` or ``prim_haloprop`` argument"
```

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/tests/test_zu_mandelbaum15_components.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/tests/test_zu_mandelbaum15_components.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/tinker13_components.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/tinker13_components.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,41 +13,48 @@
 from ..smhm_models import Behroozi10SmHm
 from ..assembias_models import HeavisideAssembias
 
 from ...utils.array_utils import custom_len
 from ... import sim_manager
 from ...custom_exceptions import HalotoolsError
 
-__all__ = ('Tinker13Cens', 'Tinker13QuiescentSats',
-           'Tinker13ActiveSats', 'AssembiasTinker13Cens')
+__all__ = (
+    "Tinker13Cens",
+    "Tinker13QuiescentSats",
+    "Tinker13ActiveSats",
+    "AssembiasTinker13Cens",
+)
 
 # The following 4 lines of copde maintain python 2 and 3 compatability.
 # See Tinker13Cens.mean_occupation() method for the use the unicode type
 try:
     unicode  # Python 2: type "unicode" is built-in
 except NameError:
     unicode = str  # Python 3
 
 
 class Tinker13Cens(OccupationComponent):
-    """ HOD-style model for a central galaxy occupation that derives from
+    """HOD-style model for a central galaxy occupation that derives from
     two distinct active/quiescent stellar-to-halo-mass relations.
 
     .. note::
 
         The `Tinker13Cens` model is part of the ``tinker13``
         prebuilt composite HOD-style model. For a tutorial on the ``tinker13``
         composite model, see :ref:`tinker13_composite_model`.
 
     """
 
-    def __init__(self, threshold=model_defaults.default_stellar_mass_threshold,
-            prim_haloprop_key=model_defaults.prim_haloprop_key,
-            redshift=sim_manager.sim_defaults.default_redshift,
-            **kwargs):
+    def __init__(
+        self,
+        threshold=model_defaults.default_stellar_mass_threshold,
+        prim_haloprop_key=model_defaults.prim_haloprop_key,
+        redshift=sim_manager.sim_defaults.default_redshift,
+        **kwargs
+    ):
         """
         Parameters
         ----------
         threshold : float, optional
             Stellar mass threshold of the mock galaxy sample in h=1 solar mass units.
             Default value is specified in the `~halotools.empirical_models.model_defaults` module.
 
@@ -72,241 +79,266 @@
         upper_occupation_bound = 1.0
 
         self.littleh = 0.72
 
         # Call the super class constructor, which binds all the
         # arguments to the instance.
         super(Tinker13Cens, self).__init__(
-            gal_type='centrals', threshold=threshold,
+            gal_type="centrals",
+            threshold=threshold,
             upper_occupation_bound=upper_occupation_bound,
             prim_haloprop_key=prim_haloprop_key,
-            **kwargs)
+            **kwargs
+        )
         self.redshift = redshift
 
-        self.smhm_model = Behroozi10SmHm(
-            prim_haloprop_key=prim_haloprop_key, **kwargs)
+        self.smhm_model = Behroozi10SmHm(prim_haloprop_key=prim_haloprop_key, **kwargs)
 
         self._initialize_param_dict(**kwargs)
 
-        self.sfr_designation_key = 'central_sfr_designation'
+        self.sfr_designation_key = "central_sfr_designation"
 
-        self.publications = ['arXiv:1308.2974', 'arXiv:1103.2077', 'arXiv:1104.0928']
+        self.publications = ["arXiv:1308.2974", "arXiv:1103.2077", "arXiv:1104.0928"]
 
         # The _methods_to_inherit determines which methods will be directly callable
         # by the composite model built by the HodModelFactory
         # Here we are overriding this attribute that is normally defined
         # in the OccupationComponent super class
-        self._methods_to_inherit = (
-            ['mc_occupation', 'mean_occupation', 'mean_occupation_active', 'mean_occupation_quiescent',
-            'mean_stellar_mass_active', 'mean_stellar_mass_quiescent',
-            'mean_log_halo_mass_active', 'mean_log_halo_mass_quiescent']
-            )
+        self._methods_to_inherit = [
+            "mc_occupation",
+            "mean_occupation",
+            "mean_occupation_active",
+            "mean_occupation_quiescent",
+            "mean_stellar_mass_active",
+            "mean_stellar_mass_quiescent",
+            "mean_log_halo_mass_active",
+            "mean_log_halo_mass_quiescent",
+        ]
 
         # The _mock_generation_calling_sequence determines which methods
         # will be called during mock population, as well as in what order they will be called
-        self._mock_generation_calling_sequence = ['mc_sfr_designation', 'mc_occupation']
-        self._galprop_dtypes_to_allocate = np.dtype([
-            ('halo_num_' + self.gal_type, 'i4'),
-            (self.sfr_designation_key, object),
-            ('sfr_designation', object),
-            ])
-
-    def _initialize_param_dict(self,
-            quiescent_fraction_abscissa=[6.31e10, 3.98e11, 2.51e12, 1.58e13, 1.e14],
-            quiescent_fraction_ordinates=[0.052, 0.14, 0.54, 0.63, 0.77], **kwargs):
-        """
-        """
+        self._mock_generation_calling_sequence = ["mc_sfr_designation", "mc_occupation"]
+        self._galprop_dtypes_to_allocate = np.dtype(
+            [
+                ("halo_num_" + self.gal_type, "i4"),
+                (self.sfr_designation_key, object),
+                ("sfr_designation", object),
+            ]
+        )
+
+    def _initialize_param_dict(
+        self,
+        quiescent_fraction_abscissa=[6.31e10, 3.98e11, 2.51e12, 1.58e13, 1.0e14],
+        quiescent_fraction_ordinates=[0.052, 0.14, 0.54, 0.63, 0.77],
+        **kwargs
+    ):
+        """ """
         self.param_dict = {}
         for key, value in self.smhm_model.param_dict.items():
-            active_key = key + '_active'
-            quiescent_key = key + '_quiescent'
+            active_key = key + "_active"
+            quiescent_key = key + "_quiescent"
             self.param_dict[active_key] = value
             self.param_dict[quiescent_key] = value
 
         # From Table 2 of Tinker+13
-        self.param_dict['smhm_m1_0_active'] = 12.56
-        self.param_dict['smhm_m1_0_quiescent'] = 12.08
-        self.param_dict['smhm_m0_0_active'] = 10.96
-        self.param_dict['smhm_m0_0_quiescent'] = 10.7
-        self.param_dict['smhm_beta_0_active'] = 0.44
-        self.param_dict['smhm_beta_0_quiescent'] = 0.32
-        self.param_dict['smhm_delta_0_active'] = 0.52
-        self.param_dict['smhm_delta_0_quiescent'] = 0.93
-        self.param_dict['smhm_gamma_0_active'] = 1.48
-        self.param_dict['smhm_gamma_0_quiescent'] = 0.81
-        self.param_dict['scatter_model_param1_active'] = 0.21
-        self.param_dict['scatter_model_param1_quiescent'] = 0.28
-
-        self._quiescent_fraction_abscissa = np.array(quiescent_fraction_abscissa)/self.littleh
-        ordinates_key_prefix = 'quiescent_fraction_ordinates'
-        self._ordinates_keys = (
-            [ordinates_key_prefix + '_param' + str(i+1)
-            for i in range(custom_len(self._quiescent_fraction_abscissa))]
-            )
+        self.param_dict["smhm_m1_0_active"] = 12.56
+        self.param_dict["smhm_m1_0_quiescent"] = 12.08
+        self.param_dict["smhm_m0_0_active"] = 10.96
+        self.param_dict["smhm_m0_0_quiescent"] = 10.7
+        self.param_dict["smhm_beta_0_active"] = 0.44
+        self.param_dict["smhm_beta_0_quiescent"] = 0.32
+        self.param_dict["smhm_delta_0_active"] = 0.52
+        self.param_dict["smhm_delta_0_quiescent"] = 0.93
+        self.param_dict["smhm_gamma_0_active"] = 1.48
+        self.param_dict["smhm_gamma_0_quiescent"] = 0.81
+        self.param_dict["scatter_model_param1_active"] = 0.21
+        self.param_dict["scatter_model_param1_quiescent"] = 0.28
+
+        self._quiescent_fraction_abscissa = (
+            np.array(quiescent_fraction_abscissa) / self.littleh
+        )
+        ordinates_key_prefix = "quiescent_fraction_ordinates"
+        self._ordinates_keys = [
+            ordinates_key_prefix + "_param" + str(i + 1)
+            for i in range(custom_len(self._quiescent_fraction_abscissa))
+        ]
         for key, value in zip(self._ordinates_keys, quiescent_fraction_ordinates):
             self.param_dict[key] = value
 
     def mean_quiescent_fraction(self, **kwargs):
-        """
-        """
-        model_ordinates = [self.param_dict[ordinate_key] for ordinate_key in self._ordinates_keys]
+        """ """
+        model_ordinates = [
+            self.param_dict[ordinate_key] for ordinate_key in self._ordinates_keys
+        ]
         spline_function = model_helpers.custom_spline(
-            np.log10(self._quiescent_fraction_abscissa), model_ordinates)
+            np.log10(self._quiescent_fraction_abscissa), model_ordinates
+        )
 
-        if 'prim_haloprop' in kwargs:
-            prim_haloprop = np.atleast_1d(kwargs['prim_haloprop'])
-        elif 'table' in kwargs:
-            table = kwargs['table']
+        if "prim_haloprop" in kwargs:
+            prim_haloprop = np.atleast_1d(kwargs["prim_haloprop"])
+        elif "table" in kwargs:
+            table = kwargs["table"]
             try:
                 prim_haloprop = table[self.prim_haloprop_key]
             except KeyError:
-                msg = ("The ``table`` passed as a keyword argument to the mean_quiescent_fraction method\n"
-                    "does not have the requested ``%s`` key")
+                msg = (
+                    "The ``table`` passed as a keyword argument to the mean_quiescent_fraction method\n"
+                    "does not have the requested ``%s`` key"
+                )
                 raise HalotoolsError(msg % self.prim_haloprop_key)
 
         fraction = spline_function(np.log10(prim_haloprop))
 
-        fraction = np.where(fraction < 0, 0., fraction)
-        fraction = np.where(fraction > 1, 1., fraction)
+        fraction = np.where(fraction < 0, 0.0, fraction)
+        fraction = np.where(fraction > 1, 1.0, fraction)
 
         return fraction
 
     def mc_sfr_designation(self, seed=None, **kwargs):
-        """
-        """
+        """ """
         quiescent_fraction = self.mean_quiescent_fraction(**kwargs)
 
         with NumpyRNGContext(seed):
             mc_generator = np.random.random(custom_len(quiescent_fraction))
 
-        result = np.where(mc_generator < quiescent_fraction, 'quiescent', 'active')
-        if 'table' in kwargs:
-            kwargs['table'][self.sfr_designation_key] = result
-            kwargs['table']['sfr_designation'] = result
+        result = np.where(mc_generator < quiescent_fraction, "quiescent", "active")
+        if "table" in kwargs:
+            kwargs["table"][self.sfr_designation_key] = result
+            kwargs["table"]["sfr_designation"] = result
 
         return result
 
     def mean_occupation(self, **kwargs):
-        """
-        """
-        if 'table' in kwargs:
-            table = kwargs['table']
+        """ """
+        if "table" in kwargs:
+            table = kwargs["table"]
             try:
                 prim_haloprop = table[self.prim_haloprop_key]
             except KeyError:
-                msg = ("The ``table`` passed as a keyword argument to the ``mean_occupation`` method\n"
-                    "does not have the requested ``%s`` key")
+                msg = (
+                    "The ``table`` passed as a keyword argument to the ``mean_occupation`` method\n"
+                    "does not have the requested ``%s`` key"
+                )
                 raise HalotoolsError(msg % self.prim_haloprop_key)
             try:
                 sfr_designation = table[self.sfr_designation_key]
             except KeyError:
-                msg = ("The ``table`` passed as a keyword argument to the ``mean_occupation`` method\n"
-                    "does not have the requested ``%s`` key used for SFR designation")
+                msg = (
+                    "The ``table`` passed as a keyword argument to the ``mean_occupation`` method\n"
+                    "does not have the requested ``%s`` key used for SFR designation"
+                )
                 raise HalotoolsError(msg % self.sfr_designation_key)
         else:
             try:
-                prim_haloprop = np.atleast_1d(kwargs['prim_haloprop'])
-                sfr_designation = np.atleast_1d(kwargs['sfr_designation'])
+                prim_haloprop = np.atleast_1d(kwargs["prim_haloprop"])
+                sfr_designation = np.atleast_1d(kwargs["sfr_designation"])
             except KeyError:
-                msg = ("If not passing a ``table`` keyword argument to the ``mean_occupation`` method,\n"
-                    "you must pass both ``prim_haloprop`` and ``sfr_designation`` keyword arguments")
+                msg = (
+                    "If not passing a ``table`` keyword argument to the ``mean_occupation`` method,\n"
+                    "you must pass both ``prim_haloprop`` and ``sfr_designation`` keyword arguments"
+                )
                 raise HalotoolsError(msg)
             if type(sfr_designation[0]) in (str, unicode, np.string_, np.unicode_):
-                if sfr_designation[0] not in ['active', 'quiescent']:
-                    msg = ("The only acceptable values of "
-                        "``sfr_designation`` are ``active`` or ``quiescent``")
+                if sfr_designation[0] not in ["active", "quiescent"]:
+                    msg = (
+                        "The only acceptable values of "
+                        "``sfr_designation`` are ``active`` or ``quiescent``"
+                    )
                     raise HalotoolsError(msg)
 
-        if 'table' in kwargs:
+        if "table" in kwargs:
             quiescent_result = self.mean_occupation_quiescent(table=table)
             active_result = self.mean_occupation_active(table=table)
         else:
-            quiescent_result = self.mean_occupation_quiescent(prim_haloprop=prim_haloprop)
+            quiescent_result = self.mean_occupation_quiescent(
+                prim_haloprop=prim_haloprop
+            )
             active_result = self.mean_occupation_active(prim_haloprop=prim_haloprop)
 
-        result = np.where(sfr_designation == 'quiescent', quiescent_result, active_result)
+        result = np.where(
+            sfr_designation == "quiescent", quiescent_result, active_result
+        )
 
         return result
 
     def mean_occupation_active(self, **kwargs):
-        """
-        """
-        self._update_smhm_param_dict('active')
+        """ """
+        self._update_smhm_param_dict("active")
+
+        logmstar = np.log10(
+            self.smhm_model.mean_stellar_mass(redshift=self.redshift, **kwargs)
+        )
+        logscatter = math.sqrt(2) * self.smhm_model.mean_scatter(**kwargs)
 
-        logmstar = np.log10(self.smhm_model.mean_stellar_mass(
-            redshift=self.redshift, **kwargs))
-        logscatter = math.sqrt(2)*self.smhm_model.mean_scatter(**kwargs)
-
-        mean_ncen = 0.5*(1.0 -
-            erf((self.threshold - logmstar)/logscatter))
-        mean_ncen *= (1. - self.mean_quiescent_fraction(**kwargs))
+        mean_ncen = 0.5 * (1.0 - erf((self.threshold - logmstar) / logscatter))
+        mean_ncen *= 1.0 - self.mean_quiescent_fraction(**kwargs)
 
         return mean_ncen
 
     def mean_occupation_quiescent(self, **kwargs):
-        """
-        """
-        self._update_smhm_param_dict('quiescent')
+        """ """
+        self._update_smhm_param_dict("quiescent")
 
-        logmstar = np.log10(self.smhm_model.mean_stellar_mass(
-            redshift=self.redshift, **kwargs))
-        logscatter = math.sqrt(2)*self.smhm_model.mean_scatter(**kwargs)
+        logmstar = np.log10(
+            self.smhm_model.mean_stellar_mass(redshift=self.redshift, **kwargs)
+        )
+        logscatter = math.sqrt(2) * self.smhm_model.mean_scatter(**kwargs)
 
-        mean_ncen = 0.5*(1.0 -
-            erf((self.threshold - logmstar)/logscatter))
+        mean_ncen = 0.5 * (1.0 - erf((self.threshold - logmstar) / logscatter))
         mean_ncen *= self.mean_quiescent_fraction(**kwargs)
 
         return mean_ncen
 
     def mean_stellar_mass_active(self, **kwargs):
-        """
-        """
-        self._update_smhm_param_dict('active')
+        """ """
+        self._update_smhm_param_dict("active")
         return self.smhm_model.mean_stellar_mass(redshift=self.redshift, **kwargs)
 
     def mean_stellar_mass_quiescent(self, **kwargs):
-        """
-        """
-        self._update_smhm_param_dict('quiescent')
+        """ """
+        self._update_smhm_param_dict("quiescent")
         return self.smhm_model.mean_stellar_mass(redshift=self.redshift, **kwargs)
 
     def mean_log_halo_mass_active(self, log_stellar_mass):
-        """
-        """
-        self._update_smhm_param_dict('active')
-        return self.smhm_model.mean_log_halo_mass(log_stellar_mass,
-            redshift=self.redshift)
+        """ """
+        self._update_smhm_param_dict("active")
+        return self.smhm_model.mean_log_halo_mass(
+            log_stellar_mass, redshift=self.redshift
+        )
 
     def mean_log_halo_mass_quiescent(self, log_stellar_mass):
-        """
-        """
-        self._update_smhm_param_dict('quiescent')
-        return self.smhm_model.mean_log_halo_mass(log_stellar_mass,
-            redshift=self.redshift)
+        """ """
+        self._update_smhm_param_dict("quiescent")
+        return self.smhm_model.mean_log_halo_mass(
+            log_stellar_mass, redshift=self.redshift
+        )
 
     def _update_smhm_param_dict(self, sfr_key):
 
         for key, value in self.param_dict.items():
             if sfr_key in key:
-                stripped_key = key[:-len(sfr_key)-1]
+                stripped_key = key[: -len(sfr_key) - 1]
             else:
                 stripped_key = key
             if stripped_key in self.smhm_model.param_dict:
                 self.smhm_model.param_dict[stripped_key] = value
 
 
 class AssembiasTinker13Cens(Tinker13Cens, HeavisideAssembias):
-    """ HOD-style model for a central galaxy occupation that derives from
+    """HOD-style model for a central galaxy occupation that derives from
     two distinct active/quiescent stellar-to-halo-mass relations.
     """
 
-    def __init__(self, threshold=model_defaults.default_stellar_mass_threshold,
-            prim_haloprop_key=model_defaults.prim_haloprop_key,
-            redshift=sim_manager.sim_defaults.default_redshift,
-            **kwargs):
+    def __init__(
+        self,
+        threshold=model_defaults.default_stellar_mass_threshold,
+        prim_haloprop_key=model_defaults.prim_haloprop_key,
+        redshift=sim_manager.sim_defaults.default_redshift,
+        **kwargs
+    ):
         """
         Parameters
         ----------
         threshold : float, optional
             Stellar mass threshold of the mock galaxy sample in h=1 solar mass units.
             Default value is specified in the `~halotools.empirical_models.model_defaults` module.
 
@@ -354,35 +386,41 @@
             Values of the primary halo property at which the assembly bias strength is specified.
             Default is to assume a constant strength of 0.5. If passing a list, the strength
             will interpreted at the input ``assembias_strength_abscissa``.
             Default is to assume a constant strength of 0.5.
 
         """
         Tinker13Cens.__init__(self, **kwargs)
-        HeavisideAssembias.__init__(self,
-            method_name_to_decorate='mean_quiescent_fraction',
-            lower_assembias_bound=0.,
-            upper_assembias_bound=1.,
-            **kwargs)
+        HeavisideAssembias.__init__(
+            self,
+            method_name_to_decorate="mean_quiescent_fraction",
+            lower_assembias_bound=0.0,
+            upper_assembias_bound=1.0,
+            **kwargs
+        )
 
 
 class Tinker13QuiescentSats(OccupationComponent):
-    """ HOD-style model for a central galaxy occupation that derives from
+    """HOD-style model for a central galaxy occupation that derives from
     two distinct active/quiescent stellar-to-halo-mass relations.
 
     .. note::
 
         The `Tinker13QuiescentSats` model is part of the ``tinker13``
         prebuilt composite HOD-style model. For a tutorial on the ``tinker13``
         composite model, see :ref:`tinker13_composite_model`.
     """
 
-    def __init__(self, threshold=model_defaults.default_stellar_mass_threshold,
-            prim_haloprop_key=model_defaults.prim_haloprop_key,
-            redshift=sim_manager.sim_defaults.default_redshift, **kwargs):
+    def __init__(
+        self,
+        threshold=model_defaults.default_stellar_mass_threshold,
+        prim_haloprop_key=model_defaults.prim_haloprop_key,
+        redshift=sim_manager.sim_defaults.default_redshift,
+        **kwargs
+    ):
         """
         Parameters
         ----------
         threshold : float, optional
             Stellar mass threshold of the mock galaxy sample in h=1 solar mass units.
             Default value is specified in the `~halotools.empirical_models.model_defaults` module.
 
@@ -399,44 +437,48 @@
         upper_occupation_bound = float("inf")
 
         self.littleh = 0.72
 
         # Call the super class constructor, which binds all the
         # arguments to the instance.
         super(Tinker13QuiescentSats, self).__init__(
-            gal_type='quiescent_satellites', threshold=threshold,
+            gal_type="quiescent_satellites",
+            threshold=threshold,
             upper_occupation_bound=upper_occupation_bound,
-            prim_haloprop_key=prim_haloprop_key, **kwargs)
+            prim_haloprop_key=prim_haloprop_key,
+            **kwargs
+        )
         self.redshift = redshift
 
-        self.smhm_model = Behroozi10SmHm(
-            prim_haloprop_key=prim_haloprop_key, **kwargs)
+        self.smhm_model = Behroozi10SmHm(prim_haloprop_key=prim_haloprop_key, **kwargs)
 
         self._initialize_param_dict()
 
-        self.sfr_designation_key = 'sfr_designation'
+        self.sfr_designation_key = "sfr_designation"
 
-        self.publications = ['arXiv:1308.2974', 'arXiv:1103.2077', 'arXiv:1104.0928']
+        self.publications = ["arXiv:1308.2974", "arXiv:1103.2077", "arXiv:1104.0928"]
 
         # The _methods_to_inherit determines which methods will be directly callable
         # by the composite model built by the HodModelFactory
         # Here we are overriding this attribute that is normally defined
         # in the OccupationComponent super class
-        self._methods_to_inherit = ['mc_occupation', 'mean_occupation']
+        self._methods_to_inherit = ["mc_occupation", "mean_occupation"]
 
         # The _mock_generation_calling_sequence determines which methods
         # will be called during mock population, as well as in what order they will be called
-        self._mock_generation_calling_sequence = ['mc_occupation', 'mc_sfr_designation']
-        self._galprop_dtypes_to_allocate = np.dtype([
-            ('halo_num_' + self.gal_type, 'i4'),
-            (self.sfr_designation_key, object),
-            ])
+        self._mock_generation_calling_sequence = ["mc_occupation", "mc_sfr_designation"]
+        self._galprop_dtypes_to_allocate = np.dtype(
+            [
+                ("halo_num_" + self.gal_type, "i4"),
+                (self.sfr_designation_key, object),
+            ]
+        )
 
     def mean_occupation(self, **kwargs):
-        """ Expected number of central galaxies in a halo of mass halo_mass.
+        """Expected number of central galaxies in a halo of mass halo_mass.
         See Equation 12-14 of arXiv:1103.2077.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             array of masses of table in the catalog
 
@@ -454,102 +496,111 @@
         >>> mean_nsat = sat_model.mean_occupation(prim_haloprop = 1.e13)
 
         Notes
         -----
         Assumes constant scatter in the stellar-to-halo-mass relation.
         """
         # Retrieve the array storing the mass-like variable
-        if 'table' in list(kwargs.keys()):
-            mass = kwargs['table'][self.prim_haloprop_key]
-        elif 'prim_haloprop' in list(kwargs.keys()):
-            mass = np.atleast_1d(kwargs['prim_haloprop'])
+        if "table" in list(kwargs.keys()):
+            mass = kwargs["table"][self.prim_haloprop_key]
+        elif "prim_haloprop" in list(kwargs.keys()):
+            mass = np.atleast_1d(kwargs["prim_haloprop"])
         else:
             function_name = "Tinker13QuiescentSats.mean_occupation"
             raise HalotoolsError(function_name)
 
         self._update_satellite_params()
 
-        power_law_factor = (mass*self.littleh/self._msat)**self.param_dict['alphasat_quiescent']
+        power_law_factor = (mass * self.littleh / self._msat) ** self.param_dict[
+            "alphasat_quiescent"
+        ]
+
+        exp_arg_numerator = self._mcut + 10.0 ** self.smhm_model.mean_log_halo_mass(
+            log_stellar_mass=self.threshold, redshift=self.redshift
+        )
+        exp_factor = np.exp(-exp_arg_numerator / (mass * self.littleh))
 
-        exp_arg_numerator = self._mcut + 10.**self.smhm_model.mean_log_halo_mass(
-            log_stellar_mass=self.threshold, redshift=self.redshift)
-        exp_factor = np.exp(-exp_arg_numerator/(mass*self.littleh))
-
-        mean_nsat = exp_factor*power_law_factor
+        mean_nsat = exp_factor * power_law_factor
 
         return mean_nsat
 
     def mc_sfr_designation(self, table, **kwargs):
-        """
-        """
-        table[self.sfr_designation_key][:] = 'quiescent'
+        """ """
+        table[self.sfr_designation_key][:] = "quiescent"
 
     def _initialize_param_dict(self):
-        """ Set the initial values of ``self.param_dict`` according to
+        """Set the initial values of ``self.param_dict`` according to
         the SIG_MOD1 values of Table 5 of arXiv:1104.0928 for the
         lowest redshift bin.
 
         """
 
-        self.param_dict['bcut_quiescent'] = 21.42
-        self.param_dict['bsat_quiescent'] = 17.9
-        self.param_dict['betacut_quiescent'] = -0.12
-        self.param_dict['betasat_quiescent'] = 0.62
-        self.param_dict['alphasat_quiescent'] = 1.08
+        self.param_dict["bcut_quiescent"] = 21.42
+        self.param_dict["bsat_quiescent"] = 17.9
+        self.param_dict["betacut_quiescent"] = -0.12
+        self.param_dict["betasat_quiescent"] = 0.62
+        self.param_dict["alphasat_quiescent"] = 1.08
 
         for key, value in self.smhm_model.param_dict.items():
-            quiescent_key = key + '_quiescent'
+            quiescent_key = key + "_quiescent"
             self.param_dict[quiescent_key] = value
 
-        self.param_dict['smhm_m1_0_quiescent'] = 12.08
-        self.param_dict['smhm_m0_0_quiescent'] = 10.7
-        self.param_dict['smhm_beta_0_quiescent'] = 0.32
-        self.param_dict['smhm_delta_0_quiescent'] = 0.93
-        self.param_dict['smhm_gamma_0_quiescent'] = 0.81
+        self.param_dict["smhm_m1_0_quiescent"] = 12.08
+        self.param_dict["smhm_m0_0_quiescent"] = 10.7
+        self.param_dict["smhm_beta_0_quiescent"] = 0.32
+        self.param_dict["smhm_delta_0_quiescent"] = 0.93
+        self.param_dict["smhm_gamma_0_quiescent"] = 0.81
 
         self._update_satellite_params()
 
     def _update_satellite_params(self):
-        """ Private method to update the model parameters.
-
-        """
+        """Private method to update the model parameters."""
         for key, value in self.param_dict.items():
-            stripped_key = key[:-len('_quiescent')]
+            stripped_key = key[: -len("_quiescent")]
             if stripped_key in self.smhm_model.param_dict:
                 self.smhm_model.param_dict[stripped_key] = value
 
         log_halo_mass_threshold = self.smhm_model.mean_log_halo_mass(
-            log_stellar_mass=self.threshold, redshift=self.redshift)
-        knee_threshold = (10.**log_halo_mass_threshold)*self.littleh
+            log_stellar_mass=self.threshold, redshift=self.redshift
+        )
+        knee_threshold = (10.0**log_halo_mass_threshold) * self.littleh
 
-        knee_mass = 1.e12
+        knee_mass = 1.0e12
 
         self._msat = (
-            knee_mass*self.param_dict['bsat_quiescent'] *
-            (knee_threshold / knee_mass)**self.param_dict['betasat_quiescent'])
+            knee_mass
+            * self.param_dict["bsat_quiescent"]
+            * (knee_threshold / knee_mass) ** self.param_dict["betasat_quiescent"]
+        )
 
         self._mcut = (
-            knee_mass*self.param_dict['bcut_quiescent'] *
-            (knee_threshold / knee_mass)**self.param_dict['betacut_quiescent'])
+            knee_mass
+            * self.param_dict["bcut_quiescent"]
+            * (knee_threshold / knee_mass) ** self.param_dict["betacut_quiescent"]
+        )
 
 
 class Tinker13ActiveSats(OccupationComponent):
-    """ HOD-style model for a central galaxy occupation that derives from
+    """HOD-style model for a central galaxy occupation that derives from
     two distinct active/active stellar-to-halo-mass relations.
 
     .. note::
 
         The `Tinker13ActiveSats` model is part of the ``tinker13``
         prebuilt composite HOD-style model. For a tutorial on the ``tinker13``
         composite model, see :ref:`tinker13_composite_model`.
     """
 
-    def __init__(self, threshold=model_defaults.default_stellar_mass_threshold,
-            prim_haloprop_key=model_defaults.prim_haloprop_key,
-            redshift=sim_manager.sim_defaults.default_redshift, **kwargs):
+    def __init__(
+        self,
+        threshold=model_defaults.default_stellar_mass_threshold,
+        prim_haloprop_key=model_defaults.prim_haloprop_key,
+        redshift=sim_manager.sim_defaults.default_redshift,
+        **kwargs
+    ):
         """
         Parameters
         ----------
         threshold : float, optional
             Stellar mass threshold of the mock galaxy sample in h=1 solar mass units.
             Default value is specified in the `~halotools.empirical_models.model_defaults` module.
 
@@ -565,44 +616,48 @@
         upper_occupation_bound = float("inf")
 
         self.littleh = 0.72
 
         # Call the super class constructor, which binds all the
         # arguments to the instance.
         super(Tinker13ActiveSats, self).__init__(
-            gal_type='active_satellites', threshold=threshold,
+            gal_type="active_satellites",
+            threshold=threshold,
             upper_occupation_bound=upper_occupation_bound,
-            prim_haloprop_key=prim_haloprop_key, **kwargs)
+            prim_haloprop_key=prim_haloprop_key,
+            **kwargs
+        )
         self.redshift = redshift
 
-        self.smhm_model = Behroozi10SmHm(
-            prim_haloprop_key=prim_haloprop_key, **kwargs)
+        self.smhm_model = Behroozi10SmHm(prim_haloprop_key=prim_haloprop_key, **kwargs)
 
         self._initialize_param_dict()
 
-        self.sfr_designation_key = 'sfr_designation'
+        self.sfr_designation_key = "sfr_designation"
 
-        self.publications = ['arXiv:1308.2974', 'arXiv:1103.2077', 'arXiv:1104.0928']
+        self.publications = ["arXiv:1308.2974", "arXiv:1103.2077", "arXiv:1104.0928"]
 
         # The _methods_to_inherit determines which methods will be directly callable
         # by the composite model built by the HodModelFactory
         # Here we are overriding this attribute that is normally defined
         # in the OccupationComponent super class
-        self._methods_to_inherit = ['mc_occupation', 'mean_occupation']
+        self._methods_to_inherit = ["mc_occupation", "mean_occupation"]
 
         # The _mock_generation_calling_sequence determines which methods
         # will be called during mock population, as well as in what order they will be called
-        self._mock_generation_calling_sequence = ['mc_occupation', 'mc_sfr_designation']
-        self._galprop_dtypes_to_allocate = np.dtype([
-            ('halo_num_' + self.gal_type, 'i4'),
-            (self.sfr_designation_key, object),
-            ])
+        self._mock_generation_calling_sequence = ["mc_occupation", "mc_sfr_designation"]
+        self._galprop_dtypes_to_allocate = np.dtype(
+            [
+                ("halo_num_" + self.gal_type, "i4"),
+                (self.sfr_designation_key, object),
+            ]
+        )
 
     def mean_occupation(self, **kwargs):
-        """ Expected number of central galaxies in a halo of mass halo_mass.
+        """Expected number of central galaxies in a halo of mass halo_mass.
         See Equation 12-14 of arXiv:1103.2077.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             array of masses of table in the catalog
 
@@ -620,77 +675,82 @@
         >>> mean_nsat = sat_model.mean_occupation(prim_haloprop = 1.e13)
 
         Notes
         -----
         Assumes constant scatter in the stellar-to-halo-mass relation.
         """
         # Retrieve the array storing the mass-like variable
-        if 'table' in list(kwargs.keys()):
-            mass = kwargs['table'][self.prim_haloprop_key]
-        elif 'prim_haloprop' in list(kwargs.keys()):
-            mass = np.atleast_1d(kwargs['prim_haloprop'])
+        if "table" in list(kwargs.keys()):
+            mass = kwargs["table"][self.prim_haloprop_key]
+        elif "prim_haloprop" in list(kwargs.keys()):
+            mass = np.atleast_1d(kwargs["prim_haloprop"])
         else:
             function_name = "Tinker13ActiveSats.mean_occupation"
             raise HalotoolsError(function_name)
 
         self._update_satellite_params()
 
-        power_law_factor = (mass*self.littleh/self._msat)**self.param_dict['alphasat_active']
-
-        exp_arg_numerator = self._mcut + 10.**self.smhm_model.mean_log_halo_mass(
-            log_stellar_mass=self.threshold, redshift=self.redshift)
-        exp_factor = np.exp(-exp_arg_numerator/(mass*self.littleh))
+        power_law_factor = (mass * self.littleh / self._msat) ** self.param_dict[
+            "alphasat_active"
+        ]
+
+        exp_arg_numerator = self._mcut + 10.0 ** self.smhm_model.mean_log_halo_mass(
+            log_stellar_mass=self.threshold, redshift=self.redshift
+        )
+        exp_factor = np.exp(-exp_arg_numerator / (mass * self.littleh))
 
-        mean_nsat = exp_factor*power_law_factor
+        mean_nsat = exp_factor * power_law_factor
 
         return mean_nsat
 
     def mc_sfr_designation(self, table, **kwargs):
-        """
-        """
-        table[self.sfr_designation_key][:] = 'active'
+        """ """
+        table[self.sfr_designation_key][:] = "active"
 
     def _initialize_param_dict(self):
-        """ Set the initial values of ``self.param_dict`` according to
+        """Set the initial values of ``self.param_dict`` according to
         the z1 values of Table 2 of arXiv:1308.2974.
         """
 
-        self.param_dict['bcut_active'] = 0.28
-        self.param_dict['bsat_active'] = 33.96
-        self.param_dict['betacut_active'] = 0.77
-        self.param_dict['betasat_active'] = 1.05
-        self.param_dict['alphasat_active'] = 0.99
+        self.param_dict["bcut_active"] = 0.28
+        self.param_dict["bsat_active"] = 33.96
+        self.param_dict["betacut_active"] = 0.77
+        self.param_dict["betasat_active"] = 1.05
+        self.param_dict["alphasat_active"] = 0.99
 
         for key, value in self.smhm_model.param_dict.items():
-            active_key = key + '_active'
+            active_key = key + "_active"
             self.param_dict[active_key] = value
 
-        self.param_dict['smhm_m1_0_active'] = 12.56
-        self.param_dict['smhm_m0_0_active'] = 10.96
-        self.param_dict['smhm_beta_0_active'] = 0.44
-        self.param_dict['smhm_delta_0_active'] = 0.52
-        self.param_dict['smhm_gamma_0_active'] = 1.48
+        self.param_dict["smhm_m1_0_active"] = 12.56
+        self.param_dict["smhm_m0_0_active"] = 10.96
+        self.param_dict["smhm_beta_0_active"] = 0.44
+        self.param_dict["smhm_delta_0_active"] = 0.52
+        self.param_dict["smhm_gamma_0_active"] = 1.48
 
         self._update_satellite_params()
 
     def _update_satellite_params(self):
-        """ Private method to update the model parameters.
-
-        """
+        """Private method to update the model parameters."""
         for key, value in self.param_dict.items():
-            stripped_key = key[:-len('_active')]
+            stripped_key = key[: -len("_active")]
             if stripped_key in self.smhm_model.param_dict:
                 self.smhm_model.param_dict[stripped_key] = value
 
         log_halo_mass_threshold = self.smhm_model.mean_log_halo_mass(
-            log_stellar_mass=self.threshold, redshift=self.redshift)
-        knee_threshold = (10.**log_halo_mass_threshold)*self.littleh
+            log_stellar_mass=self.threshold, redshift=self.redshift
+        )
+        knee_threshold = (10.0**log_halo_mass_threshold) * self.littleh
 
-        knee_mass = 1.e12
+        knee_mass = 1.0e12
 
         self._msat = (
-            knee_mass*self.param_dict['bsat_active'] *
-            (knee_threshold / knee_mass)**self.param_dict['betasat_active'])
+            knee_mass
+            * self.param_dict["bsat_active"]
+            * (knee_threshold / knee_mass) ** self.param_dict["betasat_active"]
+        )
 
         self._mcut = (
-            knee_mass*self.param_dict['bcut_active'] *
-            (knee_threshold / knee_mass)**self.param_dict['betacut_active'])
+            knee_mass
+            * self.param_dict["bcut_active"]
+            * (knee_threshold / knee_mass) ** self.param_dict["betacut_active"]
+        )
```

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/zheng07_components.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/zheng07_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,36 +9,43 @@
 from .occupation_model_template import OccupationComponent
 
 from .. import model_defaults
 from ..assembias_models import HeavisideAssembias, PreservingNgalHeavisideAssembias
 
 from ...custom_exceptions import HalotoolsError
 
-__all__ = ('Zheng07Cens', 'Zheng07Sats',
-           'AssembiasZheng07Cens', 'AssembiasZheng07Sats',
-           'PreservingNgalAssembiasZheng07Cens', 'PreservingNgalAssembiasZheng07Sats')
+__all__ = (
+    "Zheng07Cens",
+    "Zheng07Sats",
+    "AssembiasZheng07Cens",
+    "AssembiasZheng07Sats",
+    "PreservingNgalAssembiasZheng07Cens",
+    "PreservingNgalAssembiasZheng07Sats",
+)
 
 
 class Zheng07Cens(OccupationComponent):
-    r""" ``Erf`` function model for the occupation statistics of central galaxies,
+    r"""``Erf`` function model for the occupation statistics of central galaxies,
     introduced in Zheng et al. 2005, arXiv:0408564. This implementation uses
     Zheng et al. 2007, arXiv:0703457, to assign fiducial parameter values.
 
     .. note::
 
         The `Zheng07Cens` model is part of the ``zheng07``
         prebuilt composite HOD-style model. For a tutorial on the ``zheng07``
         composite model, see :ref:`zheng07_composite_model`.
 
     """
 
-    def __init__(self,
-            threshold=model_defaults.default_luminosity_threshold,
-            prim_haloprop_key=model_defaults.prim_haloprop_key,
-            **kwargs):
+    def __init__(
+        self,
+        threshold=model_defaults.default_luminosity_threshold,
+        prim_haloprop_key=model_defaults.prim_haloprop_key,
+        **kwargs
+    ):
         r"""
         Parameters
         ----------
         threshold : float, optional
             Luminosity threshold of the mock galaxy sample. If specified,
             input value must agree with one of the thresholds used in Zheng07 to fit HODs:
             [-18, -18.5, -19, -19.5, -20, -20.5, -21, -21.5, -22].
@@ -61,25 +68,28 @@
 
         :ref:`zheng07_using_cenocc_model_tutorial`
         """
         upper_occupation_bound = 1.0
 
         # Call the super class constructor, which binds all the
         # arguments to the instance.
-        super(Zheng07Cens, self).__init__(gal_type='centrals',
-            threshold=threshold, upper_occupation_bound=upper_occupation_bound,
+        super(Zheng07Cens, self).__init__(
+            gal_type="centrals",
+            threshold=threshold,
+            upper_occupation_bound=upper_occupation_bound,
             prim_haloprop_key=prim_haloprop_key,
-            **kwargs)
+            **kwargs
+        )
 
         self.param_dict = self.get_published_parameters(self.threshold)
 
-        self.publications = ['arXiv:0408564', 'arXiv:0703457']
+        self.publications = ["arXiv:0408564", "arXiv:0703457"]
 
     def mean_occupation(self, **kwargs):
-        r""" Expected number of central galaxies in a halo of mass halo_mass.
+        r"""Expected number of central galaxies in a halo of mass halo_mass.
         See Equation 2 of arXiv:0703457.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             Array of mass-like variable upon which occupation statistics are based.
             If ``prim_haloprop`` is not passed, then ``table`` keyword argument must be passed.
@@ -121,30 +131,34 @@
         :math:`\langle N_{\mathrm{cen}} \rangle_{M} =
         \frac{1}{2}\left( 1 +
         \mathrm{erf}\left( \frac{\log_{10}M -
         \log_{10}M_{min}}{\sigma_{\log_{10}M}} \right) \right)`
 
         """
         # Retrieve the array storing the mass-like variable
-        if 'table' in list(kwargs.keys()):
-            mass = kwargs['table'][self.prim_haloprop_key]
-        elif 'prim_haloprop' in list(kwargs.keys()):
-            mass = np.atleast_1d(kwargs['prim_haloprop'])
+        if "table" in list(kwargs.keys()):
+            mass = kwargs["table"][self.prim_haloprop_key]
+        elif "prim_haloprop" in list(kwargs.keys()):
+            mass = np.atleast_1d(kwargs["prim_haloprop"])
         else:
-            msg = ("\nYou must pass either a ``table`` or ``prim_haloprop`` argument \n"
-                "to the ``mean_occupation`` function of the ``Zheng07Cens`` class.\n")
+            msg = (
+                "\nYou must pass either a ``table`` or ``prim_haloprop`` argument \n"
+                "to the ``mean_occupation`` function of the ``Zheng07Cens`` class.\n"
+            )
             raise HalotoolsError(msg)
 
         logM = np.log10(mass)
-        mean_ncen = 0.5*(1.0 + erf(
-            (logM - self.param_dict['logMmin']) / self.param_dict['sigma_logM']))
+        mean_ncen = 0.5 * (
+            1.0
+            + erf((logM - self.param_dict["logMmin"]) / self.param_dict["sigma_logM"])
+        )
 
         return mean_ncen
 
-    def get_published_parameters(self, threshold, publication='Zheng07'):
+    def get_published_parameters(self, threshold, publication="Zheng07"):
         r"""
         Best-fit HOD parameters from Table 1 of Zheng et al. 2007.
 
         Parameters
         ----------
 
         threshold : float
@@ -169,66 +183,91 @@
         >>> cen_model = Zheng07Cens()
         >>> cen_model.param_dict = cen_model.get_published_parameters(cen_model.threshold)
 
         """
 
         def get_zheng07_params(threshold):
             # Load tabulated data from Zheng et al. 2007, Table 1
-            logMmin_array = [11.35, 11.46, 11.6, 11.75, 12.02, 12.3, 12.79, 13.38, 14.22]
+            logMmin_array = [
+                11.35,
+                11.46,
+                11.6,
+                11.75,
+                12.02,
+                12.3,
+                12.79,
+                13.38,
+                14.22,
+            ]
             sigma_logM_array = [0.25, 0.24, 0.26, 0.28, 0.26, 0.21, 0.39, 0.51, 0.77]
             # define the luminosity thresholds corresponding to the above data
             threshold_array = np.arange(-22, -17.5, 0.5)
             threshold_array = threshold_array[::-1]
 
             threshold_index = np.where(threshold_array == threshold)[0]
             if len(threshold_index) == 0:
-                msg = ("\nInput luminosity threshold "
+                msg = (
+                    "\nInput luminosity threshold "
                     "does not match any of the Table 1 values \nof "
                     "Zheng et al. 2007 (arXiv:0703457).\n"
                     "Choosing the best-fit parameters "
                     "associated the default_luminosity_threshold variable \n"
                     "set in the model_defaults module.\n"
-                    "You can always manually change the values in ``param_dict``.\n")
+                    "You can always manually change the values in ``param_dict``.\n"
+                )
                 warnings.warn(msg)
                 threshold = model_defaults.default_luminosity_threshold
                 threshold_index = np.where(threshold_array == threshold)[0]
 
-            param_dict = (
-                {'logMmin': logMmin_array[threshold_index[0]],
-                'sigma_logM': sigma_logM_array[threshold_index[0]]}
-                )
+            param_dict = {
+                "logMmin": logMmin_array[threshold_index[0]],
+                "sigma_logM": sigma_logM_array[threshold_index[0]],
+            }
 
             return param_dict
 
-        if publication in ['zheng07', 'Zheng07', 'Zheng_etal07', 'zheng_etal07', 'zheng2007', 'Zheng2007']:
+        if publication in [
+            "zheng07",
+            "Zheng07",
+            "Zheng_etal07",
+            "zheng_etal07",
+            "zheng2007",
+            "Zheng2007",
+        ]:
             param_dict = get_zheng07_params(threshold)
             return param_dict
         else:
-            raise KeyError("For Zheng07Cens, only supported best-fit models are currently Zheng et al. 2007")
+            raise KeyError(
+                "For Zheng07Cens, only supported best-fit models are currently Zheng et al. 2007"
+            )
 
 
 class Zheng07Sats(OccupationComponent):
-    r""" Power law model for the occupation statistics of satellite galaxies,
+    r"""Power law model for the occupation statistics of satellite galaxies,
     introduced in Kravtsov et al. 2004, arXiv:0308519. This implementation uses
     Zheng et al. 2007, arXiv:0703457, to assign fiducial parameter values.
 
     :math:`\langle N_{sat} \rangle_{M} = \left( \frac{M - M_{0}}{M_{1}} \right)^{\alpha}`.
 
     .. note::
 
         The `Zheng07Sats` model is part of the ``zheng07``
         prebuilt composite HOD-style model. For a tutorial on the ``zheng07``
         composite model, see :ref:`zheng07_composite_model`.
 
     """
 
-    def __init__(self,
-            threshold=model_defaults.default_luminosity_threshold,
-            prim_haloprop_key=model_defaults.prim_haloprop_key,
-            modulate_with_cenocc=False, cenocc_model=None, **kwargs):
+    def __init__(
+        self,
+        threshold=model_defaults.default_luminosity_threshold,
+        prim_haloprop_key=model_defaults.prim_haloprop_key,
+        modulate_with_cenocc=False,
+        cenocc_model=None,
+        **kwargs
+    ):
         r"""
         Parameters
         ----------
         threshold : float, optional
             Luminosity threshold of the mock galaxy sample. If specified,
             input value must agree with one of the thresholds used in Zheng07 to fit HODs:
             [-18, -18.5, -19, -19.5, -20, -20.5, -21, -21.5, -22].
@@ -300,47 +339,54 @@
 
         """
         upper_occupation_bound = float("inf")
 
         # Call the super class constructor, which binds all the
         # arguments to the instance.
         super(Zheng07Sats, self).__init__(
-            gal_type='satellites', threshold=threshold,
+            gal_type="satellites",
+            threshold=threshold,
             upper_occupation_bound=upper_occupation_bound,
             prim_haloprop_key=prim_haloprop_key,
-            **kwargs)
+            **kwargs
+        )
 
         self.param_dict = self.get_published_parameters(self.threshold)
 
         if cenocc_model is None:
             cenocc_model = Zheng07Cens(
-                prim_haloprop_key=prim_haloprop_key, threshold=threshold)
+                prim_haloprop_key=prim_haloprop_key, threshold=threshold
+            )
         else:
             if modulate_with_cenocc is False:
-                msg = ("You chose to input a ``cenocc_model``, but you set the \n"
+                msg = (
+                    "You chose to input a ``cenocc_model``, but you set the \n"
                     "``modulate_with_cenocc`` keyword to False, so your "
                     "``cenocc_model`` will have no impact on the model's behavior.\n"
                     "Be sure this is what you intend before proceeding.\n"
-                    "Refer to the Zheng et al. (2007) composite model tutorial for details.\n")
+                    "Refer to the Zheng et al. (2007) composite model tutorial for details.\n"
+                )
                 warnings.warn(msg)
 
         self.modulate_with_cenocc = modulate_with_cenocc
         if self.modulate_with_cenocc:
             try:
                 assert isinstance(cenocc_model, OccupationComponent)
             except AssertionError:
-                msg = ("The input ``cenocc_model`` must be an instance of \n"
-                    "``OccupationComponent`` or one of its sub-classes.\n")
+                msg = (
+                    "The input ``cenocc_model`` must be an instance of \n"
+                    "``OccupationComponent`` or one of its sub-classes.\n"
+                )
                 raise HalotoolsError(msg)
 
             self.central_occupation_model = cenocc_model
 
             self.param_dict.update(self.central_occupation_model.param_dict)
 
-        self.publications = ['arXiv:0308519', 'arXiv:0703457']
+        self.publications = ["arXiv:0308519", "arXiv:0703457"]
 
     def mean_occupation(self, **kwargs):
         r"""Expected number of satellite galaxies in a halo of mass logM.
         See Equation 5 of arXiv:0703457.
 
         Parameters
         ----------
@@ -391,49 +437,56 @@
 
         if self.modulate_with_cenocc:
             for key, value in self.param_dict.items():
                 if key in self.central_occupation_model.param_dict:
                     self.central_occupation_model.param_dict[key] = value
 
         # Retrieve the array storing the mass-like variable
-        if 'table' in list(kwargs.keys()):
-            mass = kwargs['table'][self.prim_haloprop_key]
-        elif 'prim_haloprop' in list(kwargs.keys()):
-            mass = np.atleast_1d(kwargs['prim_haloprop'])
+        if "table" in list(kwargs.keys()):
+            mass = kwargs["table"][self.prim_haloprop_key]
+        elif "prim_haloprop" in list(kwargs.keys()):
+            mass = np.atleast_1d(kwargs["prim_haloprop"])
         else:
-            msg = ("\nYou must pass either a ``table`` or ``prim_haloprop`` argument \n"
-                "to the ``mean_occupation`` function of the ``Zheng07Sats`` class.\n")
+            msg = (
+                "\nYou must pass either a ``table`` or ``prim_haloprop`` argument \n"
+                "to the ``mean_occupation`` function of the ``Zheng07Sats`` class.\n"
+            )
             raise HalotoolsError(msg)
 
-        M0 = 10.**self.param_dict['logM0']
-        M1 = 10.**self.param_dict['logM1']
+        M0 = 10.0 ** self.param_dict["logM0"]
+        M1 = 10.0 ** self.param_dict["logM1"]
 
         # Call to np.where raises a harmless RuntimeWarning exception if
         # there are entries of input logM for which mean_nsat = 0
         # Evaluating mean_nsat using the catch_warnings context manager
         # suppresses this warning
         mean_nsat = np.zeros_like(mass)
 
         idx_nonzero = np.where(mass - M0 > 0)[0]
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", RuntimeWarning)
 
-            mean_nsat[idx_nonzero] = ((mass[idx_nonzero] - M0)/M1)**self.param_dict['alpha']
+            mean_nsat[idx_nonzero] = ((mass[idx_nonzero] - M0) / M1) ** self.param_dict[
+                "alpha"
+            ]
 
         # If a central occupation model was passed to the constructor,
         # multiply mean_nsat by an overall factor of mean_ncen
         if self.modulate_with_cenocc:
             # compatible with AB models
-            mean_ncen = getattr(self.central_occupation_model, "baseline_mean_occupation",\
-                                    self.central_occupation_model.mean_occupation)(**kwargs)
+            mean_ncen = getattr(
+                self.central_occupation_model,
+                "baseline_mean_occupation",
+                self.central_occupation_model.mean_occupation,
+            )(**kwargs)
             mean_nsat *= mean_ncen
 
         return mean_nsat
 
-    def get_published_parameters(self, threshold, publication='Zheng07'):
+    def get_published_parameters(self, threshold, publication="Zheng07"):
         r"""
         Best-fit HOD parameters from Table 1 of Zheng et al. 2007.
 
         Parameters
         ----------
         threshold : float
             Luminosity threshold of the mock galaxy sample.
@@ -464,43 +517,53 @@
             # define the luminosity thresholds corresponding to the above data
             threshold_array = np.arange(-22, -17.5, 0.5)
             threshold_array = threshold_array[::-1]
 
             threshold_index = np.where(threshold_array == threshold)[0]
 
             if len(threshold_index) == 0:
-                msg = ("\nInput luminosity threshold "
+                msg = (
+                    "\nInput luminosity threshold "
                     "does not match any of the Table 1 values \nof "
                     "Zheng et al. 2007 (arXiv:0703457).\n"
                     "Choosing the best-fit parameters "
                     "associated the default_luminosity_threshold variable \n"
                     "set in the model_defaults module.\n"
-                    "You can always manually change the values in ``param_dict``.\n")
+                    "You can always manually change the values in ``param_dict``.\n"
+                )
                 warnings.warn(msg)
                 threshold = model_defaults.default_luminosity_threshold
                 threshold_index = np.where(threshold_array == threshold)[0]
                 warnings.warn(msg)
 
-            param_dict = (
-                {'logM0': logM0_array[threshold_index[0]],
-                'logM1': logM1_array[threshold_index[0]],
-                'alpha': alpha_array[threshold_index[0]]}
-                )
+            param_dict = {
+                "logM0": logM0_array[threshold_index[0]],
+                "logM1": logM1_array[threshold_index[0]],
+                "alpha": alpha_array[threshold_index[0]],
+            }
             return param_dict
 
-        if publication in ['zheng07', 'Zheng07', 'Zheng_etal07', 'zheng_etal07', 'zheng2007', 'Zheng2007']:
+        if publication in [
+            "zheng07",
+            "Zheng07",
+            "Zheng_etal07",
+            "zheng_etal07",
+            "zheng2007",
+            "Zheng2007",
+        ]:
             param_dict = get_zheng07_params(threshold)
             return param_dict
         else:
-            raise KeyError("For Zheng07Sats, only supported best-fit models are currently Zheng et al. 2007")
+            raise KeyError(
+                "For Zheng07Sats, only supported best-fit models are currently Zheng et al. 2007"
+            )
 
 
 class AssembiasZheng07Sats(Zheng07Sats, HeavisideAssembias):
-    r""" Assembly-biased modulation of `Zheng07Sats`.
-    """
+    r"""Assembly-biased modulation of `Zheng07Sats`."""
 
     def __init__(self, **kwargs):
         r"""
         Parameters
         ----------
         threshold : float, optional
             Luminosity threshold of the mock galaxy sample. If specified,
@@ -540,24 +603,25 @@
             Values of the primary halo property at which the assembly bias strength is specified.
             Default is to assume a constant strength of 0.5. If passing a list, the strength
             will interpreted at the input ``assembias_strength_abscissa``.
             Default is to assume a constant strength of 0.5.
 
         """
         Zheng07Sats.__init__(self, **kwargs)
-        HeavisideAssembias.__init__(self,
-            method_name_to_decorate='mean_occupation',
+        HeavisideAssembias.__init__(
+            self,
+            method_name_to_decorate="mean_occupation",
             lower_assembias_bound=self._lower_occupation_bound,
             upper_assembias_bound=self._upper_occupation_bound,
-            **kwargs)
+            **kwargs
+        )
 
 
 class AssembiasZheng07Cens(Zheng07Cens, HeavisideAssembias):
-    r""" Assembly-biased modulation of `Zheng07Cens`.
-    """
+    r"""Assembly-biased modulation of `Zheng07Cens`."""
 
     def __init__(self, **kwargs):
         r"""
         Parameters
         ----------
         threshold : float, optional
             Luminosity threshold of the mock galaxy sample. If specified,
@@ -597,24 +661,25 @@
             Values of the primary halo property at which the assembly bias strength is specified.
             Default is to assume a constant strength of 0.5. If passing a list, the strength
             will interpreted at the input ``assembias_strength_abscissa``.
             Default is to assume a constant strength of 0.5.
 
         """
         Zheng07Cens.__init__(self, **kwargs)
-        HeavisideAssembias.__init__(self,
+        HeavisideAssembias.__init__(
+            self,
             lower_assembias_bound=self._lower_occupation_bound,
             upper_assembias_bound=self._upper_occupation_bound,
-            method_name_to_decorate='mean_occupation', **kwargs)
-
+            method_name_to_decorate="mean_occupation",
+            **kwargs
+        )
 
 
 class PreservingNgalAssembiasZheng07Sats(Zheng07Sats, PreservingNgalHeavisideAssembias):
-    r""" Assembly-biased modulation of `Zheng07Sats` that preserves N_gals.
-    """
+    r"""Assembly-biased modulation of `Zheng07Sats` that preserves N_gals."""
 
     def __init__(self, **kwargs):
         r"""
         Parameters
         ----------
         threshold : float, optional
             Luminosity threshold of the mock galaxy sample. If specified,
@@ -654,24 +719,25 @@
             Values of the primary halo property at which the assembly bias strength is specified.
             Default is to assume a constant strength of 0.5. If passing a list, the strength
             will interpreted at the input ``assembias_strength_abscissa``.
             Default is to assume a constant strength of 0.5.
 
         """
         Zheng07Sats.__init__(self, **kwargs)
-        PreservingNgalHeavisideAssembias.__init__(self,
-            method_name_to_decorate='mean_occupation',
+        PreservingNgalHeavisideAssembias.__init__(
+            self,
+            method_name_to_decorate="mean_occupation",
             lower_assembias_bound=self._lower_occupation_bound,
             upper_assembias_bound=self._upper_occupation_bound,
-            **kwargs)
+            **kwargs
+        )
 
 
 class PreservingNgalAssembiasZheng07Cens(Zheng07Cens, PreservingNgalHeavisideAssembias):
-    r""" Assembly-biased modulation of `Zheng07Cens` that preserves N_gals.
-    """
+    r"""Assembly-biased modulation of `Zheng07Cens` that preserves N_gals."""
 
     def __init__(self, **kwargs):
         r"""
         Parameters
         ----------
         threshold : float, optional
             Luminosity threshold of the mock galaxy sample. If specified,
@@ -711,11 +777,14 @@
             Values of the primary halo property at which the assembly bias strength is specified.
             Default is to assume a constant strength of 0.5. If passing a list, the strength
             will interpreted at the input ``assembias_strength_abscissa``.
             Default is to assume a constant strength of 0.5.
 
         """
         Zheng07Cens.__init__(self, **kwargs)
-        PreservingNgalHeavisideAssembias.__init__(self,
+        PreservingNgalHeavisideAssembias.__init__(
+            self,
             lower_assembias_bound=self._lower_occupation_bound,
             upper_assembias_bound=self._upper_occupation_bound,
-            method_name_to_decorate='mean_occupation', **kwargs)
+            method_name_to_decorate="mean_occupation",
+            **kwargs
+        )
```

### Comparing `halotools-0.8.1/halotools/empirical_models/occupation_models/zu_mandelbaum15_components.py` & `halotools-0.8.2/halotools/empirical_models/occupation_models/zu_mandelbaum15_components.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             raise KeyError(
                 "Must pass one of the following keyword arguments "
                 "to mean_occupation:\n``table`` or ``prim_haloprop``"
             )
 
         sigma = self.smhm_model.scatter_ln_mstar(halo_mass)
         mean = self.smhm_model.mean_stellar_mass(prim_haloprop=halo_mass)
-        erfarg = (np.log(10 ** self.threshold) - np.log(mean)) / (sigma * np.sqrt(2))
+        erfarg = (np.log(10**self.threshold) - np.log(mean)) / (sigma * np.sqrt(2))
         return 0.5 * (1 - erf(erfarg))
 
     def mean_stellar_mass(self, **kwargs):
         """Return the stellar mass of a central galaxy as a function
         of the input table.
 
         Parameters
@@ -326,15 +326,15 @@
     def _update_satellite_params(self):
         """Private method to update the model parameters."""
         for key, value in self.param_dict.items():
             if key in self.central_occupation_model.param_dict:
                 self.central_occupation_model.param_dict[key] = value
 
         knee_threshold = self.central_occupation_model.mean_halo_mass(
-            10 ** self.threshold
+            10**self.threshold
         )
         knee_mass = 1.0e12
 
         self._msat = (
             knee_mass
             * self.param_dict["bsat"]
             * (knee_threshold / knee_mass) ** self.param_dict["betasat"]
```

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/centrals/tests/test_trivial_profile.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/centrals/tests/test_trivial_profile.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/centrals/trivial_phase_space.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/centrals/trivial_phase_space.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/centrals/trivial_profile.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/centrals/trivial_profile.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/halo_boundary_functions.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/halo_boundary_functions.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/monte_carlo_helpers.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/monte_carlo_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/profile_model_template.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/profile_model_template.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/biased_nfw_phase_space.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/biased_nfw_phase_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "one entry for every numerical solution to the Jeans equation.\n"
     "Using this fine of a binning requires a long pre-computation of {3} integrals\n."
     "Make sure you actually need to use so many bins"
 )
 
 
 class BiasedNFWPhaseSpace(NFWPhaseSpace):
-    r""" Model for the phase space distribution of galaxies
+    r"""Model for the phase space distribution of galaxies
     in isotropic Jeans equilibrium in an NFW halo profile,
     based on Navarro, Frenk and White (1995),
     where the concentration of the tracers is permitted to differ from the
     host halo concentration.
 
     For a review of the mathematics underlying the NFW profile,
     including descriptions of how the relevant equations are
@@ -172,15 +172,15 @@
                 ("conc_galaxy", "f8"),
             ]
         )
 
         self.param_dict = self._initialize_conc_bias_param_dict(**kwargs)
 
     def _initialize_conc_bias_param_dict(self, **kwargs):
-        r""" Set up the appropriate number of keys in the parameter dictionary
+        r"""Set up the appropriate number of keys in the parameter dictionary
         and give the keys standardized names.
         """
         if "conc_gal_bias_logM_abscissa" in list(kwargs.keys()):
             _conc_bias_logM_abscissa = np.atleast_1d(
                 kwargs.get("conc_gal_bias_logM_abscissa")
             ).astype("f4")
             d = {
@@ -196,16 +196,15 @@
                 d[key] = value
             return d
 
         else:
             return {"conc_gal_bias": 1.0}
 
     def _retrieve_prof_lookup_info(self, **kwargs):
-        r""" Retrieve the arrays defining the lookup table control points
-        """
+        r"""Retrieve the arrays defining the lookup table control points"""
         cmin, cmax = (
             model_defaults.min_permitted_conc,
             model_defaults.max_permitted_conc,
         )
         dc = 1.0
         npts_conc = int(np.round((cmax - cmin) / float(dc)))
         default_conc_arr = np.linspace(cmin, cmax, npts_conc)
@@ -224,15 +223,15 @@
                 npts_conc * npts_gal_bias * model_defaults.Npts_radius_table,
             )
             warn(lookup_table_performance_warning.format(*args))
 
         return [conc_arr, conc_gal_bias_arr]
 
     def conc_NFWmodel(self, **kwargs):
-        r""" NFW concentration as a function of halo mass.
+        r"""NFW concentration as a function of halo mass.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             Array storing the mass-like variable, e.g., ``halo_mvir``.
 
             If ``prim_haloprop`` is not passed,
@@ -257,15 +256,15 @@
             values set in the `~halotools.empirical_models.model_defaults module`.
             For unclipped concentrations, set these variables to -np.inf, +np.inf.
 
         """
         return NFWPhaseSpace.conc_NFWmodel(self, **kwargs)
 
     def _clipped_galaxy_concentration(self, halo_conc, conc_gal_bias):
-        r""" Private method used to ensure that biased concentrations are still
+        r"""Private method used to ensure that biased concentrations are still
         bound by the min/max bounds permitted by the lookup tables.
         """
         gal_conc = conc_gal_bias * halo_conc
 
         try:
             cmin = self._conc_NFWmodel_lookup_table_min
             cmax = self._conc_NFWmodel_lookup_table_max
@@ -275,15 +274,15 @@
 
         # Now clip the galaxy concentration as necessary
         gal_conc = np.where(gal_conc < cmin, cmin, gal_conc)
         gal_conc = np.where(gal_conc > cmax, cmax, gal_conc)
         return gal_conc
 
     def cumulative_gal_PDF(self, scaled_radius, halo_conc, conc_gal_bias):
-        r""" Analogous to `cumulative_mass_PDF`, but for the satellite galaxy distribution
+        r"""Analogous to `cumulative_mass_PDF`, but for the satellite galaxy distribution
         instead of the host halo mass distribution.
 
         Parameters
         -------------
         scaled_radius : array_like
             Halo-centric distance *r* scaled by the halo boundary :math:`R_{\Delta}`, so that
             :math:`0 <= \tilde{r} \equiv r/R_{\Delta} <= 1`. Can be a scalar or numpy array.
@@ -433,15 +432,15 @@
 
         dimensionless_velocities = self.dimensionless_radial_velocity_dispersion(
             scaled_radius, halo_conc, conc_gal_bias
         )
         return dimensionless_velocities * virial_velocities
 
     def calculate_conc_gal_bias(self, seed=None, **kwargs):
-        r""" Calculate the ratio of the galaxy concentration to the halo concentration,
+        r"""Calculate the ratio of the galaxy concentration to the halo concentration,
         :math:`c_{\rm gal}/c_{\rm halo}`.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             Array storing the mass-like variable, e.g., ``halo_mvir``.
```

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/direct_from_halo_catalog.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/direct_from_halo_catalog.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 """
 from __future__ import division, print_function, absolute_import, unicode_literals
 
-__all__ = ('direct_from_halo_catalog', )
+__all__ = ("direct_from_halo_catalog",)
 
 
 def direct_from_halo_catalog(**kwargs):
     """
     Function returns the concentrations that are already present
     in an input halo catalog.
 
@@ -20,24 +20,28 @@
 
     Returns
     -------
     concentration : array_like
         Concentrations of the input halos.
     """
     try:
-        table = kwargs['table']
-        concentration_key = kwargs['concentration_key']
+        table = kwargs["table"]
+        concentration_key = kwargs["concentration_key"]
     except KeyError:
-        msg = ("The ``direct_from_halo_catalog`` function accepts two keyword arguments:\n"
-            "``table`` and ``concentration_key``")
+        msg = (
+            "The ``direct_from_halo_catalog`` function accepts two keyword arguments:\n"
+            "``table`` and ``concentration_key``"
+        )
         raise KeyError(msg)
 
     try:
         concentration = table[concentration_key]
     except:
-        msg = ("The ``{0}`` key does not appear in the input halo catalog.\n"
+        msg = (
+            "The ``{0}`` key does not appear in the input halo catalog.\n"
             "However, you have selected the ``direct_from_halo_catalog`` option \n"
             "to model the concentration-mass relation.\n"
-            "The available keys are:\n\n{1}\n")
+            "The available keys are:\n\n{1}\n"
+        )
         raise KeyError(msg.format(concentration_key, list(table.keys())))
 
     return concentration
```

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/dutton_maccio14.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/dutton_maccio14.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 """
 from __future__ import division, print_function, absolute_import, unicode_literals
 
 import numpy as np
 
 
-__all__ = ('dutton_maccio14', )
+__all__ = ("dutton_maccio14",)
 
 
 def dutton_maccio14(mass, redshift):
-    r""" Power-law fit to the concentration-mass relation from
+    r"""Power-law fit to the concentration-mass relation from
     Equations 12 & 13 of Dutton and Maccio 2014, arXiv:1402.7073.
 
     :math:`\log_{10}c(M, z) \equiv a + b\log_{10}(M / M_{0}),`
 
     where :math:`a, b, M_{0}` are defined as follows:
 
     :math:`a = 0.537 + (1.025 - 0.537)\exp(-0.718z^{1.08})`
@@ -41,11 +41,11 @@
     --------
     >>> c = dutton_maccio14(1e12, 0)
     >>> c = dutton_maccio14(np.logspace(11, 15, 100), 0)
     """
 
     a = 0.537 + (1.025 - 0.537) * np.exp(-0.718 * redshift**1.08)
     b = -0.097 + 0.024 * redshift
-    m0 = 1.e12
+    m0 = 1.0e12
 
     logc = a + b * np.log10(mass / m0)
     return 10**logc
```

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/tests/test_conc_mass.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/conc_mass/tests/test_conc_mass.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/__init__.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """
 """
 from .mass_profile import cumulative_mass_PDF as nfw_cumulative_mass_PDF
 from .mass_profile import dimensionless_mass_density as nfw_dimensionless_mass_density
-from .unbiased_isotropic_velocity import (dimensionless_radial_velocity_dispersion as
-    unbiased_dimless_vrad_disp)
-from .mc_generate_nfw_radial_positions import (mc_generate_nfw_radial_positions as
-    standalone_mc_generate_nfw_radial_positions)
+from .unbiased_isotropic_velocity import (
+    dimensionless_radial_velocity_dispersion as unbiased_dimless_vrad_disp,
+)
+from .mc_generate_nfw_radial_positions import (
+    mc_generate_nfw_radial_positions as standalone_mc_generate_nfw_radial_positions,
+)
 
-from .biased_isotropic_velocity import (dimensionless_radial_velocity_dispersion as
-    biased_dimless_vrad_disp)
+from .biased_isotropic_velocity import (
+    dimensionless_radial_velocity_dispersion as biased_dimless_vrad_disp,
+)
```

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/biased_isotropic_velocity.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/biased_isotropic_velocity.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,36 +2,35 @@
 """
 import numpy as np
 from scipy.integrate import quad as quad_integration
 
 from .mass_profile import _g_integral
 
 
-__all__ = ('dimensionless_radial_velocity_dispersion', )
+__all__ = ("dimensionless_radial_velocity_dispersion",)
 
 
 def _jeans_integrand_term1(y, *args):
-    r""" First term in the Jeans integrand
-    """
+    r"""First term in the Jeans integrand"""
     bias_ratio = args[0]  # = halo_conc/gal_conc
-    return np.log(1+bias_ratio*y)/(y**3*(1+y)**2)
+    return np.log(1 + bias_ratio * y) / (y**3 * (1 + y) ** 2)
 
 
 def _jeans_integrand_term2(y, *args):
-    r""" Second term in the Jeans integrand
-    """
+    r"""Second term in the Jeans integrand"""
     bias_ratio = args[0]  # = halo_conc/gal_conc
 
     numerator = bias_ratio
-    denominator = (y**2) * ((1+y)**2) * (1+bias_ratio*y)
-    return numerator/denominator
+    denominator = (y**2) * ((1 + y) ** 2) * (1 + bias_ratio * y)
+    return numerator / denominator
 
 
-def dimensionless_radial_velocity_dispersion(scaled_radius, halo_conc, gal_conc,
-        profile_integration_tol=1e-4):
+def dimensionless_radial_velocity_dispersion(
+    scaled_radius, halo_conc, gal_conc, profile_integration_tol=1e-4
+):
     r"""
     Analytical solution to the isotropic jeans equation for an NFW potential,
     rendered dimensionless via scaling by the virial velocity.
 
     :math:`\tilde{\sigma}^{2}_{r}(\tilde{r})\equiv\sigma^{2}_{r}(\tilde{r})/V_{\rm vir}^{2} = \frac{c^{2}\tilde{r}(1 + c\tilde{r})^{2}}{g(c)}\int_{c\tilde{r}}^{\infty}{\rm d}y\frac{g(y)}{y^{3}(1 + y)^{2}}`
 
     See :ref:`nfw_jeans_velocity_profile_derivations` for derivations and implementation details.
@@ -51,22 +50,32 @@
     result : array_like
         Radial velocity dispersion profile scaled by the virial velocity.
         The returned result has the same dimension as the input ``scaled_radius``.
     """
     x = np.atleast_1d(scaled_radius).astype(np.float64)
     result = np.zeros_like(x)
 
-    prefactor = gal_conc*gal_conc*x*(1. + gal_conc*x)**2/_g_integral(halo_conc)
-    extra_args = halo_conc/np.atleast_1d(gal_conc).astype('f4')
+    prefactor = (
+        gal_conc * gal_conc * x * (1.0 + gal_conc * x) ** 2 / _g_integral(halo_conc)
+    )
+    extra_args = halo_conc / np.atleast_1d(gal_conc).astype("f4")
 
-    lower_limit = gal_conc*x
+    lower_limit = gal_conc * x
     upper_limit = float("inf")
     for i in range(len(x)):
-        term1, _ = quad_integration(_jeans_integrand_term1,
-            lower_limit[i], upper_limit, epsrel=profile_integration_tol,
-            args=extra_args)
-        term2, _ = quad_integration(_jeans_integrand_term2,
-            lower_limit[i], upper_limit, epsrel=profile_integration_tol,
-            args=extra_args)
+        term1, _ = quad_integration(
+            _jeans_integrand_term1,
+            lower_limit[i],
+            upper_limit,
+            epsrel=profile_integration_tol,
+            args=extra_args,
+        )
+        term2, _ = quad_integration(
+            _jeans_integrand_term2,
+            lower_limit[i],
+            upper_limit,
+            epsrel=profile_integration_tol,
+            args=extra_args,
+        )
         result[i] = term1 - term2
 
-    return np.sqrt(result*prefactor)
+    return np.sqrt(result * prefactor)
```

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/mass_profile.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/mass_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 """
 import numpy as np
 
-__all__ = ('cumulative_mass_PDF', 'dimensionless_mass_density')
+__all__ = ("cumulative_mass_PDF", "dimensionless_mass_density")
 
 
 def _g_integral(x):
-    r""" Convenience function used to evaluate the profile.
+    r"""Convenience function used to evaluate the profile.
 
         :math:`g(x) \equiv \rm{ln}(1+x) - x / (1+x)`
 
     Parameters
     ----------
     x : array_like
 
@@ -21,15 +21,15 @@
     Examples
     --------
     >>> result = _g_integral(1)
     >>> Npts = 25
     >>> result = _g_integral(np.logspace(-1, 1, Npts))
     """
     x = np.atleast_1d(x).astype(np.float64)
-    return np.log(1.0+x) - (x/(1.0+x))
+    return np.log(1.0 + x) - (x / (1.0 + x))
 
 
 def cumulative_mass_PDF(scaled_radius, conc):
     r"""
     Analytical result for the fraction of the total mass
     enclosed within dimensionless radius of an NFW halo,
 
@@ -64,15 +64,15 @@
     >>> conc = 5
     >>> result = cumulative_mass_PDF(scaled_radius, conc)
     >>> concarr = np.linspace(1, 100, Npts)
     >>> result = cumulative_mass_PDF(scaled_radius, concarr)
     """
     scaled_radius = np.where(scaled_radius > 1, 1, scaled_radius)
     scaled_radius = np.where(scaled_radius < 0, 0, scaled_radius)
-    return _g_integral(conc*scaled_radius) / _g_integral(conc)
+    return _g_integral(conc * scaled_radius) / _g_integral(conc)
 
 
 def dimensionless_mass_density(scaled_radius, conc):
     r"""
     Physical density of the NFW halo scaled by the density threshold of the mass definition.
 
     The `dimensionless_mass_density` is defined as
@@ -108,11 +108,10 @@
         Dimensionless density of a dark matter halo
         at the input ``scaled_radius``, normalized by the
         `~halotools.empirical_models.profile_helpers.density_threshold`
         :math:`\rho_{\rm thresh}` for the
         halo mass definition, cosmology, and redshift.
         Result is an array of the dimension as the input ``scaled_radius``.
     """
-    numerator = conc**3/(3.*_g_integral(conc))
-    denominator = conc*scaled_radius*(1 + conc*scaled_radius)**2
-    return numerator/denominator
-
+    numerator = conc**3 / (3.0 * _g_integral(conc))
+    denominator = conc * scaled_radius * (1 + conc * scaled_radius) ** 2
+    return numerator / denominator
```

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/mc_generate_nfw_radial_positions.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/mc_generate_nfw_radial_positions.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,27 @@
 
 from ......model_helpers import custom_spline
 from ......model_defaults import halo_mass_definition as default_halo_mass_definition
 
 from .......sim_manager.sim_defaults import default_cosmology, default_redshift
 from .......custom_exceptions import HalotoolsError
 
-__all__ = ('mc_generate_nfw_radial_positions', )
+__all__ = ("mc_generate_nfw_radial_positions",)
 
 
-def mc_generate_nfw_radial_positions(num_pts=int(1e4), conc=5,
-            cosmology=default_cosmology, redshift=default_redshift,
-            mdef=default_halo_mass_definition, seed=None,
-            **kwargs):
-    r""" Return a Monte Carlo realization of points in an NFW profile.
+def mc_generate_nfw_radial_positions(
+    num_pts=int(1e4),
+    conc=5,
+    cosmology=default_cosmology,
+    redshift=default_redshift,
+    mdef=default_halo_mass_definition,
+    seed=None,
+    **kwargs
+):
+    r"""Return a Monte Carlo realization of points in an NFW profile.
 
     See :ref:`monte_carlo_nfw_spatial_profile` for a discussion of this technique.
 
     Parameters
     -----------
     num_pts : int, optional
         Number of points in the Monte Carlo realization of the profile.
@@ -73,38 +78,40 @@
 
     Examples
     ---------
     >>> radial_positions = mc_generate_nfw_radial_positions(halo_mass = 1e12, conc = 10)
     >>> radial_positions = mc_generate_nfw_radial_positions(halo_radius = 0.25)
     """
     try:
-        halo_radius = kwargs['halo_radius']
+        halo_radius = kwargs["halo_radius"]
     except KeyError:
         try:
-            halo_mass = kwargs['halo_mass']
+            halo_mass = kwargs["halo_mass"]
             halo_radius = halo_mass_to_halo_radius(halo_mass, cosmology, redshift, mdef)
         except KeyError:
-            msg = ("\nIf keyword argument ``halo_radius`` is unspecified, "
-                "argument ``halo_mass`` must be specified.\n")
+            msg = (
+                "\nIf keyword argument ``halo_radius`` is unspecified, "
+                "argument ``halo_mass`` must be specified.\n"
+            )
             raise HalotoolsError(msg)
         except TypeError:
             raise HalotoolsError("Input ``halo_mass`` must be a float")
 
     halo_radius = np.atleast_1d(halo_radius).astype(np.float64)
     try:
         assert len(halo_radius) == 1
     except AssertionError:
-        msg = ("Input ``halo_radius`` must be a float")
+        msg = "Input ``halo_radius`` must be a float"
         raise HalotoolsError(msg)
 
     conc = np.atleast_1d(conc).astype(np.float64)
     try:
         assert len(conc) == 1
     except AssertionError:
-        msg = ("Input ``conc`` must be a float")
+        msg = "Input ``conc`` must be a float"
         raise HalotoolsError(msg)
 
     # Build lookup table from which to tabulate the inverse cumulative_mass_PDF
     Npts_radius_table = int(1e3)
     radius_array = np.logspace(-4, 0, Npts_radius_table)
     logradius_array = np.log10(radius_array)
     table_ordinates = cumulative_mass_PDF(radius_array, conc)
@@ -113,11 +120,11 @@
 
     # Use method of Inverse Transform Sampling to generate a Monte Carlo realization
     # of the radial positions
     with NumpyRNGContext(seed):
         randoms = np.random.uniform(0, 1, num_pts)
     log_randoms = np.log10(randoms)
     log_scaled_radial_positions = funcobj(log_randoms)
-    scaled_radial_positions = 10.**log_scaled_radial_positions
-    radial_positions = scaled_radial_positions*halo_radius
+    scaled_radial_positions = 10.0**log_scaled_radial_positions
+    radial_positions = scaled_radial_positions * halo_radius
 
     return radial_positions
```

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_c10.dat` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_c10.dat`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_c5.dat` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_c5.dat`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_ch10_cg5.dat` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_ch10_cg5.dat`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_ch5_cg10.dat` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/data/van_den_bosch_nfw_vr_disp_ch5_cg10.dat`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/test_biased_isotropic_velocity.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/test_biased_isotropic_velocity.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/test_mc_generate_nfw_radial_positions.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/test_mc_generate_nfw_radial_positions.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/test_unbiased_isotropic_velocity.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/tests/test_unbiased_isotropic_velocity.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/unbiased_isotropic_velocity.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/kernels/unbiased_isotropic_velocity.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 """
 import numpy as np
 from scipy.integrate import quad as quad_integration
 
 from .mass_profile import _g_integral
 
 
-__all__ = ('dimensionless_radial_velocity_dispersion', )
+__all__ = ("dimensionless_radial_velocity_dispersion",)
 
 
 def _jeans_integrand_term1(y):
-    r"""
-    """
-    return np.log(1+y)/(y**3*(1+y)**2)
+    r""" """
+    return np.log(1 + y) / (y**3 * (1 + y) ** 2)
 
 
 def _jeans_integrand_term2(y):
-    r"""
-    """
-    return 1/(y**2*(1+y)**3)
+    r""" """
+    return 1 / (y**2 * (1 + y) ** 3)
 
 
 def dimensionless_radial_velocity_dispersion(scaled_radius, *conc):
     r"""
     Analytical solution to the isotropic jeans equation for an NFW potential,
     rendered dimensionless via scaling by the virial velocity.
 
@@ -45,19 +43,21 @@
     result : array_like
         Radial velocity dispersion profile scaled by the virial velocity.
         The returned result has the same dimension as the input ``scaled_radius``.
     """
     x = np.atleast_1d(scaled_radius).astype(np.float64)
     result = np.zeros_like(x)
 
-    prefactor = conc*(conc*x)*(1. + conc*x)**2/_g_integral(conc)
+    prefactor = conc * (conc * x) * (1.0 + conc * x) ** 2 / _g_integral(conc)
 
-    lower_limit = conc*x
+    lower_limit = conc * x
     upper_limit = float("inf")
     for i in range(len(x)):
-        term1, _ = quad_integration(_jeans_integrand_term1,
-            lower_limit[i], upper_limit, epsrel=1e-5)
-        term2, _ = quad_integration(_jeans_integrand_term2,
-            lower_limit[i], upper_limit, epsrel=1e-5)
+        term1, _ = quad_integration(
+            _jeans_integrand_term1, lower_limit[i], upper_limit, epsrel=1e-5
+        )
+        term2, _ = quad_integration(
+            _jeans_integrand_term2, lower_limit[i], upper_limit, epsrel=1e-5
+        )
         result[i] = term1 - term2
 
-    return np.sqrt(result*prefactor)
+    return np.sqrt(result * prefactor)
```

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/nfw_phase_space.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/nfw_phase_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """
 """
-from __future__ import division, print_function, absolute_import
+from __future__ import absolute_import, division, print_function
 
 import numpy as np
 from astropy.table import Table
 
-from .nfw_profile import NFWProfile
-from .kernels import unbiased_dimless_vrad_disp as unbiased_dimless_vrad_disp_kernel
-
-from ...monte_carlo_helpers import MonteCarloGalProf
-
 from ..... import model_defaults
-
+from ...monte_carlo_helpers import MonteCarloGalProf
+from .kernels import unbiased_dimless_vrad_disp as unbiased_dimless_vrad_disp_kernel
+from .nfw_profile import NFWProfile
 
 __author__ = ["Andrew Hearin"]
 __all__ = ["NFWPhaseSpace"]
 
 
 class NFWPhaseSpace(NFWProfile, MonteCarloGalProf):
-    r""" Model for the phase space distribution of mass and/or galaxies
+    r"""Model for the phase space distribution of mass and/or galaxies
     in isotropic Jeans equilibrium in an NFW halo profile,
     based on Navarro, Frenk and White (1995),
     where the concentration of the galaxies is the same
     as the concentration of the parent halo
 
     For a review of the mathematics underlying the NFW profile,
     including descriptions of how the relevant equations are
@@ -79,28 +76,27 @@
 
         prof_lookup_args = self._retrieve_prof_lookup_info(**kwargs)
         self.setup_prof_lookup_tables(*prof_lookup_args)
 
         self._mock_generation_calling_sequence = ["assign_phase_space"]
 
     def _retrieve_prof_lookup_info(self, **kwargs):
-        r""" Retrieve the arrays defining the lookup table control points
-        """
+        r"""Retrieve the arrays defining the lookup table control points"""
         cmin, cmax = (
             model_defaults.min_permitted_conc,
             model_defaults.max_permitted_conc,
         )
         dc = 1.0
         npts_conc = int(np.round((cmax - cmin) / float(dc)))
         default_conc_arr = np.linspace(cmin, cmax, npts_conc)
         conc_arr = kwargs.get("concentration_bins", default_conc_arr)
         return [conc_arr]
 
     def assign_phase_space(self, table, seed=None):
-        r""" Primary method of the `NFWPhaseSpace` class
+        r"""Primary method of the `NFWPhaseSpace` class
         called during the mock-population sequence.
 
         Parameters
         -----------
         table : object
             `~astropy.table.Table` storing halo catalog.
 
@@ -116,15 +112,15 @@
         """
         MonteCarloGalProf.mc_pos(self, table=table, seed=seed)
         if seed is not None:
             seed += 1
         MonteCarloGalProf.mc_vel(self, table=table, seed=seed)
 
     def conc_NFWmodel(self, *args, **kwargs):
-        r""" NFW concentration as a function of halo mass.
+        r"""NFW concentration as a function of halo mass.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             Array storing the mass-like variable, e.g., ``halo_mvir``.
 
             If ``prim_haloprop`` is not passed,
@@ -279,15 +275,15 @@
         Notes
         ------
         See :ref:`halo_profile_definitions` for derivations and implementation details.
         """
         return NFWProfile.mass_density(self, radius, mass, conc)
 
     def cumulative_gal_PDF(self, scaled_radius, conc):
-        r""" Analogous to `cumulative_mass_PDF`, but for the satellite galaxy distribution
+        r"""Analogous to `cumulative_mass_PDF`, but for the satellite galaxy distribution
         instead of the host halo mass distribution.
 
         In `~halotools.empirical_models.NFWPhaseSpace` there is no distinction between the
         two methods, but in `~halotools.empirical_models.BiasedNFWPhaseSpace` these two
         function are different.
 
         Parameters
@@ -400,15 +396,15 @@
         Notes
         ------
         See :ref:`halo_profile_definitions` for derivations and implementation details.
         """
         return NFWProfile.enclosed_mass(self, radius, total_mass, conc)
 
     def virial_velocity(self, total_mass):
-        r""" The circular velocity evaluated at the halo boundary,
+        r"""The circular velocity evaluated at the halo boundary,
         :math:`V_{\rm vir} \equiv \sqrt{GM_{\rm halo}/R_{\rm halo}}`.
 
         Parameters
         --------------
         total_mass : array_like
             Total mass of the halo; can be a scalar or numpy array.
 
@@ -468,15 +464,15 @@
         Notes
         ------
         See :ref:`halo_profile_definitions` for derivations and implementation details.
         """
         return NFWProfile.circular_velocity(self, radius, total_mass, conc)
 
     def vmax(self, total_mass, conc):
-        r""" Maximum circular velocity of the halo profile.
+        r"""Maximum circular velocity of the halo profile.
 
         Parameters
         ----------
         total_mass: array_like
             Total halo mass in :math:`M_{\odot}/h`; can be a number or a numpy array.
 
         conc : array_like
@@ -626,15 +622,15 @@
 
     def build_lookup_tables(
         self,
         logrmin=model_defaults.default_lograd_min,
         logrmax=model_defaults.default_lograd_max,
         Npts_radius_table=model_defaults.Npts_radius_table,
     ):
-        r""" Method used to create a lookup table of the spatial and velocity radial profiles.
+        r"""Method used to create a lookup table of the spatial and velocity radial profiles.
 
         Parameters
         ----------
         logrmin : float, optional
             Minimum radius used to build the spline table.
             Default is set in `~halotools.empirical_models.model_defaults`.
 
@@ -646,15 +642,15 @@
             Number of control points used in the spline.
             Default is set in `~halotools.empirical_models.model_defaults`.
 
         """
         MonteCarloGalProf.build_lookup_tables(self, logrmin, logrmax, Npts_radius_table)
 
     def mc_unit_sphere(self, Npts, **kwargs):
-        r""" Returns Npts random points on the unit sphere.
+        r"""Returns Npts random points on the unit sphere.
 
         Parameters
         ----------
         Npts : int
             Number of 3d points to generate
 
         seed : int, optional
@@ -666,15 +662,15 @@
         x, y, z : array_like
             Length-Npts arrays of the coordinate positions.
 
         """
         return MonteCarloGalProf.mc_unit_sphere(self, Npts, **kwargs)
 
     def mc_solid_sphere(self, *concentration_array, **kwargs):
-        r""" Method to generate random, three-dimensional, halo-centric positions of galaxies.
+        r"""Method to generate random, three-dimensional, halo-centric positions of galaxies.
 
         Parameters
         ----------
         concentration_array : array_like, optional
             Length-Ngals numpy array storing the concentrations of the mock galaxies.
 
         table : data table, optional
@@ -690,15 +686,15 @@
         x, y, z : arrays
             Length-Ngals array storing a Monte Carlo realization of the galaxy positions.
 
         """
         return MonteCarloGalProf.mc_solid_sphere(self, *concentration_array, **kwargs)
 
     def mc_halo_centric_pos(self, *concentration_array, **kwargs):
-        r""" Method to generate random, three-dimensional
+        r"""Method to generate random, three-dimensional
         halo-centric positions of galaxies.
 
         Parameters
         ----------
         table : data table, optional
             Astropy Table storing a length-Ngals galaxy catalog.
             If ``table`` is not passed, ``concentration_array`` and
@@ -726,15 +722,15 @@
 
         """
         return MonteCarloGalProf.mc_halo_centric_pos(
             self, *concentration_array, **kwargs
         )
 
     def mc_pos(self, *concentration_array, **kwargs):
-        r""" Method to generate random, three-dimensional positions of galaxies.
+        r"""Method to generate random, three-dimensional positions of galaxies.
 
         Parameters
         ----------
         table : data table, optional
             Astropy Table storing a length-Ngals galaxy catalog.
             If ``table`` is not passed, ``concentration_array`` and ``halo_radius`` must be passed.
 
@@ -772,15 +768,15 @@
             Random number seed used in the Monte Carlo realization.
             Default is None, which will produce stochastic results.
 
         """
         return MonteCarloGalProf.mc_pos(self, *concentration_array, **kwargs)
 
     def _vrad_disp_from_lookup(self, scaled_radius, *concentration_array, **kwargs):
-        r""" Method to generate Monte Carlo realizations of the profile model.
+        r"""Method to generate Monte Carlo realizations of the profile model.
 
         Parameters
         ----------
         scaled_radius : array_like
             Halo-centric distance *r* scaled by the halo boundary :math:`R_{\Delta}`, so that
             :math:`0 <= \tilde{r} \equiv r/R_{\Delta} <= 1`. Can be a scalar or numpy array.
 
@@ -829,15 +825,15 @@
             solution to the Jeans equation.
         """
         return MonteCarloGalProf.mc_radial_velocity(
             self, scaled_radius, total_mass, *concentration_array, **kwargs
         )
 
     def mc_vel(self, table, seed=None):
-        r""" Method assigns a Monte Carlo realization of the Jeans velocity
+        r"""Method assigns a Monte Carlo realization of the Jeans velocity
         solution to the halos in the input ``table``.
 
         Parameters
         -----------
         table : Astropy Table
             `astropy.table.Table` object storing the halo catalog.
             Calling the `mc_vel` method will over-write the existing values of
@@ -849,15 +845,15 @@
 
         """
         MonteCarloGalProf.mc_vel(self, table, seed=seed)
 
     def mc_generate_nfw_phase_space_points(
         self, Ngals=int(1e4), conc=5, mass=1e12, verbose=True, seed=None
     ):
-        r""" Return a Monte Carlo realization of points
+        r"""Return a Monte Carlo realization of points
         in the phase space of an NFW halo in isotropic Jeans equilibrium.
 
         Parameters
         -----------
         Ngals : int, optional
             Number of galaxies in the Monte Carlo realization of the
             phase space distribution. Default is 1e4.
@@ -882,14 +878,18 @@
         --------
         t : table
             `~astropy.table.Table` containing the Monte Carlo realization of the
             phase space distribution.
             Keys are 'x', 'y', 'z', 'vx', 'vy', 'vz', 'radial_position', 'radial_velocity'.
             Length units in Mpc/h, velocity units in km/s.
 
+            Sign convention on the returned `radial_velocity` column is such that
+            negative (positive) values correspond to
+            satellites moving radially inward (outward)
+
         Examples
         ---------
         >>> nfw = NFWPhaseSpace()
         >>> mass, conc = 1e13, 8.
         >>> data = nfw.mc_generate_nfw_phase_space_points(Ngals=100, mass=mass, conc=conc, verbose=False)
 
         Now suppose you wish to compute the radial velocity dispersion of all the returned points:
@@ -929,15 +929,15 @@
             m = np.zeros(Ngals) + mass
 
         rvir = NFWProfile.halo_mass_to_halo_radius(self, total_mass=m)
 
         x, y, z = MonteCarloGalProf.mc_halo_centric_pos(
             self, c, halo_radius=rvir, seed=seed
         )
-        r = np.sqrt(x ** 2 + y ** 2 + z ** 2)
+        r = np.sqrt(x**2 + y**2 + z**2)
         scaled_radius = r / rvir
 
         if seed is not None:
             seed += 1
         vx = MonteCarloGalProf.mc_radial_velocity(self, scaled_radius, m, c, seed=seed)
         if seed is not None:
             seed += 1
@@ -993,14 +993,16 @@
     if return_pbc_correction:
         return result, pbc_correction
     else:
         return result
 
 
 def _relative_positions_and_velocities(x1, x2, period=None, **kwargs):
+    """Sign convention on the returned velocity is such that
+    negative (positive) values correspond to approaching (receding) objects"""
     s = _sign_pbc(x1, x2, period=period, equality_fill_val=1.0)
     absd = np.abs(x1 - x2)
     if period is None:
         xrel = s * absd
     else:
         xrel = s * np.where(absd > period / 2.0, period - absd, absd)
```

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/nfw_profile.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/nfw_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 __all__ = ("NFWProfile",)
 __author__ = ("Andrew Hearin", "Benedikt Diemer")
 
 
 class NFWProfile(AnalyticDensityProf):
-    r""" Model for the spatial distribution of mass
+    r"""Model for the spatial distribution of mass
     and/or galaxies residing in an NFW halo profile,
     based on Navarro, Frenk and White (1995),
     `arXiv:9508025 <http://arxiv.org/abs/astro-ph/9508025/>`_.
 
     For a review of the mathematics underlying the NFW profile,
     including descriptions of how the relevant equations are
     implemented in the Halotools code base, see :ref:`nfw_profile_tutorial`.
@@ -102,15 +102,15 @@
             self.concentration_key = kwargs.get(
                 "concentration_key", model_defaults.concentration_key
             )
 
         self.conc_mass_model = conc_mass_model
 
     def conc_NFWmodel(self, *args, **kwargs):
-        r""" NFW concentration as a function of halo mass.
+        r"""NFW concentration as a function of halo mass.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             Array storing the mass-like variable, e.g., ``halo_mvir``.
 
             If ``prim_haloprop`` is not passed,
@@ -383,15 +383,15 @@
         Notes
         ------
         See :ref:`halo_profile_definitions` for derivations and implementation details.
         """
         return AnalyticDensityProf.enclosed_mass(self, radius, total_mass, conc)
 
     def virial_velocity(self, total_mass):
-        r""" The circular velocity evaluated at the halo boundary,
+        r"""The circular velocity evaluated at the halo boundary,
         :math:`V_{\rm vir} \equiv \sqrt{GM_{\rm halo}/R_{\rm halo}}`.
 
         Parameters
         --------------
         total_mass : array_like
             Total mass of the halo; can be a scalar or numpy array.
 
@@ -451,15 +451,15 @@
         Notes
         ------
         See :ref:`halo_profile_definitions` for derivations and implementation details.
         """
         return AnalyticDensityProf.circular_velocity(self, radius, total_mass, conc)
 
     def rmax(self, total_mass, conc):
-        r""" Radius at which the halo attains its maximum circular velocity,
+        r"""Radius at which the halo attains its maximum circular velocity,
         :math:`R_{\rm max}^{\rm NFW} = 2.16258R_{\Delta}/c`.
 
         Parameters
         ----------
         total_mass: array_like
             Total halo mass in :math:`M_{\odot}/h`; can be a number or a numpy array.
 
@@ -488,15 +488,15 @@
 
         """
         halo_radius = self.halo_mass_to_halo_radius(total_mass)
         scale_radius = halo_radius / conc
         return 2.16258 * scale_radius
 
     def vmax(self, total_mass, conc):
-        r""" Maximum circular velocity of the halo profile,
+        r"""Maximum circular velocity of the halo profile,
         :math:`V_{\rm max}^{\rm NFW} = V_{\rm cir}^{\rm NFW}(r = 2.16258R_{\Delta}/c)`.
 
         Parameters
         ----------
         total_mass: array_like
             Total halo mass in :math:`M_{\odot}/h`; can be a number or a numpy array.
 
@@ -573,15 +573,15 @@
         --------
         >>> model = NFWProfile()
         >>> halo_mass = model.halo_mass_to_halo_radius(500.)
         """
         return AnalyticDensityProf.halo_radius_to_halo_mass(self, radius)
 
     def mc_generate_nfw_radial_positions(self, **kwargs):
-        r""" Return a Monte Carlo realization of points in an NFW profile.
+        r"""Return a Monte Carlo realization of points in an NFW profile.
 
         See :ref:`monte_carlo_nfw_spatial_profile` for a discussion of this technique.
 
         Parameters
         -----------
         num_pts : int, optional
             Number of points in the Monte Carlo realization of the profile.
```

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/sfr_biased_nfw_phase_space.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/sfr_biased_nfw_phase_space.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 from __future__ import division, print_function, absolute_import
 
 import numpy as np
 
 from .biased_nfw_phase_space import BiasedNFWPhaseSpace
 
 
-__author__ = ('Andrew Hearin', )
-__all__ = ('SFRBiasedNFWPhaseSpace', )
+__author__ = ("Andrew Hearin",)
+__all__ = ("SFRBiasedNFWPhaseSpace",)
 
 
-missing_quiescent_key_msg = ("The `SFRBiasedNFWPhaseSpace` class "
+missing_quiescent_key_msg = (
+    "The `SFRBiasedNFWPhaseSpace` class "
     "can only be used to make mocks \nin concert "
     "with some other component model that is responsible for \nmodeling an"
-    "``quiescent`` property of the ``galaxy_table``.\n")
+    "``quiescent`` property of the ``galaxy_table``.\n"
+)
 
 
 class SFRBiasedNFWPhaseSpace(BiasedNFWPhaseSpace):
-    r""" Model for the phase space distribution of galaxies
+    r"""Model for the phase space distribution of galaxies
     in isotropic Jeans equilibrium in an NFW halo profile,
     based on Navarro, Frenk and White (1995),
     where the concentration of the tracers is permitted to differ from the
     host halo concentration, independently for red and blue galaxies.
 
     For a review of the mathematics underlying the NFW profile,
     including descriptions of how the relevant equations are
@@ -141,42 +143,49 @@
         between the control points will be determined by log-linear interpolation.
         When extrapolating :math:`F_{\rm q}` and :math:`F_{\rm sf}` beyond
         the specified range, the values will be kept constant at the end point values.
         """
         BiasedNFWPhaseSpace.__init__(self, **kwargs)
 
     def _initialize_conc_bias_param_dict(self, **kwargs):
-        r""" Set up the appropriate number of keys in the parameter dictionary
+        r"""Set up the appropriate number of keys in the parameter dictionary
         and give the keys standardized names.
         """
 
-        if 'conc_gal_bias_logM_abscissa' in list(kwargs.keys()):
+        if "conc_gal_bias_logM_abscissa" in list(kwargs.keys()):
             _conc_bias_logM_abscissa = np.atleast_1d(
-                kwargs.get('conc_gal_bias_logM_abscissa')).astype('f4')
+                kwargs.get("conc_gal_bias_logM_abscissa")
+            ).astype("f4")
 
-            d_q = ({'quiescent_conc_gal_bias_param'+str(i): 1.
-                for i in range(len(_conc_bias_logM_abscissa))})
-            d_sf = ({'star_forming_conc_gal_bias_param'+str(i): 1.
-                for i in range(len(_conc_bias_logM_abscissa))})
-
-            d_abscissa = ({'conc_gal_bias_logM_abscissa_param'+str(i): float(logM)
-                for i, logM in enumerate(_conc_bias_logM_abscissa)})
+            d_q = {
+                "quiescent_conc_gal_bias_param" + str(i): 1.0
+                for i in range(len(_conc_bias_logM_abscissa))
+            }
+            d_sf = {
+                "star_forming_conc_gal_bias_param" + str(i): 1.0
+                for i in range(len(_conc_bias_logM_abscissa))
+            }
+
+            d_abscissa = {
+                "conc_gal_bias_logM_abscissa_param" + str(i): float(logM)
+                for i, logM in enumerate(_conc_bias_logM_abscissa)
+            }
             self._num_conc_bias_params = len(_conc_bias_logM_abscissa)
 
             d = {}
             d.update(d_q)
             d.update(d_sf)
             d.update(d_abscissa)
             return d
 
         else:
-            return {'quiescent_conc_gal_bias': 1., 'star_forming_conc_gal_bias': 1.}
+            return {"quiescent_conc_gal_bias": 1.0, "star_forming_conc_gal_bias": 1.0}
 
     def calculate_conc_gal_bias(self, seed=None, **kwargs):
-        r""" Calculate the ratio of the galaxy concentration to the halo concentration,
+        r"""Calculate the ratio of the galaxy concentration to the halo concentration,
         :math:`c_{\rm gal}/c_{\rm halo}`.
 
         Parameters
         ----------
         prim_haloprop : array, optional
             Array storing the mass-like variable, e.g., ``halo_mvir``.
 
@@ -207,54 +216,64 @@
         --------
         >>> model = SFRBiasedNFWPhaseSpace()
         >>> mass = np.logspace(10, 15, 100)
         >>> quiescent = np.zeros(100).astype(bool)
         >>> quiescent[::2] = True
         >>> conc_gal_bias = model.calculate_conc_gal_bias(prim_haloprop=mass, quiescent=quiescent)
         """
-        if 'table' in list(kwargs.keys()):
-            table = kwargs['table']
+        if "table" in list(kwargs.keys()):
+            table = kwargs["table"]
             mass = table[self.prim_haloprop_key]
             try:
-                quiescent = table['quiescent']
+                quiescent = table["quiescent"]
             except KeyError:
                 raise KeyError(missing_quiescent_key_msg)
-        elif 'prim_haloprop' in list(kwargs.keys()):
-            mass = np.atleast_1d(kwargs['prim_haloprop']).astype('f4')
-            quiescent = np.atleast_1d(kwargs['quiescent']).astype(bool)
+        elif "prim_haloprop" in list(kwargs.keys()):
+            mass = np.atleast_1d(kwargs["prim_haloprop"]).astype("f4")
+            quiescent = np.atleast_1d(kwargs["quiescent"]).astype(bool)
             if len(quiescent) == 1:
                 quiescent = (np.zeros_like(mass) + quiescent[0]).astype(bool)
         else:
-            msg = ("\nYou must pass either a ``table`` or ``prim_haloprop`` argument \n"
-                "to the ``assign_conc_gal_bias`` function of the ``BiasedNFWPhaseSpace`` class.\n")
+            msg = (
+                "\nYou must pass either a ``table`` or ``prim_haloprop`` argument \n"
+                "to the ``assign_conc_gal_bias`` function of the ``BiasedNFWPhaseSpace`` class.\n"
+            )
             raise KeyError(msg)
 
-        if 'conc_gal_bias_logM_abscissa_param0' in self.param_dict.keys():
-            abscissa_keys = list('conc_gal_bias_logM_abscissa_param'+str(i)
-                for i in range(self._num_conc_bias_params))
+        if "conc_gal_bias_logM_abscissa_param0" in self.param_dict.keys():
+            abscissa_keys = list(
+                "conc_gal_bias_logM_abscissa_param" + str(i)
+                for i in range(self._num_conc_bias_params)
+            )
             abscissa = [self.param_dict[key] for key in abscissa_keys]
 
-            q_ordinates_keys = list('quiescent_conc_gal_bias_param'+str(i)
-                for i in range(self._num_conc_bias_params))
+            q_ordinates_keys = list(
+                "quiescent_conc_gal_bias_param" + str(i)
+                for i in range(self._num_conc_bias_params)
+            )
             q_ordinates = [self.param_dict[key] for key in q_ordinates_keys]
 
-            sf_ordinates_keys = list('star_forming_conc_gal_bias_param'+str(i)
-                for i in range(self._num_conc_bias_params))
+            sf_ordinates_keys = list(
+                "star_forming_conc_gal_bias_param" + str(i)
+                for i in range(self._num_conc_bias_params)
+            )
             sf_ordinates = [self.param_dict[key] for key in sf_ordinates_keys]
 
             result = np.zeros_like(mass)
-            result[quiescent] = np.interp(np.log10(mass[quiescent]),
-                abscissa, q_ordinates)
-            result[~quiescent] = np.interp(np.log10(mass[~quiescent]),
-                abscissa, sf_ordinates)
+            result[quiescent] = np.interp(
+                np.log10(mass[quiescent]), abscissa, q_ordinates
+            )
+            result[~quiescent] = np.interp(
+                np.log10(mass[~quiescent]), abscissa, sf_ordinates
+            )
         else:
             result = np.zeros_like(mass)
-            result[quiescent] = self.param_dict['quiescent_conc_gal_bias']
-            result[~quiescent] = self.param_dict['star_forming_conc_gal_bias']
+            result[quiescent] = self.param_dict["quiescent_conc_gal_bias"]
+            result[~quiescent] = self.param_dict["star_forming_conc_gal_bias"]
 
-        if 'table' in list(kwargs.keys()):
-            table['conc_gal_bias'][:] = result
-            halo_conc = table['conc_NFWmodel']
+        if "table" in list(kwargs.keys()):
+            table["conc_gal_bias"][:] = result
+            halo_conc = table["conc_NFWmodel"]
             gal_conc = self._clipped_galaxy_concentration(halo_conc, result)
-            table['conc_galaxy'][:] = gal_conc
+            table["conc_galaxy"][:] = gal_conc
         else:
             return result
```

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_consistency.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_consistency.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_consistency_mockpop.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_consistency_mockpop.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_initialization.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_initialization.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_phase_space.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_phase_space.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_phase_space_argument_handling.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_biased_nfw_phase_space_argument_handling.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_conc_gal_bias_behavior.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_conc_gal_bias_behavior.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_mockpop.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_biased_nfw/test_mockpop.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_conc_mass_inheritance/test_direct_from_halo_catalog.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_conc_mass_inheritance/test_direct_from_halo_catalog.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_argument_handling.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_argument_handling.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_functions.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_functions.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_initialization.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_initialization.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_monte_carlo.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_phase_space/test_nfw_phase_space_monte_carlo.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_profile/test_colossus_consistency.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_profile/test_colossus_consistency.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_profile/test_nfw_profile.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/satellites/nfw/tests/test_nfw_profile/test_nfw_profile.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/analytic_models/tests/test_halo_boundary_functions.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/analytic_models/tests/test_halo_boundary_functions.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/subhalo_phase_space.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/subhalo_phase_space.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/subhalo_selection_kernel.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/subhalo_selection_kernel.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/test_composite_model.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/test_composite_model.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/test_subhalo_phase_space.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/test_subhalo_phase_space.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/test_subhalo_selection_kernel.py` & `halotools-0.8.2/halotools/empirical_models/phase_space_models/subhalo_based_models/tests/test_subhalo_selection_kernel.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/sfr_models/halo_mass_quenching.py` & `halotools-0.8.2/halotools/empirical_models/sfr_models/halo_mass_quenching.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/sfr_models/tests/test_halo_mass_quenching.py` & `halotools-0.8.2/halotools/empirical_models/sfr_models/tests/test_halo_mass_quenching.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/sfr_models/tests/test_zu_mandelbaum16.py` & `halotools-0.8.2/halotools/empirical_models/sfr_models/tests/test_zu_mandelbaum16.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/sfr_models/zu_mandelbaum16.py` & `halotools-0.8.2/halotools/empirical_models/sfr_models/zu_mandelbaum16.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/smhm_models/behroozi10.py` & `halotools-0.8.2/halotools/empirical_models/smhm_models/behroozi10.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/smhm_models/moster13.py` & `halotools-0.8.2/halotools/empirical_models/smhm_models/moster13.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/smhm_models/smhm_helpers.py` & `halotools-0.8.2/halotools/empirical_models/smhm_models/smhm_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/smhm_models/tests/test_behroozi10.py` & `halotools-0.8.2/halotools/empirical_models/smhm_models/tests/test_behroozi10.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/smhm_models/tests/test_moster13.py` & `halotools-0.8.2/halotools/empirical_models/smhm_models/tests/test_moster13.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/smhm_models/tests/test_redshift_defensiveness.py` & `halotools-0.8.2/halotools/empirical_models/smhm_models/tests/test_redshift_defensiveness.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/smhm_models/zu_mandelbaum15.py` & `halotools-0.8.2/halotools/empirical_models/smhm_models/zu_mandelbaum15.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/empirical_models/tests/test_model_helpers.py` & `halotools-0.8.2/halotools/empirical_models/tests/test_model_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/__init__.py` & `halotools-0.8.2/halotools/mock_observables/__init__.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/catalog_analysis_helpers.py` & `halotools-0.8.2/halotools/mock_observables/catalog_analysis_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 r""" Common functions used when analyzing catalogs of galaxies/halos.
 """
-from __future__ import (absolute_import, division, print_function, unicode_literals)
+from __future__ import absolute_import, division, print_function, unicode_literals
 
 import numpy as np
 from scipy.stats import binned_statistic
 
+from ..custom_exceptions import HalotoolsError
 from ..empirical_models import enforce_periodicity_of_box
 from ..sim_manager.sim_defaults import default_cosmology, default_redshift
 
-from ..custom_exceptions import HalotoolsError
-
-__all__ = ('mean_y_vs_x', 'return_xyz_formatted_array', 'cuboid_subvolume_labels',
-    'relative_positions_and_velocities', 'sign_pbc', 'apply_zspace_distortion')
-__author__ = ['Andrew Hearin']
+__all__ = (
+    "mean_y_vs_x",
+    "return_xyz_formatted_array",
+    "cuboid_subvolume_labels",
+    "relative_positions_and_velocities",
+    "sign_pbc",
+    "apply_zspace_distortion",
+)
+__author__ = ["Andrew Hearin"]
 
 
-def mean_y_vs_x(x, y, error_estimator='error_on_mean', **kwargs):
+def mean_y_vs_x(x, y, error_estimator="error_on_mean", **kwargs):
     r"""
     Estimate the mean value of the property *y* as a function of *x*
     for an input sample of galaxies/halos,
     optionally returning an error estimate.
 
     The `mean_y_vs_x` function is just a convenience wrapper
     around `scipy.stats.binned_statistic` and `np.histogram`.
@@ -69,42 +74,51 @@
 
     See also
     ---------
     :ref:`galaxy_catalog_analysis_tutorial1`
 
     """
     try:
-        assert error_estimator in ('error_on_mean', 'variance')
+        assert error_estimator in ("error_on_mean", "variance")
     except AssertionError:
-        msg = ("\nInput ``error_estimator`` must be either "
-            "``error_on_mean`` or ``variance``\n")
+        msg = (
+            "\nInput ``error_estimator`` must be either "
+            "``error_on_mean`` or ``variance``\n"
+        )
         raise HalotoolsError(msg)
 
-    modified_kwargs = {key: kwargs[key] for key in kwargs if key != 'error_estimator'}
-    result = binned_statistic(x, y, statistic='mean', **modified_kwargs)
+    modified_kwargs = {key: kwargs[key] for key in kwargs if key != "error_estimator"}
+    result = binned_statistic(x, y, statistic="mean", **modified_kwargs)
     mean, bin_edges, binnumber = result
-    bin_midpoints = (bin_edges[1:] + bin_edges[:-1])/2.
+    bin_midpoints = (bin_edges[1:] + bin_edges[:-1]) / 2.0
 
-    modified_kwargs['bins'] = bin_edges
+    modified_kwargs["bins"] = bin_edges
 
     result = binned_statistic(x, y, statistic=np.std, **modified_kwargs)
     variance, _, _ = result
 
-    if error_estimator == 'variance':
+    if error_estimator == "variance":
         err = variance
     else:
         counts = np.histogram(x, bins=bin_edges)
-        err = variance/np.sqrt(counts[0])
+        err = variance / np.sqrt(counts[0])
 
     return bin_midpoints, mean, err
 
 
-def return_xyz_formatted_array(x, y, z, period=np.inf,
-        cosmology=default_cosmology, redshift=default_redshift, **kwargs):
-    r""" Returns a Numpy array of shape *(Npts, 3)* storing the
+def return_xyz_formatted_array(
+    x,
+    y,
+    z,
+    period=np.inf,
+    cosmology=default_cosmology,
+    redshift=default_redshift,
+    **kwargs
+):
+    r"""Returns a Numpy array of shape *(Npts, 3)* storing the
     xyz-positions in the format used throughout
     the `~halotools.mock_observables` package, optionally applying redshift-space
     distortions according to the input ``velocity``, ``redshift`` and ``cosmology``.
 
     See :ref:`mock_obs_pos_formatting` for a tutorial.
 
     Parameters
@@ -190,58 +204,75 @@
         period = np.repeat(period, 3)
     elif len(period) == 3:
         pass
     else:
         msg = "Input ``period`` must be a single float or a 3-element sequence"
         raise ValueError(msg)
 
-    posdict = {'x': np.copy(x), 'y': np.copy(y), 'z': np.copy(z)}
-    period_dict = {'x': period[0], 'y': period[1], 'z': period[2]}
-
-    a = 'velocity_distortion_dimension' in list(kwargs.keys())
-    b = 'velocity' in list(kwargs.keys())
-    if bool(a+b) is True:
-        if bool(a*b) is False:
-            msg = ("You must either both or none of the following keyword arguments: "
-                "``velocity_distortion_dimension`` and ``velocity``\n")
+    x = np.mod(x, period[0])
+    y = np.mod(y, period[1])
+    z = np.mod(z, period[2])
+
+    posdict = {"x": np.copy(x), "y": np.copy(y), "z": np.copy(z)}
+    period_dict = {"x": period[0], "y": period[1], "z": period[2]}
+
+    a = "velocity_distortion_dimension" in list(kwargs.keys())
+    b = "velocity" in list(kwargs.keys())
+    if bool(a + b) is True:
+        if bool(a * b) is False:
+            msg = (
+                "You must either both or none of the following keyword arguments: "
+                "``velocity_distortion_dimension`` and ``velocity``\n"
+            )
             raise KeyError(msg)
         else:
-            vel_dist_dim = kwargs['velocity_distortion_dimension']
-            velocity = np.copy(kwargs['velocity'])
+            vel_dist_dim = kwargs["velocity_distortion_dimension"]
+            velocity = np.copy(kwargs["velocity"])
             apply_distortion = True
     else:
         apply_distortion = False
 
     if apply_distortion is True:
         try:
-            assert vel_dist_dim in ('x', 'y', 'z')
-            spatial_distortion = (1. + redshift)*np.copy(velocity)/100./cosmology.efunc(redshift)
+            assert vel_dist_dim in ("x", "y", "z")
+            spatial_distortion = (
+                (1.0 + redshift) * np.copy(velocity) / 100.0 / cosmology.efunc(redshift)
+            )
             posdict[vel_dist_dim] = np.copy(posdict[vel_dist_dim]) + spatial_distortion
             Lbox = period_dict[vel_dist_dim]
             if Lbox != np.inf:
                 posdict[vel_dist_dim] = enforce_periodicity_of_box(
-                    posdict[vel_dist_dim], Lbox)
+                    posdict[vel_dist_dim], Lbox
+                )
         except AssertionError:
-            msg = ("\nInput ``velocity_distortion_dimension`` must be either \n"
-                "``'x'``, ``'y'`` or ``'z'``.")
+            msg = (
+                "\nInput ``velocity_distortion_dimension`` must be either \n"
+                "``'x'``, ``'y'`` or ``'z'``."
+            )
             raise KeyError(msg)
 
-    xout, yout, zout = np.copy(posdict['x']), np.copy(posdict['y']), np.copy(posdict['z'])
+    xout, yout, zout = (
+        np.copy(posdict["x"]),
+        np.copy(posdict["y"]),
+        np.copy(posdict["z"]),
+    )
     pos = np.vstack([xout, yout, zout]).T
 
     # Apply a mask, if applicable
     try:
-        mask = kwargs['mask']
+        mask = kwargs["mask"]
         return pos[mask]
     except KeyError:
         return pos
 
 
-def apply_zspace_distortion(true_pos, peculiar_velocity, redshift, cosmology, Lbox=None):
-    r""" Apply redshift-space distortions to the comoving simulation coordinate,
+def apply_zspace_distortion(
+    true_pos, peculiar_velocity, redshift, cosmology, Lbox=None
+):
+    r"""Apply redshift-space distortions to the comoving simulation coordinate,
     optionally accounting for periodic boundary conditions.
 
     This function implements the following formula:
 
     .. math::
 
         s_{\rm com}^{\rm z-space} = s_{\rm com}^{\rm true} + \frac{1 + z}{H(z)}v_{\rm pec}
@@ -284,16 +315,16 @@
     >>> true_pos = halocat.halo_table['halo_z']
     >>> peculiar_velocity = halocat.halo_table['halo_vz']
     >>> redshift = halocat.redshift
     >>> cosmology = halocat.cosmology
     >>> Lbox = halocat.Lbox[2]
     >>> zspace_zcoord = apply_zspace_distortion(true_pos, peculiar_velocity, redshift, cosmology, Lbox)
     """
-    scale_factor = 1./(1. + redshift)
-    pos_err = peculiar_velocity/100./cosmology.efunc(redshift)/scale_factor
+    scale_factor = 1.0 / (1.0 + redshift)
+    pos_err = peculiar_velocity / 100.0 / cosmology.efunc(redshift) / scale_factor
     zspace_pos = true_pos + pos_err
     if Lbox is not None:
         zspace_pos = enforce_periodicity_of_box(zspace_pos, Lbox)
     return zspace_pos
 
 
 def cuboid_subvolume_labels(sample, Nsub, Lbox):
@@ -348,53 +379,53 @@
     Divide the volume into cubes with length 0.25 on a side.
 
     >>> Nsub = [4,4,4]
     >>> labels, N_sub_vol = cuboid_subvolume_labels(sample, Nsub, Lbox)
     """
 
     # process inputs and check for consistency
-    sample = np.atleast_1d(sample).astype('f8')
+    sample = np.atleast_1d(sample).astype("f8")
     try:
         assert sample.ndim == 2
         assert sample.shape[1] == 3
     except AssertionError:
-        msg = ("Input ``sample`` must have shape (Npts, 3)")
+        msg = "Input ``sample`` must have shape (Npts, 3)"
         raise TypeError(msg)
 
-    Nsub = np.atleast_1d(Nsub).astype('i4')
+    Nsub = np.atleast_1d(Nsub).astype("i4")
     if len(Nsub) == 1:
         Nsub = np.array([Nsub[0], Nsub[0], Nsub[0]])
     elif len(Nsub) != 3:
         msg = "Input ``Nsub`` must be a scalar or length-3 sequence"
         raise TypeError(msg)
 
-    Lbox = np.atleast_1d(Lbox).astype('f8')
+    Lbox = np.atleast_1d(Lbox).astype("f8")
     if len(Lbox) == 1:
-        Lbox = np.array([Lbox[0]]*3)
+        Lbox = np.array([Lbox[0]] * 3)
     elif len(Lbox) != 3:
         msg = "Input ``Lbox`` must be a scalar or length-3 sequence"
         raise TypeError(msg)
 
-    dL = Lbox/Nsub  # length of subvolumes along each dimension
+    dL = Lbox / Nsub  # length of subvolumes along each dimension
     N_sub_vol = int(np.prod(Nsub))  # total the number of subvolumes
     # create an array of unique integer IDs for each subvolume
-    inds = np.arange(1, N_sub_vol+1).reshape(Nsub[0], Nsub[1], Nsub[2])
+    inds = np.arange(1, N_sub_vol + 1).reshape(Nsub[0], Nsub[1], Nsub[2])
 
     # tag each particle with an integer indicating which subvolume it is in
-    index = np.floor(sample/dL).astype(int)
+    index = np.floor(sample / dL).astype(int)
     # take care of the case where a point falls on the boundary
     for i in range(3):
         index[:, i] = np.where(index[:, i] == Nsub[i], Nsub[i] - 1, index[:, i])
     index = inds[index[:, 0], index[:, 1], index[:, 2]].astype(int)
 
     return index, int(N_sub_vol)
 
 
-def sign_pbc(x1, x2, period=None, equality_fill_val=0., return_pbc_correction=False):
-    r""" Return the sign of the unit vector pointing from x2 towards x1,
+def sign_pbc(x1, x2, period=None, equality_fill_val=0.0, return_pbc_correction=False):
+    r"""Return the sign of the unit vector pointing from x2 towards x1,
     that is, the sign of (x1 - x2), accounting for periodic boundary conditions.
 
     If x1 > x2, returns 1. If x1 < x2, returns -1. If x1 == x2, returns equality_fill_val.
 
     Parameters
     ----------
     x1 : array
@@ -447,29 +478,29 @@
             assert np.all(x2 >= 0)
             assert np.all(x1 < period)
             assert np.all(x2 < period)
         except AssertionError:
             msg = "If period is not None, all values of x and y must be between [0, period)"
             raise ValueError(msg)
 
-        d = np.abs(x1-x2)
-        pbc_correction = np.sign(period/2. - d)
-        result = pbc_correction*result
+        d = np.abs(x1 - x2)
+        pbc_correction = np.sign(period / 2.0 - d)
+        result = pbc_correction * result
 
     if equality_fill_val != 0:
         result = np.where(result == 0, equality_fill_val, result)
 
     if return_pbc_correction:
         return result, pbc_correction
     else:
         return result
 
 
 def relative_positions_and_velocities(x1, x2, period=None, **kwargs):
-    r""" Return the vector pointing from x2 towards x1,
+    r"""Return the vector pointing from x2 towards x1,
     that is, x1 - x2, accounting for periodic boundary conditions.
 
     If keyword arguments ``v1`` and ``v2`` are passed in,
     additionally return the velocity ``v1`` with respect to ``v2``, with sign convention
     such that positive (negative) values correspond to receding (approaching) points.
 
     Parameters
@@ -526,20 +557,20 @@
     >>> xcen, vcen = 0.1, 100
     >>> xsat, vsat = 249.9, -300
     >>> xrel, vrel = relative_positions_and_velocities(xsat, xcen, v1=vsat, v2=vcen, period=Lbox)
     >>> assert np.isclose(xrel, -0.2)
     >>> assert np.isclose(vrel, +400)
 
     """
-    s = sign_pbc(x1, x2, period=period, equality_fill_val=1.)
+    s = sign_pbc(x1, x2, period=period, equality_fill_val=1.0)
     absd = np.abs(x1 - x2)
     if period is None:
-        xrel = s*absd
+        xrel = s * absd
     else:
-        xrel = s*np.where(absd > period/2., period - absd, absd)
+        xrel = s * np.where(absd > period / 2.0, period - absd, absd)
 
     try:
-        v1 = kwargs['v1']
-        v2 = kwargs['v2']
-        return xrel, s*(v1-v2)
+        v1 = kwargs["v1"]
+        v2 = kwargs["v2"]
+        return xrel, s * (v1 - v2)
     except KeyError:
         return xrel
```

### Comparing `halotools-0.8.1/halotools/mock_observables/counts_in_cells/counts_in_cylinders.py` & `halotools-0.8.2/halotools/mock_observables/counts_in_cells/counts_in_cylinders.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/counts_in_cells/engines/conditions/conditions.pyx` & `halotools-0.8.2/halotools/mock_observables/counts_in_cells/engines/conditions/conditions.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/counts_in_cells/engines/counts_in_cylinders_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/counts_in_cells/engines/counts_in_cylinders_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/counts_in_cells/engines/setup_package.py` & `halotools-0.8.2/halotools/mock_observables/counts_in_cells/engines/setup_package.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/counts_in_cells/tests/pure_python_counts_in_cells.py` & `halotools-0.8.2/halotools/mock_observables/counts_in_cells/tests/pure_python_counts_in_cells.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/counts_in_cells/tests/test_counts_in_cylinders.py` & `halotools-0.8.2/halotools/mock_observables/counts_in_cells/tests/test_counts_in_cylinders.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/group_identification/fof_groups.py` & `halotools-0.8.2/halotools/mock_observables/group_identification/fof_groups.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/group_identification/test_groups/test_fof_groups.py` & `halotools-0.8.2/halotools/mock_observables/group_identification/test_groups/test_fof_groups.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/conditional_cylindrical_isolation.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/conditional_cylindrical_isolation.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/conditional_spherical_isolation.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/conditional_spherical_isolation.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/cylindrical_isolation.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/cylindrical_isolation.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/__init__.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/cylindrical_isolation_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/cylindrical_isolation_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/isolation_criteria_marking_functions.pyx` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/isolation_criteria_marking_functions.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/marked_cylindrical_isolation_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/marked_cylindrical_isolation_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/marked_spherical_isolation_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/marked_spherical_isolation_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/setup_package.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/setup_package.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/engines/spherical_isolation_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/engines/spherical_isolation_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/isolation_functions_helpers.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/isolation_functions_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/spherical_isolation.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/spherical_isolation.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/pure_python_isolation.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/pure_python_isolation.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_brute_force_comparisons.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_brute_force_comparisons.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_conditional_cylindrical_isolation.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_conditional_cylindrical_isolation.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_conditional_spherical_isolation.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_conditional_spherical_isolation.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_cylindrical_isolation.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_cylindrical_isolation.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_isolation_helpers.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_isolation_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_pure_python_isolation.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_pure_python_isolation.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/isolation_functions/tests/test_spherical_isolation.py` & `halotools-0.8.2/halotools/mock_observables/isolation_functions/tests/test_spherical_isolation.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/large_scale_density/large_scale_density_spherical_annulus.py` & `halotools-0.8.2/halotools/mock_observables/large_scale_density/large_scale_density_spherical_annulus.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/large_scale_density/large_scale_density_spherical_volume.py` & `halotools-0.8.2/halotools/mock_observables/large_scale_density/large_scale_density_spherical_volume.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/large_scale_density/tests/test_large_scale_density_spherical_annulus.py` & `halotools-0.8.2/halotools/mock_observables/large_scale_density/tests/test_large_scale_density_spherical_annulus.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/large_scale_density/tests/test_large_scale_density_spherical_volume.py` & `halotools-0.8.2/halotools/mock_observables/large_scale_density/tests/test_large_scale_density_spherical_volume.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/mock_observables_helpers.py` & `halotools-0.8.2/halotools/mock_observables/mock_observables_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/mock_survey.py` & `halotools-0.8.2/halotools/mock_observables/mock_survey.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/occupation_stats.py` & `halotools-0.8.2/halotools/mock_observables/occupation_stats.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/__init__.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/__init__.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/README.md` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/README.md`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/__init__.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/__init__.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/distances.pxd` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/distances.pxd`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/distances.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/distances.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_3d_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_3d_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_jackknife_3d_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_jackknife_3d_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_jackknife_xy_z_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_jackknife_xy_z_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_per_object_3d_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_per_object_3d_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_projected_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_projected_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_s_mu_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_s_mu_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/npairs_xy_z_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/npairs_xy_z_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/pairwise_distance_3d_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/pairwise_distance_3d_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/pairwise_distance_xy_z_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/pairwise_distance_xy_z_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/pairwise_distances.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/pairwise_distances.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/setup_package.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/setup_package.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/cpairs/weighted_npairs_s_mu_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/cpairs/weighted_npairs_s_mu_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/README.md` & `halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/README.md`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/conditional_pairwise_distances.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/conditional_pairwise_distances.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/distances.pxd` & `halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/distances.pxd`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/distances.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/distances.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/marked_npairs_3d_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/marked_npairs_3d_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/marked_npairs_xy_z_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/marked_npairs_xy_z_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/marking_functions.pxd` & `halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/marking_functions.pxd`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/marking_functions.pyx` & `halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/marking_functions.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/marked_cpairs/setup_package.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/marked_cpairs/setup_package.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/marked_npairs_3d.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/marked_npairs_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/marked_npairs_xy_z.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/marked_npairs_xy_z.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/mesh_helpers.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/mesh_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_3d.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_jackknife_3d.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_jackknife_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_jackknife_xy_z.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_jackknife_xy_z.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_per_object_3d.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_per_object_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_projected.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_projected.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_s_mu.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_s_mu.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/npairs_xy_z.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/npairs_xy_z.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/pairs.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/pairs.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/pairwise_distance_3d.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/pairwise_distance_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/pairwise_distance_xy_z.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/pairwise_distance_xy_z.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/rectangular_mesh.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/rectangular_mesh.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/rectangular_mesh_2d.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/rectangular_mesh_2d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/pure_python_distance_matrix.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/pure_python_distance_matrix.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/pure_python_npairs_per_object_3d.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/pure_python_npairs_per_object_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_marked_npairs_3d.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_marked_npairs_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_marked_npairs_xy_z.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_marked_npairs_xy_z.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_mesh_helpers.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_mesh_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_non_cubic_volumes.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_non_cubic_volumes.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_3d.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_jackknife_3d.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_jackknife_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_jackknife_xy_z.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_jackknife_xy_z.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_per_object_3d.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_per_object_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_projected.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_projected.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_s_mu.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_s_mu.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_xy_z.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_npairs_xy_z.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_pairwise_distance_3d.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_pairwise_distance_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_rectangular_mesh.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_rectangular_mesh.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_weighted_npairs_s_mu.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_weighted_npairs_s_mu.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/test_pair_counters/test_wnpairs_pure_python.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/test_pair_counters/test_wnpairs_pure_python.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pair_counters/weighted_npairs_s_mu.py` & `halotools-0.8.2/halotools/mock_observables/pair_counters/weighted_npairs_s_mu.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/__init__.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/__init__.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/mean_radial_velocity_vs_r_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/mean_radial_velocity_vs_r_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/radial_pvd_vs_r_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/radial_pvd_vs_r_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/setup_package.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/setup_package.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/velocity_marked_npairs_3d_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/velocity_marked_npairs_3d_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/velocity_marked_npairs_xy_z_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/velocity_marked_npairs_xy_z_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/velocity_marking_functions.pxd` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/velocity_marking_functions.pxd`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/engines/velocity_marking_functions.pyx` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/engines/velocity_marking_functions.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/los_pvd_vs_rp.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/los_pvd_vs_rp.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/mean_los_velocity_vs_rp.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/mean_los_velocity_vs_rp.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/mean_radial_velocity_vs_r.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/mean_radial_velocity_vs_r.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/pairwise_velocities_helpers.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/pairwise_velocities_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/radial_pvd_vs_r.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/radial_pvd_vs_r.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/pure_python_mean_radial_velocity_vs_r.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/pure_python_mean_radial_velocity_vs_r.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_los_pvd_vs_rp.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_los_pvd_vs_rp.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_mean_los_velocity_vs_rp.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_mean_los_velocity_vs_rp.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_mean_radial_velocity_vs_r.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_mean_radial_velocity_vs_r.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_pairwise_velocity_helpers.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_pairwise_velocity_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_pairwise_velocity_stats.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_pairwise_velocity_stats.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_pure_python_mean_radial_velocity_vs_r.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_pure_python_mean_radial_velocity_vs_r.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_radial_pvd_vs_r.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_radial_pvd_vs_r.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/tests/test_velocity_marked_npairs_3d.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/tests/test_velocity_marked_npairs_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/velocity_marked_npairs_3d.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/velocity_marked_npairs_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/pairwise_velocities/velocity_marked_npairs_xy_z.py` & `halotools-0.8.2/halotools/mock_observables/pairwise_velocities/velocity_marked_npairs_xy_z.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/radial_profiles/engines/radial_profile_3d_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/radial_profiles/engines/radial_profile_3d_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/radial_profiles/engines/setup_package.py` & `halotools-0.8.2/halotools/mock_observables/radial_profiles/engines/setup_package.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/radial_profiles/radial_profile_3d.py` & `halotools-0.8.2/halotools/mock_observables/radial_profiles/radial_profile_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/radial_profiles/radial_profiles_helpers.py` & `halotools-0.8.2/halotools/mock_observables/radial_profiles/radial_profiles_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/radial_profiles/tests/test_radial_profile_3d.py` & `halotools-0.8.2/halotools/mock_observables/radial_profiles/tests/test_radial_profile_3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/engines/mean_delta_sigma_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/surface_density/engines/mean_delta_sigma_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/engines/mean_ds_one_two_halo_decomp_halo_id_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/surface_density/engines/mean_ds_one_two_halo_decomp_halo_id_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/engines/mean_ds_one_two_halo_decomp_rhalo_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/surface_density/engines/mean_ds_one_two_halo_decomp_rhalo_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/engines/setup_package.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/engines/setup_package.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/engines/weighted_npairs_per_object_xy_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/surface_density/engines/weighted_npairs_per_object_xy_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/engines/weighted_npairs_xy_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/surface_density/engines/weighted_npairs_xy_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/mass_in_cylinders.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/mass_in_cylinders.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/mean_delta_sigma.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/mean_delta_sigma.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/surface_density.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/surface_density.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/surface_density_helpers.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/surface_density_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/tests/pure_python_weighted_npairs_per_object_xy.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/tests/pure_python_weighted_npairs_per_object_xy.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/tests/pure_python_weighted_npairs_xy.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/tests/pure_python_weighted_npairs_xy.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_mass_in_cylinders.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_mass_in_cylinders.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_mean_delta_sigma.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_mean_delta_sigma.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_pure_python_weighted_npairs_xy.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_pure_python_weighted_npairs_xy.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_surface_density.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_surface_density.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_surface_density_helpers.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_surface_density_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_weighted_npairs_per_object_xy.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_weighted_npairs_per_object_xy.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/tests/test_weighted_npairs_xy.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/tests/test_weighted_npairs_xy.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/weighted_npairs_per_object_xy.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/weighted_npairs_per_object_xy.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/surface_density/weighted_npairs_xy.py` & `halotools-0.8.2/halotools/mock_observables/surface_density/weighted_npairs_xy.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/tensor_calculations/engines/inertia_tensor_3d_engine.pyx` & `halotools-0.8.2/halotools/mock_observables/tensor_calculations/engines/inertia_tensor_3d_engine.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/tensor_calculations/engines/setup_package.py` & `halotools-0.8.2/halotools/mock_observables/tensor_calculations/engines/setup_package.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/tensor_calculations/inertia_tensor.py` & `halotools-0.8.2/halotools/mock_observables/tensor_calculations/inertia_tensor.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/tensor_calculations/tensor_derived_quantities.py` & `halotools-0.8.2/halotools/mock_observables/tensor_calculations/tensor_derived_quantities.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/tensor_calculations/tests/test_inertia_tensor.py` & `halotools-0.8.2/halotools/mock_observables/tensor_calculations/tests/test_inertia_tensor.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/tensor_calculations/tests/test_tensor_derived_quantities.py` & `halotools-0.8.2/halotools/mock_observables/tensor_calculations/tests/test_tensor_derived_quantities.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/tests/cf_helpers.py` & `halotools-0.8.2/halotools/mock_observables/tests/cf_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/tests/test_catalog_analysis_helpers.py` & `halotools-0.8.2/halotools/mock_observables/tests/test_catalog_analysis_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,28 +2,24 @@
 `~halotools.mock_observables.catalog_analysis_helpers` module.
 """
 from __future__ import absolute_import, division, print_function
 
 from unittest import TestCase
 
 import numpy as np
-
 import pytest
 from astropy.utils.misc import NumpyRNGContext
 
+from ...custom_exceptions import HalotoolsError
+from ...sim_manager import FakeSim
 from .. import catalog_analysis_helpers as cat_helpers
 from ..catalog_analysis_helpers import cuboid_subvolume_labels
-
-from ...sim_manager import FakeSim
-
 from .cf_helpers import generate_locus_of_3d_points
 
-from ...custom_exceptions import HalotoolsError
-
-__all__ = ('TestCatalogAnalysisHelpers', )
+__all__ = ("TestCatalogAnalysisHelpers",)
 
 fixed_seed = 43
 
 
 def test_cuboid_subvolume_labels_bounds_checking():
     Npts = 100
     with NumpyRNGContext(fixed_seed):
@@ -84,285 +80,343 @@
     assert np.all(s == [1, 0, -1, -1, 1])
 
     s = cat_helpers.sign_pbc(x1, x2, equality_fill_val=9)
     assert np.all(s == [1, 9, -1, -1, 1])
 
 
 def test_sign_pbc2():
-    x1 = np.array((1, 4, 6, 9.))
+    x1 = np.array((1, 4, 6, 9.0))
 
     x2 = np.array((0, 3, 5, 8))
     s = cat_helpers.sign_pbc(x1, x2, period=10)
-    assert np.all(s == [1, 1, 1., 1])
+    assert np.all(s == [1, 1, 1.0, 1])
 
 
 def test_sign_pbc3():
-    x1 = np.array((1, 4, 6, 9.))
+    x1 = np.array((1, 4, 6, 9.0))
     x2 = np.array((9, 9.9, 0, 0))
 
     s = cat_helpers.sign_pbc(x1, x2, period=10)
     assert np.all(s == (1, 1, -1, -1))
 
     s = cat_helpers.sign_pbc(x1, x2)
     assert np.all(s == (-1, -1, 1, 1))
 
 
 def test_sign_pbc_catches_out_of_bounds():
-    x1 = np.array((1, 4, 6, 9.))
+    x1 = np.array((1, 4, 6, 9.0))
 
     x2 = np.array((2, 5, 7, 10))
     with pytest.raises(ValueError) as err:
         __ = cat_helpers.sign_pbc(x1, x2, period=10)
     substr = "If period is not None, all values of x and y must be between [0, period)"
     assert substr in err.value.args[0]
 
     s = cat_helpers.sign_pbc(x1, x2)
     assert np.all(s == (-1, -1, -1, -1))
 
 
 def test_relative_positions_and_velocities_catches_out_of_bounds():
-    x1 = np.array((1, 4, 6, 10.))
+    x1 = np.array((1, 4, 6, 10.0))
     x2 = x1
     with pytest.raises(ValueError) as err:
         __ = cat_helpers.relative_positions_and_velocities(x1, x2, period=10)
     substr = "If period is not None, all values of x and y must be between [0, period)"
     assert substr in err.value.args[0]
 
 
 def test_relative_positions_and_velocities1():
-    """ In this test, x1 > x2 and PBCs are irrelevant
-    """
+    """In this test, x1 > x2 and PBCs are irrelevant"""
     period = 10
-    x1 = np.array((1, 4, 6, 9.))
+    x1 = np.array((1, 4, 6, 9.0))
     x2 = x1 - 1
     result = cat_helpers.relative_positions_and_velocities(x1, x2, period=period)
     assert np.all(result == np.ones(len(x1)))
     result = cat_helpers.relative_positions_and_velocities(x1, x2)
     assert np.all(result == np.ones(len(x1)))
 
 
 def test_relative_positions_and_velocities2():
-    """ In this test, x1 > x2 and PBCs impact the results
-    """
+    """In this test, x1 > x2 and PBCs impact the results"""
     period = 10
-    x1 = np.array((1, 4, 6, 9.))
+    x1 = np.array((1, 4, 6, 9.0))
     x2 = np.mod(x1 - 1 + period, period)
     result = cat_helpers.relative_positions_and_velocities(x1, x2, period=period)
     assert np.all(result == np.ones(len(x1)))
 
 
 def test_relative_positions_and_velocities3():
-    """ In this test, x1 < x2 and PBCs are irrelevant
-    """
+    """In this test, x1 < x2 and PBCs are irrelevant"""
     period = 100
-    x1 = np.array((1, 4, 6, 9.))
+    x1 = np.array((1, 4, 6, 9.0))
     x2 = x1 + 1
     result = cat_helpers.relative_positions_and_velocities(x1, x2, period=period)
     assert np.all(result == -np.ones(len(x1)))
     result = cat_helpers.relative_positions_and_velocities(x1, x2)
     assert np.all(result == -np.ones(len(x1)))
 
 
 def test_relative_positions_and_velocities4():
-    """ In this test, x1 < x2 and PBCs impact the results
-    """
+    """In this test, x1 < x2 and PBCs impact the results"""
     period = 10
-    x1 = np.array((1, 4, 6, 9.))
+    x1 = np.array((1, 4, 6, 9.0))
     x2 = np.zeros(len(x1))
     result = cat_helpers.relative_positions_and_velocities(x1, x2, period=period)
     assert np.all(result == np.array((1, 4, -4, -1)))
     result = cat_helpers.relative_positions_and_velocities(x1, x2)
     assert np.all(result == x1)
 
 
 def test_relative_velocities1():
-    """ In this test, x1 > x2 and PBCs are irrelevant
-    """
+    """In this test, x1 > x2 and PBCs are irrelevant"""
     period = 100
     x1 = np.array((9, 9, 9, 9))
     x2 = x1 - 1
     v1 = np.array((100, 100, 100, 100))
     v2 = np.array((-100, -10, 90, 110))
-    xrel, vrel = cat_helpers.relative_positions_and_velocities(x1, x2, period=period, v1=v1, v2=v2)
+    xrel, vrel = cat_helpers.relative_positions_and_velocities(
+        x1, x2, period=period, v1=v1, v2=v2
+    )
     assert np.all(vrel == (200, 110, 10, -10))
     xrel, vrel = cat_helpers.relative_positions_and_velocities(x1, x2, v1=v1, v2=v2)
     assert np.all(vrel == (200, 110, 10, -10))
 
 
 def test_relative_velocities2():
-    """ In this test, x1 > x2 and PBCs impact the results
-    """
+    """In this test, x1 > x2 and PBCs impact the results"""
     period = 10
     x1 = np.array((9, 9, 9, 9))
     x2 = np.zeros(len(x1))
     v1 = np.array((100, 100, 100, 100))
     v2 = np.array((-100, -10, 90, 110))
     correct_result = np.array((-200, -110, -10, 10))
-    xrel, vrel = cat_helpers.relative_positions_and_velocities(x1, x2, period=period, v1=v1, v2=v2)
+    xrel, vrel = cat_helpers.relative_positions_and_velocities(
+        x1, x2, period=period, v1=v1, v2=v2
+    )
     assert np.all(vrel == correct_result)
     xrel, vrel = cat_helpers.relative_positions_and_velocities(x1, x2, v1=v1, v2=v2)
     assert np.all(vrel == -correct_result)
 
 
 def test_relative_velocities3():
-    """ In this test, x1 < x2 and PBCs are irrelevant
-    """
+    """In this test, x1 < x2 and PBCs are irrelevant"""
     period = 100
     x1 = np.array((9, 9, 9, 9))
     x2 = x1 + 1
     v1 = np.array((100, 100, 100, 100))
     v2 = np.array((-100, -10, 90, 110))
-    xrel, vrel = cat_helpers.relative_positions_and_velocities(x1, x2, period=period, v1=v1, v2=v2)
+    xrel, vrel = cat_helpers.relative_positions_and_velocities(
+        x1, x2, period=period, v1=v1, v2=v2
+    )
     correct_result = np.array((-200, -110, -10, 10))
     assert np.all(vrel == correct_result)
     xrel, vrel = cat_helpers.relative_positions_and_velocities(x1, x2, v1=v1, v2=v2)
     assert np.all(vrel == correct_result)
 
 
 def test_relative_velocities4():
-    """ In this test, x1 < x2 and PBCs are irrelevant
-    """
+    """In this test, x1 < x2 and PBCs are irrelevant"""
     period = 10
     x1 = np.zeros(4)
-    x2 = np.zeros(4) + 9.
+    x2 = np.zeros(4) + 9.0
     v1 = np.array((100, 100, 100, 100))
     v2 = np.array((-100, -10, 90, 110))
-    xrel, vrel = cat_helpers.relative_positions_and_velocities(x1, x2, period=period, v1=v1, v2=v2)
+    xrel, vrel = cat_helpers.relative_positions_and_velocities(
+        x1, x2, period=period, v1=v1, v2=v2
+    )
     correct_result = np.array((200, 110, 10, -10))
     assert np.all(vrel == correct_result)
     xrel, vrel = cat_helpers.relative_positions_and_velocities(x1, x2, v1=v1, v2=v2)
     assert np.all(vrel == -correct_result)
 
 
 def test_return_xyz_formatted_array1():
     npts = 10
     period = [1, 2, 3]
-    x = np.linspace(0.001, period[0]-0.001, npts)
-    y = np.linspace(0.001, period[1]-0.001, npts)
-    z = np.linspace(0.001, period[2]-0.001, npts)
+    x = np.linspace(0.001, period[0] - 0.001, npts)
+    y = np.linspace(0.001, period[1] - 0.001, npts)
+    z = np.linspace(0.001, period[2] - 0.001, npts)
     v = np.zeros(npts)
     result1 = cat_helpers.return_xyz_formatted_array(x, y, z)
-    result2 = cat_helpers.return_xyz_formatted_array(x, y, z, velocity=v, velocity_distortion_dimension='x')
-    result3 = cat_helpers.return_xyz_formatted_array(x, y, z, velocity=v, velocity_distortion_dimension='y')
-    result4 = cat_helpers.return_xyz_formatted_array(x, y, z, velocity=v, velocity_distortion_dimension='z')
-    result5 = cat_helpers.return_xyz_formatted_array(x, y, z, velocity=v,
-        velocity_distortion_dimension='x', period=period)
-    result6 = cat_helpers.return_xyz_formatted_array(x, y, z, velocity=v,
-        velocity_distortion_dimension='y', period=period)
+    result2 = cat_helpers.return_xyz_formatted_array(
+        x, y, z, velocity=v, velocity_distortion_dimension="x"
+    )
+    result3 = cat_helpers.return_xyz_formatted_array(
+        x, y, z, velocity=v, velocity_distortion_dimension="y"
+    )
+    result4 = cat_helpers.return_xyz_formatted_array(
+        x, y, z, velocity=v, velocity_distortion_dimension="z"
+    )
+    result5 = cat_helpers.return_xyz_formatted_array(
+        x, y, z, velocity=v, velocity_distortion_dimension="x", period=period
+    )
+    result6 = cat_helpers.return_xyz_formatted_array(
+        x, y, z, velocity=v, velocity_distortion_dimension="y", period=period
+    )
 
     assert np.all(result1 == result2)
     assert np.all(result1 == result3)
     assert np.all(result1 == result4)
     assert np.all(result1 == result5)
     assert np.all(result1 == result6)
 
 
 def test_return_xyz_formatted_array2():
-    """ verify that redshift keyword is operative
-    """
+    """verify that redshift keyword is operative"""
     npts = int(1e4)
     x = np.linspace(0.001, 0.999, npts)
     y = np.linspace(0.001, 0.999, npts)
     z = np.linspace(0.001, 0.999, npts)
     v = np.random.normal(loc=0, scale=150, size=npts)
-    result_z0 = cat_helpers.return_xyz_formatted_array(x, y, z,
-        velocity=v, velocity_distortion_dimension='x', redshift=0)
-    result_z1 = cat_helpers.return_xyz_formatted_array(x, y, z,
-        velocity=v, velocity_distortion_dimension='x', redshift=1)
+    result_z0 = cat_helpers.return_xyz_formatted_array(
+        x, y, z, velocity=v, velocity_distortion_dimension="x", redshift=0
+    )
+    result_z1 = cat_helpers.return_xyz_formatted_array(
+        x, y, z, velocity=v, velocity_distortion_dimension="x", redshift=1
+    )
     assert not np.all(result_z0 == result_z1)
 
 
 def test_return_xyz_formatted_array3():
-    """ verify that cosmology keyword is operative
-    """
+    """verify that cosmology keyword is operative"""
     npts = int(1e4)
     x = np.linspace(0.001, 0.999, npts)
     y = np.linspace(0.001, 0.999, npts)
     z = np.linspace(0.001, 0.999, npts)
     v = np.random.normal(loc=0, scale=150, size=npts)
 
     from astropy.cosmology import WMAP5, Planck15
-    result_z0a = cat_helpers.return_xyz_formatted_array(x, y, z,
-        velocity=v, velocity_distortion_dimension='x', redshift=0.5, cosmology=WMAP5)
-    result_z0b = cat_helpers.return_xyz_formatted_array(x, y, z,
-        velocity=v, velocity_distortion_dimension='x', redshift=0.5, cosmology=Planck15)
+
+    result_z0a = cat_helpers.return_xyz_formatted_array(
+        x,
+        y,
+        z,
+        velocity=v,
+        velocity_distortion_dimension="x",
+        redshift=0.5,
+        cosmology=WMAP5,
+    )
+    result_z0b = cat_helpers.return_xyz_formatted_array(
+        x,
+        y,
+        z,
+        velocity=v,
+        velocity_distortion_dimension="x",
+        redshift=0.5,
+        cosmology=Planck15,
+    )
     assert not np.all(result_z0a == result_z0b)
 
 
 def test_return_xyz_formatted_array4():
-    """ Verify consistent behavior between
+    """Verify consistent behavior between
     the `~halotools.mock_observables.return_xyz_formatted_array` function and the
     independently-written `~halotools.mock_observables.return_xyz_formatted_array` function.
     """
     npts = int(1e4)
     x = np.linspace(0.001, 0.999, npts)
     y = np.linspace(0.001, 0.999, npts)
     z = np.linspace(0.001, 0.999, npts)
     v = np.random.normal(loc=0, scale=0.5, size=npts)
 
     from astropy.cosmology import WMAP5
-    result1 = cat_helpers.return_xyz_formatted_array(x, y, z,
-        velocity=v, velocity_distortion_dimension='x', redshift=0.5, cosmology=WMAP5, period=1)
+
+    result1 = cat_helpers.return_xyz_formatted_array(
+        x,
+        y,
+        z,
+        velocity=v,
+        velocity_distortion_dimension="x",
+        redshift=0.5,
+        cosmology=WMAP5,
+        period=1,
+    )
 
     result2 = cat_helpers.apply_zspace_distortion(x, v, 0.5, WMAP5, Lbox=1)
     assert np.allclose(result1[:, 0], result2)
 
 
+def test_return_xyz_formatted_array_wraps_pbcs():
+    npts = int(1e4)
+    Lbox = 1.0
+    x = np.linspace(-2 * Lbox, 2 * Lbox, npts)
+    y = np.linspace(-2 * Lbox, 2 * Lbox, npts)
+    z = np.linspace(-2 * Lbox, 2 * Lbox, npts)
+
+    pos = cat_helpers.return_xyz_formatted_array(x, y, z, period=Lbox)
+    assert np.all(pos >= 0)
+    assert np.all(pos <= Lbox)
+
+
 class TestCatalogAnalysisHelpers(TestCase):
-    """ Class providing tests of the `~halotools.mock_observables.catalog_analysis_helpers`.
-    """
+    """Class providing tests of the `~halotools.mock_observables.catalog_analysis_helpers`."""
 
     def setUp(self):
-
         halocat = FakeSim()
         self.halo_table = halocat.halo_table
         self.Lbox = halocat.Lbox
 
     def test_mean_y_vs_x1(self):
         abscissa, mean, err = cat_helpers.mean_y_vs_x(
-            self.halo_table['halo_mvir'], self.halo_table['halo_spin'])
+            self.halo_table["halo_mvir"], self.halo_table["halo_spin"]
+        )
 
     def test_mean_y_vs_x2(self):
         abscissa, mean, err = cat_helpers.mean_y_vs_x(
-            self.halo_table['halo_mvir'], self.halo_table['halo_spin'],
-            error_estimator='variance')
+            self.halo_table["halo_mvir"],
+            self.halo_table["halo_spin"],
+            error_estimator="variance",
+        )
 
     def test_mean_y_vs_x3(self):
         with pytest.raises(HalotoolsError) as err:
             abscissa, mean, err = cat_helpers.mean_y_vs_x(
-                self.halo_table['halo_mvir'], self.halo_table['halo_spin'],
-                error_estimator='Jose Canseco')
+                self.halo_table["halo_mvir"],
+                self.halo_table["halo_spin"],
+                error_estimator="Jose Canseco",
+            )
         substr = "Input ``error_estimator`` must be either"
         assert substr in err.value.args[0]
 
     def test_return_xyz_formatted_array1(self):
-        x, y, z = (self.halo_table['halo_x'],
-            self.halo_table['halo_y'], self.halo_table['halo_z'])
+        x, y, z = (
+            self.halo_table["halo_x"],
+            self.halo_table["halo_y"],
+            self.halo_table["halo_z"],
+        )
         pos = cat_helpers.return_xyz_formatted_array(x, y, z)
         assert np.shape(pos) == (len(x), 3)
 
-        mask = self.halo_table['halo_mvir'] >= 10**13.5
+        mask = self.halo_table["halo_mvir"] >= 10**13.5
         masked_pos = cat_helpers.return_xyz_formatted_array(x, y, z, mask=mask)
         npts = len(self.halo_table[mask])
         assert np.shape(masked_pos) == (npts, 3)
 
         assert masked_pos.shape[0] < pos.shape[0]
 
         pos_zdist = cat_helpers.return_xyz_formatted_array(
-            x, y, z, velocity=self.halo_table['halo_vz'],
-            velocity_distortion_dimension='z')
+            x,
+            y,
+            z,
+            velocity=self.halo_table["halo_vz"],
+            velocity_distortion_dimension="z",
+        )
         assert np.all(pos_zdist[:, 0] == pos[:, 0])
         assert np.all(pos_zdist[:, 1] == pos[:, 1])
         assert np.any(pos_zdist[:, 2] != pos[:, 2])
         assert np.all(abs(pos_zdist[:, 2] - pos[:, 2]) < 50)
 
         pos_zdist_pbc = cat_helpers.return_xyz_formatted_array(
-            x, y, z, velocity=self.halo_table['halo_vz'],
-            velocity_distortion_dimension='z',
-            period=self.Lbox)
+            x,
+            y,
+            z,
+            velocity=self.halo_table["halo_vz"],
+            velocity_distortion_dimension="z",
+            period=self.Lbox,
+        )
         assert np.all(pos_zdist_pbc[:, 0] == pos[:, 0])
         assert np.all(pos_zdist_pbc[:, 1] == pos[:, 1])
         assert np.any(pos_zdist_pbc[:, 2] != pos[:, 2])
 
         assert np.any(abs(pos_zdist_pbc[:, 2] - pos[:, 2]) > 50)
 
     def tearDown(self):
```

### Comparing `halotools-0.8.1/halotools/mock_observables/tests/test_mock_observables_helpers.py` & `halotools-0.8.2/halotools/mock_observables/tests/test_mock_observables_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/tests/test_mock_survey.py` & `halotools-0.8.2/halotools/mock_observables/tests/test_mock_survey.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/tests/test_occupation_stats.py` & `halotools-0.8.2/halotools/mock_observables/tests/test_occupation_stats.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/__init__.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/angular_tpcf.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/angular_tpcf.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/clustering_helpers.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/clustering_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/marked_tpcf.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/marked_tpcf.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/rp_pi_tpcf.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/rp_pi_tpcf.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/rp_pi_tpcf_jackknife.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/rp_pi_tpcf_jackknife.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/s_mu_tpcf.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/s_mu_tpcf.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/locate_external_unit_testing_data.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/locate_external_unit_testing_data.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_angular_tpcf.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_angular_tpcf.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_clustering_helpers.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_clustering_helpers.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_marked_tpcf.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_marked_tpcf.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_rp_pi_tpcf.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_rp_pi_tpcf.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_rp_pi_tpcf_jackknife.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_rp_pi_tpcf_jackknife.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_s_mu_tpcf.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_s_mu_tpcf.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_tpcf.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_tpcf.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_tpcf_estimators.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_tpcf_estimators.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_tpcf_jackknife.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_tpcf_jackknife.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_tpcf_multipole.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_tpcf_multipole.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_tpcf_one_two_halo.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_tpcf_one_two_halo.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_wp.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_wp.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tests/test_wp_jackknife.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tests/test_wp_jackknife.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tpcf.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tpcf.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tpcf_estimators.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tpcf_estimators.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tpcf_jackknife.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tpcf_jackknife.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tpcf_multipole.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tpcf_multipole.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/tpcf_one_two_halo_decomp.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/tpcf_one_two_halo_decomp.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/wp.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/wp.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/two_point_clustering/wp_jackknife.py` & `halotools-0.8.2/halotools/mock_observables/two_point_clustering/wp_jackknife.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/velocity_decomposition/radial_velocity_decomposition.py` & `halotools-0.8.2/halotools/mock_observables/velocity_decomposition/radial_velocity_decomposition.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/velocity_decomposition/tests/test_radial_velocity.py` & `halotools-0.8.2/halotools/mock_observables/velocity_decomposition/tests/test_radial_velocity.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/void_statistics/tests/test_underdensity_prob_func.py` & `halotools-0.8.2/halotools/mock_observables/void_statistics/tests/test_underdensity_prob_func.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/void_statistics/tests/test_void_prob_func.py` & `halotools-0.8.2/halotools/mock_observables/void_statistics/tests/test_void_prob_func.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/void_statistics/underdensity_prob_func.py` & `halotools-0.8.2/halotools/mock_observables/void_statistics/underdensity_prob_func.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/mock_observables/void_statistics/void_prob_func.py` & `halotools-0.8.2/halotools/mock_observables/void_statistics/void_prob_func.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/__init__.py` & `halotools-0.8.2/halotools/sim_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/cached_halo_catalog.py` & `halotools-0.8.2/halotools/sim_manager/cached_halo_catalog.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/download_manager.py` & `halotools-0.8.2/halotools/sim_manager/download_manager.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/fake_sim.py` & `halotools-0.8.2/halotools/sim_manager/fake_sim.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/halo_table_cache.py` & `halotools-0.8.2/halotools/sim_manager/halo_table_cache.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/halo_table_cache_log_entry.py` & `halotools-0.8.2/halotools/sim_manager/halo_table_cache_log_entry.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/ptcl_table_cache.py` & `halotools-0.8.2/halotools/sim_manager/ptcl_table_cache.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/ptcl_table_cache_log_entry.py` & `halotools-0.8.2/halotools/sim_manager/ptcl_table_cache_log_entry.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/rockstar_hlist_reader.py` & `halotools-0.8.2/halotools/sim_manager/rockstar_hlist_reader.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/sim_defaults.py` & `halotools-0.8.2/halotools/sim_manager/sim_defaults.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/supported_sims.py` & `halotools-0.8.2/halotools/sim_manager/supported_sims.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tabular_ascii_reader.py` & `halotools-0.8.2/halotools/sim_manager/tabular_ascii_reader.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/data/dummy_halocat_0.07812.list` & `halotools-0.8.2/halotools/sim_manager/tests/data/dummy_halocat_0.07812.list`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/helper_functions.py` & `halotools-0.8.2/halotools/sim_manager/tests/helper_functions.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_cached_halo_catalog.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_cached_halo_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 """
 """
 from __future__ import absolute_import, division, print_function
 
-from unittest import TestCase
 import os
 import shutil
+from unittest import TestCase
 
 from astropy.config.paths import _find_home
-from astropy.tests.helper import pytest
 from astropy.table import Table
+from astropy.tests.helper import pytest
 
 try:
     import h5py
 
     HAS_H5PY = True
 except ImportError:
     HAS_H5PY = False
 
 import numpy as np
 
-from . import helper_functions
-
-from ..cached_halo_catalog import CachedHaloCatalog
-from ..halo_table_cache import HaloTableCache
-from ..ptcl_table_cache import PtclTableCache
-from ..download_manager import DownloadManager
+from ...custom_exceptions import HalotoolsError, InvalidCacheLogEntry
 from ...utils.python_string_comparisons import (
-    compare_strings_py23_safe,
     _passively_decode_string,
+    compare_strings_py23_safe,
 )
-from ...custom_exceptions import HalotoolsError, InvalidCacheLogEntry
+from ..cached_halo_catalog import CachedHaloCatalog
+from ..download_manager import DownloadManager
+from ..halo_table_cache import HaloTableCache
+from ..ptcl_table_cache import PtclTableCache
+from . import helper_functions
 
 # Determine whether the machine is mine
 # This will be used to select tests whose
 # returned values depend on the configuration
 # of my personal cache directory files
 aph_home = "/Users/aphearin"
 detected_home = _find_home()
@@ -350,15 +349,14 @@
     def test_acceptable_arguments6(self):
         cache = HaloTableCache()
         fname = cache.log[0].fname
         halocat = CachedHaloCatalog(fname=fname)
 
     @pytest.mark.skipif("not APH_MACHINE")
     def test_relocate_simulation_data(self):
-
         dman = DownloadManager()
         cache = HaloTableCache()
 
         ######################################################
         # Make sure the file does not already exist on disk or in cache
         tmp_fname = "/Users/aphearin/.astropy/cache/halotools/halo_catalogs/bolshoi/rockstar/hlist_0.07835.list.halotools_alpha_version2.hdf5"
 
@@ -491,15 +489,14 @@
                 redshift=11.7632,
             )
         # ######################################################
 
     @pytest.mark.skipif("not HAS_H5PY")
     @pytest.mark.skipif("not APH_MACHINE")
     def test_user_supplied_ptcl_consistency(self):
-
         from ..user_supplied_ptcl_catalog import UserSuppliedPtclCatalog
 
         halocat = CachedHaloCatalog()
 
         ptclcat = UserSuppliedPtclCatalog(
             redshift=halocat.redshift,
             Lbox=halocat.Lbox,
```

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_download_manager.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_download_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """ Module providing unit-testing for `~halotools.sim_manager.DownloadManager`.
 """
 
 import os
 import shutil
+from unittest import TestCase
+
 import numpy as np
 from astropy.config.paths import _find_home
-from astropy.tests.helper import pytest
 from astropy.table import Table
-from unittest import TestCase
+from astropy.tests.helper import pytest
 
+from ...custom_exceptions import HalotoolsError
+from .. import sim_defaults
 from ..download_manager import DownloadManager
 from ..halo_table_cache import HaloTableCache
-from .. import sim_defaults
-from ...custom_exceptions import HalotoolsError
 
 # Determine whether the machine is mine
 # This will be used to select tests whose
 # returned values depend on the configuration
 # of my personal cache directory files
 aph_home = "/Users/aphearin"
 detected_home = _find_home()
@@ -27,21 +28,19 @@
 
 
 __all__ = ("TestDownloadManager",)
 
 
 class TestDownloadManager(TestCase):
     def setUp(self):
-
         homedir = _find_home()
 
         self.downman = DownloadManager()
 
         def defensively_create_empty_dir(dirname):
-
             if os.path.isdir(dirname) is False:
                 os.mkdir(dirname)
             else:
                 shutil.rmtree(dirname)
                 os.mkdir(dirname)
 
         # First create an empty directory where we will
@@ -139,15 +138,14 @@
         full_fname = os.path.join(p, f)
         assert os.path.isfile(full_fname)
 
         self.clear_APH_MACHINE_of_highz_file()
 
     @pytest.mark.skipif("not APH_MACHINE")
     def test_ptcl_tables_available_for_download(self):
-
         file_list = self.downman._ptcl_tables_available_for_download(simname="bolshoi")
         assert len(file_list) == 1
         assert "hlist_1.00035.particles.halotools_v0p4.hdf5" == os.path.basename(
             file_list[0]
         )
 
         file_list = self.downman._ptcl_tables_available_for_download(
@@ -184,31 +182,28 @@
         )
         assert len(file_list) == 4
         file_set = set([os.path.basename(f) for f in file_list])
         assert file_set == bolplanck_set
 
     @pytest.mark.skipif("not APH_MACHINE")
     def test_processed_halo_tables_available_for_download1(self):
-
         file_list = self.downman._processed_halo_tables_available_for_download(
             simname="bolshoi", halo_finder="rockstar"
         )
         assert file_list != []
 
     @pytest.mark.skipif("not APH_MACHINE")
     def test_processed_halo_tables_available_for_download2(self):
-
         file_list = self.downman._processed_halo_tables_available_for_download(
             simname="bolshoi"
         )
         assert file_list != []
 
     @pytest.mark.skipif("not APH_MACHINE")
     def test_processed_halo_tables_available_for_download3(self):
-
         file_list = self.downman._processed_halo_tables_available_for_download(
             halo_finder="bdm"
         )
         assert file_list != []
 
     @pytest.mark.skipif("not APH_MACHINE")
     def test_ptcl_tables_available_for_download2(self):
@@ -346,15 +341,14 @@
         fname, redshift = self.downman._closest_catalog_on_web(
             simname="bolplanck", desired_redshift=2, catalog_type="particles"
         )
         assert "bolplanck/hlist_0.33406.particles.halotools_v0p4.hdf5" in fname
 
     @classmethod
     def clear_APH_MACHINE_of_highz_file(self, delete_corresponding_halo_catalog=True):
-
         cache = HaloTableCache()
         matching_log_entries = cache.matching_log_entry_generator(
             simname="bolshoi",
             halo_finder="rockstar",
             version_name="halotools_alpha_version2",
             redshift=11.7,
             dz_tol=0.2,
```

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_fake_sim.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_fake_sim.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_halo_table_cache.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_halo_table_cache.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_halo_table_cache_log_entry.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_halo_table_cache_log_entry.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_load_default_halocat.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_load_default_halocat.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_ptcl_table_cache.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_ptcl_table_cache.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_ptcl_table_cache_log_entry.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_ptcl_table_cache_log_entry.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_rockstar_hlist_reader.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_rockstar_hlist_reader.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_supported_sims.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_supported_sims.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,110 +1,117 @@
 """
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import numpy as np
-
-from astropy.config.paths import _find_home
 import pytest
-
-from ..cached_halo_catalog import CachedHaloCatalog, InvalidCacheLogEntry
+from astropy.config.paths import _find_home
 
 from ...custom_exceptions import HalotoolsError
+from ..cached_halo_catalog import CachedHaloCatalog, InvalidCacheLogEntry
 
 slow = pytest.mark.slow
 
-aph_home = '/Users/aphearin'
+aph_home = "/Users/aphearin"
 detected_home = _find_home()
 if aph_home == detected_home:
     APH_MACHINE = True
 else:
     APH_MACHINE = False
 
 try:
     import h5py
+
     HAS_H5PY = True
 except ImportError:
     HAS_H5PY = False
 
-__all__ = ('test_load_halo_catalogs', 'test_halo_rvir_in_correct_units')
+__all__ = ("test_load_halo_catalogs", "test_halo_rvir_in_correct_units")
 
-adict = {'bolshoi': [0.33035, 0.54435, 0.67035, 1], 'bolplanck': [0.33406, 0.50112, 0.67, 1],
-    'consuelo': [0.333, 0.506, 0.6754, 1], 'multidark': [0.318, 0.5, 0.68, 1]}
+adict = {
+    "bolshoi": [0.33035, 0.54435, 0.67035, 1],
+    "bolplanck": [0.33406, 0.50112, 0.67, 1],
+    "consuelo": [0.333, 0.506, 0.6754, 1],
+    "multidark": [0.318, 0.5, 0.68, 1],
+}
 
 
 @pytest.mark.slow
-@pytest.mark.skipif('not APH_MACHINE')
+@pytest.mark.skipif("not APH_MACHINE")
 def test_load_halo_catalogs():
-    """
-    """
+    """ """
 
     for simname in list(adict.keys()):
         alist = adict[simname]
         for a in alist:
-            z = 1/a - 1
+            z = 1 / a - 1
             halocat = CachedHaloCatalog(simname=simname, redshift=z)
             assert np.allclose(halocat.redshift, z, atol=0.01)
 
-            if simname not in ['bolshoi', 'multidark']:
+            if simname not in ["bolshoi", "multidark"]:
                 particles = halocat.ptcl_table
             else:
                 if a == 1:
                     particles = halocat.ptcl_table
 
 
 @pytest.mark.slow
-@pytest.mark.skipif('not APH_MACHINE')
+@pytest.mark.skipif("not APH_MACHINE")
 def test_halo_rvir_in_correct_units():
-    """ Loop over all halo catalogs in cache and verify that the
+    """Loop over all halo catalogs in cache and verify that the
     ``halo_rvir`` column never exeeds the number 50. This is a crude way of
     ensuring that units are in Mpc/h, not kpc/h.
     """
     for simname in list(adict.keys()):
         alist = adict[simname]
         a = alist[0]
-        z = 1/a - 1
+        z = 1 / a - 1
         halocat = CachedHaloCatalog(simname=simname, redshift=z)
-        r = halocat.halo_table['halo_rvir']
-        assert np.all(r < 50.)
+        r = halocat.halo_table["halo_rvir"]
+        assert np.all(r < 50.0)
 
 
 def test_bolplanck_particle_mass():
-    """ This is a regression test for https://github.com/astropy/halotools/issues/576
+    """This is a regression test for https://github.com/astropy/halotools/issues/576
 
     This test should never be deleted or refactored.
     """
     from ..supported_sims import BolPlanck
+
     bp = BolPlanck()
     assert np.allclose(bp.particle_mass, 1.55e8, rtol=0.01)
 
 
-@pytest.mark.skipif('not HAS_H5PY')
+@pytest.mark.skipif("not HAS_H5PY")
 def test_forbidden_sims():
-    """ This is a regression test that ensures no one will use the
+    """This is a regression test that ensures no one will use the
     z = 0 halotools_alpha_version2 halo catalog.
 
     This test should never be deleted or refactored.
     """
     with pytest.raises(HalotoolsError) as err:
-        __ = CachedHaloCatalog(simname='bolplanck', version_name='halotools_alpha_version2')
+        __ = CachedHaloCatalog(
+            simname="bolplanck", version_name="halotools_alpha_version2"
+        )
     substr = "See https://github.com/astropy/halotools/issues/598"
     assert substr in err.value.args[0]
 
 
 def test_lbox_vector():
-    """ Ensure that the Lbox attribute of CachedHaloCatalog instances
+    """Ensure that the Lbox attribute of CachedHaloCatalog instances
     is always a 3-element vector.
     """
     for simname in list(adict.keys()):
         alist = adict[simname]
         a = alist[0]
-        z = 1/a - 1
+        z = 1 / a - 1
         try:
             halocat = CachedHaloCatalog(simname=simname, redshift=z)
             assert len(halocat.Lbox) == 3
         except (InvalidCacheLogEntry, HalotoolsError, AssertionError):
             if APH_MACHINE:
-                raise HalotoolsError("APH_MACHINE should never fail Lbox_vector test\n"
-                    "simname = {0}\nscale factor = {1}".format(simname, a))
+                raise HalotoolsError(
+                    "APH_MACHINE should never fail Lbox_vector test\n"
+                    "simname = {0}\nscale factor = {1}".format(simname, a)
+                )
             else:
                 pass
```

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_tabular_ascii_reader.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_tabular_ascii_reader.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_user_supplied_halo_catalog.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_user_supplied_halo_catalog.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/tests/test_user_supplied_ptcl_catalog.py` & `halotools-0.8.2/halotools/sim_manager/tests/test_user_supplied_ptcl_catalog.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/user_supplied_halo_catalog.py` & `halotools-0.8.2/halotools/sim_manager/user_supplied_halo_catalog.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/sim_manager/user_supplied_ptcl_catalog.py` & `halotools-0.8.2/halotools/sim_manager/user_supplied_ptcl_catalog.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/tests/coveragerc` & `halotools-0.8.2/halotools/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/tests/docs_code_block_tests/test_hod_model_factory_tutorial.py` & `halotools-0.8.2/halotools/tests/docs_code_block_tests/test_hod_model_factory_tutorial.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/tests/docs_code_block_tests/test_preloaded_mockpop.py` & `halotools-0.8.2/halotools/tests/docs_code_block_tests/test_preloaded_mockpop.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/tests/test_amurrica.py` & `halotools-0.8.2/halotools/tests/test_amurrica.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/tests/test_seed.py` & `halotools-0.8.2/halotools/tests/test_seed.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/__init__.py` & `halotools-0.8.2/halotools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/array_indexing_manipulations.py` & `halotools-0.8.2/halotools/utils/array_indexing_manipulations.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/array_utils.py` & `halotools-0.8.2/halotools/utils/array_utils.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/conditional_percentile.py` & `halotools-0.8.2/halotools/utils/conditional_percentile.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/crossmatch.py` & `halotools-0.8.2/halotools/utils/crossmatch.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/distribution_matching.py` & `halotools-0.8.2/halotools/utils/distribution_matching.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/engines/conditional_rank_kernel.pyx` & `halotools-0.8.2/halotools/utils/engines/conditional_rank_kernel.pyx`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/engines/setup_package.py` & `halotools-0.8.2/halotools/utils/engines/setup_package.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/group_member_generator.py` & `halotools-0.8.2/halotools/utils/group_member_generator.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/inverse_transformation_sampling.py` & `halotools-0.8.2/halotools/utils/inverse_transformation_sampling.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/io_utils.py` & `halotools-0.8.2/halotools/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/load_umachine_binaries.py` & `halotools-0.8.2/halotools/utils/load_umachine_binaries.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/mcrotations.py` & `halotools-0.8.2/halotools/utils/mcrotations.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/probabilistic_binning.py` & `halotools-0.8.2/halotools/utils/probabilistic_binning.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/rotations2d.py` & `halotools-0.8.2/halotools/utils/rotations2d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/rotations3d.py` & `halotools-0.8.2/halotools/utils/rotations3d.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/spherical_geometry.py` & `halotools-0.8.2/halotools/utils/spherical_geometry.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/table_utils.py` & `halotools-0.8.2/halotools/utils/table_utils.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_2d_rotations.py` & `halotools-0.8.2/halotools/utils/tests/test_2d_rotations.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_3d_rotations.py` & `halotools-0.8.2/halotools/utils/tests/test_3d_rotations.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_array_indexing_manipulations.py` & `halotools-0.8.2/halotools/utils/tests/test_array_indexing_manipulations.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_array_utils.py` & `halotools-0.8.2/halotools/utils/tests/test_array_utils.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_compute_richness.py` & `halotools-0.8.2/halotools/utils/tests/test_compute_richness.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_conditional_percentile.py` & `halotools-0.8.2/halotools/utils/tests/test_conditional_percentile.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_crossmatch.py` & `halotools-0.8.2/halotools/utils/tests/test_crossmatch.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_distribution_matching.py` & `halotools-0.8.2/halotools/utils/tests/test_distribution_matching.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_group_member_generator.py` & `halotools-0.8.2/halotools/utils/tests/test_group_member_generator.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_its.py` & `halotools-0.8.2/halotools/utils/tests/test_its.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_mcrotations.py` & `halotools-0.8.2/halotools/utils/tests/test_mcrotations.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_probabilistic_binning.py` & `halotools-0.8.2/halotools/utils/tests/test_probabilistic_binning.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_rotate_vector_collection.py` & `halotools-0.8.2/halotools/utils/tests/test_rotate_vector_collection.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_table_utils.py` & `halotools-0.8.2/halotools/utils/tests/test_table_utils.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_value_added_halo_table_functions.py` & `halotools-0.8.2/halotools/utils/tests/test_value_added_halo_table_functions.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/tests/test_vector_utilities.py` & `halotools-0.8.2/halotools/utils/tests/test_vector_utilities.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/value_added_halo_table_functions.py` & `halotools-0.8.2/halotools/utils/value_added_halo_table_functions.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools/utils/vector_utilities.py` & `halotools-0.8.2/halotools/utils/vector_utilities.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/halotools.egg-info/PKG-INFO` & `halotools-0.8.2/halotools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halotools
-Version: 0.8.1
+Version: 0.8.2
 Summary: Package designed to analyze N-body simulations and constrain models of cosmology and galaxy evolution.
 Home-page: http://astropy.org
 Author: Andrew Hearin
 Author-email: ahearin@anl.gov
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
@@ -161,8 +161,9 @@
            adsurl = {https://ui.adsabs.harvard.edu/abs/2017AJ....154..190H},
           adsnote = {Provided by the SAO/NASA Astrophysics Data System}
     }
 
 License
 -------
 
-Halotools is licensed under a 3-clause BSD style license - see the licenses/LICENSE.rst file.
+Halotools is licensed by Argonne National Lab under a 3-clause BSD style license - see the licenses/LICENSE.rst file.
+
```

### Comparing `halotools-0.8.1/halotools.egg-info/SOURCES.txt` & `halotools-0.8.2/halotools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,19 @@
 docs/_static/cam_example_complex_sfr_dmdt_correlation.png
 docs/_static/cam_example_complex_sfr_recovery.png
 docs/_static/color_correlation_pdf.png
 docs/_static/dm-splatting-large.png
 docs/_static/fuzzy_binning_example.png
 docs/_static/halotools.css
 docs/_static/matched_distributions.png
+docs/_static/mbk10_nsat_up0_behavior.png
 docs/_static/monte_carlo_example.png
 docs/_static/monte_carlo_example2.png
 docs/_static/noisy_percentile_demo.png
+docs/_static/non_poisson_mc_realization.png
 docs/_static/quenching_gradient_model_clustering.png
 docs/_static/quenching_gradient_models.png
 docs/_static/spin_percentile.png
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
 docs/full_ref_api/halotools_full_api.rst
@@ -277,24 +279,26 @@
 halotools/empirical_models/factories/tests/test_mock_helpers.py
 halotools/empirical_models/factories/tests/test_prebuilt_hod_model_factory.py
 halotools/empirical_models/factories/tests/test_prebuilt_subhalo_model_factory.py
 halotools/empirical_models/factories/tests/test_subhalo_model_factory.py
 halotools/empirical_models/occupation_models/__init__.py
 halotools/empirical_models/occupation_models/cacciato09_components.py
 halotools/empirical_models/occupation_models/leauthaud11_components.py
+halotools/empirical_models/occupation_models/negative_binomial_sats.py
 halotools/empirical_models/occupation_models/occupation_model_template.py
 halotools/empirical_models/occupation_models/tinker13_components.py
 halotools/empirical_models/occupation_models/zheng07_components.py
 halotools/empirical_models/occupation_models/zu_mandelbaum15_components.py
 halotools/empirical_models/occupation_models/engines/__init__.py
 halotools/empirical_models/occupation_models/engines/cacciato09_sats_mc_prim_galprop_engine.pyx
 halotools/empirical_models/occupation_models/engines/setup_package.py
 halotools/empirical_models/occupation_models/tests/__init__.py
 halotools/empirical_models/occupation_models/tests/test_cacciato09_clf.py
 halotools/empirical_models/occupation_models/tests/test_leauthaud11_hod.py
+halotools/empirical_models/occupation_models/tests/test_negative_binomial_sats.py
 halotools/empirical_models/occupation_models/tests/test_occupation_component.py
 halotools/empirical_models/occupation_models/tests/test_tinker13.py
 halotools/empirical_models/occupation_models/tests/test_zheng07_centrals.py
 halotools/empirical_models/occupation_models/tests/test_zheng07_satellites.py
 halotools/empirical_models/occupation_models/tests/test_zu_mandelbaum15_components.py
 halotools/empirical_models/phase_space_models/__init__.py
 halotools/empirical_models/phase_space_models/analytic_models/__init__.py
```

### Comparing `halotools-0.8.1/licenses/LICENSE.rst` & `halotools-0.8.2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/scripts/convert_documentation_tutorials.py` & `halotools-0.8.2/scripts/convert_documentation_tutorials.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/scripts/download_additional_halocat.py` & `halotools-0.8.2/scripts/download_additional_halocat.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/scripts/download_initial_halocat.py` & `halotools-0.8.2/scripts/download_initial_halocat.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/scripts/rebuild_halo_table_cache_log.py` & `halotools-0.8.2/scripts/rebuild_halo_table_cache_log.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/scripts/rebuild_ptcl_table_cache_log.py` & `halotools-0.8.2/scripts/rebuild_ptcl_table_cache_log.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/setup.cfg` & `halotools-0.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/setup.py` & `halotools-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `halotools-0.8.1/tox.ini` & `halotools-0.8.2/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -5,22 +5,22 @@
     linkcheck
     codestyle
 requires =
     setuptools >= 30.3.0
     pip >= 19.3.1
 isolated_build = true
 indexserver =
-    NIGHTLY = https://pypi.anaconda.org/scipy-wheels-nightly/simple
+    NIGHTLY = https://pypi.anaconda.org/scientific-python-nightly-wheels/simple
 
 [testenv]
 # Suppress display of matplotlib plots generated during docs build
 setenv = MPLBACKEND=agg
 
 # Pass through the following environment variables which may be needed for the CI
-passenv = HOME WINDIR LC_ALL LC_CTYPE CC CI TRAVIS
+passenv = HOME, WINDIR, LC_ALL, LC_CTYPE, CC, CI, TRAVIS
 
 # Run the tests in a temporary directory to make sure that we don't import
 # this package from the source tree
 changedir = .tmp/{envname}
 
 # tox environments are constructed with so-called 'factors' (or terms)
 # separated by hyphens, e.g. test-devdeps-cov. Lines below starting with factor:
```

