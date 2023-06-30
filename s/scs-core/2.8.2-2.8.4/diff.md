# Comparing `tmp/scs-core-2.8.2.tar.gz` & `tmp/scs-core-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-core-2.8.2.tar", last modified: Mon Jun 26 13:24:09 2023, max compression
+gzip compressed data, was "scs-core-2.8.4.tar", last modified: Fri Jun 30 08:18:12 2023, max compression
```

## Comparing `scs-core-2.8.2.tar` & `scs-core-2.8.4.tar`

### file list

```diff
@@ -1,419 +1,419 @@
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.770826 scs-core-2.8.2/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:27.000000 scs-core-2.8.2/LICENSE
--rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:27.000000 scs-core-2.8.2/MANIFEST.in
--rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-06-26 13:24:09.770826 scs-core-2.8.2/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)     1404 2023-06-26 09:33:48.000000 scs-core-2.8.2/README.md
--rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:27.000000 scs-core-2.8.2/README.rst
--rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-02-06 14:01:57.000000 scs-core-2.8.2/requirements.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-26 13:24:09.770826 scs-core-2.8.2/setup.cfg
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1996 2022-08-17 09:53:27.000000 scs-core-2.8.2/setup.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.738826 scs-core-2.8.2/src/
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/
--rw-rw-r--   0 jade      (1002) jade      (1002)      183 2023-06-26 13:23:15.000000 scs-core-2.8.2/src/scs_core/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/aqcsv/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/aqcsv/conf/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/conf/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2617 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/conf/airnow_site_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1034 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/conf/airnow_uploader_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/aqcsv/connector/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/connector/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10203 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/aqcsv/connector/airnow_mapping_task.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6655 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/connector/datum_mapping.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5042 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/connector/source_mapping.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/aqcsv/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3750 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/data/aqcsv_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    13723 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/data/aqcsv_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3033 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/data/aqcsv_site.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/aqcsv/specification/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2824 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/agency.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2728 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/country.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1163 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/country_iso.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1175 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/country_numeric.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9800 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/method.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3765 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/mpc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3453 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/parameter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2855 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/qc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3732 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/qualifier.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2879 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/unit.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/aws/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.746826 scs-core-2.8.2/src/scs_core/aws/client/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/client/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3585 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/client/access_key.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2332 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/client/api_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2113 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/client/api_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1217 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/client/client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5103 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/client/client_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1281 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/client/device_control_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3294 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/client/email_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3361 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/client/monitor_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5891 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/aws/client/mqtt_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3856 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/client/rest_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.746826 scs-core-2.8.2/src/scs_core/aws/config/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/config/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      744 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/config/aws.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4471 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/aws/config/project.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.746826 scs-core-2.8.2/src/scs_core/aws/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    16736 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/data/alert.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9320 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/data/byline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1792 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/byline_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4640 2023-04-17 09:22:53.000000 scs-core-2.8.2/src/scs_core/aws/data/dataset.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3550 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/deployment.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3337 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/data/device_monitor_email_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    12653 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/data/device_monitor_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3313 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/data/device_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4032 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/aws/data/email_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2859 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/data/http_response.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/message.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1776 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/power_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1820 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/runtime_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1795 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/status_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2884 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/upload_interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1793 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/uptime_list.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.746826 scs-core-2.8.2/src/scs_core/aws/greengrass/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1998 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/aws_deployer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3017 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/aws_deployment_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9610 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/aws_group.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    16440 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/aws_group_configuration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11557 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/aws_identity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      440 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/gg_errors.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.750826 scs-core-2.8.2/src/scs_core/aws/manager/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/manager/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8285 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/alert_specification_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/alert_status_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3950 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/byline_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/configuration_check_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3256 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/configuration_check_requester.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10816 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/configuration_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2248 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/device_monitor_specification_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1497 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/device_monitor_status_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10307 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/dynamo_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3551 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/manager/ec2_message_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6470 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/lambda_bylines.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    15996 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/aws/manager/lambda_message_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    18045 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/aws/manager/s3_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4295 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/manager/sagemaker_model_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7802 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/manager/sagemaker_trial_manager.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.750826 scs-core-2.8.2/src/scs_core/aws/security/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/security/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/access_key_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5114 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_client_credentials.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7498 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_device.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1527 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_device_creator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3111 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_device_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1911 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_device_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10555 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_login_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2181 2023-04-17 09:22:53.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_membership.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2314 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_password_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11840 2023-06-26 13:23:15.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_user.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3227 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_user_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3540 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_user_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/device_whitelist_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1947 2023-04-17 09:22:53.000000 scs-core-2.8.2/src/scs_core/aws/security/opr_membership.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    22905 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/organisation.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9601 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/organisation_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1752 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/path_filter.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.750826 scs-core-2.8.2/src/scs_core/client/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/client/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4470 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/client/http_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6933 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/client/http_exception.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      497 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/client/http_status.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2831 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/client/network.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1415 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/client/resource_unavailable_exception.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2638 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/client/sftp_client_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.750826 scs-core-2.8.2/src/scs_core/climate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1407 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/absolute_humidity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1418 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/icp10101_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3081 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/mpl115a2_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2911 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/mpl115a2_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2290 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/pressure_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2188 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/pressure_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3156 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/sht_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1844 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/sht_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.750826 scs-core-2.8.2/src/scs_core/comms/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/comms/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3125 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/comms/mqtt_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2395 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/comms/uds_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1552 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/comms/uds_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2350 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/comms/uds_server.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1614 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/comms/uds_writer.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.750826 scs-core-2.8.2/src/scs_core/control/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/control/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4918 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/control/command.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4896 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/control/control_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3792 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/control/control_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4737 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/control/control_receipt.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.754826 scs-core-2.8.2/src/scs_core/csv/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/csv/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1979 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/csv/csv_archive.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7484 2023-04-17 09:22:53.000000 scs-core-2.8.2/src/scs_core/csv/csv_dict.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5996 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/csv/csv_log.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8594 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/csv/csv_log_cursor_queue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8574 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/csv/csv_log_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8240 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/csv/csv_logger.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3323 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/csv/csv_logger_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5347 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/csv/csv_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4503 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/csv/csv_writer.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.754826 scs-core-2.8.2/src/scs_core/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4802 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/aggregate.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1947 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/data/array_dict.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2415 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/average.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2158 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/categorical_regression.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8964 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/data/checkpoint_generator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1008 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/crc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2092 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/crypt.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    19704 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/data/datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6448 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/data/datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2634 2023-04-17 09:22:53.000000 scs-core-2.8.2/src/scs_core/data/duplicates.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3809 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/data/histogram.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1747 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5951 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/join.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    14204 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/data/json.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3274 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/lin_regress.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5364 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/linear_regression.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/low_pass_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1628 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/median_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1892 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/min_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5682 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/data/model_delta.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8334 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/data/path_dict.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1291 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/precision.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3466 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/publication.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4181 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/data/queue_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8858 2023-04-17 09:22:53.000000 scs-core-2.8.2/src/scs_core/data/recurring_period.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1265 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/regression.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4348 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/data/rtc_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2249 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/data/sample_delta.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10713 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/stats.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1280 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/str.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7391 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/timedelta.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2185 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/tokens.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7456 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/data/topic_path.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.754826 scs-core-2.8.2/src/scs_core/display/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/display/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3786 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/display/display_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.754826 scs-core-2.8.2/src/scs_core/email/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/email/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2131 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/email/email_queue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2420 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/email/email_queue_manager.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/estate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/estate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6202 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/estate/baseline_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    33022 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/estate/configuration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4521 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/estate/configuration_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5221 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/estate/git_pull.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3621 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/estate/git_pull_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6675 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/estate/mqtt_device_poller.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2450 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/estate/mqtt_peer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6563 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/estate/package_version.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/exegesis/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/exegesis/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/exegesis/gas/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/exegesis/gas/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      693 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/exegesis/gas/exegete_catalogue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1345 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/exegesis/gas/exegete_collection.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/exegesis/particulate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/exegesis/particulate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      701 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/exegesis/particulate/exegete_catalogue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1353 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/exegesis/particulate/exegete_collection.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2248 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/exegesis/particulate/text.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/gas/
--rw-rw-r--   0 jade      (1002) jade      (1002)      292 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/gas/a4/
--rw-rw-r--   0 jade      (1002) jade      (1002)      410 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3700 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10274 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5667 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4131 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_v1.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3932 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_vA.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_vB.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_vC.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4662 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6990 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_temp_comp.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/gas/afe/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/afe/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1542 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/afe/afe_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3242 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/afe/pt1000_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2445 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/afe/pt1000_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3600 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/afe_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11555 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/afe_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6742 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/afe_id.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/gas/d4/
--rw-rw-r--   0 jade      (1002) jade      (1002)      130 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/d4/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3710 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/d4/d4_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3106 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/dsi_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4204 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/gas.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/gas/isi/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/isi/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1373 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/isi/isi_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7366 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/gas/minimum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/gas/ndir/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/ndir/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1777 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/ndir/ndir.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2723 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/ndir/ndir_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3350 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/ndir/ndir_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3649 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/ndir/ndir_version.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3065 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/ndir/ndir_voltages.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/gas/pid/
--rw-rw-r--   0 jade      (1002) jade      (1002)      378 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/pid/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4106 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/pid/pid.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4196 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/pid/pid_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4028 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/pid/pid_calibrated_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3730 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/pid/pid_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3694 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/pid/pid_temp_comp.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/gas/scd30/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/scd30/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2538 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/scd30/scd30_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2804 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/scd30/scd30_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2866 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/scd30/scd30_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3556 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/sensor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6165 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/gas/sensor_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3043 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/sensor_calib.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/gps/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gps/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4077 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gps/gps_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/interface/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/interface/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2271 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/interface/interface_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/led/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/led/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      870 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/led/led.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2343 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/led/led_state.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/location/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/location/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2992 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/location/timezone.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3708 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/location/timezone_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2379 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/location/timezone_offset.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/catalogue/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/catalogue/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11042 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/model/catalogue/model_compendium.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4774 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/catalogue/model_compendium_group.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5220 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/catalogue/term.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2038 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/catalogue/training_period.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/gas/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3349 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1354 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/gas_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1545 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/gas_inference_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2932 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/gas_model_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/gas/s1/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/s1/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2704 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/s1/gas_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3344 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/s1/s1_gas_inference_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/gas/vB/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/vB/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2702 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/vB/gas_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3120 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/vB/vb_gas_inference_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/gas/vE/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/vE/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3535 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/vE/gas_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4409 2022-10-03 10:46:58.000000 scs-core-2.8.2/src/scs_core/model/gas/vE/ve_gas_inference_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1218 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/vcal_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3488 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/model/model_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/pmx/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/pmx/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1549 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/pmx/pmx_inference_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1609 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/pmx/pmx_model_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/model/pmx/s1/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/pmx/s1/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2215 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/pmx/s1/pmx_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2051 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/monitor/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/monitor/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1558 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/monitor/monitor_error.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1557 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/monitor/monitor_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1395 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/monitor/monitor_response.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/particulate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/particulate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4558 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/particulate/opc_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5142 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/particulate/opc_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2610 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/particulate/opc_version.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2103 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/particulate/pmx_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6405 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/particulate/sps_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/position/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4062 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/position/gps_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/position/nmea/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1578 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gpdatetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4215 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gpgga.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gpgll.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gpgsa.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3850 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gpgsv.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2500 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gploc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4056 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gprmc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1318 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gptime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gpvtg.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2535 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/nmea_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      782 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/nmea_sentence.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3884 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/position/position.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/psu/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/psu/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2320 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/psu/psu.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4543 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/psu/psu_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1733 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/psu/psu_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1728 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/psu/psu_uptime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5663 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/psu/psu_version.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/sample/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sample/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3421 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sample/climate_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    12029 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/sample/configuration_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5262 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sample/gases_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3724 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sample/particulates_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2872 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sample/pressure_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4034 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sample/sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5876 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sample/status_sample.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/sampler/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sampler/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1263 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sampler/sampler.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/sync/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sync/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2168 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sync/interval_timer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1681 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sync/line_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      606 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sync/runner.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6819 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/sync/schedule.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1811 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sync/synchronised_process.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1724 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sync/timed_runner.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.770826 scs-core-2.8.2/src/scs_core/sys/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1791 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/sys/command.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4443 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/disk_usage.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/disk_volume.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2399 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/eeprom_image.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2622 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/exception_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6991 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/sys/filesystem.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1994 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/ipv4_address.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1167 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/sys/logging.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1297 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sys/memory.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    17409 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/sys/modem.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5733 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/network.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5974 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/sys/node.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3851 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/persistence_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2318 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/sys/platform.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      834 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/process_comms.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4919 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/sys/ps_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3284 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/serial.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2405 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/shared_secret.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2506 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/signalled_exit.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2244 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/subprocess.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5730 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/sys/system_id.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2013 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/sys/system_temp.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6610 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/sys/tail.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1409 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/timeout.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1192 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sys/timer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1784 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/trace_entry.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5602 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/sys/uptime_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core.egg-info/
--rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-06-26 13:24:09.000000 scs-core-2.8.2/src/scs_core.egg-info/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)    13337 2023-06-26 13:24:09.000000 scs-core-2.8.2/src/scs_core.egg-info/SOURCES.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-26 13:24:09.000000 scs-core-2.8.2/src/scs_core.egg-info/dependency_links.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-06-26 13:24:09.000000 scs-core-2.8.2/src/scs_core.egg-info/requires.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        9 2023-06-26 13:24:09.000000 scs-core-2.8.2/src/scs_core.egg-info/top_level.txt
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.373073 scs-core-2.8.4/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:27.000000 scs-core-2.8.4/LICENSE
+-rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:27.000000 scs-core-2.8.4/MANIFEST.in
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-06-30 08:18:12.373073 scs-core-2.8.4/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1404 2023-06-26 09:33:48.000000 scs-core-2.8.4/README.md
+-rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:27.000000 scs-core-2.8.4/README.rst
+-rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-02-06 14:01:57.000000 scs-core-2.8.4/requirements.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-30 08:18:12.373073 scs-core-2.8.4/setup.cfg
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1996 2022-08-17 09:53:27.000000 scs-core-2.8.4/setup.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.289073 scs-core-2.8.4/src/
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.293073 scs-core-2.8.4/src/scs_core/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      183 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.293073 scs-core-2.8.4/src/scs_core/aqcsv/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.293073 scs-core-2.8.4/src/scs_core/aqcsv/conf/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/conf/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2617 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/conf/airnow_site_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1034 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/conf/airnow_uploader_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.293073 scs-core-2.8.4/src/scs_core/aqcsv/connector/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/connector/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10203 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/aqcsv/connector/airnow_mapping_task.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6655 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/connector/datum_mapping.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5042 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/connector/source_mapping.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.297073 scs-core-2.8.4/src/scs_core/aqcsv/data/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/data/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3750 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/data/aqcsv_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    13723 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/data/aqcsv_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3033 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/data/aqcsv_site.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.297073 scs-core-2.8.4/src/scs_core/aqcsv/specification/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2824 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/agency.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2728 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/country.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1163 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/country_iso.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1175 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/country_numeric.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9800 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/method.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3765 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/mpc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3453 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/parameter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2855 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/qc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3732 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/qualifier.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2879 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aqcsv/specification/unit.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.297073 scs-core-2.8.4/src/scs_core/aws/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.301073 scs-core-2.8.4/src/scs_core/aws/client/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/client/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3585 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/client/access_key.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2332 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/client/api_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2113 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/client/api_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1217 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/client/client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5103 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/client/client_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1281 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/client/device_control_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3294 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/client/email_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3361 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/client/monitor_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5891 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/aws/client/mqtt_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3856 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/client/rest_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.301073 scs-core-2.8.4/src/scs_core/aws/config/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/config/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      744 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/config/aws.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4471 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/aws/config/project.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.305073 scs-core-2.8.4/src/scs_core/aws/data/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    16736 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/data/alert.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9274 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/data/byline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1792 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/byline_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4640 2023-04-17 09:22:53.000000 scs-core-2.8.4/src/scs_core/aws/data/dataset.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3550 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/deployment.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5315 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/data/device_monitor_email_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    13432 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/data/device_monitor_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3313 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/data/device_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4032 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/aws/data/email_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2859 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/data/http_response.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/message.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1776 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/power_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1820 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/runtime_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1795 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/status_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2884 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/upload_interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1793 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/data/uptime_list.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.305073 scs-core-2.8.4/src/scs_core/aws/greengrass/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1998 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/aws_deployer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3017 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/aws_deployment_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9610 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/aws_group.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    16440 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/aws_group_configuration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11557 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/aws_identity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      440 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/greengrass/gg_errors.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.313073 scs-core-2.8.4/src/scs_core/aws/manager/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/manager/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8285 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/alert_specification_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/alert_status_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3950 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/byline_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/configuration_check_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3256 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/configuration_check_requester.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10816 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/configuration_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2288 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/manager/device_monitor_specification_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/manager/device_monitor_status_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10307 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/dynamo_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3551 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/manager/ec2_message_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6470 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/manager/lambda_bylines.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    15996 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/aws/manager/lambda_message_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    18045 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/aws/manager/s3_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4295 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/manager/sagemaker_model_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7802 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/manager/sagemaker_trial_manager.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.313073 scs-core-2.8.4/src/scs_core/aws/security/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/aws/security/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/access_key_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5114 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_client_credentials.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7717 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_device.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1498 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_device_creator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3111 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_device_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1911 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_device_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10555 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_login_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2181 2023-04-17 09:22:53.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_membership.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2314 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_password_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11627 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_user.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3227 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_user_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3871 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/aws/security/cognito_user_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/device_whitelist_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1947 2023-04-17 09:22:53.000000 scs-core-2.8.4/src/scs_core/aws/security/opr_membership.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    22905 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/organisation.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9601 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/organisation_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1752 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/aws/security/path_filter.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.317073 scs-core-2.8.4/src/scs_core/client/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/client/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4470 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/client/http_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7463 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/client/http_exception.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      497 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/client/http_status.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2831 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/client/network.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1415 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/client/resource_unavailable_exception.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2638 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/client/sftp_client_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.317073 scs-core-2.8.4/src/scs_core/climate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1407 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/absolute_humidity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1418 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/icp10101_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3081 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/mpl115a2_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2911 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/mpl115a2_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2290 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/pressure_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2188 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/pressure_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3156 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/sht_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1844 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/climate/sht_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.321073 scs-core-2.8.4/src/scs_core/comms/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/comms/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3125 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/comms/mqtt_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2395 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/comms/uds_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1552 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/comms/uds_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2350 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/comms/uds_server.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1614 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/comms/uds_writer.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.321073 scs-core-2.8.4/src/scs_core/control/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/control/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4918 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/control/command.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4896 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/control/control_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3792 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/control/control_handler.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4737 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/control/control_receipt.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.325073 scs-core-2.8.4/src/scs_core/csv/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/csv/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1979 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/csv/csv_archive.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7484 2023-04-17 09:22:53.000000 scs-core-2.8.4/src/scs_core/csv/csv_dict.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5996 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/csv/csv_log.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8594 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/csv/csv_log_cursor_queue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8574 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/csv/csv_log_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8240 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/csv/csv_logger.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3323 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/csv/csv_logger_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5347 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/csv/csv_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4503 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/csv/csv_writer.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.333073 scs-core-2.8.4/src/scs_core/data/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4802 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/aggregate.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2050 2023-06-30 08:17:13.000000 scs-core-2.8.4/src/scs_core/data/array_dict.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2415 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/average.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2158 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/categorical_regression.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8964 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/data/checkpoint_generator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1008 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/crc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2092 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/crypt.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    19704 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/data/datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6448 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/data/datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2634 2023-04-17 09:22:53.000000 scs-core-2.8.4/src/scs_core/data/duplicates.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3809 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/data/histogram.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1747 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5951 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/join.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    14204 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/data/json.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3274 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/lin_regress.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5364 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/linear_regression.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/low_pass_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1628 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/median_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1892 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/min_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5682 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/data/model_delta.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8334 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/data/path_dict.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1291 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/precision.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3466 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/publication.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4181 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/data/queue_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8858 2023-04-17 09:22:53.000000 scs-core-2.8.4/src/scs_core/data/recurring_period.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1265 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/regression.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4348 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/data/rtc_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2249 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/data/sample_delta.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10713 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/stats.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1280 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/str.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7391 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/timedelta.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2185 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/data/tokens.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7456 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/data/topic_path.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.333073 scs-core-2.8.4/src/scs_core/display/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/display/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3786 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/display/display_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.333073 scs-core-2.8.4/src/scs_core/email/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/email/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2131 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/email/email_queue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2420 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/email/email_queue_manager.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.337073 scs-core-2.8.4/src/scs_core/estate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/estate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6202 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/estate/baseline_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    33022 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/estate/configuration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4521 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/estate/configuration_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5221 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/estate/git_pull.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3621 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/estate/git_pull_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6675 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/estate/mqtt_device_poller.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2450 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/estate/mqtt_peer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6563 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/estate/package_version.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.337073 scs-core-2.8.4/src/scs_core/exegesis/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/exegesis/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.337073 scs-core-2.8.4/src/scs_core/exegesis/gas/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/exegesis/gas/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      693 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/exegesis/gas/exegete_catalogue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1345 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/exegesis/gas/exegete_collection.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.337073 scs-core-2.8.4/src/scs_core/exegesis/particulate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/exegesis/particulate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      701 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/exegesis/particulate/exegete_catalogue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1353 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/exegesis/particulate/exegete_collection.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2248 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/exegesis/particulate/text.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.337073 scs-core-2.8.4/src/scs_core/gas/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      292 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.341073 scs-core-2.8.4/src/scs_core/gas/a4/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      410 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3700 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10274 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5667 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4131 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_v1.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3932 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_vA.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_vB.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_vC.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4662 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6990 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/a4/a4_temp_comp.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.341073 scs-core-2.8.4/src/scs_core/gas/afe/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/afe/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1542 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/afe/afe_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3242 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/afe/pt1000_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2445 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/afe/pt1000_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3600 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/afe_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11555 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/afe_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6742 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/afe_id.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.341073 scs-core-2.8.4/src/scs_core/gas/d4/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      130 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/d4/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3710 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/d4/d4_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3106 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/dsi_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4204 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/gas.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.341073 scs-core-2.8.4/src/scs_core/gas/isi/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/isi/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1373 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/isi/isi_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7366 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/gas/minimum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.345073 scs-core-2.8.4/src/scs_core/gas/ndir/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/ndir/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1777 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/ndir/ndir.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2723 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/ndir/ndir_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3350 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/ndir/ndir_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3649 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/ndir/ndir_version.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3065 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/ndir/ndir_voltages.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.345073 scs-core-2.8.4/src/scs_core/gas/pid/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      378 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/pid/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4106 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/pid/pid.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4196 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/pid/pid_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4028 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/pid/pid_calibrated_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3730 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/pid/pid_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3694 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/pid/pid_temp_comp.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.345073 scs-core-2.8.4/src/scs_core/gas/scd30/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/scd30/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2538 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/scd30/scd30_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2804 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/scd30/scd30_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2866 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gas/scd30/scd30_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3556 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/sensor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6165 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/gas/sensor_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3043 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/gas/sensor_calib.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.345073 scs-core-2.8.4/src/scs_core/gps/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gps/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4077 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/gps/gps_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.345073 scs-core-2.8.4/src/scs_core/interface/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/interface/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2271 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/interface/interface_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.345073 scs-core-2.8.4/src/scs_core/led/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/led/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      870 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/led/led.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2343 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/led/led_state.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.349073 scs-core-2.8.4/src/scs_core/location/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/location/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2992 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/location/timezone.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3708 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/location/timezone_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2379 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/location/timezone_offset.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.349073 scs-core-2.8.4/src/scs_core/model/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.349073 scs-core-2.8.4/src/scs_core/model/catalogue/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/catalogue/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11042 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/model/catalogue/model_compendium.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4774 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/catalogue/model_compendium_group.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5220 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/catalogue/term.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2038 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/catalogue/training_period.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.349073 scs-core-2.8.4/src/scs_core/model/gas/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3349 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1354 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/gas_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1545 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/gas_inference_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2932 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/gas_model_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.349073 scs-core-2.8.4/src/scs_core/model/gas/s1/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/s1/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2704 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/s1/gas_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3344 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/s1/s1_gas_inference_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.353073 scs-core-2.8.4/src/scs_core/model/gas/vB/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/vB/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2702 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/vB/gas_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3120 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/vB/vb_gas_inference_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.353073 scs-core-2.8.4/src/scs_core/model/gas/vE/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/vE/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3535 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/vE/gas_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4409 2022-10-03 10:46:58.000000 scs-core-2.8.4/src/scs_core/model/gas/vE/ve_gas_inference_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1218 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/gas/vcal_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3488 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/model/model_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.353073 scs-core-2.8.4/src/scs_core/model/pmx/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/pmx/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1549 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/pmx/pmx_inference_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1609 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/pmx/pmx_model_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.353073 scs-core-2.8.4/src/scs_core/model/pmx/s1/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/pmx/s1/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2215 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/pmx/s1/pmx_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2051 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.353073 scs-core-2.8.4/src/scs_core/monitor/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/monitor/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1558 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/monitor/monitor_error.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1557 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/monitor/monitor_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1395 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/monitor/monitor_response.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.357073 scs-core-2.8.4/src/scs_core/particulate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/particulate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4558 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/particulate/opc_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5142 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/particulate/opc_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2610 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/particulate/opc_version.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2103 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/particulate/pmx_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6405 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/particulate/sps_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.357073 scs-core-2.8.4/src/scs_core/position/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4062 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/position/gps_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.361073 scs-core-2.8.4/src/scs_core/position/nmea/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1578 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gpdatetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4215 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gpgga.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gpgll.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gpgsa.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3850 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gpgsv.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2500 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gploc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4056 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gprmc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1318 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gptime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/gpvtg.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2535 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/nmea_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      782 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/position/nmea/nmea_sentence.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3884 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/position/position.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.361073 scs-core-2.8.4/src/scs_core/psu/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/psu/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2320 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/psu/psu.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4543 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/psu/psu_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1733 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/psu/psu_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1728 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/psu/psu_uptime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5663 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/psu/psu_version.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.361073 scs-core-2.8.4/src/scs_core/sample/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sample/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3421 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sample/climate_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    12029 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/sample/configuration_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5262 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sample/gases_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3724 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sample/particulates_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2872 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sample/pressure_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4034 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sample/sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5876 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sample/status_sample.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.365073 scs-core-2.8.4/src/scs_core/sampler/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sampler/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1263 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sampler/sampler.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.365073 scs-core-2.8.4/src/scs_core/sync/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sync/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2168 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sync/interval_timer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1681 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sync/line_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      606 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sync/runner.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6819 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/sync/schedule.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1811 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sync/synchronised_process.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1724 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sync/timed_runner.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.373073 scs-core-2.8.4/src/scs_core/sys/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1791 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/sys/command.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4443 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/disk_usage.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/disk_volume.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2399 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/eeprom_image.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2622 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/exception_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6991 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/sys/filesystem.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1994 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/ipv4_address.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1167 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/sys/logging.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1297 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sys/memory.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    17409 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/sys/modem.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5733 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/network.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5974 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/sys/node.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3851 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/persistence_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2318 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/sys/platform.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      834 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/process_comms.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4919 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/sys/ps_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3284 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/serial.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2405 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/shared_secret.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2506 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/signalled_exit.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2244 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/subprocess.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5730 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/sys/system_id.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2013 2023-06-26 09:33:48.000000 scs-core-2.8.4/src/scs_core/sys/system_temp.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6610 2023-03-20 10:12:25.000000 scs-core-2.8.4/src/scs_core/sys/tail.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1409 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/timeout.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1192 2023-02-06 14:01:57.000000 scs-core-2.8.4/src/scs_core/sys/timer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1784 2022-08-17 09:53:27.000000 scs-core-2.8.4/src/scs_core/sys/trace_entry.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5602 2022-09-20 10:07:36.000000 scs-core-2.8.4/src/scs_core/sys/uptime_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:18:12.293073 scs-core-2.8.4/src/scs_core.egg-info/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-06-30 08:18:12.000000 scs-core-2.8.4/src/scs_core.egg-info/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)    13337 2023-06-30 08:18:12.000000 scs-core-2.8.4/src/scs_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-30 08:18:12.000000 scs-core-2.8.4/src/scs_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-06-30 08:18:12.000000 scs-core-2.8.4/src/scs_core.egg-info/requires.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        9 2023-06-30 08:18:12.000000 scs-core-2.8.4/src/scs_core.egg-info/top_level.txt
```

### Comparing `scs-core-2.8.2/LICENSE` & `scs-core-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/PKG-INFO` & `scs-core-2.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-core
-Version: 2.8.2
+Version: 2.8.4
 Summary: The root of all South Coast Science environmental monitoring applications.
 Home-page: https://github.com/south-coast-science/scs_core
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scs-core-2.8.2/README.md` & `scs-core-2.8.4/README.md`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/setup.py` & `scs-core-2.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/conf/airnow_site_conf.py` & `scs-core-2.8.4/src/scs_core/aqcsv/conf/airnow_site_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/conf/airnow_uploader_conf.py` & `scs-core-2.8.4/src/scs_core/aqcsv/conf/airnow_uploader_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/connector/airnow_mapping_task.py` & `scs-core-2.8.4/src/scs_core/aqcsv/connector/airnow_mapping_task.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/connector/datum_mapping.py` & `scs-core-2.8.4/src/scs_core/aqcsv/connector/datum_mapping.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/connector/source_mapping.py` & `scs-core-2.8.4/src/scs_core/aqcsv/connector/source_mapping.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/data/aqcsv_datetime.py` & `scs-core-2.8.4/src/scs_core/aqcsv/data/aqcsv_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/data/aqcsv_record.py` & `scs-core-2.8.4/src/scs_core/aqcsv/data/aqcsv_record.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/data/aqcsv_site.py` & `scs-core-2.8.4/src/scs_core/aqcsv/data/aqcsv_site.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/specification/agency.py` & `scs-core-2.8.4/src/scs_core/aqcsv/specification/agency.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/specification/country.py` & `scs-core-2.8.4/src/scs_core/aqcsv/specification/country.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/specification/country_iso.py` & `scs-core-2.8.4/src/scs_core/aqcsv/specification/country_iso.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/specification/country_numeric.py` & `scs-core-2.8.4/src/scs_core/aqcsv/specification/country_numeric.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/specification/method.py` & `scs-core-2.8.4/src/scs_core/aqcsv/specification/method.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/specification/mpc.py` & `scs-core-2.8.4/src/scs_core/aqcsv/specification/mpc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/specification/parameter.py` & `scs-core-2.8.4/src/scs_core/aqcsv/specification/parameter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/specification/qc.py` & `scs-core-2.8.4/src/scs_core/aqcsv/specification/qc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/specification/qualifier.py` & `scs-core-2.8.4/src/scs_core/aqcsv/specification/qualifier.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aqcsv/specification/unit.py` & `scs-core-2.8.4/src/scs_core/aqcsv/specification/unit.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/client/access_key.py` & `scs-core-2.8.4/src/scs_core/aws/client/access_key.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/client/api_auth.py` & `scs-core-2.8.4/src/scs_core/aws/client/api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/client/api_client.py` & `scs-core-2.8.4/src/scs_core/aws/client/api_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/client/client.py` & `scs-core-2.8.4/src/scs_core/aws/client/client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/client/client_auth.py` & `scs-core-2.8.4/src/scs_core/aws/client/client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/client/device_control_client.py` & `scs-core-2.8.4/src/scs_core/aws/client/device_control_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/client/email_client.py` & `scs-core-2.8.4/src/scs_core/aws/client/email_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/client/monitor_auth.py` & `scs-core-2.8.4/src/scs_core/aws/client/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/client/mqtt_client.py` & `scs-core-2.8.4/src/scs_core/aws/client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/client/rest_client.py` & `scs-core-2.8.4/src/scs_core/aws/client/rest_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/config/aws.py` & `scs-core-2.8.4/src/scs_core/aws/config/aws.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/config/project.py` & `scs-core-2.8.4/src/scs_core/aws/config/project.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/alert.py` & `scs-core-2.8.4/src/scs_core/aws/data/alert.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/byline.py` & `scs-core-2.8.4/src/scs_core/aws/data/byline.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import json
 
 from collections import OrderedDict
 
 from scs_core.data.array_dict import ArrayDict
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.json import JSONable
-from scs_core.data.str import Str
 from scs_core.data.topic_path import TopicPath
 
 from scs_core.sys.logging import Logging
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
@@ -241,15 +240,15 @@
             for byline in bylines:
                 yield byline
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return self.__class__.__name__ + ":{device_bylines:%s}" % Str.collection(self._device_bylines)
+        return self.__class__.__name__ + ":{device_bylines:%s}" % self._device_bylines
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class DeviceBylineGroup(BylineGroup):
     """
     classdocs
@@ -291,15 +290,15 @@
 
         self.__logger = Logging.getLogger()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def bylines_for_device(self, device):
-        return self._device_bylines[device]                     # may raise KeyError
+        return self._device_bylines[device]
 
 
     def topic_roots(self):
         topic_roots = set()
         for device_tag, bylines in self._device_bylines.items():
             for byline in bylines:
                 try:
@@ -313,7 +312,8 @@
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def devices(self):
         return tuple(self._device_bylines.keys())
+        # return self._device_bylines.keys()
```

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/byline_list.py` & `scs-core-2.8.4/src/scs_core/aws/data/byline_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/dataset.py` & `scs-core-2.8.4/src/scs_core/aws/data/dataset.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/deployment.py` & `scs-core-2.8.4/src/scs_core/aws/data/deployment.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/device_monitor_email_list.py` & `scs-core-2.8.4/src/scs_core/climate/sht_conf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,111 +1,116 @@
 """
-Created on 14 Jun 2023
+Created on 13 Dec 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-document example:
+the I2C addresses of the internal (in A4 pot) and external (exposed to air) SHTs
+
+example JSON:
+{"int": "0x44", "ext": "0x45"}
 """
 
 from collections import OrderedDict
 
 from scs_core.data.json import PersistentJSONable
