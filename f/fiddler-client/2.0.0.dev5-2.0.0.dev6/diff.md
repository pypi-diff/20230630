# Comparing `tmp/fiddler-client-2.0.0.dev5.tar.gz` & `tmp/fiddler-client-2.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-2.0.0.dev5.tar", last modified: Fri Jun 16 00:06:47 2023, max compression
+gzip compressed data, was "fiddler-client-2.0.0.dev6.tar", last modified: Thu Jun 29 07:27:03 2023, max compression
```

## Comparing `fiddler-client-2.0.0.dev5.tar` & `fiddler-client-2.0.0.dev6.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.658751 fiddler-client-2.0.0.dev5/
--rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1000) docker    (1001)    19816 2023-06-16 00:06:47.658751 fiddler-client-2.0.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)    16156 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/PUBLIC.md
--rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/README.md
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.650751 fiddler-client-2.0.0.dev5/fiddler/
--rw-r--r--   0 runner    (1000) docker    (1001)     9468 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/_version.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.650751 fiddler-client-2.0.0.dev5/fiddler/assets/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/assets/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/assets/pg_reserved_words.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5105 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/client.py
--rw-r--r--   0 runner    (1000) docker    (1001)    21393 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/connection.py
--rw-r--r--   0 runner    (1000) docker    (1001)      354 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/constants.py
--rw-r--r--   0 runner    (1000) docker    (1001)   128501 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/core_objects.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4721 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2786 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)    26077 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/fiddler_api.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/libs/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6446 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/libs/http_client.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5056 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)    17897 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/monitoring_validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/packtools/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/packtools/template_model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1808 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/project.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)     4370 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3213 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/formatting.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/general_checks.py
--rw-r--r--   0 runner    (1000) docker    (1001)      782 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/helper.py
--rw-r--r--   0 runner    (1000) docker    (1001)      188 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/logging.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5010 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/pandas.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/v2/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/v2/api/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)    16048 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/alert_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2140 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6602 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/baseline_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15923 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/dataset_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14948 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/events_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15328 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/explainability_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4725 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4502 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/job_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/model_artifact_deploy.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3066 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/model_deployment_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    16988 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/model_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2937 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/project_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1241 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/constants.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/v2/schema/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4923 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/alert.py
--rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/base.py
--rw-r--r--   0 runner    (1000) docker    (1001)      490 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/baseline.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3071 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)      885 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/events.py
--rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/job.py
--rw-r--r--   0 runner    (1000) docker    (1001)      453 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1085 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/model_deployment.py
--rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/project.py
--rw-r--r--   0 runner    (1000) docker    (1001)      364 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/server_info.py
--rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/user.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/v2/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3144 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/utils/decorators.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2306 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/utils/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1835 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/utils/response_handler.py
--rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/utils/validations.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/v2/validators/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/validators/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1498 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/validators/dataset_validator.py
--rw-r--r--   0 runner    (1000) docker    (1001)    13986 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1000) docker    (1001)    19816 2023-06-16 00:06:47.000000 fiddler-client-2.0.0.dev5/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)     2073 2023-06-16 00:06:47.000000 fiddler-client-2.0.0.dev5/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-06-16 00:06:47.000000 fiddler-client-2.0.0.dev5/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) docker    (1001)      203 2023-06-16 00:06:47.000000 fiddler-client-2.0.0.dev5/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-06-16 00:06:47.000000 fiddler-client-2.0.0.dev5/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-06-16 00:06:47.658751 fiddler-client-2.0.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1000) docker    (1001)     1375 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/setup.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.658751 fiddler-client-2.0.0.dev5/tests/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1787 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/tests/test_fiddler_api.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/
+-rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1000) docker    (1001)    20044 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)    16360 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/PUBLIC.md
+-rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/README.md
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.121202 fiddler-client-2.0.0.dev6/fiddler/
+-rw-r--r--   0 runner    (1000) docker    (1001)     2019 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/_version.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.121202 fiddler-client-2.0.0.dev6/fiddler/assets/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/assets/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/assets/pg_reserved_words.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5105 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/client.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    21393 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/connection.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      354 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/constants.py
+-rw-r--r--   0 runner    (1000) docker    (1001)   127839 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/core_objects.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4721 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2786 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    26077 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/fiddler_api.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.121202 fiddler-client-2.0.0.dev6/fiddler/libs/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6455 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/libs/http_client.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5056 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    17897 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/monitoring_validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.121202 fiddler-client-2.0.0.dev6/fiddler/packtools/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/packtools/template_model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1808 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/project.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.121202 fiddler-client-2.0.0.dev6/fiddler/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)     4370 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3213 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/formatting.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/general_checks.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      782 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/helper.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      188 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/logging.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5010 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/pandas.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.121202 fiddler-client-2.0.0.dev6/fiddler/v2/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/fiddler/v2/api/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14561 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/alert_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2603 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6602 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/baseline_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15923 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/dataset_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14948 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/events_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15328 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/explainability_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4725 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4502 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/job_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/model_artifact_deploy.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3066 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/model_deployment_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    16989 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/model_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2937 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/project_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1241 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/constants.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/fiddler/v2/schema/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4635 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/alert.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/base.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      490 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/baseline.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3071 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      885 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/events.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/job.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      453 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1107 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/model_deployment.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/project.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      364 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/server_info.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/user.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/fiddler/v2/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3144 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/utils/decorators.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2306 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/utils/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1835 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/utils/response_handler.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/utils/validations.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/fiddler/v2/validators/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/validators/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1498 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/validators/dataset_validator.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    13986 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1000) docker    (1001)    20044 2023-06-29 07:27:03.000000 fiddler-client-2.0.0.dev6/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)     2073 2023-06-29 07:27:03.000000 fiddler-client-2.0.0.dev6/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-06-29 07:27:03.000000 fiddler-client-2.0.0.dev6/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)      203 2023-06-29 07:27:03.000000 fiddler-client-2.0.0.dev6/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-06-29 07:27:03.000000 fiddler-client-2.0.0.dev6/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/setup.cfg
+-rw-r--r--   0 runner    (1000) docker    (1001)     1375 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/setup.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/tests/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2080 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/tests/test_fiddler_api.py
```

### Comparing `fiddler-client-2.0.0.dev5/PKG-INFO` & `fiddler-client-2.0.0.dev6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 2.0.0.dev5
+Version: 2.0.0.dev6
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
         
