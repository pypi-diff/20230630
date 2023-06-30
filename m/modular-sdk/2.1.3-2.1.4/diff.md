# Comparing `tmp/modular_sdk-2.1.3.tar.gz` & `tmp/modular_sdk-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/onsha/Develop/EPAM/temp-modular-sdk/dist/.tmp-1zf3cw2s/modular_sdk-2.1.3.tar", last modified: Thu Jun 29 14:46:43 2023, max compression
+gzip compressed data, was "/Users/onsha/Develop/EPAM/temp-modular-sdk/dist/.tmp-lau1mgvn/modular_sdk-2.1.4.tar", last modified: Fri Jun 30 09:15:25 2023, max compression
```

## Comparing `modular_sdk-2.1.3.tar` & `modular_sdk-2.1.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.896141 modular_sdk-2.1.3/
--rw-r--r--   0 onsha      (501) staff       (20)    11357 2023-06-29 14:09:33.000000 modular_sdk-2.1.3/LICENSE
--rw-r--r--   0 onsha      (501) staff       (20)      361 2023-06-29 14:46:43.896252 modular_sdk-2.1.3/PKG-INFO
--rw-r--r--   0 onsha      (501) staff       (20)     3507 2023-06-28 12:04:17.000000 modular_sdk-2.1.3/README.md
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.853529 modular_sdk-2.1.3/modular_sdk/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/__init__.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.861920 modular_sdk-2.1.3/modular_sdk/commons/
--rw-r--r--   0 onsha      (501) staff       (20)     4869 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/commons/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     4865 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/commons/constants.py
--rw-r--r--   0 onsha      (501) staff       (20)     2045 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/commons/error_helper.py
--rw-r--r--   0 onsha      (501) staff       (20)      200 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/commons/exception.py
--rw-r--r--   0 onsha      (501) staff       (20)      800 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/commons/helpers.py
--rw-r--r--   0 onsha      (501) staff       (20)     2642 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/commons/log_helper.py
--rw-r--r--   0 onsha      (501) staff       (20)      951 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/commons/time_helper.py
--rw-r--r--   0 onsha      (501) staff       (20)     2458 2023-06-21 10:06:07.000000 modular_sdk-2.1.3/modular_sdk/commons/trace_helper.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.863563 modular_sdk-2.1.3/modular_sdk/connections/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/connections/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     1754 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/connections/mongodb_connection.py
--rw-r--r--   0 onsha      (501) staff       (20)     4723 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/connections/rabbit_connection.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.864633 modular_sdk-2.1.3/modular_sdk/helpers/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/helpers/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)      985 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/helpers/response_helper.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.872593 modular_sdk-2.1.3/modular_sdk/models/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     1579 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/application.py
--rw-r--r--   0 onsha      (501) staff       (20)      929 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/base_meta.py
--rw-r--r--   0 onsha      (501) staff       (20)      689 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/customer.py
--rw-r--r--   0 onsha      (501) staff       (20)     1050 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/execution_trace.py
--rw-r--r--   0 onsha      (501) staff       (20)      490 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/heartbeat.py
--rw-r--r--   0 onsha      (501) staff       (20)      712 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/job.py
--rw-r--r--   0 onsha      (501) staff       (20)      662 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/operation_mode.py
--rw-r--r--   0 onsha      (501) staff       (20)     1570 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/parent.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.877418 modular_sdk-2.1.3/modular_sdk/models/pynamodb_extension/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/pynamodb_extension/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)    22311 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/pynamodb_extension/base_model.py
--rw-r--r--   0 onsha      (501) staff       (20)     2261 2023-06-21 10:06:07.000000 modular_sdk-2.1.3/modular_sdk/models/pynamodb_extension/base_role_access_model.py
--rw-r--r--   0 onsha      (501) staff       (20)     7045 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/pynamodb_extension/base_safe_update_model.py
--rw-r--r--   0 onsha      (501) staff       (20)    16520 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py
--rw-r--r--   0 onsha      (501) staff       (20)      811 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py
--rw-r--r--   0 onsha      (501) staff       (20)     2565 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/region.py
--rw-r--r--   0 onsha      (501) staff       (20)      476 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/setting.py
--rw-r--r--   0 onsha      (501) staff       (20)     4048 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/tenant.py
--rw-r--r--   0 onsha      (501) staff       (20)     1081 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/models/tenant_settings.py
--rw-r--r--   0 onsha      (501) staff       (20)    10963 2023-06-21 10:06:07.000000 modular_sdk-2.1.3/modular_sdk/modular.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.886620 modular_sdk-2.1.3/modular_sdk/services/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     4860 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/application_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     4559 2023-06-21 10:06:07.000000 modular_sdk-2.1.3/modular_sdk/services/aws_creds_provider.py
--rw-r--r--   0 onsha      (501) staff       (20)      803 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/customer_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     5073 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/environment_service.py
--rw-r--r--   0 onsha      (501) staff       (20)      618 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/events_service.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.888687 modular_sdk-2.1.3/modular_sdk/services/impl/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/impl/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)    25123 2023-06-28 12:04:17.000000 modular_sdk-2.1.3/modular_sdk/services/impl/maestro_credentials_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     9096 2023-06-21 10:18:14.000000 modular_sdk-2.1.3/modular_sdk/services/impl/maestro_rabbit_transport_service.py
--rw-r--r--   0 onsha      (501) staff       (20)      620 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/lambda_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     5862 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/parent_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     3751 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/rabbit_transport_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     2602 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/region_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     9806 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/settings_management_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     1488 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/sqs_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     7305 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/ssm_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     8390 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/sts_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     7165 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/tenant_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     2143 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/services/tenant_settings_service.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.889315 modular_sdk-2.1.3/modular_sdk/utils/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/utils/__init__.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.890378 modular_sdk-2.1.3/modular_sdk/utils/job_tracer/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/utils/job_tracer/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)      354 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/utils/job_tracer/abstract.py
--rw-r--r--   0 onsha      (501) staff       (20)     3832 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/utils/job_tracer/generic.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.891602 modular_sdk-2.1.3/modular_sdk/utils/operation_mode/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/utils/operation_mode/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)      776 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/utils/operation_mode/abstract.py
--rw-r--r--   0 onsha      (501) staff       (20)     2171 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/utils/operation_mode/generic.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.892888 modular_sdk-2.1.3/modular_sdk/utils/runtime_tracer/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/utils/runtime_tracer/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     1061 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/utils/runtime_tracer/abstract.py
--rw-r--r--   0 onsha      (501) staff       (20)     4091 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/modular_sdk/utils/runtime_tracer/generic.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.856254 modular_sdk-2.1.3/modular_sdk.egg-info/
--rw-r--r--   0 onsha      (501) staff       (20)      361 2023-06-29 14:46:43.000000 modular_sdk-2.1.3/modular_sdk.egg-info/PKG-INFO
--rw-r--r--   0 onsha      (501) staff       (20)     2945 2023-06-29 14:46:43.000000 modular_sdk-2.1.3/modular_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 onsha      (501) staff       (20)        1 2023-06-29 14:46:43.000000 modular_sdk-2.1.3/modular_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 onsha      (501) staff       (20)      271 2023-06-29 14:46:43.000000 modular_sdk-2.1.3/modular_sdk.egg-info/requires.txt
--rw-r--r--   0 onsha      (501) staff       (20)       18 2023-06-29 14:46:43.000000 modular_sdk-2.1.3/modular_sdk.egg-info/top_level.txt
--rw-r--r--   0 onsha      (501) staff       (20)       86 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/pyproject.toml
--rw-r--r--   0 onsha      (501) staff       (20)      759 2023-06-29 14:46:43.896898 modular_sdk-2.1.3/setup.cfg
--rw-r--r--   0 onsha      (501) staff       (20)       38 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/setup.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.893452 modular_sdk-2.1.3/tests/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/tests/__init__.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.894727 modular_sdk-2.1.3/tests/test_commons/
--rw-r--r--   0 onsha      (501) staff       (20)      119 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/tests/test_commons/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     1852 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/tests/test_commons/import_helper.py
--rw-r--r--   0 onsha      (501) staff       (20)     2846 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/tests/test_commons/utils.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-29 14:46:43.895529 modular_sdk-2.1.3/tests/test_models/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/tests/test_models/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)    11617 2023-06-21 08:08:16.000000 modular_sdk-2.1.3/tests/test_models/test_base_safe_update_model.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.042288 modular_sdk-2.1.4/
+-rw-r--r--   0 onsha      (501) staff       (20)    11357 2023-06-29 14:09:33.000000 modular_sdk-2.1.4/LICENSE
+-rw-r--r--   0 onsha      (501) staff       (20)     4014 2023-06-30 09:15:25.042433 modular_sdk-2.1.4/PKG-INFO
+-rw-r--r--   0 onsha      (501) staff       (20)     3507 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/README.md
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.000300 modular_sdk-2.1.4/modular_sdk/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/__init__.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.006476 modular_sdk-2.1.4/modular_sdk/commons/
+-rw-r--r--   0 onsha      (501) staff       (20)     4869 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4865 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/constants.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2045 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/error_helper.py
+-rw-r--r--   0 onsha      (501) staff       (20)      200 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/exception.py
+-rw-r--r--   0 onsha      (501) staff       (20)      800 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/helpers.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2642 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/log_helper.py
+-rw-r--r--   0 onsha      (501) staff       (20)      951 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/time_helper.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2458 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/trace_helper.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.007818 modular_sdk-2.1.4/modular_sdk/connections/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/connections/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1754 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/connections/mongodb_connection.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4723 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/connections/rabbit_connection.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.008967 modular_sdk-2.1.4/modular_sdk/helpers/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/helpers/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)      985 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/helpers/response_helper.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.017760 modular_sdk-2.1.4/modular_sdk/models/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1579 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/application.py
+-rw-r--r--   0 onsha      (501) staff       (20)      929 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/base_meta.py
+-rw-r--r--   0 onsha      (501) staff       (20)      689 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/customer.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1050 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/execution_trace.py
+-rw-r--r--   0 onsha      (501) staff       (20)      490 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/heartbeat.py
+-rw-r--r--   0 onsha      (501) staff       (20)      712 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/job.py
+-rw-r--r--   0 onsha      (501) staff       (20)      662 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/operation_mode.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1570 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/parent.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.022548 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)    22311 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/base_model.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2261 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/base_role_access_model.py
+-rw-r--r--   0 onsha      (501) staff       (20)     7045 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/base_safe_update_model.py
+-rw-r--r--   0 onsha      (501) staff       (20)    16520 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py
+-rw-r--r--   0 onsha      (501) staff       (20)      811 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2565 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/region.py
+-rw-r--r--   0 onsha      (501) staff       (20)      476 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/setting.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4048 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/tenant.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1081 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/tenant_settings.py
+-rw-r--r--   0 onsha      (501) staff       (20)    10963 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/modular.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.033396 modular_sdk-2.1.4/modular_sdk/services/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4860 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/application_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4559 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/aws_creds_provider.py
+-rw-r--r--   0 onsha      (501) staff       (20)      803 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/customer_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     5073 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/environment_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)      618 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/events_service.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.035000 modular_sdk-2.1.4/modular_sdk/services/impl/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/impl/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)    25123 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/impl/maestro_credentials_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     9096 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/impl/maestro_rabbit_transport_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)      620 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/lambda_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     5862 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/parent_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     3751 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/rabbit_transport_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2602 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/region_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     9806 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/settings_management_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1488 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/sqs_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     7305 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/ssm_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     8390 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/sts_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     7165 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/tenant_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2143 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/tenant_settings_service.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.035638 modular_sdk-2.1.4/modular_sdk/utils/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/__init__.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.036775 modular_sdk-2.1.4/modular_sdk/utils/job_tracer/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/job_tracer/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)      354 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/job_tracer/abstract.py
+-rw-r--r--   0 onsha      (501) staff       (20)     3832 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/job_tracer/generic.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.038279 modular_sdk-2.1.4/modular_sdk/utils/operation_mode/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/operation_mode/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)      776 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/operation_mode/abstract.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2171 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/operation_mode/generic.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.039420 modular_sdk-2.1.4/modular_sdk/utils/runtime_tracer/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/runtime_tracer/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1061 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/runtime_tracer/abstract.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4091 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/runtime_tracer/generic.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.002252 modular_sdk-2.1.4/modular_sdk.egg-info/
+-rw-r--r--   0 onsha      (501) staff       (20)     4014 2023-06-30 09:15:24.000000 modular_sdk-2.1.4/modular_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 onsha      (501) staff       (20)     2945 2023-06-30 09:15:24.000000 modular_sdk-2.1.4/modular_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 onsha      (501) staff       (20)        1 2023-06-30 09:15:24.000000 modular_sdk-2.1.4/modular_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 onsha      (501) staff       (20)      271 2023-06-30 09:15:24.000000 modular_sdk-2.1.4/modular_sdk.egg-info/requires.txt
+-rw-r--r--   0 onsha      (501) staff       (20)       18 2023-06-30 09:15:24.000000 modular_sdk-2.1.4/modular_sdk.egg-info/top_level.txt
+-rw-r--r--   0 onsha      (501) staff       (20)       86 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/pyproject.toml
+-rw-r--r--   0 onsha      (501) staff       (20)      923 2023-06-30 09:15:25.043102 modular_sdk-2.1.4/setup.cfg
+-rw-r--r--   0 onsha      (501) staff       (20)       38 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/setup.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.039976 modular_sdk-2.1.4/tests/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/tests/__init__.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.041232 modular_sdk-2.1.4/tests/test_commons/
+-rw-r--r--   0 onsha      (501) staff       (20)      119 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/tests/test_commons/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1852 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/tests/test_commons/import_helper.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2846 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/tests/test_commons/utils.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.041911 modular_sdk-2.1.4/tests/test_models/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/tests/test_models/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)    11617 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/tests/test_models/test_base_safe_update_model.py
```

### Comparing `modular_sdk-2.1.3/LICENSE` & `modular_sdk-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/README.md` & `modular_sdk-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/commons/__init__.py` & `modular_sdk-2.1.4/modular_sdk/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/commons/constants.py` & `modular_sdk-2.1.4/modular_sdk/commons/constants.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/commons/error_helper.py` & `modular_sdk-2.1.4/modular_sdk/commons/error_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/commons/helpers.py` & `modular_sdk-2.1.4/modular_sdk/commons/helpers.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/commons/log_helper.py` & `modular_sdk-2.1.4/modular_sdk/commons/log_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/commons/time_helper.py` & `modular_sdk-2.1.4/modular_sdk/commons/time_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/commons/trace_helper.py` & `modular_sdk-2.1.4/modular_sdk/commons/trace_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/connections/mongodb_connection.py` & `modular_sdk-2.1.4/modular_sdk/connections/mongodb_connection.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/connections/rabbit_connection.py` & `modular_sdk-2.1.4/modular_sdk/connections/rabbit_connection.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/helpers/response_helper.py` & `modular_sdk-2.1.4/modular_sdk/helpers/response_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/application.py` & `modular_sdk-2.1.4/modular_sdk/models/application.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/base_meta.py` & `modular_sdk-2.1.4/modular_sdk/models/base_meta.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/customer.py` & `modular_sdk-2.1.4/modular_sdk/models/customer.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/execution_trace.py` & `modular_sdk-2.1.4/modular_sdk/models/execution_trace.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/job.py` & `modular_sdk-2.1.4/modular_sdk/models/job.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/operation_mode.py` & `modular_sdk-2.1.4/modular_sdk/models/operation_mode.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/parent.py` & `modular_sdk-2.1.4/modular_sdk/models/parent.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/pynamodb_extension/base_model.py` & `modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/base_model.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/pynamodb_extension/base_role_access_model.py` & `modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/base_role_access_model.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/pynamodb_extension/base_safe_update_model.py` & `modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/base_safe_update_model.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py` & `modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py` & `modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/region.py` & `modular_sdk-2.1.4/modular_sdk/models/region.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/tenant.py` & `modular_sdk-2.1.4/modular_sdk/models/tenant.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/models/tenant_settings.py` & `modular_sdk-2.1.4/modular_sdk/models/tenant_settings.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/modular.py` & `modular_sdk-2.1.4/modular_sdk/modular.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/application_service.py` & `modular_sdk-2.1.4/modular_sdk/services/application_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/aws_creds_provider.py` & `modular_sdk-2.1.4/modular_sdk/services/aws_creds_provider.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/customer_service.py` & `modular_sdk-2.1.4/modular_sdk/services/customer_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/environment_service.py` & `modular_sdk-2.1.4/modular_sdk/services/environment_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/events_service.py` & `modular_sdk-2.1.4/modular_sdk/services/events_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/impl/maestro_credentials_service.py` & `modular_sdk-2.1.4/modular_sdk/services/impl/maestro_credentials_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/impl/maestro_rabbit_transport_service.py` & `modular_sdk-2.1.4/modular_sdk/services/impl/maestro_rabbit_transport_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/lambda_service.py` & `modular_sdk-2.1.4/modular_sdk/services/lambda_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/parent_service.py` & `modular_sdk-2.1.4/modular_sdk/services/parent_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/rabbit_transport_service.py` & `modular_sdk-2.1.4/modular_sdk/services/rabbit_transport_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/region_service.py` & `modular_sdk-2.1.4/modular_sdk/services/region_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/settings_management_service.py` & `modular_sdk-2.1.4/modular_sdk/services/settings_management_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/sqs_service.py` & `modular_sdk-2.1.4/modular_sdk/services/sqs_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/ssm_service.py` & `modular_sdk-2.1.4/modular_sdk/services/ssm_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/sts_service.py` & `modular_sdk-2.1.4/modular_sdk/services/sts_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/tenant_service.py` & `modular_sdk-2.1.4/modular_sdk/services/tenant_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/services/tenant_settings_service.py` & `modular_sdk-2.1.4/modular_sdk/services/tenant_settings_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/utils/job_tracer/generic.py` & `modular_sdk-2.1.4/modular_sdk/utils/job_tracer/generic.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/utils/operation_mode/abstract.py` & `modular_sdk-2.1.4/modular_sdk/utils/operation_mode/abstract.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/utils/operation_mode/generic.py` & `modular_sdk-2.1.4/modular_sdk/utils/operation_mode/generic.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/utils/runtime_tracer/abstract.py` & `modular_sdk-2.1.4/modular_sdk/utils/runtime_tracer/abstract.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk/utils/runtime_tracer/generic.py` & `modular_sdk-2.1.4/modular_sdk/utils/runtime_tracer/generic.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/modular_sdk.egg-info/SOURCES.txt` & `modular_sdk-2.1.4/modular_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/tests/test_commons/import_helper.py` & `modular_sdk-2.1.4/tests/test_commons/import_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/tests/test_commons/utils.py` & `modular_sdk-2.1.4/tests/test_commons/utils.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.3/tests/test_models/test_base_safe_update_model.py` & `modular_sdk-2.1.4/tests/test_models/test_base_safe_update_model.py`

 * *Files identical despite different names*