-from scs_core.data.str import Str
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class DeviceMonitorEmailList(PersistentJSONable):
+class SHTConf(PersistentJSONable):
     """
     classdocs
     """
 
-    __FILENAME = "device_monitor_email_list.json"
+    __FILENAME = "sht_conf.json"
 
     @classmethod
     def persistence_location(cls):
-        return cls.aws_dir(), cls.__FILENAME
+        return cls.conf_dir(), cls.__FILENAME
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    @classmethod
+    def __addr_str(cls, addr):
+        if addr is None:
+            return None
+
+        return "0x%02x" % addr
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict, skeleton=False):
         if not jdict:
             return None
 
-        device_dict = {device_tag: set(recipients) for device_tag, recipients in jdict.items()}
+        int_str = jdict.get('int')
+        ext_str = jdict.get('ext')
+
+        int_addr = None if int_str is None else int(int_str, 0)
+        ext_addr = None if ext_str is None else int(ext_str, 0)
 
-        return cls(device_dict)
+        return cls(int_addr, ext_addr)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, device_dict):
+    def __init__(self, int_addr, ext_addr):
         """
         Constructor
         """
         super().__init__()
 
-        self.__device_dict = device_dict                            # dict of device-tag: set of emails
-
-
-    # ----------------------------------------------------------------------------------------------------------------
+        self.__int_addr = int_addr          # int       I2C address of SHT in A4 package
+        self.__ext_addr = ext_addr          # int       I2C address of SHT exposed to air
 
