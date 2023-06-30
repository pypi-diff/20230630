# Comparing `tmp/scs-analysis-2.7.6.tar.gz` & `tmp/scs-analysis-2.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-analysis-2.7.6.tar", last modified: Mon Jun 26 13:24:37 2023, max compression
+gzip compressed data, was "scs-analysis-2.7.7.tar", last modified: Fri Jun 30 08:21:15 2023, max compression
```

## Comparing `scs-analysis-2.7.6.tar` & `scs-analysis-2.7.7.tar`

### file list

```diff
@@ -1,162 +1,166 @@
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:37.782988 scs-analysis-2.7.6/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/LICENSE
--rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/MANIFEST.in
--rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-26 13:24:37.782988 scs-analysis-2.7.6/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)      766 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/README.md
--rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/README.rst
--rw-rw-r--   0 jade      (1002) jade      (1002)      216 2023-06-26 13:23:15.000000 scs-analysis-2.7.6/requirements.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-26 13:24:37.782988 scs-analysis-2.7.6/setup.cfg
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5100 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/setup.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:37.770988 scs-analysis-2.7.6/src/
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:37.778988 scs-analysis-2.7.6/src/scs_analysis/
--rwxrwxr-x   0 jade      (1002) jade      (1002)      183 2023-06-26 13:23:15.000000 scs-analysis-2.7.6/src/scs_analysis/__init__.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2467 2023-04-17 09:22:53.000000 scs-analysis-2.7.6/src/scs_analysis/access_key.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)    10112 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/alert.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4014 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/alert_status.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2235 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/aws_api_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4611 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/aws_byline.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2655 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/aws_client_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7224 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/aws_mqtt_client.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7079 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/aws_topic_history.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2139 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/aws_topic_publisher.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2918 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/aws_upload_interval.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)    14469 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/baseline.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5964 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/baseline_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:37.778988 scs-analysis-2.7.6/src/scs_analysis/chart/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/chart/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1630 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/chart/chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4546 2023-04-17 09:22:53.000000 scs-analysis-2.7.6/src/scs_analysis/chart/histo_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4249 2023-04-17 09:22:53.000000 scs-analysis-2.7.6/src/scs_analysis/chart/multi_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4317 2023-04-17 09:22:53.000000 scs-analysis-2.7.6/src/scs_analysis/chart/single_chart.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:37.782988 scs-analysis-2.7.6/src/scs_analysis/cmd/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1966 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_access_key.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9948 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_alert.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5170 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_alert_status.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2713 2022-11-09 12:09:25.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_aws_api_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3826 2022-11-09 12:09:25.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_aws_byline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3092 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_aws_client_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7868 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_aws_topic_history.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1522 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7348 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6605 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_baseline_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4665 2023-06-26 13:23:15.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_cognito_devices.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2943 2023-03-20 10:12:25.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_cognito_password.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3570 2023-03-20 10:12:25.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3183 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_cognito_user_identity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7027 2023-03-20 10:12:25.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_cognito_users.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5419 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_configuration_csv.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4706 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_configuration_monitor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4426 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3321 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_csv_collation_summary.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2867 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_csv_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_csv_join.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2774 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_csv_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2761 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_csv_segmentor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3372 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_csv_writer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3657 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_device_controller.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4066 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_histo_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3039 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_localised_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2011 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_monitor_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5603 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_mqtt_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3378 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_multi_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3490 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_node.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5404 2023-03-20 10:12:25.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_organisation_devices.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4524 2023-04-17 09:22:53.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_organisation_path_roots.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4630 2023-04-17 09:22:53.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_organisation_user_paths.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6422 2023-03-20 10:12:25.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_organisation_users.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4992 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_organisations.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3560 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_aggregate.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3536 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2628 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_concentration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2813 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_distance.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2189 2023-04-17 09:22:53.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_duplicates.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3020 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_error.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1677 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1688 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4763 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_iso_8601.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_low_pass.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2312 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_median.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2782 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_nullify.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1224 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_paths.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1579 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3899 2023-04-17 09:22:53.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_slope.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1577 2022-09-20 10:07:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_sort.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3100 2022-09-20 10:07:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_stats.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5204 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_subset.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2264 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_tally.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_time_shift.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2325 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_timezone.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3701 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_single_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1441 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_socket_receiver.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1540 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_uds.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5225 2023-06-26 13:23:15.000000 scs-analysis-2.7.6/src/scs_analysis/cognito_devices.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5753 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/cognito_password.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5483 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/cognito_user_credentials.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7831 2023-06-26 13:23:15.000000 scs-analysis-2.7.6/src/scs_analysis/cognito_user_identity.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     8197 2023-06-26 13:23:15.000000 scs-analysis-2.7.6/src/scs_analysis/cognito_users.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7418 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/configuration_csv.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3494 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/configuration_monitor.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3854 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/configuration_monitor_check.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6401 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/csv_collation_summary.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3967 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/csv_collator.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6835 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/csv_join.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5065 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/csv_reader.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4697 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/csv_segmentor.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3800 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/csv_writer.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6115 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/device_controller.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:37.782988 scs-analysis-2.7.6/src/scs_analysis/handler/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/handler/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4051 2023-03-20 10:12:25.000000 scs-analysis-2.7.6/src/scs_analysis/handler/aws_mqtt_publisher.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2329 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/handler/batch_download_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1436 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/handler/configuration_csv_generator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/handler/csv_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5893 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/handler/csv_segmentor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1184 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/handler/mqtt_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2007 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/handler/sample_midpoint.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/handler/sample_regression.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4308 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/histo_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2127 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/localised_datetime.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2544 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/monitor_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4367 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/multi_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5982 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/node.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5896 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/organisation_devices.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4713 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/organisation_path_roots.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4925 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/organisation_user_paths.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5783 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/organisation_users.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5300 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/organisations.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7233 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/sample_aggregate.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4821 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/sample_average.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5162 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/sample_collator.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5566 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/sample_concentration.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3970 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/sample_distance.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3765 2023-04-17 09:22:53.000000 scs-analysis-2.7.6/src/scs_analysis/sample_duplicates.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4685 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/sample_error.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3102 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/sample_interval.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7990 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/sample_iso_8601.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3802 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/sample_low_pass.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3571 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/sample_max.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3776 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/sample_median.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3529 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/sample_midpoint.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3570 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/sample_min.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5072 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/sample_noise.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4017 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/sample_nullify.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1667 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/sample_paths.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3320 2023-06-26 09:33:48.000000 scs-analysis-2.7.6/src/scs_analysis/sample_regression.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5707 2023-04-17 09:22:53.000000 scs-analysis-2.7.6/src/scs_analysis/sample_slope.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2502 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/sample_sort.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5928 2022-09-20 10:07:36.000000 scs-analysis-2.7.6/src/scs_analysis/sample_stats.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6001 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/sample_subset.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2897 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/sample_time_shift.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4732 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/sample_timezone.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4463 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/single_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2451 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/socket_receiver.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1891 2023-02-06 14:01:57.000000 scs-analysis-2.7.6/src/scs_analysis/timer.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1849 2022-08-17 09:53:36.000000 scs-analysis-2.7.6/src/scs_analysis/uds_receiver.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:37.778988 scs-analysis-2.7.6/src/scs_analysis.egg-info/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-26 13:24:37.000000 scs-analysis-2.7.6/src/scs_analysis.egg-info/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)     5870 2023-06-26 13:24:37.000000 scs-analysis-2.7.6/src/scs_analysis.egg-info/SOURCES.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-26 13:24:37.000000 scs-analysis-2.7.6/src/scs_analysis.egg-info/dependency_links.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)      231 2023-06-26 13:24:37.000000 scs-analysis-2.7.6/src/scs_analysis.egg-info/requires.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       13 2023-06-26 13:24:37.000000 scs-analysis-2.7.6/src/scs_analysis.egg-info/top_level.txt
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.425173 scs-analysis-2.7.7/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/LICENSE
+-rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/MANIFEST.in
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-30 08:21:15.425173 scs-analysis-2.7.7/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)      766 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/README.md
+-rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/README.rst
+-rw-rw-r--   0 jade      (1002) jade      (1002)      232 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/requirements.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-30 08:21:15.425173 scs-analysis-2.7.7/setup.cfg
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5196 2023-06-30 08:21:07.000000 scs-analysis-2.7.7/setup.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.409173 scs-analysis-2.7.7/src/
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.417173 scs-analysis-2.7.7/src/scs_analysis/
+-rwxrwxr-x   0 jade      (1002) jade      (1002)      183 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/__init__.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2467 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/access_key.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)    10112 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/alert.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4013 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/alert_status.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2235 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/aws_api_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4611 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/aws_byline.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2655 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/aws_client_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7224 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/aws_mqtt_client.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7079 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/aws_topic_history.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2139 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/aws_topic_publisher.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2918 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/aws_upload_interval.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)    14469 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/baseline.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5964 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/baseline_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.417173 scs-analysis-2.7.7/src/scs_analysis/chart/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/chart/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1630 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/chart/chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4546 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/chart/histo_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4249 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/chart/multi_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4317 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/chart/single_chart.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.425173 scs-analysis-2.7.7/src/scs_analysis/cmd/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1966 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_access_key.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9948 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_alert.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5170 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_alert_status.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2713 2022-11-09 12:09:25.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_api_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3826 2022-11-09 12:09:25.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_byline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3092 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_client_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7868 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_topic_history.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1522 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7348 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6605 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_baseline_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4665 2023-06-26 13:23:15.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_devices.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3043 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_email.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3570 2023-03-20 10:12:25.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3183 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_user_identity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7027 2023-03-20 10:12:25.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_users.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5419 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_configuration_csv.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4707 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_configuration_monitor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4426 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3321 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_collation_summary.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2867 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_join.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2774 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2761 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_segmentor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3372 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_writer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3657 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_device_controller.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5046 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_device_monitor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3267 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_device_monitor_status.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4066 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_histo_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3039 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_localised_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2011 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_monitor_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5603 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_mqtt_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3378 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_multi_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3490 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_node.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5404 2023-03-20 10:12:25.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_devices.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4524 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_path_roots.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4630 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_user_paths.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6422 2023-03-20 10:12:25.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_users.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4992 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisations.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3560 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_aggregate.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3536 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2628 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_concentration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2813 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_distance.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2189 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_duplicates.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3020 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_error.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1677 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1688 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4763 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_iso_8601.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_low_pass.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2312 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_median.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2782 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_nullify.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1224 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_paths.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1579 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3899 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_slope.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1577 2022-09-20 10:07:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_sort.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3100 2022-09-20 10:07:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_stats.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5204 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_subset.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2264 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_tally.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_time_shift.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2325 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_timezone.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3701 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_single_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1441 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_socket_receiver.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1540 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_uds.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5425 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cognito_devices.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6472 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cognito_email.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5460 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cognito_user_credentials.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7844 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cognito_user_identity.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     8291 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/cognito_users.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7435 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/configuration_csv.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3511 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/configuration_monitor.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3859 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/configuration_monitor_check.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6401 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/csv_collation_summary.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3967 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/csv_collator.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6835 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/csv_join.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5065 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/csv_reader.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4697 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/csv_segmentor.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3800 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/csv_writer.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6115 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/device_controller.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4288 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/device_monitor.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4456 2023-06-30 08:17:13.000000 scs-analysis-2.7.7/src/scs_analysis/device_monitor_status.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.425173 scs-analysis-2.7.7/src/scs_analysis/handler/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4051 2023-03-20 10:12:25.000000 scs-analysis-2.7.7/src/scs_analysis/handler/aws_mqtt_publisher.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2329 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/batch_download_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1436 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/configuration_csv_generator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/csv_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5893 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/csv_segmentor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1184 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/mqtt_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2007 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/sample_midpoint.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/handler/sample_regression.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4308 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/histo_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2127 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/localised_datetime.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2544 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/monitor_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4367 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/multi_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5982 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/node.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5896 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/organisation_devices.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4713 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/organisation_path_roots.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4925 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/organisation_user_paths.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5783 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/organisation_users.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5300 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/organisations.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7233 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/sample_aggregate.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4821 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_average.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5162 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_collator.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5566 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_concentration.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3970 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/sample_distance.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3765 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/sample_duplicates.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4685 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_error.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3102 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_interval.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7990 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_iso_8601.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3802 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_low_pass.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3571 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_max.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3776 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_median.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3529 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_midpoint.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3570 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_min.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5072 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/sample_noise.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4017 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_nullify.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1667 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/sample_paths.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3320 2023-06-26 09:33:48.000000 scs-analysis-2.7.7/src/scs_analysis/sample_regression.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5707 2023-04-17 09:22:53.000000 scs-analysis-2.7.7/src/scs_analysis/sample_slope.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2502 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_sort.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5928 2022-09-20 10:07:36.000000 scs-analysis-2.7.7/src/scs_analysis/sample_stats.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6001 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_subset.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2897 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/sample_time_shift.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4732 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/sample_timezone.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4463 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/single_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2451 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/socket_receiver.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1891 2023-02-06 14:01:57.000000 scs-analysis-2.7.7/src/scs_analysis/timer.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1849 2022-08-17 09:53:36.000000 scs-analysis-2.7.7/src/scs_analysis/uds_receiver.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:21:15.417173 scs-analysis-2.7.7/src/scs_analysis.egg-info/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-30 08:21:15.000000 scs-analysis-2.7.7/src/scs_analysis.egg-info/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6034 2023-06-30 08:21:15.000000 scs-analysis-2.7.7/src/scs_analysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-30 08:21:15.000000 scs-analysis-2.7.7/src/scs_analysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)      247 2023-06-30 08:21:15.000000 scs-analysis-2.7.7/src/scs_analysis.egg-info/requires.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       13 2023-06-30 08:21:15.000000 scs-analysis-2.7.7/src/scs_analysis.egg-info/top_level.txt
```

### Comparing `scs-analysis-2.7.6/LICENSE` & `scs-analysis-2.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/PKG-INFO` & `scs-analysis-2.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 2.7.6
+Version: 2.7.7
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `scs-analysis-2.7.6/README.md` & `scs-analysis-2.7.7/README.md`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/setup.py` & `scs-analysis-2.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,28 +66,30 @@
         'src/scs_analysis/aws_mqtt_client.py',
         'src/scs_analysis/aws_topic_history.py',
         'src/scs_analysis/aws_topic_publisher.py',
         'src/scs_analysis/aws_upload_interval.py',
         'src/scs_analysis/baseline.py',
         'src/scs_analysis/baseline_conf.py',
         'src/scs_analysis/cognito_devices.py',
