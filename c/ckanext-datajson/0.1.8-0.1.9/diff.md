# Comparing `tmp/ckanext-datajson-0.1.8.tar.gz` & `tmp/ckanext-datajson-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-datajson-0.1.8.tar", last modified: Fri Nov 11 16:19:54 2022, max compression
+gzip compressed data, was "ckanext-datajson-0.1.9.tar", last modified: Wed Nov 16 17:32:54 2022, max compression
```

## Comparing `ckanext-datajson-0.1.8.tar` & `ckanext-datajson-0.1.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.671636 ckanext-datajson-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6621 2022-11-11 16:19:54.671636 ckanext-datajson-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5061 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.663636 ckanext-datajson-0.1.8/ckanext/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.663636 ckanext-datajson-0.1.8/ckanext/datajson/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15988 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (121)    37546 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/datajson.py
--rw-r--r--   0 runner    (1001) docker     (121)     8063 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/datajsonvalidator.py
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.667636 ckanext-datajson-0.1.8/ckanext/datajson/export_map/
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/export_map/export.catalog.map.sample.json
--rw-r--r--   0 runner    (1001) docker     (121)     3659 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/export_map/export.inventory.map.sample.json
--rw-r--r--   0 runner    (1001) docker     (121)     3522 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/export_map/export.spatial.map.sample.json
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/harvester_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3651 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/harvester_cmsdatanavigator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/harvester_datajson.py
--rw-r--r--   0 runner    (1001) docker     (121)     6905 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    19105 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/package2pod.py
--rw-r--r--   0 runner    (1001) docker     (121)     7973 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/parse_datajson.py
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.667636 ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.667636 ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/federal-v1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/federal-v1.1/catalog.json
--rw-r--r--   0 runner    (1001) docker     (121)    24019 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/federal-v1.1/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.667636 ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/non-federal/
--rw-r--r--   0 runner    (1001) docker     (121)    19588 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/non-federal/single_entry.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.667636 ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/non-federal-v1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/non-federal-v1.1/catalog.json
--rw-r--r--   0 runner    (1001) docker     (121)    20053 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/non-federal-v1.1/dataset-non-federal.json
--rw-r--r--   0 runner    (1001) docker     (121)    19860 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/single_entry.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.667636 ckanext-datajson-0.1.8/ckanext/datajson/resources/
--rw-r--r--   0 runner    (1001) docker     (121)    13149 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/resources/harvest-to-program-codes.json
--rw-r--r--   0 runner    (1001) docker     (121)    78378 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/resources/omb-agency-bureau-treasury-codes.json
--rw-r--r--   0 runner    (1001) docker     (121)    29245 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/resources/omb_bureau_codes.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.659636 ckanext-datajson-0.1.8/ckanext/datajson/templates_datajson/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.667636 ckanext-datajson-0.1.8/ckanext/datajson/templates_datajson/organization/
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/templates_datajson/organization/read.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.667636 ckanext-datajson-0.1.8/ckanext/datajson/templates_validator/
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/templates_validator/datajsonvalidator.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.667636 ckanext-datajson-0.1.8/ckanext/datajson/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (121)     3984 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/tests/mock_datajson_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     5354 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/tests/test_collections_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)    25907 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/tests/test_datajson_ckan_all_harvester.py
--rw-r--r--   0 runner    (1001) docker     (121)     5279 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/tests/test_datajson_validation.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7146 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext/datajson/tests/test_export.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:19:54.671636 ckanext-datajson-0.1.8/ckanext_datajson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6621 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext_datajson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1927 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext_datajson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext_datajson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext_datajson.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext_datajson.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext_datajson.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext_datajson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/ckanext_datajson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-11-11 16:19:54.671636 ckanext-datajson-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-11-11 16:19:54.000000 ckanext-datajson-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6621 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5061 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.551537 ckanext-datajson-0.1.9/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/ckanext/datajson/
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16593 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37546 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/datajson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8063 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/datajsonvalidator.py
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/ckanext/datajson/export_map/
+-rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/export_map/export.catalog.map.sample.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3659 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/export_map/export.inventory.map.sample.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3522 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/export_map/export.spatial.map.sample.json
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/harvester_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3579 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/harvester_cmsdatanavigator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3266 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/harvester_datajson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6905 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19105 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/package2pod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7973 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/parse_datajson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/federal-v1.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/federal-v1.1/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (121)    24019 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/federal-v1.1/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/non-federal/
+-rw-r--r--   0 runner    (1001) docker     (121)    19588 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/non-federal/single_entry.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/non-federal-v1.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/non-federal-v1.1/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (121)    20053 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/non-federal-v1.1/dataset-non-federal.json
+-rw-r--r--   0 runner    (1001) docker     (121)    19860 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/single_entry.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/ckanext/datajson/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)    13149 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/resources/harvest-to-program-codes.json
+-rw-r--r--   0 runner    (1001) docker     (121)    78378 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/resources/omb-agency-bureau-treasury-codes.json
+-rw-r--r--   0 runner    (1001) docker     (121)    29245 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/resources/omb_bureau_codes.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.551537 ckanext-datajson-0.1.9/ckanext/datajson/templates_datajson/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/ckanext/datajson/templates_datajson/organization/
+-rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/templates_datajson/organization/read.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/ckanext/datajson/templates_validator/
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/templates_validator/datajsonvalidator.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/ckanext/datajson/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4102 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/tests/mock_datajson_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5354 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/tests/test_collections_ui.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26575 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/tests/test_datajson_ckan_all_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5291 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/tests/test_datajson_validation.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7146 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext/datajson/tests/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/ckanext_datajson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6621 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext_datajson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1927 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext_datajson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext_datajson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext_datajson.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext_datajson.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext_datajson.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext_datajson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/ckanext_datajson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-11-16 17:32:54.555538 ckanext-datajson-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-11-16 17:32:54.000000 ckanext-datajson-0.1.9/setup.py
```

### Comparing `ckanext-datajson-0.1.8/PKG-INFO` & `ckanext-datajson-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-datajson
-Version: 0.1.8
+Version: 0.1.9
 Summary: CKAN extension to generate /data.json
 Home-page: https://github.com/GSA/ckanext-datajson
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: Public Domain
 Description: # ckanext-datajson