-    def add(self, device_tag, email_address):
-        if device_tag not in self.__device_dict:
-            self.__device_dict[device_tag] = set()
 
-        self.__device_dict[device_tag].add(email_address)
-
-
-    def discard(self, device_tag, email_address):
-        # all devices...
-        if device_tag is None:
-            for device_tag in self.__device_dict:
-                self.__device_dict[device_tag].discard(email_address)
-            return
-
-        # specific device...
-        if device_tag not in self.__device_dict:
-            return
+    def __eq__(self, other):
+        try:
+            return self.int_addr == other.int_addr and self.ext_addr == other.ext_addr
 
-        self.__device_dict[device_tag].discard(email_address)
+        except (TypeError, AttributeError):
+            return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def subset(self, email_address):
-        device_dict = {device_tag: recipients for device_tag, recipients in self.__device_dict.items()
-                       if email_address in recipients}
+    # noinspection PyMethodMayBeStatic
+    def int_sht(self):
+        return None
 
-        return DeviceMonitorEmailList(device_dict)
 
-
-    def recipients(self, device_tag):
-        try:
-            return self.__device_dict[device_tag]
-        except KeyError:
-            return None
+    # noinspection PyMethodMayBeStatic
+    def ext_sht(self):
+        return None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def device_dict(self):
-        device_dict = OrderedDict()
-        for device_tag in sorted(self.__device_dict):
-            device_dict[device_tag] = sorted(self.__device_dict[device_tag])
+    def int_addr(self):
+        return self.__int_addr
+
 