-        'src/scs_analysis/cognito_password.py',
+        'src/scs_analysis/cognito_email.py',
         'src/scs_analysis/cognito_user_credentials.py',
         'src/scs_analysis/cognito_user_identity.py',
         'src/scs_analysis/cognito_users.py',
         'src/scs_analysis/configuration_csv.py',
         'src/scs_analysis/configuration_monitor.py',
         'src/scs_analysis/configuration_monitor_check.py',
         'src/scs_analysis/csv_collation_summary.py',
         'src/scs_analysis/csv_collator.py',
         'src/scs_analysis/csv_join.py',
         'src/scs_analysis/csv_reader.py',
         'src/scs_analysis/csv_segmentor.py',
         'src/scs_analysis/csv_writer.py',
         'src/scs_analysis/device_controller.py',
+        'src/scs_analysis/device_monitor.py',
+        'src/scs_analysis/device_monitor_status.py',
         'src/scs_analysis/histo_chart.py',
         'src/scs_analysis/localised_datetime.py',
         'src/scs_analysis/monitor_auth.py',
         'src/scs_analysis/multi_chart.py',
         'src/scs_analysis/node.py',
         'src/scs_analysis/organisation_devices.py',
         'src/scs_analysis/organisation_path_roots.py',
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/access_key.py` & `scs-analysis-2.7.7/src/scs_analysis/access_key.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/alert.py` & `scs-analysis-2.7.7/src/scs_analysis/alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 DESCRIPTION
 The alert utility is used to create, update, delete or find alert specifications.
 
 Alerts take the form of emails. These are sent when a parameter falls below or above specified bounds, or when the
 value is null (a null value is being reported, or no reports are available). The alert specification sets these bounds,
 together with the aggregation period (usually in minutes). The minimum period is one minute.
 
