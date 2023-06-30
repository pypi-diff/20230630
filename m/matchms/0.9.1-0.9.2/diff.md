# Comparing `tmp/matchms-0.9.1.tar.gz` & `tmp/matchms-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/matchms-0.9.1.tar", last modified: Wed Jun 16 15:15:21 2021, max compression
+gzip compressed data, was "dist/matchms-0.9.2.tar", last modified: Tue Jul 20 18:04:03 2021, max compression
```

## Comparing `matchms-0.9.1.tar` & `matchms-0.9.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-16 15:15:21.000000 matchms-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11359 2021-06-16 15:15:11.000000 matchms-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-06-16 15:15:11.000000 matchms-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    17174 2021-06-16 15:15:21.000000 matchms-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13756 2021-06-16 15:15:11.000000 matchms-0.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms/
--rw-r--r--   0 runner    (1001) docker     (121)    10051 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/Scores.py
--rw-r--r--   0 runner    (1001) docker     (121)     6526 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/Spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/Spikes.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2485 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/calculate_scores.py
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms/data/
--rw-r--r--   0 runner    (1001) docker     (121)      729 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/data/known_adduct_conversions.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/data/known_adducts_table.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms/exporting/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/exporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/exporting/save_as_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/exporting/save_as_mgf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2211 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/exporting/save_as_msp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms/filtering/
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/SpeciesString.py
--rw-r--r--   0 runner    (1001) docker     (121)     3959 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/add_compound_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/add_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/add_losses.py
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/add_parent_mass.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/add_precursor_mz.py
--rw-r--r--   0 runner    (1001) docker     (121)     3117 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/clean_compound_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/correct_charge.py
--rw-r--r--   0 runner    (1001) docker     (121)     1781 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/default_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/derive_adduct_from_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/derive_formula_from_name.py
--rw-r--r--   0 runner    (1001) docker     (121)      753 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/derive_inchi_from_smiles.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/derive_inchikey_from_inchi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/derive_ionmode.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/derive_smiles_from_inchi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/harmonize_undefined_inchi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/harmonize_undefined_inchikey.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/harmonize_undefined_smiles.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/make_charge_int.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/make_charge_scalar.py
--rw-r--r--   0 runner    (1001) docker     (121)      449 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/make_ionmode_lowercase.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/normalize_intensities.py
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/reduce_to_number_of_peaks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/remove_peaks_around_precursor_mz.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/remove_peaks_outside_top_k.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/repair_inchi_inchikey_smiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/require_minimum_number_of_peaks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/require_minimum_of_high_peaks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/require_precursor_below_mz.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/require_precursor_mz.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/select_by_intensity.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/select_by_mz.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/select_by_relative_intensity.py
--rw-r--r--   0 runner    (1001) docker     (121)      449 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/filtering/set_ionmode_na_when_missing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms/importing/
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/importing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3294 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/importing/load_adducts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3299 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/importing/load_from_json.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/importing/load_from_mgf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4157 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/importing/load_from_msp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/importing/load_from_mzml.py
--rw-r--r--   0 runner    (1001) docker     (121)     1731 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/importing/load_from_mzxml.py
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/importing/load_from_usi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3106 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/importing/parsing_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms/networking/
--rw-r--r--   0 runner    (1001) docker     (121)     7404 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/networking/SimilarityNetwork.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/networking/networking_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms/similarity/
--rw-r--r--   0 runner    (1001) docker     (121)     3082 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/similarity/BaseSimilarity.py
--rw-r--r--   0 runner    (1001) docker     (121)     4101 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/similarity/CosineGreedy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5340 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/similarity/CosineHungarian.py
--rw-r--r--   0 runner    (1001) docker     (121)     6939 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/similarity/FingerprintSimilarity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/similarity/IntersectMz.py
--rw-r--r--   0 runner    (1001) docker     (121)     5285 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/similarity/ModifiedCosine.py
--rw-r--r--   0 runner    (1001) docker     (121)     5261 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/similarity/ParentMassMatch.py
--rw-r--r--   0 runner    (1001) docker     (121)     7322 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/similarity/PrecursorMzMatch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4060 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/similarity/spectrum_similarity_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/similarity/vector_similarity_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     9081 2021-06-16 15:15:11.000000 matchms-0.9.1/matchms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17174 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-06-16 15:15:21.000000 matchms-0.9.1/matchms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      686 2021-06-16 15:15:21.000000 matchms-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2021-06-16 15:15:11.000000 matchms-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 18:04:03.000000 matchms-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)    11359 2021-07-20 18:03:55.000000 matchms-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2021-07-20 18:03:55.000000 matchms-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    17288 2021-07-20 18:04:03.000000 matchms-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13812 2021-07-20 18:03:55.000000 matchms-0.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 18:04:03.000000 matchms-0.9.2/matchms/
+-rw-r--r--   0 runner    (1001) docker     (121)    10051 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/Scores.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6526 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/Spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1864 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/Spikes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2485 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/calculate_scores.py
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 18:04:03.000000 matchms-0.9.2/matchms/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/data/known_adduct_conversions.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2087 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/data/known_adducts_table.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 18:04:03.000000 matchms-0.9.2/matchms/exporting/
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/exporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/exporting/save_as_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1520 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/exporting/save_as_mgf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2211 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/exporting/save_as_msp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 18:04:03.000000 matchms-0.9.2/matchms/filtering/
+-rw-r--r--   0 runner    (1001) docker     (121)     2644 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/SpeciesString.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3959 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/add_compound_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/add_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1299 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/add_losses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2553 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/add_parent_mass.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1645 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/add_precursor_mz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3117 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/clean_compound_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/correct_charge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1781 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/default_filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1854 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/derive_adduct_from_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2218 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/derive_formula_from_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      753 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/derive_inchi_from_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/derive_inchikey_from_inchi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/derive_ionmode.py
+-rw-r--r--   0 runner    (1001) docker     (121)      757 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/derive_smiles_from_inchi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/harmonize_undefined_inchi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/harmonize_undefined_inchikey.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/harmonize_undefined_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/make_charge_int.py
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/make_charge_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/make_ionmode_lowercase.py
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/normalize_intensities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2032 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/reduce_to_number_of_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1294 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/remove_peaks_around_precursor_mz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1369 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/remove_peaks_outside_top_k.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1285 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/repair_inchi_inchikey_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/require_minimum_number_of_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1253 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/require_minimum_of_high_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/require_precursor_below_mz.py
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/require_precursor_mz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/select_by_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/select_by_mz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1419 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/select_by_relative_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/filtering/set_ionmode_na_when_missing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 18:04:03.000000 matchms-0.9.2/matchms/importing/
+-rw-r--r--   0 runner    (1001) docker     (121)     1338 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/importing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3294 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/importing/load_adducts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3299 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/importing/load_from_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/importing/load_from_mgf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4157 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/importing/load_from_msp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1630 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/importing/load_from_mzml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1731 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/importing/load_from_mzxml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/importing/load_from_usi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3106 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/importing/parsing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 18:04:03.000000 matchms-0.9.2/matchms/networking/
+-rw-r--r--   0 runner    (1001) docker     (121)     7404 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/networking/SimilarityNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2359 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/networking/networking_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 18:04:03.000000 matchms-0.9.2/matchms/similarity/
+-rw-r--r--   0 runner    (1001) docker     (121)     3082 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/similarity/BaseSimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4101 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/similarity/CosineGreedy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5340 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/similarity/CosineHungarian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6939 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/similarity/FingerprintSimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1822 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/similarity/IntersectMz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5285 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/similarity/ModifiedCosine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5255 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/similarity/ParentMassMatch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7316 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/similarity/PrecursorMzMatch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1312 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4060 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/similarity/spectrum_similarity_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5289 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/similarity/vector_similarity_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9081 2021-07-20 18:03:55.000000 matchms-0.9.2/matchms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 18:04:03.000000 matchms-0.9.2/matchms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    17288 2021-07-20 18:04:02.000000 matchms-0.9.2/matchms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2992 2021-07-20 18:04:03.000000 matchms-0.9.2/matchms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-20 18:04:02.000000 matchms-0.9.2/matchms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-20 18:04:02.000000 matchms-0.9.2/matchms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2021-07-20 18:04:02.000000 matchms-0.9.2/matchms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-07-20 18:04:02.000000 matchms-0.9.2/matchms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2021-07-20 18:04:03.000000 matchms-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2257 2021-07-20 18:03:55.000000 matchms-0.9.2/setup.py
```

### Comparing `matchms-0.9.1/LICENSE` & `matchms-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/PKG-INFO` & `matchms-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchms
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python library for fuzzy comparison of mass spectrum data and other Python objects
 Home-page: https://github.com/matchms/matchms
 Author: Netherlands eScience Center
 Author-email: generalization@esciencecenter.nl
 License: Apache Software License 2.0
 Description: .. image:: readthedocs/_static/matchms_header.png
            :target: readthedocs/_static/matchms.png
