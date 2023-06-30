# Comparing `tmp/funding-service-design-utils-2.0.7.tar.gz` & `tmp/funding-service-design-utils-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funding-service-design-utils-2.0.7.tar", last modified: Wed Jun 28 13:41:33 2023, max compression
+gzip compressed data, was "funding-service-design-utils-2.0.8.tar", last modified: Fri Jun 30 10:27:47 2023, max compression
```

## Comparing `funding-service-design-utils-2.0.7.tar` & `funding-service-design-utils-2.0.8.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.321271 funding-service-design-utils-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-06-28 13:41:33.321271 funding-service-design-utils-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.317271 funding-service-design-utils-2.0.7/fsd_test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.317271 funding-service-design-utils-2.0.7/fsd_test_utils/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_test_utils/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_test_utils/fixtures/db_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.317271 funding-service-design-utils-2.0.7/fsd_test_utils/test_config/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_test_utils/test_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_test_utils/test_config/useful_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.317271 funding-service-design-utils-2.0.7/fsd_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.317271 funding-service-design-utils-2.0.7/fsd_utils/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/authentication/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/authentication/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/authentication/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/authentication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.317271 funding-service-design-utils-2.0.7/fsd_utils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/config/commonconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/config/configclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/config/notify_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.317271 funding-service-design-utils-2.0.7/fsd_utils/gunicorn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/gunicorn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.317271 funding-service-design-utils-2.0.7/fsd_utils/gunicorn/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/gunicorn/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/gunicorn/config/devtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/gunicorn/config/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.317271 funding-service-design-utils-2.0.7/fsd_utils/healthchecks/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/healthchecks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/healthchecks/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/healthchecks/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.317271 funding-service-design-utils-2.0.7/fsd_utils/locale_selector/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/locale_selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/locale_selector/get_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/locale_selector/set_lang.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.321271 funding-service-design-utils-2.0.7/fsd_utils/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.321271 funding-service-design-utils-2.0.7/fsd_utils/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/mapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.321271 funding-service-design-utils-2.0.7/fsd_utils/mapping/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/mapping/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/mapping/application/application_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/mapping/application/free_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/mapping/application/multi_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/mapping/application/qa_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.321271 funding-service-design-utils-2.0.7/fsd_utils/sentry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/sentry/init_sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.321271 funding-service-design-utils-2.0.7/fsd_utils/simple_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/simple_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/simple_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/simple_utils/date_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.321271 funding-service-design-utils-2.0.7/fsd_utils/toggles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/toggles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/fsd_utils/toggles/toggles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.321271 funding-service-design-utils-2.0.7/funding_service_design_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-06-28 13:41:33.000000 funding-service-design-utils-2.0.7/funding_service_design_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-28 13:41:33.000000 funding-service-design-utils-2.0.7/funding_service_design_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 13:41:33.000000 funding-service-design-utils-2.0.7/funding_service_design_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-28 13:41:33.000000 funding-service-design-utils-2.0.7/funding_service_design_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-28 13:41:33.000000 funding-service-design-utils-2.0.7/funding_service_design_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 13:41:33.321271 funding-service-design-utils-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:33.321271 funding-service-design-utils-2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/tests/test_get_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/tests/test_mapping_application.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-28 13:41:18.000000 funding-service-design-utils-2.0.7/tests/test_set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.457517 funding-service-design-utils-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-06-30 10:27:47.457517 funding-service-design-utils-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_test_utils/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_test_utils/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_test_utils/fixtures/db_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_test_utils/test_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_test_utils/test_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_test_utils/test_config/useful_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_utils/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/authentication/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/authentication/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/authentication/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/authentication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_utils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/config/commonconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/config/configclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/config/notify_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_utils/gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/gunicorn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_utils/gunicorn/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/gunicorn/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/gunicorn/config/devtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/gunicorn/config/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_utils/healthchecks/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/healthchecks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/healthchecks/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/healthchecks/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.453517 funding-service-design-utils-2.0.8/fsd_utils/locale_selector/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/locale_selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/locale_selector/get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/locale_selector/set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.453517 funding-service-design-utils-2.0.8/fsd_utils/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.453517 funding-service-design-utils-2.0.8/fsd_utils/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/mapping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.453517 funding-service-design-utils-2.0.8/fsd_utils/mapping/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/mapping/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/mapping/application/application_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/mapping/application/free_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/mapping/application/multi_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/mapping/application/qa_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.453517 funding-service-design-utils-2.0.8/fsd_utils/sentry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/sentry/init_sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.453517 funding-service-design-utils-2.0.8/fsd_utils/simple_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/simple_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/simple_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/simple_utils/date_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.457517 funding-service-design-utils-2.0.8/fsd_utils/toggles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/toggles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/toggles/toggles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.457517 funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-06-30 10:27:47.000000 funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-30 10:27:47.000000 funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:27:47.000000 funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-30 10:27:47.000000 funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-30 10:27:47.000000 funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 10:27:47.457517 funding-service-design-utils-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.457517 funding-service-design-utils-2.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_mapping_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_set_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_utils.py
```

### Comparing `funding-service-design-utils-2.0.7/LICENSE` & `funding-service-design-utils-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/PKG-INFO` & `funding-service-design-utils-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 2.0.7
+Version: 2.0.8
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `funding-service-design-utils-2.0.7/README.md` & `funding-service-design-utils-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_test_utils/fixtures/db_fixtures.py` & `funding-service-design-utils-2.0.8/fsd_test_utils/fixtures/db_fixtures.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/__init__.py` & `funding-service-design-utils-2.0.8/fsd_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/authentication/decorators.py` & `funding-service-design-utils-2.0.8/fsd_utils/authentication/decorators.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/authentication/models.py` & `funding-service-design-utils-2.0.8/fsd_utils/authentication/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Data models for authentication
 """
 from dataclasses import dataclass
 from os import getenv
 from typing import List
+from typing import Mapping
 
 from sentry_sdk import set_user
 
-from .utils import get_highest_role
+from .utils import get_highest_role_map
 
 
 @dataclass
 class User:
     full_name: str
     email: str
     roles: List[str]
-    highest_role: str
+    highest_role_map: Mapping[str, str]
 
     @classmethod
     def set_with_token(cls, token_payload):
         full_name = token_payload.get("fullName")
         email = token_payload.get("email")
         roles = token_payload.get("roles")
         # Set user in Sentry
@@ -31,9 +32,9 @@
                     "username": token_payload.get("fullName"),
                 }
             )
         return cls(
             full_name=full_name,
             email=email,
             roles=roles,
-            highest_role=get_highest_role(roles),
+            highest_role_map=get_highest_role_map(roles),
         )
```

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/config/commonconfig.py` & `funding-service-design-utils-2.0.8/fsd_utils/config/commonconfig.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/config/configclass.py` & `funding-service-design-utils-2.0.8/fsd_utils/config/configclass.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/config/notify_constants.py` & `funding-service-design-utils-2.0.8/fsd_utils/config/notify_constants.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/gunicorn/config/devtest.py` & `funding-service-design-utils-2.0.8/fsd_utils/gunicorn/config/devtest.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/gunicorn/config/local.py` & `funding-service-design-utils-2.0.8/fsd_utils/gunicorn/config/local.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/healthchecks/checkers.py` & `funding-service-design-utils-2.0.8/fsd_utils/healthchecks/checkers.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/healthchecks/healthcheck.py` & `funding-service-design-utils-2.0.8/fsd_utils/healthchecks/healthcheck.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/locale_selector/get_lang.py` & `funding-service-design-utils-2.0.8/fsd_utils/locale_selector/get_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/locale_selector/set_lang.py` & `funding-service-design-utils-2.0.8/fsd_utils/locale_selector/set_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/logging/logging.py` & `funding-service-design-utils-2.0.8/fsd_utils/logging/logging.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/mapping/application/application_utils.py` & `funding-service-design-utils-2.0.8/fsd_utils/mapping/application/application_utils.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/mapping/application/free_text.py` & `funding-service-design-utils-2.0.8/fsd_utils/mapping/application/free_text.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/mapping/application/multi_input.py` & `funding-service-design-utils-2.0.8/fsd_utils/mapping/application/multi_input.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/mapping/application/qa_mapping.py` & `funding-service-design-utils-2.0.8/fsd_utils/mapping/application/qa_mapping.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/sentry/init_sentry.py` & `funding-service-design-utils-2.0.8/fsd_utils/sentry/init_sentry.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/simple_utils/date_utils.py` & `funding-service-design-utils-2.0.8/fsd_utils/simple_utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/fsd_utils/toggles/toggles.py` & `funding-service-design-utils-2.0.8/fsd_utils/toggles/toggles.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/funding_service_design_utils.egg-info/PKG-INFO` & `funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 2.0.7
+Version: 2.0.8
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `funding-service-design-utils-2.0.7/funding_service_design_utils.egg-info/SOURCES.txt` & `funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,8 +51,9 @@
 tests/conftest.py
 tests/test_authentication.py
 tests/test_checkers.py
 tests/test_data_utils.py
 tests/test_get_lang.py
 tests/test_healthcheck.py
 tests/test_mapping_application.py
-tests/test_set_lang.py
+tests/test_set_lang.py
+tests/test_utils.py
```