-        return device_dict
+    @property
+    def ext_addr(self):
+        return self.__ext_addr
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
-        return self.device_dict
+        jdict = OrderedDict()
+
+        jdict['int'] = SHTConf.__addr_str(self.__int_addr)
+        jdict['ext'] = SHTConf.__addr_str(self.__ext_addr)
+
+        return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "DeviceMonitorEmailList:{device_dict:%s}" %  Str.collection(self.device_dict)
+        return "SHTConf(core):{int_addr:%s, ext_addr:%s}" %  \
+               (SHTConf.__addr_str(self.int_addr), SHTConf.__addr_str(self.ext_addr))
```

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/device_monitor_report.py` & `scs-core-2.8.4/src/scs_core/aws/data/device_monitor_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class DeviceStatus(JSONable):
     """
     classdocs
     """
+
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
@@ -81,15 +82,15 @@
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
         jdict['is-ok'] = self.is_ok
-        jdict['since'] = self.since.utc()
+        jdict['since'] = None if self.since is None else self.since.utc()
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
@@ -304,14 +305,23 @@
 
         except AttributeError:
             return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
+    def matches(self, device_tag, exact):
+        if device_tag is None:
+            return True
+
+        return (exact and device_tag == self.device_tag) or (not exact and device_tag in self.device_tag)
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
     def as_json(self):
         jdict = OrderedDict()
 
         jdict['device-tag'] = self.device_tag
 
         jdict['availability'] = self.availability
         jdict['data'] = self.data
@@ -410,14 +420,26 @@
     def device(self, device_tag):
         try:
             return self.__device_dict[device_tag]
         except KeyError:
             return None
 
 
+    def filter(self, device_tag=None, exact=False):
+        device_dict = {key: report for key, report in self.__device_dict.items() if report.matches(device_tag, exact)}
+
+        return DeviceMonitorReport(device_dict)
+
+
+    def filter_devices(self, device_tags):
+        device_dict = {key: self.__device_dict[key] for key in self.__device_dict.keys() & device_tags}
+
+        return DeviceMonitorReport(device_dict)
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         return self.device_dict
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/device_report.py` & `scs-core-2.8.4/src/scs_core/aws/data/device_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/email_list.py` & `scs-core-2.8.4/src/scs_core/aws/data/email_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/http_response.py` & `scs-core-2.8.4/src/scs_core/aws/data/http_response.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/message.py` & `scs-core-2.8.4/src/scs_core/aws/data/message.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/power_list.py` & `scs-core-2.8.4/src/scs_core/aws/data/power_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/runtime_record.py` & `scs-core-2.8.4/src/scs_core/aws/data/runtime_record.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/status_list.py` & `scs-core-2.8.4/src/scs_core/aws/data/status_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/upload_interval.py` & `scs-core-2.8.4/src/scs_core/aws/data/upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/data/uptime_list.py` & `scs-core-2.8.4/src/scs_core/aws/data/uptime_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/greengrass/aws_deployer.py` & `scs-core-2.8.4/src/scs_core/aws/greengrass/aws_deployer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/greengrass/aws_deployment_reporter.py` & `scs-core-2.8.4/src/scs_core/aws/greengrass/aws_deployment_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/greengrass/aws_group.py` & `scs-core-2.8.4/src/scs_core/aws/greengrass/aws_group.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/greengrass/aws_group_configuration.py` & `scs-core-2.8.4/src/scs_core/aws/greengrass/aws_group_configuration.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/greengrass/aws_identity.py` & `scs-core-2.8.4/src/scs_core/aws/greengrass/aws_identity.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/alert_specification_manager.py` & `scs-core-2.8.4/src/scs_core/aws/manager/alert_specification_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/alert_status_manager.py` & `scs-core-2.8.4/src/scs_core/aws/manager/alert_status_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/byline_manager.py` & `scs-core-2.8.4/src/scs_core/aws/manager/byline_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/configuration_check_finder.py` & `scs-core-2.8.4/src/scs_core/aws/manager/configuration_check_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/configuration_check_requester.py` & `scs-core-2.8.4/src/scs_core/aws/manager/configuration_check_requester.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/configuration_finder.py` & `scs-core-2.8.4/src/scs_core/aws/manager/configuration_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/device_monitor_specification_manager.py` & `scs-core-2.8.4/src/scs_core/aws/manager/device_monitor_specification_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,57 +12,58 @@
 # --------------------------------------------------------------------------------------------------------------------
 
 class DeviceMonitorSpecificationManager(APIClient):
     """
     classdocs
     """
 
-    # TODO: update URL
-    __URL = "https://n0ctatmvjl.execute-api.us-west-2.amazonaws.com/default/DeviceMonitorSpecification"
+    __URL = "https://psnunpg4gb.execute-api.us-west-2.amazonaws.com/default/DeviceMonitorSpecification"
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, http_client):
         super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def find(self, token, email_address=None, device_tag_filter=None, exact=False):
+    def find(self, token, email_address=None, device_tag=None, exact=False):
         payload = {
             'email_address': email_address,
-            'device_tag': device_tag_filter,
+            'device_tag': device_tag,
             'exact': exact
         }
 
         response = self._http_client.get(self.__URL, headers=self._token_headers(token), json=payload)
         self._check_response(response)
 
-        return DeviceMonitorEmailList(response.json())
+        return DeviceMonitorEmailList.construct_from_jdict(response.json())
 
 
     def add(self, token, email_address, device_tag):
         payload = {
             'email_address': email_address,
             'device_tag': device_tag
         }
 
         response = self._http_client.post(self.__URL, headers=self._token_headers(token), json=payload)
         self._check_response(response)
 
-        return DeviceMonitorEmailList(response.json())      # only the updated entry is returned
+        return DeviceMonitorEmailList.construct_from_jdict(response.json())
 
 
     def remove(self, token, email_address, device_tag=None):
         payload = {
             'email_address': email_address,
             'device_tag': device_tag
         }
 
         response = self._http_client.delete(self.__URL, headers=self._token_headers(token), json=payload)
         self._check_response(response)
 
+        return DeviceMonitorEmailList.construct_from_jdict(response.json())
+
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
         return "DeviceMonitorSpecificationManager:{}"
```

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/device_monitor_status_manager.py` & `scs-core-2.8.4/src/scs_core/aws/manager/device_monitor_status_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 # --------------------------------------------------------------------------------------------------------------------
 
 class DeviceMonitorStatusManager(APIClient):
     """
     classdocs
     """
 