@@ -104,15 +104,15 @@
         For more extensive documentation `see our readthedocs <https://matchms.readthedocs.io/en/latest/>`_ and our `matchms introduction tutorial <https://blog.esciencecenter.nl/build-your-own-mass-spectrometry-analysis-pipeline-in-python-using-matchms-part-i-d96c718c68ee>`_.
         
         Installation
         ============
         
         Prerequisites:  
         
-        - Python 3.7 or 3.8 
+        - Python 3.7, 3.8 or 3.9
         - Anaconda (recommended)
         
         We recommend installing matchms from Anaconda Cloud with
         
         .. code-block:: console
         
           # install matchms in a new virtual environment to avoid dependency clashes
@@ -233,18 +233,19 @@
         
         To install matchms, do:
         
         .. code-block:: console
         
           git clone https://github.com/matchms/matchms.git
           cd matchms
-          conda env create matchms-dev
+          conda create --name matchms-dev python=3.8
           conda activate matchms-dev
           # Install rdkit using conda, rest of dependencies can be installed with pip
           conda install -c conda-forge rdkit
+          python -m pip install --upgrade pip
           pip install --editable .[dev]
         
         Run the linter with:
         
         .. code-block:: console
         
           prospector
@@ -322,11 +323,12 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: chemistry
```

### Comparing `matchms-0.9.1/README.rst` & `matchms-0.9.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 For more extensive documentation `see our readthedocs <https://matchms.readthedocs.io/en/latest/>`_ and our `matchms introduction tutorial <https://blog.esciencecenter.nl/build-your-own-mass-spectrometry-analysis-pipeline-in-python-using-matchms-part-i-d96c718c68ee>`_.
 
 Installation
 ============
 
 Prerequisites:  
 