```

### Comparing `ckanext-datajson-0.1.8/README.md` & `ckanext-datajson-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/blueprint.py` & `ckanext-datajson-0.1.9/ckanext/datajson/blueprint.py`

 * *Files 3% similar despite different names*

```diff
@@ -329,26 +329,36 @@
     # Validates that a URL is a good data.json file.
     if request.method == "POST":
         c.errors = []
         try:
             assert request.form.get('url').strip() != ""
             c.source_url = request.form.get('url').strip()
 
-            import urllib.request
-            import urllib.parse
-            import urllib.error
-            import json
+            import requests
+            try:
+                from requests.exceptions import JSONDecodeError
+            except ImportError:
+                from simplejson.scanner import JSONDecodeError
             from collections import deque
 
             body = None
             try:
-                body = json.load(urllib.request.urlopen(c.source_url))
-            except IOError as e:
-                c.errors.append(("Error Loading File", ["The address could not be loaded: " + str(e)]))
-            except ValueError as e:
+                response = requests.get(c.source_url)
+                response.raise_for_status()
+                body = response.json()
+            except requests.exceptions.ProxyError as e:
+                c.errors.append((
+                    "Error Connecting URL",
+                    ["Addresses other than .gov, .mil or github.com domain could not be reached: " + str(e)]
+                ))
+            except requests.exceptions.ConnectionError as e:
+                c.errors.append(("Error Connecting URL", ["The address could not be accessed: " + str(e)]))
+            except requests.exceptions.HTTPError as e:
+                c.errors.append(("Error Loading URL", ["The address could not be loaded: " + str(e)]))
+            except JSONDecodeError as e:
                 c.errors.append(("Invalid JSON", ["The file does not meet basic JSON syntax requirements: " + str(
                     e) + ". Try using JSONLint.com."]))
             except Exception as e:
                 c.errors.append((
                     "Internal Error",
                     ["Something bad happened while trying to load and parse the file: " + str(e)]))
```

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/datajson.py` & `ckanext-datajson-0.1.9/ckanext/datajson/datajson.py`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/datajsonvalidator.py` & `ckanext-datajson-0.1.9/ckanext/datajson/datajsonvalidator.py`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/export_map/export.catalog.map.sample.json` & `ckanext-datajson-0.1.9/ckanext/datajson/export_map/export.catalog.map.sample.json`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/export_map/export.inventory.map.sample.json` & `ckanext-datajson-0.1.9/ckanext/datajson/export_map/export.inventory.map.sample.json`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/export_map/export.spatial.map.sample.json` & `ckanext-datajson-0.1.9/ckanext/datajson/export_map/export.spatial.map.sample.json`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/harvester_cmsdatanavigator.py` & `ckanext-datajson-0.1.9/ckanext/datajson/harvester_cmsdatanavigator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from __future__ import division
 from __future__ import print_function
 from future import standard_library
 standard_library.install_aliases()
 from past.utils import old_div
 from ckanext.datajson.harvester_base import DatasetHarvesterBase
 
