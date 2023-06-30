# Comparing `tmp/genomehubs-2.7.5.tar.gz` & `tmp/genomehubs-2.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomehubs-2.7.5.tar", last modified: Tue May 30 11:03:54 2023, max compression
+gzip compressed data, was "genomehubs-2.7.6.tar", last modified: Fri Jun 30 15:58:29 2023, max compression
```

## Comparing `genomehubs-2.7.5.tar` & `genomehubs-2.7.6.tar`

### file list

```diff
@@ -1,113 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.559165 genomehubs-2.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-30 11:03:14.000000 genomehubs-2.7.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-30 11:03:14.000000 genomehubs-2.7.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-30 11:03:14.000000 genomehubs-2.7.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-30 11:03:14.000000 genomehubs-2.7.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 11:03:14.000000 genomehubs-2.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-30 11:03:14.000000 genomehubs-2.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-30 11:03:54.559165 genomehubs-2.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-30 11:03:14.000000 genomehubs-2.7.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-30 11:03:14.000000 genomehubs-2.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-30 11:03:54.559165 genomehubs-2.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-30 11:03:14.000000 genomehubs-2.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.543163 genomehubs-2.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.547164 genomehubs-2.7.5/src/genomehubs/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.547164 genomehubs-2.7.5/src/genomehubs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/config/dist.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/genomehubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.551164 genomehubs-2.7.5/src/genomehubs/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/btk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/busco.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/es_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    34258 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/gbif.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    35765 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    37857 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/taxon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/wikidata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.555164 genomehubs-2.7.5/src/genomehubs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/ATTR_busco.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/ATTR_feature.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/ATTR_window_stats.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/assembly.json
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/assembly.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/btk.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/busco.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/busco_feature.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/feature.json
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/file.json
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/identifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/organelle.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/sample.types.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.559165 genomehubs-2.7.5/src/genomehubs/templates/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/analysis_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/analysis_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/assembly_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/assembly_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/attribute_types_by_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/attribute_values_by_taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/attributes_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/attributes_identifiers_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/attributes_names_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/file_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/file_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/max_nested_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/max_nested_value_by_key_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/max_nested_value_by_type.json
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/search_by_taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_attributes_by_taxon_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_any_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_name.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_specific_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_names.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_names_by_root.json
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxonomy_node_by_taxon_id.json
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/value_by_type_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/taxon.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/taxonomy.json
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/wikidata.names.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/window_full.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/window_stats.types.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.547164 genomehubs-2.7.5/src/genomehubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-30 11:03:54.000000 genomehubs-2.7.5/src/genomehubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-30 11:03:54.000000 genomehubs-2.7.5/src/genomehubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:03:54.000000 genomehubs-2.7.5/src/genomehubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-30 11:03:54.000000 genomehubs-2.7.5/src/genomehubs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-30 11:03:54.000000 genomehubs-2.7.5/src/genomehubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 11:03:54.000000 genomehubs-2.7.5/src/genomehubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.432419 genomehubs-2.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 15:57:45.000000 genomehubs-2.7.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 15:57:45.000000 genomehubs-2.7.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-30 15:57:45.000000 genomehubs-2.7.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-30 15:57:45.000000 genomehubs-2.7.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-30 15:57:45.000000 genomehubs-2.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-30 15:57:45.000000 genomehubs-2.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-30 15:58:29.432419 genomehubs-2.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-30 15:57:45.000000 genomehubs-2.7.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-30 15:57:45.000000 genomehubs-2.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-30 15:58:29.432419 genomehubs-2.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-30 15:57:45.000000 genomehubs-2.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.416419 genomehubs-2.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.420419 genomehubs-2.7.6/src/genomehubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.420419 genomehubs-2.7.6/src/genomehubs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/config/dist.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/genomehubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.424419 genomehubs-2.7.6/src/genomehubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/btk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/busco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/es_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34397 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/gbif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35765 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37857 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/taxon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/wikidata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.428419 genomehubs-2.7.6/src/genomehubs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/ATTR_assembly.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/ATTR_btk.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/ATTR_busco.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/ATTR_feature.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/ATTR_sample.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/ATTR_window_stats.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/TAXON_assembly.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/analysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/assembly.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/assembly.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/attributes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/btk.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/busco.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/busco_feature.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/identifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/organelle.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/sample.types.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.432419 genomehubs-2.7.6/src/genomehubs/templates/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/analysis_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/analysis_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/assembly_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/assembly_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/attribute_types_by_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/attribute_values_by_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/attributes_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/attributes_identifiers_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/attributes_names_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/file_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/file_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/max_nested_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/max_nested_value_by_key_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/max_nested_value_by_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/search_by_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_attributes_by_taxon_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_any_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_specific_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_names_by_root.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxonomy_node_by_taxon_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/value_by_type_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/taxon.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/taxonomy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/wikidata.names.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/window_full.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/window_stats.types.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.420419 genomehubs-2.7.6/src/genomehubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-30 15:58:29.000000 genomehubs-2.7.6/src/genomehubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-30 15:58:29.000000 genomehubs-2.7.6/src/genomehubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:58:29.000000 genomehubs-2.7.6/src/genomehubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-30 15:58:29.000000 genomehubs-2.7.6/src/genomehubs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-30 15:58:29.000000 genomehubs-2.7.6/src/genomehubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 15:58:29.000000 genomehubs-2.7.6/src/genomehubs.egg-info/top_level.txt
```

### Comparing `genomehubs-2.7.5/CONTRIBUTING.rst` & `genomehubs-2.7.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/LICENSE` & `genomehubs-2.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/PKG-INFO` & `genomehubs-2.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomehubs
-Version: 2.7.5
+Version: 2.7.6
 Summary: GenomeHubs
 Home-page: https://github.com/genomehubs/genomehubs
 Author: genomehubs
 Author-email: genomehubs@genomehubs.org
 Project-URL: Bug Reports, https://github.com/genomehubs/genomehubs/issues
 Project-URL: Source, https://github.com/genomehubs/genomehubs
 Keywords: bioinformatics