-WARNING: when an alert is triggered, only one email is sent to each of the specified recipients. No further email
-is sent until the parameter has returned within bounds and then, subsequently, exceeds the bounds. The end of an
+Important note: when an alert is triggered, only one email is sent to each of the specified recipients. No further
+email is sent until the parameter has returned within bounds and then, subsequently, exceeds the bounds. The end of an
 out-of-bound event is logged in the alert status history. A history of out-of-bounds events for each alert
 specification can be found using the alert_status utility.
 
 In --find mode, results can be filtered by description, topic, field or creator email address.
 Finder matches are exact.
 
 SYNOPSIS
@@ -259,15 +259,15 @@
         # end...
 
         # report...
         if report is not None:
             print(JSONify.dumps(report, indent=cmd.indent))
 
         if cmd.find:
-            logger.info('retrieved: %s' % len(response.alerts))
+            logger.info('retrieved: %s' % len(response))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPException as ex:
         logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/alert_status.py` & `scs-analysis-2.7.7/src/scs_analysis/alert_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 SYNOPSIS
 alert_status.py [-c CREDENTIALS] { -F { -l | -d [-a CAUSE] } | -D } [-i INDENT] [-v] ID
 
 EXAMPLES
 alert_status.py -vi4 -c bruno -Fl 87
 
 DOCUMENT EXAMPLE
-{"id": 77, "rec": "2021-09-07T11:40:00Z", "cause": null, "val": 589.6}
+{"id": 88, "rec": "2023-06-29T09:48:42Z", "cause": "NV", "val": null}
 
 SEE ALSO
 scs_analysis/alert
 scs_analysis/cognito_user_credentials
 """
 
 import requests
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/aws_api_auth.py` & `scs-analysis-2.7.7/src/scs_analysis/aws_api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/aws_byline.py` & `scs-analysis-2.7.7/src/scs_analysis/aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/aws_client_auth.py` & `scs-analysis-2.7.7/src/scs_analysis/aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/aws_mqtt_client.py` & `scs-analysis-2.7.7/src/scs_analysis/aws_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/aws_topic_history.py` & `scs-analysis-2.7.7/src/scs_analysis/aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/aws_topic_publisher.py` & `scs-analysis-2.7.7/src/scs_analysis/aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/aws_upload_interval.py` & `scs-analysis-2.7.7/src/scs_analysis/aws_upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/baseline.py` & `scs-analysis-2.7.7/src/scs_analysis/baseline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/baseline_conf.py` & `scs-analysis-2.7.7/src/scs_analysis/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/chart/chart.py` & `scs-analysis-2.7.7/src/scs_analysis/chart/chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/chart/histo_chart.py` & `scs-analysis-2.7.7/src/scs_analysis/chart/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/chart/multi_chart.py` & `scs-analysis-2.7.7/src/scs_analysis/chart/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/chart/single_chart.py` & `scs-analysis-2.7.7/src/scs_analysis/chart/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_access_key.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_access_key.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_alert.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_alert.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_alert_status.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_alert_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_aws_api_auth.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_aws_byline.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_aws_client_auth.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_aws_topic_history.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_aws_topic_publisher.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_baseline.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_baseline_conf.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_cognito_devices.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_cognito_password.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_segmentor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,89 @@
 """