-    # TODO: update URL
-    __URL = "https://n0ctatmvjl.execute-api.us-west-2.amazonaws.com/default/DeviceMonitorStatus"
+    __URL = "https://0l7fwqkzr8.execute-api.us-west-2.amazonaws.com/default/DeviceMonitorStatus"
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, http_client):
         super().__init__(http_client)
 
 
@@ -32,16 +31,16 @@
             'device_tag': device_tag_filter,
             'exact': exact
         }
 
         response = self._http_client.get(self.__URL, headers=self._token_headers(token), json=payload)
         self._check_response(response)
 
-        report = DeviceMonitorReport(response.json())
+        return DeviceMonitorReport(response.json())
 
-        return report.device(device_tag_filter) if exact else report
+        # return report.device(device_tag_filter) if exact else report
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
         return "DeviceMonitorStatusManager:{}"
```

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/dynamo_manager.py` & `scs-core-2.8.4/src/scs_core/aws/manager/dynamo_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/ec2_message_manager.py` & `scs-core-2.8.4/src/scs_core/aws/manager/ec2_message_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/lambda_bylines.py` & `scs-core-2.8.4/src/scs_core/aws/manager/lambda_bylines.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/lambda_message_manager.py` & `scs-core-2.8.4/src/scs_core/aws/manager/lambda_message_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/s3_manager.py` & `scs-core-2.8.4/src/scs_core/aws/manager/s3_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/sagemaker_model_manager.py` & `scs-core-2.8.4/src/scs_core/aws/manager/sagemaker_model_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/manager/sagemaker_trial_manager.py` & `scs-core-2.8.4/src/scs_core/aws/manager/sagemaker_trial_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/access_key_manager.py` & `scs-core-2.8.4/src/scs_core/aws/security/access_key_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/cognito_client_credentials.py` & `scs-core-2.8.4/src/scs_core/aws/security/cognito_client_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/cognito_device.py` & `scs-core-2.8.4/src/scs_core/aws/security/cognito_device.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Created on 5 Apr 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 example document (credentials):
-{"username": "scs-opc-1", "password": "Ytzglk6oYpzJY0FB"}
+{"username": "scs-opc-1", "password": "########"}
 
 example document (identity):
-{"username": "scs-bgx-401", "password": "CiykHTLjdmE4Oqxa", "invoice": "INV-000123",
+{"username": "scs-bgx-401", "password": "########", "invoice": "INV-000123",
 "created": "2023-06-23T10:32:52+01:00", "last-updated": "2023-06-23T10:32:52+01:00"}
 """
 
 import re
 
 from collections import OrderedDict
 
@@ -143,14 +143,24 @@
 # --------------------------------------------------------------------------------------------------------------------
 
 class CognitoDeviceIdentity(CognitoDeviceCredentials):
     """
     classdocs
     """
 
+    @classmethod
+    def is_valid_invoice_number(cls, invoice_number):
+        try:
+            match = re.match(r'INV-\d{4,}', invoice_number)
+            return match is not None
+
+        except TypeError:
+            return False
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_res(cls, res):
         if not res:
             return None
```

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/cognito_device_creator.py` & `scs-core-2.8.4/src/scs_core/aws/security/cognito_device_creator.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 Enables a device to register itself as a CognitoDevice
 """
 
 from scs_core.aws.client.api_client import APIClient
-from scs_core.aws.security.cognito_device import CognitoDeviceCredentials, CognitoDeviceIdentity
+from scs_core.aws.security.cognito_device import CognitoDeviceIdentity
 
 from scs_core.data.json import JSONify
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CognitoDeviceCreator(APIClient):
@@ -26,15 +26,15 @@
 
     def __init__(self, http_client):
         super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def create(self, identity: CognitoDeviceCredentials):
+    def create(self, identity: CognitoDeviceIdentity):
         response = self._http_client.post(self.__URL, headers=self._auth_headers(self.__AUTH),
                                           data=JSONify.dumps(identity))
         self._check_response(response)
 
         return CognitoDeviceIdentity.construct_from_jdict(response.json())
```

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/cognito_device_finder.py` & `scs-core-2.8.4/src/scs_core/aws/security/cognito_device_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/cognito_device_manager.py` & `scs-core-2.8.4/src/scs_core/aws/security/cognito_device_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/cognito_login_manager.py` & `scs-core-2.8.4/src/scs_core/aws/security/cognito_login_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/cognito_membership.py` & `scs-core-2.8.4/src/scs_core/aws/security/cognito_membership.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/cognito_password_manager.py` & `scs-core-2.8.4/src/scs_core/aws/security/cognito_password_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/cognito_user.py` & `scs-core-2.8.4/src/scs_core/aws/security/cognito_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,19 @@
 Created on 22 Nov 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 https://docs.aws.amazon.com/cognito/latest/developerguide/signing-up-users-in-your-app.html
 https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-policies.html
 
-example document (identity):
-{"username": "8", "creation-date": "2021-11-24T12:51:12Z", "confirmation-status": "CONFIRMED", "enabled": true,
-"email": "bruno.beloff@southcoastscience.com", "given-name": "Bruno", "family-name": "Beloff", "is-super": true}
-
-example AWS response:
-{"username": 22, "email": "bruno.beloff@southcoastscience.com", "given-name": "Bruno", "family-name": "Beloff",
-"confirmation-status": "FORCE_CHANGE_PASSWORD", "enabled": true, "email-verified": false, "is-super": false,
-"is-tester": false, "created": "2023-03-07T15:32:17Z", "last-updated": "2023-03-08T14:12:00Z"}
+example document:
+{"username": "506cd055-1978-4984-9f17-2fad77797fa1", "email": "bruno.beloff@southcoastscience.com",
+"given-name": "Bruno", "family-name": "Beloff", "confirmation-status": "CONFIRMED", "enabled": true,
+"email-verified": true, "is-super": false, "is-tester": false, "is-financial": false,
+"created": "2023-04-20T11:45:21Z", "last-updated": "2023-06-26T14:39:17Z"}
 """
 
 import re
 
 from collections import OrderedDict
 
 from scs_core.data.datetime import LocalizedDatetime
```

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/cognito_user_finder.py` & `scs-core-2.8.4/src/scs_core/aws/security/cognito_user_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/cognito_user_manager.py` & `scs-core-2.8.4/src/scs_core/aws/security/cognito_user_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,25 @@
 
         response = self._http_client.post(self.__URL, headers=headers, json=identity.as_json())
         self._check_response(response)
 
         return CognitoUserIdentity.construct_from_jdict(response.json())
 
 
+    def confirm(self, email, confirmation_code):
+        headers = self._auth_headers(self.__AUTH)
+        payload = {
+            'email': email,
+            'confirmation': confirmation_code
+        }
+
+        response = self._http_client.patch(self.__URL, headers=headers, json=payload)
+        self._check_response(response)
+
+
 # --------------------------------------------------------------------------------------------------------------------
 
 class CognitoUserEditor(APIClient):
     """
     classdocs
     """
```

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/device_whitelist_manager.py` & `scs-core-2.8.4/src/scs_core/aws/security/device_whitelist_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/opr_membership.py` & `scs-core-2.8.4/src/scs_core/aws/security/opr_membership.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/organisation.py` & `scs-core-2.8.4/src/scs_core/aws/security/organisation.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/organisation_manager.py` & `scs-core-2.8.4/src/scs_core/aws/security/organisation_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/aws/security/path_filter.py` & `scs-core-2.8.4/src/scs_core/aws/security/path_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/client/http_client.py` & `scs-core-2.8.4/src/scs_core/client/http_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/client/http_exception.py` & `scs-core-2.8.4/src/scs_core/client/http_exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 
         if status == HTTPNotAllowedException.STATUS:
             return HTTPNotAllowedException(status, reason, data)
 
         if status == HTTPConflictException.STATUS:
             return HTTPConflictException(status, reason, data)
 