@@ -41,20 +41,23 @@
               - list_org_roles
               - unshare_project
               - share_project
               - process_avro
               - process_csv
           - #### **New Features**
             - Add `monitor_components` as an attribute of `CustomFeature`. Default to `False`
-            - Add `columns` as a parameter in `add_alert_rule` and `get_alert_rules` functions
+            - Remove `column` as a parameter in `add_alert_rule` and `get_alert_rules` functions
+            
         ### 1.8.0
           - #### **Modifications**
             - Add new alert type -  `statistic` for setting alerts
             - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
               `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
+            - Add `columns` as a parameter in `add_alert_rule` and `get_alert_rules` functions
+            - Add deprecation warning for `column` as a parameter in `add_alert_rule` and `get_alert_rules` functions
         
         ### 1.7.4
           - #### **Modification**
             - Do not typecast column with strings in get_slice()
         
         ### 1.7.3
           - #### **Modification**
```

### Comparing `fiddler-client-2.0.0.dev5/PUBLIC.md` & `fiddler-client-2.0.0.dev6/PUBLIC.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,23 @@
       - list_org_roles
       - unshare_project
       - share_project
       - process_avro
       - process_csv
   - #### **New Features**
     - Add `monitor_components` as an attribute of `CustomFeature`. Default to `False`
-    - Add `columns` as a parameter in `add_alert_rule` and `get_alert_rules` functions
+    - Remove `column` as a parameter in `add_alert_rule` and `get_alert_rules` functions
+    
 ### 1.8.0
   - #### **Modifications**
     - Add new alert type -  `statistic` for setting alerts
     - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
       `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
+    - Add `columns` as a parameter in `add_alert_rule` and `get_alert_rules` functions
+    - Add deprecation warning for `column` as a parameter in `add_alert_rule` and `get_alert_rules` functions
 
 ### 1.7.4
   - #### **Modification**
     - Do not typecast column with strings in get_slice()
 
 ### 1.7.3
   - #### **Modification**
```

### Comparing `fiddler-client-2.0.0.dev5/README.md` & `fiddler-client-2.0.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/assets/pg_reserved_words.py` & `fiddler-client-2.0.0.dev6/fiddler/assets/pg_reserved_words.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/client.py` & `fiddler-client-2.0.0.dev6/fiddler/client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/connection.py` & `fiddler-client-2.0.0.dev6/fiddler/connection.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/core_objects.py` & `fiddler-client-2.0.0.dev6/fiddler/core_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,14 @@
 
     FLOAT = 'float'
     INTEGER = 'int'
     BOOLEAN = 'bool'
     STRING = 'str'
     CATEGORY = 'category'
     TIMESTAMP = 'timestamp'
-    EMBEDDINGS = 'embeddings'
 
     def is_numeric(self):
         return self.value in (DataType.INTEGER.value, DataType.FLOAT.value)
 
     def is_bool_or_cat(self):
         return self.value in (DataType.BOOLEAN.value, DataType.CATEGORY.value)
 
@@ -589,14 +588,15 @@
             res['is-nullable'] = self.is_nullable
         if self.value_range_min is not None:
             res['value-range-min'] = self.value_range_min
         if self.value_range_max is not None:
             res['value-range-max'] = self.value_range_max
         return res
 
+
     @staticmethod
     def _value_is_na_or_none(value):
         if value is None:
             return True
         # This needs to be added because when we add `pandas._libs.missing.NAType` type in rabbitmq.
         # When we read the message, it converts the value to the "<NA>".
         if isinstance(value, str):
