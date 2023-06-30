# Comparing `tmp/pyatlan-0.1.3.tar.gz` & `tmp/pyatlan-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.1.3.tar", last modified: Mon Jun 19 11:26:22 2023, max compression
+gzip compressed data, was "pyatlan-0.2.0.tar", last modified: Fri Jun 30 12:17:20 2023, max compression
```

## Comparing `pyatlan-0.1.3.tar` & `pyatlan-0.2.0.tar`

### file list

```diff
@@ -1,106 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.771959 pyatlan-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-19 11:26:11.000000 pyatlan-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 11:26:11.000000 pyatlan-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-19 11:26:11.000000 pyatlan-0.1.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-19 11:26:22.771959 pyatlan-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-19 11:26:11.000000 pyatlan-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.759959 pyatlan-0.1.3/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.763959 pyatlan-0.1.3/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.763959 pyatlan-0.1.3/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43669 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.763959 pyatlan-0.1.3/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.763959 pyatlan-0.1.3/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.767959 pyatlan-0.1.3/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   986605 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    56226 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.763959 pyatlan-0.1.3/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-19 11:26:22.000000 pyatlan-0.1.3/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-19 11:26:22.000000 pyatlan-0.1.3/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 11:26:22.000000 pyatlan-0.1.3/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 11:26:22.000000 pyatlan-0.1.3/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-19 11:26:22.000000 pyatlan-0.1.3/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 11:26:22.000000 pyatlan-0.1.3/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 11:26:22.771959 pyatlan-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-19 11:26:11.000000 pyatlan-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.767959 pyatlan-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.767959 pyatlan-0.1.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35674 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/persona_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/purpose_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/test_sql_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.771959 pyatlan-0.1.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.771959 pyatlan-0.1.3/tests/unit/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/badge_condition_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/badge_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/column_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/glossary_category_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/glossary_term_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/materialised_view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/process_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/readme_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/s3_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/s3object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31770 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.100695 pyatlan-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-30 12:17:06.000000 pyatlan-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 12:17:06.000000 pyatlan-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-30 12:17:06.000000 pyatlan-0.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-30 12:17:20.100695 pyatlan-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-30 12:17:06.000000 pyatlan-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.080695 pyatlan-0.2.0/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.084695 pyatlan-0.2.0/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/atlan_tag_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.084695 pyatlan-0.2.0/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47536 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.084695 pyatlan-0.2.0/pyatlan/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/events/atlan_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/events/atlan_lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.084695 pyatlan-0.2.0/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.084695 pyatlan-0.2.0/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.088696 pyatlan-0.2.0/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   982643 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56219 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60973 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24877 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.080695 pyatlan-0.2.0/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-30 12:17:20.000000 pyatlan-0.2.0/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-30 12:17:20.000000 pyatlan-0.2.0/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:17:20.000000 pyatlan-0.2.0/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:17:19.000000 pyatlan-0.2.0/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 12:17:20.000000 pyatlan-0.2.0/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 12:17:20.000000 pyatlan-0.2.0/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:17:20.100695 pyatlan-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-30 12:17:06.000000 pyatlan-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.088696 pyatlan-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.092696 pyatlan-0.2.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/atlan_tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35670 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/persona_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/purpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/test_sql_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.096696 pyatlan-0.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.100695 pyatlan-0.2.0/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/badge_condition_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/badge_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/column_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/glossary_category_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/glossary_term_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/materialised_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/readme_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/s3_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/s3object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_atlan_tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30532 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36634 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.1.3/LICENSE` & `pyatlan-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/PKG-INFO` & `pyatlan-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.1.3
+Version: 0.2.0
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.1.3/README.md` & `pyatlan-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/cache/classification_cache.py` & `pyatlan-0.2.0/pyatlan/cache/atlan_tag_cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 from typing import Optional
 
 from pyatlan.model.enums import AtlanTypeCategory
-from pyatlan.model.typedef import ClassificationDef
+from pyatlan.model.typedef import AtlanTagDef
 
 
-class ClassificationCache:
-    cache_by_id: dict[str, ClassificationDef] = dict()
+class AtlanTagCache:
+    cache_by_id: dict[str, AtlanTagDef] = dict()
     map_id_to_name: dict[str, str] = dict()
     map_name_to_id: dict[str, str] = dict()
     deleted_ids: set[str] = set()
     deleted_names: set[str] = set()
 
     @classmethod
     def refresh_cache(cls) -> None:
@@ -21,20 +21,20 @@
         if client is None:
             client = AtlanClient()
         response = client.get_typedefs(type_category=AtlanTypeCategory.CLASSIFICATION)
         if response is not None:
             cls.cache_by_id = {}
             cls.map_id_to_name = {}
             cls.map_name_to_id = {}
-            for classification in response.classification_defs:
-                classification_id = classification.name
-                classification_name = classification.display_name
-                cls.cache_by_id[classification_id] = classification
-                cls.map_id_to_name[classification_id] = classification_name
-                cls.map_name_to_id[classification_name] = classification_id
+            for atlan_tag in response.atlan_tag_defs:
+                atlan_tag_id = atlan_tag.name
+                atlan_tag_name = atlan_tag.display_name
+                cls.cache_by_id[atlan_tag_id] = atlan_tag
+                cls.map_id_to_name[atlan_tag_id] = atlan_tag_name
+                cls.map_name_to_id[atlan_tag_name] = atlan_tag_id
 
     @classmethod
     def get_id_for_name(cls, name: str) -> Optional[str]:
         """
         Translate the provided human-readable classification name to its Atlan-internal ID string.
         """
         cls_id = cls.map_name_to_id.get(name)
```

### Comparing `pyatlan-0.1.3/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.2.0/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/cache/enum_cache.py` & `pyatlan-0.2.0/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/cache/group_cache.py` & `pyatlan-0.2.0/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/cache/role_cache.py` & `pyatlan-0.2.0/pyatlan/cache/role_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     map_name_to_id: dict[str, str] = dict()
 
     @classmethod
     def _refresh_cache(cls) -> None:
         client = AtlanClient.get_default_client()
         if client is None:
             client = AtlanClient()
-        response = client.get_all_roles()
+        response = client.get_roles(limit=100, post_filter='{"name":{"$ilike":"$%"}}')
         if response is not None:
             cls.cache_by_id = {}
             cls.map_id_to_name = {}
             cls.map_name_to_id = {}
             for role in response.records:
                 role_id = role.id
                 role_name = role.name
```

### Comparing `pyatlan-0.1.3/pyatlan/cache/user_cache.py` & `pyatlan-0.2.0/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/client/atlan.py` & `pyatlan-0.2.0/pyatlan/client/atlan.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from typing import ClassVar, Generator, Optional, Type, TypeVar, Union
 
 import requests
 from pydantic import (
     BaseSettings,
     HttpUrl,
     PrivateAttr,
+    StrictStr,
     ValidationError,
+    constr,
     parse_obj_as,
     validate_arguments,
 )
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from pyatlan.client.constants import (
@@ -73,18 +75,18 @@
 )
 from pyatlan.model.atlan_image import AtlanImage
 from pyatlan.model.core import (
     Announcement,
     AssetRequest,
     AssetResponse,
     AtlanObject,
+    AtlanTag,
+    AtlanTagName,
+    AtlanTags,
     BulkRequest,
-    Classification,
-    ClassificationName,
-    Classifications,
 )
 from pyatlan.model.custom_metadata import CustomMetadataDict, CustomMetadataRequest
 from pyatlan.model.enums import (
     AtlanConnectorType,
     AtlanDeleteType,
     AtlanTypeCategory,
     CertificateStatus,
@@ -102,17 +104,25 @@
     LineageListResponse,
     LineageRequest,
     LineageResponse,
 )
 from pyatlan.model.query import ParsedQuery, QueryParserRequest
 from pyatlan.model.response import AssetMutationResponse
 from pyatlan.model.role import RoleResponse
-from pyatlan.model.search import DSL, IndexSearchRequest, Term
+from pyatlan.model.search import (
+    DSL,
+    IndexSearchRequest,
+    Query,
+    Term,
+    with_active_category,
+    with_active_glossary,
+    with_active_term,
+)
 from pyatlan.model.typedef import (
-    ClassificationDef,
+    AtlanTagDef,
     CustomMetadataDef,
     EnumDef,
     TypeDef,
     TypeDefResponse,
 )
 from pyatlan.model.user import (
     AddToGroupsRequest,
@@ -163,38 +173,38 @@
     session = requests.session()
     session.mount("https://", adapter)
     session.headers.update({"x-atlan-agent": "sdk", "x-atlan-agent-id": "python"})
     return session
 
 
 def _build_typedef_request(typedef: TypeDef) -> TypeDefResponse:
-    if isinstance(typedef, ClassificationDef):
+    if isinstance(typedef, AtlanTagDef):
         # Set up the request payload...
         payload = TypeDefResponse(
-            classification_defs=[typedef],
+            atlan_tag_defs=[typedef],
             enum_defs=[],
             struct_defs=[],
             entity_defs=[],
             relationship_defs=[],
             custom_metadata_defs=[],
         )
     elif isinstance(typedef, CustomMetadataDef):
         # Set up the request payload...
         payload = TypeDefResponse(
-            classification_defs=[],
+            atlan_tag_defs=[],
             enum_defs=[],
             struct_defs=[],
             entity_defs=[],
             relationship_defs=[],
             custom_metadata_defs=[typedef],
         )
     elif isinstance(typedef, EnumDef):
         # Set up the request payload...
         payload = TypeDefResponse(
-            classification_defs=[],
+            atlan_tag_defs=[],
             enum_defs=[typedef],
             struct_defs=[],
             entity_defs=[],
             relationship_defs=[],
             custom_metadata_defs=[],
         )
     else:
@@ -203,18 +213,18 @@
             param="category",
         )
         # Throw an invalid request exception
     return payload
 
 
 def _refresh_caches(typedef: TypeDef) -> None:
-    if isinstance(typedef, ClassificationDef):
-        from pyatlan.cache.classification_cache import ClassificationCache
+    if isinstance(typedef, AtlanTagDef):
+        from pyatlan.cache.atlan_tag_cache import AtlanTagCache
 
-        ClassificationCache.refresh_cache()
+        AtlanTagCache.refresh_cache()
     if isinstance(typedef, CustomMetadataDef):
         from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
 
         CustomMetadataCache.refresh_cache()
     if isinstance(typedef, EnumDef):
         from pyatlan.cache.enum_cache import EnumCache
 
@@ -400,25 +410,23 @@
         self,
         limit: int,
         post_filter: Optional[str] = None,
         sort: Optional[str] = None,
         count: bool = True,
         offset: int = 0,
     ) -> RoleResponse:
-        if post_filter is None:
-            post_filter = ""
-        if sort is None:
-            sort = ""
-        query_params = {
-            "filter": post_filter,
-            "sort": sort,
-            "count": count,
-            "offset": offset,
-            "limit": limit,
+        query_params: dict[str, str] = {
+            "count": str(count),
+            "offset": str(offset),
+            "limit": str(limit),
         }
+        if post_filter:
+            query_params["filter"] = post_filter
+        if sort:
+            query_params["sort"] = sort
         raw_json = self._call_api(GET_ROLES.format_path_with_params(), query_params)
         return RoleResponse(**raw_json)
 
     def get_all_roles(self) -> RoleResponse:
         """
         Retrieve all roles defined in Atlan.
         """
@@ -770,20 +778,20 @@
             min_ext_info=True,
             ignore_relationships=True,
         )
 
     def upsert(
         self,
         entity: Union[Asset, list[Asset]],
-        replace_classifications: bool = False,
+        replace_atlan_tags: bool = False,
         replace_custom_metadata: bool = False,
         overwrite_custom_metadata: bool = False,
     ) -> AssetMutationResponse:
         query_params = {
-            "replaceClassifications": replace_classifications,
+            "replaceClassifications": replace_atlan_tags,
             "replaceBusinessAttributes": replace_custom_metadata,
             "overwriteBusinessAttributes": overwrite_custom_metadata,
         }
         entities: list[Asset] = []
         if isinstance(entity, list):
             entities.extend(entity)
         else:
@@ -791,18 +799,18 @@
         for asset in entities:
             asset.validate_required()
         request = BulkRequest[Asset](entities=entities)
         raw_json = self._call_api(BULK_UPDATE, query_params, request)
         return AssetMutationResponse(**raw_json)
 
     def upsert_merging_cm(
-        self, entity: Union[Asset, list[Asset]], replace_classifications: bool = False
+        self, entity: Union[Asset, list[Asset]], replace_atlan_tags: bool = False
     ) -> AssetMutationResponse:
         query_params = {
-            "replaceClassifications": replace_classifications,
+            "replaceClassifications": replace_atlan_tags,
             "replaceBusinessAttributes": True,
             "overwriteBusinessAttributes": False,
         }
         entities: list[Asset] = []
         if isinstance(entity, list):
             entities.extend(entity)
         else:
@@ -810,18 +818,18 @@
         for asset in entities:
             asset.validate_required()
         request = BulkRequest[Asset](entities=entities)
         raw_json = self._call_api(BULK_UPDATE, query_params, request)
         return AssetMutationResponse(**raw_json)
 
     def upsert_replacing_cm(
-        self, entity: Union[Asset, list[Asset]], replace_classifications: bool = False
+        self, entity: Union[Asset, list[Asset]], replace_atlan_tagss: bool = False
     ) -> AssetMutationResponse:
         query_params = {
-            "replaceClassifications": replace_classifications,
+            "replaceClassifications": replace_atlan_tagss,
             "replaceBusinessAttributes": True,
             "overwriteBusinessAttributes": True,
         }
         entities: list[Asset] = []
         if isinstance(entity, list):
             entities.extend(entity)
         else:
@@ -900,18 +908,18 @@
     def purge_typedef(self, name: str, typedef_type: type) -> None:
         if typedef_type == CustomMetadataDef:
             from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
 
             internal_name = CustomMetadataCache.get_id_for_name(name)
         elif typedef_type == EnumDef:
             internal_name = name
-        elif typedef_type == ClassificationDef:
-            from pyatlan.cache.classification_cache import ClassificationCache
+        elif typedef_type == AtlanTagDef:
+            from pyatlan.cache.atlan_tag_cache import AtlanTagCache
 