-Created on 22 Nov 2021
+Created on 10 Mar 2020
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
+
+source repo: scs_analysis
 """
 
 import optparse
 
+from scs_core.data.timedelta import Timedelta
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdCognitoPassword(object):
+class CmdCSVSegmentor(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog { -e | -s | -r } EMAIL [-v]",
-                                              version="%prog 1.0")
-
-        # functions...
-        self.__parser.add_option("--send-email", "-e", type="string", action="store", dest="send_email",
-                                 help="send password email")
+        self.__parser = optparse.OptionParser(usage="%prog -m { [DD-]HH:MM[:SS] | :SS } [-i ISO] [-f FILE_PREFIX] "
+                                                    "[-v]", version="%prog 1.0")
 
-        self.__parser.add_option("--set-password", "-s", type="string", action="store", dest="set_password",
-                                 help="set password (using temporary password)")
+        # compulsory...
+        self.__parser.add_option("--max-interval", "-m", type="string", nargs=1, action="store", dest="max_interval",
+                                 help="maximum permitted interval")
+
+        # optional...
+        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
+                                 help="path for ISO 8601 datetime field (default 'rec')")
 
-        self.__parser.add_option("--reset-password", "-r", type="string", action="store", dest="reset_password",
-                                 help="reset password (using code)")
+        self.__parser.add_option("--file-prefix", "-f", type="string", nargs=1, action="store", dest="file_prefix",
+                                 help="file prefix for contiguous CSVs")
 
-        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        count = 0
-
-        if self.send_email:
-            count += 1
-
-        if self.set_password:
-            count += 1
-
-        if self.reset_password:
-            count += 1
-
-        if count != 1:
+        if self.__opts.max_interval is None:
             return False
 
         return True
 
 
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @property
-    def email(self):
-        if self.send_email:
-            return self.__opts.send_email
-
-        if self.set_password:
-            return self.__opts.set_password
+    def is_valid_interval(self):
+        if self.__opts.max_interval is None:
+            return True
 
-        if self.reset_password:
-            return self.__opts.reset_password
+        return self.max_interval is not None
 
-        return None
 
+    # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def send_email(self):
-        return self.__opts.send_email is not None
+    def max_interval(self):
+        return Timedelta.construct_from_flag(self.__opts.max_interval)
 
 
     @property
-    def set_password(self):
-        return self.__opts.set_password is not None
+    def iso(self):
+        return self.__opts.iso
 
 
     @property
-    def reset_password(self):
-        return self.__opts.reset_password is not None
+    def file_prefix(self):
+        return self.__opts.file_prefix
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdCognitoPassword:{send_email:%s, set_password:%s, reset:%s, verbose:%s}" % \
-               (self.__opts.send_email, self.__opts.set_password, self.__opts.reset_password, self.verbose)
+        return "CmdCSVSegmentor:{max_interval:%s, iso:%s, file_prefix:%s, verbose:%s}" % \
+               (self.__opts.max_interval, self.iso, self.file_prefix, self.verbose)
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_cognito_user_credentials.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_cognito_user_identity.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_user_identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class CmdCognitoUserIdentity(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] | -C | -R | -U } [-i INDENT] [-v]",
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -C | -R | -U } [-i INDENT] [-v]",
                                               version="%prog 1.0")
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_cognito_users.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_configuration_csv.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_configuration_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -n | -s | -l OUTPUT_CSV | "
-                                                    "{ -d | -f } [-o OUTPUT_CSV_DIR] } [-t DEVICE_TAG [-e]] "
+                                                    "{ -d | -f } [-o OUTPUT_CSV_DIR] } [-t DEVICE_TAG [-x]] "
                                                     "[-v] [NODE_1..NODE_N]", version="%prog 1.0")
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # help...
@@ -43,15 +43,15 @@
         self.__parser.add_option("--full-histories", "-f", action="store_true", dest="full_histories", default=False,
                                  help="retrieve full configuration histories")
 
         # filter...
         self.__parser.add_option("--device-tag", "-t", type="string", action="store", dest="device_tag",
                                  help="the device for the history report")
 
-        self.__parser.add_option("--exactly", "-e", action="store_true", dest="exact_match", default=False,
+        self.__parser.add_option("--exactly", "-x", action="store_true", dest="exact_match", default=False,
                                  help="exact match for tag")
 
         # output...
         self.__parser.add_option("--output-csv-dir", "-o", type="string", action="store", dest="output_csv_dir",
                                  help="the directory in which to write histories")
 
         # narrative...
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_configuration_monitor.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_configuration_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 class CmdConfigurationMonitor(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [-t TAG [-e]] { -l | -f | -d | -o } "
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [-t TAG [-x]] { -l | -f | -d | -o } "
                                                     "[-i INDENT] [-v]", version="%prog 1.0")
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # filters...
         self.__parser.add_option("--tag-filter", "-t", type="string", action="store", dest="tag_filter",
                                  help="the (partial) tag of the device(s)")
 
-        self.__parser.add_option("--exactly", "-e", action="store_true", dest="exact_match", default=False,
+        self.__parser.add_option("--exactly", "-x", action="store_true", dest="exact_match", default=False,
                                  help="exact match for tag")
 
         # mode...
         self.__parser.add_option("--latest", "-l", action="store_true", dest="latest", default=False,
                                  help="report latest configuration for each device")
 
         self.__parser.add_option("--full-history", "-f", action="store_true", dest="history", default=False,
@@ -99,14 +99,15 @@
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def credentials_name(self):
         return self.__opts.credentials_name
 
+
     @property
     def tag_filter(self):
         return self.__opts.tag_filter
 
 
     @property
     def exact_match(self):
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_configuration_monitor_check.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_configuration_monitor_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 
     def __init__(self):
         """
         Constructor
         """
         codes = ' | '.join(ConfigurationCheck.result_codes())
 
-        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -f TAG | [-t TAG [-e]] [-o] } "
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -f TAG | [-t TAG [-x]] [-o] } "
                                                     "[-i INDENT] [-v]", version="%prog 1.0")
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--force", "-f", type="string", action="store", dest="force",
                                  help="force check the device with TAG now")
 
         # filters...
         self.__parser.add_option("--tag-filter", "-t", type="string", action="store", dest="tag_filter",
                                  help="the (partial) tag of the device(s)")
 
-        self.__parser.add_option("--exactly", "-e", action="store_true", dest="exact_match", default=False,
+        self.__parser.add_option("--exactly", "-x", action="store_true", dest="exact_match", default=False,
                                  help="exact match for tag")
 
         self.__parser.add_option("--result", "-r", type="string", nargs=1, action="store", dest="result_code",
                                  help="match the result { %s }" % codes)
 
         # output...
         self.__parser.add_option("--tags-only", "-o", action="store_true", dest="tags_only", default=False,
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_csv_collation_summary.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_csv_collator.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_csv_join.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_csv_reader.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_csv_segmentor.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_distance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,95 @@
 """
-Created on 10 Mar 2020
+Created on 11 Jul 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
-from scs_core.data.timedelta import Timedelta
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdCSVSegmentor(object):
+class CmdSampleDistance(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog -m { [DD-]HH:MM[:SS] | :SS } [-i ISO] [-f FILE_PREFIX] "
-                                                    "[-v]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog -p LAT LNG [-i ISO] [-q QUALITY] [-v] GPS_PATH",
+                                              version="%prog 1.0")
 
         # compulsory...
-        self.__parser.add_option("--max-interval", "-m", type="string", nargs=1, action="store", dest="max_interval",
-                                 help="maximum permitted interval")
+        self.__parser.add_option("--position", "-p", type="float", nargs=2, action="store", dest="position",
+                                 help="position (in degrees)")
 
         # optional...
         self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
-                                 help="path for ISO 8601 datetime field (default 'rec')")
+                                 help="path for ISO 8601 datetime output (default 'rec')")
 
-        self.__parser.add_option("--file-prefix", "-f", type="string", nargs=1, action="store", dest="file_prefix",
-                                 help="file prefix for contiguous CSVs")
+        self.__parser.add_option("--quality", "-q", type="int", nargs=1, action="store", dest="quality",
+                                 help="minimum acceptable GPS quality")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.__opts.max_interval is None:
+        if self.position is None or self.path is None:
             return False
 
         return True
 
 
-    def is_valid_interval(self):
-        if self.__opts.max_interval is None:
-            return True
+    # ----------------------------------------------------------------------------------------------------------------
 
-        return self.max_interval is not None
+    @property
+    def position(self):
+        return self.__opts.position
 
 
-    # ----------------------------------------------------------------------------------------------------------------
+    @property
+    def lat(self):
+        return None if self.__opts.position is None else self.__opts.position[0]
+
 
     @property
-    def max_interval(self):
-        return Timedelta.construct_from_flag(self.__opts.max_interval)
+    def lng(self):
+        return None if self.__opts.position is None else self.__opts.position[1]
 
 
     @property
     def iso(self):
         return self.__opts.iso
 
 
     @property