@@ -741,16 +741,14 @@
             return DataType.FLOAT
         if pd.api.types.is_integer_dtype(pd_dtype):
             return DataType.INTEGER
         if pd.api.types.is_bool_dtype(pd_dtype):
             return DataType.BOOLEAN
         if pd.api.types.is_categorical_dtype(pd_dtype):
             return DataType.CATEGORY
-        if pd_dtype == 'ndarray':
-            return DataType.EMBEDDINGS
 
         return DataType.STRING
 
     @classmethod
     def update_stats_for_existing_schema(
         cls, dataset: dict, info, max_inferred_cardinality: Optional[int] = None
     ):
@@ -858,54 +856,47 @@
             df = df.reset_index(inplace=False)
         name_series_iter = df.items()
         for column_name, column_series in name_series_iter:
             column_info = cls._calculate_stats_for_col(
                 column_name,
                 column_series,
                 max_inferred_cardinality,
-                data_type_version=CURRENT_DATA_TYPE_VERSION,
+                data_type_version=CURRENT_DATA_TYPE_VERSION
             )
             columns.append(column_info)
         return cls(
             display_name,
             columns,
             dataset_id=dataset_id,
             data_type_version=CURRENT_DATA_TYPE_VERSION,
         )
 
     @staticmethod
     def _calculate_stats_for_col(
         column_name,
         column_series,
         max_inferred_cardinality,
-        data_type_version: Optional[str] = 'v0',
-    ):
+        data_type_version:Optional[str]='v0'):
         # @TODO Automatically drop the empty column with warning and proceed instead of aborting the upload
         if column_series.isna().all():
             raise ValueError(
                 f'Column {column_name} is empty. '
                 f'Please remove it and re-upload the dataset.'
             )
 
         # if we infer string or categorical, ensure that the underlying data
         # is also string by casting it.
 
         # FDL-10905: dropna is needed to take care of cases where having None changes
         # data type of int, float, bool to category. dropna() won't change
         # is_nullable detection as column_series.dropna() returns a new instance.
         column_series_dropped_na = column_series.dropna()
-        pd_column_dtype = column_series_dropped_na.infer_objects().dtype
-        if pd_column_dtype == 'object':
-            column_count = column_series_dropped_na.shape[0]
-            for i in range(column_count):
-                if isinstance(column_series_dropped_na[i], np.ndarray):
-                    pd_column_dtype = 'ndarray'
-                    break
-
-        column_dtype = DatasetInfo.datatype_from_pandas_dtype(pd_column_dtype)
+        column_dtype = DatasetInfo.datatype_from_pandas_dtype(
+            column_series_dropped_na.infer_objects().dtype
+        )
         # get nullability before any datatype modifications like 'astype'
         # which distorts None values.
         is_nullable = bool(column_series.isna().any())
 
         if column_dtype in [DataType.CATEGORY, DataType.STRING]:
             if 'mixed' in pd.api.types.infer_dtype(column_series):
                 LOG.warning(
@@ -925,17 +916,15 @@
             column_dtype = DataType.CATEGORY
 
         # get possible values for categorical type
         if column_dtype.is_bool_or_cat():
             # Only when data_type_version is 'v0',
             # categorical column values undergo int/bool -> float -> string conversion.
             if data_type_version == 'v0':
-                possible_values = np.sort(
-                    column_series_dropped_na.astype(str).unique()
-                ).tolist()
+                possible_values = np.sort(column_series_dropped_na.astype(str).unique()).tolist()
                 possible_values_floats = None
                 if column_dtype.value == DataType.CATEGORY.value:
                     try:
                         possible_values_floats = [
                             str(float(raw_val)) for raw_val in possible_values
                         ]
                     except ValueError:
@@ -1245,16 +1234,15 @@
         self.data_type_version = data_type_version
 
         self.is_binary_ranking_model = is_binary_ranking_model
 
         self._validate_columns()
 
         self.target_class_order = self.get_target_class_order(
-            self.target_class_order, self.model_task, self.targets[0]
-        )
+            self.target_class_order, self.model_task, self.targets[0])
 
         if model_task == ModelTask.RANKING:
             if group_by is None:
                 raise ValueError(
                     'The argument group_by cannot be empty for Ranking models'
                 )
             self.is_binary_ranking_model = len(self.target_class_order) == 2
@@ -1348,28 +1336,23 @@
                 )
             if len(self.custom_features) > MAX_NUMBER_OF_CUSTOM_FEATURES:
                 raise ValueError(
                     f'The maximum number of custom features in a project cannot exceed {MAX_NUMBER_OF_CUSTOM_FEATURES}. {len(self.custom_features)} custom features are defined.'
                 )
 
             available_cols = (
-                self.get_input_names()
-                + self.get_target_names()
-                + self.get_metadata_names()
+                self.get_input_names() + self.get_target_names() + self.get_metadata_names()
             )
             numeric_cols = self.get_input_pandas_dtypes()
             if self.metadata:
                 numeric_cols.update(self.get_metadata_pandas_dtypes())
             if self.targets:
                 numeric_cols.update(self.get_target_pandas_dtypes())