+        if status == HTTPGoneException.STATUS:
+            return HTTPGoneException(status, reason, data)
+
         if status == HTTPBadGatewayException.STATUS:
             return HTTPBadGatewayException(status, reason, data)
 
         if status == HTTPServiceUnavailableException.STATUS:
             return HTTPServiceUnavailableException(status, reason, data)
 
         if status == HTTPGatewayTimeoutException.STATUS:
@@ -180,14 +183,28 @@
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, status, reason, data):
         super().__init__(status, reason, data)
 
 
+# --------------------------------------------------------------------------------------------------------------------
+
+class HTTPGoneException(HTTPException):
+    """
+    classdocs
+    """
+    STATUS = 410
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def __init__(self, status, reason, data):
+        super().__init__(status, reason, data)
+
+
 # --------------------------------------------------------------------------------------------------------------------
 # 500 server errors...
 
 class HTTPBadGatewayException(HTTPException):
     """
     classdocs
     """
```

### Comparing `scs-core-2.8.2/src/scs_core/client/network.py` & `scs-core-2.8.4/src/scs_core/client/network.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/client/resource_unavailable_exception.py` & `scs-core-2.8.4/src/scs_core/client/resource_unavailable_exception.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/client/sftp_client_conf.py` & `scs-core-2.8.4/src/scs_core/client/sftp_client_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/climate/absolute_humidity.py` & `scs-core-2.8.4/src/scs_core/climate/absolute_humidity.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/climate/icp10101_datum.py` & `scs-core-2.8.4/src/scs_core/climate/icp10101_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/climate/mpl115a2_calib.py` & `scs-core-2.8.4/src/scs_core/climate/mpl115a2_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/climate/mpl115a2_datum.py` & `scs-core-2.8.4/src/scs_core/climate/mpl115a2_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/climate/pressure_conf.py` & `scs-core-2.8.4/src/scs_core/climate/pressure_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/climate/pressure_datum.py` & `scs-core-2.8.4/src/scs_core/climate/pressure_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/climate/sht_conf.py` & `scs-core-2.8.4/src/scs_core/exegesis/particulate/text.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,90 @@
 """
-Created on 13 Dec 2016
+Created on 26 Oct 2019
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
-
-the I2C addresses of the internal (in A4 pot) and external (exposed to air) SHTs
-
-example JSON:
-{"int": "0x44", "ext": "0x45"}
 """
 
 from collections import OrderedDict
 
-from scs_core.data.json import PersistentJSONable
+from scs_core.data.datum import Datum
+from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class SHTConf(PersistentJSONable):
+class Text(JSONable):
     """
     classdocs
     """
 
-    __FILENAME = "sht_conf.json"
-
-    @classmethod
-    def persistence_location(cls):
-        return cls.conf_dir(), cls.__FILENAME
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @classmethod
-    def __addr_str(cls, addr):
-        if addr is None:
-            return None
-
-        return "0x%02x" % addr
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_jdict(cls, jdict, skeleton=False):
+    def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
-        int_str = jdict.get('int')
-        ext_str = jdict.get('ext')
-
-        int_addr = None if int_str is None else int(int_str, 0)
-        ext_addr = None if ext_str is None else int(ext_str, 0)
+        pm1 = jdict.get('pm1')
+        pm2p5 = jdict.get('pm2p5')
+        pm10 = jdict.get('pm10')
 
-        return cls(int_addr, ext_addr)
+        return cls(pm1, pm2p5, pm10)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, int_addr, ext_addr):
+    def __init__(self, pm1, pm2p5, pm10):
         """
         Constructor
         """
-        super().__init__()
+        self.__pm1 = Datum.float(pm1, 1)                # PM1
+        self.__pm2p5 = Datum.float(pm2p5, 1)            # PM2.5
+        self.__pm10 = Datum.float(pm10, 1)              # PM10
 
-        self.__int_addr = int_addr          # int       I2C address of SHT in A4 package
-        self.__ext_addr = ext_addr          # int       I2C address of SHT exposed to air
 
+    # ----------------------------------------------------------------------------------------------------------------
 
-    def __eq__(self, other):
-        try:
-            return self.int_addr == other.int_addr and self.ext_addr == other.ext_addr
+    def as_json(self):
+        jdict = OrderedDict()
 
-        except (TypeError, AttributeError):
-            return False
+        jdict['pm1'] = self.pm1
+        jdict['pm2p5'] = self.pm2p5
+        jdict['pm10'] = self.pm10
+
+        return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    # noinspection PyMethodMayBeStatic
-    def int_sht(self):
-        return None
+    def pm(self, species):
+        if species == 'pm1':
+            return self.__pm1
 
+        if species == 'pm2p5':
+            return self.__pm2p5
 
-    # noinspection PyMethodMayBeStatic
-    def ext_sht(self):
-        return None
+        if species == 'pm10':
+            return self.__pm10
 
+        raise ValueError(species)
 
-    # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def int_addr(self):
-        return self.__int_addr
+    def pm1(self):
+        return self.__pm1
 
 
     @property
-    def ext_addr(self):
-        return self.__ext_addr
-
+    def pm2p5(self):
+        return self.__pm2p5
 
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def as_json(self):
-        jdict = OrderedDict()
 
-        jdict['int'] = SHTConf.__addr_str(self.__int_addr)
-        jdict['ext'] = SHTConf.__addr_str(self.__ext_addr)
-
-        return jdict
+    @property
+    def pm10(self):
+        return self.__pm10
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "SHTConf(core):{int_addr:%s, ext_addr:%s}" %  \
-               (SHTConf.__addr_str(self.int_addr), SHTConf.__addr_str(self.ext_addr))
+        return "Text:{pm1:%s, pm2p5:%s, pm10:%s}" % (self.pm1, self.pm2p5, self.pm10)
```

### Comparing `scs-core-2.8.2/src/scs_core/climate/sht_datum.py` & `scs-core-2.8.4/src/scs_core/climate/sht_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/comms/mqtt_conf.py` & `scs-core-2.8.4/src/scs_core/comms/mqtt_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/comms/uds_client.py` & `scs-core-2.8.4/src/scs_core/comms/uds_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/comms/uds_reader.py` & `scs-core-2.8.4/src/scs_core/comms/uds_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/comms/uds_server.py` & `scs-core-2.8.4/src/scs_core/comms/uds_server.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/comms/uds_writer.py` & `scs-core-2.8.4/src/scs_core/comms/uds_writer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/control/command.py` & `scs-core-2.8.4/src/scs_core/control/command.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/control/control_datum.py` & `scs-core-2.8.4/src/scs_core/control/control_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/control/control_handler.py` & `scs-core-2.8.4/src/scs_core/control/control_handler.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/control/control_receipt.py` & `scs-core-2.8.4/src/scs_core/control/control_receipt.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/csv/csv_archive.py` & `scs-core-2.8.4/src/scs_core/csv/csv_archive.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/csv/csv_dict.py` & `scs-core-2.8.4/src/scs_core/csv/csv_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/csv/csv_log.py` & `scs-core-2.8.4/src/scs_core/csv/csv_log.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/csv/csv_log_cursor_queue.py` & `scs-core-2.8.4/src/scs_core/csv/csv_log_cursor_queue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/csv/csv_log_reader.py` & `scs-core-2.8.4/src/scs_core/csv/csv_log_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/csv/csv_logger.py` & `scs-core-2.8.4/src/scs_core/csv/csv_logger.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/csv/csv_logger_conf.py` & `scs-core-2.8.4/src/scs_core/csv/csv_logger_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/csv/csv_reader.py` & `scs-core-2.8.4/src/scs_core/csv/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/csv/csv_writer.py` & `scs-core-2.8.4/src/scs_core/csv/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/aggregate.py` & `scs-core-2.8.4/src/scs_core/data/aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/array_dict.py` & `scs-core-2.8.4/src/scs_core/data/array_dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         return len(self.__data)
 
 
     def __contains__(self, key):
         return key in self.__data
 
 
+    def __getitem__(self, key):
+        return self.__data[key]                 # may raise KeyError
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     def append(self, key, value):
         if key not in self.__data:
             self.__data[key] = []
 
         self.__data[key].append(value)