-    def file_prefix(self):
-        return self.__opts.file_prefix
+    def quality(self):
+        return self.__opts.quality
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
+    @property
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdCSVSegmentor:{max_interval:%s, iso:%s, file_prefix:%s, verbose:%s}" % \
-               (self.__opts.max_interval, self.iso, self.file_prefix, self.verbose)
+        return "CmdSampleDistance:{position:%s, iso:%s, quality:%s, verbose:%s, path:%s}" % \
+               (self.position, self.iso, self.quality, self.verbose, self.path)
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_csv_writer.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_device_controller.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_device_controller.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_histo_chart.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_localised_datetime.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_monitor_auth.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_mqtt_client.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_multi_chart.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_node.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_organisation_devices.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_organisation_path_roots.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_organisation_user_paths.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_organisation_users.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_organisations.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_organisations.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_aggregate.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_collator.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_concentration.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_concentration.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_distance.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_nullify.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,91 @@
 """
-Created on 11 Jul 2016
+Created on 4 Sep 2019
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleDistance(object):
+class CmdSampleNullify(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog -p LAT LNG [-i ISO] [-q QUALITY] [-v] GPS_PATH",
-                                              version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog -t TARGET_PATH -s SOURCE_PATH [-l LOWER] [-u UPPER]"
+                                                    " [-v]", version="%prog 1.0")
 
         # compulsory...
-        self.__parser.add_option("--position", "-p", type="float", nargs=2, action="store", dest="position",
-                                 help="position (in degrees)")
+        self.__parser.add_option("--target", "-t", type="string", nargs=1, action="store", dest="target",
+                                 help="field to be nullified")
+
+        self.__parser.add_option("--source", "-s", type="string", nargs=1, action="store", dest="source",
+                                 help="field providing the test value")
 
         # optional...
-        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
-                                 help="path for ISO 8601 datetime output (default 'rec')")
+        self.__parser.add_option("--lower", "-l", type="float", nargs=1, action="store", dest="lower",
+                                 help="lower bound")
 
-        self.__parser.add_option("--quality", "-q", type="int", nargs=1, action="store", dest="quality",
-                                 help="minimum acceptable GPS quality")
+        self.__parser.add_option("--upper", "-u", type="float", nargs=1, action="store", dest="upper",
+                                 help="upper bound")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.position is None or self.path is None:
+        if self.target is None or self.source is None:
+            return False
+
+        if self.lower is not None and self.upper is not None and self.upper <= self.lower:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def position(self):
-        return self.__opts.position
+    def target(self):
+        return self.__opts.target
 
 
     @property
-    def lat(self):
-        return None if self.__opts.position is None else self.__opts.position[0]
+    def source(self):
+        return self.__opts.source
 
 
     @property
-    def lng(self):
-        return None if self.__opts.position is None else self.__opts.position[1]
+    def lower(self):
+        return self.__opts.lower
 
 
     @property
-    def iso(self):
-        return self.__opts.iso
-
-
-    @property
-    def quality(self):
-        return self.__opts.quality
+    def upper(self):
+        return self.__opts.upper
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
-    @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleDistance:{position:%s, iso:%s, quality:%s, verbose:%s, path:%s}" % \
-               (self.position, self.iso, self.quality, self.verbose, self.path)
+        return "CmdSampleNullify:{target:%s, source:%s, lower:%s, upper:%s, verbose:%s}" % \
+               (self.target, self.source, self.lower, self.upper, self.verbose)
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_duplicates.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_error.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_filter.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_filter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_interval.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_iso_8601.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_low_pass.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_median.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_median.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_nullify.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_device_monitor_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,97 @@
 """
-Created on 4 Sep 2019
+Created on 28 Jun 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
-
-source repo: scs_analysis
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleNullify(object):
+class CmdDeviceMonitorStatus(object):
     """unix command line handler"""
 
+    # --------------------------------------------------------------------------------------------------------------------
+
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog -t TARGET_PATH -s SOURCE_PATH [-l LOWER] [-u UPPER]"
-                                                    " [-v]", version="%prog 1.0")
-
-        # compulsory...
-        self.__parser.add_option("--target", "-t", type="string", nargs=1, action="store", dest="target",
-                                 help="field to be nullified")
-
-        self.__parser.add_option("--source", "-s", type="string", nargs=1, action="store", dest="source",
-                                 help="field providing the test value")
-
-        # optional...
-        self.__parser.add_option("--lower", "-l", type="float", nargs=1, action="store", dest="lower",
-                                 help="lower bound")
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [-t DEVICE_TAG [-x]] "
+                                                    "[-i INDENT] [-v]", version="%prog 1.0")
 
-        self.__parser.add_option("--upper", "-u", type="float", nargs=1, action="store", dest="upper",
-                                 help="upper bound")
+        # identity...
+        self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
+                                 help="the stored credentials to be presented")
+
+        # filters...
+        self.__parser.add_option("--tag-filter", "-t", type="string", action="store", dest="tag_filter",
+                                 help="the (partial) tag of the device(s)")
+
+        self.__parser.add_option("--exactly", "-x", action="store_true", dest="exact_match", default=False,
+                                 help="exact match for tag")
+
+        # output...
+        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+                                 help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.target is None or self.source is None:
-            return False
-
-        if self.lower is not None and self.upper is not None and self.upper <= self.lower:
+        if self.exact_match and self.tag_filter is None:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
+    # properties: identity...
 
     @property
-    def target(self):
-        return self.__opts.target
+    def credentials_name(self):
+        return self.__opts.credentials_name
 
 
+    # ----------------------------------------------------------------------------------------------------------------
+    # properties: filters...
+
     @property
-    def source(self):
-        return self.__opts.source
+    def tag_filter(self):
+        return self.__opts.tag_filter
 
 
     @property
-    def lower(self):
-        return self.__opts.lower
+    def exact_match(self):
+        return self.__opts.exact_match
+
 
 
+    # ----------------------------------------------------------------------------------------------------------------
+    # properties: output...
+
     @property
-    def upper(self):
-        return self.__opts.upper
+    def indent(self):
+        return self.__opts.indent
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleNullify:{target:%s, source:%s, lower:%s, upper:%s, verbose:%s}" % \
-               (self.target, self.source, self.lower, self.upper, self.verbose)
+        return "CmdDeviceMonitorStatus:{credentials_name:%s, tag_filter:%s, exact_match:%s, indent:%s, verbose:%s}" % \
+               (self.credentials_name, self.tag_filter, self.exact_match, self.indent, self.verbose)
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_paths.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_record.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_record.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_slope.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_sort.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_stats.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_subset.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_tally.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_tally.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_time_shift.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_sample_timezone.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_sample_timezone.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_single_chart.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_socket_receiver.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cmd/cmd_uds.py` & `scs-analysis-2.7.7/src/scs_analysis/cmd/cmd_uds.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cognito_devices.py` & `scs-analysis-2.7.7/src/scs_analysis/cognito_devices.py`

 * *Files 7% similar despite different names*

```diff
@@ -127,14 +127,18 @@
             # find...
             device = finder.get_by_tag(auth.id_token, cmd.update_tag)
 
             if device is None:
                 logger.error("no device found for tag: '%s'." % cmd.update)
                 exit(1)
 