```

### Comparing `genomehubs-2.7.5/README.rst` & `genomehubs-2.7.6/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     :alt: Install with Conda
     :target: https://anaconda.org/tolkit/genomehubs
 
 .. |platforms| image:: https://anaconda.org/tolkit/genomehubs/badges/platforms.svg
     :alt: Conda platforms
     :target: https://anaconda.org/tolkit/genomehubs
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/genomehubs/genomehubs/2.7.5.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/genomehubs/genomehubs/2.7.6.svg
     :alt: Commits since latest release
-    :target: https://github.com/genomehubs/genomehubs/compare/2.7.5...main
+    :target: https://github.com/genomehubs/genomehubs/compare/2.7.6...main
 
 .. |license| image:: https://anaconda.org/tolkit/genomehubs/badges/license.svg
     :alt: MIT License
     :target: https://anaconda.org/tolkit/genomehubs
 
 .. end-badges
```

### Comparing `genomehubs-2.7.5/setup.cfg` & `genomehubs-2.7.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/setup.py` & `genomehubs-2.7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="genomehubs",  # Required
-    version="2.7.5",
+    version="2.7.6",
     description="GenomeHubs",  # Optional
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
```

### Comparing `genomehubs-2.7.5/src/genomehubs/config/dist.config.yaml` & `genomehubs-2.7.6/src/genomehubs/config/dist.config.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/genomehubs.py` & `genomehubs-2.7.6/src/genomehubs/genomehubs.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/attributes.py` & `genomehubs-2.7.6/src/genomehubs/lib/attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 
 def stream_attributes(group, attributes, *, index_type="attribute"):
     """Stream attributes for indexing."""
     for name, obj in attributes.items():
         ret = {"group": group, "name": name}
         for prop, value in obj.items():
-            if not prop.startswith("taxon_"):
-                ret.update({prop: value})
+            # if not prop.startswith("taxon_"):
+            ret.update({prop: value})
         yield "%s-%s-%s" % (index_type, group, name), ret
 
 
 def index(es, group, attributes, opts, *, index_type="attribute"):
     """Index a set of attributes or names."""
     LOGGER.info("Indexing %s" % index_type)
     template = index_template(opts, index_type=index_type)
@@ -77,29 +77,39 @@
                     obj[key].append(value)
             else:
                 obj[key] = value
 
 
 def index_types(es, types_name, types, opts, *, dry_run=False):
     """Index types into Elasticsearch."""
-    # TODO: fetch existing types to allow new sources to add, not overwrite
     try:
         attributes = fetch_types(es, types_name, opts)
     except Exception:
         attributes = {}
     if "attributes" in types:
         new_attributes = {}
         for key, value in types["attributes"].items():
             if "defaults" in types and "attributes" in types["defaults"]:
                 value = {**types["defaults"]["attributes"], **value}
             if key in attributes:
-                types["attributes"][key] = {
-                    **attributes[key],
-                    **value,
-                }
+                if (
+                    "header" not in types["attributes"][key]
+                    and "index" not in types["attributes"][key]
+                ):
+                    types["attributes"][key] = {
+                        **types["attributes"][key],
+                        **attributes[key],
+                        **value,
+                    }
+                    new_attributes[key] = types["attributes"][key]
+                else:
+                    types["attributes"][key] = {
+                        **attributes[key],
+                        **value,
+                    }
             else:
                 new_attributes[key] = {**value}
                 new_attributes[key].pop("header", None)
                 new_attributes[key].pop("index", None)
         if new_attributes:
             template, stream = index(
                 es, types_name, new_attributes, opts, index_type="attribute"
```

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/btk.py` & `genomehubs-2.7.6/src/genomehubs/lib/btk.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/busco.py` & `genomehubs-2.7.6/src/genomehubs/lib/busco.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/config.py` & `genomehubs-2.7.6/src/genomehubs/lib/config.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/directory.py` & `genomehubs-2.7.6/src/genomehubs/lib/directory.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/es_functions.py` & `genomehubs-2.7.6/src/genomehubs/lib/es_functions.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/files.py` & `genomehubs-2.7.6/src/genomehubs/lib/files.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/fill.py` & `genomehubs-2.7.6/src/genomehubs/lib/fill.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,19 @@
         value_type = f'{meta["type"]}_value'
         primary_values = []
         if "values" in attribute:
             # iterate_values(attribute, meta)
             if values is None:
                 values = []
                 for value in attribute["values"]:
-                    values.append(value[value_type])
+                    try:
+                        values.append(value[value_type])
+                    except KeyError:
+                        print(meta)
+                        print(value)
                     if "is_primary_value" in value and value["is_primary_value"]:
                         primary_values.append(value[value_type])
             else:
                 # TODO: handle existing value here
                 values += [value[value_type] for value in attribute["values"]]
         if not values:
             return None, None, None
```

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/gbif.py` & `genomehubs-2.7.6/src/genomehubs/lib/gbif.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/geo.py` & `genomehubs-2.7.6/src/genomehubs/lib/geo.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/hub.py` & `genomehubs-2.7.6/src/genomehubs/lib/hub.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/index.py` & `genomehubs-2.7.6/src/genomehubs/lib/index.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/init.py` & `genomehubs-2.7.6/src/genomehubs/lib/init.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/ncbi.py` & `genomehubs-2.7.6/src/genomehubs/lib/ncbi.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,69 +215,70 @@
     """Parse a single NCBI datasets record."""
     obj = {
         key: record.get(key, "None")
         for key in ("taxId", "organismName", "commonName", "isolate", "sex")
     }
 
     assemblyInfo = record.get("assemblyInfo", {})
+    annotationInfo = record.get("annotationInfo", {})
     if assemblyInfo.get("atypical", False):
         return
     for key in (
         "assemblyLevel",
         "assemblyName",
         "assemblyType",
         "biosampleAccession",
         "genbankAssmAccession",
         "refseqAssmAccession",
         "refseqCategory",
         "submissionDate",
         "submitter",
     ):
-        obj[key] = assemblyInfo.get(key, None)
-        if key == "refseqCategory":
-            obj["primaryValue"] = 1 if obj[key] == "representative genome" else None
+        obj[key] = assemblyInfo.get(key, annotationInfo.get(key, "None"))
     if obj["refseqAssmAccession"] == "na":
-        obj["refseqAssmAccession"] = None
-        obj["refseqCategory"] = None
-        obj["primaryValue"] = None
-    if annotationInfo := record.get("annotationInfo", {}):
+        obj["refseqAssmAccession"] = "None"
+    elif obj["refseqCategory"] != "None":
+        obj["primaryValue"] = 1
+    if annotationInfo:
         annot = {
-            f"annotation{key.capitalize()}": annotationInfo.get(key, None)
+            f"annotation{key.capitalize()}": annotationInfo.get(key, "None")
             for key in ("name", "releaseDate", "reportUrl", "source")
         }
 
         if annot and "stats" in annotationInfo:
-            geneCounts = annotationInfo["stats"].get("geneCounts", None)
+            geneCounts = annotationInfo["stats"].get("geneCounts", "None")
             for key in ("nonCoding", "proteinCoding", "pseudogene", "total"):
-                annot[f"geneCount{key.capitalize()}"] = geneCounts.get(key, None)
-            if obj["genbankAssmAccession"] in parsed:
-                parsed[obj["genbankAssmAccession"]].update(annot)
-                return
+                annot[f"geneCount{key.capitalize()}"] = geneCounts.get(key, "None")
             obj.update(annot)
     bioprojects = []
     for lineage in assemblyInfo.get("bioprojectLineage", []):
         if "bioprojects" in lineage:
             bioprojects.extend(
                 bioproject["accession"] for bioproject in lineage["bioprojects"]
             )
 
     if not bioprojects and "bioprojects" in assemblyInfo.get("biosample", {}):
         bioprojects.extend(
             bioproject["accession"]
             for bioproject in assemblyInfo["biosample"]["bioprojects"]
         )
 
-    obj["bioProjectAccession"] = ";".join(bioprojects) if bioprojects else None
+    obj["bioProjectAccession"] = ";".join(bioprojects) if bioprojects else "None"
     assemblyStats = record.get("assemblyStats", {})
     obj.update(assemblyStats)
     metricDates(obj)
     wgsInfo = record.get("wgsInfo", {})
     for key in ("masterWgsUrl", "wgsContigsUrl", "wgsProjectAccession"):
-        obj[key] = wgsInfo.get(key, None)
-    parsed[obj["genbankAssmAccession"]] = obj
+        obj[key] = wgsInfo.get(key, "None")
+    if obj["genbankAssmAccession"] in parsed:
+        for key, value in obj.items():
+            if value != "None":
+                parsed[obj["genbankAssmAccession"]][key] = value
+    else:
+        parsed[obj["genbankAssmAccession"]] = obj
 
 
 def parse_ncbi_datasets_sample(record, parsed):
     """Parse sample information from a single NCBI datasets record."""
     obj = {key: record.get(key, "None") for key in ("taxId", "isolate", "sex")}
     assemblyInfo = record.get("assemblyInfo", {})
     if assemblyInfo.get("atypical", False):
@@ -286,19 +287,19 @@
         "assemblyLevel",
         "biosampleAccession",
         "genbankAssmAccession",
         "refseqAssmAccession",
         "refseqCategory",
         "submitter",
     ):