-- Python 3.7 or 3.8 
+- Python 3.7, 3.8 or 3.9
 - Anaconda (recommended)
 
 We recommend installing matchms from Anaconda Cloud with
 
 .. code-block:: console
 
   # install matchms in a new virtual environment to avoid dependency clashes
@@ -225,18 +225,19 @@
 
 To install matchms, do:
 
 .. code-block:: console
 
   git clone https://github.com/matchms/matchms.git
   cd matchms
-  conda env create matchms-dev
+  conda create --name matchms-dev python=3.8
   conda activate matchms-dev
   # Install rdkit using conda, rest of dependencies can be installed with pip
   conda install -c conda-forge rdkit
+  python -m pip install --upgrade pip
   pip install --editable .[dev]
 
 Run the linter with:
 
 .. code-block:: console
 
   prospector
```

### Comparing `matchms-0.9.1/matchms/Scores.py` & `matchms-0.9.2/matchms/Scores.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/Spectrum.py` & `matchms-0.9.2/matchms/Spectrum.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/Spikes.py` & `matchms-0.9.2/matchms/Spikes.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/__init__.py` & `matchms-0.9.2/matchms/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from . import exporting
 from . import filtering
 from . import importing
+from . import networking
 from . import similarity
 from .__version__ import __version__
 from .calculate_scores import calculate_scores
 from .Scores import Scores
 from .Spectrum import Spectrum
 from .Spikes import Spikes
 
@@ -16,12 +17,13 @@
 __email__ = 'generalization@esciencecenter.nl'
 __all__ = [
     "__version__",
     "calculate_scores",
     "exporting",
     "filtering",
     "importing",
+    "networking",
     "Scores",
     "similarity",
     "Spectrum",
     "Spikes"
 ]