+            if not CognitoDeviceIdentity.is_valid_invoice_number(cmd.update_invoice):
+                logger.error("'%s' is not a valid invoice number." % cmd.update_invoice)
+                exit(2)
+
             # update...
             updated = CognitoDeviceIdentity(cmd.update_tag, None, cmd.update_invoice, None, None)
             report = device_manager.update(auth.id_token, updated)
 
         if cmd.delete:
             device_manager.delete(auth.id_token, cmd.delete)
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cognito_password.py` & `scs-analysis-2.7.7/src/scs_analysis/cognito_user_credentials.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,180 +1,168 @@
 #!/usr/bin/env python3
 
 """
-Created on 9 Feb 2022
+Created on 22 Nov 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The cognito_password utility is used to set or reset the user's password, or to request an email to permit
-password operations. Which email message is sent depends on the state of the state of the user's account:
+The cognito_user_credentials utility is used to manage the AWS Cognito credentials for the user. The credentials are
+composed of an email address and a password.
 
-* UNCONFIRMED - the account creation email is re-sent
-* CONFIRMED - a password reset code is sent and the user account enters the PASSWORD_RESET_REQUIRED state
-* PASSWORD_RESET_REQUIRED - a password reset code is re-sent
-* FORCE_CHANGE_PASSWORD - the temporary password is re-sent
+The JSON identity document managed by this utility is encrypted, and a password must be used to retrieve the document.
+By default, the retrieval password is the same as the Cognito credentials password. However, a separate retrieval
+password can be specified (in order, for example, to standardise the retrieval password across multiple Cognito
+credentials.
 
-Emails cannot be sent to users in the DISABLED state.
+The password must be specified when the credentials are created and is required when the credentials are accessed.
 
 SYNOPSIS
-cognito_password.py { -e | -s | -r } EMAIL [-v]
+cognito_user_credentials.py [{ -l | [-c CREDENTIALS] [{ -s | -t | -d }] }] [-v]
 
 EXAMPLES
-./cognito_password.py -r someone@me.com
+./cognito_user_credentials.py -s
+
+FILES
+~/SCS/aws/cognito_user_credentials.json
+
+DOCUMENT EXAMPLE
+{"email": "production@southcoastscience.com", "password": "###", "retrieval-password": "###"}
 
 SEE ALSO
-scs_analysis/cognito_user_credentials
-scs_analysis/cognito_user_identity
-scs_analysis/cognito_users
+scs_analysis/cognito_identity
+
+RESOURCES
+https://stackoverflow.com/questions/42568262/how-to-encrypt-text-with-a-password-in-python
 """
 
 import requests
 import sys
 
-from scs_analysis.cmd.cmd_cognito_password import CmdCognitoPassword
+from scs_analysis.cmd.cmd_cognito_user_credentials import CmdCognitoUserCredentials
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
-from scs_core.aws.security.cognito_login_manager import CognitoLoginManager, AuthenticationStatus
-from scs_core.aws.security.cognito_password_manager import CognitoPasswordManager
+from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 from scs_core.aws.security.cognito_user import CognitoUserIdentity
 
-from scs_core.client.http_exception import HTTPException, HTTPBadRequestException, HTTPUnauthorizedException, \
-    HTTPNotFoundException, HTTPNotAllowedException
+from scs_core.client.http_exception import HTTPException
 
 from scs_core.data.datum import Datum
-
+from scs_core.data.json import JSONify
 
 from scs_core.sys.logging import Logging
 
-from scs_host.comms.stdio import StdIO
+from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-def do_password(do_set):
-    new_password = StdIO.prompt("Enter new password")
-
-    if not CognitoUserIdentity.is_valid_password(new_password):
-        logger.error("The password must include lower and upper case, numeric and punctuation characters.")
-        exit(1)
-
+def load_credentials(credentials_name):
     try:
-        if do_set:
-            manager.do_set_password(cmd.email, new_password, auth.content.session)
-        else:
-            manager.do_reset_password(cmd.email, code, new_password)
+        password = CognitoClientCredentials.password_from_user()
+        return CognitoClientCredentials.load(Host, name=credentials_name, encryption_key=password)
 
-    except HTTPNotFoundException:
-        logger.error("no user could be found for email '%s'." % cmd.email)
+    except (KeyError, ValueError):
+        logger.error("incorrect password.")
         exit(1)
 
-    except HTTPUnauthorizedException:
-        logger.error("the user '%s' is disabled." % cmd.email)
-        exit(1)
-
-    except HTTPNotAllowedException:
-        alternative = '--reset-password' if do_set else '--set-password'
-        logger.error("the operation is not permitted in the current user state. Try %s?" % alternative)
-        exit(1)
-
-    except HTTPBadRequestException as error:
-        if error.data == "Mismatch":
-            logger.error("the code '%s' is not valid." % code)
-            exit(1)
-
-        if error.data == "Expired":
-            logger.error("the code has expired.")
-            exit(1)
-
-        logger.error(repr(ex))
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
     credentials = None
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
-        cmd = CmdCognitoPassword()
+        cmd = CmdCognitoUserCredentials()
 
         if not cmd.is_valid():
             cmd.print_help(sys.stderr)
             exit(2)
 
-        Logging.config('cognito_password', verbose=cmd.verbose)
+        Logging.config('cognito_user_credentials', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
 
         # ------------------------------------------------------------------------------------------------------------
-        # resources...
+        # run...
 
-        manager = CognitoPasswordManager(requests)
-        gatekeeper = CognitoLoginManager(requests)
+        if cmd.list:
+            for conf_name in sorted(CognitoClientCredentials.list(Host)):
+                print(conf_name, file=sys.stderr)
+            exit(0)
 
+        elif cmd.set:
+            credentials = CognitoClientCredentials.from_user(cmd.credentials_name)
 
-        # ------------------------------------------------------------------------------------------------------------
-        # validation...
+            if not Datum.is_email_address(credentials.email):
+                logger.error("The email address is not valid.")
+                exit(1)
+
+            if not CognitoUserIdentity.is_valid_password(credentials.password):
+                logger.error("The password must include lower and upper case, numeric and punctuation characters.")
+                exit(1)
 
-        if not Datum.is_email_address(cmd.email):
-            logger.error("The email address is not valid.")
-            exit(1)
+            credentials.save(Host, encryption_key=credentials.retrieval_password)
 
+        elif cmd.update_password:
+            credentials = load_credentials(cmd.credentials_name)
 
-        # ------------------------------------------------------------------------------------------------------------
-        # run...
+            if credentials is None:
+                logger.error("credentials not found.")
+                exit(1)
 
-        if cmd.send_email:
-            try:
-                manager.send_email(cmd.email)
-                logger.error("an email has been sent.")
-                exit(0)
+            credentials = CognitoClientCredentials.from_user(cmd.credentials_name, existing_email=credentials.email)
 
-            except HTTPUnauthorizedException:
-                logger.error("the user '%s' is disabled." % cmd.email)
+            if not Datum.is_email_address(credentials.email):
+                logger.error("The email address is not valid.")
                 exit(1)
 
-            except HTTPNotFoundException:
-                logger.error("no user could be found for email '%s'." % cmd.email)
+            if not CognitoUserIdentity.is_valid_password(credentials.password):
+                logger.error("The password must include lower and upper case, numeric and punctuation characters.")
                 exit(1)
 
-        if cmd.set_password:
-            temporary_password = StdIO.prompt("Enter temporary password")
+            credentials.save(Host, encryption_key=credentials.retrieval_password)
 
-            # login
-            credentials = CognitoClientCredentials(None, cmd.email, temporary_password, None)
-            auth = gatekeeper.user_login(credentials)
+        elif cmd.test:
+            gatekeeper = CognitoLoginManager(requests)
 
-            if auth.authentication_status != AuthenticationStatus.Challenge:
-                logger.error(auth.authentication_status.description)
+            credentials = load_credentials(cmd.credentials_name)
+
+            if credentials is None:
+                logger.error("no credentials are available")
                 exit(1)
 
-            do_password(True)
-            logger.error("the password has been set.")
-            exit(0)
+            logger.info(credentials)
 
-        if cmd.reset_password:
-            code = StdIO.prompt("Enter verification code")
+            result = gatekeeper.user_login(credentials)
+            logger.error(result.authentication_status.description)
 
-            do_password(False)
-            logger.error("the password has been reset.")
-            exit(0)
+            exit(0 if result.is_ok() else 1)
+
+        elif cmd.delete:
+            CognitoClientCredentials.delete(Host)
+
+        else:
+            credentials = load_credentials(cmd.credentials_name)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
+        if credentials:
+            print(JSONify.dumps(credentials))
+
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPException as ex:
         logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cognito_user_identity.py` & `scs-analysis-2.7.7/src/scs_analysis/cognito_user_identity.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,32 +131,32 @@
                 exit(1)
 
             if not CognitoUserIdentity.is_valid_password(password):
                 logger.error("The password must include lower and upper case, numeric and punctuation characters.")
                 exit(1)
 
             # save identity...
-            report = CognitoUserIdentity(email, None, None, True, False, email,
-                                         given_name, family_name, password, False, False, False, None)
+            identity = CognitoUserIdentity(None, None, None, True, False, email,
+                                           given_name, family_name, password, False, False, False, None)
 
             manager = CognitoUserCreator(requests)
-            report = manager.create(report)
+            report = manager.create(identity)
 
             # create credentials...
             credentials = CognitoClientCredentials(cmd.credentials_name, email, password, retrieval_password)
             credentials.save(Host, encryption_key=retrieval_password)
 
         if cmd.update:
             # find...
             identity = finder.get_self(auth.id_token)
 
             # update identity...
             given_name = StdIO.prompt("Enter given name", default=identity.given_name)
             family_name = StdIO.prompt("Enter family name", default=identity.family_name)
-            email = StdIO.prompt("Enter email", default=identity.email)
+            email = StdIO.prompt("Enter email address", default=identity.email)
             password = StdIO.prompt("Enter password (RETURN to keep existing)")
 
             if not password:
                 password = credentials.password
 
             if credentials.retrieval_password == credentials.password:
                 retrieval_password = StdIO.prompt("Enter retrieval password (RETURN for same)")
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/cognito_users.py` & `scs-analysis-2.7.7/src/scs_analysis/cognito_users.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 cognito_users.py  [-c CREDENTIALS] { -F [{ -e EMAIL_ADDR | -l ORG_LABEL | -c CONFIRMATION | -s { 1 | 0 } } }] | \
 -C | -U -e EMAIL_ADDR | -D -e EMAIL_ADDR } [-i INDENT] [-v]
 
 EXAMPLES
 cognito_users.py -Fe bruno.beloff@southcoastscience.com
 
 DOCUMENT EXAMPLE