-            internal_name = str(ClassificationCache.get_id_for_name(name))
+            internal_name = str(AtlanTagCache.get_id_for_name(name))
         else:
             raise InvalidRequestException(
                 message=f"Unable to purge type definitions of type: {typedef_type}",
             )
             # Throw an invalid request exception
         if internal_name:
             self._call_api(
@@ -927,58 +935,58 @@
             from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
 
             CustomMetadataCache.refresh_cache()
         elif typedef_type == EnumDef:
             from pyatlan.cache.enum_cache import EnumCache
 
             EnumCache.refresh_cache()
-        elif typedef_type == ClassificationDef:
-            from pyatlan.cache.classification_cache import ClassificationCache
+        elif typedef_type == AtlanTagDef:
+            from pyatlan.cache.atlan_tag_cache import AtlanTagCache
 
-            ClassificationCache.refresh_cache()
+            AtlanTagCache.refresh_cache()
 
     @validate_arguments()
-    def add_classifications(
+    def add_atlan_tags(
         self,
         asset_type: Type[A],
         qualified_name: str,
-        classification_names: list[str],
+        atlan_tag_names: list[str],
         propagate: bool = True,
         remove_propagation_on_delete: bool = True,
         restrict_lineage_propagation: bool = True,
     ) -> None:
-        classifications = Classifications(
+        atlan_tags = AtlanTags(
             __root__=[
-                Classification(
-                    type_name=ClassificationName(display_text=name),
+                AtlanTag(
+                    type_name=AtlanTagName(display_text=name),
                     propagate=propagate,
                     remove_propagations_on_entity_delete=remove_propagation_on_delete,
                     restrict_propagation_through_lineage=restrict_lineage_propagation,
                 )
-                for name in classification_names
+                for name in atlan_tag_names
             ]
         )
         query_params = {"attr:qualifiedName": qualified_name}
         self._call_api(
             UPDATE_ENTITY_BY_ATTRIBUTE.format_path_with_params(
                 asset_type.__name__, "classifications"
             ),
             query_params,
-            classifications,
+            atlan_tags,
         )
 
     @validate_arguments()
-    def remove_classification(
-        self, asset_type: Type[A], qualified_name: str, classification_name: str
+    def remove_atlan_tag(
+        self, asset_type: Type[A], qualified_name: str, atlan_tag_name: str
     ) -> None:
-        from pyatlan.cache.classification_cache import ClassificationCache
+        from pyatlan.cache.atlan_tag_cache import AtlanTagCache
 
-        classification_id = ClassificationCache.get_id_for_name(classification_name)
+        classification_id = AtlanTagCache.get_id_for_name(atlan_tag_name)
         if not classification_id:
-            raise ValueError(f"{classification_name} is not a valid Classification")
+            raise ValueError(f"{atlan_tag_name} is not a valid AtlanTag")
         query_params = {"attr:qualifiedName": qualified_name}
         self._call_api(
             DELETE_ENTITY_BY_ATTRIBUTE.format_path_with_params(
                 asset_type.__name__, "classification", classification_id
             ),
             query_params,
         )
@@ -1256,15 +1264,14 @@
         search_request = IndexSearchRequest(
             dsl=dsl,
             attributes=attributes,
         )
         results = self.search(search_request)
         return [asset for asset in results if isinstance(asset, Persona)]
 
-    @validate_arguments()
     def find_purposes_by_name(
         self,
         name: str,
         attributes: Optional[list[str]] = None,
     ) -> list[Purpose]:
         if attributes is None:
             attributes = []
@@ -1276,7 +1283,115 @@
         dsl = DSL(query=query)
         search_request = IndexSearchRequest(
             dsl=dsl,
             attributes=attributes,
         )
         results = self.search(search_request)
         return [asset for asset in results if isinstance(asset, Purpose)]
+
+    @validate_arguments()
+    def find_glossary_by_name(
+        self,
+        name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+        attributes: Optional[list[StrictStr]] = None,
+    ) -> AtlasGlossary:
+        if attributes is None:
+            attributes = []
+        query = with_active_glossary(name=name)
+        return self._search_for_asset_with_name(
+            query=query, name=name, asset_type=AtlasGlossary, attributes=attributes
+        )
+
+    @validate_arguments()
+    def find_category_fast_by_name(
+        self,
+        name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+        glossary_qualified_name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+        attributes: Optional[list[StrictStr]] = None,
+    ) -> AtlasGlossaryCategory:
+        if attributes is None:
+            attributes = []
+        query = with_active_category(
+            name=name, glossary_qualified_name=glossary_qualified_name
+        )
+        return self._search_for_asset_with_name(
+            query=query,
+            name=name,
+            asset_type=AtlasGlossaryCategory,
+            attributes=attributes,
+        )
+
+    @validate_arguments()
+    def find_category_by_name(
+        self,
+        name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+        glossary_name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+        attributes: Optional[list[StrictStr]] = None,
+    ):
+        glossary = self.find_glossary_by_name(name=glossary_name)
+        return self.find_category_fast_by_name(
+            name=name,
+            glossary_qualified_name=glossary.qualified_name,
+            attributes=attributes,
+        )
+
+    def _search_for_asset_with_name(
+        self,
+        query: Query,
+        name: str,
+        asset_type: Type[A],
+        attributes: Optional[list[StrictStr]],
+    ) -> A:
+        dsl = DSL(query=query)
+        search_request = IndexSearchRequest(
+            dsl=dsl,
+            attributes=attributes,
+        )
+        results = self.search(search_request)
+        if results.count > 0 and (
+            assets := [
+                asset
+                for asset in results.current_page()
+                if isinstance(asset, asset_type)
+            ]
+        ):
+            if len(assets) > 1:
+                LOGGER.warning(
+                    "More than 1 %s found with the name '%s', returning only the first.",
+                    asset_type.__name__,
+                    name,
+                )
+            return assets[0]
+        raise NotFoundError(
+            f"The {asset_type.__name__} asset could not be found by name: {name}.",
+            "ATLAN-PYTHON-404-014",
+        )
+
+    @validate_arguments()
+    def find_term_fast_by_name(
+        self,
+        name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+        glossary_qualified_name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+        attributes: Optional[list[StrictStr]] = None,
+    ) -> AtlasGlossaryTerm:
+        if attributes is None:
+            attributes = []
+        query = with_active_term(
+            name=name, glossary_qualified_name=glossary_qualified_name
+        )
+        return self._search_for_asset_with_name(
+            query=query, name=name, asset_type=AtlasGlossaryTerm, attributes=attributes
+        )
+
+    @validate_arguments()
+    def find_term_by_name(
+        self,
+        name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+        glossary_name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+        attributes: Optional[list[StrictStr]] = None,
+    ):
+        glossary = self.find_glossary_by_name(name=glossary_name)
+        return self.find_term_fast_by_name(
+            name=name,
+            glossary_qualified_name=glossary.qualified_name,
+            attributes=attributes,
+        )
```

### Comparing `pyatlan-0.1.3/pyatlan/client/constants.py` & `pyatlan-0.2.0/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/error.py` & `pyatlan-0.2.0/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/exceptions.py` & `pyatlan-0.2.0/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.2.0/pyatlan/generator/generate_from_typdefs.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,19 @@
         self.add_entity_def(entity_defs, name)
         while True:
             self.add_children(i, entity_defs)
             i = i + 1
             if i >= len(entity_defs):
                 break
         content = self.template.render(
-            {"struct_defs": self.type_defs.struct_defs, "entity_defs": entity_defs}
+            {
+                "struct_defs": self.type_defs.struct_defs,
+                "entity_defs": entity_defs,
+                "existz": os.path.exists,
+            }
         )
         with (PARENT.parent / "model" / "assets.py").open("w") as script:
             script.write(content)
         content = self.structs.render({"struct_defs": self.type_defs.struct_defs})
         with (PARENT.parent / "model" / "structs.py").open("w") as script:
             script.write(content)
```

### Comparing `pyatlan-0.1.3/pyatlan/model/assets.py` & `pyatlan-0.2.0/pyatlan/model/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 # Based on original code from https://github.com/apache/atlas (under Apache-2.0 license)
+
 from __future__ import annotations
 
 import hashlib
 import sys
 from datetime import datetime
 from io import StringIO
 from typing import Any, ClassVar, Dict, List, Optional, Set, Type, TypeVar
 from urllib.parse import quote, unquote
 
 from pydantic import Field, PrivateAttr, StrictStr, root_validator, validator
 
-from pyatlan.model.core import Announcement, AtlanObject, Classification, Meaning
+from pyatlan.model.core import Announcement, AtlanObject, AtlanTag, Meaning
 from pyatlan.model.custom_metadata import CustomMetadataDict, CustomMetadataProxy
 from pyatlan.model.enums import (
     ADLSAccessTier,
     ADLSAccountStatus,
     ADLSEncryptionTypes,
     ADLSLeaseState,
     ADLSLeaseStatus,
@@ -96,14 +97,27 @@
             __pydantic_self__.business_attributes
         )
 
     def json(self, *args, **kwargs) -> str:
         self.business_attributes = self._metadata_proxy.business_attributes
         return super().json(**kwargs)
 
+    def validate_required(self):
+        if not self.create_time or self.created_by:
+            self.attributes.validate_required()
+
+    def get_custom_metadata(self, name: str) -> CustomMetadataDict:
+        return self._metadata_proxy.get_custom_metadata(name=name)
+
+    def set_custom_metadata(self, custom_metadata: CustomMetadataDict):
+        return self._metadata_proxy.set_custom_metadata(custom_metadata=custom_metadata)
+
+    def flush_custom_metadata(self):
+        self.business_attributes = self._metadata_proxy.business_attributes
+
     def __setattr__(self, name, value):
         if name in Referenceable._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qualified_name",
@@ -220,16 +234,16 @@
         None,
         description="Time (epoch) at which this object was last assets_updated, in milliseconds.\n",
         example=1649172284333,
     )
     version: Optional[int] = Field(
         None, description="Version of this object.\n", example=2
     )
-    classifications: Optional[list[Classification]] = Field(
-        None, description="classifications"
+    atlan_tags: Optional[list[AtlanTag]] = Field(
+        None, description="Atlan tags", alias="classifications"
     )
     classification_names: Optional[list[str]] = Field(
         None, description="The names of the classifications that exist on the asset."
     )
     display_text: Optional[str] = Field(
         None,
         description="Human-readable name of the entity..\n",
@@ -260,30 +274,133 @@
     scrubbed: Optional[bool] = Field(
         None, description="", alias="fields removed from results"
     )
     pending_tasks: Optional[list[str]] = Field(None)
 
     unique_attributes: Optional[dict[str, Any]] = Field(None)
 
-    def validate_required(self):
-        if not self.create_time or self.created_by:
-            self.attributes.validate_required()
 
-    def get_custom_metadata(self, name: str) -> CustomMetadataDict:
-        return self._metadata_proxy.get_custom_metadata(name=name)
+class Asset(Referenceable):
+    """Description"""
 
-    def set_custom_metadata(self, custom_metadata: CustomMetadataDict):
-        return self._metadata_proxy.set_custom_metadata(custom_metadata=custom_metadata)
+    _subtypes_: dict[str, type] = dict()
 
-    def flush_custom_metadata(self):
-        self.business_attributes = self._metadata_proxy.business_attributes
+    def __init_subclass__(cls, type_name=None):
+        cls._subtypes_[type_name or cls.__name__.lower()] = cls
 
+    def trim_to_required(self: SelfAsset) -> SelfAsset:
+        return self.create_for_modification(
+            qualified_name=self.qualified_name, name=self.name
+        )
 
-class Asset(Referenceable):
-    """Description"""
+    @classmethod
+    def create(cls: Type[SelfAsset], *args, **kwargs) -> SelfAsset:
+        raise NotImplementedError(
+            "Create has not been implemented for this class. Please submit an enhancement"
+            "request if you need it implemented."
+        )
+
+    @classmethod
+    def create_for_modification(
+        cls: type[SelfAsset], qualified_name: str = "", name: str = ""
+    ) -> SelfAsset:
+        validate_required_fields(
+            ["name", "qualified_name"],
+            [name, qualified_name],
+        )
+        return cls(attributes=cls.Attributes(qualified_name=qualified_name, name=name))
+
+    @classmethod
+    def ref_by_guid(cls: type[SelfAsset], guid: str) -> SelfAsset:
+        retval: SelfAsset = cls(attributes=cls.Attributes())
+        retval.guid = guid
+        return retval
+
+    @classmethod
+    def ref_by_qualified_name(cls: type[SelfAsset], qualified_name: str) -> SelfAsset:
+        ret_value: SelfAsset = cls(
+            attributes=cls.Attributes(qualified_name=qualified_name)
+        )
+        ret_value.unique_attributes = {"qualifiedName": qualified_name}
+        return ret_value
+
+    @classmethod
+    def __get_validators__(cls):
+        yield cls._convert_to_real_type_
+
+    @classmethod
+    def _convert_to_real_type_(cls, data):
+
+        if isinstance(data, Asset):
+            return data
+
+        data_type = (
+            data.get("type_name") if "type_name" in data else data.get("typeName")
+        )
+
+        if data_type is None:
+            if issubclass(cls, Asset):
+                return cls(**data)
+            raise ValueError("Missing 'type' in Asset")
+
+        sub = cls._subtypes_.get(data_type)
+        if sub is None:
+            sub = getattr(sys.modules[__name__], data_type)
+
+        if sub is None:
+            raise TypeError(f"Unsupport sub-type: {data_type}")
+
+        return sub(**data)
+
+    def has_announcement(self) -> bool:
+        return bool(
+            self.attributes
+            and (
+                self.attributes.announcement_title or self.attributes.announcement_type
+            )
+        )
+
+    def set_announcement(self, announcement: Announcement) -> None:
+        self.attributes.announcement_type = announcement.announcement_type.value
+        self.attributes.announcement_title = announcement.announcement_title
+        self.attributes.announcement_message = announcement.announcement_message
+
+    def get_announcment(self) -> Optional[Announcement]:
+        if self.attributes.announcement_type and self.attributes.announcement_title:
+            return Announcement(
+                announcement_type=AnnouncementType[
+                    self.attributes.announcement_type.upper()
+                ],
+                announcement_title=self.attributes.announcement_title,
+                announcement_message=self.attributes.announcement_message,
+            )
+        return None
+
+    def remove_announcement(self):
+        self.attributes.remove_announcement()
+
+    def remove_description(self):
+        self.attributes.remove_description()
+
+    def remove_user_description(self):
+        self.attributes.remove_user_description()
+
+    def remove_owners(self):
+        self.attributes.remove_owners()
+
+    def remove_certificate(self):
+        self.attributes.remove_certificate()
+
+    type_name: str = Field("Asset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Asset":
+            raise ValueError("must be Asset")
+        return v
 
     def __setattr__(self, name, value):
         if name in Asset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
@@ -1950,91 +2067,14 @@
 
     @assigned_terms.setter
     def assigned_terms(self, assigned_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.meanings = assigned_terms
 
-    _subtypes_: dict[str, type] = dict()
-
-    def __init_subclass__(cls, type_name=None):
-        cls._subtypes_[type_name or cls.__name__.lower()] = cls
-
-    def trim_to_required(self: SelfAsset) -> SelfAsset:
-        return self.create_for_modification(
-            qualified_name=self.qualified_name, name=self.name
-        )
-
-    @classmethod
-    def create(cls: Type[SelfAsset], *args, **kwargs) -> SelfAsset:
-        raise NotImplementedError(
-            "Create has not been implemented for this class. Please submit an enhancement"
-            "request if you need it implemented."
-        )
-
-    @classmethod
-    def create_for_modification(
-        cls: type[SelfAsset], qualified_name: str = "", name: str = ""
-    ) -> SelfAsset:
-        validate_required_fields(
-            ["name", "qualified_name"],
-            [name, qualified_name],
-        )
-        return cls(attributes=cls.Attributes(qualified_name=qualified_name, name=name))
-
-    @classmethod
-    def ref_by_guid(cls: type[SelfAsset], guid: str) -> SelfAsset:
-        retval: SelfAsset = cls(attributes=cls.Attributes())
-        retval.guid = guid
-        return retval
-
-    @classmethod
-    def ref_by_qualified_name(cls: type[SelfAsset], qualified_name: str) -> SelfAsset:
-        ret_value: SelfAsset = cls(
-            attributes=cls.Attributes(qualified_name=qualified_name)
-        )
-        ret_value.unique_attributes = {"qualifiedName": qualified_name}
-        return ret_value
-
-    @classmethod
-    def __get_validators__(cls):
-        yield cls._convert_to_real_type_
-
-    @classmethod
-    def _convert_to_real_type_(cls, data):
-
-        if isinstance(data, Asset):
-            return data
-
-        data_type = (
-            data.get("type_name") if "type_name" in data else data.get("typeName")
-        )
-
-        if data_type is None:
-            if issubclass(cls, Asset):
-                return cls(**data)
-            raise ValueError("Missing 'type' in Asset")
-
-        sub = cls._subtypes_.get(data_type)
-        if sub is None:
-            sub = getattr(sys.modules[__name__], data_type)
-
-        if sub is None:
-            raise TypeError(f"Unsupport sub-type: {data_type}")
-
-        return sub(**data)
-
-    type_name: str = Field("Asset", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Asset":
-            raise ValueError("must be Asset")
-        return v
-
     class Attributes(Referenceable.Attributes):
         name: str = Field(None, description="", alias="name")
         display_name: Optional[str] = Field(None, description="", alias="displayName")
         description: Optional[str] = Field(None, description="", alias="description")
         user_description: Optional[str] = Field(
             None, description="", alias="userDescription"
         )
@@ -2382,76 +2422,96 @@
 
     attributes: "Asset.Attributes" = Field(
         default_factory=lambda: Asset.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
-    def has_announcement(self) -> bool:
-        return bool(
-            self.attributes
-            and (
-                self.attributes.announcement_title or self.attributes.announcement_type
-            )
-        )
 
-    def set_announcement(self, announcement: Announcement) -> None:
-        self.attributes.announcement_type = announcement.announcement_type.value
-        self.attributes.announcement_title = announcement.announcement_title
-        self.attributes.announcement_message = announcement.announcement_message
+class DataSet(Asset, type_name="DataSet"):
+    """Description"""
 
-    def get_announcment(self) -> Optional[Announcement]:
-        if self.attributes.announcement_type and self.attributes.announcement_title:
-            return Announcement(
-                announcement_type=AnnouncementType[
-                    self.attributes.announcement_type.upper()
-                ],
-                announcement_title=self.attributes.announcement_title,
-                announcement_message=self.attributes.announcement_message,
-            )
-        return None
+    type_name: str = Field("DataSet", allow_mutation=False)
 
-    def remove_announcement(self):
-        self.attributes.remove_announcement()
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "DataSet":
+            raise ValueError("must be DataSet")
+        return v
 
-    def remove_description(self):
-        self.attributes.remove_description()
+    def __setattr__(self, name, value):
+        if name in DataSet._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
 
-    def remove_user_description(self):
-        self.attributes.remove_user_description()
+    _convience_properties: ClassVar[list[str]] = []
 
-    def remove_owners(self):
-        self.attributes.remove_owners()
 
-    def remove_certificate(self):
-        self.attributes.remove_certificate()
+class Connection(Asset, type_name="Connection"):
+    """Description"""
 
+    @classmethod
+    # @validate_arguments()
+    def create(
+        cls,
+        *,
+        name: str,
+        connector_type: AtlanConnectorType,
+        admin_users: Optional[list[str]] = None,
+        admin_groups: Optional[list[str]] = None,
+        admin_roles: Optional[list[str]] = None,
+    ) -> Connection:
+        validate_required_fields(["name", "connector_type"], [name, connector_type])
+        if not admin_users and not admin_groups and not admin_roles:
+            raise ValueError(
+                "One of admin_user, admin_groups or admin_roles is required"
+            )
+        if admin_roles:
+            from pyatlan.cache.role_cache import RoleCache
 
-class DataSet(Asset, type_name="DataSet"):
-    """Description"""
+            for role_id in admin_roles:
+                if not RoleCache.get_name_for_id(role_id):
+                    raise ValueError(
+                        f"Provided role ID {role_id} was not found in Atlan."
+                    )
+        if admin_groups:
+            from pyatlan.cache.group_cache import GroupCache
 
-    def __setattr__(self, name, value):
-        if name in DataSet._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
+            for group_alias in admin_groups:
+                if not GroupCache.get_id_for_alias(group_alias):
+                    raise ValueError(
+                        f"Provided group name {group_alias} was not found in Atlan."
+                    )
+        if admin_users:
+            from pyatlan.cache.user_cache import UserCache
 
-    _convience_properties: ClassVar[list[str]] = []
+            for username in admin_users:
+                if not UserCache.get_id_for_name(username):
+                    raise ValueError(
+                        f"Provided username {username} was not found in Atlan."
+                    )
+        attr = cls.Attributes(
+            name=name,
+            qualified_name=connector_type.to_qualified_name(),
+            connector_name=connector_type.value,
+            category=connector_type.category.value,
+            admin_users=admin_users or [],
+            admin_groups=admin_groups or [],
+            admin_roles=admin_roles or [],
+        )
+        return cls(attributes=attr)
 
-    type_name: str = Field("DataSet", allow_mutation=False)
+    type_name: str = Field("Connection", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "DataSet":
-            raise ValueError("must be DataSet")
+        if v != "Connection":
+            raise ValueError("must be Connection")
         return v
 
-
-class Connection(Asset, type_name="Connection"):
-    """Description"""
-
     def __setattr__(self, name, value):
         if name in Connection._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "category",
@@ -2463,15 +2523,14 @@
         "query_preview_config",
         "query_config",
         "credential_strategy",
         "preview_credential_strategy",
         "policy_strategy",
         "query_username_strategy",
         "row_limit",
-        "query_timeout",
         "default_credential_guid",
         "connector_icon",
         "connector_image",
         "source_logo",
         "is_sample_data_preview_enabled",
         "popularity_insights_timeframe",
         "has_popularity_insights",
@@ -2614,24 +2673,14 @@
     @row_limit.setter
     def row_limit(self, row_limit: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.row_limit = row_limit
 
     @property
-    def query_timeout(self) -> Optional[int]:
-        return None if self.attributes is None else self.attributes.query_timeout
-
-    @query_timeout.setter
-    def query_timeout(self, query_timeout: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.query_timeout = query_timeout
-
-    @property
     def default_credential_guid(self) -> Optional[str]:
         return (
             None if self.attributes is None else self.attributes.default_credential_guid
         )
 
     @default_credential_guid.setter
     def default_credential_guid(self, default_credential_guid: Optional[str]):
@@ -2743,22 +2792,14 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.connection_s_s_o_credential_guid = (
             connection_s_s_o_credential_guid
         )
 
-    type_name: str = Field("Connection", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Connection":
-            raise ValueError("must be Connection")
-        return v
-
     class Attributes(Asset.Attributes):
         category: Optional[str] = Field(None, description="", alias="category")
         sub_category: Optional[str] = Field(None, description="", alias="subCategory")
         host: Optional[str] = Field(None, description="", alias="host")
         port: Optional[int] = Field(None, description="", alias="port")
         allow_query: Optional[bool] = Field(None, description="", alias="allowQuery")
         allow_query_preview: Optional[bool] = Field(
@@ -2777,15 +2818,14 @@
         policy_strategy: Optional[str] = Field(
             None, description="", alias="policyStrategy"
         )
         query_username_strategy: Optional[QueryUsernameStrategy] = Field(
             None, description="", alias="queryUsernameStrategy"
         )
         row_limit: Optional[int] = Field(None, description="", alias="rowLimit")
-        query_timeout: Optional[int] = Field(None, description="", alias="queryTimeout")
         default_credential_guid: Optional[str] = Field(
             None, description="", alias="defaultCredentialGuid"
         )
         connector_icon: Optional[str] = Field(
             None, description="", alias="connectorIcon"
         )
         connector_image: Optional[str] = Field(
@@ -2810,70 +2850,46 @@
 
     attributes: "Connection.Attributes" = Field(
         default_factory=lambda: Connection.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+
+class Process(Asset, type_name="Process"):
+    """Description"""
+
     @classmethod
-    # @validate_arguments()
     def create(
         cls,
-        *,
         name: str,
-        connector_type: AtlanConnectorType,
-        admin_users: Optional[list[str]] = None,
-        admin_groups: Optional[list[str]] = None,
-        admin_roles: Optional[list[str]] = None,
-    ) -> Connection:
-        if not name:
-            raise ValueError("name cannot be blank")
-        validate_required_fields(["connector_type"], [connector_type])
-        if not admin_users and not admin_groups and not admin_roles:
-            raise ValueError(
-                "One of admin_user, admin_groups or admin_roles is required"
+        connection_qualified_name: str,
+        inputs: list["Catalog"],
+        outputs: list["Catalog"],
+        process_id: Optional[str] = None,
+        parent: Optional[Process] = None,
+    ) -> Process:
+        return Process(
+            attributes=Process.Attributes.create(
+                name=name,
+                connection_qualified_name=connection_qualified_name,
+                process_id=process_id,
+                inputs=inputs,
+                outputs=outputs,
+                parent=parent,
             )
-        if admin_roles:
-            from pyatlan.cache.role_cache import RoleCache
-
-            for role_id in admin_roles:
-                if not RoleCache.get_name_for_id(role_id):
-                    raise ValueError(
-                        f"Provided role ID {role_id} was not found in Atlan."
-                    )
-        if admin_groups:
-            from pyatlan.cache.group_cache import GroupCache
-
-            for group_alias in admin_groups:
-                if not GroupCache.get_id_for_alias(group_alias):
-                    raise ValueError(
-                        f"Provided group name {group_alias} was not found in Atlan."
-                    )
-        if admin_users:
-            from pyatlan.cache.user_cache import UserCache
-
-            for username in admin_users:
-                if not UserCache.get_id_for_name(username):
-                    raise ValueError(
-                        f"Provided username {username} was not found in Atlan."
-                    )
-        attr = cls.Attributes(
-            name=name,
-            qualified_name=connector_type.to_qualified_name(),
-            connector_name=connector_type.value,
-            category=connector_type.category.value,
-            admin_users=admin_users or [],
-            admin_groups=admin_groups or [],
-            admin_roles=admin_roles or [],
         )
-        return cls(attributes=attr)
 
+    type_name: str = Field("Process", allow_mutation=False)
 
-class Process(Asset, type_name="Process"):
-    """Description"""
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Process":
+            raise ValueError("must be Process")
+        return v
 
     def __setattr__(self, name, value):
         if name in Process._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
@@ -2941,22 +2957,14 @@
 
     @column_processes.setter
     def column_processes(self, column_processes: Optional[list[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_processes = column_processes
 
-    type_name: str = Field("Process", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Process":
-            raise ValueError("must be Process")
-        return v
-
     class Attributes(Asset.Attributes):
         inputs: Optional[list[Catalog]] = Field(None, description="", alias="inputs")
         outputs: Optional[list[Catalog]] = Field(None, description="", alias="outputs")
         code: Optional[str] = Field(None, description="", alias="code")
         sql: Optional[str] = Field(None, description="", alias="sql")
         ast: Optional[str] = Field(None, description="", alias="ast")
         column_processes: Optional[list[ColumnProcess]] = Field(
@@ -3029,38 +3037,79 @@
 
     attributes: "Process.Attributes" = Field(
         default_factory=lambda: Process.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+
+class AtlasGlossaryCategory(Asset, type_name="AtlasGlossaryCategory"):
+    """Description"""
+
+    @root_validator()
+    def _set_qualified_name_fallback(cls, values):
+        if (
+            "attributes" in values
+            and values["attributes"]
+            and not values["attributes"].qualified_name
+        ):
+            values["attributes"].qualified_name = values["guid"]
+        return values
+
     @classmethod
+    # @validate_arguments()
     def create(
         cls,
-        name: str,
-        connection_qualified_name: str,
-        inputs: list["Catalog"],
-        outputs: list["Catalog"],
-        process_id: Optional[str] = None,
-        parent: Optional[Process] = None,
-    ) -> Process:
-        return Process(
-            attributes=Process.Attributes.create(
-                name=name,
-                connection_qualified_name=connection_qualified_name,
-                process_id=process_id,
-                inputs=inputs,
-                outputs=outputs,
-                parent=parent,
+        *,
+        name: StrictStr,
+        anchor: AtlasGlossary,
+        parent_category: Optional[AtlasGlossaryCategory] = None,
+    ) -> AtlasGlossaryCategory:
+        validate_required_fields(["name", "anchor"], [name, anchor])
+        return cls(
+            attributes=AtlasGlossaryCategory.Attributes.create(
+                name=name, anchor=anchor, parent_category=parent_category
             )
         )
 
+    def trim_to_required(self) -> AtlasGlossaryCategory:
+        if self.anchor is None or not self.anchor.guid:
+            raise ValueError("anchor.guid must be available")
+        return self.create_for_modification(
+            qualified_name=self.qualified_name,
+            name=self.name,
+            glossary_guid=self.anchor.guid,
+        )
 
-class AtlasGlossaryCategory(Asset, type_name="AtlasGlossaryCategory"):
-    """Description"""
+    @classmethod
+    def create_for_modification(
+        cls: type[SelfAsset],
+        qualified_name: str = "",
+        name: str = "",
+        glossary_guid: str = "",
+    ) -> SelfAsset:
+        validate_required_fields(
+            ["name", "qualified_name", "glossary_guid"],
+            [name, qualified_name, glossary_guid],
+        )
+        glossary = AtlasGlossary()
+        glossary.guid = glossary_guid
+        return cls(
+            attributes=cls.Attributes(
+                qualified_name=qualified_name, name=name, anchor=glossary
+            )
+        )
+
+    type_name: str = Field("AtlasGlossaryCategory", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "AtlasGlossaryCategory":
+            raise ValueError("must be AtlasGlossaryCategory")
+        return v
 
     def __setattr__(self, name, value):
         if name in AtlasGlossaryCategory._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
@@ -3143,22 +3192,14 @@
     def children_categories(
         self, children_categories: Optional[list[AtlasGlossaryCategory]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.children_categories = children_categories
 
-    type_name: str = Field("AtlasGlossaryCategory", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "AtlasGlossaryCategory":
-            raise ValueError("must be AtlasGlossaryCategory")
-        return v
-
     class Attributes(Asset.Attributes):
         short_description: Optional[str] = Field(
             None, description="", alias="shortDescription"
         )
         long_description: Optional[str] = Field(
             None, description="", alias="longDescription"
         )
@@ -3197,71 +3238,45 @@
 
     attributes: "AtlasGlossaryCategory.Attributes" = Field(
         default_factory=lambda: AtlasGlossaryCategory.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
-    @root_validator()
-    def update_qualified_name(cls, values):
-        if (
-            "attributes" in values
-            and values["attributes"]
-            and not values["attributes"].qualified_name
-        ):
-            values["attributes"].qualified_name = values["guid"]
-        return values
+
+class Badge(Asset, type_name="Badge"):
+    """Description"""
 
     @classmethod
     # @validate_arguments()
     def create(
         cls,
         *,
         name: StrictStr,
-        anchor: AtlasGlossary,
-        parent_category: Optional[AtlasGlossaryCategory] = None,
-    ) -> AtlasGlossaryCategory:
-        validate_required_fields(["name", "anchor"], [name, anchor])
-        return cls(
-            attributes=AtlasGlossaryCategory.Attributes.create(
-                name=name, anchor=anchor, parent_category=parent_category
-            )
-        )
-
-    def trim_to_required(self) -> AtlasGlossaryCategory:
-        if self.anchor is None or not self.anchor.guid:
-            raise ValueError("anchor.guid must be available")
-        return self.create_for_modification(
-            qualified_name=self.qualified_name,
-            name=self.name,
-            glossary_guid=self.anchor.guid,
-        )
-
-    @classmethod
-    def create_for_modification(
-        cls: type[SelfAsset],
-        qualified_name: str = "",
-        name: str = "",
-        glossary_guid: str = "",
-    ) -> SelfAsset:
-        validate_required_fields(
-            ["name", "qualified_name", "glossary_guid"],
-            [name, qualified_name, glossary_guid],
-        )
-        glossary = AtlasGlossary()
-        glossary.guid = glossary_guid
+        cm_name: str,
+        cm_attribute: str,
+        badge_conditions: list[BadgeCondition],
+    ) -> Badge:
         return cls(
-            attributes=cls.Attributes(
-                qualified_name=qualified_name, name=name, anchor=glossary
-            )
+            status=EntityStatus.ACTIVE,
+            attributes=Badge.Attributes.create(
+                name=name,
+                cm_name=cm_name,
+                cm_attribute=cm_attribute,
+                badge_conditions=badge_conditions,
+            ),
         )
 
+    type_name: str = Field("Badge", allow_mutation=False)
 
-class Badge(Asset, type_name="Badge"):
-    """Description"""
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Badge":
+            raise ValueError("must be Badge")
+        return v
 
     def __setattr__(self, name, value):
         if name in Badge._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
@@ -3289,42 +3304,14 @@
 
     @badge_metadata_attribute.setter
     def badge_metadata_attribute(self, badge_metadata_attribute: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.badge_metadata_attribute = badge_metadata_attribute
 
-    type_name: str = Field("Badge", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Badge":
-            raise ValueError("must be Badge")
-        return v
-
-    @classmethod
-    # @validate_arguments()
-    def create(
-        cls,
-        *,
-        name: StrictStr,
-        cm_name: str,
-        cm_attribute: str,
-        badge_conditions: list[BadgeCondition],
-    ) -> Badge:
-        return cls(
-            status=EntityStatus.ACTIVE,
-            attributes=Badge.Attributes.create(
-                name=name,
-                cm_name=cm_name,
-                cm_attribute=cm_attribute,
-                badge_conditions=badge_conditions,
-            ),
-        )
-
     class Attributes(Asset.Attributes):
         badge_conditions: Optional[list[BadgeCondition]] = Field(
             None, description="", alias="badgeConditions"
         )
         badge_metadata_attribute: Optional[str] = Field(
             None, description="", alias="badgeMetadataAttribute"
         )
@@ -3362,14 +3349,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class AccessControl(Asset, type_name="AccessControl"):
     """Description"""
 
+    type_name: str = Field("AccessControl", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "AccessControl":
+            raise ValueError("must be AccessControl")
+        return v
+
     def __setattr__(self, name, value):
         if name in AccessControl._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "is_access_control_enabled",
@@ -3435,22 +3430,14 @@
 
     @policies.setter
     def policies(self, policies: Optional[list[AuthPolicy]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policies = policies
 
-    type_name: str = Field("AccessControl", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "AccessControl":
-            raise ValueError("must be AccessControl")
-        return v
-
     class Attributes(Asset.Attributes):
         is_access_control_enabled: Optional[bool] = Field(
             None, description="", alias="isAccessControlEnabled"
         )
         deny_custom_metadata_guids: Optional[set[str]] = Field(
             None, description="", alias="denyCustomMetadataGuids"
         )
@@ -3468,14 +3455,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Namespace(Asset, type_name="Namespace"):
     """Description"""
 
+    type_name: str = Field("Namespace", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Namespace":
+            raise ValueError("must be Namespace")
+        return v
+
     def __setattr__(self, name, value):
         if name in Namespace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "children_queries",
@@ -3498,22 +3493,14 @@
 
     @children_folders.setter
     def children_folders(self, children_folders: Optional[list[Folder]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.children_folders = children_folders
 
-    type_name: str = Field("Namespace", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Namespace":
-            raise ValueError("must be Namespace")
-        return v
-
     class Attributes(Asset.Attributes):
         children_queries: Optional[list[Query]] = Field(
             None, description="", alias="childrenQueries"
         )  # relationship
         children_folders: Optional[list[Folder]] = Field(
             None, description="", alias="childrenFolders"
         )  # relationship
@@ -3524,14 +3511,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Catalog(Asset, type_name="Catalog"):
     """Description"""
 
+    type_name: str = Field("Catalog", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Catalog":
+            raise ValueError("must be Catalog")
+        return v
+
     def __setattr__(self, name, value):
         if name in Catalog._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "input_to_processes",
@@ -3556,22 +3551,14 @@
 
     @output_from_processes.setter
     def output_from_processes(self, output_from_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_from_processes = output_from_processes
 
-    type_name: str = Field("Catalog", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Catalog":
-            raise ValueError("must be Catalog")
-        return v
-
     class Attributes(Asset.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
@@ -3582,14 +3569,38 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class AtlasGlossary(Asset, type_name="AtlasGlossary"):
     """Description"""
 
+    @root_validator()
+    def _set_qualified_name_fallback(cls, values):
+        if (
+            "attributes" in values
+            and values["attributes"]
+            and not values["attributes"].qualified_name
+        ):
+            values["attributes"].qualified_name = values["guid"]
+        return values
+
+    @classmethod
+    # @validate_arguments()
+    def create(cls, *, name: StrictStr) -> AtlasGlossary:
+        validate_required_fields(["name"], [name])
+        return AtlasGlossary(attributes=AtlasGlossary.Attributes.create(name=name))
+
+    type_name: str = Field("AtlasGlossary", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "AtlasGlossary":
+            raise ValueError("must be AtlasGlossary")
+        return v
+
     def __setattr__(self, name, value):
         if name in AtlasGlossary._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "short_description",
@@ -3669,22 +3680,14 @@
 
     @categories.setter
     def categories(self, categories: Optional[list[AtlasGlossaryCategory]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.categories = categories
 
-    type_name: str = Field("AtlasGlossary", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "AtlasGlossary":
-            raise ValueError("must be AtlasGlossary")
-        return v
-
     class Attributes(Asset.Attributes):
         short_description: Optional[str] = Field(
             None, description="", alias="shortDescription"
         )
         long_description: Optional[str] = Field(
             None, description="", alias="longDescription"
         )
@@ -3708,33 +3711,32 @@
 
     attributes: "AtlasGlossary.Attributes" = Field(
         default_factory=lambda: AtlasGlossary.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
-    @root_validator()
-    def update_qualified_name(cls, values):
-        if (
-            "attributes" in values
-            and values["attributes"]
-            and not values["attributes"].qualified_name
-        ):
-            values["attributes"].qualified_name = values["guid"]
-        return values
+
+class AuthPolicy(Asset, type_name="AuthPolicy"):
+    """Description"""
 
     @classmethod
     # @validate_arguments()
-    def create(cls, *, name: StrictStr) -> AtlasGlossary:
+    def __create(cls, *, name: str) -> AuthPolicy:
         validate_required_fields(["name"], [name])
-        return AtlasGlossary(attributes=AtlasGlossary.Attributes.create(name=name))
+        attributes = AuthPolicy.Attributes._Attributes__create(name=name)  # type: ignore
+        return cls(attributes=attributes)
 
+    type_name: str = Field("AuthPolicy", allow_mutation=False)
 
-class AuthPolicy(Asset, type_name="AuthPolicy"):
-    """Description"""
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "AuthPolicy":
+            raise ValueError("must be AuthPolicy")
+        return v
 
     def __setattr__(self, name, value):
         if name in AuthPolicy._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
@@ -3950,22 +3952,14 @@
 
     @access_control.setter
     def access_control(self, access_control: Optional[AccessControl]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.access_control = access_control
 
-    type_name: str = Field("AuthPolicy", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "AuthPolicy":
-            raise ValueError("must be AuthPolicy")
-        return v
-
     class Attributes(Asset.Attributes):
         policy_type: Optional[AuthPolicyType] = Field(
             None, description="", alias="policyType"
         )
         policy_service_name: Optional[str] = Field(
             None, description="", alias="policyServiceName"
         )
@@ -4016,58 +4010,117 @@
         )
         access_control: Optional[AccessControl] = Field(
             None, description="", alias="accessControl"
         )  # relationship
 
         @classmethod
         # @validate_arguments()
-        def create(cls, name: str) -> AuthPolicy.Attributes:
-            if not name:
-                raise ValueError("name cannot be blank")
+        def __create(cls, name: str) -> AuthPolicy.Attributes:
             validate_required_fields(["name"], [name])
             return AuthPolicy.Attributes(
                 qualified_name=name, name=name, display_name=""
             )
 
     attributes: "AuthPolicy.Attributes" = Field(
         default_factory=lambda: AuthPolicy.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
-    @classmethod
-    # @validate_arguments()
-    def create(cls, *, name: str) -> AuthPolicy:
-        validate_required_fields(["name"], [name])
-        attributes = AuthPolicy.Attributes.create(name=name)
-        return cls(attributes=attributes)
-
 
 class ProcessExecution(Asset, type_name="ProcessExecution"):
     """Description"""
 
-    def __setattr__(self, name, value):
-        if name in ProcessExecution._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
     type_name: str = Field("ProcessExecution", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ProcessExecution":
             raise ValueError("must be ProcessExecution")
         return v
 
+    def __setattr__(self, name, value):
+        if name in ProcessExecution._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
 
 class AtlasGlossaryTerm(Asset, type_name="AtlasGlossaryTerm"):
     """Description"""
 
+    @root_validator()
+    def _set_qualified_name_fallback(cls, values):
+        if (
+            "attributes" in values
+            and values["attributes"]
+            and not values["attributes"].qualified_name
+        ):
+            values["attributes"].qualified_name = values["guid"]
+        return values
+
+    @classmethod
+    # @validate_arguments()
+    def create(
+        cls,
+        *,
+        name: StrictStr,
+        anchor: Optional[AtlasGlossary] = None,
+        glossary_qualified_name: Optional[StrictStr] = None,
+        glossary_guid: Optional[StrictStr] = None,
+        categories: Optional[list[AtlasGlossaryCategory]] = None,
+    ) -> AtlasGlossaryTerm:
+        validate_required_fields(["name"], [name])
+        return cls(
+            attributes=AtlasGlossaryTerm.Attributes.create(
+                name=name,
+                anchor=anchor,
+                glossary_qualified_name=glossary_qualified_name,
+                glossary_guid=glossary_guid,
+                categories=categories,
+            )
+        )
+
+    def trim_to_required(self) -> AtlasGlossaryTerm:
+        if self.anchor is None or not self.anchor.guid:
+            raise ValueError("anchor.guid must be available")
+        return self.create_for_modification(
+            qualified_name=self.qualified_name,
+            name=self.name,
+            glossary_guid=self.anchor.guid,
+        )
+
+    @classmethod
+    def create_for_modification(
+        cls: type[SelfAsset],
+        qualified_name: str = "",
+        name: str = "",
+        glossary_guid: str = "",
+    ) -> SelfAsset:
+        validate_required_fields(
+            ["name", "qualified_name", "glossary_guid"],
+            [name, qualified_name, glossary_guid],
+        )
+        glossary = AtlasGlossary()
+        glossary.guid = glossary_guid
+        return cls(
+            attributes=cls.Attributes(
+                qualified_name=qualified_name, name=name, anchor=glossary
+            )
+        )
+
+    type_name: str = Field("AtlasGlossaryTerm", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "AtlasGlossaryTerm":
+            raise ValueError("must be AtlasGlossaryTerm")
+        return v
+
     def __setattr__(self, name, value):
         if name in AtlasGlossaryTerm._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "short_description",
@@ -4312,22 +4365,14 @@
 
     @preferred_terms.setter
     def preferred_terms(self, preferred_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preferred_terms = preferred_terms
 
-    type_name: str = Field("AtlasGlossaryTerm", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "AtlasGlossaryTerm":
-            raise ValueError("must be AtlasGlossaryTerm")
-        return v
-
     class Attributes(Asset.Attributes):
         short_description: Optional[str] = Field(
             None, description="", alias="shortDescription"
         )
         long_description: Optional[str] = Field(
             None, description="", alias="longDescription"
         )
@@ -4417,78 +4462,26 @@
 
     attributes: "AtlasGlossaryTerm.Attributes" = Field(
         default_factory=lambda: AtlasGlossaryTerm.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
-    @root_validator()
-    def update_qualified_name(cls, values):
-        if (
-            "attributes" in values
-            and values["attributes"]
-            and not values["attributes"].qualified_name
-        ):
-            values["attributes"].qualified_name = values["guid"]
-        return values
-
-    @classmethod
-    # @validate_arguments()
-    def create(
-        cls,
-        *,
-        name: StrictStr,
-        anchor: Optional[AtlasGlossary] = None,
-        glossary_qualified_name: Optional[StrictStr] = None,
-        glossary_guid: Optional[StrictStr] = None,
-        categories: Optional[list[AtlasGlossaryCategory]] = None,
-    ) -> AtlasGlossaryTerm:
-        validate_required_fields(["name"], [name])
-        return cls(
-            attributes=AtlasGlossaryTerm.Attributes.create(
-                name=name,
-                anchor=anchor,
-                glossary_qualified_name=glossary_qualified_name,
-                glossary_guid=glossary_guid,
-                categories=categories,
-            )
-        )
-
-    def trim_to_required(self) -> AtlasGlossaryTerm:
-        if self.anchor is None or not self.anchor.guid:
-            raise ValueError("anchor.guid must be available")
-        return self.create_for_modification(
-            qualified_name=self.qualified_name,
-            name=self.name,
-            glossary_guid=self.anchor.guid,
-        )
-
-    @classmethod
-    def create_for_modification(
-        cls: type[SelfAsset],
-        qualified_name: str = "",
-        name: str = "",
-        glossary_guid: str = "",
-    ) -> SelfAsset:
-        validate_required_fields(
-            ["name", "qualified_name", "glossary_guid"],
-            [name, qualified_name, glossary_guid],
-        )
-        glossary = AtlasGlossary()
-        glossary.guid = glossary_guid
-        return cls(
-            attributes=cls.Attributes(
-                qualified_name=qualified_name, name=name, anchor=glossary
-            )
-        )
-
 
 class AuthService(Asset, type_name="AuthService"):
     """Description"""
 
+    type_name: str = Field("AuthService", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "AuthService":
+            raise ValueError("must be AuthService")
+        return v
+
     def __setattr__(self, name, value):
         if name in AuthService._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "auth_service_type",
@@ -4552,22 +4545,14 @@
     def auth_service_policy_last_sync(
         self, auth_service_policy_last_sync: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.auth_service_policy_last_sync = auth_service_policy_last_sync
 
-    type_name: str = Field("AuthService", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "AuthService":
-            raise ValueError("must be AuthService")
-        return v
-
     class Attributes(Asset.Attributes):
         auth_service_type: Optional[str] = Field(
             None, description="", alias="authServiceType"
         )
         tag_service: Optional[str] = Field(None, description="", alias="tagService")
         auth_service_is_enabled: Optional[bool] = Field(
             None, description="", alias="authServiceIsEnabled"
@@ -4585,52 +4570,60 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Cloud(Asset, type_name="Cloud"):
     """Description"""
 
-    def __setattr__(self, name, value):
-        if name in Cloud._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
     type_name: str = Field("Cloud", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Cloud":
             raise ValueError("must be Cloud")
         return v
 
-
-class Infrastructure(Asset, type_name="Infrastructure"):
-    """Description"""
-
     def __setattr__(self, name, value):
-        if name in Infrastructure._convience_properties:
+        if name in Cloud._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = []
 
+
+class Infrastructure(Asset, type_name="Infrastructure"):
+    """Description"""
+
     type_name: str = Field("Infrastructure", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Infrastructure":
             raise ValueError("must be Infrastructure")
         return v
 
+    def __setattr__(self, name, value):
+        if name in Infrastructure._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
 
 class BIProcess(Process):
     """Description"""
 
+    type_name: str = Field("BIProcess", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "BIProcess":
+            raise ValueError("must be BIProcess")
+        return v
+
     def __setattr__(self, name, value):
         if name in BIProcess._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "outputs",
@@ -4653,22 +4646,14 @@
 
     @inputs.setter
     def inputs(self, inputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.inputs = inputs
 
-    type_name: str = Field("BIProcess", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "BIProcess":
-            raise ValueError("must be BIProcess")
-        return v
-
     class Attributes(Process.Attributes):
         outputs: Optional[list[Catalog]] = Field(
             None, description="", alias="outputs"
         )  # relationship
         inputs: Optional[list[Catalog]] = Field(
             None, description="", alias="inputs"
         )  # relationship
@@ -4679,14 +4664,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ColumnProcess(Process):
     """Description"""
 
+    type_name: str = Field("ColumnProcess", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ColumnProcess":
+            raise ValueError("must be ColumnProcess")
+        return v
+
     def __setattr__(self, name, value):
         if name in ColumnProcess._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "outputs",
@@ -4720,22 +4713,14 @@
 
     @inputs.setter
     def inputs(self, inputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.inputs = inputs
 
-    type_name: str = Field("ColumnProcess", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ColumnProcess":
-            raise ValueError("must be ColumnProcess")
-        return v
-
     class Attributes(Process.Attributes):
         outputs: Optional[list[Catalog]] = Field(
             None, description="", alias="outputs"
         )  # relationship
         process: Optional[Process] = Field(
             None, description="", alias="process"
         )  # relationship
@@ -4749,92 +4734,14 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Persona(AccessControl):
     """Description"""
 
-    def __setattr__(self, name, value):
-        if name in Persona._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "persona_groups",
-        "persona_users",
-        "role_id",
-    ]
-
-    @property
-    def persona_groups(self) -> Optional[set[str]]:
-        return None if self.attributes is None else self.attributes.persona_groups
-
-    @persona_groups.setter
-    def persona_groups(self, persona_groups: Optional[set[str]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.persona_groups = persona_groups
-
-    @property
-    def persona_users(self) -> Optional[set[str]]:
-        return None if self.attributes is None else self.attributes.persona_users
-
-    @persona_users.setter
-    def persona_users(self, persona_users: Optional[set[str]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.persona_users = persona_users
-
-    @property
-    def role_id(self) -> Optional[str]:
-        return None if self.attributes is None else self.attributes.role_id
-
-    @role_id.setter
-    def role_id(self, role_id: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.role_id = role_id
-
-    type_name: str = Field("Persona", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Persona":
-            raise ValueError("must be Persona")
-        return v
-
-    class Attributes(AccessControl.Attributes):
-        persona_groups: Optional[set[str]] = Field(
-            None, description="", alias="personaGroups"
-        )
-        persona_users: Optional[set[str]] = Field(
-            None, description="", alias="personaUsers"
-        )
-        role_id: Optional[str] = Field(None, description="", alias="roleId")
-
-        @classmethod
-        # @validate_arguments()
-        def create(cls, name: str) -> Persona.Attributes:
-            if not name:
-                raise ValueError("name cannot be blank")
-            validate_required_fields(["name"], [name])
-            return Persona.Attributes(
-                qualified_name=name,
-                name=name,
-                display_name=name,
-                is_access_control_enabled=True,
-                description="",
-            )
-
-    attributes: "Persona.Attributes" = Field(
-        default_factory=lambda: Persona.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
     @classmethod
     # @validate_arguments()
     def create(cls, *, name: str) -> Persona:
         validate_required_fields(["name"], [name])
         attributes = Persona.Attributes.create(name=name)
         return cls(attributes=attributes)
 
@@ -4850,15 +4757,15 @@
         connection_qualified_name: str,
         resources: Set[str],
     ) -> AuthPolicy:
         validate_required_fields(
             ["name", "persona_id", "policy_type", "actions", "resources"],
             [name, persona_id, policy_type, actions, resources],
         )
-        policy = AuthPolicy.create(name=name)
+        policy = AuthPolicy._AuthPolicy__create(name=name)  # type: ignore
         policy.policy_actions = {x.value for x in actions}
         policy.policy_category = AuthPolicyCategory.PERSONA.value
         policy.policy_type = policy_type
         policy.connection_qualified_name = connection_qualified_name
         policy.policy_resources = resources
         policy.policy_resource_category = AuthPolicyResourceCategory.CUSTOM.value
         policy.policy_service_name = "atlas"
@@ -4879,15 +4786,15 @@
         connection_qualified_name: str,
         resources: Set[str],
     ) -> AuthPolicy:
         validate_required_fields(
             ["name", "persona_id", "policy_type", "resources"],
             [name, persona_id, policy_type, resources],
         )
-        policy = AuthPolicy.create(name=name)
+        policy = AuthPolicy._AuthPolicy__create(name=name)  # type: ignore
         policy.policy_actions = {DataAction.SELECT.value}
         policy.policy_category = AuthPolicyCategory.PERSONA.value
         policy.policy_type = policy_type
         policy.connection_qualified_name = connection_qualified_name
         policy.policy_resources = resources
         policy.policy_resources.add("entity-type:*")
         policy.policy_resource_category = AuthPolicyResourceCategory.ENTITY.value
@@ -4909,15 +4816,15 @@
         actions: Set[PersonaGlossaryAction],
         resources: Set[str],
     ) -> AuthPolicy:
         validate_required_fields(
             ["name", "persona_id", "policy_type", "actions", "resources"],
             [name, persona_id, policy_type, actions, resources],
         )
-        policy = AuthPolicy.create(name=name)
+        policy = AuthPolicy._AuthPolicy__create(name=name)  # type: ignore
         policy.policy_actions = {x.value for x in actions}
         policy.policy_category = AuthPolicyCategory.PERSONA.value
         policy.policy_type = policy_type
         policy.policy_resources = resources
         policy.policy_resource_category = AuthPolicyResourceCategory.CUSTOM.value
         policy.policy_service_name = "atlas"
         policy.policy_sub_category = "glossary"
@@ -4941,80 +4848,101 @@
             attributes=cls.Attributes(
                 qualified_name=qualified_name,
                 name=name,
                 is_access_control_enabled=is_enabled,
             )
         )
 
+    type_name: str = Field("Persona", allow_mutation=False)
 
-class Purpose(AccessControl):
-    """Description"""
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Persona":
+            raise ValueError("must be Persona")
+        return v
 
     def __setattr__(self, name, value):
-        if name in Purpose._convience_properties:
+        if name in Persona._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "purpose_classifications",
+        "persona_groups",
+        "persona_users",
+        "role_id",
     ]
 
     @property
-    def purpose_classifications(self) -> Optional[set[str]]:
-        return (
-            None if self.attributes is None else self.attributes.purpose_classifications
-        )
+    def persona_groups(self) -> Optional[set[str]]:
+        return None if self.attributes is None else self.attributes.persona_groups
 
-    @purpose_classifications.setter
-    def purpose_classifications(self, purpose_classifications: Optional[set[str]]):
+    @persona_groups.setter
+    def persona_groups(self, persona_groups: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.purpose_classifications = purpose_classifications
+        self.attributes.persona_groups = persona_groups
 
-    type_name: str = Field("Purpose", allow_mutation=False)
+    @property
+    def persona_users(self) -> Optional[set[str]]:
+        return None if self.attributes is None else self.attributes.persona_users
 
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Purpose":
-            raise ValueError("must be Purpose")
-        return v
+    @persona_users.setter
+    def persona_users(self, persona_users: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.persona_users = persona_users
+
+    @property
+    def role_id(self) -> Optional[str]:
+        return None if self.attributes is None else self.attributes.role_id
+
+    @role_id.setter
+    def role_id(self, role_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.role_id = role_id
 
     class Attributes(AccessControl.Attributes):
-        purpose_classifications: Optional[set[str]] = Field(
-            None, description="", alias="purposeClassifications"
+        persona_groups: Optional[set[str]] = Field(
+            None, description="", alias="personaGroups"
         )
+        persona_users: Optional[set[str]] = Field(
+            None, description="", alias="personaUsers"
+        )
+        role_id: Optional[str] = Field(None, description="", alias="roleId")
 
         @classmethod
         # @validate_arguments()
-        def create(cls, name: str, classifications: list[str]) -> Purpose.Attributes:
-            validate_required_fields(
-                ["name", "classifications"], [name, classifications]
-            )
-            return Purpose.Attributes(
+        def create(cls, name: str) -> Persona.Attributes:
+            if not name:
+                raise ValueError("name cannot be blank")
+            validate_required_fields(["name"], [name])
+            return Persona.Attributes(
                 qualified_name=name,
                 name=name,
                 display_name=name,
                 is_access_control_enabled=True,
                 description="",
-                purpose_classifications=classifications,
             )
 
-    attributes: "Purpose.Attributes" = Field(
-        default_factory=lambda: Purpose.Attributes(),
+    attributes: "Persona.Attributes" = Field(
+        default_factory=lambda: Persona.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+
+class Purpose(AccessControl):
+    """Description"""
+
     @classmethod
     # @validate_arguments()
-    def create(cls, *, name: str, classifications: list[str]) -> Purpose:
-        validate_required_fields(["name", "classifications"], [name, classifications])
-        attributes = Purpose.Attributes.create(
-            name=name, classifications=classifications
-        )
+    def create(cls, *, name: str, atlan_tags: list[str]) -> Purpose:
+        validate_required_fields(["name", "atlan_tags"], [name, atlan_tags])
+        attributes = Purpose.Attributes.create(name=name, atlan_tags=atlan_tags)
         return cls(attributes=attributes)
 
     @classmethod
     # @validate_arguments()
     def create_metadata_policy(
         cls,
         *,
@@ -5027,15 +4955,15 @@
         all_users: bool = False,
     ) -> AuthPolicy:
         validate_required_fields(
             ["name", "purpose_id", "policy_type", "actions"],
             [name, purpose_id, policy_type, actions],
         )
         target_found = False
-        policy = AuthPolicy.create(name=name)
+        policy = AuthPolicy._AuthPolicy__create(name=name)  # type: ignore
         policy.policy_actions = {x.value for x in actions}
         policy.policy_category = AuthPolicyCategory.PURPOSE.value
         policy.policy_type = policy_type
         policy.policy_resource_category = AuthPolicyResourceCategory.TAG.value
         policy.policy_service_name = "atlas_tag"
         policy.policy_sub_category = "metadata"
         purpose = Purpose()
@@ -5085,15 +5013,15 @@
         policy_groups: Optional[Set[str]] = None,
         policy_users: Optional[Set[str]] = None,
         all_users: bool = False,
     ) -> AuthPolicy:
         validate_required_fields(
             ["name", "purpose_id", "policy_type"], [name, purpose_id, policy_type]
         )
-        policy = AuthPolicy.create(name=name)
+        policy = AuthPolicy._AuthPolicy__create(name=name)  # type: ignore
         policy.policy_actions = {DataAction.SELECT.value}
         policy.policy_category = AuthPolicyCategory.PURPOSE.value
         policy.policy_type = policy_type
         policy.policy_resource_category = AuthPolicyResourceCategory.TAG.value
         policy.policy_service_name = "atlas_tag"
         policy.policy_sub_category = "data"
         purpose = Purpose()
@@ -5147,18 +5075,77 @@
             attributes=cls.Attributes(
                 qualified_name=qualified_name,
                 name=name,
                 is_access_control_enabled=is_enabled,
             )
         )
 
+    type_name: str = Field("Purpose", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Purpose":
+            raise ValueError("must be Purpose")
+        return v
+
+    def __setattr__(self, name, value):
+        if name in Purpose._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "purpose_atlan_tags",
+    ]
+
+    @property
+    def purpose_atlan_tags(self) -> Optional[set[str]]:
+        return None if self.attributes is None else self.attributes.purpose_atlan_tags
+
+    @purpose_atlan_tags.setter
+    def purpose_atlan_tags(self, purpose_atlan_tags: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.purpose_atlan_tags = purpose_atlan_tags
+
+    class Attributes(AccessControl.Attributes):
+        purpose_atlan_tags: Optional[set[str]] = Field(
+            None, description="", alias="purposeClassifications"
+        )
+
+        @classmethod
+        # @validate_arguments()
+        def create(cls, name: str, atlan_tags: list[str]) -> Purpose.Attributes:
+            validate_required_fields(["name", "atlan_tags"], [name, atlan_tags])
+            return Purpose.Attributes(
+                qualified_name=name,
+                name=name,
+                display_name=name,
+                is_access_control_enabled=True,
+                description="",
+                purpose_atlan_tags=atlan_tags,
+            )
+
+    attributes: "Purpose.Attributes" = Field(
+        default_factory=lambda: Purpose.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class Collection(Namespace):
     """Description"""
 
+    type_name: str = Field("Collection", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Collection":
+            raise ValueError("must be Collection")
+        return v
+
     def __setattr__(self, name, value):
         if name in Collection._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "icon",
@@ -5181,36 +5168,36 @@
 
     @icon_type.setter
     def icon_type(self, icon_type: Optional[IconType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
-    type_name: str = Field("Collection", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Collection":
-            raise ValueError("must be Collection")
-        return v
-
     class Attributes(Namespace.Attributes):
         icon: Optional[str] = Field(None, description="", alias="icon")
         icon_type: Optional[IconType] = Field(None, description="", alias="iconType")
 
     attributes: "Collection.Attributes" = Field(
         default_factory=lambda: Collection.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Folder(Namespace):
     """Description"""
 
+    type_name: str = Field("Folder", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Folder":
+            raise ValueError("must be Folder")
+        return v
+
     def __setattr__(self, name, value):
         if name in Folder._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "parent_qualified_name",
@@ -5250,22 +5237,14 @@
 
     @parent.setter
     def parent(self, parent: Namespace):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.parent = parent
 
-    type_name: str = Field("Folder", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Folder":
-            raise ValueError("must be Folder")
-        return v
-
     class Attributes(Namespace.Attributes):
         parent_qualified_name: str = Field(
             None, description="", alias="parentQualifiedName"
         )
         collection_qualified_name: str = Field(
             None, description="", alias="collectionQualifiedName"
         )
@@ -5277,109 +5256,117 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class EventStore(Catalog):
     """Description"""
 
-    def __setattr__(self, name, value):
-        if name in EventStore._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
     type_name: str = Field("EventStore", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "EventStore":
             raise ValueError("must be EventStore")
         return v
 
-
-class ObjectStore(Catalog):
-    """Description"""
-
     def __setattr__(self, name, value):
-        if name in ObjectStore._convience_properties:
+        if name in EventStore._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = []
 
+
+class ObjectStore(Catalog):
+    """Description"""
+
     type_name: str = Field("ObjectStore", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ObjectStore":
             raise ValueError("must be ObjectStore")
         return v
 
-
-class DataQuality(Catalog):
-    """Description"""
-
     def __setattr__(self, name, value):
-        if name in DataQuality._convience_properties:
+        if name in ObjectStore._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = []
 
+
+class DataQuality(Catalog):
+    """Description"""
+
     type_name: str = Field("DataQuality", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataQuality":
             raise ValueError("must be DataQuality")
         return v
 
-
-class BI(Catalog):
-    """Description"""
-
     def __setattr__(self, name, value):
-        if name in BI._convience_properties:
+        if name in DataQuality._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = []
 
+
+class BI(Catalog):
+    """Description"""
+
     type_name: str = Field("BI", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "BI":
             raise ValueError("must be BI")
         return v
 
-
-class SaaS(Catalog):
-    """Description"""
-
     def __setattr__(self, name, value):
-        if name in SaaS._convience_properties:
+        if name in BI._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = []
 
+
+class SaaS(Catalog):
+    """Description"""
+
     type_name: str = Field("SaaS", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SaaS":
             raise ValueError("must be SaaS")
         return v
 
+    def __setattr__(self, name, value):
+        if name in SaaS._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
 
 class Dbt(Catalog):
     """Description"""
 
+    type_name: str = Field("Dbt", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Dbt":
+            raise ValueError("must be Dbt")
+        return v
+
     def __setattr__(self, name, value):
         if name in Dbt._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "dbt_alias",
@@ -5600,22 +5587,14 @@
 
     @dbt_semantic_layer_proxy_url.setter
     def dbt_semantic_layer_proxy_url(self, dbt_semantic_layer_proxy_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_semantic_layer_proxy_url = dbt_semantic_layer_proxy_url
 
-    type_name: str = Field("Dbt", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Dbt":
-            raise ValueError("must be Dbt")
-        return v
-
     class Attributes(Catalog.Attributes):
         dbt_alias: Optional[str] = Field(None, description="", alias="dbtAlias")
         dbt_meta: Optional[str] = Field(None, description="", alias="dbtMeta")
         dbt_unique_id: Optional[str] = Field(None, description="", alias="dbtUniqueId")
         dbt_account_name: Optional[str] = Field(
             None, description="", alias="dbtAccountName"
         )
@@ -5664,14 +5643,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Resource(Catalog):
     """Description"""
 
+    type_name: str = Field("Resource", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Resource":
+            raise ValueError("must be Resource")
+        return v
+
     def __setattr__(self, name, value):
         if name in Resource._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "link",
@@ -5716,22 +5703,14 @@
 
     @resource_metadata.setter
     def resource_metadata(self, resource_metadata: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.resource_metadata = resource_metadata
 
-    type_name: str = Field("Resource", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Resource":
-            raise ValueError("must be Resource")
-        return v
-
     class Attributes(Catalog.Attributes):
         link: Optional[str] = Field(None, description="", alias="link")
         is_global: Optional[bool] = Field(None, description="", alias="isGlobal")
         reference: Optional[str] = Field(None, description="", alias="reference")
         resource_metadata: Optional[dict[str, str]] = Field(
             None, description="", alias="resourceMetadata"
         )
@@ -5742,33 +5721,41 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Insight(Catalog):
     """Description"""
 
-    def __setattr__(self, name, value):
-        if name in Insight._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
     type_name: str = Field("Insight", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Insight":
             raise ValueError("must be Insight")
         return v
 
+    def __setattr__(self, name, value):
+        if name in Insight._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
 
 class API(Catalog):
     """Description"""
 
+    type_name: str = Field("API", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "API":
+            raise ValueError("must be API")
+        return v
+
     def __setattr__(self, name, value):
         if name in API._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "api_spec_type",
@@ -5837,22 +5824,14 @@
 
     @api_is_auth_optional.setter
     def api_is_auth_optional(self, api_is_auth_optional: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_is_auth_optional = api_is_auth_optional
 
-    type_name: str = Field("API", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "API":
-            raise ValueError("must be API")
-        return v
-
     class Attributes(Catalog.Attributes):
         api_spec_type: Optional[str] = Field(None, description="", alias="apiSpecType")
         api_spec_version: Optional[str] = Field(
             None, description="", alias="apiSpecVersion"
         )
         api_spec_name: Optional[str] = Field(None, description="", alias="apiSpecName")
         api_spec_qualified_name: Optional[str] = Field(
@@ -5871,24 +5850,32 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Tag(Catalog):
     """Description"""
 
+    type_name: str = Field("Tag", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Tag":
+            raise ValueError("must be Tag")
+        return v
+
     def __setattr__(self, name, value):
         if name in Tag._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "tag_id",
         "tag_attributes",
         "tag_allowed_values",
-        "mapped_classification_name",
+        "mapped_atlan_tag_name",
     ]
 
     @property
     def tag_id(self) -> Optional[str]:
         return None if self.attributes is None else self.attributes.tag_id
 
     @tag_id.setter
@@ -5914,57 +5901,55 @@
     @tag_allowed_values.setter
     def tag_allowed_values(self, tag_allowed_values: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tag_allowed_values = tag_allowed_values
 
     @property
-    def mapped_classification_name(self) -> Optional[str]:
+    def mapped_atlan_tag_name(self) -> Optional[str]:
         return (
-            None
-            if self.attributes is None
-            else self.attributes.mapped_classification_name
+            None if self.attributes is None else self.attributes.mapped_atlan_tag_name
         )
 
-    @mapped_classification_name.setter
-    def mapped_classification_name(self, mapped_classification_name: Optional[str]):
+    @mapped_atlan_tag_name.setter
+    def mapped_atlan_tag_name(self, mapped_atlan_tag_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.mapped_classification_name = mapped_classification_name
-
-    type_name: str = Field("Tag", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Tag":
-            raise ValueError("must be Tag")
-        return v
+        self.attributes.mapped_atlan_tag_name = mapped_atlan_tag_name
 
     class Attributes(Catalog.Attributes):
         tag_id: Optional[str] = Field(None, description="", alias="tagId")
         tag_attributes: Optional[list[SourceTagAttribute]] = Field(
             None, description="", alias="tagAttributes"
         )
         tag_allowed_values: Optional[set[str]] = Field(
             None, description="", alias="tagAllowedValues"
         )
-        mapped_classification_name: Optional[str] = Field(
+        mapped_atlan_tag_name: Optional[str] = Field(
             None, description="", alias="mappedClassificationName"
         )
 
     attributes: "Tag.Attributes" = Field(
         default_factory=lambda: Tag.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SQL(Catalog):
     """Description"""
 
+    type_name: str = Field("SQL", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SQL":
+            raise ValueError("must be SQL")
+        return v
+
     def __setattr__(self, name, value):
         if name in SQL._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "query_count",
@@ -6169,22 +6154,14 @@
 
     @dbt_models.setter
     def dbt_models(self, dbt_models: Optional[list[DbtModel]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_models = dbt_models
 
-    type_name: str = Field("SQL", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SQL":
-            raise ValueError("must be SQL")
-        return v
-
     class Attributes(Catalog.Attributes):
         query_count: Optional[int] = Field(None, description="", alias="queryCount")
         query_user_count: Optional[int] = Field(
             None, description="", alias="queryUserCount"
         )
         query_user_map: Optional[dict[str, int]] = Field(
             None, description="", alias="queryUserMap"
@@ -6231,14 +6208,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Google(Cloud):
     """Description"""
 
+    type_name: str = Field("Google", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Google":
+            raise ValueError("must be Google")
+        return v
+
     def __setattr__(self, name, value):
         if name in Google._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "google_service",
@@ -6329,22 +6314,14 @@
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
-    type_name: str = Field("Google", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Google":
-            raise ValueError("must be Google")
-        return v
-
     class Attributes(Cloud.Attributes):
         google_service: Optional[str] = Field(
             None, description="", alias="googleService"
         )
         google_project_name: Optional[str] = Field(
             None, description="", alias="googleProjectName"
         )
@@ -6373,14 +6350,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Azure(Cloud):
     """Description"""
 
+    type_name: str = Field("Azure", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Azure":
+            raise ValueError("must be Azure")
+        return v
+
     def __setattr__(self, name, value):
         if name in Azure._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "azure_resource_id",
@@ -6433,22 +6418,14 @@
 
     @azure_tags.setter
     def azure_tags(self, azure_tags: Optional[list[AzureTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_tags = azure_tags
 
-    type_name: str = Field("Azure", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Azure":
-            raise ValueError("must be Azure")
-        return v
-
     class Attributes(Cloud.Attributes):
         azure_resource_id: Optional[str] = Field(
             None, description="", alias="azureResourceId"
         )
         azure_location: Optional[str] = Field(
             None, description="", alias="azureLocation"
         )
@@ -6465,14 +6442,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class AWS(Cloud):
     """Description"""
 
+    type_name: str = Field("AWS", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "AWS":
+            raise ValueError("must be AWS")
+        return v
+
     def __setattr__(self, name, value):
         if name in AWS._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "aws_arn",
@@ -6572,22 +6557,14 @@
 
     @aws_tags.setter
     def aws_tags(self, aws_tags: Optional[list[AwsTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_tags = aws_tags
 
-    type_name: str = Field("AWS", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "AWS":
-            raise ValueError("must be AWS")
-        return v
-
     class Attributes(Cloud.Attributes):
         aws_arn: Optional[str] = Field(None, description="", alias="awsArn")
         aws_partition: Optional[str] = Field(None, description="", alias="awsPartition")
         aws_service: Optional[str] = Field(None, description="", alias="awsService")
         aws_region: Optional[str] = Field(None, description="", alias="awsRegion")
         aws_account_id: Optional[str] = Field(
             None, description="", alias="awsAccountId"
@@ -6607,14 +6584,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtColumnProcess(Dbt):
     """Description"""
 
+    type_name: str = Field("DbtColumnProcess", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "DbtColumnProcess":
+            raise ValueError("must be DbtColumnProcess")
+        return v
+
     def __setattr__(self, name, value):
         if name in DbtColumnProcess._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "dbt_column_process_job_status",
@@ -6929,22 +6914,14 @@
 
     @column_processes.setter
     def column_processes(self, column_processes: Optional[list[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_processes = column_processes
 
-    type_name: str = Field("DbtColumnProcess", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "DbtColumnProcess":
-            raise ValueError("must be DbtColumnProcess")
-        return v
-
     class Attributes(Dbt.Attributes):
         dbt_column_process_job_status: Optional[str] = Field(
             None, description="", alias="dbtColumnProcessJobStatus"
         )
         dbt_alias: Optional[str] = Field(None, description="", alias="dbtAlias")
         dbt_meta: Optional[str] = Field(None, description="", alias="dbtMeta")
         dbt_unique_id: Optional[str] = Field(None, description="", alias="dbtUniqueId")
@@ -7007,33 +6984,41 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Kafka(EventStore):
     """Description"""
 
-    def __setattr__(self, name, value):
-        if name in Kafka._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
     type_name: str = Field("Kafka", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Kafka":
             raise ValueError("must be Kafka")
         return v
 
+    def __setattr__(self, name, value):
+        if name in Kafka._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
 
 class S3(ObjectStore):
     """Description"""
 
+    type_name: str = Field("S3", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "S3":
+            raise ValueError("must be S3")
+        return v
+
     def __setattr__(self, name, value):
         if name in S3._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "s3_e_tag",
@@ -7155,22 +7140,14 @@
 
     @aws_tags.setter
     def aws_tags(self, aws_tags: Optional[list[AwsTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_tags = aws_tags
 
-    type_name: str = Field("S3", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "S3":
-            raise ValueError("must be S3")
-        return v
-
     class Attributes(ObjectStore.Attributes):
         s3_e_tag: Optional[str] = Field(None, description="", alias="s3ETag")
         s3_encryption: Optional[str] = Field(None, description="", alias="s3Encryption")
         aws_arn: Optional[str] = Field(None, description="", alias="awsArn")
         aws_partition: Optional[str] = Field(None, description="", alias="awsPartition")
         aws_service: Optional[str] = Field(None, description="", alias="awsService")
         aws_region: Optional[str] = Field(None, description="", alias="awsRegion")
@@ -7192,14 +7169,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ADLS(ObjectStore):
     """Description"""
 
+    type_name: str = Field("ADLS", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ADLS":
+            raise ValueError("must be ADLS")
+        return v
+
     def __setattr__(self, name, value):
         if name in ADLS._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "adls_account_qualified_name",
@@ -7267,22 +7252,14 @@
 
     @azure_tags.setter
     def azure_tags(self, azure_tags: Optional[list[AzureTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_tags = azure_tags
 
-    type_name: str = Field("ADLS", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ADLS":
-            raise ValueError("must be ADLS")
-        return v
-
     class Attributes(ObjectStore.Attributes):
         adls_account_qualified_name: Optional[str] = Field(
             None, description="", alias="adlsAccountQualifiedName"
         )
         azure_resource_id: Optional[str] = Field(
             None, description="", alias="azureResourceId"
         )
@@ -7302,14 +7279,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class GCS(Google):
     """Description"""
 
+    type_name: str = Field("GCS", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "GCS":
+            raise ValueError("must be GCS")
+        return v
+
     def __setattr__(self, name, value):
         if name in GCS._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "gcs_storage_class",
@@ -7492,22 +7477,14 @@
 
     @output_from_processes.setter
     def output_from_processes(self, output_from_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_from_processes = output_from_processes
 
-    type_name: str = Field("GCS", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "GCS":
-            raise ValueError("must be GCS")
-        return v
-
     class Attributes(Google.Attributes):
         gcs_storage_class: Optional[str] = Field(
             None, description="", alias="gcsStorageClass"
         )
         gcs_encryption_type: Optional[str] = Field(
             None, description="", alias="gcsEncryptionType"
         )
@@ -7558,14 +7535,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MonteCarlo(DataQuality):
     """Description"""
 
+    type_name: str = Field("MonteCarlo", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MonteCarlo":
+            raise ValueError("must be MonteCarlo")
+        return v
+
     def __setattr__(self, name, value):
         if name in MonteCarlo._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mc_labels",
@@ -7592,22 +7577,14 @@
 
     @mc_asset_qualified_names.setter
     def mc_asset_qualified_names(self, mc_asset_qualified_names: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_asset_qualified_names = mc_asset_qualified_names
 
-    type_name: str = Field("MonteCarlo", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MonteCarlo":
-            raise ValueError("must be MonteCarlo")
-        return v
-
     class Attributes(DataQuality.Attributes):
         mc_labels: Optional[set[str]] = Field(None, description="", alias="mcLabels")
         mc_asset_qualified_names: Optional[set[str]] = Field(
             None, description="", alias="mcAssetQualifiedNames"
         )
 
     attributes: "MonteCarlo.Attributes" = Field(
@@ -7616,14 +7593,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Metric(DataQuality):
     """Description"""
 
+    type_name: str = Field("Metric", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Metric":
+            raise ValueError("must be Metric")
+        return v
+
     def __setattr__(self, name, value):
         if name in Metric._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metric_type",
@@ -7709,22 +7694,14 @@
 
     @metric_timestamp_column.setter
     def metric_timestamp_column(self, metric_timestamp_column: Optional[Column]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_timestamp_column = metric_timestamp_column
 
-    type_name: str = Field("Metric", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Metric":
-            raise ValueError("must be Metric")
-        return v
-
     class Attributes(DataQuality.Attributes):
         metric_type: Optional[str] = Field(None, description="", alias="metricType")
         metric_s_q_l: Optional[str] = Field(None, description="", alias="metricSQL")
         metric_filters: Optional[str] = Field(
             None, description="", alias="metricFilters"
         )
         metric_time_grains: Optional[set[str]] = Field(
@@ -7746,14 +7723,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Preset(BI):
     """Description"""
 
+    type_name: str = Field("Preset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Preset":
+            raise ValueError("must be Preset")
+        return v
+
     def __setattr__(self, name, value):
         if name in Preset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "preset_workspace_id",
@@ -7814,22 +7799,14 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard_qualified_name = (
             preset_dashboard_qualified_name
         )
 
-    type_name: str = Field("Preset", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Preset":
-            raise ValueError("must be Preset")
-        return v
-
     class Attributes(BI.Attributes):
         preset_workspace_id: Optional[int] = Field(
             None, description="", alias="presetWorkspaceId"
         )
         preset_workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="presetWorkspaceQualifiedName"
         )
@@ -7846,14 +7823,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Mode(BI):
     """Description"""
 
+    type_name: str = Field("Mode", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Mode":
+            raise ValueError("must be Mode")
+        return v
+
     def __setattr__(self, name, value):
         if name in Mode._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_id",
@@ -7969,22 +7954,14 @@
 
     @mode_query_qualified_name.setter
     def mode_query_qualified_name(self, mode_query_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_query_qualified_name = mode_query_qualified_name
 
-    type_name: str = Field("Mode", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Mode":
-            raise ValueError("must be Mode")
-        return v
-
     class Attributes(BI.Attributes):
         mode_id: Optional[str] = Field(None, description="", alias="modeId")
         mode_token: Optional[str] = Field(None, description="", alias="modeToken")
         mode_workspace_name: Optional[str] = Field(
             None, description="", alias="modeWorkspaceName"
         )
         mode_workspace_username: Optional[str] = Field(
@@ -8012,14 +7989,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Sigma(BI):
     """Description"""
 
+    type_name: str = Field("Sigma", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Sigma":
+            raise ValueError("must be Sigma")
+        return v
+
     def __setattr__(self, name, value):
         if name in Sigma._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_workbook_qualified_name",
@@ -8106,22 +8091,14 @@
 
     @sigma_data_element_name.setter
     def sigma_data_element_name(self, sigma_data_element_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_name = sigma_data_element_name
 
-    type_name: str = Field("Sigma", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Sigma":
-            raise ValueError("must be Sigma")
-        return v
-
     class Attributes(BI.Attributes):
         sigma_workbook_qualified_name: Optional[str] = Field(
             None, description="", alias="sigmaWorkbookQualifiedName"
         )
         sigma_workbook_name: Optional[str] = Field(
             None, description="", alias="sigmaWorkbookName"
         )
@@ -8144,52 +8121,60 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Tableau(BI):
     """Description"""
 
-    def __setattr__(self, name, value):
-        if name in Tableau._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
     type_name: str = Field("Tableau", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Tableau":
             raise ValueError("must be Tableau")
         return v
 
-
-class Looker(BI):
-    """Description"""
-
     def __setattr__(self, name, value):
-        if name in Looker._convience_properties:
+        if name in Tableau._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = []
 
+
+class Looker(BI):
+    """Description"""
+
     type_name: str = Field("Looker", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Looker":
             raise ValueError("must be Looker")
         return v
 
+    def __setattr__(self, name, value):
+        if name in Looker._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
 
 class Redash(BI):
     """Description"""
 
+    type_name: str = Field("Redash", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Redash":
+            raise ValueError("must be Redash")
+        return v
+
     def __setattr__(self, name, value):
         if name in Redash._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "redash_is_published",
@@ -8201,22 +8186,14 @@
 
     @redash_is_published.setter
     def redash_is_published(self, redash_is_published: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_is_published = redash_is_published
 
-    type_name: str = Field("Redash", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Redash":
-            raise ValueError("must be Redash")
-        return v
-
     class Attributes(BI.Attributes):
         redash_is_published: Optional[bool] = Field(
             None, description="", alias="redashIsPublished"
         )
 
     attributes: "Redash.Attributes" = Field(
         default_factory=lambda: Redash.Attributes(),
@@ -8224,14 +8201,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DataStudio(Google):
     """Description"""
 
+    type_name: str = Field("DataStudio", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "DataStudio":
+            raise ValueError("must be DataStudio")
+        return v
+
     def __setattr__(self, name, value):
         if name in DataStudio._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "google_service",
@@ -8346,22 +8331,14 @@
 
     @output_from_processes.setter
     def output_from_processes(self, output_from_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_from_processes = output_from_processes
 
-    type_name: str = Field("DataStudio", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "DataStudio":
-            raise ValueError("must be DataStudio")
-        return v
-
     class Attributes(Google.Attributes):
         google_service: Optional[str] = Field(
             None, description="", alias="googleService"
         )
         google_project_name: Optional[str] = Field(
             None, description="", alias="googleProjectName"
         )
@@ -8396,14 +8373,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Metabase(BI):
     """Description"""
 
+    type_name: str = Field("Metabase", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Metabase":
+            raise ValueError("must be Metabase")
+        return v
+
     def __setattr__(self, name, value):
         if name in Metabase._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metabase_collection_name",
@@ -8438,22 +8423,14 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_collection_qualified_name = (
             metabase_collection_qualified_name
         )
 
-    type_name: str = Field("Metabase", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Metabase":
-            raise ValueError("must be Metabase")
-        return v
-
     class Attributes(BI.Attributes):
         metabase_collection_name: Optional[str] = Field(
             None, description="", alias="metabaseCollectionName"
         )
         metabase_collection_qualified_name: Optional[str] = Field(
             None, description="", alias="metabaseCollectionQualifiedName"
         )
@@ -8464,14 +8441,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSight(BI):
     """Description"""
 
+    type_name: str = Field("QuickSight", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSight":
+            raise ValueError("must be QuickSight")
+        return v
+
     def __setattr__(self, name, value):
         if name in QuickSight._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_id",
@@ -8507,22 +8492,14 @@
 
     @quick_sight_sheet_name.setter
     def quick_sight_sheet_name(self, quick_sight_sheet_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_sheet_name = quick_sight_sheet_name
 
-    type_name: str = Field("QuickSight", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSight":
-            raise ValueError("must be QuickSight")
-        return v
-
     class Attributes(BI.Attributes):
         quick_sight_id: Optional[str] = Field(
             None, description="", alias="quickSightId"
         )
         quick_sight_sheet_id: Optional[str] = Field(
             None, description="", alias="quickSightSheetId"
         )
@@ -8536,14 +8513,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Thoughtspot(BI):
     """Description"""
 
+    type_name: str = Field("Thoughtspot", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Thoughtspot":
+            raise ValueError("must be Thoughtspot")
+        return v
+
     def __setattr__(self, name, value):
         if name in Thoughtspot._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "thoughtspot_chart_type",
@@ -8572,22 +8557,14 @@
 
     @thoughtspot_question_text.setter
     def thoughtspot_question_text(self, thoughtspot_question_text: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.thoughtspot_question_text = thoughtspot_question_text
 
-    type_name: str = Field("Thoughtspot", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Thoughtspot":
-            raise ValueError("must be Thoughtspot")
-        return v
-
     class Attributes(BI.Attributes):
         thoughtspot_chart_type: Optional[str] = Field(
             None, description="", alias="thoughtspotChartType"
         )
         thoughtspot_question_text: Optional[str] = Field(
             None, description="", alias="thoughtspotQuestionText"
         )
@@ -8598,14 +8575,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBI(BI):
     """Description"""
 
+    type_name: str = Field("PowerBI", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBI":
+            raise ValueError("must be PowerBI")
+        return v
+
     def __setattr__(self, name, value):
         if name in PowerBI._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "power_b_i_is_hidden",
@@ -8662,22 +8647,14 @@
     def power_b_i_endorsement(
         self, power_b_i_endorsement: Optional[PowerbiEndorsement]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_endorsement = power_b_i_endorsement
 
-    type_name: str = Field("PowerBI", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBI":
-            raise ValueError("must be PowerBI")
-        return v
-
     class Attributes(BI.Attributes):
         power_b_i_is_hidden: Optional[bool] = Field(
             None, description="", alias="powerBIIsHidden"
         )
         power_b_i_table_qualified_name: Optional[str] = Field(
             None, description="", alias="powerBITableQualifiedName"
         )
@@ -8694,14 +8671,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MicroStrategy(BI):
     """Description"""
 
+    type_name: str = Field("MicroStrategy", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategy":
+            raise ValueError("must be MicroStrategy")
+        return v
+
     def __setattr__(self, name, value):
         if name in MicroStrategy._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "micro_strategy_project_qualified_name",
@@ -8868,22 +8853,14 @@
     def micro_strategy_location(
         self, micro_strategy_location: Optional[list[dict[str, str]]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_location = micro_strategy_location
 
-    type_name: str = Field("MicroStrategy", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MicroStrategy":
-            raise ValueError("must be MicroStrategy")
-        return v
-
     class Attributes(BI.Attributes):
         micro_strategy_project_qualified_name: Optional[str] = Field(
             None, description="", alias="microStrategyProjectQualifiedName"
         )
         micro_strategy_project_name: Optional[str] = Field(
             None, description="", alias="microStrategyProjectName"
         )
@@ -8918,14 +8895,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Qlik(BI):
     """Description"""
 
+    type_name: str = Field("Qlik", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Qlik":
+            raise ValueError("must be Qlik")
+        return v
+
     def __setattr__(self, name, value):
         if name in Qlik._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_id",
@@ -9020,22 +9005,14 @@
 
     @qlik_is_published.setter
     def qlik_is_published(self, qlik_is_published: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_is_published = qlik_is_published
 
-    type_name: str = Field("Qlik", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Qlik":
-            raise ValueError("must be Qlik")
-        return v
-
     class Attributes(BI.Attributes):
         qlik_id: Optional[str] = Field(None, description="", alias="qlikId")
         qlik_q_r_i: Optional[str] = Field(None, description="", alias="qlikQRI")
         qlik_space_id: Optional[str] = Field(None, description="", alias="qlikSpaceId")
         qlik_space_qualified_name: Optional[str] = Field(
             None, description="", alias="qlikSpaceQualifiedName"
         )
@@ -9054,14 +9031,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Salesforce(SaaS):
     """Description"""
 
+    type_name: str = Field("Salesforce", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Salesforce":
+            raise ValueError("must be Salesforce")
+        return v
+
     def __setattr__(self, name, value):
         if name in Salesforce._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "organization_qualified_name",
@@ -9088,22 +9073,14 @@
 
     @api_name.setter
     def api_name(self, api_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_name = api_name
 
-    type_name: str = Field("Salesforce", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Salesforce":
-            raise ValueError("must be Salesforce")
-        return v
-
     class Attributes(SaaS.Attributes):
         organization_qualified_name: Optional[str] = Field(
             None, description="", alias="organizationQualifiedName"
         )
         api_name: Optional[str] = Field(None, description="", alias="apiName")
 
     attributes: "Salesforce.Attributes" = Field(
@@ -9112,14 +9089,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtModelColumn(Dbt):
     """Description"""
 
+    type_name: str = Field("DbtModelColumn", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "DbtModelColumn":
+            raise ValueError("must be DbtModelColumn")
+        return v
+
     def __setattr__(self, name, value):
         if name in DbtModelColumn._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "dbt_model_qualified_name",
@@ -9202,22 +9187,14 @@
 
     @dbt_model.setter
     def dbt_model(self, dbt_model: Optional[DbtModel]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model = dbt_model
 
-    type_name: str = Field("DbtModelColumn", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "DbtModelColumn":
-            raise ValueError("must be DbtModelColumn")
-        return v
-
     class Attributes(Dbt.Attributes):
         dbt_model_qualified_name: Optional[str] = Field(
             None, description="", alias="dbtModelQualifiedName"
         )
         dbt_model_column_data_type: Optional[str] = Field(
             None, description="", alias="dbtModelColumnDataType"
         )
@@ -9240,14 +9217,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtModel(Dbt):
     """Description"""
 
+    type_name: str = Field("DbtModel", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "DbtModel":
+            raise ValueError("must be DbtModel")
+        return v
+
     def __setattr__(self, name, value):
         if name in DbtModel._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "dbt_status",
@@ -9477,22 +9462,14 @@
 
     @sql_asset.setter
     def sql_asset(self, sql_asset: Optional[SQL]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_asset = sql_asset
 
-    type_name: str = Field("DbtModel", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "DbtModel":
-            raise ValueError("must be DbtModel")
-        return v
-
     class Attributes(Dbt.Attributes):
         dbt_status: Optional[str] = Field(None, description="", alias="dbtStatus")
         dbt_error: Optional[str] = Field(None, description="", alias="dbtError")
         dbt_raw_s_q_l: Optional[str] = Field(None, description="", alias="dbtRawSQL")
         dbt_compiled_s_q_l: Optional[str] = Field(
             None, description="", alias="dbtCompiledSQL"
         )
@@ -9540,14 +9517,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtMetric(Dbt):
     """Description"""
 
+    type_name: str = Field("DbtMetric", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "DbtMetric":
+            raise ValueError("must be DbtMetric")
+        return v
+
     def __setattr__(self, name, value):
         if name in DbtMetric._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "dbt_metric_filters",
@@ -9892,22 +9877,14 @@
     def dbt_metric_filter_columns(
         self, dbt_metric_filter_columns: Optional[list[Column]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_metric_filter_columns = dbt_metric_filter_columns
 
-    type_name: str = Field("DbtMetric", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "DbtMetric":
-            raise ValueError("must be DbtMetric")
-        return v
-
     class Attributes(Dbt.Attributes):
         dbt_metric_filters: Optional[list[DbtMetricFilter]] = Field(
             None, description="", alias="dbtMetricFilters"
         )
         dbt_alias: Optional[str] = Field(None, description="", alias="dbtAlias")
         dbt_meta: Optional[str] = Field(None, description="", alias="dbtMeta")
         dbt_unique_id: Optional[str] = Field(None, description="", alias="dbtUniqueId")
@@ -9982,14 +9959,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtSource(Dbt):
     """Description"""
 
+    type_name: str = Field("DbtSource", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "DbtSource":
+            raise ValueError("must be DbtSource")
+        return v
+
     def __setattr__(self, name, value):
         if name in DbtSource._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "dbt_state",
@@ -10036,22 +10021,14 @@
 
     @sql_asset.setter
     def sql_asset(self, sql_asset: Optional[SQL]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_asset = sql_asset
 
-    type_name: str = Field("DbtSource", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "DbtSource":
-            raise ValueError("must be DbtSource")
-        return v
-
     class Attributes(Dbt.Attributes):
         dbt_state: Optional[str] = Field(None, description="", alias="dbtState")
         dbt_freshness_criteria: Optional[str] = Field(
             None, description="", alias="dbtFreshnessCriteria"
         )
         sql_assets: Optional[list[SQL]] = Field(
             None, description="", alias="sqlAssets"
@@ -10066,14 +10043,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtProcess(Dbt):
     """Description"""
 
+    type_name: str = Field("DbtProcess", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "DbtProcess":
+            raise ValueError("must be DbtProcess")
+        return v
+
     def __setattr__(self, name, value):
         if name in DbtProcess._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "dbt_process_job_status",
@@ -10373,22 +10358,14 @@
 
     @column_processes.setter
     def column_processes(self, column_processes: Optional[list[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_processes = column_processes
 
-    type_name: str = Field("DbtProcess", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "DbtProcess":
-            raise ValueError("must be DbtProcess")
-        return v
-
     class Attributes(Dbt.Attributes):
         dbt_process_job_status: Optional[str] = Field(
             None, description="", alias="dbtProcessJobStatus"
         )
         dbt_alias: Optional[str] = Field(None, description="", alias="dbtAlias")
         dbt_meta: Optional[str] = Field(None, description="", alias="dbtMeta")
         dbt_unique_id: Optional[str] = Field(None, description="", alias="dbtUniqueId")
@@ -10448,14 +10425,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ReadmeTemplate(Resource):
     """Description"""
 
+    type_name: str = Field("ReadmeTemplate", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ReadmeTemplate":
+            raise ValueError("must be ReadmeTemplate")
+        return v
+
     def __setattr__(self, name, value):
         if name in ReadmeTemplate._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "icon",
@@ -10478,36 +10463,60 @@
 
     @icon_type.setter
     def icon_type(self, icon_type: Optional[IconType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
-    type_name: str = Field("ReadmeTemplate", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ReadmeTemplate":
-            raise ValueError("must be ReadmeTemplate")
-        return v
-
     class Attributes(Resource.Attributes):
         icon: Optional[str] = Field(None, description="", alias="icon")
         icon_type: Optional[IconType] = Field(None, description="", alias="iconType")
 
     attributes: "ReadmeTemplate.Attributes" = Field(
         default_factory=lambda: ReadmeTemplate.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Readme(Resource):
     """Description"""
 
+    @classmethod
+    # @validate_arguments()
+    def create(
+        cls, *, asset: Asset, content: str, asset_name: Optional[str] = None
+    ) -> Readme:
+        return Readme(
+            attributes=Readme.Attributes.create(
+                asset=asset, content=content, asset_name=asset_name
+            )
+        )
+
+    @property
+    def description(self) -> Optional[str]:
+        ret_value = self.attributes.description
+        return unquote(ret_value) if ret_value is not None else ret_value
+
+    @description.setter
+    def description(self, description: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.description = (
+            quote(description) if description is not None else description
+        )
+
+    type_name: str = Field("Readme", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Readme":
+            raise ValueError("must be Readme")
+        return v
+
     def __setattr__(self, name, value):
         if name in Readme._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "internal",
@@ -10541,46 +10550,14 @@
 
     @see_also.setter
     def see_also(self, see_also: Optional[list[Readme]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.see_also = see_also
 
-    type_name: str = Field("Readme", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Readme":
-            raise ValueError("must be Readme")
-        return v
-
-    @classmethod
-    # @validate_arguments()
-    def create(
-        cls, *, asset: Asset, content: str, asset_name: Optional[str] = None
-    ) -> Readme:
-        return Readme(
-            attributes=Readme.Attributes.create(
-                asset=asset, content=content, asset_name=asset_name
-            )
-        )
-
-    @property
-    def description(self) -> Optional[str]:
-        ret_value = self.attributes.description
-        return unquote(ret_value) if ret_value is not None else ret_value
-
-    @description.setter
-    def description(self, description: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.description = (
-            quote(description) if description is not None else description
-        )
-
     class Attributes(Resource.Attributes):
         internal: Optional[Internal] = Field(
             None, description="", alias="__internal"
         )  # relationship
         asset: Optional[Asset] = Field(
             None, description="", alias="asset"
         )  # relationship
@@ -10618,14 +10595,35 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class File(Resource):
     """Description"""
 
+    @classmethod
+    # @validate_arguments()
+    def create(
+        cls, *, name: str, connection_qualified_name: str, file_type: FileType
+    ) -> File:
+        return File(
+            attributes=File.Attributes.create(
+                name=name,
+                connection_qualified_name=connection_qualified_name,
+                file_type=file_type,
+            )
+        )
+
+    type_name: str = Field("File", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "File":
+            raise ValueError("must be File")
+        return v
+
     def __setattr__(self, name, value):
         if name in File._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "file_type",
@@ -10659,39 +10657,55 @@
 
     @file_assets.setter
     def file_assets(self, file_assets: Optional[Asset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.file_assets = file_assets
 
-    type_name: str = Field("File", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "File":
-            raise ValueError("must be File")
-        return v
-
     class Attributes(Resource.Attributes):
         file_type: Optional[FileType] = Field(None, description="", alias="fileType")
         file_path: Optional[str] = Field(None, description="", alias="filePath")
         file_assets: Optional[Asset] = Field(
             None, description="", alias="fileAssets"
         )  # relationship
 
+        @classmethod
+        # @validate_arguments()
+        def create(
+            cls, *, name: str, connection_qualified_name: str, file_type: FileType
+        ) -> File.Attributes:
+            validate_required_fields(
+                ["name", "connection_qualified_name", "file_type"],
+                [name, connection_qualified_name, file_type],
+            )
+            return File.Attributes(
+                name=name,
+                qualified_name=f"{connection_qualified_name}/{name}",
+                connection_qualified_name=connection_qualified_name,
+                file_type=file_type,
+            )
+
     attributes: "File.Attributes" = Field(
         default_factory=lambda: File.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Link(Resource):
     """Description"""
 
+    type_name: str = Field("Link", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Link":
+            raise ValueError("must be Link")
+        return v
+
     def __setattr__(self, name, value):
         if name in Link._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "icon",
@@ -10736,22 +10750,14 @@
 
     @asset.setter
     def asset(self, asset: Optional[Asset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset = asset
 
-    type_name: str = Field("Link", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Link":
-            raise ValueError("must be Link")
-        return v
-
     class Attributes(Resource.Attributes):
         icon: Optional[str] = Field(None, description="", alias="icon")
         icon_type: Optional[IconType] = Field(None, description="", alias="iconType")
         internal: Optional[Internal] = Field(
             None, description="", alias="internal"
         )  # relationship
         asset: Optional[Asset] = Field(
@@ -10764,14 +10770,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class APISpec(API):
     """Description"""
 
+    type_name: str = Field("APISpec", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "APISpec":
+            raise ValueError("must be APISpec")
+        return v
+
     def __setattr__(self, name, value):
         if name in APISpec._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "api_spec_terms_of_service_url",
@@ -10889,22 +10903,14 @@
 
     @api_paths.setter
     def api_paths(self, api_paths: Optional[list[APIPath]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_paths = api_paths
 
-    type_name: str = Field("APISpec", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "APISpec":
-            raise ValueError("must be APISpec")
-        return v
-
     class Attributes(API.Attributes):
         api_spec_terms_of_service_url: Optional[str] = Field(
             None, description="", alias="apiSpecTermsOfServiceURL"
         )
         api_spec_contact_email: Optional[str] = Field(
             None, description="", alias="apiSpecContactEmail"
         )
@@ -10936,14 +10942,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class APIPath(API):
     """Description"""
 
+    type_name: str = Field("APIPath", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "APIPath":
+            raise ValueError("must be APIPath")
+        return v
+
     def __setattr__(self, name, value):
         if name in APIPath._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "api_path_summary",
@@ -11041,22 +11055,14 @@
 
     @api_spec.setter
     def api_spec(self, api_spec: Optional[APISpec]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec = api_spec
 
-    type_name: str = Field("APIPath", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "APIPath":
-            raise ValueError("must be APIPath")
-        return v
-
     class Attributes(API.Attributes):
         api_path_summary: Optional[str] = Field(
             None, description="", alias="apiPathSummary"
         )
         api_path_raw_u_r_i: Optional[str] = Field(
             None, description="", alias="apiPathRawURI"
         )
@@ -11082,24 +11088,32 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SnowflakeTag(Tag):
     """Description"""
 
+    type_name: str = Field("SnowflakeTag", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SnowflakeTag":
+            raise ValueError("must be SnowflakeTag")
+        return v
+
     def __setattr__(self, name, value):
         if name in SnowflakeTag._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "tag_id",
         "tag_attributes",
         "tag_allowed_values",
-        "mapped_classification_name",
+        "mapped_atlan_tag_name",
         "query_count",
         "query_user_count",
         "query_user_map",
         "query_count_updated_at",
         "database_name",
         "database_qualified_name",
         "schema_name",
@@ -11144,26 +11158,24 @@
     @tag_allowed_values.setter
     def tag_allowed_values(self, tag_allowed_values: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tag_allowed_values = tag_allowed_values
 
     @property
-    def mapped_classification_name(self) -> Optional[str]:
+    def mapped_atlan_tag_name(self) -> Optional[str]:
         return (
-            None
-            if self.attributes is None
-            else self.attributes.mapped_classification_name
+            None if self.attributes is None else self.attributes.mapped_atlan_tag_name
         )
 
-    @mapped_classification_name.setter
-    def mapped_classification_name(self, mapped_classification_name: Optional[str]):
+    @mapped_atlan_tag_name.setter
+    def mapped_atlan_tag_name(self, mapped_atlan_tag_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.mapped_classification_name = mapped_classification_name
+        self.attributes.mapped_atlan_tag_name = mapped_atlan_tag_name
 
     @property
     def query_count(self) -> Optional[int]:
         return None if self.attributes is None else self.attributes.query_count
 
     @query_count.setter
     def query_count(self, query_count: Optional[int]):
@@ -11353,31 +11365,23 @@
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
-    type_name: str = Field("SnowflakeTag", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SnowflakeTag":
-            raise ValueError("must be SnowflakeTag")
-        return v
-
     class Attributes(Tag.Attributes):
         tag_id: Optional[str] = Field(None, description="", alias="tagId")
         tag_attributes: Optional[list[SourceTagAttribute]] = Field(
             None, description="", alias="tagAttributes"
         )
         tag_allowed_values: Optional[set[str]] = Field(
             None, description="", alias="tagAllowedValues"
         )
-        mapped_classification_name: Optional[str] = Field(
+        mapped_atlan_tag_name: Optional[str] = Field(
             None, description="", alias="mappedClassificationName"
         )
         query_count: Optional[int] = Field(None, description="", alias="queryCount")
         query_user_count: Optional[int] = Field(
             None, description="", alias="queryUserCount"
         )
         query_user_map: Optional[dict[str, int]] = Field(
@@ -11428,14 +11432,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TablePartition(SQL):
     """Description"""
 
+    type_name: str = Field("TablePartition", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TablePartition":
+            raise ValueError("must be TablePartition")
+        return v
+
     def __setattr__(self, name, value):
         if name in TablePartition._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "constraint",
@@ -11631,22 +11643,14 @@
 
     @parent_table.setter
     def parent_table(self, parent_table: Optional[Table]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.parent_table = parent_table
 
-    type_name: str = Field("TablePartition", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TablePartition":
-            raise ValueError("must be TablePartition")
-        return v
-
     class Attributes(SQL.Attributes):
         constraint: Optional[str] = Field(None, description="", alias="constraint")
         column_count: Optional[int] = Field(None, description="", alias="columnCount")
         row_count: Optional[int] = Field(None, description="", alias="rowCount")
         size_bytes: Optional[int] = Field(None, description="", alias="sizeBytes")
         alias: Optional[str] = Field(None, description="", alias="alias")
         is_temporary: Optional[bool] = Field(None, description="", alias="isTemporary")
@@ -11690,14 +11694,33 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Table(SQL):
     """Description"""
 
+    @classmethod
+    # @validate_arguments()
+    def create(cls, *, name: str, schema_qualified_name: str) -> Table:
+        validate_required_fields(
+            ["name", "schema_qualified_name"], [name, schema_qualified_name]
+        )
+        attributes = Table.Attributes.create(
+            name=name, schema_qualified_name=schema_qualified_name
+        )
+        return cls(attributes=attributes)
+
+    type_name: str = Field("Table", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Table":
+            raise ValueError("must be Table")
+        return v
+
     def __setattr__(self, name, value):
         if name in Table._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "column_count",
@@ -11926,22 +11949,14 @@
 
     @dimensions.setter
     def dimensions(self, dimensions: Optional[list[Table]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dimensions = dimensions
 
-    type_name: str = Field("Table", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Table":
-            raise ValueError("must be Table")
-        return v
-
     class Attributes(SQL.Attributes):
         column_count: Optional[int] = Field(None, description="", alias="columnCount")
         row_count: Optional[int] = Field(None, description="", alias="rowCount")
         size_bytes: Optional[int] = Field(None, description="", alias="sizeBytes")
         alias: Optional[str] = Field(None, description="", alias="alias")
         is_temporary: Optional[bool] = Field(None, description="", alias="isTemporary")
         is_query_preview: Optional[bool] = Field(
@@ -12017,29 +12032,26 @@
 
     attributes: "Table.Attributes" = Field(
         default_factory=lambda: Table.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
-    @classmethod
-    # @validate_arguments()
-    def create(cls, *, name: str, schema_qualified_name: str) -> Table:
-        validate_required_fields(
-            ["name", "schema_qualified_name"], [name, schema_qualified_name]
-        )
-        attributes = Table.Attributes.create(
-            name=name, schema_qualified_name=schema_qualified_name
-        )
-        return cls(attributes=attributes)
-
 
 class Query(SQL):
     """Description"""
 
+    type_name: str = Field("Query", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Query":
+            raise ValueError("must be Query")
+        return v
+
     def __setattr__(self, name, value):
         if name in Query._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "raw_query",
@@ -12220,22 +12232,14 @@
 
     @views.setter
     def views(self, views: Optional[list[View]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.views = views
 
-    type_name: str = Field("Query", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Query":
-            raise ValueError("must be Query")
-        return v
-
     class Attributes(SQL.Attributes):
         raw_query: Optional[str] = Field(None, description="", alias="rawQuery")
         default_schema_qualified_name: Optional[str] = Field(
             None, description="", alias="defaultSchemaQualifiedName"
         )
         default_database_qualified_name: Optional[str] = Field(
             None, description="", alias="defaultDatabaseQualifiedName"
@@ -12276,25 +12280,45 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Column(SQL):
     """Description"""
 
+    @classmethod
+    # @validate_arguments()
+    def create(
+        cls, *, name: str, parent_qualified_name: str, parent_type: type, order: int
+    ) -> Column:
+        return Column(
+            attributes=Column.Attributes.create(
+                name=name,
+                parent_qualified_name=parent_qualified_name,
+                parent_type=parent_type,
+                order=order,
+            )
+        )
+
+    type_name: str = Field("Column", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Column":
+            raise ValueError("must be Column")
+        return v
+
     def __setattr__(self, name, value):
         if name in Column._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "data_type",
         "sub_data_type",
-        "raw_data_type_definition",
         "order",
-        "nested_column_count",
         "is_partition",
         "partition_order",
         "is_clustered",
         "is_primary",
         "is_foreign",
         "is_indexed",
         "is_sort",
@@ -12304,16 +12328,14 @@
         "pinned_at",
         "precision",
         "default_value",
         "is_nullable",
         "numeric_scale",
         "max_length",
         "validations",
-        "parent_column_qualified_name",
-        "parent_column_name",
         "column_distinct_values_count",
         "column_distinct_values_count_long",
         "column_histogram",
         "column_max",
         "column_min",
         "column_mean",
         "column_sum",
@@ -12331,23 +12353,20 @@
         "column_mins",
         "column_missing_values_count",
         "column_missing_values_count_long",
         "column_missing_values_percentage",
         "column_uniqueness_percentage",
         "column_variance",
         "column_top_values",
-        "column_depth_level",
         "view",
-        "nested_columns",
         "data_quality_metric_dimensions",
         "dbt_model_columns",
         "table",
         "column_dbt_model_columns",
         "materialised_view",
-        "parent_column",
         "queries",
         "metric_timestamps",
         "foreign_key_to",
         "foreign_key_from",
         "dbt_metrics",
         "table_partition",
     ]
@@ -12369,48 +12388,24 @@
     @sub_data_type.setter
     def sub_data_type(self, sub_data_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sub_data_type = sub_data_type
 
     @property
-    def raw_data_type_definition(self) -> Optional[str]:
-        return (
-            None
-            if self.attributes is None
-            else self.attributes.raw_data_type_definition
-        )
-
-    @raw_data_type_definition.setter
-    def raw_data_type_definition(self, raw_data_type_definition: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.raw_data_type_definition = raw_data_type_definition
-
-    @property
     def order(self) -> Optional[int]:
         return None if self.attributes is None else self.attributes.order
 
     @order.setter
     def order(self, order: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.order = order
 
     @property
-    def nested_column_count(self) -> Optional[int]:
-        return None if self.attributes is None else self.attributes.nested_column_count
-
-    @nested_column_count.setter
-    def nested_column_count(self, nested_column_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.nested_column_count = nested_column_count
-
-    @property
     def is_partition(self) -> Optional[bool]:
         return None if self.attributes is None else self.attributes.is_partition
 
     @is_partition.setter
     def is_partition(self, is_partition: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -12573,38 +12568,14 @@
     @validations.setter
     def validations(self, validations: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.validations = validations
 
     @property
-    def parent_column_qualified_name(self) -> Optional[str]:
-        return (
-            None
-            if self.attributes is None
-            else self.attributes.parent_column_qualified_name
-        )
-
-    @parent_column_qualified_name.setter
-    def parent_column_qualified_name(self, parent_column_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.parent_column_qualified_name = parent_column_qualified_name
-
-    @property
-    def parent_column_name(self) -> Optional[str]:
-        return None if self.attributes is None else self.attributes.parent_column_name
-
-    @parent_column_name.setter
-    def parent_column_name(self, parent_column_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.parent_column_name = parent_column_name
-
-    @property
     def column_distinct_values_count(self) -> Optional[int]:
         return (
             None
             if self.attributes is None
             else self.attributes.column_distinct_values_count
         )
 
@@ -12927,44 +12898,24 @@
         self, column_top_values: Optional[list[ColumnValueFrequencyMap]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_top_values = column_top_values
 
     @property
-    def column_depth_level(self) -> Optional[int]:
-        return None if self.attributes is None else self.attributes.column_depth_level
-
-    @column_depth_level.setter
-    def column_depth_level(self, column_depth_level: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.column_depth_level = column_depth_level
-
-    @property
     def view(self) -> Optional[View]:
         return None if self.attributes is None else self.attributes.view
 
     @view.setter
     def view(self, view: Optional[View]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.view = view
 
     @property
-    def nested_columns(self) -> Optional[list[Column]]:
-        return None if self.attributes is None else self.attributes.nested_columns
-
-    @nested_columns.setter
-    def nested_columns(self, nested_columns: Optional[list[Column]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.nested_columns = nested_columns
-
-    @property
     def data_quality_metric_dimensions(self) -> Optional[list[Metric]]:
         return (
             None
             if self.attributes is None
             else self.attributes.data_quality_metric_dimensions
         )
 
@@ -13019,24 +12970,14 @@
     @materialised_view.setter
     def materialised_view(self, materialised_view: Optional[MaterialisedView]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.materialised_view = materialised_view
 
     @property
-    def parent_column(self) -> Optional[Column]:
-        return None if self.attributes is None else self.attributes.parent_column
-
-    @parent_column.setter
-    def parent_column(self, parent_column: Optional[Column]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.parent_column = parent_column
-
-    @property
     def queries(self) -> Optional[list[Query]]:
         return None if self.attributes is None else self.attributes.queries
 
     @queries.setter
     def queries(self, queries: Optional[list[Query]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -13088,32 +13029,18 @@
 
     @table_partition.setter
     def table_partition(self, table_partition: Optional[TablePartition]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.table_partition = table_partition
 
-    type_name: str = Field("Column", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Column":
-            raise ValueError("must be Column")
-        return v
-
     class Attributes(SQL.Attributes):
         data_type: Optional[str] = Field(None, description="", alias="dataType")
         sub_data_type: Optional[str] = Field(None, description="", alias="subDataType")
-        raw_data_type_definition: Optional[str] = Field(
-            None, description="", alias="rawDataTypeDefinition"
-        )
         order: Optional[int] = Field(None, description="", alias="order")
-        nested_column_count: Optional[int] = Field(
-            None, description="", alias="nestedColumnCount"
-        )
         is_partition: Optional[bool] = Field(None, description="", alias="isPartition")
         partition_order: Optional[int] = Field(
             None, description="", alias="partitionOrder"
         )
         is_clustered: Optional[bool] = Field(None, description="", alias="isClustered")
         is_primary: Optional[bool] = Field(None, description="", alias="isPrimary")
         is_foreign: Optional[bool] = Field(None, description="", alias="isForeign")
@@ -13129,20 +13056,14 @@
         numeric_scale: Optional[float] = Field(
             None, description="", alias="numericScale"
         )
         max_length: Optional[int] = Field(None, description="", alias="maxLength")
         validations: Optional[dict[str, str]] = Field(
             None, description="", alias="validations"
         )
-        parent_column_qualified_name: Optional[str] = Field(
-            None, description="", alias="parentColumnQualifiedName"
-        )
-        parent_column_name: Optional[str] = Field(
-            None, description="", alias="parentColumnName"
-        )
         column_distinct_values_count: Optional[int] = Field(
             None, description="", alias="columnDistinctValuesCount"
         )
         column_distinct_values_count_long: Optional[int] = Field(
             None, description="", alias="columnDistinctValuesCountLong"
         )
         column_histogram: Optional[Histogram] = Field(
@@ -13202,21 +13123,15 @@
         )
         column_variance: Optional[float] = Field(
             None, description="", alias="columnVariance"
         )
         column_top_values: Optional[list[ColumnValueFrequencyMap]] = Field(
             None, description="", alias="columnTopValues"
         )
-        column_depth_level: Optional[int] = Field(
-            None, description="", alias="columnDepthLevel"
-        )
         view: Optional[View] = Field(None, description="", alias="view")  # relationship
-        nested_columns: Optional[list[Column]] = Field(
-            None, description="", alias="nestedColumns"
-        )  # relationship
         data_quality_metric_dimensions: Optional[list[Metric]] = Field(
             None, description="", alias="dataQualityMetricDimensions"
         )  # relationship
         dbt_model_columns: Optional[list[DbtModelColumn]] = Field(
             None, description="", alias="dbtModelColumns"
         )  # relationship
         table: Optional[Table] = Field(
@@ -13224,17 +13139,14 @@
         )  # relationship
         column_dbt_model_columns: Optional[list[DbtModelColumn]] = Field(
             None, description="", alias="columnDbtModelColumns"
         )  # relationship
         materialised_view: Optional[MaterialisedView] = Field(
             None, description="", alias="materialisedView"
         )  # relationship
-        parent_column: Optional[Column] = Field(
-            None, description="", alias="parentColumn"
-        )  # relationship
         queries: Optional[list[Query]] = Field(
             None, description="", alias="queries"
         )  # relationship
         metric_timestamps: Optional[list[Metric]] = Field(
             None, description="", alias="metricTimestamps"
         )  # relationship
         foreign_key_to: Optional[list[Column]] = Field(
@@ -13295,38 +13207,43 @@
                 ret_value.view_name = fields[5]
             else:
                 raise ValueError(
                     "parent_type must be either Table, View or MaterializeView"
                 )
             return ret_value
 
-    @classmethod
-    # @validate_arguments()
-    def create(
-        cls, *, name: str, parent_qualified_name: str, parent_type: type, order: int
-    ) -> Column:
-        return Column(
-            attributes=Column.Attributes.create(
-                name=name,
-                parent_qualified_name=parent_qualified_name,
-                parent_type=parent_type,
-                order=order,
-            )
-        )
-
     attributes: "Column.Attributes" = Field(
         default_factory=lambda: Column.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Schema(SQL):
     """Description"""
 
+    @classmethod
+    # @validate_arguments()
+    def create(cls, *, name: str, database_qualified_name: str) -> Schema:
+        validate_required_fields(
+            ["name", "database_qualified_name"], [name, database_qualified_name]
+        )
+        attributes = Schema.Attributes.create(
+            name=name, database_qualified_name=database_qualified_name
+        )
+        return cls(attributes=attributes)
+
+    type_name: str = Field("Schema", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Schema":
+            raise ValueError("must be Schema")
+        return v
+
     def __setattr__(self, name, value):
         if name in Schema._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "table_count",
@@ -13437,22 +13354,14 @@
 
     @views.setter
     def views(self, views: Optional[list[View]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.views = views
 
-    type_name: str = Field("Schema", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Schema":
-            raise ValueError("must be Schema")
-        return v
-
     class Attributes(SQL.Attributes):
         table_count: Optional[int] = Field(None, description="", alias="tableCount")
         views_count: Optional[int] = Field(None, description="", alias="viewsCount")
         snowflake_tags: Optional[list[SnowflakeTag]] = Field(
             None, description="", alias="snowflakeTags"
         )  # relationship
         materialised_views: Optional[list[MaterialisedView]] = Field(
@@ -13506,29 +13415,26 @@
 
     attributes: "Schema.Attributes" = Field(
         default_factory=lambda: Schema.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
-    @classmethod
-    # @validate_arguments()
-    def create(cls, *, name: str, database_qualified_name: str) -> Schema:
-        validate_required_fields(
-            ["name", "database_qualified_name"], [name, database_qualified_name]
-        )
-        attributes = Schema.Attributes.create(
-            name=name, database_qualified_name=database_qualified_name
-        )
-        return cls(attributes=attributes)
-
 
 class SnowflakeStream(SQL):
     """Description"""
 
+    type_name: str = Field("SnowflakeStream", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SnowflakeStream":
+            raise ValueError("must be SnowflakeStream")
+        return v
+
     def __setattr__(self, name, value):
         if name in SnowflakeStream._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "snowflake_stream_type",
@@ -13613,22 +13519,14 @@
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
-    type_name: str = Field("SnowflakeStream", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SnowflakeStream":
-            raise ValueError("must be SnowflakeStream")
-        return v
-
     class Attributes(SQL.Attributes):
         snowflake_stream_type: Optional[str] = Field(
             None, description="", alias="snowflakeStreamType"
         )
         snowflake_stream_source_type: Optional[str] = Field(
             None, description="", alias="snowflakeStreamSourceType"
         )
@@ -13651,14 +13549,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SnowflakePipe(SQL):
     """Description"""
 
+    type_name: str = Field("SnowflakePipe", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SnowflakePipe":
+            raise ValueError("must be SnowflakePipe")
+        return v
+
     def __setattr__(self, name, value):
         if name in SnowflakePipe._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "definition",
@@ -13719,22 +13625,14 @@
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
-    type_name: str = Field("SnowflakePipe", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SnowflakePipe":
-            raise ValueError("must be SnowflakePipe")
-        return v
-
     class Attributes(SQL.Attributes):
         definition: Optional[str] = Field(None, description="", alias="definition")
         snowflake_pipe_is_auto_ingest_enabled: Optional[bool] = Field(
             None, description="", alias="snowflakePipeIsAutoIngestEnabled"
         )
         snowflake_pipe_notification_channel_name: Optional[str] = Field(
             None, description="", alias="snowflakePipeNotificationChannelName"
@@ -13749,14 +13647,43 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Database(SQL):
     """Description"""
 
+    @classmethod
+    # @validate_arguments()
+    def create(cls, *, name: str, connection_qualified_name: str) -> Database:
+        validate_required_fields(
+            ["name", "connection_qualified_name"], [name, connection_qualified_name]
+        )
+        fields = connection_qualified_name.split("/")
+        if len(fields) != 3:
+            raise ValueError("Invalid connection_qualified_name")
+        try:
+            connector_type = AtlanConnectorType(fields[1])  # type:ignore
+        except ValueError as e:
+            raise ValueError("Invalid connection_qualified_name") from e
+        attributes = Database.Attributes(
+            name=name,
+            connection_qualified_name=connection_qualified_name,
+            qualified_name=f"{connection_qualified_name}/{name}",
+            connector_name=connector_type.value,
+        )
+        return cls(attributes=attributes)
+
+    type_name: str = Field("Database", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Database":
+            raise ValueError("must be Database")
+        return v
+
     def __setattr__(self, name, value):
         if name in Database._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "schema_count",
@@ -13779,37 +13706,27 @@
 
     @schemas.setter
     def schemas(self, schemas: Optional[list[Schema]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.schemas = schemas
 
-    type_name: str = Field("Database", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Database":
-            raise ValueError("must be Database")
-        return v
-
     class Attributes(SQL.Attributes):
         schema_count: Optional[int] = Field(None, description="", alias="schemaCount")
         schemas: Optional[list[Schema]] = Field(
             None, description="", alias="schemas"
         )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls, name: str, connection_qualified_name: str
         ) -> Database.Attributes:
-            if not name:
-                raise ValueError("name cannot be blank")
             validate_required_fields(
-                ["connection_qualified_name"], [connection_qualified_name]
+                ["name", "connection_qualified_name"], [name, connection_qualified_name]
             )
             fields = connection_qualified_name.split("/")
             if len(fields) != 3:
                 raise ValueError("Invalid connection_qualified_name")
             try:
                 connector_type = AtlanConnectorType(fields[1])  # type:ignore
             except ValueError as e:
@@ -13823,41 +13740,26 @@
 
     attributes: "Database.Attributes" = Field(
         default_factory=lambda: Database.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
-    @classmethod
-    # @validate_arguments()
-    def create(cls, *, name: str, connection_qualified_name: str) -> Database:
-        if not name:
-            raise ValueError("name cannot be blank")
-        validate_required_fields(
-            ["connection_qualified_name"], [connection_qualified_name]
-        )
-        fields = connection_qualified_name.split("/")
-        if len(fields) != 3:
-            raise ValueError("Invalid connection_qualified_name")
-        try:
-            connector_type = AtlanConnectorType(fields[1])  # type:ignore
-        except ValueError as e:
-            raise ValueError("Invalid connection_qualified_name") from e
-        attributes = Database.Attributes(
-            name=name,
-            connection_qualified_name=connection_qualified_name,
-            qualified_name=f"{connection_qualified_name}/{name}",
-            connector_name=connector_type.value,
-        )
-        return cls(attributes=attributes)
-
 
 class Procedure(SQL):
     """Description"""
 
+    type_name: str = Field("Procedure", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Procedure":
+            raise ValueError("must be Procedure")
+        return v
+
     def __setattr__(self, name, value):
         if name in Procedure._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "definition",
@@ -13880,22 +13782,14 @@
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
-    type_name: str = Field("Procedure", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Procedure":
-            raise ValueError("must be Procedure")
-        return v
-
     class Attributes(SQL.Attributes):
         definition: str = Field(None, description="", alias="definition")
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
 
     attributes: "Procedure.Attributes" = Field(
@@ -13904,14 +13798,33 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class View(SQL):
     """Description"""
 
+    @classmethod
+    # @validate_arguments()
+    def create(cls, *, name: str, schema_qualified_name: str) -> View:
+        validate_required_fields(
+            ["name", "schema_qualified_name"], [name, schema_qualified_name]
+        )
+        attributes = View.Attributes.create(
+            name=name, schema_qualified_name=schema_qualified_name
+        )
+        return cls(attributes=attributes)
+
+    type_name: str = Field("View", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "View":
+            raise ValueError("must be View")
+        return v
+
     def __setattr__(self, name, value):
         if name in View._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "column_count",
@@ -14033,22 +13946,14 @@
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
-    type_name: str = Field("View", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "View":
-            raise ValueError("must be View")
-        return v
-
     class Attributes(SQL.Attributes):
         column_count: Optional[int] = Field(None, description="", alias="columnCount")
         row_count: Optional[int] = Field(None, description="", alias="rowCount")
         size_bytes: Optional[int] = Field(None, description="", alias="sizeBytes")
         is_query_preview: Optional[bool] = Field(
             None, description="", alias="isQueryPreview"
         )
@@ -14095,28 +14000,36 @@
 
     attributes: "View.Attributes" = Field(
         default_factory=lambda: View.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+
+class MaterialisedView(SQL):
+    """Description"""
+
     @classmethod
     # @validate_arguments()
-    def create(cls, *, name: str, schema_qualified_name: str) -> View:
+    def create(cls, *, name: str, schema_qualified_name: str) -> MaterialisedView:
         validate_required_fields(
             ["name", "schema_qualified_name"], [name, schema_qualified_name]
         )
-        attributes = View.Attributes.create(
+        attributes = MaterialisedView.Attributes.create(
             name=name, schema_qualified_name=schema_qualified_name
         )
         return cls(attributes=attributes)
 
+    type_name: str = Field("MaterialisedView", allow_mutation=False)
 
-class MaterialisedView(SQL):
-    """Description"""
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MaterialisedView":
+            raise ValueError("must be MaterialisedView")
+        return v
 
     def __setattr__(self, name, value):
         if name in MaterialisedView._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
@@ -14272,22 +14185,14 @@
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
-    type_name: str = Field("MaterialisedView", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MaterialisedView":
-            raise ValueError("must be MaterialisedView")
-        return v
-
     class Attributes(SQL.Attributes):
         refresh_mode: Optional[str] = Field(None, description="", alias="refreshMode")
         refresh_method: Optional[str] = Field(
             None, description="", alias="refreshMethod"
         )
         staleness: Optional[str] = Field(None, description="", alias="staleness")
         stale_since_date: Optional[datetime] = Field(
@@ -14341,29 +14246,26 @@
 
     attributes: "MaterialisedView.Attributes" = Field(
         default_factory=lambda: MaterialisedView.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
-    @classmethod
-    # @validate_arguments()
-    def create(cls, *, name: str, schema_qualified_name: str) -> MaterialisedView:
-        validate_required_fields(
-            ["name", "schema_qualified_name"], [name, schema_qualified_name]
-        )
-        attributes = MaterialisedView.Attributes.create(
-            name=name, schema_qualified_name=schema_qualified_name
-        )
-        return cls(attributes=attributes)
-
 
 class DataStudioAsset(DataStudio):
     """Description"""
 
+    type_name: str = Field("DataStudioAsset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "DataStudioAsset":
+            raise ValueError("must be DataStudioAsset")
+        return v
+
     def __setattr__(self, name, value):
         if name in DataStudioAsset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "data_studio_asset_type",
@@ -14512,22 +14414,14 @@
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
-    type_name: str = Field("DataStudioAsset", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "DataStudioAsset":
-            raise ValueError("must be DataStudioAsset")
-        return v
-
     class Attributes(DataStudio.Attributes):
         data_studio_asset_type: Optional[GoogleDatastudioAssetType] = Field(
             None, description="", alias="dataStudioAssetType"
         )
         data_studio_asset_title: Optional[str] = Field(
             None, description="", alias="dataStudioAssetTitle"
         )
@@ -14568,14 +14462,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class KafkaTopic(Kafka):
     """Description"""
 
+    type_name: str = Field("KafkaTopic", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "KafkaTopic":
+            raise ValueError("must be KafkaTopic")
+        return v
+
     def __setattr__(self, name, value):
         if name in KafkaTopic._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "kafka_topic_is_internal",
@@ -14715,22 +14617,14 @@
     def kafka_consumer_groups(
         self, kafka_consumer_groups: Optional[list[KafkaConsumerGroup]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_consumer_groups = kafka_consumer_groups
 
-    type_name: str = Field("KafkaTopic", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "KafkaTopic":
-            raise ValueError("must be KafkaTopic")
-        return v
-
     class Attributes(Kafka.Attributes):
         kafka_topic_is_internal: Optional[bool] = Field(
             None, description="", alias="kafkaTopicIsInternal"
         )
         kafka_topic_compression_type: Optional[KafkaTopicCompressionType] = Field(
             None, description="", alias="kafkaTopicCompressionType"
         )
@@ -14762,14 +14656,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class KafkaConsumerGroup(Kafka):
     """Description"""
 
+    type_name: str = Field("KafkaConsumerGroup", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "KafkaConsumerGroup":
+            raise ValueError("must be KafkaConsumerGroup")
+        return v
+
     def __setattr__(self, name, value):
         if name in KafkaConsumerGroup._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "kafka_consumer_group_topic_consumption_properties",
@@ -14852,22 +14754,14 @@
 
     @kafka_topics.setter
     def kafka_topics(self, kafka_topics: Optional[list[KafkaTopic]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topics = kafka_topics
 
-    type_name: str = Field("KafkaConsumerGroup", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "KafkaConsumerGroup":
-            raise ValueError("must be KafkaConsumerGroup")
-        return v
-
     class Attributes(Kafka.Attributes):
         kafka_consumer_group_topic_consumption_properties: Optional[
             list[KafkaTopicConsumption]
         ] = Field(
             None, description="", alias="kafkaConsumerGroupTopicConsumptionProperties"
         )
         kafka_consumer_group_member_count: Optional[int] = Field(
@@ -14889,14 +14783,38 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class S3Bucket(S3):
     """Description"""
 
+    @classmethod
+    # @validate_arguments()
+    def create(
+        cls, *, name: str, connection_qualified_name: str, aws_arn: str
+    ) -> S3Bucket:
+        validate_required_fields(
+            ["name", "connection_qualified_name", "aws_arn"],
+            [name, connection_qualified_name, aws_arn],
+        )
+        attributes = S3Bucket.Attributes.create(
+            name=name,
+            connection_qualified_name=connection_qualified_name,
+            aws_arn=aws_arn,
+        )
+        return cls(attributes=attributes)
+
+    type_name: str = Field("S3Bucket", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "S3Bucket":
+            raise ValueError("must be S3Bucket")
+        return v
+
     def __setattr__(self, name, value):
         if name in S3Bucket._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "s3_object_count",
@@ -14936,22 +14854,14 @@
 
     @objects.setter
     def objects(self, objects: Optional[list[S3Object]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.objects = objects
 
-    type_name: str = Field("S3Bucket", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "S3Bucket":
-            raise ValueError("must be S3Bucket")
-        return v
-
     class Attributes(S3.Attributes):
         s3_object_count: Optional[int] = Field(
             None, description="", alias="s3ObjectCount"
         )
         s3_bucket_versioning_enabled: Optional[bool] = Field(
             None, description="", alias="s3BucketVersioningEnabled"
         )
@@ -14989,33 +14899,47 @@
 
     attributes: "S3Bucket.Attributes" = Field(
         default_factory=lambda: S3Bucket.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+
+class S3Object(S3):
+    """Description"""
+
     @classmethod
     # @validate_arguments()
     def create(
-        cls, *, name: str, connection_qualified_name: str, aws_arn: str
-    ) -> S3Bucket:
+        cls,
+        *,
+        name: str,
+        connection_qualified_name: str,
+        aws_arn: str,
+        s3_bucket_qualified_name: Optional[str] = None,
+    ) -> S3Object:
         validate_required_fields(
             ["name", "connection_qualified_name", "aws_arn"],
             [name, connection_qualified_name, aws_arn],
         )
-        attributes = S3Bucket.Attributes.create(
+        attributes = S3Object.Attributes.create(
             name=name,
             connection_qualified_name=connection_qualified_name,
             aws_arn=aws_arn,
+            s3_bucket_qualified_name=s3_bucket_qualified_name,
         )
         return cls(attributes=attributes)
 
+    type_name: str = Field("S3Object", allow_mutation=False)
 
-class S3Object(S3):
-    """Description"""
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "S3Object":
+            raise ValueError("must be S3Object")
+        return v
 
     def __setattr__(self, name, value):
         if name in S3Object._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
@@ -15147,22 +15071,14 @@
 
     @bucket.setter
     def bucket(self, bucket: Optional[S3Bucket]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.bucket = bucket
 
-    type_name: str = Field("S3Object", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "S3Object":
-            raise ValueError("must be S3Object")
-        return v
-
     class Attributes(S3.Attributes):
         s3_object_last_modified_time: Optional[datetime] = Field(
             None, description="", alias="s3ObjectLastModifiedTime"
         )
         s3_bucket_name: Optional[str] = Field(
             None, description="", alias="s3BucketName"
         )
@@ -15225,40 +15141,26 @@
 
     attributes: "S3Object.Attributes" = Field(
         default_factory=lambda: S3Object.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
-    @classmethod
-    # @validate_arguments()
-    def create(
-        cls,
-        *,
-        name: str,
-        connection_qualified_name: str,
-        aws_arn: str,
-        s3_bucket_qualified_name: Optional[str] = None,
-    ) -> S3Object:
-        validate_required_fields(
-            ["name", "connection_qualified_name", "aws_arn"],
-            [name, connection_qualified_name, aws_arn],
-        )
-        attributes = S3Object.Attributes.create(
-            name=name,
-            connection_qualified_name=connection_qualified_name,
-            aws_arn=aws_arn,
-            s3_bucket_qualified_name=s3_bucket_qualified_name,
-        )
-        return cls(attributes=attributes)
-
 
 class ADLSAccount(ADLS):
     """Description"""
 
+    type_name: str = Field("ADLSAccount", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ADLSAccount":
+            raise ValueError("must be ADLSAccount")
+        return v
+
     def __setattr__(self, name, value):
         if name in ADLSAccount._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "adls_e_tag",
@@ -15416,22 +15318,14 @@
 
     @adls_containers.setter
     def adls_containers(self, adls_containers: Optional[list[ADLSContainer]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_containers = adls_containers
 
-    type_name: str = Field("ADLSAccount", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ADLSAccount":
-            raise ValueError("must be ADLSAccount")
-        return v
-
     class Attributes(ADLS.Attributes):
         adls_e_tag: Optional[str] = Field(None, description="", alias="adlsETag")
         adls_encryption_type: Optional[ADLSEncryptionTypes] = Field(
             None, description="", alias="adlsEncryptionType"
         )
         adls_account_resource_group: Optional[str] = Field(
             None, description="", alias="adlsAccountResourceGroup"
@@ -15467,14 +15361,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ADLSContainer(ADLS):
     """Description"""
 
+    type_name: str = Field("ADLSContainer", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ADLSContainer":
+            raise ValueError("must be ADLSContainer")
+        return v
+
     def __setattr__(self, name, value):
         if name in ADLSContainer._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "adls_container_url",
@@ -15591,22 +15493,14 @@
 
     @adls_account.setter
     def adls_account(self, adls_account: Optional[ADLSAccount]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account = adls_account
 
-    type_name: str = Field("ADLSContainer", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ADLSContainer":
-            raise ValueError("must be ADLSContainer")
-        return v
-
     class Attributes(ADLS.Attributes):
         adls_container_url: Optional[str] = Field(
             None, description="", alias="adlsContainerUrl"
         )
         adls_container_lease_state: Optional[ADLSLeaseState] = Field(
             None, description="", alias="adlsContainerLeaseState"
         )
@@ -15635,14 +15529,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ADLSObject(ADLS):
     """Description"""
 
+    type_name: str = Field("ADLSObject", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ADLSObject":
+            raise ValueError("must be ADLSObject")
+        return v
+
     def __setattr__(self, name, value):
         if name in ADLSObject._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "adls_object_url",
@@ -15909,22 +15811,14 @@
 
     @adls_container.setter
     def adls_container(self, adls_container: Optional[ADLSContainer]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_container = adls_container
 
-    type_name: str = Field("ADLSObject", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ADLSObject":
-            raise ValueError("must be ADLSObject")
-        return v
-
     class Attributes(ADLS.Attributes):
         adls_object_url: Optional[str] = Field(
             None, description="", alias="adlsObjectUrl"
         )
         adls_object_version_id: Optional[str] = Field(
             None, description="", alias="adlsObjectVersionId"
         )
@@ -15983,14 +15877,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class GCSObject(GCS):
     """Description"""
 
+    type_name: str = Field("GCSObject", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "GCSObject":
+            raise ValueError("must be GCSObject")
+        return v
+
     def __setattr__(self, name, value):
         if name in GCSObject._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "gcs_bucket_name",
@@ -16213,22 +16115,14 @@
 
     @gcs_bucket.setter
     def gcs_bucket(self, gcs_bucket: Optional[GCSBucket]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_bucket = gcs_bucket
 
-    type_name: str = Field("GCSObject", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "GCSObject":
-            raise ValueError("must be GCSObject")
-        return v
-
     class Attributes(GCS.Attributes):
         gcs_bucket_name: Optional[str] = Field(
             None, description="", alias="gcsBucketName"
         )
         gcs_bucket_qualified_name: Optional[str] = Field(
             None, description="", alias="gcsBucketQualifiedName"
         )
@@ -16281,14 +16175,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class GCSBucket(GCS):
     """Description"""
 
+    type_name: str = Field("GCSBucket", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "GCSBucket":
+            raise ValueError("must be GCSBucket")
+        return v
+
     def __setattr__(self, name, value):
         if name in GCSBucket._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "gcs_object_count",
@@ -16407,22 +16309,14 @@
 
     @gcs_objects.setter
     def gcs_objects(self, gcs_objects: Optional[list[GCSObject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_objects = gcs_objects
 
-    type_name: str = Field("GCSBucket", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "GCSBucket":
-            raise ValueError("must be GCSBucket")
-        return v
-
     class Attributes(GCS.Attributes):
         gcs_object_count: Optional[int] = Field(
             None, description="", alias="gcsObjectCount"
         )
         gcs_bucket_versioning_enabled: Optional[bool] = Field(
             None, description="", alias="gcsBucketVersioningEnabled"
         )
@@ -16451,14 +16345,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MCIncident(MonteCarlo):
     """Description"""
 
+    type_name: str = Field("MCIncident", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MCIncident":
+            raise ValueError("must be MCIncident")
+        return v
+
     def __setattr__(self, name, value):
         if name in MCIncident._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mc_incident_id",
@@ -16551,22 +16453,14 @@
 
     @mc_monitor.setter
     def mc_monitor(self, mc_monitor: Optional[MCMonitor]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor = mc_monitor
 
-    type_name: str = Field("MCIncident", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MCIncident":
-            raise ValueError("must be MCIncident")
-        return v
-
     class Attributes(MonteCarlo.Attributes):
         mc_incident_id: Optional[str] = Field(
             None, description="", alias="mcIncidentId"
         )
         mc_incident_type: Optional[str] = Field(
             None, description="", alias="mcIncidentType"
         )
@@ -16595,14 +16489,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MCMonitor(MonteCarlo):
     """Description"""
 
+    type_name: str = Field("MCMonitor", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MCMonitor":
+            raise ValueError("must be MCMonitor")
+        return v
+
     def __setattr__(self, name, value):
         if name in MCMonitor._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mc_monitor_id",
@@ -16861,22 +16763,14 @@
 
     @mc_monitor_assets.setter
     def mc_monitor_assets(self, mc_monitor_assets: Optional[list[Asset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_assets = mc_monitor_assets
 
-    type_name: str = Field("MCMonitor", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MCMonitor":
-            raise ValueError("must be MCMonitor")
-        return v
-
     class Attributes(MonteCarlo.Attributes):
         mc_monitor_id: Optional[str] = Field(None, description="", alias="mcMonitorId")
         mc_monitor_status: Optional[str] = Field(
             None, description="", alias="mcMonitorStatus"
         )
         mc_monitor_type: Optional[str] = Field(
             None, description="", alias="mcMonitorType"
@@ -16933,14 +16827,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PresetChart(Preset):
     """Description"""
 
+    type_name: str = Field("PresetChart", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PresetChart":
+            raise ValueError("must be PresetChart")
+        return v
+
     def __setattr__(self, name, value):
         if name in PresetChart._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "preset_chart_description_markdown",
@@ -16984,22 +16886,14 @@
 
     @preset_dashboard.setter
     def preset_dashboard(self, preset_dashboard: Optional[PresetDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard = preset_dashboard
 
-    type_name: str = Field("PresetChart", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PresetChart":
-            raise ValueError("must be PresetChart")
-        return v
-
     class Attributes(Preset.Attributes):
         preset_chart_description_markdown: Optional[str] = Field(
             None, description="", alias="presetChartDescriptionMarkdown"
         )
         preset_chart_form_data: Optional[dict[str, str]] = Field(
             None, description="", alias="presetChartFormData"
         )
@@ -17013,14 +16907,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PresetDataset(Preset):
     """Description"""
 
+    type_name: str = Field("PresetDataset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PresetDataset":
+            raise ValueError("must be PresetDataset")
+        return v
+
     def __setattr__(self, name, value):
         if name in PresetDataset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "preset_dataset_datasource_name",
@@ -17071,22 +16973,14 @@
 
     @preset_dashboard.setter
     def preset_dashboard(self, preset_dashboard: Optional[PresetDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard = preset_dashboard
 
-    type_name: str = Field("PresetDataset", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PresetDataset":
-            raise ValueError("must be PresetDataset")
-        return v
-
     class Attributes(Preset.Attributes):
         preset_dataset_datasource_name: Optional[str] = Field(
             None, description="", alias="presetDatasetDatasourceName"
         )
         preset_dataset_id: Optional[int] = Field(
             None, description="", alias="presetDatasetId"
         )
@@ -17103,14 +16997,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PresetDashboard(Preset):
     """Description"""
 
+    type_name: str = Field("PresetDashboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PresetDashboard":
+            raise ValueError("must be PresetDashboard")
+        return v
+
     def __setattr__(self, name, value):
         if name in PresetDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "preset_dashboard_changed_by_name",
@@ -17250,22 +17152,14 @@
 
     @preset_workspace.setter
     def preset_workspace(self, preset_workspace: Optional[PresetWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace = preset_workspace
 
-    type_name: str = Field("PresetDashboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PresetDashboard":
-            raise ValueError("must be PresetDashboard")
-        return v
-
     class Attributes(Preset.Attributes):
         preset_dashboard_changed_by_name: Optional[str] = Field(
             None, description="", alias="presetDashboardChangedByName"
         )
         preset_dashboard_changed_by_url: Optional[str] = Field(
             None, description="", alias="presetDashboardChangedByURL"
         )
@@ -17297,14 +17191,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PresetWorkspace(Preset):
     """Description"""
 
+    type_name: str = Field("PresetWorkspace", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PresetWorkspace":
+            raise ValueError("must be PresetWorkspace")
+        return v
+
     def __setattr__(self, name, value):
         if name in PresetWorkspace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "preset_workspace_public_dashboards_allowed",
@@ -17463,22 +17365,14 @@
 
     @preset_dashboards.setter
     def preset_dashboards(self, preset_dashboards: Optional[list[PresetDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboards = preset_dashboards
 
-    type_name: str = Field("PresetWorkspace", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PresetWorkspace":
-            raise ValueError("must be PresetWorkspace")
-        return v
-
     class Attributes(Preset.Attributes):
         preset_workspace_public_dashboards_allowed: Optional[bool] = Field(
             None, description="", alias="presetWorkspacePublicDashboardsAllowed"
         )
         preset_workspace_cluster_id: Optional[int] = Field(
             None, description="", alias="presetWorkspaceClusterId"
         )
@@ -17513,14 +17407,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ModeReport(Mode):
     """Description"""
 
+    type_name: str = Field("ModeReport", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ModeReport":
+            raise ValueError("must be ModeReport")
+        return v
+
     def __setattr__(self, name, value):
         if name in ModeReport._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_collection_token",
@@ -17626,22 +17528,14 @@
 
     @mode_queries.setter
     def mode_queries(self, mode_queries: Optional[list[ModeQuery]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_queries = mode_queries
 
-    type_name: str = Field("ModeReport", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ModeReport":
-            raise ValueError("must be ModeReport")
-        return v
-
     class Attributes(Mode.Attributes):
         mode_collection_token: Optional[str] = Field(
             None, description="", alias="modeCollectionToken"
         )
         mode_report_published_at: Optional[datetime] = Field(
             None, description="", alias="modeReportPublishedAt"
         )
@@ -17673,14 +17567,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ModeQuery(Mode):
     """Description"""
 
+    type_name: str = Field("ModeQuery", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ModeQuery":
+            raise ValueError("must be ModeQuery")
+        return v
+
     def __setattr__(self, name, value):
         if name in ModeQuery._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_raw_query",
@@ -17729,22 +17631,14 @@
 
     @mode_report.setter
     def mode_report(self, mode_report: Optional[ModeReport]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_report = mode_report
 
-    type_name: str = Field("ModeQuery", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ModeQuery":
-            raise ValueError("must be ModeQuery")
-        return v
-
     class Attributes(Mode.Attributes):
         mode_raw_query: Optional[str] = Field(
             None, description="", alias="modeRawQuery"
         )
         mode_report_import_count: Optional[int] = Field(
             None, description="", alias="modeReportImportCount"
         )
@@ -17761,14 +17655,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ModeChart(Mode):
     """Description"""
 
+    type_name: str = Field("ModeChart", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ModeChart":
+            raise ValueError("must be ModeChart")
+        return v
+
     def __setattr__(self, name, value):
         if name in ModeChart._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_chart_type",
@@ -17791,22 +17693,14 @@
 
     @mode_query.setter
     def mode_query(self, mode_query: Optional[ModeQuery]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_query = mode_query
 
-    type_name: str = Field("ModeChart", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ModeChart":
-            raise ValueError("must be ModeChart")
-        return v
-
     class Attributes(Mode.Attributes):
         mode_chart_type: Optional[str] = Field(
             None, description="", alias="modeChartType"
         )
         mode_query: Optional[ModeQuery] = Field(
             None, description="", alias="modeQuery"
         )  # relationship
@@ -17817,14 +17711,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ModeWorkspace(Mode):
     """Description"""
 
+    type_name: str = Field("ModeWorkspace", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ModeWorkspace":
+            raise ValueError("must be ModeWorkspace")
+        return v
+
     def __setattr__(self, name, value):
         if name in ModeWorkspace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_collection_count",
@@ -17849,22 +17751,14 @@
 
     @mode_collections.setter
     def mode_collections(self, mode_collections: Optional[list[ModeCollection]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_collections = mode_collections
 
-    type_name: str = Field("ModeWorkspace", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ModeWorkspace":
-            raise ValueError("must be ModeWorkspace")
-        return v
-
     class Attributes(Mode.Attributes):
         mode_collection_count: Optional[int] = Field(
             None, description="", alias="modeCollectionCount"
         )
         mode_collections: Optional[list[ModeCollection]] = Field(
             None, description="", alias="modeCollections"
         )  # relationship
@@ -17875,14 +17769,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ModeCollection(Mode):
     """Description"""
 
+    type_name: str = Field("ModeCollection", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ModeCollection":
+            raise ValueError("must be ModeCollection")
+        return v
+
     def __setattr__(self, name, value):
         if name in ModeCollection._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_collection_type",
@@ -17929,22 +17831,14 @@
 
     @mode_reports.setter
     def mode_reports(self, mode_reports: Optional[list[ModeReport]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_reports = mode_reports
 
-    type_name: str = Field("ModeCollection", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ModeCollection":
-            raise ValueError("must be ModeCollection")
-        return v
-
     class Attributes(Mode.Attributes):
         mode_collection_type: Optional[str] = Field(
             None, description="", alias="modeCollectionType"
         )
         mode_collection_state: Optional[str] = Field(
             None, description="", alias="modeCollectionState"
         )
@@ -17961,14 +17855,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SigmaDatasetColumn(Sigma):
     """Description"""
 
+    type_name: str = Field("SigmaDatasetColumn", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SigmaDatasetColumn":
+            raise ValueError("must be SigmaDatasetColumn")
+        return v
+
     def __setattr__(self, name, value):
         if name in SigmaDatasetColumn._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_dataset_qualified_name",
@@ -18006,22 +17908,14 @@
 
     @sigma_dataset.setter
     def sigma_dataset(self, sigma_dataset: Optional[SigmaDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_dataset = sigma_dataset
 
-    type_name: str = Field("SigmaDatasetColumn", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SigmaDatasetColumn":
-            raise ValueError("must be SigmaDatasetColumn")
-        return v
-
     class Attributes(Sigma.Attributes):
         sigma_dataset_qualified_name: Optional[str] = Field(
             None, description="", alias="sigmaDatasetQualifiedName"
         )
         sigma_dataset_name: Optional[str] = Field(
             None, description="", alias="sigmaDatasetName"
         )
@@ -18035,14 +17929,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SigmaDataset(Sigma):
     """Description"""
 
+    type_name: str = Field("SigmaDataset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SigmaDataset":
+            raise ValueError("must be SigmaDataset")
+        return v
+
     def __setattr__(self, name, value):
         if name in SigmaDataset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_dataset_column_count",
@@ -18073,22 +17975,14 @@
     def sigma_dataset_columns(
         self, sigma_dataset_columns: Optional[list[SigmaDatasetColumn]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_dataset_columns = sigma_dataset_columns
 
-    type_name: str = Field("SigmaDataset", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SigmaDataset":
-            raise ValueError("must be SigmaDataset")
-        return v
-
     class Attributes(Sigma.Attributes):
         sigma_dataset_column_count: Optional[int] = Field(
             None, description="", alias="sigmaDatasetColumnCount"
         )
         sigma_dataset_columns: Optional[list[SigmaDatasetColumn]] = Field(
             None, description="", alias="sigmaDatasetColumns"
         )  # relationship
@@ -18099,14 +17993,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SigmaWorkbook(Sigma):
     """Description"""
 
+    type_name: str = Field("SigmaWorkbook", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SigmaWorkbook":
+            raise ValueError("must be SigmaWorkbook")
+        return v
+
     def __setattr__(self, name, value):
         if name in SigmaWorkbook._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_page_count",
@@ -18129,22 +18031,14 @@
 
     @sigma_pages.setter
     def sigma_pages(self, sigma_pages: Optional[list[SigmaPage]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_pages = sigma_pages
 
-    type_name: str = Field("SigmaWorkbook", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SigmaWorkbook":
-            raise ValueError("must be SigmaWorkbook")
-        return v
-
     class Attributes(Sigma.Attributes):
         sigma_page_count: Optional[int] = Field(
             None, description="", alias="sigmaPageCount"
         )
         sigma_pages: Optional[list[SigmaPage]] = Field(
             None, description="", alias="sigmaPages"
         )  # relationship
@@ -18155,14 +18049,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SigmaDataElementField(Sigma):
     """Description"""
 
+    type_name: str = Field("SigmaDataElementField", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SigmaDataElementField":
+            raise ValueError("must be SigmaDataElementField")
+        return v
+
     def __setattr__(self, name, value):
         if name in SigmaDataElementField._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_data_element_field_is_hidden",
@@ -18212,22 +18114,14 @@
 
     @sigma_data_element.setter
     def sigma_data_element(self, sigma_data_element: Optional[SigmaDataElement]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element = sigma_data_element
 
-    type_name: str = Field("SigmaDataElementField", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SigmaDataElementField":
-            raise ValueError("must be SigmaDataElementField")
-        return v
-
     class Attributes(Sigma.Attributes):
         sigma_data_element_field_is_hidden: Optional[bool] = Field(
             None, description="", alias="sigmaDataElementFieldIsHidden"
         )
         sigma_data_element_field_formula: Optional[str] = Field(
             None, description="", alias="sigmaDataElementFieldFormula"
         )
@@ -18241,14 +18135,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SigmaPage(Sigma):
     """Description"""
 
+    type_name: str = Field("SigmaPage", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SigmaPage":
+            raise ValueError("must be SigmaPage")
+        return v
+
     def __setattr__(self, name, value):
         if name in SigmaPage._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_data_element_count",
@@ -18288,22 +18190,14 @@
 
     @sigma_workbook.setter
     def sigma_workbook(self, sigma_workbook: Optional[SigmaWorkbook]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_workbook = sigma_workbook
 
-    type_name: str = Field("SigmaPage", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SigmaPage":
-            raise ValueError("must be SigmaPage")
-        return v
-
     class Attributes(Sigma.Attributes):
         sigma_data_element_count: Optional[int] = Field(
             None, description="", alias="sigmaDataElementCount"
         )
         sigma_data_elements: Optional[list[SigmaDataElement]] = Field(
             None, description="", alias="sigmaDataElements"
         )  # relationship
@@ -18317,14 +18211,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SigmaDataElement(Sigma):
     """Description"""
 
+    type_name: str = Field("SigmaDataElement", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SigmaDataElement":
+            raise ValueError("must be SigmaDataElement")
+        return v
+
     def __setattr__(self, name, value):
         if name in SigmaDataElement._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_data_element_query",
@@ -18398,22 +18300,14 @@
     def sigma_data_element_fields(
         self, sigma_data_element_fields: Optional[list[SigmaDataElementField]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_fields = sigma_data_element_fields
 
-    type_name: str = Field("SigmaDataElement", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SigmaDataElement":
-            raise ValueError("must be SigmaDataElement")
-        return v
-
     class Attributes(Sigma.Attributes):
         sigma_data_element_query: Optional[str] = Field(
             None, description="", alias="sigmaDataElementQuery"
         )
         sigma_data_element_type: Optional[str] = Field(
             None, description="", alias="sigmaDataElementType"
         )
@@ -18433,14 +18327,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauWorkbook(Tableau):
     """Description"""
 
+    type_name: str = Field("TableauWorkbook", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TableauWorkbook":
+            raise ValueError("must be TableauWorkbook")
+        return v
+
     def __setattr__(self, name, value):
         if name in TableauWorkbook._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
@@ -18552,22 +18454,14 @@
 
     @datasources.setter
     def datasources(self, datasources: Optional[list[TableauDatasource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasources = datasources
 
-    type_name: str = Field("TableauWorkbook", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TableauWorkbook":
-            raise ValueError("must be TableauWorkbook")
-        return v
-
     class Attributes(Tableau.Attributes):
         site_qualified_name: Optional[str] = Field(
             None, description="", alias="siteQualifiedName"
         )
         project_qualified_name: Optional[str] = Field(
             None, description="", alias="projectQualifiedName"
         )
@@ -18599,14 +18493,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauDatasourceField(Tableau):
     """Description"""
 
+    type_name: str = Field("TableauDatasourceField", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TableauDatasourceField":
+            raise ValueError("must be TableauDatasourceField")
+        return v
+
     def __setattr__(self, name, value):
         if name in TableauDatasourceField._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
@@ -18861,22 +18763,14 @@
 
     @datasource.setter
     def datasource(self, datasource: Optional[TableauDatasource]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasource = datasource
 
-    type_name: str = Field("TableauDatasourceField", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TableauDatasourceField":
-            raise ValueError("must be TableauDatasourceField")
-        return v
-
     class Attributes(Tableau.Attributes):
         site_qualified_name: Optional[str] = Field(
             None, description="", alias="siteQualifiedName"
         )
         project_qualified_name: Optional[str] = Field(
             None, description="", alias="projectQualifiedName"
         )
@@ -18935,14 +18829,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauCalculatedField(Tableau):
     """Description"""
 
+    type_name: str = Field("TableauCalculatedField", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TableauCalculatedField":
+            raise ValueError("must be TableauCalculatedField")
+        return v
+
     def __setattr__(self, name, value):
         if name in TableauCalculatedField._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
@@ -19102,22 +19004,14 @@
 
     @datasource.setter
     def datasource(self, datasource: Optional[TableauDatasource]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasource = datasource
 
-    type_name: str = Field("TableauCalculatedField", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TableauCalculatedField":
-            raise ValueError("must be TableauCalculatedField")
-        return v
-
     class Attributes(Tableau.Attributes):
         site_qualified_name: Optional[str] = Field(
             None, description="", alias="siteQualifiedName"
         )
         project_qualified_name: Optional[str] = Field(
             None, description="", alias="projectQualifiedName"
         )
@@ -19155,14 +19049,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauProject(Tableau):
     """Description"""
 
+    type_name: str = Field("TableauProject", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TableauProject":
+            raise ValueError("must be TableauProject")
+        return v
+
     def __setattr__(self, name, value):
         if name in TableauProject._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
@@ -19281,22 +19183,14 @@
 
     @child_projects.setter
     def child_projects(self, child_projects: Optional[list[TableauProject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.child_projects = child_projects
 
-    type_name: str = Field("TableauProject", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TableauProject":
-            raise ValueError("must be TableauProject")
-        return v
-
     class Attributes(Tableau.Attributes):
         site_qualified_name: Optional[str] = Field(
             None, description="", alias="siteQualifiedName"
         )
         top_level_project_qualified_name: Optional[str] = Field(
             None, description="", alias="topLevelProjectQualifiedName"
         )
@@ -19331,14 +19225,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauMetric(Tableau):
     """Description"""
 
+    type_name: str = Field("TableauMetric", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TableauMetric":
+            raise ValueError("must be TableauMetric")
+        return v
+
     def __setattr__(self, name, value):
         if name in TableauMetric._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
@@ -19404,22 +19306,14 @@
 
     @project.setter
     def project(self, project: Optional[TableauProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project = project
 
-    type_name: str = Field("TableauMetric", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TableauMetric":
-            raise ValueError("must be TableauMetric")
-        return v
-
     class Attributes(Tableau.Attributes):
         site_qualified_name: Optional[str] = Field(
             None, description="", alias="siteQualifiedName"
         )
         project_qualified_name: Optional[str] = Field(
             None, description="", alias="projectQualifiedName"
         )
@@ -19439,14 +19333,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauSite(Tableau):
     """Description"""
 
+    type_name: str = Field("TableauSite", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TableauSite":
+            raise ValueError("must be TableauSite")
+        return v
+
     def __setattr__(self, name, value):
         if name in TableauSite._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "projects",
@@ -19458,22 +19360,14 @@
 
     @projects.setter
     def projects(self, projects: Optional[list[TableauProject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.projects = projects
 
-    type_name: str = Field("TableauSite", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TableauSite":
-            raise ValueError("must be TableauSite")
-        return v
-
     class Attributes(Tableau.Attributes):
         projects: Optional[list[TableauProject]] = Field(
             None, description="", alias="projects"
         )  # relationship
 
     attributes: "TableauSite.Attributes" = Field(
         default_factory=lambda: TableauSite.Attributes(),
@@ -19481,14 +19375,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauDatasource(Tableau):
     """Description"""
 
+    type_name: str = Field("TableauDatasource", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TableauDatasource":
+            raise ValueError("must be TableauDatasource")
+        return v
+
     def __setattr__(self, name, value):
         if name in TableauDatasource._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
@@ -19681,22 +19583,14 @@
 
     @fields.setter
     def fields(self, fields: Optional[list[TableauDatasourceField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
-    type_name: str = Field("TableauDatasource", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TableauDatasource":
-            raise ValueError("must be TableauDatasource")
-        return v
-
     class Attributes(Tableau.Attributes):
         site_qualified_name: Optional[str] = Field(
             None, description="", alias="siteQualifiedName"
         )
         project_qualified_name: Optional[str] = Field(
             None, description="", alias="projectQualifiedName"
         )
@@ -19743,14 +19637,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauDashboard(Tableau):
     """Description"""
 
+    type_name: str = Field("TableauDashboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TableauDashboard":
+            raise ValueError("must be TableauDashboard")
+        return v
+
     def __setattr__(self, name, value):
         if name in TableauDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
@@ -19840,22 +19742,14 @@
 
     @worksheets.setter
     def worksheets(self, worksheets: Optional[list[TableauWorksheet]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.worksheets = worksheets
 
-    type_name: str = Field("TableauDashboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TableauDashboard":
-            raise ValueError("must be TableauDashboard")
-        return v
-
     class Attributes(Tableau.Attributes):
         site_qualified_name: Optional[str] = Field(
             None, description="", alias="siteQualifiedName"
         )
         project_qualified_name: Optional[str] = Field(
             None, description="", alias="projectQualifiedName"
         )
@@ -19881,14 +19775,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauFlow(Tableau):
     """Description"""
 
+    type_name: str = Field("TableauFlow", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TableauFlow":
+            raise ValueError("must be TableauFlow")
+        return v
+
     def __setattr__(self, name, value):
         if name in TableauFlow._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
@@ -19987,22 +19889,14 @@
 
     @project.setter
     def project(self, project: Optional[TableauProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project = project
 
-    type_name: str = Field("TableauFlow", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TableauFlow":
-            raise ValueError("must be TableauFlow")
-        return v
-
     class Attributes(Tableau.Attributes):
         site_qualified_name: Optional[str] = Field(
             None, description="", alias="siteQualifiedName"
         )
         project_qualified_name: Optional[str] = Field(
             None, description="", alias="projectQualifiedName"
         )
@@ -20031,14 +19925,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauWorksheet(Tableau):
     """Description"""
 
+    type_name: str = Field("TableauWorksheet", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TableauWorksheet":
+            raise ValueError("must be TableauWorksheet")
+        return v
+
     def __setattr__(self, name, value):
         if name in TableauWorksheet._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
@@ -20154,22 +20056,14 @@
 
     @dashboards.setter
     def dashboards(self, dashboards: Optional[list[TableauDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboards = dashboards
 
-    type_name: str = Field("TableauWorksheet", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TableauWorksheet":
-            raise ValueError("must be TableauWorksheet")
-        return v
-
     class Attributes(Tableau.Attributes):
         site_qualified_name: Optional[str] = Field(
             None, description="", alias="siteQualifiedName"
         )
         project_qualified_name: Optional[str] = Field(
             None, description="", alias="projectQualifiedName"
         )
@@ -20201,14 +20095,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerLook(Looker):
     """Description"""
 
+    type_name: str = Field("LookerLook", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "LookerLook":
+            raise ValueError("must be LookerLook")
+        return v
+
     def __setattr__(self, name, value):
         if name in LookerLook._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "folder_name",
@@ -20373,22 +20275,14 @@
 
     @dashboard.setter
     def dashboard(self, dashboard: Optional[LookerDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboard = dashboard
 
-    type_name: str = Field("LookerLook", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "LookerLook":
-            raise ValueError("must be LookerLook")
-        return v
-
     class Attributes(Looker.Attributes):
         folder_name: Optional[str] = Field(None, description="", alias="folderName")
         source_user_id: Optional[int] = Field(
             None, description="", alias="sourceUserId"
         )
         source_view_count: Optional[int] = Field(
             None, description="", alias="sourceViewCount"
@@ -20431,14 +20325,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerDashboard(Looker):
     """Description"""
 
+    type_name: str = Field("LookerDashboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "LookerDashboard":
+            raise ValueError("must be LookerDashboard")
+        return v
+
     def __setattr__(self, name, value):
         if name in LookerDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "folder_name",
@@ -20555,22 +20457,14 @@
 
     @folder.setter
     def folder(self, folder: Optional[LookerFolder]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.folder = folder
 
-    type_name: str = Field("LookerDashboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "LookerDashboard":
-            raise ValueError("must be LookerDashboard")
-        return v
-
     class Attributes(Looker.Attributes):
         folder_name: Optional[str] = Field(None, description="", alias="folderName")
         source_user_id: Optional[int] = Field(
             None, description="", alias="sourceUserId"
         )
         source_view_count: Optional[int] = Field(
             None, description="", alias="sourceViewCount"
@@ -20603,14 +20497,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerFolder(Looker):
     """Description"""
 
+    type_name: str = Field("LookerFolder", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "LookerFolder":
+            raise ValueError("must be LookerFolder")
+        return v
+
     def __setattr__(self, name, value):
         if name in LookerFolder._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_content_metadata_id",
@@ -20681,22 +20583,14 @@
 
     @dashboards.setter
     def dashboards(self, dashboards: Optional[list[LookerDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboards = dashboards
 
-    type_name: str = Field("LookerFolder", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "LookerFolder":
-            raise ValueError("must be LookerFolder")
-        return v
-
     class Attributes(Looker.Attributes):
         source_content_metadata_id: Optional[int] = Field(
             None, description="", alias="sourceContentMetadataId"
         )
         source_creator_id: Optional[int] = Field(
             None, description="", alias="sourceCreatorId"
         )
@@ -20719,14 +20613,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerTile(Looker):
     """Description"""
 
+    type_name: str = Field("LookerTile", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "LookerTile":
+            raise ValueError("must be LookerTile")
+        return v
+
     def __setattr__(self, name, value):
         if name in LookerTile._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "lookml_link_id",
@@ -20837,22 +20739,14 @@
 
     @dashboard.setter
     def dashboard(self, dashboard: Optional[LookerDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboard = dashboard
 
-    type_name: str = Field("LookerTile", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "LookerTile":
-            raise ValueError("must be LookerTile")
-        return v
-
     class Attributes(Looker.Attributes):
         lookml_link_id: Optional[str] = Field(
             None, description="", alias="lookmlLinkId"
         )
         merge_result_id: Optional[str] = Field(
             None, description="", alias="mergeResultId"
         )
@@ -20879,14 +20773,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerModel(Looker):
     """Description"""
 
+    type_name: str = Field("LookerModel", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "LookerModel":
+            raise ValueError("must be LookerModel")
+        return v
+
     def __setattr__(self, name, value):
         if name in LookerModel._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "project_name",
@@ -20953,22 +20855,14 @@
 
     @fields.setter
     def fields(self, fields: Optional[list[LookerField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
-    type_name: str = Field("LookerModel", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "LookerModel":
-            raise ValueError("must be LookerModel")
-        return v
-
     class Attributes(Looker.Attributes):
         project_name: Optional[str] = Field(None, description="", alias="projectName")
         explores: Optional[list[LookerExplore]] = Field(
             None, description="", alias="explores"
         )  # relationship
         project: Optional[LookerProject] = Field(
             None, description="", alias="project"
@@ -20989,14 +20883,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerExplore(Looker):
     """Description"""
 
+    type_name: str = Field("LookerExplore", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "LookerExplore":
+            raise ValueError("must be LookerExplore")
+        return v
+
     def __setattr__(self, name, value):
         if name in LookerExplore._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "project_name",
@@ -21087,22 +20989,14 @@
 
     @fields.setter
     def fields(self, fields: Optional[list[LookerField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
-    type_name: str = Field("LookerExplore", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "LookerExplore":
-            raise ValueError("must be LookerExplore")
-        return v
-
     class Attributes(Looker.Attributes):
         project_name: Optional[str] = Field(None, description="", alias="projectName")
         model_name: Optional[str] = Field(None, description="", alias="modelName")
         source_connection_name: Optional[str] = Field(
             None, description="", alias="sourceConnectionName"
         )
         view_name: Optional[str] = Field(None, description="", alias="viewName")
@@ -21125,14 +21019,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerProject(Looker):
     """Description"""
 
+    type_name: str = Field("LookerProject", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "LookerProject":
+            raise ValueError("must be LookerProject")
+        return v
+
     def __setattr__(self, name, value):
         if name in LookerProject._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "models",
@@ -21177,22 +21079,14 @@
 
     @views.setter
     def views(self, views: Optional[list[LookerView]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.views = views
 
-    type_name: str = Field("LookerProject", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "LookerProject":
-            raise ValueError("must be LookerProject")
-        return v
-
     class Attributes(Looker.Attributes):
         models: Optional[list[LookerModel]] = Field(
             None, description="", alias="models"
         )  # relationship
         explores: Optional[list[LookerExplore]] = Field(
             None, description="", alias="explores"
         )  # relationship
@@ -21209,14 +21103,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerQuery(Looker):
     """Description"""
 
+    type_name: str = Field("LookerQuery", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "LookerQuery":
+            raise ValueError("must be LookerQuery")
+        return v
+
     def __setattr__(self, name, value):
         if name in LookerQuery._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_definition",
@@ -21302,22 +21204,14 @@
 
     @model.setter
     def model(self, model: Optional[LookerModel]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.model = model
 
-    type_name: str = Field("LookerQuery", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "LookerQuery":
-            raise ValueError("must be LookerQuery")
-        return v
-
     class Attributes(Looker.Attributes):
         source_definition: Optional[str] = Field(
             None, description="", alias="sourceDefinition"
         )
         source_definition_database: Optional[str] = Field(
             None, description="", alias="sourceDefinitionDatabase"
         )
@@ -21341,14 +21235,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerField(Looker):
     """Description"""
 
+    type_name: str = Field("LookerField", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "LookerField":
+            raise ValueError("must be LookerField")
+        return v
+
     def __setattr__(self, name, value):
         if name in LookerField._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "project_name",
@@ -21482,22 +21384,14 @@
 
     @model.setter
     def model(self, model: Optional[LookerModel]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.model = model
 
-    type_name: str = Field("LookerField", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "LookerField":
-            raise ValueError("must be LookerField")
-        return v
-
     class Attributes(Looker.Attributes):
         project_name: Optional[str] = Field(None, description="", alias="projectName")
         looker_explore_qualified_name: Optional[str] = Field(
             None, description="", alias="lookerExploreQualifiedName"
         )
         looker_view_qualified_name: Optional[str] = Field(
             None, description="", alias="lookerViewQualifiedName"
@@ -21531,14 +21425,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerView(Looker):
     """Description"""
 
+    type_name: str = Field("LookerView", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "LookerView":
+            raise ValueError("must be LookerView")
+        return v
+
     def __setattr__(self, name, value):
         if name in LookerView._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "project_name",
@@ -21572,22 +21474,14 @@
 
     @fields.setter
     def fields(self, fields: Optional[list[LookerField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
-    type_name: str = Field("LookerView", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "LookerView":
-            raise ValueError("must be LookerView")
-        return v
-
     class Attributes(Looker.Attributes):
         project_name: Optional[str] = Field(None, description="", alias="projectName")
         project: Optional[LookerProject] = Field(
             None, description="", alias="project"
         )  # relationship
         fields: Optional[list[LookerField]] = Field(
             None, description="", alias="fields"
@@ -21599,14 +21493,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class RedashDashboard(Redash):
     """Description"""
 
+    type_name: str = Field("RedashDashboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "RedashDashboard":
+            raise ValueError("must be RedashDashboard")
+        return v
+
     def __setattr__(self, name, value):
         if name in RedashDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "redash_dashboard_widget_count",
@@ -21624,22 +21526,14 @@
     def redash_dashboard_widget_count(
         self, redash_dashboard_widget_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_dashboard_widget_count = redash_dashboard_widget_count
 
-    type_name: str = Field("RedashDashboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "RedashDashboard":
-            raise ValueError("must be RedashDashboard")
-        return v
-
     class Attributes(Redash.Attributes):
         redash_dashboard_widget_count: Optional[int] = Field(
             None, description="", alias="redashDashboardWidgetCount"
         )
 
     attributes: "RedashDashboard.Attributes" = Field(
         default_factory=lambda: RedashDashboard.Attributes(),
@@ -21647,14 +21541,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class RedashQuery(Redash):
     """Description"""
 
+    type_name: str = Field("RedashQuery", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "RedashQuery":
+            raise ValueError("must be RedashQuery")
+        return v
+
     def __setattr__(self, name, value):
         if name in RedashQuery._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "redash_query_s_q_l",
@@ -21762,22 +21664,14 @@
     def redash_visualizations(
         self, redash_visualizations: Optional[list[RedashVisualization]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_visualizations = redash_visualizations
 
-    type_name: str = Field("RedashQuery", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "RedashQuery":
-            raise ValueError("must be RedashQuery")
-        return v
-
     class Attributes(Redash.Attributes):
         redash_query_s_q_l: Optional[str] = Field(
             None, description="", alias="redashQuerySQL"
         )
         redash_query_parameters: Optional[str] = Field(
             None, description="", alias="redashQueryParameters"
         )
@@ -21803,14 +21697,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class RedashVisualization(Redash):
     """Description"""
 
+    type_name: str = Field("RedashVisualization", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "RedashVisualization":
+            raise ValueError("must be RedashVisualization")
+        return v
+
     def __setattr__(self, name, value):
         if name in RedashVisualization._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "redash_visualization_type",
@@ -21863,22 +21765,14 @@
 
     @redash_query.setter
     def redash_query(self, redash_query: Optional[RedashQuery]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_query = redash_query
 
-    type_name: str = Field("RedashVisualization", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "RedashVisualization":
-            raise ValueError("must be RedashVisualization")
-        return v
-
     class Attributes(Redash.Attributes):
         redash_visualization_type: Optional[str] = Field(
             None, description="", alias="redashVisualizationType"
         )
         redash_query_name: Optional[str] = Field(
             None, description="", alias="redashQueryName"
         )
@@ -21895,14 +21789,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MetabaseQuestion(Metabase):
     """Description"""
 
+    type_name: str = Field("MetabaseQuestion", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MetabaseQuestion":
+            raise ValueError("must be MetabaseQuestion")
+        return v
+
     def __setattr__(self, name, value):
         if name in MetabaseQuestion._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metabase_dashboard_count",
@@ -21964,22 +21866,14 @@
 
     @metabase_collection.setter
     def metabase_collection(self, metabase_collection: Optional[MetabaseCollection]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_collection = metabase_collection
 
-    type_name: str = Field("MetabaseQuestion", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MetabaseQuestion":
-            raise ValueError("must be MetabaseQuestion")
-        return v
-
     class Attributes(Metabase.Attributes):
         metabase_dashboard_count: Optional[int] = Field(
             None, description="", alias="metabaseDashboardCount"
         )
         metabase_query_type: Optional[str] = Field(
             None, description="", alias="metabaseQueryType"
         )
@@ -21999,14 +21893,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MetabaseCollection(Metabase):
     """Description"""
 
+    type_name: str = Field("MetabaseCollection", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MetabaseCollection":
+            raise ValueError("must be MetabaseCollection")
+        return v
+
     def __setattr__(self, name, value):
         if name in MetabaseCollection._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metabase_slug",
@@ -22083,22 +21985,14 @@
 
     @metabase_questions.setter
     def metabase_questions(self, metabase_questions: Optional[list[MetabaseQuestion]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_questions = metabase_questions
 
-    type_name: str = Field("MetabaseCollection", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MetabaseCollection":
-            raise ValueError("must be MetabaseCollection")
-        return v
-
     class Attributes(Metabase.Attributes):
         metabase_slug: Optional[str] = Field(None, description="", alias="metabaseSlug")
         metabase_color: Optional[str] = Field(
             None, description="", alias="metabaseColor"
         )
         metabase_namespace: Optional[str] = Field(
             None, description="", alias="metabaseNamespace"
@@ -22119,14 +22013,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MetabaseDashboard(Metabase):
     """Description"""
 
+    type_name: str = Field("MetabaseDashboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MetabaseDashboard":
+            raise ValueError("must be MetabaseDashboard")
+        return v
+
     def __setattr__(self, name, value):
         if name in MetabaseDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metabase_question_count",
@@ -22162,22 +22064,14 @@
 
     @metabase_collection.setter
     def metabase_collection(self, metabase_collection: Optional[MetabaseCollection]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_collection = metabase_collection
 
-    type_name: str = Field("MetabaseDashboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MetabaseDashboard":
-            raise ValueError("must be MetabaseDashboard")
-        return v
-
     class Attributes(Metabase.Attributes):
         metabase_question_count: Optional[int] = Field(
             None, description="", alias="metabaseQuestionCount"
         )
         metabase_questions: Optional[list[MetabaseQuestion]] = Field(
             None, description="", alias="metabaseQuestions"
         )  # relationship
@@ -22191,14 +22085,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightFolder(QuickSight):
     """Description"""
 
+    type_name: str = Field("QuickSightFolder", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightFolder":
+            raise ValueError("must be QuickSightFolder")
+        return v
+
     def __setattr__(self, name, value):
         if name in QuickSightFolder._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_folder_type",
@@ -22272,22 +22174,14 @@
     def quick_sight_datasets(
         self, quick_sight_datasets: Optional[list[QuickSightDataset]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_datasets = quick_sight_datasets
 
-    type_name: str = Field("QuickSightFolder", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightFolder":
-            raise ValueError("must be QuickSightFolder")
-        return v
-
     class Attributes(QuickSight.Attributes):
         quick_sight_folder_type: Optional[QuickSightFolderType] = Field(
             None, description="", alias="quickSightFolderType"
         )
         quick_sight_folder_hierarchy: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="quickSightFolderHierarchy"
         )
@@ -22307,14 +22201,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightDashboardVisual(QuickSight):
     """Description"""
 
+    type_name: str = Field("QuickSightDashboardVisual", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightDashboardVisual":
+            raise ValueError("must be QuickSightDashboardVisual")
+        return v
+
     def __setattr__(self, name, value):
         if name in QuickSightDashboardVisual._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dashboard_qualified_name",
@@ -22349,22 +22251,14 @@
     def quick_sight_dashboard(
         self, quick_sight_dashboard: Optional[QuickSightDashboard]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dashboard = quick_sight_dashboard
 
-    type_name: str = Field("QuickSightDashboardVisual", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightDashboardVisual":
-            raise ValueError("must be QuickSightDashboardVisual")
-        return v
-
     class Attributes(QuickSight.Attributes):
         quick_sight_dashboard_qualified_name: Optional[str] = Field(
             None, description="", alias="quickSightDashboardQualifiedName"
         )
         quick_sight_dashboard: Optional[QuickSightDashboard] = Field(
             None, description="", alias="quickSightDashboard"
         )  # relationship
@@ -22375,14 +22269,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightAnalysisVisual(QuickSight):
     """Description"""
 
+    type_name: str = Field("QuickSightAnalysisVisual", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightAnalysisVisual":
+            raise ValueError("must be QuickSightAnalysisVisual")
+        return v
+
     def __setattr__(self, name, value):
         if name in QuickSightAnalysisVisual._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_analysis_qualified_name",
@@ -22413,22 +22315,14 @@
 
     @quick_sight_analysis.setter
     def quick_sight_analysis(self, quick_sight_analysis: Optional[QuickSightAnalysis]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis = quick_sight_analysis
 
-    type_name: str = Field("QuickSightAnalysisVisual", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightAnalysisVisual":
-            raise ValueError("must be QuickSightAnalysisVisual")
-        return v
-
     class Attributes(QuickSight.Attributes):
         quick_sight_analysis_qualified_name: Optional[str] = Field(
             None, description="", alias="quickSightAnalysisQualifiedName"
         )
         quick_sight_analysis: Optional[QuickSightAnalysis] = Field(
             None, description="", alias="quickSightAnalysis"
         )  # relationship
@@ -22439,14 +22333,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightDatasetField(QuickSight):
     """Description"""
 
+    type_name: str = Field("QuickSightDatasetField", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightDatasetField":
+            raise ValueError("must be QuickSightDatasetField")
+        return v
+
     def __setattr__(self, name, value):
         if name in QuickSightDatasetField._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dataset_field_type",
@@ -22494,22 +22396,14 @@
 
     @quick_sight_dataset.setter
     def quick_sight_dataset(self, quick_sight_dataset: Optional[QuickSightDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dataset = quick_sight_dataset
 
-    type_name: str = Field("QuickSightDatasetField", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightDatasetField":
-            raise ValueError("must be QuickSightDatasetField")
-        return v
-
     class Attributes(QuickSight.Attributes):
         quick_sight_dataset_field_type: Optional[QuickSightDatasetFieldType] = Field(
             None, description="", alias="quickSightDatasetFieldType"
         )
         quick_sight_dataset_qualified_name: Optional[str] = Field(
             None, description="", alias="quickSightDatasetQualifiedName"
         )
@@ -22523,14 +22417,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightAnalysis(QuickSight):
     """Description"""
 
+    type_name: str = Field("QuickSightAnalysis", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightAnalysis":
+            raise ValueError("must be QuickSightAnalysis")
+        return v
+
     def __setattr__(self, name, value):
         if name in QuickSightAnalysis._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_analysis_status",
@@ -22639,22 +22541,14 @@
     def quick_sight_analysis_folders(
         self, quick_sight_analysis_folders: Optional[list[QuickSightFolder]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis_folders = quick_sight_analysis_folders
 
-    type_name: str = Field("QuickSightAnalysis", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightAnalysis":
-            raise ValueError("must be QuickSightAnalysis")
-        return v
-
     class Attributes(QuickSight.Attributes):
         quick_sight_analysis_status: Optional[QuickSightAnalysisStatus] = Field(
             None, description="", alias="quickSightAnalysisStatus"
         )
         quick_sight_analysis_calculated_fields: Optional[set[str]] = Field(
             None, description="", alias="quickSightAnalysisCalculatedFields"
         )
@@ -22677,14 +22571,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightDashboard(QuickSight):
     """Description"""
 
+    type_name: str = Field("QuickSightDashboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightDashboard":
+            raise ValueError("must be QuickSightDashboard")
+        return v
+
     def __setattr__(self, name, value):
         if name in QuickSightDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dashboard_published_version_number",
@@ -22759,22 +22661,14 @@
     def quick_sight_dashboard_visuals(
         self, quick_sight_dashboard_visuals: Optional[list[QuickSightDashboardVisual]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dashboard_visuals = quick_sight_dashboard_visuals
 
-    type_name: str = Field("QuickSightDashboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightDashboard":
-            raise ValueError("must be QuickSightDashboard")
-        return v
-
     class Attributes(QuickSight.Attributes):
         quick_sight_dashboard_published_version_number: Optional[int] = Field(
             None, description="", alias="quickSightDashboardPublishedVersionNumber"
         )
         quick_sight_dashboard_last_published_time: Optional[datetime] = Field(
             None, description="", alias="quickSightDashboardLastPublishedTime"
         )
@@ -22793,14 +22687,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightDataset(QuickSight):
     """Description"""
 
+    type_name: str = Field("QuickSightDataset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightDataset":
+            raise ValueError("must be QuickSightDataset")
+        return v
+
     def __setattr__(self, name, value):
         if name in QuickSightDataset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dataset_import_mode",
@@ -22873,22 +22775,14 @@
     def quick_sight_dataset_fields(
         self, quick_sight_dataset_fields: Optional[list[QuickSightDatasetField]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dataset_fields = quick_sight_dataset_fields
 
-    type_name: str = Field("QuickSightDataset", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightDataset":
-            raise ValueError("must be QuickSightDataset")
-        return v
-
     class Attributes(QuickSight.Attributes):
         quick_sight_dataset_import_mode: Optional[QuickSightDatasetImportMode] = Field(
             None, description="", alias="quickSightDatasetImportMode"
         )
         quick_sight_dataset_column_count: Optional[int] = Field(
             None, description="", alias="quickSightDatasetColumnCount"
         )
@@ -22905,14 +22799,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ThoughtspotLiveboard(Thoughtspot):
     """Description"""
 
+    type_name: str = Field("ThoughtspotLiveboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ThoughtspotLiveboard":
+            raise ValueError("must be ThoughtspotLiveboard")
+        return v
+
     def __setattr__(self, name, value):
         if name in ThoughtspotLiveboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "thoughtspot_dashlets",
@@ -22926,22 +22828,14 @@
     def thoughtspot_dashlets(
         self, thoughtspot_dashlets: Optional[list[ThoughtspotDashlet]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.thoughtspot_dashlets = thoughtspot_dashlets
 
-    type_name: str = Field("ThoughtspotLiveboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ThoughtspotLiveboard":
-            raise ValueError("must be ThoughtspotLiveboard")
-        return v
-
     class Attributes(Thoughtspot.Attributes):
         thoughtspot_dashlets: Optional[list[ThoughtspotDashlet]] = Field(
             None, description="", alias="thoughtspotDashlets"
         )  # relationship
 
     attributes: "ThoughtspotLiveboard.Attributes" = Field(
         default_factory=lambda: ThoughtspotLiveboard.Attributes(),
@@ -22949,14 +22843,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ThoughtspotDashlet(Thoughtspot):
     """Description"""
 
+    type_name: str = Field("ThoughtspotDashlet", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ThoughtspotDashlet":
+            raise ValueError("must be ThoughtspotDashlet")
+        return v
+
     def __setattr__(self, name, value):
         if name in ThoughtspotDashlet._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "thoughtspot_liveboard_name",
@@ -23006,22 +22908,14 @@
     def thoughtspot_liveboard(
         self, thoughtspot_liveboard: Optional[ThoughtspotLiveboard]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.thoughtspot_liveboard = thoughtspot_liveboard
 
-    type_name: str = Field("ThoughtspotDashlet", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ThoughtspotDashlet":
-            raise ValueError("must be ThoughtspotDashlet")
-        return v
-
     class Attributes(Thoughtspot.Attributes):
         thoughtspot_liveboard_name: Optional[str] = Field(
             None, description="", alias="thoughtspotLiveboardName"
         )
         thoughtspot_liveboard_qualified_name: Optional[str] = Field(
             None, description="", alias="thoughtspotLiveboardQualifiedName"
         )
@@ -23035,33 +22929,41 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ThoughtspotAnswer(Thoughtspot):
     """Description"""
 
-    def __setattr__(self, name, value):
-        if name in ThoughtspotAnswer._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
     type_name: str = Field("ThoughtspotAnswer", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ThoughtspotAnswer":
             raise ValueError("must be ThoughtspotAnswer")
         return v
 
+    def __setattr__(self, name, value):
+        if name in ThoughtspotAnswer._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
 
 class PowerBIReport(PowerBI):
     """Description"""
 
+    type_name: str = Field("PowerBIReport", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIReport":
+            raise ValueError("must be PowerBIReport")
+        return v
+
     def __setattr__(self, name, value):
         if name in PowerBIReport._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
@@ -23156,22 +23058,14 @@
 
     @dataset.setter
     def dataset(self, dataset: Optional[PowerBIDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataset = dataset
 
-    type_name: str = Field("PowerBIReport", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIReport":
-            raise ValueError("must be PowerBIReport")
-        return v
-
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         dataset_qualified_name: Optional[str] = Field(
             None, description="", alias="datasetQualifiedName"
         )
@@ -23196,14 +23090,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIMeasure(PowerBI):
     """Description"""
 
+    type_name: str = Field("PowerBIMeasure", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIMeasure":
+            raise ValueError("must be PowerBIMeasure")
+        return v
+
     def __setattr__(self, name, value):
         if name in PowerBIMeasure._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
@@ -23275,22 +23177,14 @@
 
     @table.setter
     def table(self, table: Optional[PowerBITable]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.table = table
 
-    type_name: str = Field("PowerBIMeasure", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIMeasure":
-            raise ValueError("must be PowerBIMeasure")
-        return v
-
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         dataset_qualified_name: Optional[str] = Field(
             None, description="", alias="datasetQualifiedName"
         )
@@ -23310,14 +23204,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIColumn(PowerBI):
     """Description"""
 
+    type_name: str = Field("PowerBIColumn", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIColumn":
+            raise ValueError("must be PowerBIColumn")
+        return v
+
     def __setattr__(self, name, value):
         if name in PowerBIColumn._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
@@ -23421,22 +23323,14 @@
 
     @table.setter
     def table(self, table: Optional[PowerBITable]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.table = table
 
-    type_name: str = Field("PowerBIColumn", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIColumn":
-            raise ValueError("must be PowerBIColumn")
-        return v
-
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         dataset_qualified_name: Optional[str] = Field(
             None, description="", alias="datasetQualifiedName"
         )
@@ -23462,14 +23356,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBITable(PowerBI):
     """Description"""
 
+    type_name: str = Field("PowerBITable", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBITable":
+            raise ValueError("must be PowerBITable")
+        return v
+
     def __setattr__(self, name, value):
         if name in PowerBITable._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
@@ -23582,22 +23484,14 @@
 
     @dataset.setter
     def dataset(self, dataset: Optional[PowerBIDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataset = dataset
 
-    type_name: str = Field("PowerBITable", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBITable":
-            raise ValueError("must be PowerBITable")
-        return v
-
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         dataset_qualified_name: Optional[str] = Field(
             None, description="", alias="datasetQualifiedName"
         )
@@ -23626,14 +23520,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBITile(PowerBI):
     """Description"""
 
+    type_name: str = Field("PowerBITile", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBITile":
+            raise ValueError("must be PowerBITile")
+        return v
+
     def __setattr__(self, name, value):
         if name in PowerBITile._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
@@ -23697,22 +23599,14 @@
 
     @dashboard.setter
     def dashboard(self, dashboard: Optional[PowerBIDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboard = dashboard
 
-    type_name: str = Field("PowerBITile", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBITile":
-            raise ValueError("must be PowerBITile")
-        return v
-
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         dashboard_qualified_name: Optional[str] = Field(
             None, description="", alias="dashboardQualifiedName"
         )
@@ -23732,14 +23626,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIDatasource(PowerBI):
     """Description"""
 
+    type_name: str = Field("PowerBIDatasource", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIDatasource":
+            raise ValueError("must be PowerBIDatasource")
+        return v
+
     def __setattr__(self, name, value):
         if name in PowerBIDatasource._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "connection_details",
@@ -23762,22 +23664,14 @@
 
     @datasets.setter
     def datasets(self, datasets: Optional[list[PowerBIDataset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasets = datasets
 
-    type_name: str = Field("PowerBIDatasource", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIDatasource":
-            raise ValueError("must be PowerBIDatasource")
-        return v
-
     class Attributes(PowerBI.Attributes):
         connection_details: Optional[dict[str, str]] = Field(
             None, description="", alias="connectionDetails"
         )
         datasets: Optional[list[PowerBIDataset]] = Field(
             None, description="", alias="datasets"
         )  # relationship
@@ -23788,14 +23682,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIWorkspace(PowerBI):
     """Description"""
 
+    type_name: str = Field("PowerBIWorkspace", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIWorkspace":
+            raise ValueError("must be PowerBIWorkspace")
+        return v
+
     def __setattr__(self, name, value):
         if name in PowerBIWorkspace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "web_url",
@@ -23895,22 +23797,14 @@
 
     @dataflows.setter
     def dataflows(self, dataflows: Optional[list[PowerBIDataflow]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataflows = dataflows
 
-    type_name: str = Field("PowerBIWorkspace", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIWorkspace":
-            raise ValueError("must be PowerBIWorkspace")
-        return v
-
     class Attributes(PowerBI.Attributes):
         web_url: Optional[str] = Field(None, description="", alias="webUrl")
         report_count: Optional[int] = Field(None, description="", alias="reportCount")
         dashboard_count: Optional[int] = Field(
             None, description="", alias="dashboardCount"
         )
         dataset_count: Optional[int] = Field(None, description="", alias="datasetCount")
@@ -23936,14 +23830,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIDataset(PowerBI):
     """Description"""
 
+    type_name: str = Field("PowerBIDataset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIDataset":
+            raise ValueError("must be PowerBIDataset")
+        return v
+
     def __setattr__(self, name, value):
         if name in PowerBIDataset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
@@ -24036,22 +23938,14 @@
 
     @datasources.setter
     def datasources(self, datasources: Optional[list[PowerBIDatasource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasources = datasources
 
-    type_name: str = Field("PowerBIDataset", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIDataset":
-            raise ValueError("must be PowerBIDataset")
-        return v
-
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         web_url: Optional[str] = Field(None, description="", alias="webUrl")
         reports: Optional[list[PowerBIReport]] = Field(
             None, description="", alias="reports"
@@ -24078,14 +23972,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIDashboard(PowerBI):
     """Description"""
 
+    type_name: str = Field("PowerBIDashboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIDashboard":
+            raise ValueError("must be PowerBIDashboard")
+        return v
+
     def __setattr__(self, name, value):
         if name in PowerBIDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
@@ -24145,22 +24047,14 @@
 
     @workspace.setter
     def workspace(self, workspace: Optional[PowerBIWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace = workspace
 
-    type_name: str = Field("PowerBIDashboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIDashboard":
-            raise ValueError("must be PowerBIDashboard")
-        return v
-
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         web_url: Optional[str] = Field(None, description="", alias="webUrl")
         tile_count: Optional[int] = Field(None, description="", alias="tileCount")
         tiles: Optional[list[PowerBITile]] = Field(
@@ -24176,14 +24070,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIDataflow(PowerBI):
     """Description"""
 
+    type_name: str = Field("PowerBIDataflow", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIDataflow":
+            raise ValueError("must be PowerBIDataflow")
+        return v
+
     def __setattr__(self, name, value):
         if name in PowerBIDataflow._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
@@ -24232,22 +24134,14 @@
 
     @datasets.setter
     def datasets(self, datasets: Optional[list[PowerBIDataset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasets = datasets
 
-    type_name: str = Field("PowerBIDataflow", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIDataflow":
-            raise ValueError("must be PowerBIDataflow")
-        return v
-
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         web_url: Optional[str] = Field(None, description="", alias="webUrl")
         workspace: Optional[PowerBIWorkspace] = Field(
             None, description="", alias="workspace"
@@ -24262,14 +24156,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIPage(PowerBI):
     """Description"""
 
+    type_name: str = Field("PowerBIPage", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIPage":
+            raise ValueError("must be PowerBIPage")
+        return v
+
     def __setattr__(self, name, value):
         if name in PowerBIPage._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
@@ -24309,22 +24211,14 @@
 
     @report.setter
     def report(self, report: Optional[PowerBIReport]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.report = report
 
-    type_name: str = Field("PowerBIPage", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIPage":
-            raise ValueError("must be PowerBIPage")
-        return v
-
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         report_qualified_name: Optional[str] = Field(
             None, description="", alias="reportQualifiedName"
         )
@@ -24338,14 +24232,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MicroStrategyReport(MicroStrategy):
     """Description"""
 
+    type_name: str = Field("MicroStrategyReport", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyReport":
+            raise ValueError("must be MicroStrategyReport")
+        return v
+
     def __setattr__(self, name, value):
         if name in MicroStrategyReport._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "micro_strategy_report_type",
@@ -24408,22 +24310,14 @@
     def micro_strategy_attributes(
         self, micro_strategy_attributes: Optional[list[MicroStrategyAttribute]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_attributes = micro_strategy_attributes
 
-    type_name: str = Field("MicroStrategyReport", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MicroStrategyReport":
-            raise ValueError("must be MicroStrategyReport")
-        return v
-
     class Attributes(MicroStrategy.Attributes):
         micro_strategy_report_type: Optional[str] = Field(
             None, description="", alias="microStrategyReportType"
         )
         micro_strategy_metrics: Optional[list[MicroStrategyMetric]] = Field(
             None, description="", alias="microStrategyMetrics"
         )  # relationship
@@ -24440,14 +24334,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MicroStrategyProject(MicroStrategy):
     """Description"""
 
+    type_name: str = Field("MicroStrategyProject", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyProject":
+            raise ValueError("must be MicroStrategyProject")
+        return v
+
     def __setattr__(self, name, value):
         if name in MicroStrategyProject._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "micro_strategy_reports",
@@ -24572,22 +24474,14 @@
     def micro_strategy_attributes(
         self, micro_strategy_attributes: Optional[list[MicroStrategyAttribute]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_attributes = micro_strategy_attributes
 
-    type_name: str = Field("MicroStrategyProject", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MicroStrategyProject":
-            raise ValueError("must be MicroStrategyProject")
-        return v
-
     class Attributes(MicroStrategy.Attributes):
         micro_strategy_reports: Optional[list[MicroStrategyReport]] = Field(
             None, description="", alias="microStrategyReports"
         )  # relationship
         micro_strategy_facts: Optional[list[MicroStrategyFact]] = Field(
             None, description="", alias="microStrategyFacts"
         )  # relationship
@@ -24618,14 +24512,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MicroStrategyMetric(MicroStrategy):
     """Description"""
 
+    type_name: str = Field("MicroStrategyMetric", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyMetric":
+            raise ValueError("must be MicroStrategyMetric")
+        return v
+
     def __setattr__(self, name, value):
         if name in MicroStrategyMetric._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "micro_strategy_metric_expression",
@@ -24860,22 +24762,14 @@
     def micro_strategy_attributes(
         self, micro_strategy_attributes: Optional[list[MicroStrategyAttribute]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_attributes = micro_strategy_attributes
 
-    type_name: str = Field("MicroStrategyMetric", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MicroStrategyMetric":
-            raise ValueError("must be MicroStrategyMetric")
-        return v
-
     class Attributes(MicroStrategy.Attributes):
         micro_strategy_metric_expression: Optional[str] = Field(
             None, description="", alias="microStrategyMetricExpression"
         )
         micro_strategy_attribute_qualified_names: Optional[set[str]] = Field(
             None, description="", alias="microStrategyAttributeQualifiedNames"
         )
@@ -24922,14 +24816,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MicroStrategyCube(MicroStrategy):
     """Description"""
 
+    type_name: str = Field("MicroStrategyCube", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyCube":
+            raise ValueError("must be MicroStrategyCube")
+        return v
+
     def __setattr__(self, name, value):
         if name in MicroStrategyCube._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "micro_strategy_cube_type",
@@ -25007,22 +24909,14 @@
     def micro_strategy_attributes(
         self, micro_strategy_attributes: Optional[list[MicroStrategyAttribute]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_attributes = micro_strategy_attributes
 
-    type_name: str = Field("MicroStrategyCube", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MicroStrategyCube":
-            raise ValueError("must be MicroStrategyCube")
-        return v
-
     class Attributes(MicroStrategy.Attributes):
         micro_strategy_cube_type: Optional[str] = Field(
             None, description="", alias="microStrategyCubeType"
         )
         micro_strategy_cube_query: Optional[str] = Field(
             None, description="", alias="microStrategyCubeQuery"
         )
@@ -25042,14 +24936,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MicroStrategyDossier(MicroStrategy):
     """Description"""
 
+    type_name: str = Field("MicroStrategyDossier", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyDossier":
+            raise ValueError("must be MicroStrategyDossier")
+        return v
+
     def __setattr__(self, name, value):
         if name in MicroStrategyDossier._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "micro_strategy_dossier_chapter_names",
@@ -25103,22 +25005,14 @@
     def micro_strategy_visualizations(
         self, micro_strategy_visualizations: Optional[list[MicroStrategyVisualization]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_visualizations = micro_strategy_visualizations
 
-    type_name: str = Field("MicroStrategyDossier", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MicroStrategyDossier":
-            raise ValueError("must be MicroStrategyDossier")
-        return v
-
     class Attributes(MicroStrategy.Attributes):
         micro_strategy_dossier_chapter_names: Optional[set[str]] = Field(
             None, description="", alias="microStrategyDossierChapterNames"
         )
         micro_strategy_project: Optional[MicroStrategyProject] = Field(
             None, description="", alias="microStrategyProject"
         )  # relationship
@@ -25134,14 +25028,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MicroStrategyFact(MicroStrategy):
     """Description"""
 
+    type_name: str = Field("MicroStrategyFact", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyFact":
+            raise ValueError("must be MicroStrategyFact")
+        return v
+
     def __setattr__(self, name, value):
         if name in MicroStrategyFact._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "micro_strategy_fact_expressions",
@@ -25191,22 +25093,14 @@
     def micro_strategy_project(
         self, micro_strategy_project: Optional[MicroStrategyProject]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_project = micro_strategy_project
 
-    type_name: str = Field("MicroStrategyFact", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MicroStrategyFact":
-            raise ValueError("must be MicroStrategyFact")
-        return v
-
     class Attributes(MicroStrategy.Attributes):
         micro_strategy_fact_expressions: Optional[set[str]] = Field(
             None, description="", alias="microStrategyFactExpressions"
         )
         micro_strategy_metrics: Optional[list[MicroStrategyMetric]] = Field(
             None, description="", alias="microStrategyMetrics"
         )  # relationship
@@ -25220,14 +25114,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MicroStrategyDocument(MicroStrategy):
     """Description"""
 
+    type_name: str = Field("MicroStrategyDocument", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyDocument":
+            raise ValueError("must be MicroStrategyDocument")
+        return v
+
     def __setattr__(self, name, value):
         if name in MicroStrategyDocument._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "micro_strategy_project",
@@ -25243,22 +25145,14 @@
     def micro_strategy_project(
         self, micro_strategy_project: Optional[MicroStrategyProject]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_project = micro_strategy_project
 
-    type_name: str = Field("MicroStrategyDocument", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MicroStrategyDocument":
-            raise ValueError("must be MicroStrategyDocument")
-        return v
-
     class Attributes(MicroStrategy.Attributes):
         micro_strategy_project: Optional[MicroStrategyProject] = Field(
             None, description="", alias="microStrategyProject"
         )  # relationship
 
     attributes: "MicroStrategyDocument.Attributes" = Field(
         default_factory=lambda: MicroStrategyDocument.Attributes(),
@@ -25266,14 +25160,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MicroStrategyAttribute(MicroStrategy):
     """Description"""
 
+    type_name: str = Field("MicroStrategyAttribute", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyAttribute":
+            raise ValueError("must be MicroStrategyAttribute")
+        return v
+
     def __setattr__(self, name, value):
         if name in MicroStrategyAttribute._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "micro_strategy_attribute_forms",
@@ -25349,22 +25251,14 @@
     def micro_strategy_project(
         self, micro_strategy_project: Optional[MicroStrategyProject]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_project = micro_strategy_project
 
-    type_name: str = Field("MicroStrategyAttribute", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MicroStrategyAttribute":
-            raise ValueError("must be MicroStrategyAttribute")
-        return v
-
     class Attributes(MicroStrategy.Attributes):
         micro_strategy_attribute_forms: Optional[str] = Field(
             None, description="", alias="microStrategyAttributeForms"
         )
         micro_strategy_reports: Optional[list[MicroStrategyReport]] = Field(
             None, description="", alias="microStrategyReports"
         )  # relationship
@@ -25384,14 +25278,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MicroStrategyVisualization(MicroStrategy):
     """Description"""
 
+    type_name: str = Field("MicroStrategyVisualization", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyVisualization":
+            raise ValueError("must be MicroStrategyVisualization")
+        return v
+
     def __setattr__(self, name, value):
         if name in MicroStrategyVisualization._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "micro_strategy_visualization_type",
@@ -25475,22 +25377,14 @@
     def micro_strategy_project(
         self, micro_strategy_project: Optional[MicroStrategyProject]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_project = micro_strategy_project
 
-    type_name: str = Field("MicroStrategyVisualization", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MicroStrategyVisualization":
-            raise ValueError("must be MicroStrategyVisualization")
-        return v
-
     class Attributes(MicroStrategy.Attributes):
         micro_strategy_visualization_type: Optional[str] = Field(
             None, description="", alias="microStrategyVisualizationType"
         )
         micro_strategy_dossier_qualified_name: Optional[str] = Field(
             None, description="", alias="microStrategyDossierQualifiedName"
         )
@@ -25510,14 +25404,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QlikSpace(Qlik):
     """Description"""
 
+    type_name: str = Field("QlikSpace", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QlikSpace":
+            raise ValueError("must be QlikSpace")
+        return v
+
     def __setattr__(self, name, value):
         if name in QlikSpace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_space_type",
@@ -25551,22 +25453,14 @@
 
     @qlik_apps.setter
     def qlik_apps(self, qlik_apps: Optional[list[QlikApp]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_apps = qlik_apps
 
-    type_name: str = Field("QlikSpace", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QlikSpace":
-            raise ValueError("must be QlikSpace")
-        return v
-
     class Attributes(Qlik.Attributes):
         qlik_space_type: Optional[str] = Field(
             None, description="", alias="qlikSpaceType"
         )
         qlik_datasets: Optional[list[QlikDataset]] = Field(
             None, description="", alias="qlikDatasets"
         )  # relationship
@@ -25580,14 +25474,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QlikApp(Qlik):
     """Description"""
 
+    type_name: str = Field("QlikApp", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QlikApp":
+            raise ValueError("must be QlikApp")
+        return v
+
     def __setattr__(self, name, value):
         if name in QlikApp._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_has_section_access",
@@ -25675,22 +25577,14 @@
 
     @qlik_sheets.setter
     def qlik_sheets(self, qlik_sheets: Optional[list[QlikSheet]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_sheets = qlik_sheets
 
-    type_name: str = Field("QlikApp", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QlikApp":
-            raise ValueError("must be QlikApp")
-        return v
-
     class Attributes(Qlik.Attributes):
         qlik_has_section_access: Optional[bool] = Field(
             None, description="", alias="qlikHasSectionAccess"
         )
         qlik_origin_app_id: Optional[str] = Field(
             None, description="", alias="qlikOriginAppId"
         )
@@ -25716,14 +25610,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QlikChart(Qlik):
     """Description"""
 
+    type_name: str = Field("QlikChart", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QlikChart":
+            raise ValueError("must be QlikChart")
+        return v
+
     def __setattr__(self, name, value):
         if name in QlikChart._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_chart_subtitle",
@@ -25781,22 +25683,14 @@
 
     @qlik_sheet.setter
     def qlik_sheet(self, qlik_sheet: Optional[QlikSheet]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_sheet = qlik_sheet
 
-    type_name: str = Field("QlikChart", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QlikChart":
-            raise ValueError("must be QlikChart")
-        return v
-
     class Attributes(Qlik.Attributes):
         qlik_chart_subtitle: Optional[str] = Field(
             None, description="", alias="qlikChartSubtitle"
         )
         qlik_chart_footnote: Optional[str] = Field(
             None, description="", alias="qlikChartFootnote"
         )
@@ -25816,14 +25710,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QlikDataset(Qlik):
     """Description"""
 
+    type_name: str = Field("QlikDataset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QlikDataset":
+            raise ValueError("must be QlikDataset")
+        return v
+
     def __setattr__(self, name, value):
         if name in QlikDataset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_dataset_technical_name",
@@ -25883,22 +25785,14 @@
 
     @qlik_space.setter
     def qlik_space(self, qlik_space: Optional[QlikSpace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_space = qlik_space
 
-    type_name: str = Field("QlikDataset", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QlikDataset":
-            raise ValueError("must be QlikDataset")
-        return v
-
     class Attributes(Qlik.Attributes):
         qlik_dataset_technical_name: Optional[str] = Field(
             None, description="", alias="qlikDatasetTechnicalName"
         )
         qlik_dataset_type: Optional[str] = Field(
             None, description="", alias="qlikDatasetType"
         )
@@ -25918,14 +25812,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QlikSheet(Qlik):
     """Description"""
 
+    type_name: str = Field("QlikSheet", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QlikSheet":
+            raise ValueError("must be QlikSheet")
+        return v
+
     def __setattr__(self, name, value):
         if name in QlikSheet._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_sheet_is_approved",
@@ -25961,22 +25863,14 @@
 
     @qlik_charts.setter
     def qlik_charts(self, qlik_charts: Optional[list[QlikChart]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_charts = qlik_charts
 
-    type_name: str = Field("QlikSheet", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QlikSheet":
-            raise ValueError("must be QlikSheet")
-        return v
-
     class Attributes(Qlik.Attributes):
         qlik_sheet_is_approved: Optional[bool] = Field(
             None, description="", alias="qlikSheetIsApproved"
         )
         qlik_app: Optional[QlikApp] = Field(
             None, description="", alias="qlikApp"
         )  # relationship
@@ -25990,14 +25884,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SalesforceObject(Salesforce):
     """Description"""
 
+    type_name: str = Field("SalesforceObject", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SalesforceObject":
+            raise ValueError("must be SalesforceObject")
+        return v
+
     def __setattr__(self, name, value):
         if name in SalesforceObject._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "is_custom",
@@ -26075,22 +25977,14 @@
 
     @fields.setter
     def fields(self, fields: Optional[list[SalesforceField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
-    type_name: str = Field("SalesforceObject", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SalesforceObject":
-            raise ValueError("must be SalesforceObject")
-        return v
-
     class Attributes(Salesforce.Attributes):
         is_custom: Optional[bool] = Field(None, description="", alias="isCustom")
         is_mergable: Optional[bool] = Field(None, description="", alias="isMergable")
         is_queryable: Optional[bool] = Field(None, description="", alias="isQueryable")
         field_count: Optional[int] = Field(None, description="", alias="fieldCount")
         organization: Optional[SalesforceOrganization] = Field(
             None, description="", alias="organization"
@@ -26108,14 +26002,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SalesforceField(Salesforce):
     """Description"""
 
+    type_name: str = Field("SalesforceField", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SalesforceField":
+            raise ValueError("must be SalesforceField")
+        return v
+
     def __setattr__(self, name, value):
         if name in SalesforceField._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "data_type",
@@ -26322,22 +26224,14 @@
 
     @object.setter
     def object(self, object: Optional[SalesforceObject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.object = object
 
-    type_name: str = Field("SalesforceField", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SalesforceField":
-            raise ValueError("must be SalesforceField")
-        return v
-
     class Attributes(Salesforce.Attributes):
         data_type: Optional[str] = Field(None, description="", alias="dataType")
         object_qualified_name: Optional[str] = Field(
             None, description="", alias="objectQualifiedName"
         )
         order: Optional[int] = Field(None, description="", alias="order")
         inline_help_text: Optional[str] = Field(
@@ -26380,14 +26274,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SalesforceOrganization(Salesforce):
     """Description"""
 
+    type_name: str = Field("SalesforceOrganization", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SalesforceOrganization":
+            raise ValueError("must be SalesforceOrganization")
+        return v
+
     def __setattr__(self, name, value):
         if name in SalesforceOrganization._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_id",
@@ -26432,22 +26334,14 @@
 
     @dashboards.setter
     def dashboards(self, dashboards: Optional[list[SalesforceDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboards = dashboards
 
-    type_name: str = Field("SalesforceOrganization", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SalesforceOrganization":
-            raise ValueError("must be SalesforceOrganization")
-        return v
-
     class Attributes(Salesforce.Attributes):
         source_id: Optional[str] = Field(None, description="", alias="sourceId")
         reports: Optional[list[SalesforceReport]] = Field(
             None, description="", alias="reports"
         )  # relationship
         objects: Optional[list[SalesforceObject]] = Field(
             None, description="", alias="objects"
@@ -26462,14 +26356,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SalesforceDashboard(Salesforce):
     """Description"""
 
+    type_name: str = Field("SalesforceDashboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SalesforceDashboard":
+            raise ValueError("must be SalesforceDashboard")
+        return v
+
     def __setattr__(self, name, value):
         if name in SalesforceDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_id",
@@ -26525,22 +26427,14 @@
 
     @organization.setter
     def organization(self, organization: Optional[SalesforceOrganization]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.organization = organization
 
-    type_name: str = Field("SalesforceDashboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SalesforceDashboard":
-            raise ValueError("must be SalesforceDashboard")
-        return v
-
     class Attributes(Salesforce.Attributes):
         source_id: Optional[str] = Field(None, description="", alias="sourceId")
         dashboard_type: Optional[str] = Field(
             None, description="", alias="dashboardType"
         )
         report_count: Optional[int] = Field(None, description="", alias="reportCount")
         reports: Optional[list[SalesforceReport]] = Field(
@@ -26556,14 +26450,22 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SalesforceReport(Salesforce):
     """Description"""
 
+    type_name: str = Field("SalesforceReport", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SalesforceReport":
+            raise ValueError("must be SalesforceReport")
+        return v
+
     def __setattr__(self, name, value):
         if name in SalesforceReport._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_id",
@@ -26619,22 +26521,14 @@
 
     @dashboards.setter
     def dashboards(self, dashboards: Optional[list[SalesforceDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboards = dashboards
 
-    type_name: str = Field("SalesforceReport", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SalesforceReport":
-            raise ValueError("must be SalesforceReport")
-        return v
-
     class Attributes(Salesforce.Attributes):
         source_id: Optional[str] = Field(None, description="", alias="sourceId")
         report_type: Optional[dict[str, str]] = Field(
             None, description="", alias="reportType"
         )
         detail_columns: Optional[set[str]] = Field(
             None, description="", alias="detailColumns"
@@ -26652,29 +26546,29 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QlikStream(QlikSpace):
     """Description"""
 
-    def __setattr__(self, name, value):
-        if name in QlikStream._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
     type_name: str = Field("QlikStream", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikStream":
             raise ValueError("must be QlikStream")
         return v
 
+    def __setattr__(self, name, value):
+        if name in QlikStream._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
 
 Referenceable.update_forward_refs()
 AtlasGlossary.update_forward_refs()
 
 Referenceable.Attributes.update_forward_refs()
 
 Asset.Attributes.update_forward_refs()
```

### Comparing `pyatlan-0.1.3/pyatlan/model/atlan_image.py` & `pyatlan-0.2.0/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/model/core.py` & `pyatlan-0.2.0/pyatlan/model/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from pyatlan.model.enums import AnnouncementType, EntityStatus
 
 CAMEL_CASE_OVERRIDES = {
     "IndexTypeEsFields": "IndexTypeESFields",
     "sourceUrl": "sourceURL",
     "sourceEmbedUrl": "sourceEmbedURL",
     "sql_dbt_sources": "sqlDBTSources",
+    "purpose_atlan_tags": "purposeClassifications",
+    "mapped_atlan_tag_name": "mappedClassificationName",
 }
 
 
 def to_camel_case(value: str) -> str:
     if not isinstance(value, str):
         raise ValueError("Value must be a string")
     if value == "__root__":
@@ -36,92 +38,96 @@
         value = value[2:]
     return f"{value[0].lower()}{value[1:]}"
 
 
 def to_snake_case(value):
     if value.startswith("__"):
         value = value[2:]
+    if value == "purposeClassifications":
+        return "purpose_atlan_tags"
+    elif value == "mappedClassificationName":
+        return "mapped_atlan_tag_name"
     res = [value[0].lower()]
     for c in (
         value.replace("URL", "Url").replace("DBT", "Dbt").replace("GDPR", "Gdpr")[1:]
     ):
         if c in "ABCDEFGHIJKLMNOPQRSTUVWXYZ":
             res.append("_")
             res.append(c.lower())
         else:
             res.append(c)
     return "".join(res).replace(" _", "_").replace(" ", "_")
 
 
-class ClassificationName:
+class AtlanTagName:
     def __init__(self, display_text: str):
-        from pyatlan.cache.classification_cache import ClassificationCache
+        from pyatlan.cache.atlan_tag_cache import AtlanTagCache
 
-        if not ClassificationCache.get_id_for_name(display_text):
+        if not AtlanTagCache.get_id_for_name(display_text):
             raise ValueError(f"{display_text} is not a valid Classification")
         self._display_text = display_text
 
     @classmethod
     def __get_validators__(cls):
         yield cls._convert_to_display_text
 
     def __str__(self):
         return self._display_text
 
     def __repr__(self):
-        return f"ClassificationName({self._display_text.__repr__()})"
+        return f"AtlanTagName({self._display_text.__repr__()})"
 
     def __hash__(self):
         return self._display_text.__hash__()
 
     def __eq__(self, other):
         return (
-            isinstance(other, ClassificationName)
+            isinstance(other, AtlanTagName)
             and self._display_text == other._display_text
         )
 
     @classmethod
     def _convert_to_display_text(cls, data):
-        from pyatlan.cache.classification_cache import ClassificationCache
+        from pyatlan.cache.atlan_tag_cache import AtlanTagCache
 
-        if isinstance(data, ClassificationName):
+        if isinstance(data, AtlanTagName):
             return data
-        if display_text := ClassificationCache.get_name_for_id(data):
-            return ClassificationName(display_text)
+        if display_text := AtlanTagCache.get_name_for_id(data):
+            return AtlanTagName(display_text)
         else:
-            raise ValueError(f"{data} is not a valid Classification")
+            raise ValueError(f"{data} is not a valid AtlanTag")
 
     @staticmethod
-    def json_encode_classification(classification_name: "ClassificationName"):
-        from pyatlan.cache.classification_cache import ClassificationCache
+    def json_encode_atlan_tag(atlan_tag_name: "AtlanTagName"):
+        from pyatlan.cache.atlan_tag_cache import AtlanTagCache
 
-        return ClassificationCache.get_id_for_name(classification_name._display_text)
+        return AtlanTagCache.get_id_for_name(atlan_tag_name._display_text)
 
 
 class AtlanObject(BaseModel):
     class Config:
         allow_population_by_field_name = True
         alias_generator = to_camel_case
         extra = Extra.ignore
         json_encoders = {
             datetime: lambda v: int(v.timestamp() * 1000),
-            "ClassificationName": ClassificationName.json_encode_classification,
+            "AtlanTagName": AtlanTagName.json_encode_atlan_tag,
         }
         validate_assignment = True
 
 
 @dataclass
 class Announcement:
     announcement_title: str
     announcement_message: Optional[str]
     announcement_type: AnnouncementType
 
 
-class Classification(AtlanObject):
-    type_name: Optional[ClassificationName] = Field(
+class AtlanTag(AtlanObject):
+    type_name: Optional[AtlanTagName] = Field(
         None,
         description="Name of the type definition that defines this instance.\n",
         alias="typeName",
     )
     entity_guid: Optional[str] = Field(
         None,
         description="Unique identifier of the entity instance.\n",
@@ -140,16 +146,16 @@
     )
     restrict_propagation_through_lineage: Optional[bool] = Field(
         None, description="", alias="restrictPropagationThroughLineage"
     )
     validity_periods: Optional[list[str]] = Field(None, alias="validityPeriods")
 
 
-class Classifications(AtlanObject):
-    __root__: list[Classification] = Field(
+class AtlanTags(AtlanObject):
+    __root__: list[AtlanTag] = Field(
         default_factory=list, description="classifications"
     )
 
 
 class Meaning(AtlanObject):
     term_guid: str = Field(
         description="Unique identifier (GUID) of the related term.",
```

### Comparing `pyatlan-0.1.3/pyatlan/model/custom_metadata.py` & `pyatlan-0.2.0/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/model/enums.py` & `pyatlan-0.2.0/pyatlan/model/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
     ) -> "AtlanConnectorType":
         obj = str.__new__(cls, value)
         obj._value_ = value
         obj.category = category
         return obj
 
     def to_qualified_name(self):
-        return f"default/{self.value}/{int(datetime.now().timestamp() * 1000)}"
+        return f"default/{self.value}/{int(datetime.now().timestamp())}"
 
     SNOWFLAKE = ("snowflake", AtlanConnectionCategory.WAREHOUSE)
     TABLEAU = ("tableau", AtlanConnectionCategory.BI)
     REDSHIFT = ("redshift", AtlanConnectionCategory.WAREHOUSE)
     POSTGRES = ("postgres", AtlanConnectionCategory.DATABASE)
     ATHENA = ("athena", AtlanConnectionCategory.QUERY_ENGINE)
     DATABRICKS = ("databricks", AtlanConnectionCategory.LAKE)
```

### Comparing `pyatlan-0.1.3/pyatlan/model/group.py` & `pyatlan-0.2.0/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/model/lineage.py` & `pyatlan-0.2.0/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/model/query.py` & `pyatlan-0.2.0/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/model/response.py` & `pyatlan-0.2.0/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/model/role.py` & `pyatlan-0.2.0/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/model/search.py` & `pyatlan-0.2.0/pyatlan/model/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pydantic import (
     ConfigDict,
     Field,
     StrictBool,
     StrictFloat,
     StrictInt,
     StrictStr,
+    constr,
     validate_arguments,
     validator,
 )
 
 from pyatlan.model.core import AtlanObject
 from pyatlan.model.enums import AtlanConnectorType, SortOrder
 
@@ -366,16 +367,18 @@
     @classmethod
     @validate_arguments()
     def with_created_by(cls, value: StrictStr):
         return cls(field=TermAttributes.CREATED_BY.value, value=value)
 
     @classmethod
     @validate_arguments()
-    def with_glossary(cls, value: StrictStr):
-        return cls(field=TermAttributes.GLOSSARY.value, value=value)
+    def with_glossary(
+        cls, qualified_name: constr(strip_whitespace=True, min_length=1, strict=True)  # type: ignore
+    ):
+        return cls(field=TermAttributes.GLOSSARY.value, value=qualified_name)
 
     @classmethod
     @validate_arguments()
     def with_guid(cls, value: StrictStr):
         # Use a GUID as a Query Term
         return cls(field=TermAttributes.GUID.value, value=value)
 
@@ -398,15 +401,15 @@
     @classmethod
     @validate_arguments()
     def with_modified_by(cls, value: StrictStr):
         return cls(field=TermAttributes.MODIFIED_BY.value, value=value)
 
     @classmethod
     @validate_arguments()
-    def with_name(cls, value: StrictStr):
+    def with_name(cls, value: constr(strip_whitespace=True, min_length=1, strict=True)):  # type: ignore
         return cls(field=TermAttributes.NAME.value, value=value)
 
     @classmethod
     @validate_arguments()
     def with_owner_groups(cls, value: StrictStr):
         return cls(field=TermAttributes.OWNER_GROUPS.value, value=value)
 
@@ -569,15 +572,15 @@
                     q.should.extend(qx.should)
                 # not all are required, add a should list to the must with proper min_should_match
                 else:
                     q.must.append(
                         Bool(should=qx.should, minimum_should_match=min_should_match)
                     )
         else:
-            if not (q.must or q.filter) and q.should:
+            if not q.must and not q.filter and q.should:
                 q.minimum_should_match = 1
             q.must.append(other)
         return q
 
     __rand__ = __and__
 
     def to_dict(self) -> dict[Any, Any]:
@@ -1743,17 +1746,16 @@
     order: Optional[SortOrder] = None
 
     def to_dict(self):
         return {self.field: {"order": self.order.value}}
 
     @validator("order", always=True)
     def validate_order(cls, v, values):
-        if not v:
-            if "field" in values:
-                v = SortOrder.ASCENDING
+        if not v and "field" in values:
+            v = SortOrder.ASCENDING
         return v
 
 
 class DSL(AtlanObject):
     from_: int = Field(0, alias="from")
     size: int = 100
     track_total_hits: bool = Field(True, alias="track_total_hits")
@@ -1766,21 +1768,54 @@
 
     def __init__(__pydantic_self__, **data: Any) -> None:
         super().__init__(**data)
         __pydantic_self__.__fields_set__.update(["from_", "size", "track_total_hits"])
 
     @validator("query", always=True)
     def validate_query(cls, v, values):
-        if not v and ("post_filter" not in values or not values["post_filter"]):
+        if v or "post_filter" in values and values["post_filter"]:
+            return v
+        else:
             raise ValueError("Either query or post_filter is required")
-        return v
 
 
 class IndexSearchRequest(AtlanObject):
     dsl: DSL
     attributes: list[str] = Field(default_factory=list)
     relation_attributes: list[str] = Field(
         default_factory=list, alias="relationAttributes"
     )
 
     class Config:
         json_encoders = {Query: lambda v: v.to_dict(), SortItem: lambda v: v.to_dict()}
+
+
+def with_active_glossary(name: StrictStr) -> "Bool":
+    return (
+        Term.with_state("ACTIVE")
+        + Term.with_type_name("AtlasGlossary")
+        + Term.with_name(name)
+    )
+
+
+def with_active_category(
+    name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+    glossary_qualified_name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+) -> Bool:
+    return (
+        Term.with_state("ACTIVE")
+        + Term.with_type_name("AtlasGlossaryCategory")
+        + Term.with_name(name)
+        + Term.with_glossary(glossary_qualified_name)
+    )
+
+
+def with_active_term(
+    name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+    glossary_qualified_name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+) -> Bool:
+    return (
+        Term.with_state("ACTIVE")
+        + Term.with_type_name("AtlasGlossaryTerm")
+        + Term.with_name(name)
+        + Term.with_glossary(glossary_qualified_name)
+    )
```

### Comparing `pyatlan-0.1.3/pyatlan/model/structs.py` & `pyatlan-0.2.0/pyatlan/model/structs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -37,80 +37,40 @@
         None, description="", alias="awsCloudWatchMetricName"
     )
     aws_cloud_watch_metric_scope: "str" = Field(
         None, description="", alias="awsCloudWatchMetricScope"
     )
 
 
-class Histogram(AtlanObject):
-    """Description"""
-
-    boundaries: "set[float]" = Field(None, description="", alias="boundaries")
-    frequencies: "set[float]" = Field(None, description="", alias="frequencies")
-
-
 class KafkaTopicConsumption(AtlanObject):
     """Description"""
 
     topic_name: Optional["str"] = Field(None, description="", alias="topicName")
     topic_partition: Optional["str"] = Field(
         None, description="", alias="topicPartition"
     )
     topic_lag: Optional["int"] = Field(None, description="", alias="topicLag")
     topic_current_offset: Optional["int"] = Field(
         None, description="", alias="topicCurrentOffset"
     )
 
 
-class ColumnValueFrequencyMap(AtlanObject):
-    """Description"""
-
-    column_value: Optional["str"] = Field(None, description="", alias="columnValue")
-    column_value_frequency: Optional["int"] = Field(
-        None, description="", alias="columnValueFrequency"
-    )
-
-
-class SourceTagAttachment(AtlanObject):
+class Histogram(AtlanObject):
     """Description"""
 
-    source_tag_name: Optional["str"] = Field(
-        None, description="", alias="sourceTagName"
-    )
-    source_tag_qualified_name: Optional["str"] = Field(
-        None, description="", alias="sourceTagQualifiedName"
-    )
-    source_tag_guid: Optional["str"] = Field(
-        None, description="", alias="sourceTagGuid"
-    )
-    source_tag_connector_name: Optional["str"] = Field(
-        None, description="", alias="sourceTagConnectorName"
-    )
-    source_tag_value: Optional["list[SourceTagAttachmentValue]"] = Field(
-        None, description="", alias="sourceTagValue"
-    )
-    is_source_tag_synced: Optional["bool"] = Field(
-        None, description="", alias="isSourceTagSynced"
-    )
-    source_tag_sync_timestamp: Optional["datetime"] = Field(
-        None, description="", alias="sourceTagSyncTimestamp"
-    )
-    source_tag_sync_error: Optional["str"] = Field(
-        None, description="", alias="sourceTagSyncError"
-    )
+    boundaries: "set[float]" = Field(None, description="", alias="boundaries")
+    frequencies: "set[float]" = Field(None, description="", alias="frequencies")
 
 
-class SourceTagAttachmentValue(AtlanObject):
+class ColumnValueFrequencyMap(AtlanObject):
     """Description"""
 
-    tag_attachment_key: Optional["str"] = Field(
-        None, description="", alias="tagAttachmentKey"
-    )
-    tag_attachment_value: Optional["str"] = Field(
-        None, description="", alias="tagAttachmentValue"
+    column_value: Optional["str"] = Field(None, description="", alias="columnValue")
+    column_value_frequency: Optional["int"] = Field(
+        None, description="", alias="columnValueFrequency"
     )
 
 
 class BadgeCondition(AtlanObject):
     """Description"""
 
     @classmethod
@@ -145,14 +105,54 @@
         None, description="", alias="badgeConditionValue"
     )
     badge_condition_colorhex: Optional["str"] = Field(
         None, description="", alias="badgeConditionColorhex"
     )
 
 
+class SourceTagAttachmentValue(AtlanObject):
+    """Description"""
+
+    tag_attachment_key: Optional["str"] = Field(
+        None, description="", alias="tagAttachmentKey"
+    )
+    tag_attachment_value: Optional["str"] = Field(
+        None, description="", alias="tagAttachmentValue"
+    )
+
+
+class SourceTagAttachment(AtlanObject):
+    """Description"""
+
+    source_tag_name: Optional["str"] = Field(
+        None, description="", alias="sourceTagName"
+    )
+    source_tag_qualified_name: Optional["str"] = Field(
+        None, description="", alias="sourceTagQualifiedName"
+    )
+    source_tag_guid: Optional["str"] = Field(
+        None, description="", alias="sourceTagGuid"
+    )
+    source_tag_connector_name: Optional["str"] = Field(
+        None, description="", alias="sourceTagConnectorName"
+    )
+    source_tag_value: Optional["list[SourceTagAttachmentValue]"] = Field(
+        None, description="", alias="sourceTagValue"
+    )
+    is_source_tag_synced: Optional["bool"] = Field(
+        None, description="", alias="isSourceTagSynced"
+    )
+    source_tag_sync_timestamp: Optional["datetime"] = Field(
+        None, description="", alias="sourceTagSyncTimestamp"
+    )
+    source_tag_sync_error: Optional["str"] = Field(
+        None, description="", alias="sourceTagSyncError"
+    )
+
+
 class AzureTag(AtlanObject):
     """Description"""
 
     azure_tag_key: "str" = Field(None, description="", alias="azureTagKey")
     azure_tag_value: "str" = Field(None, description="", alias="azureTagValue")
 
 
@@ -170,14 +170,21 @@
 class AwsTag(AtlanObject):
     """Description"""
 
     aws_tag_key: "str" = Field(None, description="", alias="awsTagKey")
     aws_tag_value: "str" = Field(None, description="", alias="awsTagValue")
 
 
+class GoogleTag(AtlanObject):
+    """Description"""
+
+    google_tag_key: "str" = Field(None, description="", alias="googleTagKey")
+    google_tag_value: "str" = Field(None, description="", alias="googleTagValue")
+
+
 class DbtMetricFilter(AtlanObject):
     """Description"""
 
     dbt_metric_filter_column_qualified_name: Optional["str"] = Field(
         None, description="", alias="dbtMetricFilterColumnQualifiedName"
     )
     dbt_metric_filter_field: Optional["str"] = Field(
@@ -187,21 +194,14 @@
         None, description="", alias="dbtMetricFilterOperator"
     )
     dbt_metric_filter_value: Optional["str"] = Field(
         None, description="", alias="dbtMetricFilterValue"
     )
 
 
-class GoogleTag(AtlanObject):
-    """Description"""
-
-    google_tag_key: "str" = Field(None, description="", alias="googleTagKey")
-    google_tag_value: "str" = Field(None, description="", alias="googleTagValue")
-
-
 class AuthPolicyValiditySchedule(AtlanObject):
     """Description"""
 
     policy_validity_schedule_start_time: "str" = Field(
         None, description="", alias="policyValidityScheduleStartTime"
     )
     policy_validity_schedule_end_time: "str" = Field(
```

### Comparing `pyatlan-0.1.3/pyatlan/model/typedef.py` & `pyatlan-0.2.0/pyatlan/model/typedef.py`

 * *Files 2% similar despite different names*

```diff
@@ -462,15 +462,15 @@
         description="List of attributes that should be available in the type_ definition.",
     )
     service_type: Optional[str] = Field(
         None, description="Internal use only.", example="atlan"
     )
 
 
-class ClassificationDef(TypeDef):
+class AtlanTagDef(TypeDef):
     attribute_defs: Optional[List[Dict[str, Any]]] = Field(description="Unused.")
     category: AtlanTypeCategory = AtlanTypeCategory.CLASSIFICATION
     display_name: str = Field(
         description="Name used for display purposes (in user interfaces)."
     )
     entity_types: Optional[List[str]] = Field(
         description="A list of the entity types that this classification can be used against."
@@ -495,15 +495,15 @@
 
     @staticmethod
     def create(
         name: str,
         color: AtlanClassificationColor,
         icon: AtlanIcon = AtlanIcon.ATLAN_TAG,
         image: Optional[AtlanImage] = None,
-    ) -> ClassificationDef:
+    ) -> AtlanTagDef:
         from pyatlan.model.assets import validate_required_fields
 
         validate_required_fields(
             ["name", "color"],
             [name, color],
         )
         cls_options = {
@@ -514,15 +514,15 @@
             cls_options["imageID"] = str(image.id)
             cls_options["iconType"] = IconType.IMAGE.value
         else:
             cls_options["imageID"] = ""
             cls_options["iconType"] = IconType.ICON.value
 
         # Explicitly set all defaults to ensure inclusion during pydantic serialization
-        return ClassificationDef(
+        return AtlanTagDef(
             category=AtlanTypeCategory.CLASSIFICATION,
             name=name,
             display_name=name,
             options=cls_options,
             skip_display_name_uniqueness_check=False,
         )
 
@@ -656,16 +656,18 @@
 class TypeDefResponse(AtlanObject):
     enum_defs: List[EnumDef] = Field(
         [], description="List of enumeration type definitions."
     )
     struct_defs: List[StructDef] = Field(
         [], description="List of struct type definitions."
     )
-    classification_defs: List[ClassificationDef] = Field(
-        [], description="List of classification type definitions."
+    atlan_tag_defs: List[AtlanTagDef] = Field(
+        [],
+        description="List of classification type definitions.",
+        alias="classificationDefs",
     )
     entity_defs: List[EntityDef] = Field(
         [], description="List of entity type_ definitions."
     )
     relationship_defs: List[RelationshipDef] = Field(
         [], description="List of relationship type_ definitions."
     )
```

### Comparing `pyatlan-0.1.3/pyatlan/model/user.py` & `pyatlan-0.2.0/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/multipart_data_generator.py` & `pyatlan-0.2.0/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan/utils.py` & `pyatlan-0.2.0/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.2.0/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.1.3
+Version: 0.2.0
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.1.3/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.2.0/pyatlan.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,77 +12,84 @@
 pyatlan.egg-info/PKG-INFO
 pyatlan.egg-info/SOURCES.txt
 pyatlan.egg-info/dependency_links.txt
 pyatlan.egg-info/not-zip-safe
 pyatlan.egg-info/requires.txt
 pyatlan.egg-info/top_level.txt
 pyatlan/cache/__init__.py
-pyatlan/cache/classification_cache.py
+pyatlan/cache/atlan_tag_cache.py
 pyatlan/cache/custom_metadata_cache.py
 pyatlan/cache/enum_cache.py
 pyatlan/cache/group_cache.py
 pyatlan/cache/role_cache.py
 pyatlan/cache/user_cache.py
 pyatlan/client/__init__.py
 pyatlan/client/atlan.py
 pyatlan/client/constants.py
+pyatlan/events/__init__.py
+pyatlan/events/atlan_event_handler.py
+pyatlan/events/atlan_lambda_handler.py
 pyatlan/generator/__init__.py
 pyatlan/generator/generate_from_typdefs.py
 pyatlan/generator/templates/__init__.py
 pyatlan/model/__init__.py
 pyatlan/model/assets.py
 pyatlan/model/atlan_image.py
 pyatlan/model/core.py
 pyatlan/model/custom_metadata.py
 pyatlan/model/enums.py
+pyatlan/model/events.py
 pyatlan/model/group.py
 pyatlan/model/internal.py
 pyatlan/model/lineage.py
 pyatlan/model/query.py
 pyatlan/model/response.py
 pyatlan/model/role.py
 pyatlan/model/search.py
 pyatlan/model/structs.py
 pyatlan/model/typedef.py
 pyatlan/model/user.py
 tests/__init__.py
 tests/integration/__init__.py
 tests/integration/admin_test.py
-tests/integration/classification_test.py
+tests/integration/atlan_tag_test.py
 tests/integration/client.py
 tests/integration/conftest.py
 tests/integration/connection_test.py
 tests/integration/custom_metadata_test.py
+tests/integration/file_test.py
 tests/integration/glossary_test.py
 tests/integration/lineage_test.py
 tests/integration/persona_test.py
 tests/integration/purpose_test.py
 tests/integration/query_parser_test.py
 tests/integration/s3_asset_test.py
 tests/integration/test_client.py
 tests/integration/test_index_search.py
 tests/integration/test_sql_assets.py
 tests/unit/__init__.py
 tests/unit/conftest.py
-tests/unit/test_classification_name.py
+tests/unit/test_atlan_tag_name.py
 tests/unit/test_client.py
 tests/unit/test_custom_metadata.py
+tests/unit/test_events.py
 tests/unit/test_glossary_term.py
 tests/unit/test_lineage.py
 tests/unit/test_model.py
 tests/unit/test_search_model.py
 tests/unit/test_typedef_model.py
 tests/unit/test_utils.py
 tests/unit/model/__init__.py
 tests/unit/model/badge_condition_test.py
 tests/unit/model/badge_test.py
 tests/unit/model/column_test.py
 tests/unit/model/connection_test.py
 tests/unit/model/constants.py
 tests/unit/model/database_test.py
+tests/unit/model/file_test.py
 tests/unit/model/glossary_category_test.py
 tests/unit/model/glossary_term_test.py
 tests/unit/model/glossary_test.py
 tests/unit/model/materialised_view_test.py
 tests/unit/model/process_test.py
 tests/unit/model/readme_test.py
 tests/unit/model/s3_bucket_test.py
```

### Comparing `pyatlan-0.1.3/setup.py` & `pyatlan-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/integration/admin_test.py` & `pyatlan-0.2.0/tests/integration/admin_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/integration/client.py` & `pyatlan-0.2.0/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/integration/connection_test.py` & `pyatlan-0.2.0/tests/integration/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/integration/custom_metadata_test.py` & `pyatlan-0.2.0/tests/integration/custom_metadata_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -750,15 +750,15 @@
     raci[CM_ATTR_RACI_CONSULTED] = [group1.name]
     raci[CM_ATTR_RACI_INFORMED] = [group1.name, group2.name]
     raci[CM_ATTR_RACI_EXTRA] = "something extra..."
     to_update = AtlasGlossaryTerm.create_for_modification(
         qualified_name=term.qualified_name, name=term.name, glossary_guid=glossary.guid
     )
     to_update.set_custom_metadata(custom_metadata=raci)
-    response = client.upsert_replacing_cm(to_update, replace_classifications=False)
+    response = client.upsert_replacing_cm(to_update, replace_atlan_tagss=False)
     assert response
     assert len(response.assets_deleted(asset_type=AtlasGlossaryTerm)) == 0
     assert len(response.assets_created(asset_type=AtlasGlossaryTerm)) == 0
     assert len(response.assets_updated(asset_type=AtlasGlossaryTerm)) == 1
     t = response.assets_updated(asset_type=AtlasGlossaryTerm)[0]
     assert isinstance(t, AtlasGlossaryTerm)
     assert t.guid == term.guid
```

### Comparing `pyatlan-0.1.3/tests/integration/lineage_test.py` & `pyatlan-0.2.0/tests/integration/lineage_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/integration/persona_test.py` & `pyatlan-0.2.0/tests/integration/persona_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/integration/purpose_test.py` & `pyatlan-0.2.0/tests/integration/purpose_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,39 +11,38 @@
     AssetSidebarTab,
     AtlanClassificationColor,
     AuthPolicyType,
     DataAction,
     DataMaskingType,
     PurposeMetadataAction,
 )
-from pyatlan.model.typedef import ClassificationDef
+from pyatlan.model.typedef import AtlanTagDef
 from tests.integration.client import TestId, delete_asset
 
 MODULE_NAME = TestId.make_unique("Purpose")
 
 
 @pytest.fixture(scope="module")
 def atlan_tag(
     client: AtlanClient,
-) -> Generator[ClassificationDef, None, None]:
-    classification_def = ClassificationDef.create(
+) -> Generator[AtlanTagDef, None, None]:
+    atlan_tag_def = AtlanTagDef.create(
         name=MODULE_NAME, color=AtlanClassificationColor.GREEN
     )
-    yield client.create_typedef(classification_def).classification_defs[0]
-    client.purge_typedef(MODULE_NAME, typedef_type=ClassificationDef)
+    typedef = client.create_typedef(atlan_tag_def)
+    yield typedef.atlan_tag_defs[0]
+    client.purge_typedef(MODULE_NAME, typedef_type=AtlanTagDef)
 
 
 @pytest.fixture(scope="module")
 def purpose(
     client: AtlanClient,
-    atlan_tag: ClassificationDef,
+    atlan_tag: AtlanTagDef,
 ) -> Generator[Purpose, None, None]:
-    to_create = Purpose.create(
-        name=MODULE_NAME, classifications=[atlan_tag.display_name]
-    )
+    to_create = Purpose.create(name=MODULE_NAME, atlan_tags=[atlan_tag.display_name])
     response = client.upsert(to_create)
     p = response.assets_created(asset_type=Purpose)[0]
     yield p
     delete_asset(client, guid=p.guid, asset_type=Purpose)
 
 
 def test_purpose(
```

### Comparing `pyatlan-0.1.3/tests/integration/query_parser_test.py` & `pyatlan-0.2.0/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/integration/s3_asset_test.py` & `pyatlan-0.2.0/tests/integration/s3_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/integration/test_client.py` & `pyatlan-0.2.0/tests/integration/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,31 +242,31 @@
     glossary = client.get_asset_by_qualified_name(
         qualified_name=qualified_name, asset_type=AtlasGlossary
     )
     assert glossary.attributes.qualified_name == qualified_name
 
 
 def test_add_classification(client: AtlanClient, term1: AtlasGlossaryTerm):
-    client.add_classifications(
+    client.add_atlan_tags(
         AtlasGlossaryTerm, term1.qualified_name, [CLASSIFICATION_NAME]
     )
     glossary_term = client.get_asset_by_guid(term1.guid, asset_type=AtlasGlossaryTerm)
-    assert glossary_term.classifications
-    assert len(glossary_term.classifications) == 1
-    classification = glossary_term.classifications[0]
+    assert glossary_term.atlan_tags
+    assert len(glossary_term.atlan_tags) == 1
+    classification = glossary_term.atlan_tags[0]
     assert str(classification.type_name) == CLASSIFICATION_NAME
 
 
 @pytest.mark.order(after="test_add_classification")
 def test_remove_classification(client: AtlanClient, term1: AtlasGlossaryTerm):
-    client.remove_classification(
+    client.remove_atlan_tag(
         AtlasGlossaryTerm, term1.qualified_name, CLASSIFICATION_NAME
     )
     glossary_term = client.get_asset_by_guid(term1.guid, asset_type=AtlasGlossaryTerm)
-    assert not glossary_term.classifications
+    assert not glossary_term.atlan_tags
 
 
 def test_update_certificate(client: AtlanClient, glossary: AtlasGlossary):
     message = "An important message"
     client.update_certificate(
         asset_type=AtlasGlossary,
         qualified_name=glossary.qualified_name,
```

### Comparing `pyatlan-0.1.3/tests/integration/test_index_search.py` & `pyatlan-0.2.0/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/integration/test_sql_assets.py` & `pyatlan-0.2.0/tests/integration/test_sql_assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/conftest.py` & `pyatlan-0.2.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/badge_condition_test.py` & `pyatlan-0.2.0/tests/unit/model/badge_condition_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/badge_test.py` & `pyatlan-0.2.0/tests/unit/model/badge_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/column_test.py` & `pyatlan-0.2.0/tests/unit/model/column_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/connection_test.py` & `pyatlan-0.2.0/tests/unit/model/connection_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pyatlan.model.enums import AtlanConnectorType
 from tests.unit.model.constants import CONNECTION_NAME, CONNECTION_QUALIFIED_NAME
 
 
 @pytest.mark.parametrize(
     "name, connector_type, admin_users, admin_groups, admin_roles, message",
     [
-        (None, AtlanConnectorType.SNOWFLAKE, [], [], [], "name cannot be blank"),
+        (None, AtlanConnectorType.SNOWFLAKE, [], [], [], "name is required"),
         (CONNECTION_NAME, None, [], [], [], "connector_type is required"),
         (
             CONNECTION_NAME,
             AtlanConnectorType.SNOWFLAKE,
             [],
             [],
             [],
```

### Comparing `pyatlan-0.1.3/tests/unit/model/constants.py` & `pyatlan-0.2.0/tests/unit/model/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,7 +22,10 @@
 CONNECTION_QUALIFIED_NAME = f"{DEFAULT}/{CONNECTOR_TYPE}/{TIME_STAMP}"
 DATABASE_QUALIFIED_NAME = f"{CONNECTION_QUALIFIED_NAME}/{DATABASE_NAME}"
 SCHEMA_QUALIFIED_NAME = f"{DATABASE_QUALIFIED_NAME}/{SCHEMA_NAME}"
 TABLE_QUALIFIED_NAME = f"{SCHEMA_QUALIFIED_NAME}/{TABLE_NAME}"
 VIEW_QUALIFIED_NAME = f"{SCHEMA_QUALIFIED_NAME}/{VIEW_NAME}"
 TABLE_COLUMN_QUALIFIED_NAME = f"{TABLE_QUALIFIED_NAME}/{COLUMN_NAME}"
 VIEW_COLUMN_QUALIFIED_NAME = f"{VIEW_QUALIFIED_NAME}/{COLUMN_NAME}"
+FILE_NAME = "file.pdf"
+FILE_CONNECTION_QUALIFIED_NAME = "default/api/1686535364"
+FILE_QUALIFIED_NAME = f"{FILE_CONNECTION_QUALIFIED_NAME}/{FILE_NAME}"
```

### Comparing `pyatlan-0.1.3/tests/unit/model/database_test.py` & `pyatlan-0.2.0/tests/unit/model/database_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     DATABASE_QUALIFIED_NAME,
 )
 
 
 @pytest.mark.parametrize(
     "name, connection_qualified_name, message",
     [
-        (None, "connection/name", "name cannot be blank"),
+        (None, "connection/name", "name is required"),
         (DATABASE_NAME, None, "connection_qualified_name is required"),
         (DATABASE_NAME, "abc", "Invalid connection_qualified_name"),
         (DATABASE_NAME, "default/snowflake", "Invalid connection_qualified_name"),
         (
             DATABASE_NAME,
             "default/snowflke/1686532494/RAW",
             "Invalid connection_qualified_name",
```

### Comparing `pyatlan-0.1.3/tests/unit/model/glossary_category_test.py` & `pyatlan-0.2.0/tests/unit/model/glossary_category_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 from pyatlan.model.assets import AtlasGlossary, AtlasGlossaryCategory
 from tests.unit.model.constants import (
+    GLOSSARY_CATEGORY_NAME,
+    GLOSSARY_CATEGORY_QUALIFIED_NAME,
     GLOSSARY_NAME,
     GLOSSARY_QUALIFIED_NAME,
-    GLOSSARY_TERM_NAME,
-    GLOSSARY_TERM_QUALIFIED_NAME,
 )
 
 ANCHOR = AtlasGlossary.create_for_modification(
     qualified_name=GLOSSARY_QUALIFIED_NAME, name=GLOSSARY_NAME
 )
 GLOSSARY_GUID = "123"
 PARENT_CATEGORY = AtlasGlossaryCategory.create_for_modification(
@@ -50,33 +50,33 @@
     ],
 )
 def test_create(
     anchor: AtlasGlossary,
     parent_category: AtlasGlossaryCategory,
 ):
     sut = AtlasGlossaryCategory.create(
-        name=GLOSSARY_TERM_NAME,
+        name=GLOSSARY_CATEGORY_NAME,
         anchor=anchor,
         parent_category=parent_category,
     )
 
-    assert sut.name == GLOSSARY_TERM_NAME
+    assert sut.name == GLOSSARY_CATEGORY_NAME
     assert sut.qualified_name
     assert sut.parent_category == parent_category
     assert sut.anchor == anchor
 
 
 @pytest.mark.parametrize(
     "name, qualified_name, glossary_guid, message",
     [
-        (None, GLOSSARY_TERM_QUALIFIED_NAME, GLOSSARY_GUID, "name is required"),
-        (GLOSSARY_TERM_NAME, None, GLOSSARY_GUID, "qualified_name is required"),
+        (None, GLOSSARY_CATEGORY_QUALIFIED_NAME, GLOSSARY_GUID, "name is required"),
+        (GLOSSARY_CATEGORY_NAME, None, GLOSSARY_GUID, "qualified_name is required"),
         (
-            GLOSSARY_TERM_NAME,
-            GLOSSARY_TERM_QUALIFIED_NAME,
+            GLOSSARY_CATEGORY_NAME,
+            GLOSSARY_CATEGORY_QUALIFIED_NAME,
             None,
             "glossary_guid is required",
         ),
     ],
 )
 def test_create_for_modification_with_invalid_parameter_raises_value_error(
     name: str, qualified_name: str, glossary_guid: str, message: str
@@ -85,43 +85,43 @@
         AtlasGlossaryCategory.create_for_modification(
             qualified_name=qualified_name, name=name, glossary_guid=glossary_guid
         )
 
 
 def test_create_for_modification():
     sut = AtlasGlossaryCategory.create_for_modification(
-        qualified_name=GLOSSARY_TERM_QUALIFIED_NAME,
-        name=GLOSSARY_TERM_NAME,
+        qualified_name=GLOSSARY_CATEGORY_QUALIFIED_NAME,
+        name=GLOSSARY_CATEGORY_NAME,
         glossary_guid=GLOSSARY_GUID,
     )
 
-    assert sut.name == GLOSSARY_TERM_NAME
-    assert sut.qualified_name == GLOSSARY_TERM_QUALIFIED_NAME
+    assert sut.name == GLOSSARY_CATEGORY_NAME
+    assert sut.qualified_name == GLOSSARY_CATEGORY_QUALIFIED_NAME
     assert sut.anchor.guid == GLOSSARY_GUID
 
 
 def test_trim_to_required():
     sut = AtlasGlossaryCategory.create_for_modification(
-        qualified_name=GLOSSARY_TERM_QUALIFIED_NAME,
-        name=GLOSSARY_TERM_NAME,
+        qualified_name=GLOSSARY_CATEGORY_QUALIFIED_NAME,
+        name=GLOSSARY_CATEGORY_NAME,
         glossary_guid=GLOSSARY_GUID,
     ).trim_to_required()
 
-    assert sut.name == GLOSSARY_TERM_NAME
-    assert sut.qualified_name == GLOSSARY_TERM_QUALIFIED_NAME
+    assert sut.name == GLOSSARY_CATEGORY_NAME
+    assert sut.qualified_name == GLOSSARY_CATEGORY_QUALIFIED_NAME
     assert sut.anchor.guid == GLOSSARY_GUID
 
 
 @pytest.mark.parametrize(
     "anchor",
     [(None), (AtlasGlossary())],
 )
 def test_trim_to_required_raises_value_error_when_anchor_is_none(anchor):
     sut = AtlasGlossaryCategory.create_for_modification(
-        qualified_name=GLOSSARY_TERM_QUALIFIED_NAME,
-        name=GLOSSARY_TERM_NAME,
+        qualified_name=GLOSSARY_CATEGORY_QUALIFIED_NAME,
+        name=GLOSSARY_CATEGORY_NAME,
         glossary_guid=GLOSSARY_GUID,
     )
     sut.anchor = anchor
 
     with pytest.raises(ValueError, match="anchor.guid must be available"):
         sut.trim_to_required()
```

### Comparing `pyatlan-0.1.3/tests/unit/model/glossary_term_test.py` & `pyatlan-0.2.0/tests/unit/model/glossary_term_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/glossary_test.py` & `pyatlan-0.2.0/tests/unit/model/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/materialised_view_test.py` & `pyatlan-0.2.0/tests/unit/model/materialised_view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/process_test.py` & `pyatlan-0.2.0/tests/unit/model/process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/readme_test.py` & `pyatlan-0.2.0/tests/unit/model/readme_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/s3_bucket_test.py` & `pyatlan-0.2.0/tests/unit/model/s3_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/s3object_test.py` & `pyatlan-0.2.0/tests/unit/model/s3object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/schema_test.py` & `pyatlan-0.2.0/tests/unit/model/schema_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/table_test.py` & `pyatlan-0.2.0/tests/unit/model/table_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/model/view_test.py` & `pyatlan-0.2.0/tests/unit/model/view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/test_custom_metadata.py` & `pyatlan-0.2.0/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/test_glossary_term.py` & `pyatlan-0.2.0/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/test_lineage.py` & `pyatlan-0.2.0/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/test_model.py` & `pyatlan-0.2.0/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.3/tests/unit/test_search_model.py` & `pyatlan-0.2.0/tests/unit/test_search_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,23 @@
     Regexp,
     SortItem,
     SortOrder,
     Term,
     TermAttributes,
     Terms,
     Wildcard,
+    with_active_category,
+    with_active_glossary,
+    with_active_term,
+)
+from tests.unit.model.constants import (
+    GLOSSARY_CATEGORY_NAME,
+    GLOSSARY_NAME,
+    GLOSSARY_QUALIFIED_NAME,
+    GLOSSARY_TERM_NAME,
 )
 
 NOW = datetime.now()
 VALUES_BY_TYPE: dict[Union[type, object], Union[str, datetime, object]] = {
     StrictStr: "abc",
     StrictBool: True,
     datetime: NOW,
@@ -480,15 +489,15 @@
     b = q1 & q2
     assert b.to_dict() == expected
 
 
 @pytest.fixture()
 def with_name(request):
     attribute = request.param
-    return "with_" + attribute.name.lower()
+    return f"with_{attribute.name.lower()}"
 
 
 def test_terms_to_dict():
     assert Terms(field="name", values=["john", "dave"]).to_dict() == {
         "terms": {"name": ["john", "dave"]}
     }
 
@@ -811,15 +820,15 @@
     )
 
 
 @pytest.mark.parametrize(
     "name, value, fuzziness, max_expansions, prefix_length, transpositions, rewrite, attributes, incompatable",
     [
         (
-            "with_" + a.name.lower(),
+            f"with_{a.name.lower()}",
             "ki",
             "AUTO",
             3,
             0,
             1,
             "constant_score",
             a,
@@ -1208,7 +1217,153 @@
             minimum_should_match=minimum_should_match,
             zero_terms_query=zero_terms_query,
             max_expansions=max_expansions,
             prefix_length=prefix_length,
         ).to_dict()
         == expected
     )
+
+
+@pytest.mark.parametrize(
+    "name, message",
+    [
+        (
+            None,
+            "1 validation error for WithName\nvalue\n  none is not an allowed value",
+        ),
+        (
+            " ",
+            "1 validation error for WithName\nvalue\n  ensure this value has at least 1 characters",
+        ),
+    ],
+)
+def test_with_active_glossary_when_invalid_parameter_raises_value_error(name, message):
+    with pytest.raises(ValueError, match=message):
+        with_active_glossary(name)
+
+
+def test_with_active_glossary():
+
+    sut = with_active_glossary(name=GLOSSARY_NAME)
+
+    assert sut.must
+    assert 3 == len(sut.must)
+    term1, term2, term3 = sut.must
+    assert isinstance(term1, Term) is True
+    assert term1.field == "__state"
+    assert term1.value == "ACTIVE"
+    assert isinstance(term2, Term) is True
+    assert term2.field == "__typeName.keyword"
+    assert term2.value == "AtlasGlossary"
+    assert isinstance(term3, Term) is True
+    assert term3.field == "name.keyword"
+    assert term3.value == GLOSSARY_NAME
+
+
+@pytest.mark.parametrize(
+    "name, glossary_qualified_name, message",
+    [
+        (
+            None,
+            GLOSSARY_QUALIFIED_NAME,
+            "1 validation error for WithName\nvalue\n  none is not an allowed value",
+        ),
+        (
+            " ",
+            GLOSSARY_QUALIFIED_NAME,
+            "1 validation error for WithName\nvalue\n  ensure this value has at least 1 characters",
+        ),
+        (
+            GLOSSARY_CATEGORY_NAME,
+            None,
+            "1 validation error for WithGlossary\nqualified_name\n  none is not an allowed value",
+        ),
+        (
+            GLOSSARY_CATEGORY_NAME,
+            " ",
+            "1 validation error for WithGlossary\nqualified_name\n  ensure this value has at least 1 characters",
+        ),
+    ],
+)
+def test_with_active_category_when_invalid_parameter_raises_value_error(
+    name, glossary_qualified_name, message
+):
+    with pytest.raises(ValueError, match=message):
+        with_active_category(name=name, glossary_qualified_name=glossary_qualified_name)
+
+
+def test_with_active_category():
+
+    sut = with_active_category(
+        name=GLOSSARY_CATEGORY_NAME, glossary_qualified_name=GLOSSARY_QUALIFIED_NAME
+    )
+
+    assert sut.must
+    assert 4 == len(sut.must)
+    term1, term2, term3, term4 = sut.must
+    assert isinstance(term1, Term) is True
+    assert term1.field == "__state"
+    assert term1.value == "ACTIVE"
+    assert isinstance(term2, Term) is True
+    assert term2.field == "__typeName.keyword"
+    assert term2.value == "AtlasGlossaryCategory"
+    assert isinstance(term3, Term) is True
+    assert term3.field == "name.keyword"
+    assert term3.value == GLOSSARY_CATEGORY_NAME
+    assert isinstance(term4, Term) is True
+    assert term4.field == "__glossary"
+    assert term4.value == GLOSSARY_QUALIFIED_NAME
+
+
+@pytest.mark.parametrize(
+    "name, glossary_qualified_name, message",
+    [
+        (
+            None,
+            GLOSSARY_QUALIFIED_NAME,
+            "1 validation error for WithName\nvalue\n  none is not an allowed value",
+        ),
+        (
+            " ",
+            GLOSSARY_QUALIFIED_NAME,
+            "1 validation error for WithName\nvalue\n  ensure this value has at least 1 characters",
+        ),
+        (
+            GLOSSARY_TERM_NAME,
+            None,
+            "1 validation error for WithGlossary\nqualified_name\n  none is not an allowed value",
+        ),
+        (
+            GLOSSARY_TERM_NAME,
+            " ",
+            "1 validation error for WithGlossary\nqualified_name\n  ensure this value has at least 1 characters",
+        ),
+    ],
+)
+def test_with_active_term_when_invalid_parameter_raises_value_error(
+    name, glossary_qualified_name, message
+):
+    with pytest.raises(ValueError, match=message):
+        with_active_term(name=name, glossary_qualified_name=glossary_qualified_name)
+
+
+def test_with_active_term():
+
+    sut = with_active_term(
+        name=GLOSSARY_TERM_NAME, glossary_qualified_name=GLOSSARY_QUALIFIED_NAME
+    )
+
+    assert sut.must
+    assert 4 == len(sut.must)
+    term1, term2, term3, term4 = sut.must
+    assert isinstance(term1, Term) is True
+    assert term1.field == "__state"
+    assert term1.value == "ACTIVE"
+    assert isinstance(term2, Term) is True
+    assert term2.field == "__typeName.keyword"
+    assert term2.value == "AtlasGlossaryTerm"
+    assert isinstance(term3, Term) is True
+    assert term3.field == "name.keyword"
+    assert term3.value == GLOSSARY_TERM_NAME
+    assert isinstance(term4, Term) is True
+    assert term4.field == "__glossary"
+    assert term4.value == GLOSSARY_QUALIFIED_NAME
```

### Comparing `pyatlan-0.1.3/tests/unit/test_typedef_model.py` & `pyatlan-0.2.0/tests/unit/test_typedef_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 import pytest
 
 from pyatlan.model.core import to_camel_case, to_snake_case
 from pyatlan.model.enums import AtlanTypeCategory
 from pyatlan.model.typedef import (
-    ClassificationDef,
+    AtlanTagDef,
     CustomMetadataDef,
     EntityDef,
     EnumDef,
     RelationshipDef,
     StructDef,
     TypeDef,
     TypeDefResponse,
@@ -207,15 +207,15 @@
         attribute_defs = STRUCT_DEF["attributeDefs"][index]
         for key in attribute_def.__dict__.keys():
             check_attribute(attribute_def, key, attribute_defs)
 
 
 def test_classification_def(type_defs):
     for classification_def_json in type_defs["classificationDefs"]:
-        classification_def = ClassificationDef(**classification_def_json)
+        classification_def = AtlanTagDef(**classification_def_json)
         assert classification_def.category == AtlanTypeCategory.CLASSIFICATION
         check_type_def_properties(classification_def, classification_def_json)
         check_has_attributes(classification_def, classification_def_json)
 
 
 def check_has_attributes(type_def: TypeDef, type_def_json: dict):
     for key in type_def_json:
```