```

### Comparing `matchms-0.9.1/matchms/calculate_scores.py` & `matchms-0.9.2/matchms/calculate_scores.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/data/known_adduct_conversions.csv` & `matchms-0.9.2/matchms/data/known_adduct_conversions.csv`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/data/known_adducts_table.csv` & `matchms-0.9.2/matchms/data/known_adducts_table.csv`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/exporting/save_as_json.py` & `matchms-0.9.2/matchms/exporting/save_as_json.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/exporting/save_as_mgf.py` & `matchms-0.9.2/matchms/exporting/save_as_mgf.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/exporting/save_as_msp.py` & `matchms-0.9.2/matchms/exporting/save_as_msp.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/SpeciesString.py` & `matchms-0.9.2/matchms/filtering/SpeciesString.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/__init__.py` & `matchms-0.9.2/matchms/filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/add_compound_name.py` & `matchms-0.9.2/matchms/filtering/add_compound_name.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/add_fingerprint.py` & `matchms-0.9.2/matchms/filtering/add_fingerprint.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/add_losses.py` & `matchms-0.9.2/matchms/filtering/add_losses.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/add_parent_mass.py` & `matchms-0.9.2/matchms/filtering/add_parent_mass.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/add_precursor_mz.py` & `matchms-0.9.2/matchms/filtering/add_precursor_mz.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/clean_compound_name.py` & `matchms-0.9.2/matchms/filtering/clean_compound_name.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/correct_charge.py` & `matchms-0.9.2/matchms/filtering/correct_charge.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/default_filters.py` & `matchms-0.9.2/matchms/filtering/default_filters.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/derive_adduct_from_name.py` & `matchms-0.9.2/matchms/filtering/derive_adduct_from_name.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/derive_formula_from_name.py` & `matchms-0.9.2/matchms/filtering/derive_formula_from_name.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/derive_inchi_from_smiles.py` & `matchms-0.9.2/matchms/filtering/derive_inchi_from_smiles.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/derive_inchikey_from_inchi.py` & `matchms-0.9.2/matchms/filtering/derive_inchikey_from_inchi.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/derive_ionmode.py` & `matchms-0.9.2/matchms/filtering/derive_ionmode.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/derive_smiles_from_inchi.py` & `matchms-0.9.2/matchms/filtering/derive_smiles_from_inchi.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/harmonize_undefined_inchi.py` & `matchms-0.9.2/matchms/filtering/harmonize_undefined_inchi.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/harmonize_undefined_inchikey.py` & `matchms-0.9.2/matchms/filtering/harmonize_undefined_inchikey.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/harmonize_undefined_smiles.py` & `matchms-0.9.2/matchms/filtering/harmonize_undefined_smiles.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/make_charge_int.py` & `matchms-0.9.2/matchms/filtering/make_charge_int.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/normalize_intensities.py` & `matchms-0.9.2/matchms/filtering/normalize_intensities.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/reduce_to_number_of_peaks.py` & `matchms-0.9.2/matchms/filtering/reduce_to_number_of_peaks.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/remove_peaks_around_precursor_mz.py` & `matchms-0.9.2/matchms/filtering/remove_peaks_around_precursor_mz.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/remove_peaks_outside_top_k.py` & `matchms-0.9.2/matchms/filtering/remove_peaks_outside_top_k.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/repair_inchi_inchikey_smiles.py` & `matchms-0.9.2/matchms/filtering/repair_inchi_inchikey_smiles.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/require_minimum_number_of_peaks.py` & `matchms-0.9.2/matchms/filtering/require_minimum_number_of_peaks.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/require_minimum_of_high_peaks.py` & `matchms-0.9.2/matchms/filtering/require_minimum_of_high_peaks.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/require_precursor_below_mz.py` & `matchms-0.9.2/matchms/filtering/require_precursor_below_mz.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/require_precursor_mz.py` & `matchms-0.9.2/matchms/filtering/require_precursor_mz.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/select_by_intensity.py` & `matchms-0.9.2/matchms/filtering/select_by_intensity.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/select_by_mz.py` & `matchms-0.9.2/matchms/filtering/select_by_mz.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/filtering/select_by_relative_intensity.py` & `matchms-0.9.2/matchms/filtering/select_by_relative_intensity.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/importing/__init__.py` & `matchms-0.9.2/matchms/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/importing/load_adducts.py` & `matchms-0.9.2/matchms/importing/load_adducts.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/importing/load_from_json.py` & `matchms-0.9.2/matchms/importing/load_from_json.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/importing/load_from_mgf.py` & `matchms-0.9.2/matchms/importing/load_from_mgf.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/importing/load_from_msp.py` & `matchms-0.9.2/matchms/importing/load_from_msp.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/importing/load_from_mzml.py` & `matchms-0.9.2/matchms/importing/load_from_mzml.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/importing/load_from_mzxml.py` & `matchms-0.9.2/matchms/importing/load_from_mzxml.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/importing/load_from_usi.py` & `matchms-0.9.2/matchms/importing/load_from_usi.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/importing/parsing_utils.py` & `matchms-0.9.2/matchms/importing/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/networking/SimilarityNetwork.py` & `matchms-0.9.2/matchms/networking/SimilarityNetwork.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/networking/networking_functions.py` & `matchms-0.9.2/matchms/networking/networking_functions.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/similarity/BaseSimilarity.py` & `matchms-0.9.2/matchms/similarity/BaseSimilarity.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/similarity/CosineGreedy.py` & `matchms-0.9.2/matchms/similarity/CosineGreedy.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/similarity/CosineHungarian.py` & `matchms-0.9.2/matchms/similarity/CosineHungarian.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/similarity/FingerprintSimilarity.py` & `matchms-0.9.2/matchms/similarity/FingerprintSimilarity.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/similarity/IntersectMz.py` & `matchms-0.9.2/matchms/similarity/IntersectMz.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/similarity/ModifiedCosine.py` & `matchms-0.9.2/matchms/similarity/ModifiedCosine.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/similarity/ParentMassMatch.py` & `matchms-0.9.2/matchms/similarity/ParentMassMatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         Parentmass match between 2 and 3 is 0.00
         Parentmass match between 2 and 4 is 1.00
 
     """
     # Set key characteristics as class attributes
     is_commutative = True
     # Set output data type, e.g.  "float" or [("score", "float"), ("matches", "int")]
-    score_datatype = numpy.bool
+    score_datatype = bool
 
     def __init__(self, tolerance: float = 0.1):
         """
         Parameters
         ----------
         tolerance
             Specify tolerance below which two masses are counted as match.