-{"username": "8", "creation-date": "2021-11-24T12:51:12Z", "confirmation-status": "CONFIRMED", "enabled": true,
-"email": "bruno.beloff@southcoastscience.com", "given-name": "Bruno", "family-name": "Beloff", "is-super": true}
+{"username": "506cd055-1978-4984-9f17-2fad77797fa1", "email": "bruno.beloff@southcoastscience.com",
+"given-name": "Bruno", "family-name": "Beloff", "confirmation-status": "CONFIRMED", "enabled": true,
+"email-verified": true, "is-super": false, "is-tester": false, "is-financial": false,
+"created": "2023-04-20T11:45:21Z", "last-updated": "2023-06-26T14:39:17Z"}
 
 SEE ALSO
 scs_analysis/cognito_credentials
 scs_analysis/cognito_devices
 scs_analysis/organisation_users
 
 RESOURCES
@@ -161,16 +163,15 @@
             password = StdIO.prompt("Enter password")       # TODO: don't set password - use FORCE CHANGE
 
             if not CognitoUserIdentity.is_valid_password(password):
                 logger.error("The password '%s' is not valid." % password)
                 exit(1)
 
             identity = CognitoUserIdentity(None, None, None, True, False, cmd.email,
-                                           cmd.given_name, cmd.family_name, password, False, False,
-                                           False, None)
+                                           cmd.given_name, cmd.family_name, password, False, False, False, None)
 
             manager = CognitoUserCreator(requests)
             report = manager.create(identity)
 
         if cmd.update:
             # find...
             identity = finder.get_by_email(auth.id_token, cmd.update)
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/configuration_csv.py` & `scs-analysis-2.7.7/src/scs_analysis/configuration_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 be included in the CSV file)
 
 For diff-histories and full-histories modes, a single rec value is included, equivalent to rec.update.
 
 Output CSV cell values are always wrapped in quotes ('"').
 
 SYNOPSIS
-configuration_csv.py { -n | -s | -l OUTPUT_CSV | { -d | -f } [-o OUTPUT_CSV_DIR] } [-t DEVICE_TAG [-e]] [-v]
-[NODE_1..NODE_N]
+configuration_csv.py [-c CREDENTIALS] { -n | -s | -l OUTPUT_CSV | { -d | -f } [-o OUTPUT_CSV_DIR] }
+[-t DEVICE_TAG [-x]] [-v] [NODE_1..NODE_N]
 
 EXAMPLES
 configuration_csv.py -vs configs.csv
 configuration_csv.py -vdo afe_ids afe-id
 configuration_csv.py -vft scs-bgx-431
 
 SEE ALSO
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/configuration_monitor.py` & `scs-analysis-2.7.7/src/scs_analysis/configuration_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 DESCRIPTION
 The configuration_monitor utility is used to retrieve configuration information relating to one or more devices.
 Flags enable the selection of either the latest recorded configuration for the device(s), or a history of
 configuration changes. In the case of historical reports, either all the field values can be returned, or
 only those that changed from the previous recording.
 
 SYNOPSIS
-configuration_monitor.py [-t TAG [-e]] { -l | -f | -d | -o } [-i INDENT] [-v]
+configuration_monitor.py [-c CREDENTIALS] [-t TAG [-x]] { -l | -f | -d | -o } [-i INDENT] [-v]
 
 EXAMPLES
 configuration_monitor.py -t scs-bgx-401 -d | node.py -s | csv_writer.py -s
 
 SEE ALSO
 scs_analysis/configuration_csv
 scs_analysis/configuration_monitor_check
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/configuration_monitor_check.py` & `scs-analysis-2.7.7/src/scs_analysis/configuration_monitor_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 * NSP - NOT SUPPORTED
 * R - RECEIVED:
 * RNW - RECEIVED:NEW
 * RUN - RECEIVED:UNCHANGED
 * RUP - RECEIVED:UPDATED
 
 SYNOPSIS