### Comparing `funding-service-design-utils-2.0.7/pyproject.toml` & `funding-service-design-utils-2.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "funding-service-design-utils"
-version = "2.0.7"
+version = "2.0.8"
 authors = [
   { name="DLUHC", email="FundingServiceDesignTeam@levellingup.gov.uk" },
 ]
 description = "Utilities used by the DLUHC Funding Service Design Team"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10,<4.0"
```

### Comparing `funding-service-design-utils-2.0.7/tests/conftest.py` & `funding-service-design-utils-2.0.8/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,16 +94,16 @@
                 "COOKIE_DOMAIN": None,
                 "FLASK_ENV": "development",
                 "DEBUG_USER_ON": True,
                 "DEBUG_USER_ROLE": "ADMIN",
                 "DEBUG_USER": {
                     "full_name": "Development User",
                     "email": "dev@example.com",
-                    "roles": ["ADMIN", "TEST"],
-                    "highest_role": "ADMIN",
+                    "roles": ["COF_ADMIN", "COF_TEST"],
+                    "highest_role_map": {"COF": "ADMIN"},
                 },
                 "FSD_USER_TOKEN_COOKIE_NAME": "fsd-user-token",
                 "AUTHENTICATOR_HOST": "https://authenticator",
                 "RSA256_PUBLIC_KEY": rsa256_public_key,
             }
         )
         app_context.app.add_url_rule(
@@ -130,16 +130,16 @@
     g: {
         "is_authenticated": True,
         "logout_url": "https://authenticator/sessions/sign-out",
         "account_id": "test-user",
         "user": User(
             email="test@example.com",
             full_name="Test User",
-            highest_role="LEAD_ASSESSOR",
-            roles=["LEAD_ASSESSOR", "ASSESSOR", "COMMENTER"]
+            highest_role_map={"COF": "LEAD_ASSESSOR"},
+            roles=["COF_LEAD_ASSESSOR", "COF_ASSESSOR", "COF_COMMENTER"]
         )
     :return: the Flask g variable serialised as a dict/json
     """
     return vars(g)
 
 
 @login_requested
@@ -151,30 +151,30 @@
     g: {
         "is_authenticated": True,
         "logout_url": "https://authenticator/sessions/sign-out",
         "account_id": "test-user",
         "user": User(
             email="test@example.com",
             full_name="Test User",
-            highest_role="LEAD_ASSESSOR",
-            roles=["LEAD_ASSESSOR", "ASSESSOR", "COMMENTER"]
+            highest_role_map={"COF": "LEAD_ASSESSOR"},
+            roles=["COF_LEAD_ASSESSOR", "COF_ASSESSOR", "COF_COMMENTER"]
         )
     and a non logged in user to have the Flask request g variables
     set as below:
     g: {
         "is_authenticated": False,
         "logout_url": "https://authenticator/sessions/sign-out",
         "account_id": None,
     }
     :return: the Flask g variable serialised as a dict/json
     """
     return vars(g)
 
 
-@login_required(roles_required=["COMMENTER"])
+@login_required(roles_required=["COF_COMMENTER"])
 def mock_login_required_roles_route():
     """
     A mock route function decorated with
     @login_required(roles_required=["COMMENTER"])
     Here we expect a logged in user without the "COMMENTER"
     role to be redirected to a missing roles required
     error page on authenticator,
@@ -184,23 +184,23 @@
     g: {
         "is_authenticated": True,
         "logout_url": "https://authenticator/sessions/sign-out",
         "account_id": "test-user",
         "user": User(
             email="test@example.com",
             full_name="Test User",
-            highest_role="LEAD_ASSESSOR",
-            roles=["LEAD_ASSESSOR", "ASSESSOR", "COMMENTER"]
+            highest_role_map={"COF": "LEAD_ASSESSOR"},
+            roles=["COF_LEAD_ASSESSOR", "COF_ASSESSOR", "COF_COMMENTER"]
         )
     :return: the Flask g variable serialised as a dict/json
     """
     return vars(g)
 
 
-@login_required(roles_required=["ADMIN", "TEST"])
+@login_required(roles_required=["COF_ADMIN", "COF_TEST"])
 def mock_login_required_admin_roles_route():
     """
     A mock route function decorated with
     @login_required(roles_required=["ADMIN","TEST"])
     Here we expect a logged in user without the "ADMIN","TEST"
     role to be redirected to a missing roles required
     error page on authenticator,
@@ -210,16 +210,16 @@
     g: {
         "is_authenticated": True,
         "logout_url": "https://authenticator/sessions/sign-out",
         "account_id": "test-user",
         "user": User(
             email="test@example.com",
             full_name="Test User",
-            highest_role="LEAD_ASSESSOR",
-            roles=["LEAD_ASSESSOR", "ASSESSOR", "COMMENTER"]
+            highest_role_map={"COF": "LEAD_ASSESSOR"},
+            roles=["COF_LEAD_ASSESSOR", "COF_ASSESSOR", "COF_COMMENTER"]
         )
     :return: the Flask g variable serialised as a dict/json
     """
     return vars(g)
 
 
 @login_required(return_app=SupportedApp.POST_AWARD_FRONTEND)
@@ -232,16 +232,16 @@
     g: {
         "is_authenticated": True,
         "logout_url": "https://authenticator/sessions/sign-out?return_app=post-award-frontend",
         "account_id": "test-user",
         "user": User(
             email="test@example.com",
             full_name="Test User",
-            highest_role="LEAD_ASSESSOR",
-            roles=["LEAD_ASSESSOR", "ASSESSOR", "COMMENTER"]
+            highest_role_map={"COF": "LEAD_ASSESSOR"},
+            roles=["COF_LEAD_ASSESSOR", "COF_ASSESSOR", "COF_COMMENTER"]
         )
     and a non logged in user to have the Flask request g variables
     set as below:
     g: {
         "is_authenticated": False,
         "logout_url": "https://authenticator/sessions/sign-out?return_app=post-award-frontend",
         "account_id": None,
```

### Comparing `funding-service-design-utils-2.0.7/tests/test_authentication.py` & `funding-service-design-utils-2.0.8/tests/test_authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 class TestAuthentication:
 
     test_payload = {
         "accountId": "test-user",
         "email": "test@example.com",
         "fullName": "Test User",
-        "roles": ["LEAD_ASSESSOR", "ASSESSOR", "COMMENTER"],
+        "roles": ["COF_LEAD_ASSESSOR", "COF_ASSESSOR", "COF_COMMENTER"],
     }
     expected_valid_g_attributes = {
         "is_authenticated": True,
         "logout_url": "https://authenticator/sessions/sign-out",
         "account_id": "test-user",
         "user": {
             "email": "test@example.com",
             "full_name": "Test User",
-            "highest_role": "LEAD_ASSESSOR",
-            "roles": ["LEAD_ASSESSOR", "ASSESSOR", "COMMENTER"],
+            "highest_role_map": {"COF": "LEAD_ASSESSOR"},
+            "roles": ["COF_LEAD_ASSESSOR", "COF_ASSESSOR", "COF_COMMENTER"],
         },
     }
 
     expected_unauthenticated_g_attributes = {
         "is_authenticated": False,
         "logout_url": "https://authenticator/sessions/sign-out",
         "account_id": None,
@@ -111,15 +111,15 @@
         """
         valid_token = self._create_valid_token()
         flask_test_client.set_cookie("localhost", "fsd-user-token", valid_token)
         mock_request = flask_test_client.get("/mock_login_required_admin_roles_route")
         assert mock_request.status_code == 302
         assert (
             mock_request.location
-            == "https://authenticator/service/user?roles_required=ADMIN|TEST"
+            == "https://authenticator/service/user?roles_required=COF_ADMIN|COF_TEST"
         )
 
     def test_login_required_roles_sets_user_attributes_if_user_has_roles(
         self, flask_test_client
     ):
         """
         GIVEN a flask_test_client and route decorated with
@@ -201,15 +201,15 @@
         flask_test_development_client.set_cookie("localhost", "fsd-user-token", "")
         mock_request = flask_test_development_client.get(
             "/mock_login_required_roles_route"
         )
         assert mock_request.status_code == 302
         assert (
             mock_request.location
-            == "https://authenticator/service/user?roles_required=COMMENTER"
+            == "https://authenticator/service/user?roles_required=COF_COMMENTER"
         )
 
     def test_login_required_with_return_app_redirects_to_signed_out_without_token(
         self, flask_test_client
     ):
         """
         GIVEN a flask_test_client and
```

### Comparing `funding-service-design-utils-2.0.7/tests/test_checkers.py` & `funding-service-design-utils-2.0.8/tests/test_checkers.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/tests/test_data_utils.py` & `funding-service-design-utils-2.0.8/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/tests/test_get_lang.py` & `funding-service-design-utils-2.0.8/tests/test_get_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/tests/test_healthcheck.py` & `funding-service-design-utils-2.0.8/tests/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/tests/test_mapping_application.py` & `funding-service-design-utils-2.0.8/tests/test_mapping_application.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.7/tests/test_set_lang.py` & `funding-service-design-utils-2.0.8/tests/test_set_lang.py`

 * *Files identical despite different names*