```

### Comparing `scs-core-2.8.2/src/scs_core/data/average.py` & `scs-core-2.8.4/src/scs_core/data/average.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/categorical_regression.py` & `scs-core-2.8.4/src/scs_core/data/categorical_regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/checkpoint_generator.py` & `scs-core-2.8.4/src/scs_core/data/checkpoint_generator.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/crc.py` & `scs-core-2.8.4/src/scs_core/data/crc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/crypt.py` & `scs-core-2.8.4/src/scs_core/data/crypt.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/datetime.py` & `scs-core-2.8.4/src/scs_core/data/datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/datum.py` & `scs-core-2.8.4/src/scs_core/data/datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/duplicates.py` & `scs-core-2.8.4/src/scs_core/data/duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/histogram.py` & `scs-core-2.8.4/src/scs_core/data/histogram.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/interval.py` & `scs-core-2.8.4/src/scs_core/data/interval.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/join.py` & `scs-core-2.8.4/src/scs_core/data/join.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/json.py` & `scs-core-2.8.4/src/scs_core/data/json.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/lin_regress.py` & `scs-core-2.8.4/src/scs_core/data/lin_regress.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/linear_regression.py` & `scs-core-2.8.4/src/scs_core/data/linear_regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/low_pass_filter.py` & `scs-core-2.8.4/src/scs_core/data/low_pass_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/median_filter.py` & `scs-core-2.8.4/src/scs_core/data/median_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/min_list.py` & `scs-core-2.8.4/src/scs_core/data/min_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/model_delta.py` & `scs-core-2.8.4/src/scs_core/data/model_delta.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/path_dict.py` & `scs-core-2.8.4/src/scs_core/data/path_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/precision.py` & `scs-core-2.8.4/src/scs_core/data/precision.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/publication.py` & `scs-core-2.8.4/src/scs_core/data/publication.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/queue_report.py` & `scs-core-2.8.4/src/scs_core/data/queue_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/recurring_period.py` & `scs-core-2.8.4/src/scs_core/data/recurring_period.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/regression.py` & `scs-core-2.8.4/src/scs_core/data/regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/rtc_datetime.py` & `scs-core-2.8.4/src/scs_core/data/rtc_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/sample_delta.py` & `scs-core-2.8.4/src/scs_core/data/sample_delta.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/stats.py` & `scs-core-2.8.4/src/scs_core/data/stats.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/str.py` & `scs-core-2.8.4/src/scs_core/data/str.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/timedelta.py` & `scs-core-2.8.4/src/scs_core/data/timedelta.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/tokens.py` & `scs-core-2.8.4/src/scs_core/data/tokens.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/data/topic_path.py` & `scs-core-2.8.4/src/scs_core/data/topic_path.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/display/display_conf.py` & `scs-core-2.8.4/src/scs_core/display/display_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/email/email_queue.py` & `scs-core-2.8.4/src/scs_core/email/email_queue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/email/email_queue_manager.py` & `scs-core-2.8.4/src/scs_core/email/email_queue_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/estate/baseline_conf.py` & `scs-core-2.8.4/src/scs_core/estate/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/estate/configuration.py` & `scs-core-2.8.4/src/scs_core/estate/configuration.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/estate/configuration_check.py` & `scs-core-2.8.4/src/scs_core/estate/configuration_check.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/estate/git_pull.py` & `scs-core-2.8.4/src/scs_core/estate/git_pull.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/estate/git_pull_check.py` & `scs-core-2.8.4/src/scs_core/estate/git_pull_check.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/estate/mqtt_device_poller.py` & `scs-core-2.8.4/src/scs_core/estate/mqtt_device_poller.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/estate/mqtt_peer.py` & `scs-core-2.8.4/src/scs_core/estate/mqtt_peer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/estate/package_version.py` & `scs-core-2.8.4/src/scs_core/estate/package_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/exegesis/gas/exegete_catalogue.py` & `scs-core-2.8.4/src/scs_core/exegesis/gas/exegete_catalogue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/exegesis/gas/exegete_collection.py` & `scs-core-2.8.4/src/scs_core/exegesis/gas/exegete_collection.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/exegesis/particulate/exegete_catalogue.py` & `scs-core-2.8.4/src/scs_core/exegesis/particulate/exegete_catalogue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/exegesis/particulate/exegete_collection.py` & `scs-core-2.8.4/src/scs_core/exegesis/particulate/exegete_collection.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/exegesis/particulate/text.py` & `scs-core-2.8.4/src/scs_core/sys/platform.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,91 @@
 """
-Created on 26 Oct 2019
+Created on 28 Feb 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
+
+JSON example:
+{"rel": "4.19.103-bone47", "vers": "#1buster PREEMPT Thu Feb 20 17:40:41 UTC 2020"}
+
+https://docs.python.org/3/library/platform.html
 """
 
+import platform
+
 from collections import OrderedDict
 
-from scs_core.data.datum import Datum
 from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class Text(JSONable):
+class PlatformSummary(JSONable):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
-        pm1 = jdict.get('pm1')
-        pm2p5 = jdict.get('pm2p5')
-        pm10 = jdict.get('pm10')
+        release = jdict.get('rel')
+        version = jdict.get('vers')
 
-        return cls(pm1, pm2p5, pm10)
+        return cls(release, version)
+
+
+    @classmethod
+    def construct(cls):
+        uname = platform.uname()
+
+        return cls(uname.release, uname.version)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, pm1, pm2p5, pm10):
+    def __init__(self, release, version):
         """
         Constructor
         """
-        self.__pm1 = Datum.float(pm1, 1)                # PM1
-        self.__pm2p5 = Datum.float(pm2p5, 1)            # PM2.5
-        self.__pm10 = Datum.float(pm10, 1)              # PM10
+        self.__release = release                          # string
+        self.__version = version                          # string
+
+
+    def __eq__(self, other):
+        try:
+            return self.release == other.release and self.version == other.version
+
+        except (TypeError, AttributeError):
+            return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
-        jdict['pm1'] = self.pm1
-        jdict['pm2p5'] = self.pm2p5
-        jdict['pm10'] = self.pm10
+        jdict['rel'] = self.release
+        jdict['vers'] = self.version
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def pm(self, species):
-        if species == 'pm1':
-            return self.__pm1
-
-        if species == 'pm2p5':
-            return self.__pm2p5
-
-        if species == 'pm10':
-            return self.__pm10
-
-        raise ValueError(species)
-
-
-    @property
-    def pm1(self):
-        return self.__pm1
-
-
     @property
-    def pm2p5(self):
-        return self.__pm2p5
+    def release(self):
+        return self.__release
 
 
     @property
