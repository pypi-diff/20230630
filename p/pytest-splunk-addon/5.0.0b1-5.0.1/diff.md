# Comparing `tmp/pytest_splunk_addon-5.0.0b1.tar.gz` & `tmp/pytest_splunk_addon-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_splunk_addon-5.0.0b1.tar", max compression
+gzip compressed data, was "pytest_splunk_addon-5.0.1.tar", max compression
```

## Comparing `pytest_splunk_addon-5.0.0b1.tar` & `pytest_splunk_addon-5.0.1.tar`

### file list

```diff
@@ -1,87 +1,86 @@
--rw-r--r--   0        0        0    11341 2023-02-16 15:50:10.748575 pytest_splunk_addon-5.0.0b1/LICENSE
--rw-r--r--   0        0        0     2441 2023-02-16 15:51:08.021085 pytest_splunk_addon-5.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     1847 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/.ignore_splunk_internal_errors
--rw-r--r--   0        0        0      747 2023-02-16 15:51:08.017085 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/__init__.py
--rw-r--r--   0        0        0     7547 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/plugin.py
--rw-r--r--   0        0        0    31497 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/splunk.py
--rw-r--r--   0        0        0      575 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py
--rw-r--r--   0        0        0    46777 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py
--rw-r--r--   0        0        0     1216 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/__init__.py
--rw-r--r--   0        0        0     2787 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_basic.py
--rw-r--r--   0        0        0     3308 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py
--rw-r--r--   0        0        0     2078 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py
--rw-r--r--   0        0        0     3132 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/fields.py
--rw-r--r--   0        0        0    13280 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py
--rw-r--r--   0        0        0     2756 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py
--rw-r--r--   0        0        0     2443 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py
--rw-r--r--   0        0        0     5387 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py
--rw-r--r--   0        0        0     6164 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/app_test_generator.py
--rw-r--r--   0        0        0      750 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py
--rw-r--r--   0        0        0     1247 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py
--rw-r--r--   0        0        0     1126 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py
--rw-r--r--   0        0        0     9582 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py
--rw-r--r--   0        0        0     2347 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py
--rw-r--r--   0        0        0     2797 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py
--rw-r--r--   0        0        0     2438 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py
--rw-r--r--   0        0        0     3553 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json
--rw-r--r--   0        0        0     3699 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json
--rw-r--r--   0        0        0      966 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py
--rw-r--r--   0        0        0     2020 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py
--rw-r--r--   0        0        0     2382 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py
--rw-r--r--   0        0        0     3933 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py
--rw-r--r--   0        0        0     3263 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py
--rw-r--r--   0        0        0     4222 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py
--rw-r--r--   0        0        0     9214 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py
--rw-r--r--   0        0        0     2961 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py
--rw-r--r--   0        0        0    11200 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py
--rw-r--r--   0        0        0    20764 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py
--rw-r--r--   0        0        0     2390 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Alerts.json
--rw-r--r--   0        0        0     5281 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Authentication.json
--rw-r--r--   0        0        0     9626 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Certificates.json
--rw-r--r--   0        0        0     8173 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Change.json
--rw-r--r--   0        0        0     2814 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/DLP.json
--rw-r--r--   0        0        0     8598 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Email.json
--rw-r--r--   0        0        0    18855 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json
--rw-r--r--   0        0        0     9400 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json
--rw-r--r--   0        0        0     4255 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Malware.json
--rw-r--r--   0        0        0     6608 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json
--rw-r--r--   0        0        0     5599 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json
--rw-r--r--   0        0        0    17483 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json
--rw-r--r--   0        0        0     3862 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Updates.json
--rw-r--r--   0        0        0     5184 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json
--rw-r--r--   0        0        0     7178 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Web.json
--rw-r--r--   0        0        0      885 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py
--rw-r--r--   0        0        0      858 2023-02-16 15:50:10.752575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py
--rw-r--r--   0        0        0     7335 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py
--rw-r--r--   0        0        0     4998 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py
--rw-r--r--   0        0        0     4414 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py
--rw-r--r--   0        0        0     4991 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py
--rw-r--r--   0        0        0     3611 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py
--rw-r--r--   0        0        0     3011 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py
--rw-r--r--   0        0        0      808 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py
--rw-r--r--   0        0        0     3301 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py
--rw-r--r--   0        0        0     5416 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py
--rw-r--r--   0        0        0    11033 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py
--rw-r--r--   0        0        0    10356 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py
--rw-r--r--   0        0        0    21980 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py
--rw-r--r--   0        0        0      762 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/index_tests/__init__.py
--rw-r--r--   0        0        0      707 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py
--rw-r--r--   0        0        0    11983 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py
--rw-r--r--   0        0        0    11453 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py
--rw-r--r--   0        0        0      905 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py
--rw-r--r--   0        0        0     7287 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py
--rw-r--r--   0        0        0    46396 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/rule.py
--rw-r--r--   0        0        0    15409 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py
--rw-r--r--   0        0        0     2286 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py
--rw-r--r--   0        0        0    16788 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py
--rw-r--r--   0        0        0     6028 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py
--rw-r--r--   0        0        0     9990 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd
--rw-r--r--   0        0        0     6213 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py
--rw-r--r--   0        0        0      830 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/utilities/__init__.py
--rw-r--r--   0        0        0     4630 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py
--rw-r--r--   0        0        0     1623 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/utilities/log_helper.py
--rw-r--r--   0        0        0     3030 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py
--rw-r--r--   0        0        0     3410 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py
--rw-r--r--   0        0        0    17581 2023-02-16 15:50:10.756575 pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/tools/cim_field_report.py
--rw-r--r--   0        0        0     2244 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.0.0b1/setup.py
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-06-30 14:54:54.450121 pytest_splunk_addon-5.0.1/LICENSE
+-rw-r--r--   0        0        0     2457 2023-06-30 14:55:31.474431 pytest_splunk_addon-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1847 2023-06-30 14:54:54.454121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/.ignore_splunk_internal_errors
+-rw-r--r--   0        0        0      740 2023-06-30 14:55:31.474431 pytest_splunk_addon-5.0.1/pytest_splunk_addon/__init__.py
+-rw-r--r--   0        0        0     7547 2023-06-30 14:54:54.454121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/plugin.py
+-rw-r--r--   0        0        0    31497 2023-06-30 14:54:54.454121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/splunk.py
+-rw-r--r--   0        0        0      575 2023-06-30 14:54:54.454121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py
+-rw-r--r--   0        0        0    46777 2023-06-30 14:54:54.454121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py
+-rw-r--r--   0        0        0     1216 2023-06-30 14:54:54.454121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/__init__.py
+-rw-r--r--   0        0        0     2787 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_basic.py
+-rw-r--r--   0        0        0     3308 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py
+-rw-r--r--   0        0        0     2078 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py
+-rw-r--r--   0        0        0     3132 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/fields.py
+-rw-r--r--   0        0        0    13280 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py
+-rw-r--r--   0        0        0     2756 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py
+-rw-r--r--   0        0        0     2443 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py
+-rw-r--r--   0        0        0     5387 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py
+-rw-r--r--   0        0        0     6164 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/app_test_generator.py
+-rw-r--r--   0        0        0      750 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py
+-rw-r--r--   0        0        0     1247 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py
+-rw-r--r--   0        0        0     1126 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py
+-rw-r--r--   0        0        0     9582 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py
+-rw-r--r--   0        0        0     2347 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py
+-rw-r--r--   0        0        0     2797 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py
+-rw-r--r--   0        0        0     2438 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py
+-rw-r--r--   0        0        0     3553 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json
+-rw-r--r--   0        0        0     3699 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json
+-rw-r--r--   0        0        0      966 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py
+-rw-r--r--   0        0        0     2020 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py
+-rw-r--r--   0        0        0     2382 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py
+-rw-r--r--   0        0        0     3933 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py
+-rw-r--r--   0        0        0     3263 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py
+-rw-r--r--   0        0        0     4222 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py
+-rw-r--r--   0        0        0     9214 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py
+-rw-r--r--   0        0        0     2961 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py
+-rw-r--r--   0        0        0    11200 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py
+-rw-r--r--   0        0        0    20764 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py
+-rw-r--r--   0        0        0     2390 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Alerts.json
+-rw-r--r--   0        0        0     5281 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Authentication.json
+-rw-r--r--   0        0        0     9626 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Certificates.json
+-rw-r--r--   0        0        0     8173 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Change.json
+-rw-r--r--   0        0        0     2814 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/DLP.json
+-rw-r--r--   0        0        0     8598 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Email.json
+-rw-r--r--   0        0        0    18855 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json
+-rw-r--r--   0        0        0     9400 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json
+-rw-r--r--   0        0        0     4255 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Malware.json
+-rw-r--r--   0        0        0     6608 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json
+-rw-r--r--   0        0        0     5599 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json
+-rw-r--r--   0        0        0    17483 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json
+-rw-r--r--   0        0        0     3862 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Updates.json
+-rw-r--r--   0        0        0     5184 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json
+-rw-r--r--   0        0        0     7178 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Web.json
+-rw-r--r--   0        0        0      885 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py
+-rw-r--r--   0        0        0      858 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py
+-rw-r--r--   0        0        0     7335 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py
+-rw-r--r--   0        0        0     4998 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py
+-rw-r--r--   0        0        0     4414 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py
+-rw-r--r--   0        0        0     4991 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py
+-rw-r--r--   0        0        0     3611 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py
+-rw-r--r--   0        0        0     3011 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py
+-rw-r--r--   0        0        0      808 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py
+-rw-r--r--   0        0        0     3301 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py
+-rw-r--r--   0        0        0     5416 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py
+-rw-r--r--   0        0        0    11033 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py
+-rw-r--r--   0        0        0    10356 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py
+-rw-r--r--   0        0        0    21980 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py
+-rw-r--r--   0        0        0      762 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/index_tests/__init__.py
+-rw-r--r--   0        0        0      707 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py
+-rw-r--r--   0        0        0    11983 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py
+-rw-r--r--   0        0        0    11453 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py
+-rw-r--r--   0        0        0      905 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py
+-rw-r--r--   0        0        0     7287 2023-06-30 14:54:54.458121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py
+-rw-r--r--   0        0        0    46396 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/rule.py
+-rw-r--r--   0        0        0    15409 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py
+-rw-r--r--   0        0        0     2286 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py
+-rw-r--r--   0        0        0    16788 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py
+-rw-r--r--   0        0        0     6028 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py
+-rw-r--r--   0        0        0     9990 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd
+-rw-r--r--   0        0        0     6213 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py
+-rw-r--r--   0        0        0      830 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/utilities/__init__.py
+-rw-r--r--   0        0        0     4630 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py
+-rw-r--r--   0        0        0     1623 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/utilities/log_helper.py
+-rw-r--r--   0        0        0     3030 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py
+-rw-r--r--   0        0        0     3410 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py
+-rw-r--r--   0        0        0    17581 2023-06-30 14:54:54.462121 pytest_splunk_addon-5.0.1/pytest_splunk_addon/tools/cim_field_report.py
+-rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.0.1/PKG-INFO
```

### Comparing `pytest_splunk_addon-5.0.0b1/LICENSE` & `pytest_splunk_addon-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pyproject.toml` & `pytest_splunk_addon-5.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 [tool.poetry]
 name = "pytest-splunk-addon"