```

### Comparing `matchms-0.9.1/matchms/similarity/PrecursorMzMatch.py` & `matchms-0.9.2/matchms/similarity/PrecursorMzMatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         Precursor m/z match between 1 and 4 is 0.00
         Precursor m/z match between 2 and 3 is 0.00
         Precursor m/z match between 2 and 4 is 1.00
 
     """
     # Set key characteristics as class attributes
     is_commutative = True
-    score_datatype = numpy.bool
+    score_datatype = bool
 
     def __init__(self, tolerance: float = 0.1, tolerance_type: str = "Dalton"):
         """
         Parameters
         ----------
         tolerance
             Specify tolerance below which two m/z are counted as match.
```

### Comparing `matchms-0.9.1/matchms/similarity/__init__.py` & `matchms-0.9.2/matchms/similarity/__init__.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/similarity/spectrum_similarity_functions.py` & `matchms-0.9.2/matchms/similarity/spectrum_similarity_functions.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/similarity/vector_similarity_functions.py` & `matchms-0.9.2/matchms/similarity/vector_similarity_functions.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms/utils.py` & `matchms-0.9.2/matchms/utils.py`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/matchms.egg-info/PKG-INFO` & `matchms-0.9.2/matchms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchms
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python library for fuzzy comparison of mass spectrum data and other Python objects
 Home-page: https://github.com/matchms/matchms
 Author: Netherlands eScience Center
 Author-email: generalization@esciencecenter.nl
 License: Apache Software License 2.0
 Description: .. image:: readthedocs/_static/matchms_header.png
            :target: readthedocs/_static/matchms.png
@@ -104,15 +104,15 @@
         For more extensive documentation `see our readthedocs <https://matchms.readthedocs.io/en/latest/>`_ and our `matchms introduction tutorial <https://blog.esciencecenter.nl/build-your-own-mass-spectrometry-analysis-pipeline-in-python-using-matchms-part-i-d96c718c68ee>`_.
         
         Installation
         ============
         
         Prerequisites:  
         
-        - Python 3.7 or 3.8 
+        - Python 3.7, 3.8 or 3.9
         - Anaconda (recommended)
         
         We recommend installing matchms from Anaconda Cloud with
         
         .. code-block:: console
         
           # install matchms in a new virtual environment to avoid dependency clashes
@@ -233,18 +233,19 @@
         
         To install matchms, do:
         
         .. code-block:: console
         
           git clone https://github.com/matchms/matchms.git
           cd matchms
-          conda env create matchms-dev
+          conda create --name matchms-dev python=3.8
           conda activate matchms-dev
           # Install rdkit using conda, rest of dependencies can be installed with pip
           conda install -c conda-forge rdkit
+          python -m pip install --upgrade pip
           pip install --editable .[dev]
         
         Run the linter with:
         
         .. code-block:: console
         
           prospector
@@ -322,11 +323,12 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: chemistry
```

### Comparing `matchms-0.9.1/matchms.egg-info/SOURCES.txt` & `matchms-0.9.2/matchms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matchms-0.9.1/setup.cfg` & `matchms-0.9.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.1
+current_version = 0.9.2
 
 [bumpversion:file:matchms/__version__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
 
 [metadata]
 description-file = README.rst
```

### Comparing `matchms-0.9.1/setup.py` & `matchms-0.9.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,16 @@
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8"
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9"
     ],
     test_suite="tests",
     python_requires='>=3.7',
     install_requires=[
         "deprecated",
         "lxml",
         "matplotlib",
```