-        obj[key] = assemblyInfo.get(key, None)
+        obj[key] = assemblyInfo.get(key, "None")
         if key == "refseqCategory":
-            obj["primaryValue"] = 1 if obj[key] == "representative genome" else None
+            obj["primaryValue"] = 1 if obj[key] == "representative genome" else "None"
     attributes = {
-        entry["name"]: entry.get("value", None)
+        entry["name"]: entry.get("value", "None")
         for entry in assemblyInfo.get("biosample", {}).get("attributes", [])
     }
     for key in ("estimated_size", "geo_loc_name", "num_replicons", "ploidy"):
         obj[key] = attributes.get(key)
     obj["latitude"] = degrees_to_decimal(
         attributes.get("geographic location (latitude)")
     )
@@ -315,15 +316,15 @@
 
     if not bioprojects and "bioprojects" in assemblyInfo.get("biosample", {}):
         bioprojects.extend(
             bioproject["accession"]
             for bioproject in assemblyInfo["biosample"]["bioprojects"]
         )
 
-    obj["bioProjectAccession"] = ";".join(bioprojects) if bioprojects else None
+    obj["bioProjectAccession"] = ";".join(bioprojects) if bioprojects else "None"
     parsed[obj["biosampleAccession"]] = obj
 
 
 def ncbi_genome_parser(params, opts, *, types=None, names=None):
     """Parse NCBI Datasets genome report."""
     parsed = {}
     jsonl = opts[f"ncbi-datasets-{params}"]
```

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/parse.py` & `genomehubs-2.7.6/src/genomehubs/lib/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
             if parsed is not None:
                 if isinstance(parsed, tuple):
                     parsed, files = parsed
                 data = order_parsed_fields(parsed, types, names)
                 tofile.write_file(options["parse"]["outfile"], data)
             needs = types.get("file", {}).get("needs", [])
             for needs_file in needs:
-                if needs_file.startswith("ATTR_"):
+                if needs_file.startswith("ATTR_") or needs_file.startswith("TAXON_"):
                     copy_types(needs_file, outdir)
             suff = re.compile(r"\.[^\.]+$")
             if filepath.name.endswith(".gz"):
                 stem = re.sub(suff, "", filepath.stem)
             else:
                 stem = filepath.stem
             suffix = filepath.name.replace(stem, "")
```

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/run.py` & `genomehubs-2.7.6/src/genomehubs/lib/run.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/sample.py` & `genomehubs-2.7.6/src/genomehubs/lib/sample.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/search.py` & `genomehubs-2.7.6/src/genomehubs/lib/search.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/taxon.py` & `genomehubs-2.7.6/src/genomehubs/lib/taxon.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/taxonomy.py` & `genomehubs-2.7.6/src/genomehubs/lib/taxonomy.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/test.py` & `genomehubs-2.7.6/src/genomehubs/lib/test.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/validate.py` & `genomehubs-2.7.6/src/genomehubs/lib/validate.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             attributes = {}
         try:
             stored_attributes = fetch_types(es, types_name, opts)
             attributes = {**stored_attributes, **attributes}
         except Exception:
             pass
         if attributes:
-            sequence = max(int(d['sequence']) for d in attributes.values()) + 1
+            sequence = max(int(d["sequence"]) for d in attributes.values()) + 1
         else:
             sequence = 0
         for key, entry in types["attributes"].items():
             if not isinstance(entry, dict):
                 entry = {"default": entry}
             if key in attributes:
                 entry = {**attributes[key], **entry}
@@ -45,24 +45,24 @@
                 sequence += 1
             types["attributes"][key] = entry
             enum = entry.get("constraint", {}).get("enum", [])
             if enum:
                 entry["constraint"]["enum"] = [value.lower() for value in enum]
             translate = entry.get("translate", {})
             if translate:
-                entry["translate"] = {key.lower(): value for key, value in translate.items()}
+                entry["translate"] = {
+                    key.lower(): value for key, value in translate.items()
+                }
     names = None
     exclusions = None
     data = None
     if "file" in types:
         if "name" in types["file"]:
-            if (
-                "taxonomy" not in types
-                and "features" not in types
-                and "taxon_id" not in types["features"]
+            if "taxonomy" not in types and (
+                "features" not in types or "taxon_id" not in types["features"]
             ):
                 LOGGER.error("Types file contains no taxonomy information")
                 sys.exit(1)
             datafile = Path(dir_path) / types["file"]["name"]
             data = tofile.open_file_handle(datafile)
             if data is None:
                 LOGGER.error("Data file '%s' could not de opened for reading", datafile)
@@ -80,10 +80,12 @@
         types.update({"defaults": defaults})
         if "name" in types["file"]:
             names = process_names_file(
                 types, Path(dir_path) / "names" / types["file"]["name"]
             )
             if "exclusions" in types["file"]:
                 exclusions = process_names_file(
-                    types, Path(dir_path) / "exclusions" / types["file"]["name"], value_path=types["file"]["exclusions"]
+                    types,
+                    Path(dir_path) / "exclusions" / types["file"]["name"],
+                    value_path=types["file"]["exclusions"],
                 )
     return types, data, names, exclusions
```

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/wikidata.py` & `genomehubs-2.7.6/src/genomehubs/lib/wikidata.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/lib/window.py` & `genomehubs-2.7.6/src/genomehubs/lib/window.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/ATTR_busco.types.yaml` & `genomehubs-2.7.6/src/genomehubs/templates/ATTR_busco.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/ATTR_feature.types.yaml` & `genomehubs-2.7.6/src/genomehubs/templates/ATTR_feature.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/ATTR_window_stats.types.yaml` & `genomehubs-2.7.6/src/genomehubs/templates/ATTR_window_stats.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/analysis.json` & `genomehubs-2.7.6/src/genomehubs/templates/analysis.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/assembly.json` & `genomehubs-2.7.6/src/genomehubs/templates/assembly.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/assembly.types.yaml` & `genomehubs-2.7.6/src/genomehubs/templates/ATTR_assembly.types.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,34 @@
-file:
-  display_group: general
-  exclusions:
-    identifiers:
-      - assembly_id
-    taxonomy:
-      - taxon_id
-    attributes:
-      - bioproject
-      - biosample
-  format: tsv
-  header: true
-  organelle: nucleus
-  source_url_stub: https://www.ncbi.nlm.nih.gov/assembly/
-  source: INSDC
-taxonomy:
-  taxon_id:
-    header: taxId
-  taxon:
-    header: organismName
-names:
-  common_name:
-    header: commonName
+defaults:
+  attributes:
+    display_group: general
+    organelle: nucleus
+    source_url_stub: https://www.ncbi.nlm.nih.gov/assembly/
+    source: INSDC
+    taxon_display_group: assembly
 identifiers:
   assembly_id:
     constraint:
       len: 32
-    header: genbankAssmAccession
     type: keyword
   genbank_accession:
     constraint:
       len: 32
-    header: genbankAssmAccession
     type: keyword
   refseq_accession:
     constraint:
       len: 32
-    header: refseqAssmAccession
     type: keyword
   wgs_accession:
     constraint:
       len: 16
-    header: wgsProjectAccession
     type: keyword
   assembly_name:
     constraint:
       len: 64
-    header: assemblyName
     type: keyword
 attributes:
   organelle:
     constraint:
       enum:
         - nucleus
         - mitochondrion
@@ -58,25 +37,16 @@
         - apicoplast
     default: nucleus
     type: keyword
   bioproject:
     constraint:
       len: 32
     description: INSDC bioproject ID or assembly collection name
-    header: bioProjectAccession
-    separator:
-      - ;
     synonyms:
       - bioproject_accession
-    taxon_display_group: assembly
-    taxon_summary:
-      - list
-    taxon_traverse: list
-    taxon_traverse_direction: up
-    taxon_display_level: 2
     type: keyword
     value_metadata:
       default:
         description: Click to view BioProject record on ENA
         link: https://www.ebi.ac.uk/ena/browser/view/{}
       prjna533106:
         description: "Earth Biogenome Project (click to view on ENA)"
@@ -123,273 +93,196 @@
       prjna707598:
         description: "Squalomix (click to view on ENA)"
       prjna489243:
         description: "Vertebrate Genomes Project (click to view on ENA)"
   biosample:
     constraint:
       len: 32
-    header: biosampleAccession
-    separator:
-      - ";"
     synonyms:
       - biosample_accession
-    taxon_display_group: assembly
-    taxon_summary:
-      - list
-    taxon_traverse: list
-    taxon_traverse_direction: up
-    taxon_display_level: 2
     type: keyword
     value_metadata:
       default:
         description: Click to view BioSample record on ENA
         link: https://www.ebi.ac.uk/ena/browser/view/{}
   gene_count:
     display_group: annotation
     display_level: 1
     display_name: Gene count
     constraint:
       min: 1
-    header: geneCountTotal
     type: integer
-    taxon_display_group: assembly
-    taxon_summary:
-      - primary
-      - median
-      - min
-      - max
-      - count
-    taxon_display_level: 2
     bins:
       min: 0
       max: 5
       count: 10
       scale: log10
   protein_count:
     display_group: annotation
     display_level: 2
     display_name: Protein count
     constraint:
       min: 1
-    header: geneCountProteincoding
     type: integer
   pseudogene_count:
     display_group: annotation
     display_level: 2
     display_name: Pseudogene count
     constraint:
       min: 1
-    header: geneCountPseudogene
     type: integer
   noncoding_gene_count:
     display_group: annotation
     display_level: 2
     display_name: Non-coding gene count
     constraint:
       min: 1
-    header: geneCountNoncoding
     type: integer
   sample_sex:
     display_level: 2
     display_name: Sample sex
-    header: sex
     type: keyword
   isolate:
     display_level: 2
-    header: isolate
     display_name: Isolate
     type: keyword
   assembly_level:
     display_level: 1
-    header: assemblyLevel
     display_name: Assembly level
     type: keyword
-    taxon_display_group: assembly
-    taxon_summary:
-      - primary
-      - enum
     constraint:
       enum:
         - complete genome
         - chromosome
         - scaffold
         - contig
-    taxon_traverse: enum
-    taxon_traverse_direction: up
   assembly_type:
     display_level: 2
-    header: assemblyType
     display_name: Assembly type
     type: keyword
   assembly_span:
     display_group: metrics
     display_level: 1
     display_name: Assembly span
     constraint:
       min: 1
-    header: totalSequenceLength
     type: long
     units: bases
-    taxon_display_group: assembly
-    taxon_summary:
-      - primary
-      - median
-      - min
-      - max
-      - count
-    taxon_traverse: median
-    taxon_traverse_direction: both
     bins:
       min: 6
       max: 11
       count: 10
       scale: log10
   ungapped_span:
     display_group: metrics
     display_level: 2
     display_name: Ungapped span
     constraint:
       min: 1
-    header: totalUngappedLength
     type: long
     units: bases
   contig_n50:
     display_group: metrics
     display_level: 1
     display_name: Contig N50
     constraint:
       min: 1
-    header: contigN50
     type: long
     units: bases
-    taxon_display_group: assembly
-    taxon_summary:
-      - primary
-      - max
-      - median
-      - min
-      - count
-    taxon_traverse_direction: up
-    taxon_traverse: median
-    taxon_display_level: 2
     bins:
       min: 4
       max: 9
       count: 10
       scale: log10
   contig_l50:
     display_group: metrics
     display_level: 2
     display_name: Contig L50
     constraint:
       min: 1
-    header: contigL50
     type: long
     units: bases
   scaffold_n50:
     display_group: metrics
     display_level: 1
     display_name: Scaffold N50
     constraint:
       min: 1
-    header: scaffoldN50
     type: long
     units: bases
-    taxon_display_group: assembly
-    taxon_summary:
-      - primary
-      - max
-      - median
-      - min
-      - count
-    taxon_traverse_direction: up
-    taxon_traverse: median
-    taxon_display_level: 2
     bins:
       min: 4
       max: 9
       count: 10
       scale: log10
   scaffold_l50:
     display_group: metrics
     display_level: 2
     display_name: Scaffold L50
     constraint:
       min: 1
-    header: scaffoldL50
     type: long
     units: bases
   contig_count:
     display_group: metrics
     display_level: 1
     display_name: Contig count
     constraint:
       min: 1
-    header: numberOfContigs
     type: long
     units: bases
   scaffold_count:
     display_group: metrics
     display_level: 1
     display_name: Scaffold count
     constraint:
       min: 1
-    header: numberOfScaffolds
     type: long
     units: bases
   chromosome_count:
     display_group: metrics
     display_level: 1
     display_name: Chromosome count
     constraint:
       min: 1
-    header: totalNumberOfChromosomes
     type: long
     units: bases
   sequence_count:
     display_group: metrics
     display_level: 2
     display_name: Sequence count
     constraint:
       min: 1
-    header: numberOfComponentSequences
     type: long
     units: bases
   last_updated:
     display_level: 2
     display_name: Last updated
-    header: submissionDate
-    taxon_display_group: assembly
-    taxon_name: assembly_date
-    taxon_summary:
-      - primary
-      - max
-      - min
-    taxon_traverse: min
-    taxon_traverse_direction: up
     type: date
   ebp_metric_date:
     display_level: 2
     display_name: EBP metric date
-    header: ebpMetricDate
-    taxon_display_group: assembly
-    taxon_summary:
-      - min
-      - max
-    taxon_traverse: min
-    taxon_traverse_direction: up
     type: date
   refseq_category:
     display_level: 2
-    header: refseqCategory
     display_name: RefSeq category
     type: keyword
   submitter:
     display_level: 2
-    header: submitter
     display_name: Submitter
     type: keyword
-metadata:
-  source_slug:
-    header: genbankAssmAccession
-  is_primary_value:
-    header: primaryValue
+  gc_percent:
+    display_group: metrics
+    display_level: 1
+    constraint:
+      min: 0
+      max: 100
+    type: 2dp
+    units: "%"
+  n_percent:
+    display_group: metrics
+    display_level: 2
+    constraint:
+      min: 0
+      max: 100
+    type: 2dp
+    units: "%"
```

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/attributes.json` & `genomehubs-2.7.6/src/genomehubs/templates/attributes.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/busco.types.yaml` & `genomehubs-2.7.6/src/genomehubs/templates/busco.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/busco_feature.types.yaml` & `genomehubs-2.7.6/src/genomehubs/templates/busco_feature.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/feature.json` & `genomehubs-2.7.6/src/genomehubs/templates/feature.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/file.json` & `genomehubs-2.7.6/src/genomehubs/templates/file.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/identifiers.json` & `genomehubs-2.7.6/src/genomehubs/templates/identifiers.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/organelle.types.yaml` & `genomehubs-2.7.6/src/genomehubs/templates/ATTR_sample.types.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,133 +1,108 @@
-file:
-  display_group: general
-  format: tsv
-  header: true
-  source_url_stub: https://www.ncbi.nlm.nih.gov/nuccore/
-  source: NCBI
-attributes:
-  assembly_span:
-    display_group: metrics
-    display_level: 1
-    constraint:
-      min: 1
-    index: 8
-    type: long
-    units: bases
-    taxon_display_group: "{{organelle}}_assembly"
-    taxon_name: "{{organelle}}_assembly_span"
-    taxon_key: "{{organelle}}_assembly_span"
-    taxon_display_name: "{{organelle}} span"
-    taxon_summary: median
-    taxon_traverse: median
-    taxon_traverse_limit: phylum
-    taxon_display_level: 2
-    taxon_bins:
-      min: 3
-      max: 8
-      count: 10
-      scale: log10
-  bioproject:
+defaults:
+  attributes:
+    display_group: general
+    organelle: nucleus
+    source_url_stub: https://www.ncbi.nlm.nih.gov/assembly/
+    source: INSDC
+    taxon_display_group: sample
+identifiers:
+  sample_id:
     constraint:
       len: 32
-    index: 5
-    synonyms:
-      - bioproject_accession
     type: keyword
-  biosample:
-    constraint:
-      len: 32
-    index: 6
-    synonyms:
-      - biosample_accession
+attributes:
+  sample_sex:
+    display_level: 2
+    display_name: Sample sex
     type: keyword
-  organelle:
-    constraint:
-      enum:
-        - nucleus
-        - mitochondrion
-        - chloroplast
-        - plastid
-        - apicoplast
-    default: "{{organelle}}"
+    taxon_display_group: sample
+    taxon_summary:
+      - primary
+      - list
+      - count
+    taxon_display_level: 2
+  isolate:
+    display_level: 2
+    display_name: Isolate
     type: keyword
-  gc_percent:
-    display_group: metrics
-    display_level: 1
+  estimated_genome_size:
+    display_level: 2
+    display_name: Estimated genome size
+    type: keyword
+  location_name:
+    display_level: 2
+    display_name: Location name
+    type: keyword
+  num_replicons:
     constraint:
-      min: 0
-      max: 100
-    index: 9
-    type: 2dp
-    units: "%"
-    taxon_display_group: "{{organelle}}_assembly"
-    taxon_display_name: "{{organelle}} GC%"
-    taxon_name: "{{organelle}}_gc_percent"
-    taxon_key: "{{organelle}}_gc_percent"
-    taxon_summary: median
-    taxon_traverse: median
-    taxon_traverse_limit: phylum
-    taxon_display_level: 2
-    taxon_bins:
-      min: 0
-      max: 100
-      count: 10
-      scale: linear
-  n_percent:
-    display_group: metrics
+      max: 32767
+    display_level: 2
+    display_name: Number of replicons
+    type: short
+  ploidy:
     display_level: 1
+    display_name: Ploidy
+    translate:
+      1n: 1
+      haoloid: 1
+      haoploid: 1
+      haploid: 1
+      haploidy: 1
+      heploid: 1
+      monokaryotic, haploid: 1
+      haploid/diploid: [1, 2]
+      haplo-diploidy: [1, 2]
+      "Male: haploid; female: diploid": [1, 2]
+      2n: 2
+      diploid: 2
+      diploidy: 2
+      dipolid: 2
+      diploid, occasionally higher: 2
+      diplod: 2
+      diplioid: 2
+      dipliod: 2
+      Haploid consensus of diploid genome: 2
+      Diploid (presumed): 2
+      protandrous diploid: 2
+      triploid: 3
+      allotetraploid: 4
+      allotetraploids: 4
+      protandrous tetraploid: 4
+      tetraploid: 4
+      hexaploid: 6
+      allopolyploid: NA
+      amphidiploid: NA
+      dikaryon: NA
+      dikaryotic: NA
+      polyploid macronucleus: NA
+      singal spore: NA
+      possible triploid: NA
+      polyploidy: NA
+      polyploid: NA
+      haploid /Dikaryon: NA
+      doubled haploid: NA
+      double ploidy level: NA
+      dikariotic (diploid): NA
+      Polyploid: NA
+      Dikaryon: NA
+      ">2n": NA
+      "0": NA
+    type: short
+  elevation:
     constraint:
-      min: 0
-      max: 100
-    index: 10
-    type: 2dp
-    units: "%"
-  last_updated:
+      max: 8500
     display_level: 2
-    index: 11
-    type: date
+    display_name: Elevation
+    type: short
+    unit: "m"
   sample_location:
-    display_level: 2
-    index: 12
+    h3res: 5
+    display_level: 1
+    display_name: location
     type: geo_point
-    taxon_display_group: "{{organelle}}_assembly"
-    taxon_name: "{{organelle}}_sample_location"
-    taxon_key: "{{organelle}}_sample_location"
-    taxon_display_name: "{{organelle}} sample location"
-    taxon_summary: list
+    taxon_display_group: sample
+    taxon_summary:
+      - list
+    taxon_traverse: list
+    taxon_traverse_direction: up
     taxon_display_level: 2
-identifiers:
-  assembly_id:
-    constraint:
-      len: 32
-    index: 3
-    type: keyword
-  genbank_accession:
-    constraint:
-      len: 32
-    index: 4
-    type: keyword
-  refseq_accession:
-    constraint:
-      len: 32
-    index: 3
-    type: keyword
-metadata:
-  organelle:
-    index: 7
-  source_author:
-    index: 13
-  source_year:
-    index: 14
-  source_title:
-    index: 15
-  source_pubmed_id:
-    index: 16
-  source_slug:
-    index: 3
-taxonomy:
-  taxon:
-    index: 0
-  taxon_id:
-    index: 1
-  lineage:
-    index: 2
```

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/sample.json` & `genomehubs-2.7.6/src/genomehubs/templates/sample.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/assembly_lookup.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/assembly_lookup.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/assembly_suggest.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/assembly_suggest.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/attribute_values_by_taxon.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/attribute_values_by_taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/max_nested_value_by_type.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/max_nested_value_by_type.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_any_name.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_any_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_lineage.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_name.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_specific_name.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_specific_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_lookup.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_lookup.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_suggest.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_suggest.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/scripts/value_by_type_by_lineage.json` & `genomehubs-2.7.6/src/genomehubs/templates/scripts/value_by_type_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/taxon.json` & `genomehubs-2.7.6/src/genomehubs/templates/taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/taxon.types.yaml` & `genomehubs-2.7.6/src/genomehubs/templates/taxon.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/taxonomy.json` & `genomehubs-2.7.6/src/genomehubs/templates/taxonomy.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/window_full.types.yaml` & `genomehubs-2.7.6/src/genomehubs/templates/window_full.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs/templates/window_stats.types.yaml` & `genomehubs-2.7.6/src/genomehubs/templates/window_stats.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.5/src/genomehubs.egg-info/PKG-INFO` & `genomehubs-2.7.6/src/genomehubs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomehubs
-Version: 2.7.5
+Version: 2.7.6
 Summary: GenomeHubs
 Home-page: https://github.com/genomehubs/genomehubs
 Author: genomehubs
 Author-email: genomehubs@genomehubs.org
 Project-URL: Bug Reports, https://github.com/genomehubs/genomehubs/issues
 Project-URL: Source, https://github.com/genomehubs/genomehubs
 Keywords: bioinformatics
```

### Comparing `genomehubs-2.7.5/src/genomehubs.egg-info/SOURCES.txt` & `genomehubs-2.7.6/src/genomehubs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,21 @@
 src/genomehubs/lib/taxon.py
 src/genomehubs/lib/taxonomy.py
 src/genomehubs/lib/test.py
 src/genomehubs/lib/validate.py
 src/genomehubs/lib/version.py
 src/genomehubs/lib/wikidata.py
 src/genomehubs/lib/window.py
+src/genomehubs/templates/ATTR_assembly.types.yaml
+src/genomehubs/templates/ATTR_btk.types.yaml
 src/genomehubs/templates/ATTR_busco.types.yaml
 src/genomehubs/templates/ATTR_feature.types.yaml
+src/genomehubs/templates/ATTR_sample.types.yaml
 src/genomehubs/templates/ATTR_window_stats.types.yaml
+src/genomehubs/templates/TAXON_assembly.types.yaml
 src/genomehubs/templates/analysis.json
 src/genomehubs/templates/assembly.json
 src/genomehubs/templates/assembly.types.yaml
 src/genomehubs/templates/attributes.json
 src/genomehubs/templates/btk.types.yaml
 src/genomehubs/templates/busco.types.yaml
 src/genomehubs/templates/busco_feature.types.yaml
```