-import urllib.request
-import urllib.error
-import urllib.parse
-import json
+import requests
 import re
 import datetime
 
 
 class CmsDataNavigatorHarvester(DatasetHarvesterBase):
     '''
     A Harvester for the CMS Data Navigator catalog.
@@ -24,15 +21,15 @@
         return {
             'name': 'cms-data-navigator',
             'title': 'CMS Data Navigator',
             'description': 'Harvests CMS Data Navigator-style catalogs.',
         }
 
     def load_remote_catalog(self, harvest_job):
-        catalog = json.load(urllib.request.urlopen(harvest_job.source.url))
+        catalog = requests.get(harvest_job.source.url).json()
         for item in catalog:
             item["identifier"] = item["ID"]
             item["title"] = item["Name"].strip()
         return catalog
 
     def set_dataset_info(self, package, dataset, dataset_defaults):
         extra(package, "Agency", "Department of Health & Human Services")
```

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/harvester_datajson.py` & `ckanext-datajson-0.1.9/ckanext/datajson/harvester_datajson.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import absolute_import
 from future import standard_library
 standard_library.install_aliases()
 from ckanext.datajson.harvester_base import DatasetHarvesterBase
 from .parse_datajson import parse_datajson_entry
 
+import requests
 
-import json
-import urllib.error
-import urllib.parse
-import urllib.request
+try:
+    from requests.exceptions import JSONDecodeError
+except ImportError:
+    from simplejson.scanner import JSONDecodeError
 
 
 class DataJsonHarvester(DatasetHarvesterBase):
     '''
     A Harvester for /data.json files.
     '''
 
@@ -22,42 +23,37 @@
         return {
             'name': 'datajson',
             'title': '/data.json',
             'description': 'Harvests remote /data.json files',
         }
 
     def load_remote_catalog(self, harvest_job):
-        req = urllib.request.Request(harvest_job.source.url)
+        url = harvest_job.source.url
         # todo: into config and across harvester
-        req.add_header('User-agent', 'Data.gov/2.0')
+        headers = {'User-Agent': 'Data.gov/2.0'}
         try:
-            response = urllib.request.urlopen(req)
-        except urllib.error.HTTPError as e:
-            self._save_gather_error("HTTP Error getting json source: %s." % (e), harvest_job)
+            response = requests.get(url, headers=headers)
+        except requests.exceptions.ProxyError as e:
+            self._save_gather_error("ProxyError getting json source: %s." % (e), harvest_job)
             return []
-        except urllib.error.URLError as e:
-            self._save_gather_error("URL Error getting json source: %s." % (e), harvest_job)
+        except requests.exceptions.ConnectionError as e:
+            self._save_gather_error("ConnectionError getting json source: %s." % (e), harvest_job)
             return []
 
-        data = response.read()
         try:
-            datasets = json.loads(data)
-        except UnicodeDecodeError:
-            # try different encode
-            try:
-                datasets = json.loads(data, 'cp1252')
-            except BaseException:
-                try:
-                    datasets = json.loads(data, 'iso-8859-1')
-                except BaseException as e:
-                    self._save_gather_error("Error loading json with 'cp1252' and 'iso-8859-1': %s" % (e), harvest_job)
-                    return []
-        except BaseException:
-            # remove BOM
-            datasets = json.loads(lstrip_bom(data))
+            response.raise_for_status()
+        except requests.exceptions.HTTPError as e:
+            self._save_gather_error("HTTPError getting json source: %s." % (e), harvest_job)
+            return []
+
+        try:
+            datasets = response.json()
+        except JSONDecodeError as e:
+            self._save_gather_error("JSONDecodeError loading json. %s" % (e), harvest_job)
+            return []
 
         # The first dataset should be for the data.json file itself. Check that
         # it is, and if so rewrite the dataset's title because Socrata exports
         # these items all with the same generic name that is confusing when
         # harvesting a bunch from different sources. It should have an accessURL
         # but Socrata fills the URL of these in under webService.
         if (isinstance(datasets, list) and len(datasets) > 0  # NOQA W503 W504
```

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/helpers.py` & `ckanext-datajson-0.1.9/ckanext/datajson/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/package2pod.py` & `ckanext-datajson-0.1.9/ckanext/datajson/package2pod.py`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/parse_datajson.py` & `ckanext-datajson-0.1.9/ckanext/datajson/parse_datajson.py`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/plugin.py` & `ckanext-datajson-0.1.9/ckanext/datajson/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/federal-v1.1/catalog.json` & `ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/federal-v1.1/catalog.json`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/federal-v1.1/dataset.json` & `ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/federal-v1.1/dataset.json`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/non-federal/single_entry.json` & `ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/non-federal/single_entry.json`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/non-federal-v1.1/catalog.json` & `ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/non-federal-v1.1/catalog.json`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/non-federal-v1.1/dataset-non-federal.json` & `ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/non-federal-v1.1/dataset-non-federal.json`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/pod_schema/single_entry.json` & `ckanext-datajson-0.1.9/ckanext/datajson/pod_schema/single_entry.json`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/resources/harvest-to-program-codes.json` & `ckanext-datajson-0.1.9/ckanext/datajson/resources/harvest-to-program-codes.json`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/resources/omb-agency-bureau-treasury-codes.json` & `ckanext-datajson-0.1.9/ckanext/datajson/resources/omb-agency-bureau-treasury-codes.json`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/resources/omb_bureau_codes.csv` & `ckanext-datajson-0.1.9/ckanext/datajson/resources/omb_bureau_codes.csv`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/templates_datajson/organization/read.html` & `ckanext-datajson-0.1.9/ckanext/datajson/templates_datajson/organization/read.html`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/templates_validator/datajsonvalidator.html` & `ckanext-datajson-0.1.9/ckanext/datajson/templates_validator/datajsonvalidator.html`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/tests/factories.py` & `ckanext-datajson-0.1.9/ckanext/datajson/tests/factories.py`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/tests/mock_datajson_source.py` & `ckanext-datajson-0.1.9/ckanext/datajson/tests/mock_datajson_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,17 @@
             self.test_name = 'error-reserved-title'
         elif self.path == '/error-large-spatial':
             self.sample_datajson_file = 'large-spatial.data.json'
             self.test_name = 'error-large-spatial'
         elif self.path == '/null-spatial':
             self.sample_datajson_file = 'null-spatial.data.json'
             self.test_name = 'null-spatial'
+        elif self.path == '/text':
+            self.test_name = 'test'
+            self.respond('abc123', status=200)
         elif self.path == '/404':
             self.test_name = 'e404'
             self.respond('Not found', status=404)
         elif self.path == '/500':
             self.test_name = 'e500'
             self.respond('Error', status=500)
```

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/tests/test_collections_ui.py` & `ckanext-datajson-0.1.9/ckanext/datajson/tests/test_collections_ui.py`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/tests/test_datajson_ckan_all_harvester.py` & `ckanext-datajson-0.1.9/ckanext/datajson/tests/test_datajson_ckan_all_harvester.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from datetime import datetime
 import json
 import logging
 
 import pytest
 
-from urllib.error import URLError
-
 import ckan.plugins as p
 import ckanext.harvest.model as harvest_model
 import ckanext.harvest.queue as queue
 from . import mock_datajson_source
 from ckan import model
 from ckan.lib.munge import munge_title_to_name
 from ckanext.datajson.harvester_datajson import DataJsonHarvester
@@ -222,28 +220,43 @@
         tags = [tag.name for tag in dataset.get_tags()]
         assert len(dataset.resources) == 1
         assert munge_title_to_name("Congressional Logs") in tags
 
     def test_source_returning_http_error(self):
         url = 'http://127.0.0.1:%s/404' % self.mock_port
         self.run_source(url)
+        assert self.job.gather_errors[0].message == ("HTTPError getting json source: "
+                                                     "404 Client Error: Not Found for url: %s.") % url
+        assert self.job.gather_errors[1].message == ("Error loading json content:"
+                                                     " not enough values to unpack"
+                                                     " (expected 2, got 0).")
 
-        pytest.raises(URLError)
-        assert self.job.gather_errors[0].message == "HTTP Error getting json source: HTTP Error 404: Not Found."
+        url = 'http://127.0.0.1:%s/500' % self.mock_port
+        self.run_source(url)
+        assert self.job.gather_errors[0].message == ("HTTPError getting json source: 500 Server Error: "
+                                                     "Internal Server Error for url: %s.") % url
         assert self.job.gather_errors[1].message == ("Error loading json content:"
                                                      " not enough values to unpack"
                                                      " (expected 2, got 0).")
 
     def test_source_returning_url_error(self):
         # URL failing SSL
         url = 'https://127.0.0.1:%s' % self.mock_port
         self.run_source(url)
 
-        pytest.raises(URLError)
-        assert "URL Error getting json source: <urlopen error" in self.job.gather_errors[0].message
+        assert "ConnectionError getting json source: HTTPSConnectionPool" in self.job.gather_errors[0].message
+        assert self.job.gather_errors[1].message == ("Error loading json content:"
+                                                     " not enough values to unpack"
+                                                     " (expected 2, got 0).")
+
+    def test_json_decode_error(self):
+        url = 'http://127.0.0.1:%s/text' % self.mock_port
+
+        self.run_source(url)
+        assert "JSONDecodeError loading json." in self.job.gather_errors[0].message
         assert self.job.gather_errors[1].message == ("Error loading json content:"
                                                      " not enough values to unpack"
                                                      " (expected 2, got 0).")
 
     def get_datasets_from_2_collection(self):
         url = 'http://127.0.0.1:%s/collection-2-parent-4-children.data.json' % self.mock_port
         obj_ids = self.run_gather(url=url)
@@ -620,17 +633,7 @@
 
     def test_datajson_null_spatial(self):
         url = 'http://127.0.0.1:%s/null-spatial' % self.mock_port
         datasets = self.run_source(url=url)
         dataset = datasets[0]
         expected_title = "Sample Title NUll Spatial"
         assert dataset.title == expected_title
-
-    def test_datason_404(self):
-        url = 'http://127.0.0.1:%s/404' % self.mock_port
-        self.run_source(url=url)
-        pytest.raises(URLError)
-
-    def test_datason_500(self):
-        url = 'http://127.0.0.1:%s/500' % self.mock_port
-        self.run_source(url=url)
-        pytest.raises(URLError)
```

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/tests/test_datajson_validation.py` & `ckanext-datajson-0.1.9/ckanext/datajson/tests/test_datajson_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         assert res.status_code == 200
         assert 'No Errors' in res.body
         assert 'Great job!' in res.body
 
     def test_data_json_bad_link(self, app):
         ''' Test that a bad link fails '''
 
-        res = app.post('/dcat-us/validator', data={'url': 'data.gov'})
+        res = app.post('/dcat-us/validator', data={'url': 'http://data.gov'})
 
         assert res.status_code == 200
         assert 'Invalid JSON' in res.body
         assert 'The file does not meet basic JSON syntax requirements' in res.body
 
     def test_data_json_missing_dataset_fields(self, app):
         ''' Test that an invalid data.json that is missing dataset fields fails '''
@@ -115,18 +115,18 @@
     def test_data_json_unresolvable(self, app):
 
         res = app.post('/dcat-us/validator', data={
             'url': 'http://some.unresolvable.hostname.fer-reals/data.json'
         })
 
         assert res.status_code == 200
-        assert 'Error Loading File' in res.body
-        assert 'The address could not be loaded' in res.body
+        assert 'Error Connecting URL' in res.body
+        assert 'The address could not be accessed' in res.body
 
         res = app.post('/dcat-us/validator', data={
             'url': 'https://www.google.com:443/data.json'
         })
 
         assert res.status_code == 200
-        assert 'Error Loading File' in res.body
+        assert 'Error Loading URL' in res.body
         assert 'The address could not be loaded' in res.body
-        assert 'HTTP Error 404' in res.body
+        assert '404 Client Error' in res.body
```

### Comparing `ckanext-datajson-0.1.8/ckanext/datajson/tests/test_export.py` & `ckanext-datajson-0.1.9/ckanext/datajson/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/ckanext_datajson.egg-info/PKG-INFO` & `ckanext-datajson-0.1.9/ckanext_datajson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-datajson
-Version: 0.1.8
+Version: 0.1.9
 Summary: CKAN extension to generate /data.json
 Home-page: https://github.com/GSA/ckanext-datajson
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: Public Domain
 Description: # ckanext-datajson
```

### Comparing `ckanext-datajson-0.1.8/ckanext_datajson.egg-info/SOURCES.txt` & `ckanext-datajson-0.1.9/ckanext_datajson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-datajson-0.1.8/setup.py` & `ckanext-datajson-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ckanext-datajson',
-    version='0.1.8',
+    version='0.1.9',
     description="CKAN extension to generate /data.json",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python :: 3'
     ],  # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     keywords='',
```