-    def pm10(self):
-        return self.__pm10
+    def version(self):
+        return self.__version
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "Text:{pm1:%s, pm2p5:%s, pm10:%s}" % (self.pm1, self.pm2p5, self.pm10)
+        return "PlatformSummary:{release:%s, version:%s}" %  \
+               (self.release, self.version)
```

### Comparing `scs-core-2.8.2/src/scs_core/gas/a4/a4.py` & `scs-core-2.8.4/src/scs_core/gas/a4/a4.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/a4/a4_calib.py` & `scs-core-2.8.4/src/scs_core/gas/a4/a4_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum.py` & `scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_v1.py` & `scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_v1.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_vA.py` & `scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_vA.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_vB.py` & `scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_vB.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_vC.py` & `scs-core-2.8.4/src/scs_core/gas/a4/a4_calibrated_datum_vC.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/a4/a4_datum.py` & `scs-core-2.8.4/src/scs_core/gas/a4/a4_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/a4/a4_temp_comp.py` & `scs-core-2.8.4/src/scs_core/gas/a4/a4_temp_comp.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/afe/afe_datum.py` & `scs-core-2.8.4/src/scs_core/gas/afe/afe_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/afe/pt1000_calib.py` & `scs-core-2.8.4/src/scs_core/gas/afe/pt1000_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/afe/pt1000_datum.py` & `scs-core-2.8.4/src/scs_core/gas/afe/pt1000_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/afe_baseline.py` & `scs-core-2.8.4/src/scs_core/gas/afe_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/afe_calib.py` & `scs-core-2.8.4/src/scs_core/gas/afe_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/afe_id.py` & `scs-core-2.8.4/src/scs_core/gas/afe_id.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/d4/d4_datum.py` & `scs-core-2.8.4/src/scs_core/gas/d4/d4_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/dsi_calib.py` & `scs-core-2.8.4/src/scs_core/gas/dsi_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/gas.py` & `scs-core-2.8.4/src/scs_core/gas/gas.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/isi/isi_datum.py` & `scs-core-2.8.4/src/scs_core/gas/isi/isi_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/minimum.py` & `scs-core-2.8.4/src/scs_core/gas/minimum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/ndir/ndir.py` & `scs-core-2.8.4/src/scs_core/gas/ndir/ndir.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/ndir/ndir_conf.py` & `scs-core-2.8.4/src/scs_core/gas/ndir/ndir_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/ndir/ndir_datum.py` & `scs-core-2.8.4/src/scs_core/gas/ndir/ndir_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/ndir/ndir_version.py` & `scs-core-2.8.4/src/scs_core/gas/ndir/ndir_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/ndir/ndir_voltages.py` & `scs-core-2.8.4/src/scs_core/gas/ndir/ndir_voltages.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/pid/pid.py` & `scs-core-2.8.4/src/scs_core/gas/pid/pid.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/pid/pid_calib.py` & `scs-core-2.8.4/src/scs_core/gas/pid/pid_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/pid/pid_calibrated_datum.py` & `scs-core-2.8.4/src/scs_core/gas/pid/pid_calibrated_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/pid/pid_datum.py` & `scs-core-2.8.4/src/scs_core/gas/pid/pid_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/pid/pid_temp_comp.py` & `scs-core-2.8.4/src/scs_core/gas/pid/pid_temp_comp.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/scd30/scd30_baseline.py` & `scs-core-2.8.4/src/scs_core/gas/scd30/scd30_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/scd30/scd30_conf.py` & `scs-core-2.8.4/src/scs_core/gas/scd30/scd30_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/scd30/scd30_datum.py` & `scs-core-2.8.4/src/scs_core/gas/scd30/scd30_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/sensor.py` & `scs-core-2.8.4/src/scs_core/gas/sensor.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/sensor_baseline.py` & `scs-core-2.8.4/src/scs_core/gas/sensor_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gas/sensor_calib.py` & `scs-core-2.8.4/src/scs_core/gas/sensor_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/gps/gps_conf.py` & `scs-core-2.8.4/src/scs_core/gps/gps_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/interface/interface_conf.py` & `scs-core-2.8.4/src/scs_core/interface/interface_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/led/led.py` & `scs-core-2.8.4/src/scs_core/led/led.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/led/led_state.py` & `scs-core-2.8.4/src/scs_core/led/led_state.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/location/timezone.py` & `scs-core-2.8.4/src/scs_core/location/timezone.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/location/timezone_conf.py` & `scs-core-2.8.4/src/scs_core/location/timezone_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/location/timezone_offset.py` & `scs-core-2.8.4/src/scs_core/location/timezone_offset.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/catalogue/model_compendium.py` & `scs-core-2.8.4/src/scs_core/model/catalogue/model_compendium.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/catalogue/model_compendium_group.py` & `scs-core-2.8.4/src/scs_core/model/catalogue/model_compendium_group.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/catalogue/term.py` & `scs-core-2.8.4/src/scs_core/model/catalogue/term.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/catalogue/training_period.py` & `scs-core-2.8.4/src/scs_core/model/catalogue/training_period.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/gas/baseline.py` & `scs-core-2.8.4/src/scs_core/model/gas/baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/gas/gas_baseline.py` & `scs-core-2.8.4/src/scs_core/model/gas/gas_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/gas/gas_inference_client.py` & `scs-core-2.8.4/src/scs_core/model/gas/gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/gas/gas_model_conf.py` & `scs-core-2.8.4/src/scs_core/model/gas/gas_model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/gas/s1/gas_request.py` & `scs-core-2.8.4/src/scs_core/model/gas/s1/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/gas/s1/s1_gas_inference_client.py` & `scs-core-2.8.4/src/scs_core/model/gas/s1/s1_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/gas/vB/gas_request.py` & `scs-core-2.8.4/src/scs_core/model/gas/vB/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/gas/vB/vb_gas_inference_client.py` & `scs-core-2.8.4/src/scs_core/model/gas/vB/vb_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/gas/vE/gas_request.py` & `scs-core-2.8.4/src/scs_core/model/gas/vE/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/gas/vE/ve_gas_inference_client.py` & `scs-core-2.8.4/src/scs_core/model/gas/vE/ve_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/gas/vcal_baseline.py` & `scs-core-2.8.4/src/scs_core/model/gas/vcal_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/model_conf.py` & `scs-core-2.8.4/src/scs_core/model/model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/pmx/pmx_inference_client.py` & `scs-core-2.8.4/src/scs_core/model/pmx/pmx_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/pmx/pmx_model_conf.py` & `scs-core-2.8.4/src/scs_core/model/pmx/pmx_model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/pmx/s1/pmx_request.py` & `scs-core-2.8.4/src/scs_core/model/pmx/s1/pmx_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py` & `scs-core-2.8.4/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/monitor/monitor_error.py` & `scs-core-2.8.4/src/scs_core/monitor/monitor_error.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/monitor/monitor_request.py` & `scs-core-2.8.4/src/scs_core/monitor/monitor_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/monitor/monitor_response.py` & `scs-core-2.8.4/src/scs_core/monitor/monitor_response.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/particulate/opc_conf.py` & `scs-core-2.8.4/src/scs_core/particulate/opc_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/particulate/opc_datum.py` & `scs-core-2.8.4/src/scs_core/particulate/opc_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/particulate/opc_version.py` & `scs-core-2.8.4/src/scs_core/particulate/opc_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/particulate/pmx_datum.py` & `scs-core-2.8.4/src/scs_core/particulate/pmx_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/particulate/sps_datum.py` & `scs-core-2.8.4/src/scs_core/particulate/sps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/gps_datum.py` & `scs-core-2.8.4/src/scs_core/position/gps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/nmea/gpdatetime.py` & `scs-core-2.8.4/src/scs_core/position/nmea/gpdatetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/nmea/gpgga.py` & `scs-core-2.8.4/src/scs_core/position/nmea/gpgga.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/nmea/gpgll.py` & `scs-core-2.8.4/src/scs_core/position/nmea/gpgll.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/nmea/gpgsa.py` & `scs-core-2.8.4/src/scs_core/position/nmea/gpgsa.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/nmea/gpgsv.py` & `scs-core-2.8.4/src/scs_core/position/nmea/gpgsv.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/nmea/gploc.py` & `scs-core-2.8.4/src/scs_core/position/nmea/gploc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/nmea/gprmc.py` & `scs-core-2.8.4/src/scs_core/position/nmea/gprmc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/nmea/gptime.py` & `scs-core-2.8.4/src/scs_core/position/nmea/gptime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/nmea/gpvtg.py` & `scs-core-2.8.4/src/scs_core/position/nmea/gpvtg.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/nmea/nmea_report.py` & `scs-core-2.8.4/src/scs_core/position/nmea/nmea_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/nmea/nmea_sentence.py` & `scs-core-2.8.4/src/scs_core/position/nmea/nmea_sentence.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/position/position.py` & `scs-core-2.8.4/src/scs_core/position/position.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/psu/psu.py` & `scs-core-2.8.4/src/scs_core/psu/psu.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/psu/psu_conf.py` & `scs-core-2.8.4/src/scs_core/psu/psu_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/psu/psu_report.py` & `scs-core-2.8.4/src/scs_core/psu/psu_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/psu/psu_uptime.py` & `scs-core-2.8.4/src/scs_core/psu/psu_uptime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/psu/psu_version.py` & `scs-core-2.8.4/src/scs_core/psu/psu_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sample/climate_sample.py` & `scs-core-2.8.4/src/scs_core/sample/climate_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sample/configuration_sample.py` & `scs-core-2.8.4/src/scs_core/sample/configuration_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sample/gases_sample.py` & `scs-core-2.8.4/src/scs_core/sample/gases_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sample/particulates_sample.py` & `scs-core-2.8.4/src/scs_core/sample/particulates_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sample/pressure_sample.py` & `scs-core-2.8.4/src/scs_core/sample/pressure_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sample/sample.py` & `scs-core-2.8.4/src/scs_core/sample/sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sample/status_sample.py` & `scs-core-2.8.4/src/scs_core/sample/status_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sampler/sampler.py` & `scs-core-2.8.4/src/scs_core/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sync/interval_timer.py` & `scs-core-2.8.4/src/scs_core/sync/interval_timer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sync/line_reader.py` & `scs-core-2.8.4/src/scs_core/sync/line_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sync/runner.py` & `scs-core-2.8.4/src/scs_core/sync/runner.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sync/schedule.py` & `scs-core-2.8.4/src/scs_core/sync/schedule.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sync/synchronised_process.py` & `scs-core-2.8.4/src/scs_core/sync/synchronised_process.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sync/timed_runner.py` & `scs-core-2.8.4/src/scs_core/sync/timed_runner.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/command.py` & `scs-core-2.8.4/src/scs_core/sys/command.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/disk_usage.py` & `scs-core-2.8.4/src/scs_core/sys/disk_usage.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/disk_volume.py` & `scs-core-2.8.4/src/scs_core/sys/disk_volume.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/eeprom_image.py` & `scs-core-2.8.4/src/scs_core/sys/eeprom_image.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/exception_report.py` & `scs-core-2.8.4/src/scs_core/sys/exception_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/filesystem.py` & `scs-core-2.8.4/src/scs_core/sys/filesystem.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/ipv4_address.py` & `scs-core-2.8.4/src/scs_core/sys/ipv4_address.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/logging.py` & `scs-core-2.8.4/src/scs_core/sys/logging.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/memory.py` & `scs-core-2.8.4/src/scs_core/sys/memory.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/modem.py` & `scs-core-2.8.4/src/scs_core/sys/modem.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/network.py` & `scs-core-2.8.4/src/scs_core/sys/network.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/node.py` & `scs-core-2.8.4/src/scs_core/sys/node.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/persistence_manager.py` & `scs-core-2.8.4/src/scs_core/sys/persistence_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/platform.py` & `scs-core-2.8.4/src/scs_core/sys/system_temp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,78 @@
 """
-Created on 28 Feb 2023
+Created on 10 Jan 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
-
-JSON example:
-{"rel": "4.19.103-bone47", "vers": "#1buster PREEMPT Thu Feb 20 17:40:41 UTC 2020"}
-
-https://docs.python.org/3/library/platform.html
 """
 
-import platform
-
 from collections import OrderedDict
 
 from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class PlatformSummary(JSONable):
+class SystemTemp(JSONable):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
-        release = jdict.get('rel')
-        version = jdict.get('vers')
+        board = jdict.get('brd')
+        host = jdict.get('hst')
 
-        return cls(release, version)
+        return cls(board, host)
 
 
     @classmethod
-    def construct(cls):
-        uname = platform.uname()
+    def construct(cls, board_datum, host_datum):
+        board = None if board_datum is None else board_datum.temp
+        host = None if host_datum is None else host_datum.temp
 
-        return cls(uname.release, uname.version)
+        return cls(board, host)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, release, version):
+    def __init__(self, board, host):
         """
         Constructor
         """
-        self.__release = release                          # string
-        self.__version = version                          # string
-
-
-    def __eq__(self, other):
-        try:
-            return self.release == other.release and self.version == other.version
-
-        except (TypeError, AttributeError):
-            return False
+        self.__board = board
+        self.__host = host                                          # PersistenceManager
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
-        jdict['rel'] = self.release
-        jdict['vers'] = self.version
+        jdict['brd'] = self.board
+
+        if self.host is not None:
+            jdict['hst'] = self.host
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def release(self):
-        return self.__release
+    def board(self):
+        return self.__board
 
 
     @property
-    def version(self):
-        return self.__version
+    def host(self):
+        return self.__host
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "PlatformSummary:{release:%s, version:%s}" %  \
-               (self.release, self.version)
+        return "SystemTemp:{board:%s, host:%s}" % (self.board, self.host)
```

### Comparing `scs-core-2.8.2/src/scs_core/sys/process_comms.py` & `scs-core-2.8.4/src/scs_core/sys/process_comms.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/ps_datum.py` & `scs-core-2.8.4/src/scs_core/sys/ps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/serial.py` & `scs-core-2.8.4/src/scs_core/sys/serial.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/shared_secret.py` & `scs-core-2.8.4/src/scs_core/sys/shared_secret.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/signalled_exit.py` & `scs-core-2.8.4/src/scs_core/sys/signalled_exit.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/subprocess.py` & `scs-core-2.8.4/src/scs_core/sys/subprocess.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/system_id.py` & `scs-core-2.8.4/src/scs_core/sys/system_id.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/tail.py` & `scs-core-2.8.4/src/scs_core/sys/tail.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/timeout.py` & `scs-core-2.8.4/src/scs_core/sys/timeout.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/timer.py` & `scs-core-2.8.4/src/scs_core/sys/timer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/trace_entry.py` & `scs-core-2.8.4/src/scs_core/sys/trace_entry.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core/sys/uptime_datum.py` & `scs-core-2.8.4/src/scs_core/sys/uptime_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.2/src/scs_core.egg-info/PKG-INFO` & `scs-core-2.8.4/src/scs_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-core
-Version: 2.8.2
+Version: 2.8.4
 Summary: The root of all South Coast Science environmental monitoring applications.
 Home-page: https://github.com/south-coast-science/scs_core
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scs-core-2.8.2/src/scs_core.egg-info/SOURCES.txt` & `scs-core-2.8.4/src/scs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