-configuration_monitor_check.py { -c TAG | [-t TAG [-e]] [-r RESULT] [-o] } [-i INDENT] [-v]
+configuration_monitor_check.py [-c CREDENTIALS] { -f TAG | [-t TAG [-x]] [-o] } [-i INDENT] [-v]
 
 EXAMPLES
 configuration_monitor_check.py -r ERR | node.py -s | csv_writer.py
 
 DOCUMENT EXAMPLE
 {"tag": "scs-ph1-26", "rec": "2021-05-18T14:36:00Z", "result": "ERROR",
 "context": ["TimeoutExpired(['./configuration'], 30)"]}
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis/csv_collation_summary.py` & `scs-analysis-2.7.7/src/scs_analysis/csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/csv_collator.py` & `scs-analysis-2.7.7/src/scs_analysis/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/csv_join.py` & `scs-analysis-2.7.7/src/scs_analysis/csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/csv_reader.py` & `scs-analysis-2.7.7/src/scs_analysis/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/csv_segmentor.py` & `scs-analysis-2.7.7/src/scs_analysis/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/csv_writer.py` & `scs-analysis-2.7.7/src/scs_analysis/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/device_controller.py` & `scs-analysis-2.7.7/src/scs_analysis/device_controller.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/handler/aws_mqtt_publisher.py` & `scs-analysis-2.7.7/src/scs_analysis/handler/aws_mqtt_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/handler/aws_mqtt_subscription_handler.py` & `scs-analysis-2.7.7/src/scs_analysis/handler/aws_mqtt_subscription_handler.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/handler/batch_download_reporter.py` & `scs-analysis-2.7.7/src/scs_analysis/handler/batch_download_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/handler/configuration_csv_generator.py` & `scs-analysis-2.7.7/src/scs_analysis/handler/configuration_csv_generator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/handler/csv_collator.py` & `scs-analysis-2.7.7/src/scs_analysis/handler/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/handler/csv_segmentor.py` & `scs-analysis-2.7.7/src/scs_analysis/handler/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/handler/mqtt_reporter.py` & `scs-analysis-2.7.7/src/scs_analysis/handler/mqtt_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/handler/sample_midpoint.py` & `scs-analysis-2.7.7/src/scs_analysis/handler/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/handler/sample_regression.py` & `scs-analysis-2.7.7/src/scs_analysis/handler/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/histo_chart.py` & `scs-analysis-2.7.7/src/scs_analysis/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/localised_datetime.py` & `scs-analysis-2.7.7/src/scs_analysis/localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/monitor_auth.py` & `scs-analysis-2.7.7/src/scs_analysis/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/multi_chart.py` & `scs-analysis-2.7.7/src/scs_analysis/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/node.py` & `scs-analysis-2.7.7/src/scs_analysis/node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/organisation_devices.py` & `scs-analysis-2.7.7/src/scs_analysis/organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/organisation_path_roots.py` & `scs-analysis-2.7.7/src/scs_analysis/organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/organisation_user_paths.py` & `scs-analysis-2.7.7/src/scs_analysis/organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/organisation_users.py` & `scs-analysis-2.7.7/src/scs_analysis/organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/organisations.py` & `scs-analysis-2.7.7/src/scs_analysis/organisations.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_aggregate.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_average.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_average.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_collator.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_concentration.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_concentration.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_distance.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_duplicates.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_error.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_interval.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_iso_8601.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_low_pass.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_max.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_max.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_median.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_median.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_midpoint.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_min.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_min.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_noise.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_noise.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_nullify.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_paths.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_regression.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_slope.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_sort.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_stats.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_subset.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_time_shift.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/sample_timezone.py` & `scs-analysis-2.7.7/src/scs_analysis/sample_timezone.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/single_chart.py` & `scs-analysis-2.7.7/src/scs_analysis/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/socket_receiver.py` & `scs-analysis-2.7.7/src/scs_analysis/socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/timer.py` & `scs-analysis-2.7.7/src/scs_analysis/timer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis/uds_receiver.py` & `scs-analysis-2.7.7/src/scs_analysis/uds_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.6/src/scs_analysis.egg-info/PKG-INFO` & `scs-analysis-2.7.7/src/scs_analysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 2.7.6
+Version: 2.7.7
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `scs-analysis-2.7.6/src/scs_analysis.egg-info/SOURCES.txt` & `scs-analysis-2.7.7/src/scs_analysis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 src/scs_analysis/aws_mqtt_client.py
 src/scs_analysis/aws_topic_history.py
 src/scs_analysis/aws_topic_publisher.py
 src/scs_analysis/aws_upload_interval.py
 src/scs_analysis/baseline.py
 src/scs_analysis/baseline_conf.py
 src/scs_analysis/cognito_devices.py
-src/scs_analysis/cognito_password.py
+src/scs_analysis/cognito_email.py
 src/scs_analysis/cognito_user_credentials.py
 src/scs_analysis/cognito_user_identity.py
 src/scs_analysis/cognito_users.py
 src/scs_analysis/configuration_csv.py
 src/scs_analysis/configuration_monitor.py
 src/scs_analysis/configuration_monitor_check.py
 src/scs_analysis/csv_collation_summary.py
 src/scs_analysis/csv_collator.py
 src/scs_analysis/csv_join.py
 src/scs_analysis/csv_reader.py
 src/scs_analysis/csv_segmentor.py
 src/scs_analysis/csv_writer.py
 src/scs_analysis/device_controller.py
+src/scs_analysis/device_monitor.py
+src/scs_analysis/device_monitor_status.py
 src/scs_analysis/histo_chart.py
 src/scs_analysis/localised_datetime.py
 src/scs_analysis/monitor_auth.py
 src/scs_analysis/multi_chart.py
 src/scs_analysis/node.py
 src/scs_analysis/organisation_devices.py
 src/scs_analysis/organisation_path_roots.py
@@ -88,28 +90,30 @@
 src/scs_analysis/cmd/cmd_aws_byline.py
 src/scs_analysis/cmd/cmd_aws_client_auth.py
 src/scs_analysis/cmd/cmd_aws_topic_history.py
 src/scs_analysis/cmd/cmd_aws_topic_publisher.py
 src/scs_analysis/cmd/cmd_baseline.py
 src/scs_analysis/cmd/cmd_baseline_conf.py
 src/scs_analysis/cmd/cmd_cognito_devices.py
-src/scs_analysis/cmd/cmd_cognito_password.py
+src/scs_analysis/cmd/cmd_cognito_email.py
 src/scs_analysis/cmd/cmd_cognito_user_credentials.py
 src/scs_analysis/cmd/cmd_cognito_user_identity.py
 src/scs_analysis/cmd/cmd_cognito_users.py
 src/scs_analysis/cmd/cmd_configuration_csv.py
 src/scs_analysis/cmd/cmd_configuration_monitor.py
 src/scs_analysis/cmd/cmd_configuration_monitor_check.py
 src/scs_analysis/cmd/cmd_csv_collation_summary.py
 src/scs_analysis/cmd/cmd_csv_collator.py
 src/scs_analysis/cmd/cmd_csv_join.py
 src/scs_analysis/cmd/cmd_csv_reader.py
 src/scs_analysis/cmd/cmd_csv_segmentor.py
 src/scs_analysis/cmd/cmd_csv_writer.py
 src/scs_analysis/cmd/cmd_device_controller.py
+src/scs_analysis/cmd/cmd_device_monitor.py
+src/scs_analysis/cmd/cmd_device_monitor_status.py
 src/scs_analysis/cmd/cmd_histo_chart.py
 src/scs_analysis/cmd/cmd_localised_datetime.py
 src/scs_analysis/cmd/cmd_monitor_auth.py
 src/scs_analysis/cmd/cmd_mqtt_client.py
 src/scs_analysis/cmd/cmd_multi_chart.py
 src/scs_analysis/cmd/cmd_node.py
 src/scs_analysis/cmd/cmd_organisation_devices.py
```