-            valid_col_names = [
-                k
-                for k, v in numeric_cols.items()
-                if v in (DataType.INTEGER.value, DataType.FLOAT.value)
-            ]
+            valid_col_names = [k for k, v in numeric_cols.items() if
+                               v in (DataType.INTEGER.value, DataType.FLOAT.value)]
 
             unique_cf_names = []
             for feature in self.custom_features:
 
                 if not isinstance(feature, CustomFeature):
                     raise ValueError(
                         'The custom_features argument only accepts a list of CustomFeature objects.'
@@ -1410,15 +1393,15 @@
         res = {
             'name': self.display_name,
             'input-type': self.input_type.value,
             'model-task': self.model_task.value,
             'inputs': [c.to_dict() for c in self.inputs],
             'outputs': [c.to_dict() for c in self.outputs],
             'datasets': self.datasets or [],
-            'targets': [target_col.to_dict() for target_col in self.targets],
+            'targets': [target_col.to_dict() for target_col in self.targets]
         }
         if self.target_class_order is not None:
             res['target-class-order'] = self.target_class_order
         if self.metadata:
             res['metadata'] = [metadata_col.to_dict() for metadata_col in self.metadata]
         if self.decisions:
             res['decisions'] = [
@@ -2292,14 +2275,15 @@
             return None
 
         output_columns = []
         ds_info_names_columns = {}
         for ds_column in dataset_info.columns:
             ds_info_names_columns[ds_column.name] = ds_column
 
+
         if model_task.is_classification():
             if isinstance(output_names, dict):
                 output_names = list(output_names.keys())
             for name in output_names:
                 if name in ds_info_names_columns:
                     output_columns.append(ds_info_names_columns[name])
                 else:
@@ -2321,18 +2305,15 @@
                     raise ValueError(
                         f'If outputs is a dictionary, the values should '
                         f'be a tuple of 2 values. Currently passing: '
                         f'{values} for output {name}. Please correct.'
                     )
                 if name in ds_info_names_columns:
                     column = ds_info_names_columns[name]
-                    if not (
-                        column.data_type == DataType.FLOAT
-                        or column.data_type == DataType.INTEGER
-                    ):
+                    if not (column.data_type == DataType.FLOAT or column.data_type == DataType.INTEGER):
                         raise ValueError(
                             f'Column {name} with type {column.data_type} can not be specified as output.'
                             f'Output column type has to be either INTEGER or FLOAT.'
                             f'Please correct.'
                         )
                     column.value_range_min = min(values)
                     column.value_range_max = max(values)
@@ -2358,18 +2339,15 @@
                         col = target_column.name
                     else:
                         raise ValueError(
                             f'Output {name} is not present in the dataset. '
                             f'Please provide a dictionary with the range: '
                             f'{name}: (min_value, max_value).'
                         )
-                if (
-                    dataset_info[col].value_range_min is None
-                    or dataset_info[col].value_range_max is None
-                ):
+                if dataset_info[col].value_range_min is None or dataset_info[col].value_range_max is None:
                     raise ValueError(
                         f'Column {name} with value_range_min or value_range_max as None can not be specified as output.'
                         f'Please correct.'
                     )
                 output_columns.append(
                     Column(
                         name=name,
```

### Comparing `fiddler-client-2.0.0.dev5/fiddler/dataset.py` & `fiddler-client-2.0.0.dev6/fiddler/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/exceptions.py` & `fiddler-client-2.0.0.dev6/fiddler/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/fiddler_api.py` & `fiddler-client-2.0.0.dev6/fiddler/fiddler_api.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/libs/http_client.py` & `fiddler-client-2.0.0.dev6/fiddler/libs/http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         request_headers = self.headers
         # override/update headers coming from the calling method
         if headers:
             request_headers = deepcopy(self.headers)
             request_headers.update(headers)
 
         content_type = request_headers.get('Content-Type')
-        if content_type == APP_JSON_CONTENT_TYPE:
+        if data and content_type == APP_JSON_CONTENT_TYPE:
             data = json.dumps(data)
 
         kwargs.setdefault('allow_redirects', True)
         # requests is not able to pass the value of self.session.verify to the
         # verify param in kwargs when REQUESTS_CA_BUNDLE is set.
         # So setting that as default here
         kwargs.setdefault('verify', self.session.verify)
```

### Comparing `fiddler-client-2.0.0.dev5/fiddler/model.py` & `fiddler-client-2.0.0.dev6/fiddler/model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/monitoring_validator.py` & `fiddler-client-2.0.0.dev6/fiddler/monitoring_validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/packtools/gem.py` & `fiddler-client-2.0.0.dev6/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/packtools/keras_ig_helpers.py` & `fiddler-client-2.0.0.dev6/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/packtools/project_attributions_helpers.py` & `fiddler-client-2.0.0.dev6/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/packtools/template_model.py` & `fiddler-client-2.0.0.dev6/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/project.py` & `fiddler-client-2.0.0.dev6/fiddler/project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/utils/__init__.py` & `fiddler-client-2.0.0.dev6/fiddler/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/utils/exceptions.py` & `fiddler-client-2.0.0.dev6/fiddler/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/utils/formatting.py` & `fiddler-client-2.0.0.dev6/fiddler/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/utils/general_checks.py` & `fiddler-client-2.0.0.dev6/fiddler/utils/general_checks.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/utils/helper.py` & `fiddler-client-2.0.0.dev6/fiddler/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/utils/pandas.py` & `fiddler-client-2.0.0.dev6/fiddler/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/api/alert_mixin.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/api/alert_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ComparePeriod,
     CompareTo,
     Metric,
     Priority,
     TriggeredAlerts,
 )
 from fiddler.v2.utils.decorators import handle_api_error_response
-from fiddler.v2.utils.helpers import match_semvar
+from fiddler.v2.utils.helpers import match_semver
 from fiddler.v2.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -47,15 +47,14 @@
         compare_to: CompareTo,
         priority: Priority,
         critical_threshold: float,
         condition: AlertCondition,
         bin_size: BinSize = BinSize.ONE_DAY,
         baseline_id: Optional[str] = None,
         compare_period: Optional[ComparePeriod] = None,
-        column: Optional[str] = None,
         columns: Optional[List[str]] = None,
         warning_threshold: Optional[float] = None,
         notifications_config: Optional[Dict[str, Dict[str, Any]]] = None,
     ) -> AlertRule:
         """
         To add an alert rule
         :param project_id: Unique project name for which the alert rule is created
@@ -110,65 +109,47 @@
                 2) Priority.MEDIUM
                 3) Priority.HIGH
         :param warning_threshold: Threshold value to crossing which a warning level severity alert will be triggered
         :param critical_threshold: Threshold value to crossing which a critical level severity alert will be triggered
         :param condition: Select from:
                 1) AlertCondition.LESSER
                 2) AlertCondition.GREATER
-        :param column: column name on which alert rule is to be created. It can take '__ANY__' to check for all columns
         :param columns: List of column names on which alert rule is to be created. It can take ['__ANY__'] to check for all columns
         :param notifications_config: notifications config object created using helper method build_notifications_config()
         :param baseline_id: Name of the baselne, whose histogram is compared against the same derived from current data.
                             Used only when alert type is AlertType.DATA_DRIFT.
         :return: created alert rule object
         """
-        if columns and not match_semvar(self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION):
+        if columns and not match_semver(self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION):
             raise ValueError(f'columns parameter works with server version {self.GROUP_OF_COLUMNS_API_VERSION}')
 
-        if column:
-            warnings.warn(
-                'WARNING: column is deprecated in 1.8 and will be removed '
-                'from version 2.0.0. As a replacement, use columns while constructing AlertRule.',
-                DeprecationWarning,
-            )
-
-        if column and columns:
-            raise ValueError(f'Both column and columns are specified. Please use one of them.')
-
         if not notifications_config:
             notifications_config = self.build_notifications_config()
 
         if bin_size not in BinSize.keys():
             raise ValueError(f'bin_size: {bin_size} should be one of: {BinSize.keys()}')
         if compare_to == CompareTo.TIME_PERIOD and not compare_period:
             raise ValueError(
                 f'compare_period is required when compare_to is {CompareTo.TIME_PERIOD}'
             )
         if compare_period and compare_period not in ComparePeriod.keys():
             raise ValueError(f'compare_period should be one of{ComparePeriod.keys()}')
 
-        feature_name:str = None
-        feature_names:str = None
-        if match_semvar(self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION):
-            feature_names = ",".join(columns) if columns else column
-        else:
-            feature_name = column
         request_body = AlertRulePayload(
                 organization_name=self.organization_name,
                 project_name=project_id,
                 model_name=model_id,
                 name=name,
                 alert_type=alert_type,
                 metric=metric,
                 compare_to=compare_to,
                 compare_period=compare_period,
                 priority=priority,
                 baseline_name=baseline_id,
-                feature_name=feature_name,
-                feature_names=feature_names,
+                feature_names=columns,
                 warning_threshold=warning_threshold,
                 critical_threshold=critical_threshold,
                 condition=condition,
                 time_bucket=bin_size,
                 notifications=notifications_config,
             ).dict()
         response = self.client.post(
@@ -198,15 +179,14 @@
     @handle_api_error_response
     def get_alert_rules(
         self,
         project_id: Optional[str] = None,
         model_id: Optional[str] = None,
         alert_type: Optional[AlertType] = None,
         metric: Optional[Metric] = None,
-        column: Optional[str] = None,
         columns: Optional[List[str]] = None,
         baseline_id: Optional[str] = None,
         ordering: Optional[List[str]] = None,
         offset: int = 0,
         limit: int = 20,
     ) -> List[AlertRule]:
         """
@@ -239,43 +219,32 @@
                     1) MetricType.PSI
                     2) MetricType.JSD
 
                 For data_integrity:
                     1) MetricType.RANGE_VIOLATION
                     2) MetricType.MISSING_VALUE
                     3) MetricType.TYPE_VIOLATION
-        :param column: Filter based on the column
         :param columns: Filter based on a list of column names
         :param limit: Number of records to be retrieved per page, also referred as page_size
         :param offset: Pointer to the starting of the page index. offset of the first page is 0
                         and it increments by limit for each page, for e.g., 5th pages offset when
                         limit=100 will be (5 - 1) * 100 = 400. This means 5th page will contain
                         records from index 400 to 499.
         :return: paginated list of alert rules for the set filters
         """
-        if columns and not match_semvar(self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION):
+        if columns and not match_semver(self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION):
             raise ValueError(f'columns parameter works with server version {self.GROUP_OF_COLUMNS_API_VERSION}')
 
-        if column:
-            warnings.warn(
-                'WARNING: column is deprecated in 1.8 and will be removed '
-                'from version 2.0.0. As a replacement, use columns while constructing AlertRule.',
-                DeprecationWarning,
-            )
-
-        if column and columns:
-            raise ValueError(f'Both column and columns are specified. Please use one of them.')
-
         alert_params = {
             'organization_name': self.organization_name,
             'offset': offset,
             'limit': limit,
         }
 
-        if match_semvar(
+        if match_semver(
             self.server_info.server_version, self.FILTER_ALERT_RULES_API_VERSION
         ):
             filter_by_rules = []
             if project_id:
                 filter_by_rules.append(
                     {'field': 'project_name', 'operator': 'equal', 'value': project_id}
                 )
@@ -293,17 +262,15 @@
             if metric:
                 filter_by_rules.append(
                     {'field': 'metric', 'operator': 'equal', 'value': metric}
                 )
 
             if columns:
                 filter_by_rules.append({'field': 'feature_names', 'operator': 'contains', 'value': columns})
-            elif column:
-                filter_by_rules.append({'field': 'feature_name', 'operator': 'equal', 'value': column})
-
+            
             if baseline_id:
                 filter_by_rules.append(
                     {
                         'field': 'baseline_name',
                         'operator': 'equal',
                         'value': baseline_id,
                     }
```

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/api/api.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/api/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 from fiddler.v2.api.explainability_mixin import ExplainabilityMixin
 from fiddler.v2.api.job_mixin import JobMixin
 from fiddler.v2.api.model_deployment_mixin import ModelDeploymentMixin
 from fiddler.v2.api.model_mixin import ModelMixin
 from fiddler.v2.api.project_mixin import ProjectMixin
 from fiddler.v2.constants import CURRENT_API_VERSION, FIDDLER_CLIENT_VERSION_HEADER
 from fiddler.v2.schema.server_info import ServerInfo
+from fiddler.v2.utils.helpers import match_semver, raise_not_supported
 
 logger = logging.getLogger(__name__)
 
+
 class FiddlerClient(
     ModelMixin,
     DatasetMixin,
     ProjectMixin,
     EventsMixin,
     JobMixin,
     BaselineMixin,
@@ -48,15 +50,27 @@
         self.request_headers.update({FIDDLER_CLIENT_VERSION_HEADER: f'{__version__}'})
         self.timeout = timeout
         self.client = RequestClient(
             base_url=self.url, headers=self.request_headers, verify=verify
         )
 
         self.server_info: ServerInfo = self._get_server_info()
+        self._check_server_version()
 
     def _get_server_info(self) -> ServerInfo:
         response = self.client.get(
             url='server-info',
             params={'organization_name': self.organization_name},
         )
 
         return ServerInfo(**response.json().get('data'))
+
+    def _check_server_version(self) -> bool:
+        if match_semver(
+            self.server_info.server_version,
+            '<23.2.0',
+        ):
+            raise_not_supported(
+                compatible_client_version='1.8',
+                client_version=__version__,
+                server_version=self.server_info.server_version,
+            )
```

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/api/baseline_mixin.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/api/baseline_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/api/dataset_mixin.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/api/dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/api/events_mixin.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/api/events_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/api/explainability_mixin.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/api/explainability_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/api/helpers.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/api/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/api/job_mixin.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/api/job_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/api/model_artifact_deploy.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/api/model_artifact_deploy.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/api/model_deployment_mixin.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/api/model_deployment_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/api/model_mixin.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/api/model_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                 f'object. Instead, found value of type {type(model_info)}'
             )
 
         # associate dataset_id with model_info. This was not done during
         # from_dataset_info call.
         model_info.datasets = [dataset_name]
 
-        model = self.add_model_call(
+        model = self._add_model_call(
             model_name=model_name,
             project_name=project_name,
             info=model_info,
         )
         BaselineMixin.add_baseline(
             project_name=project_name,
             model_name=model_name,
```

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/api/project_mixin.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/api/project_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/constants.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/constants.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/schema/alert.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/schema/alert.py`

 * *Files 10% similar despite different names*

```diff
@@ -135,16 +135,15 @@
 class AlertRulePayload(BaseDataSchema):
     organization_name: str
     project_name: str
     model_name: str
     name: str
     alert_type: AlertType
     metric: Metric
-    feature_name: Optional[str]
-    feature_names: Optional[str]
+    feature_names: Optional[List[str]]
     priority: Priority
     compare_to: CompareTo
     baseline_name: Optional[str]
     compare_period: Optional[ComparePeriod]
     warning_threshold: Optional[float]
     critical_threshold: float
     condition: AlertCondition
@@ -156,45 +155,37 @@
     alert_rule_uuid: str = Field(alias='uuid')
     organization_name: str
     project_id: str = Field(alias='project_name')
     model_id: str = Field(alias='model_name')
     name: Optional[str]
     alert_type: AlertType
     metric: Metric
-    columns: Optional[List[str]]
+    columns: Optional[List[str]] = Field(alias='feature_names')
     baseline_id: Optional[str] = Field(alias='baseline_name')
     priority: Priority
     compare_to: CompareTo
     compare_period: Optional[ComparePeriod]
     warning_threshold: Optional[float]
     critical_threshold: float
     condition: AlertCondition
     bin_size: BinSize = Field(alias='time_bucket')
 
     @root_validator(pre=True)
     def set_compare_period(cls, values) -> Optional[ComparePeriod]:
-
         if values['compare_period'] == 0:
             values['compare_period'] = None
         return values
 
-    @root_validator(pre=True)
-    def set_feature_names(cls, values) -> Optional[List[str]]:
-        if 'feature_names' in values:
-            values['columns'] = list(map(lambda x: x.strip(), values['feature_names'].split(",")))
-        else:
-            values['columns'] = None
-        return values
 
 class TriggeredAlerts(BaseDataSchema):
     id: int
     triggered_alert_id: str = Field(alias='uuid')
     alert_rule_uuid: str = Field(alias='alert_config_uuid')
     alert_run_start_time: int
     alert_time_bucket: int
-    alert_value: float
+    alert_value: Dict[str, float]
     baseline_time_bucket: Optional[int]
     baseline_value: Optional[float]
     is_alert: bool
     severity: Optional[str]
     failure_reason: str
     message: str
```

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/schema/dataset.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/schema/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/schema/events.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/schema/events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/schema/model_deployment.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/schema/model_deployment.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 class ArtifactType(str, Enum):
     SURROGATE = 'SURROGATE'
     PYTHON_PACKAGE = 'PYTHON_PACKAGE'
 
 
 class DeploymentType(str, Enum):
     BASE_CONTAINER = 'BASE_CONTAINER'
+    MANUAL = 'MANUAL'
 
 
 class DeploymentParams(BaseModel):
     artifact_type: ArtifactType = ArtifactType.PYTHON_PACKAGE
     deployment_type: DeploymentType = DeploymentType.BASE_CONTAINER
     image_uri: Optional[str]
     replicas: Optional[int]
```

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/utils/decorators.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/utils/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     FiddlerAPIBadRequestException,
     FiddlerAPIForbiddenException,
     FiddlerAPIConflictException,
     FiddlerAPINotFoundException,
     FiddlerAPIInternalServerErrorException
 )
 from fiddler.utils import logging
-from fiddler.v2.utils.helpers import match_semvar
+from fiddler.v2.utils.helpers import match_semver
 
 logger = logging.getLogger(__name__)
 
 map_except_resp_code = {
     HTTPStatus.BAD_REQUEST: FiddlerAPIBadRequestException,  # 400
     HTTPStatus.FORBIDDEN: FiddlerAPIForbiddenException,  # 403
     HTTPStatus.NOT_FOUND: FiddlerAPINotFoundException,  # 404
@@ -44,15 +44,15 @@
     :param version_expr: Supported version to match with. Read more at VersionInfo.match
     :return: Decorator function
     """
 
     def decorator(func) -> Callable:
         @wraps(func)
         def wrapper(self, *args: Any, **kwargs: Any) -> Any:
-            if not match_semvar(self.server_info.server_version, version_expr):
+            if not match_semver(self.server_info.server_version, version_expr):
                 raise NotSupported(
                     f'{func.__name__} method is supported with server version '
                     f'{version_expr}, but the current server version is '
                     f'{self.server_info.server_version}'
                 )
 
             return func(self, *args, **kwargs)
```

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/utils/helpers.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import yaml
 
 from fiddler.core_objects import ModelInfo
 from fiddler.exceptions import NotSupported
 from fiddler.v2.schema.server_info import Version
 
 
-def match_semvar(version: Optional[Version], match_expr: str) -> bool:
+def match_semver(version: Optional[Version], match_expr: str) -> bool:
     """
     Match the version with match_expr
     :param version: Server version
     :param match_expr: Version to match with. Read more at VersionInfo.match
     :return: True if server version matches, otherwise False
     """
     if not version:
```

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/utils/response_handler.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/utils/response_handler.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/v2/validators/dataset_validator.py` & `fiddler-client-2.0.0.dev6/fiddler/v2/validators/dataset_validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler/validator.py` & `fiddler-client-2.0.0.dev6/fiddler/validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/fiddler_client.egg-info/PKG-INFO` & `fiddler-client-2.0.0.dev6/fiddler_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 2.0.0.dev5
+Version: 2.0.0.dev6
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
         
@@ -41,20 +41,23 @@
               - list_org_roles
               - unshare_project
               - share_project
               - process_avro
               - process_csv
           - #### **New Features**
             - Add `monitor_components` as an attribute of `CustomFeature`. Default to `False`
-            - Add `columns` as a parameter in `add_alert_rule` and `get_alert_rules` functions
+            - Remove `column` as a parameter in `add_alert_rule` and `get_alert_rules` functions
+            
         ### 1.8.0
           - #### **Modifications**
             - Add new alert type -  `statistic` for setting alerts
             - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
               `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
+            - Add `columns` as a parameter in `add_alert_rule` and `get_alert_rules` functions
+            - Add deprecation warning for `column` as a parameter in `add_alert_rule` and `get_alert_rules` functions
         
         ### 1.7.4
           - #### **Modification**
             - Do not typecast column with strings in get_slice()
         
         ### 1.7.3
           - #### **Modification**
```

### Comparing `fiddler-client-2.0.0.dev5/fiddler_client.egg-info/SOURCES.txt` & `fiddler-client-2.0.0.dev6/fiddler_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/setup.py` & `fiddler-client-2.0.0.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev5/tests/test_fiddler_api.py` & `fiddler-client-2.0.0.dev6/tests/test_fiddler_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 import pytest
 from pytest_mock import MockFixture
 
-from fiddler import FiddlerApi
-from fiddler.v2.api.api import FiddlerClient
+from fiddler import FiddlerClient
+from fiddler.exceptions import NotSupported
 from fiddler.v2.schema.server_info import ServerInfo, Version
 
 
-def test_client_v1_creation_fail():
-    with pytest.raises(ValueError):
-        FiddlerApi('', '', '')
-
-
-def test_client_v2_creation_fail():
-    with pytest.raises(ValueError):
-        FiddlerApi('', '', '', version='v2')
-
-
 def test_get_server_info_without_server_version(mocker: MockFixture):
     mocker.patch('fiddler.connection.Connection.check_connection', return_value='OK')
 
     server_info_dict = {
         'feature_flags': {
             'fairness': False,
         },
     }
 
     mock_get_server_info = mocker.patch.object(FiddlerClient, '_get_server_info')
     mock_get_server_info.return_value = ServerInfo(**server_info_dict)
 
-    client = FiddlerApi('https://test.fiddler.ai', 'test', 'foo-token', version='v2')
+    client = FiddlerClient('https://test.fiddler.ai', 'test', 'foo-token')
 
-    assert client.v2.server_info.server_version is None
-    assert client.v2.server_info.feature_flags == server_info_dict['feature_flags']
+    assert client.server_info.server_version is None
+    assert client.server_info.feature_flags == server_info_dict['feature_flags']
 
 
 def test_get_server_info_with_server_version(mocker: MockFixture):
     mocker.patch('fiddler.connection.Connection.check_connection', return_value='OK')
 
     server_info_dict = {
         'feature_flags': {
             'fairness': False,
         },
-        'server_version': '23.1.1',
+        'server_version': '23.2.0',
     }
 
     mock_get_server_info = mocker.patch.object(FiddlerClient, '_get_server_info')
     mock_get_server_info.return_value = ServerInfo(**server_info_dict)
 
-    client = FiddlerApi('https://test.fiddler.ai', 'test', 'foo-token', version='v2')
+    client = FiddlerClient('https://test.fiddler.ai', 'test', 'foo-token')
 
-    assert client.v2.server_info.server_version == Version.parse(
+    assert client.server_info.server_version == Version.parse(
         server_info_dict['server_version']
     )
-    assert client.v2.server_info.feature_flags == server_info_dict['feature_flags']
+    assert client.server_info.feature_flags == server_info_dict['feature_flags']
+
+
+def test_check_semver_incorrect_version(mocker: MockFixture):
+    mocker.patch('fiddler.connection.Connection.check_connection', return_value='OK')
+    server_info_dict = {
+        'feature_flags': {
+            'fairness': False,
+        },
+        'server_version': '22.1.0',
+    }
+
+    mock_get_server_info = mocker.patch.object(FiddlerClient, '_get_server_info')
+    mock_get_server_info.return_value = ServerInfo(**server_info_dict)
+
+    with pytest.raises(NotSupported):
+        FiddlerClient('https://test.fiddler.ai', 'test', 'foo-token')
```