-version = "5.0.0-beta.1"
+version = "5.0.1"
 description = "A Dynamic test tool for Splunk Apps and Add-ons"
 authors = ["Splunk <addonfactory@splunk.com>"]
 license = "APACHE-2.0"
 classifiers = [
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Testing",
@@ -29,29 +29,30 @@
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License",
 ]
 include = ["pytest_splunk_addon/**/*.json", "pytest_splunk_addon/**/*.txt"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pytest = ">5.4.0,<7.3"
+pytest = ">5.4.0,<8"
 splunk-sdk = "^1.6"
-requests = "^2"
+requests = "^2.31.0"
 jsonschema = "^4.2.1"
 pytest-xdist = ">=2.3.0"
 filelock = "^3.0"
 pytest-ordering = "~0.6"
 lovely-pytest-docker = { version="^0", optional = true }
 junitparser = "^2.2.0"
 addonfactory-splunk-conf-parser-lib = "^0.3.3"
 defusedxml = "^0.7.1"
-Faker = "^13.12.0"
+Faker = ">=13.12,<18.0"
 xmltodict = "^0.13.0"
 xmlschema = "^1.11.3"
 splunksplwrapper = "^1.0.1"
+urllib3 = "<2"
 
 [tool.poetry.extras]
 docker = ['lovely-pytest-docker']
 
 [tool.poetry.group.dev.dependencies]
 lovely-pytest-docker = "~0.3.0"
 pytest-cov = "^3.0.0"
```

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/.ignore_splunk_internal_errors` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/.ignore_splunk_internal_errors`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/__init__.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,13 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# -*- coding: utf-8 -*-
-"""Top-level package for splunk-app-test-lib."""
-
-__author__ = """Splunk Inc."""
-__email__ = "addonfactory@splunk.com"
-__version__ = "5.0.0-beta.1"
```

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/plugin.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/splunk.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/splunk.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/utilities/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,7 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+# -*- coding: utf-8 -*-
+"""
+There are 2 utilities included:
+
+1. CIM Compliance report generator for pytest-splunk-addon
+2. pytest-splunk-addon-data.conf generator
+
+"""
+
+from .junit_parser import JunitParser
+from .xml_event_parser import escape_char_event
```

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/__init__.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_basic.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_basic.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/fields.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/fields.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/app_test_generator.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/app_test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Alerts.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Alerts.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Authentication.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Authentication.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Certificates.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Certificates.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Change.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Change.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/DLP.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/DLP.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Email.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Email.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Malware.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Malware.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Updates.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Updates.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/data_models/Web.json` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/data_models/Web.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/index_tests/__init__.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/index_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/rule.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/rule.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/utilities/log_helper.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/utilities/log_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/pytest_splunk_addon/tools/cim_field_report.py` & `pytest_splunk_addon-5.0.1/pytest_splunk_addon/tools/cim_field_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.0.0b1/PKG-INFO` & `pytest_splunk_addon-5.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-splunk-addon
-Version: 5.0.0b1
+Version: 5.0.1
 Summary: A Dynamic test tool for Splunk Apps and Add-ons
 License: Apache-2.0
 Author: Splunk
 Author-email: addonfactory@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -13,25 +13,25 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: docker
-Requires-Dist: Faker (>=13.12.0,<14.0.0)
+Requires-Dist: Faker (>=13.12,<18.0)
 Requires-Dist: addonfactory-splunk-conf-parser-lib (>=0.3.3,<0.4.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: filelock (>=3.0,<4.0)
 Requires-Dist: jsonschema (>=4.2.1,<5.0.0)
 Requires-Dist: junitparser (>=2.2.0,<3.0.0)
 Requires-Dist: lovely-pytest-docker (>=0,<1) ; extra == "docker"
-Requires-Dist: pytest (>5.4.0,<7.3)
+Requires-Dist: pytest (>5.4.0,<8)
 Requires-Dist: pytest-ordering (>=0.6,<0.7)
 Requires-Dist: pytest-xdist (>=2.3.0)
-Requires-Dist: requests (>=2,<3)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: splunk-sdk (>=1.6,<2.0)
 Requires-Dist: splunksplwrapper (>=1.0.1,<2.0.0)
+Requires-Dist: urllib3 (<2)
 Requires-Dist: xmlschema (>=1.11.3,<2.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
```

