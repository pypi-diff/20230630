# Comparing `tmp/cdisc-rules-engine-0.6.1.tar.gz` & `tmp/cdisc-rules-engine-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdisc-rules-engine-0.6.1.tar", last modified: Wed May  3 15:21:02 2023, max compression
+gzip compressed data, was "cdisc-rules-engine-0.6.2.tar", last modified: Fri Jun 30 17:24:58 2023, max compression
```

## Comparing `cdisc-rules-engine-0.6.1.tar` & `cdisc-rules-engine-0.6.2.tar`

### file list

```diff
@@ -1,218 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.406731 cdisc-rules-engine-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14452 2023-05-03 15:21:02.406731 cdisc-rules-engine-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.354732 cdisc-rules-engine-0.6.1/TestRule/
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/TestRule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.354732 cdisc-rules-engine-0.6.1/cdisc_rule_tester/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rule_tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.354732 cdisc-rules-engine-0.6.1/cdisc_rule_tester/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rule_tester/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rule_tester/models/rule_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.354732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.358732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/config/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.362732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/constants/cache_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/constants/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/constants/define_xml_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/constants/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/constants/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/constants/permissibility.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/constants/rule_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.362732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/base_dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/content_metadata_dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/contents_dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/dataset_builder_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/define_item_group_dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/define_variables_dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/domain_list_dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/variables_metadata_dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/variables_metadata_with_define_dataset_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.366732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dummy_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dummy_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dummy_models/dummy_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/dummy_models/dummy_variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.370731 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/base_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/default_file_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/define_xml_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/execution_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/library_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/optional_condition_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/progress_parameter_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/report_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/rule_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/variable_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.370731 cdisc-rules-engine-0.6.1/cdisc_rules_engine/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/exceptions/custom_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.374732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/cache_service_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/condition_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/config_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/data_reader_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/data_service_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/dictionary_term_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/factory_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/logger_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/representation_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/terms_factory_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.374732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/base_validation_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dataset_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dataset_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dataset_variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.374732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/define/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/define/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/define/value_level_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.374732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/abstract_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/dictionary_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/get_dictionary_terms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.374732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/meddra/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/meddra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/meddra/meddra_file_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/meddra/meddra_terms_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/meddra/meddra_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.374732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/meddra/terms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/meddra/terms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/meddra/terms/meddra_term.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/meddra/terms/term_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.374732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/atc_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/atc_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/base_whodrug_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/drug_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_file_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_record_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_terms_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_variable_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/failed_validation_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/operation_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/record_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.378732 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_conditions/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_conditions/allowed_conditions_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_conditions/condition_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_conditions/condition_composite_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_conditions/not_condition_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_conditions/single_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_validation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/validation_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/validation_error_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/validation_error_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/variable_metadata_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.394731 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/base_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/dataset_column_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/day_data_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/distinct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/domain_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/expected_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/extract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/library_column_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/library_model_column_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/max_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/maximum.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/meddra_code_references_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/meddra_code_term_pairs_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/meddra_term_references_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/min_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/operations_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/parent_library_model_column_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/permissible_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/record_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/required_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/study_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/valid_codelist_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/variable_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/variable_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/variable_is_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/variable_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/variable_permissibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/variable_value_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/whodrug_hierarchy_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/whodrug_references_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/rules_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.394731 cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/base_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/dataset_metadata_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/rule_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.398731 cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/term_serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/term_serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/term_serializers/atc_classification_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/term_serializers/atc_text_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/term_serializers/base_whodrug_term_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/term_serializers/drug_dictionary_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/term_serializers/meddra_term_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.398731 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/adam_variable_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.398731 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/cache/cache_populator_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/cache/cache_service_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/cache/in_memory_cache_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/cache/redis_cache_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    20318 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/cdisc_library_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.402731 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_readers/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_readers/data_reader_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_readers/xpt_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.402731 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_services/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_services/base_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_services/data_service_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_services/dummy_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_services/local_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/dataset_metadata_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/define_xml_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.402731 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/logging/console_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/logging/logging_service_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.406731 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/reporting/base_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/reporting/excel_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/reporting/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/reporting/json_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/reporting/report_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.406731 cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/dataset_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/progress_displayers.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/reporting_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/rule_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/validation_output_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:21:02.358732 cdisc-rules-engine-0.6.1/cdisc_rules_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14452 2023-05-03 15:21:02.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-05-03 15:21:02.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:21:02.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-03 15:21:02.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 15:21:02.000000 cdisc-rules-engine-0.6.1/cdisc_rules_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:21:02.406731 cdisc-rules-engine-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-03 15:20:31.000000 cdisc-rules-engine-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.635769 cdisc-rules-engine-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-06-30 17:24:58.635769 cdisc-rules-engine-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.615769 cdisc-rules-engine-0.6.2/TestRule/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/TestRule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.615769 cdisc-rules-engine-0.6.2/cdisc_rule_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rule_tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.615769 cdisc-rules-engine-0.6.2/cdisc_rule_tester/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rule_tester/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rule_tester/models/rule_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.615769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.615769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.615769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/constants/cache_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/constants/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/constants/define_xml_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/constants/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/constants/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/constants/permissibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/constants/rule_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.619769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/base_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/content_metadata_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/contents_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/contents_define_variables_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/contents_define_vlm_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/dataset_builder_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/define_item_group_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/define_variables_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/domain_list_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/values_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/variables_metadata_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/variables_metadata_with_define_dataset_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.619769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dummy_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dummy_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dummy_models/dummy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/dummy_models/dummy_variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.619769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/base_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/default_file_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/execution_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/library_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/optional_condition_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/progress_parameter_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/report_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/rule_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/variable_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.619769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/exceptions/custom_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.619769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/cache_service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/condition_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/config_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/data_reader_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/data_service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/dictionary_term_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/factory_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/logger_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/representation_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/terms_factory_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.623769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/base_validation_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dataset_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dataset_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dataset_variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.623769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/define/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/define/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/define/value_level_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.623769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/abstract_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/dictionary_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/get_dictionary_terms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.623769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/meddra/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/meddra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/meddra/meddra_file_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/meddra/meddra_terms_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/meddra/meddra_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.623769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/meddra/terms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/meddra/terms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/meddra/terms/meddra_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/meddra/terms/term_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.623769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/atc_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/atc_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/base_whodrug_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/drug_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_file_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_record_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_terms_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/failed_validation_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/operation_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/record_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.623769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_conditions/allowed_conditions_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_conditions/condition_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_conditions/condition_composite_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_conditions/not_condition_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_conditions/single_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_validation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/validation_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/validation_error_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/validation_error_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/variable_metadata_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.631769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14244 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/base_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/dataset_column_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/day_data_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/define_variable_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/distinct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/domain_is_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/domain_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/expected_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/extract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/get_model_filtered_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/label_referenced_variable_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/library_column_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/library_model_column_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/max_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/meddra_code_references_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/meddra_code_term_pairs_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/meddra_term_references_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/min_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/name_referenced_variable_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/operations_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/parent_library_model_column_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/permissible_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/record_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/required_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/study_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/valid_codelist_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/variable_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/variable_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/variable_is_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/variable_library_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/variable_value_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/whodrug_hierarchy_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/whodrug_references_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/plugin_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/rules_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.631769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/base_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/dataset_metadata_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/rule_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.631769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/term_serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/term_serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/term_serializers/atc_classification_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/term_serializers/atc_text_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/term_serializers/base_whodrug_term_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/term_serializers/drug_dictionary_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/term_serializers/meddra_term_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.631769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/adam_variable_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.631769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/cache/cache_populator_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/cache/cache_service_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/cache/in_memory_cache_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/cache/redis_cache_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/cdisc_library_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.631769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_readers/data_reader_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_readers/xpt_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.631769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_services/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_services/base_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_services/data_service_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_services/dummy_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_services/local_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/dataset_metadata_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.631769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/logging/console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/logging/logging_service_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.635769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/reporting/base_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/reporting/excel_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/reporting/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/reporting/json_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/reporting/report_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.635769 cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/dataset_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/progress_displayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/reporting_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/rule_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-30 17:24:21.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/validation_output_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:24:58.615769 cdisc-rules-engine-0.6.2/cdisc_rules_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-06-30 17:24:58.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-30 17:24:58.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:24:58.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-30 17:24:58.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 17:24:58.000000 cdisc-rules-engine-0.6.2/cdisc_rules_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 17:24:58.635769 cdisc-rules-engine-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-30 17:24:22.000000 cdisc-rules-engine-0.6.2/setup.py
```

### Comparing `cdisc-rules-engine-0.6.1/LICENSE` & `cdisc-rules-engine-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/PKG-INFO` & `cdisc-rules-engine-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: cdisc-rules-engine
-Version: 0.6.1
+Version: 0.6.2
 Summary: Open source offering of the cdisc rules engine
 Home-page: https://github.com/cdisc-org/cdisc-rules-engine
 Author: cdisc-org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Supported python versions
+
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-orange.svg)](https://www.python.org/downloads/release/python-380)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-green.svg)](https://www.python.org/downloads/release/python-390)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-310)
+
 # cdisc-rules-engine
+
 Open source offering of the cdisc rules engine
 
 ### Quick start
 
-To quickly get up and running with CORE, users can download the latest executable version of the engine for their operating system from here: https://github.com/cdisc-org/cdisc-rules-engine/releases
+To quickly get up and running with CORE, users can download the latest executable version of the engine for their operating system from here: <https://github.com/cdisc-org/cdisc-rules-engine/releases>
 
 Once downloaded, simply unzip the file and run the following command based on your Operating System:
 
 Windows:
 
 ```
 .\core.exe validate -s <standard> -v <standard_version> -d path/to/datasets
@@ -34,52 +37,58 @@
 Linux/Mac:
 
 ```
 ./core validate -s <standard> -v <standard_version> -d path/to/datasets
 
 # ex: ./core validate -s sdtmig -v 3-4 -d .\xpt\
 ```
+
 ### Code formatter
-This project uses the `black` code formatter and `flake8` linter for python.
-It also uses `pre-commit` to run `black` and `flake8` when you commit.
-Both dependencies are added to *requirements.txt*.
+
+This project uses the `black` code formatter, `flake8` linter for python and `prettier` for JSON, YAML and MD.
+It also uses `pre-commit` to run `black`, `flake8` and `prettier` when you commit.
+Both dependencies are added to _requirements.txt_.
 
 **Required**
 
 Setting up `pre-commit` requires one extra step. After installing it you have to run
 
 `pre-commit install`
 
 This installs `pre-commit` in your `.git/hooks` directory.
 
-### Installing dependencies.
+### Installing dependencies
+
 These steps should be run before running any tests or core commands using the non compiled version.
 
-* Create a virtual environment:
-`python -m venv <virtual_environment_name>`
-* Activate the virtual environment:
+- Create a virtual environment:
+  `python -m venv <virtual_environment_name>`
+- Activate the virtual environment:
 
 `./<virtual_environment_name>/bin/activate` -- on linux/mac </br>
 `.\<virtual_environment_name>\Scripts\Activate` -- on windows
 
-* Install the requirements.
+- Install the requirements.
 
 `python -m pip install -r requirements.txt` # From the root directory
 
 ### Running The Tests
+
 From the root of the project run the following command:
 
 `python -m pytest tests/unit/`
+
 ### Running a validation
 
 #### From the command line
 
 Clone the repository and run `python core.py --help` to see the full list of commands.
 
 Run `python core.py validate --help` to see the list of validation options.
+
 ```
   -ca, --cache TEXT               Relative path to cache files containing pre
                                   loaded metadata and rules
   -ps, --pool-size INTEGER         Number of parallel processes for validation
   -d, --data TEXT                 Path to directory containing data files
   -dp, --dataset-path TEXT        Absolute path to dataset file. Can be specified multiple times.
   -l, --log-level [info|debug|error|critical|disabled|warn]
@@ -114,55 +123,58 @@
                                   "[████████████████████████████--------]
                                   78%"is printed.
   --help                          Show this message and exit.
 ```
 
 ##### Available log levels
 
-* `debug` - Display all logs
-* `info` - Display info, warnings, and error logs
-* `warn` - Display warnings and errors
-* `error` - Display only error logs
-* `critical` - Display critical logs
+- `debug` - Display all logs
+- `info` - Display info, warnings, and error logs
+- `warn` - Display warnings and errors
+- `error` - Display only error logs
+- `critical` - Display critical logs
 
 ##### Validate folder
+
 To validate a folder using rules for SDTM-IG version 3.4 use the following command:
 
 `python core.py validate -s sdtmig -v 3-4 -d path/to/datasets`
 
 ##### Understanding the Rules Report
+
 The rules report tab displays the run status of each rule selected for validation
 
 The possible rule run statuses are:
 
-* `SUCCESS` - The rule ran and data was validated against the rule. May or may not produce results
-* `SKIPPED` - The rule was unable to be run. Usually due to missing required data, but could also be cause by rule execution errors.
+- `SUCCESS` - The rule ran and data was validated against the rule. May or may not produce results
+- `SKIPPED` - The rule was unable to be run. Usually due to missing required data, but could also be cause by rule execution errors.
 
 ##### Additional Core Commands
 
-* update-cache - update locally stored cache data (Requires an environment variable - `CDISC_LIBRARY_API_KEY`)
+- update-cache - update locally stored cache data (Requires an environment variable - `CDISC_LIBRARY_API_KEY`)
 
-    `python core.py update-cache`
-    
-    To obtain an api key, please follow the instructions found here: https://wiki.cdisc.org/display/LIBSUPRT/Getting+Started%3A+Access+to+CDISC+Library+API+using+API+Key+Authentication. Please note it can take up to an hour after sign up to have an api key issued
+  `python core.py update-cache`
 
-* list-rules - list rules available in the cache
+  To obtain an api key, please follow the instructions found here: <https://wiki.cdisc.org/display/LIBSUPRT/Getting+Started%3A+Access+to+CDISC+Library+API+using+API+Key+Authentication>. Please note it can take up to an hour after sign up to have an api key issued
 
-    * list all rules:
+- list-rules - list rules available in the cache
+
+  - list all rules:
 
     `python core.py list-rules`
 
-    * list rules for standard:
+  - list rules for standard:
 
     `python core.py list-rules -s sdtmig -v 3-4`
 
-* list-rule-sets - lists all standards and versions for which rules are available:
-    `python core.py list-rule-sets`
+- list-rule-sets - lists all standards and versions for which rules are available:
+  `python core.py list-rule-sets`
+
+- test - Test authored rule given dataset in json format
 
-* test - Test authored rule given dataset in json format
 ```
   -ca, --cache TEXT               Relative path to cache files containing pre
                                   loaded metadata and rules
   -dp, --dataset-path TEXT        Absolute path to dataset file
   -s, --standard TEXT             CDISC standard to validate against
                                   [required]
   -v, --version TEXT              Standard version to validate against
@@ -176,15 +188,15 @@
   --meddra TEXT                   Path to directory with MedDRA dictionary
                                   files
   -r, --rule TEXT                 Path to rule json file.
   --help                          Show this message and exit.
 ```
 
 EX: `python core.py test -s sdtmig -v 3-4 -dp <path to dataset json file> -r <path to rule json file> --meddra ./meddra/ --whodrug ./whodrug/`
-Note: JSON dataset should match the format provided by the rule editor: 
+Note: JSON dataset should match the format provided by the rule editor:
 
 ```
 {
     "datasets": [{
       "filename": "cm.xpt",
       "label": "Concomitant/Concurrent medications",
       "domain": "CM",
@@ -205,14 +217,29 @@
         ],
       }
     }
   ]
 }
 ```
 
+- list-ct - list ct packages available in the cache
+
+```
+Usage: python core.py list-ct [OPTIONS]
+
+  Command to list the ct packages available in the cache.
+
+Options:
+  -c, --cache_path TEXT  Relative path to cache files containing pre loaded
+                         metadata and rules
+  -s, --subsets TEXT     CT package subset type. Ex: sdtmct. Multiple values
+                         allowed
+  --help                 Show this message and exit.
+```
+
 #### PyPI Quickstart: Validate data within python
 
 An alternative to running the validation from the command line is to instead import the rules engine library in python and run rules against data directly (without needing your data to be in `.xpt` format).
 
 ##### Step 0: Install the library
 
 ```
@@ -231,15 +258,15 @@
 
 from multiprocessing.managers import SyncManager
 from cdisc_rules_engine.services.cache import InMemoryCacheService
 
 class CacheManager(SyncManager):
     pass
 
-# If you're working from a terminal you may need to 
+# If you're working from a terminal you may need to
 # use SyncManager directly rather than define CacheManager
 CacheManager.register("InMemoryCacheService", InMemoryCacheService)
 
 
 def load_rules_cache(path_to_rules_cache):
   cache_path = pathlib.Path(path_to_rules_cache)
   manager = CacheManager()
@@ -247,15 +274,15 @@
   cache = manager.InMemoryCacheService()
 
   files = next(os.walk(cache_path), (None, None, []))[2]
 
   for fname in files:
       with open(cache_path / fname, "rb") as f:
           cache.add_all(pickle.load(f))
-  
+
   return cache
 ```
 
 Rules in this cache can be accessed by standard and version using the `get_rules_cache_key` function.
 
 ```python
 from cdisc_rules_engine.utilities.utils import get_rules_cache_key
@@ -264,31 +291,31 @@
 # Note that the standard version is separated by a dash, not a period
 cache_key_prefix = get_rules_cache_key("sdtmig", "3-4")
 rules = cache.get_all_by_prefix(cache_key_prefix)
 ```
 
 `rules` will now be a list of dictionaries the following keys
 
- - `core_id`
-   - e.g. "CORE-000252"
- - `domains`
-   - e.g. `{'Include': ['DM'], 'Exclude': []}` or `{'Include': ['ALL']}`
- - `author`
- - `reference`
- - `sensitivity`
- - `executability`
- - `description`
- - `authorities`
- - `standards`
- - `classes`
- - `rule_type`
- - `conditions`
- - `actions`
- - `datasets`
- - `output_variables`
+- `core_id`
+  - e.g. "CORE-000252"
+- `domains`
+  - e.g. `{'Include': ['DM'], 'Exclude': []}` or `{'Include': ['ALL']}`
+- `author`
+- `reference`
+- `sensitivity`
+- `executability`
+- `description`
+- `authorities`
+- `standards`
+- `classes`
+- `rule_type`
+- `conditions`
+- `actions`
+- `datasets`
+- `output_variables`
 
 ##### Step 2: Prepare your data
 
 In order to pass your data through the rules engine, it must be a pandas dataframe of an SDTM dataset. For example:
 
 ```
 >>> data
@@ -310,15 +337,15 @@
 
 Next, we need to actually run the rules. We can select which rules we want to run based on the domain of the data we're checking and the `"Include"` and `"Exclude"` domains of the rule.
 
 ```python
 # Get the rules for the domain AE
 # (Note: we're ignoring ALL domain rules here)
 ae_rules = [
-  rule for rule in rules 
+  rule for rule in rules
   if "AE" in rule["domains"].get("Include", [])
 ]
 ```
 
 There's one last thing we need before we can actually run the rule, and that's a `COREActions` object. This object will handle generating error messages should the rule fail.
 
 To instantiate a `COREActions` object, we need to pass in the following:
@@ -352,14 +379,15 @@
   defined_actions=core_actions,
 )
 ```
 
 ##### Step 5: Interpret the results
 
 The return value of run will tell us if the rule was triggered.
+
 - A `False` value means that there were no errors
 - A `True` value means that there were errors
 
 If there were errors, they will have been appended to the results array passed into your `COREActions` instance. Here's an example error:
 
 ```python
 {
```

### Comparing `cdisc-rules-engine-0.6.1/README.md` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,32 @@
+Metadata-Version: 2.1
+Name: cdisc-rules-engine
+Version: 0.6.2
+Summary: Open source offering of the cdisc rules engine
+Home-page: https://github.com/cdisc-org/cdisc-rules-engine
+Author: cdisc-org
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ### Supported python versions
+
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-orange.svg)](https://www.python.org/downloads/release/python-380)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-green.svg)](https://www.python.org/downloads/release/python-390)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-310)
+
 # cdisc-rules-engine
+
 Open source offering of the cdisc rules engine
 
 ### Quick start
 
-To quickly get up and running with CORE, users can download the latest executable version of the engine for their operating system from here: https://github.com/cdisc-org/cdisc-rules-engine/releases
+To quickly get up and running with CORE, users can download the latest executable version of the engine for their operating system from here: <https://github.com/cdisc-org/cdisc-rules-engine/releases>
 
 Once downloaded, simply unzip the file and run the following command based on your Operating System:
 
 Windows:
 
 ```
 .\core.exe validate -s <standard> -v <standard_version> -d path/to/datasets
@@ -23,52 +37,58 @@
 Linux/Mac:
 
 ```
 ./core validate -s <standard> -v <standard_version> -d path/to/datasets
 
 # ex: ./core validate -s sdtmig -v 3-4 -d .\xpt\
 ```
+
 ### Code formatter
-This project uses the `black` code formatter and `flake8` linter for python.
-It also uses `pre-commit` to run `black` and `flake8` when you commit.
-Both dependencies are added to *requirements.txt*.
+
+This project uses the `black` code formatter, `flake8` linter for python and `prettier` for JSON, YAML and MD.
+It also uses `pre-commit` to run `black`, `flake8` and `prettier` when you commit.
+Both dependencies are added to _requirements.txt_.
 
 **Required**
 
 Setting up `pre-commit` requires one extra step. After installing it you have to run
 
 `pre-commit install`
 
 This installs `pre-commit` in your `.git/hooks` directory.
 
-### Installing dependencies.
+### Installing dependencies
+
 These steps should be run before running any tests or core commands using the non compiled version.
 
-* Create a virtual environment:
-`python -m venv <virtual_environment_name>`
-* Activate the virtual environment:
+- Create a virtual environment:
+  `python -m venv <virtual_environment_name>`
+- Activate the virtual environment:
 
 `./<virtual_environment_name>/bin/activate` -- on linux/mac </br>
 `.\<virtual_environment_name>\Scripts\Activate` -- on windows
 
-* Install the requirements.
+- Install the requirements.
 
 `python -m pip install -r requirements.txt` # From the root directory
 
 ### Running The Tests
+
 From the root of the project run the following command:
 
 `python -m pytest tests/unit/`
+
 ### Running a validation
 
 #### From the command line
 
 Clone the repository and run `python core.py --help` to see the full list of commands.
 
 Run `python core.py validate --help` to see the list of validation options.
+
 ```
   -ca, --cache TEXT               Relative path to cache files containing pre
                                   loaded metadata and rules
   -ps, --pool-size INTEGER         Number of parallel processes for validation
   -d, --data TEXT                 Path to directory containing data files
   -dp, --dataset-path TEXT        Absolute path to dataset file. Can be specified multiple times.
   -l, --log-level [info|debug|error|critical|disabled|warn]
@@ -103,55 +123,58 @@
                                   "[████████████████████████████--------]
                                   78%"is printed.
   --help                          Show this message and exit.
 ```
 
 ##### Available log levels
 
-* `debug` - Display all logs
-* `info` - Display info, warnings, and error logs
-* `warn` - Display warnings and errors
-* `error` - Display only error logs
-* `critical` - Display critical logs
+- `debug` - Display all logs
+- `info` - Display info, warnings, and error logs
+- `warn` - Display warnings and errors
+- `error` - Display only error logs
+- `critical` - Display critical logs
 
 ##### Validate folder
+
 To validate a folder using rules for SDTM-IG version 3.4 use the following command:
 
 `python core.py validate -s sdtmig -v 3-4 -d path/to/datasets`
 
 ##### Understanding the Rules Report
+
 The rules report tab displays the run status of each rule selected for validation
 
 The possible rule run statuses are:
 
-* `SUCCESS` - The rule ran and data was validated against the rule. May or may not produce results
-* `SKIPPED` - The rule was unable to be run. Usually due to missing required data, but could also be cause by rule execution errors.
+- `SUCCESS` - The rule ran and data was validated against the rule. May or may not produce results
+- `SKIPPED` - The rule was unable to be run. Usually due to missing required data, but could also be cause by rule execution errors.
 
 ##### Additional Core Commands
 
-* update-cache - update locally stored cache data (Requires an environment variable - `CDISC_LIBRARY_API_KEY`)
+- update-cache - update locally stored cache data (Requires an environment variable - `CDISC_LIBRARY_API_KEY`)
+
+  `python core.py update-cache`
 
-    `python core.py update-cache`
-    
-    To obtain an api key, please follow the instructions found here: https://wiki.cdisc.org/display/LIBSUPRT/Getting+Started%3A+Access+to+CDISC+Library+API+using+API+Key+Authentication. Please note it can take up to an hour after sign up to have an api key issued
+  To obtain an api key, please follow the instructions found here: <https://wiki.cdisc.org/display/LIBSUPRT/Getting+Started%3A+Access+to+CDISC+Library+API+using+API+Key+Authentication>. Please note it can take up to an hour after sign up to have an api key issued
 
-* list-rules - list rules available in the cache
+- list-rules - list rules available in the cache
 
-    * list all rules:
+  - list all rules:
 
     `python core.py list-rules`
 
-    * list rules for standard:
+  - list rules for standard:
 
     `python core.py list-rules -s sdtmig -v 3-4`
 
-* list-rule-sets - lists all standards and versions for which rules are available:
-    `python core.py list-rule-sets`
+- list-rule-sets - lists all standards and versions for which rules are available:
+  `python core.py list-rule-sets`
+
+- test - Test authored rule given dataset in json format
 
-* test - Test authored rule given dataset in json format
 ```
   -ca, --cache TEXT               Relative path to cache files containing pre
                                   loaded metadata and rules
   -dp, --dataset-path TEXT        Absolute path to dataset file
   -s, --standard TEXT             CDISC standard to validate against
                                   [required]
   -v, --version TEXT              Standard version to validate against
@@ -165,15 +188,15 @@
   --meddra TEXT                   Path to directory with MedDRA dictionary
                                   files
   -r, --rule TEXT                 Path to rule json file.
   --help                          Show this message and exit.
 ```
 
 EX: `python core.py test -s sdtmig -v 3-4 -dp <path to dataset json file> -r <path to rule json file> --meddra ./meddra/ --whodrug ./whodrug/`
-Note: JSON dataset should match the format provided by the rule editor: 
+Note: JSON dataset should match the format provided by the rule editor:
 
 ```
 {
     "datasets": [{
       "filename": "cm.xpt",
       "label": "Concomitant/Concurrent medications",
       "domain": "CM",
@@ -194,14 +217,29 @@
         ],
       }
     }
   ]
 }
 ```
 
+- list-ct - list ct packages available in the cache
+
+```
+Usage: python core.py list-ct [OPTIONS]
+
+  Command to list the ct packages available in the cache.
+
+Options:
+  -c, --cache_path TEXT  Relative path to cache files containing pre loaded
+                         metadata and rules
+  -s, --subsets TEXT     CT package subset type. Ex: sdtmct. Multiple values
+                         allowed
+  --help                 Show this message and exit.
+```
+
 #### PyPI Quickstart: Validate data within python
 
 An alternative to running the validation from the command line is to instead import the rules engine library in python and run rules against data directly (without needing your data to be in `.xpt` format).
 
 ##### Step 0: Install the library
 
 ```
@@ -220,15 +258,15 @@
 
 from multiprocessing.managers import SyncManager
 from cdisc_rules_engine.services.cache import InMemoryCacheService
 
 class CacheManager(SyncManager):
     pass
 
-# If you're working from a terminal you may need to 
+# If you're working from a terminal you may need to
 # use SyncManager directly rather than define CacheManager
 CacheManager.register("InMemoryCacheService", InMemoryCacheService)
 
 
 def load_rules_cache(path_to_rules_cache):
   cache_path = pathlib.Path(path_to_rules_cache)
   manager = CacheManager()
@@ -236,15 +274,15 @@
   cache = manager.InMemoryCacheService()
 
   files = next(os.walk(cache_path), (None, None, []))[2]
 
   for fname in files:
       with open(cache_path / fname, "rb") as f:
           cache.add_all(pickle.load(f))
-  
+
   return cache
 ```
 
 Rules in this cache can be accessed by standard and version using the `get_rules_cache_key` function.
 
 ```python
 from cdisc_rules_engine.utilities.utils import get_rules_cache_key
@@ -253,31 +291,31 @@
 # Note that the standard version is separated by a dash, not a period
 cache_key_prefix = get_rules_cache_key("sdtmig", "3-4")
 rules = cache.get_all_by_prefix(cache_key_prefix)
 ```
 
 `rules` will now be a list of dictionaries the following keys
 
- - `core_id`
-   - e.g. "CORE-000252"
- - `domains`
-   - e.g. `{'Include': ['DM'], 'Exclude': []}` or `{'Include': ['ALL']}`
- - `author`
- - `reference`
- - `sensitivity`
- - `executability`
- - `description`
- - `authorities`
- - `standards`
- - `classes`
- - `rule_type`
- - `conditions`
- - `actions`
- - `datasets`
- - `output_variables`
+- `core_id`
+  - e.g. "CORE-000252"
+- `domains`
+  - e.g. `{'Include': ['DM'], 'Exclude': []}` or `{'Include': ['ALL']}`
+- `author`
+- `reference`
+- `sensitivity`
+- `executability`
+- `description`
+- `authorities`
+- `standards`
+- `classes`
+- `rule_type`
+- `conditions`
+- `actions`
+- `datasets`
+- `output_variables`
 
 ##### Step 2: Prepare your data
 
 In order to pass your data through the rules engine, it must be a pandas dataframe of an SDTM dataset. For example:
 
 ```
 >>> data
@@ -299,15 +337,15 @@
 
 Next, we need to actually run the rules. We can select which rules we want to run based on the domain of the data we're checking and the `"Include"` and `"Exclude"` domains of the rule.
 
 ```python
 # Get the rules for the domain AE
 # (Note: we're ignoring ALL domain rules here)
 ae_rules = [
-  rule for rule in rules 
+  rule for rule in rules
   if "AE" in rule["domains"].get("Include", [])
 ]
 ```
 
 There's one last thing we need before we can actually run the rule, and that's a `COREActions` object. This object will handle generating error messages should the rule fail.
 
 To instantiate a `COREActions` object, we need to pass in the following:
@@ -341,14 +379,15 @@
   defined_actions=core_actions,
 )
 ```
 
 ##### Step 5: Interpret the results
 
 The return value of run will tell us if the rule was triggered.
+
 - A `False` value means that there were no errors
 - A `True` value means that there were errors
 
 If there were errors, they will have been appended to the results array passed into your `COREActions` instance. Here's an example error:
 
 ```python
 {
```

### Comparing `cdisc-rules-engine-0.6.1/TestRule/__init__.py` & `cdisc-rules-engine-0.6.2/TestRule/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             f"one or more datasets missing the following keys {missing_keys}"
         )
 
 
 def main(req: func.HttpRequest, context: func.Context) -> func.HttpResponse:
     try:
         json_data = req.get_json()
-        api_key = os.environ.get("LIBRARY_API_KEY")
+        api_key = os.environ.get("CDISC_LIBRARY_API_KEY")
         rule = json_data.get("rule")
         standards_data = json_data.get("standard", {})
         standard = standards_data.get("product")
         standard_version = standards_data.get("version")
         codelists = json_data.get("codelists", [])
         cache = InMemoryCacheService()
         if standards_data or codelists:
@@ -45,15 +45,17 @@
             raise KeyError("'rule' required in request")
         datasets = json_data.get("datasets")
         if not datasets:
             raise KeyError("'datasets' required in request")
         validate_datasets_payload(datasets)
         define_xml = json_data.get("define_xml")
         tester = RuleTester(datasets, define_xml, cache, standard, standard_version)
-        return func.HttpResponse(json.dumps(tester.validate(rule)))
+        result = tester.validate(rule)
+        result_json = json.dumps(result)
+        return func.HttpResponse(result_json)
     except KeyError as e:
         return func.HttpResponse(
             json.dumps({"error": "KeyError", "message": str(e)}), status_code=400
         )
     except Exception as e:
         return func.HttpResponse(
             json.dumps(
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rule_tester/models/rule_tester.py` & `cdisc-rules-engine-0.6.2/cdisc_rule_tester/models/rule_tester.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/config/config.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/config/config.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/constants/__init__.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/content_metadata_dataset_builder.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/content_metadata_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/contents_dataset_builder.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/contents_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/dataset_builder_factory.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/dataset_builder_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 )
 from cdisc_rules_engine.dataset_builders.variables_metadata_with_define_dataset_builder import (
     VariablesMetadataWithDefineDatasetBuilder,
 )
 from cdisc_rules_engine.dataset_builders.define_item_group_dataset_builder import (
     DefineItemGroupDatasetBuilder,
 )
+from cdisc_rules_engine.dataset_builders.contents_define_variables_dataset_builder import (
+    ContentsDefineVariablesDatasetBuilder,
+)
+from cdisc_rules_engine.dataset_builders.contents_define_vlm_dataset_builder import (
+    ContentsDefineVLMDatasetBuilder,
+)
 from cdisc_rules_engine.dataset_builders.base_dataset_builder import BaseDatasetBuilder
 from cdisc_rules_engine.enums.rule_types import RuleTypes
 
 
 class DatasetBuilderFactory(FactoryInterface):
     _builders_map = {
         RuleTypes.DATASET_METADATA_CHECK.value: ContentMetadataDatasetBuilder,
@@ -34,14 +40,16 @@
         RuleTypes.VARIABLE_METADATA_CHECK.value: VariablesMetadataDatasetBuilder,
         RuleTypes.DOMAIN_PRESENCE_CHECK.value: DomainListDatasetBuilder,
         RuleTypes.DEFINE_ITEM_METADATA_CHECK.value: DefineVariablesDatasetBuilder,
         RuleTypes.VARIABLE_METADATA_CHECK_AGAINST_DEFINE.value: VariablesMetadataWithDefineDatasetBuilder,
         RuleTypes.DATASET_CONTENTS_CHECK_AGAINST_DEFINE_AND_LIBRARY.value: ContentsDatasetBuilder,
         RuleTypes.VALUE_LEVEL_METADATA_CHECK_AGAINST_DEFINE.value: ContentsDatasetBuilder,
         RuleTypes.DEFINE_ITEM_GROUP_METADATA_CHECK.value: DefineItemGroupDatasetBuilder,
+        RuleTypes.VALUE_CHECK_AGAINST_DEFINE_XML_VARIABLE.value: ContentsDefineVariablesDatasetBuilder,
+        RuleTypes.VALUE_CHECK_AGAINST_DEFINE_XML_VLM.value: ContentsDefineVLMDatasetBuilder,
     }
 
     @classmethod
     def register_service(cls, name: str, builder: Type[BaseDatasetBuilder]) -> None:
         """
         Save mapping of operation name and it's implementation
         """
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/define_item_group_dataset_builder.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/define_item_group_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/define_variables_dataset_builder.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/define_variables_dataset_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,11 +15,15 @@
         "define_variable_role",
         "define_variable_size",
         "define_variable_ccode",
         "define_variable_format",
         "define_variable_allowed_terms",
         "define_variable_origin_type",
         "define_variable_is_collected",
+        "define_variable_has_no_data",
+        "define_variable_order_number",
+        "define_variable_has_codelist",
+        "define_variable_codelist_coded_values",
         """
         # get Define XML metadata for domain and use it as a rule comparator
         variable_metadata: List[dict] = self.get_define_xml_variables_metadata()
         return pd.DataFrame(variable_metadata)
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/domain_list_dataset_builder.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/domain_list_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/variables_metadata_dataset_builder.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/variables_metadata_dataset_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class VariablesMetadataDatasetBuilder(BaseDatasetBuilder):
     def build(self):
         """
          Returns the variable metadata from a given file as a dataframe.
          The resulting dataframe has the following columns:
         variable_name
-        variable_order
+        variable_order_number
         variable_label
         variable_size
         variable_data_type
         variable_format
         """
         return self.data_service.get_variables_metadata(
             self.dataset_path, drop_duplicates=True
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/dataset_builders/variables_metadata_with_define_dataset_builder.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/dataset_builders/variables_metadata_with_define_dataset_builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,32 @@
 
 class VariablesMetadataWithDefineDatasetBuilder(BaseDatasetBuilder):
     def build(self):
         """
         Returns the variable metadata from a given file.
         Returns a dataframe with the following columns:
         variable_name
-        variable_order
+        variable_order_number
         variable_label
         variable_size
         variable_data_type
         define_variable_name,
         define_variable_label,
         define_variable_data_type,
         define_variable_role,
         define_variable_size,
         define_variable_ccode,
         define_variable_format,
         define_variable_allowed_terms,
         define_variable_origin_type,
-
+        define_variable_is_collected,
+        define_variable_has_no_data,
+        define_variable_order_number,
+        define_variable_has_codelist,
+        define_variable_codelist_coded_values
         """
         # get Define XML metadata for domain and use it as a rule comparator
         variable_metadata: List[dict] = self.get_define_xml_variables_metadata()
         # get dataset metadata and execute the rule
         content_metadata: pd.DataFrame = self.data_service.get_variables_metadata(
             self.dataset_path, drop_duplicates=True
         )
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/dummy_models/dummy_dataset.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/dummy_models/dummy_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,20 @@
             for variable_data in dataset_data.get("variables", [])
         ]
         self.data = pd.DataFrame.from_dict(dataset_data.get("records", {}))
 
     def get_metadata(self):
         return {
             "dataset_size": [self.filesize or 1000],
-            "dataset_name": [self.filename.split(".")[0].upper() or "test"],
+            "dataset_name": [
+                self.filename.split(".")[0].upper() if self.filename else "test"
+            ],
             "dataset_label": [self.label or "test"],
             "filename": [self.filename],
+            "length": [len(self.data.index)],
         }
 
     def validate(self, dataset_data):
         required_values = ["domain"]
         for value in required_values:
             if value not in dataset_data or dataset_data.get(value) is None:
                 raise InvalidDatasetFormat(f"Dataset missing key: {value}")
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/enums/default_file_paths.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/enums/default_file_paths.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/exceptions/custom_exceptions.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/__init__.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/cache_service_interface.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/cache_service_interface.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/condition_interface.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/condition_interface.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/data_service_interface.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/data_service_interface.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/logger_interface.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/logger_interface.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/interfaces/terms_factory_interface.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/interfaces/terms_factory_interface.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/actions.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,16 @@
             "message": "AESTDY and DOMAIN are equal to test",
         }
         """
         df_columns: set = set(data)
         targets_in_dataset = targets.intersection(df_columns)
         targets_not_in_dataset = targets.difference(df_columns)
         errors_df = data[targets_in_dataset]
+        if not targets:
+            errors_df = data
         if errors_df.empty:
             raise InvalidOutputVariables(
                 f"Output variables: {list(targets)} not found in dataset"
             )
         if self.rule.get("sensitivity") == Sensitivity.DATASET.value:
             # Only generate one error for rules with dataset sensitivity
             errors_list = [
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dataset_variable.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dataset_variable.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/define/value_level_metadata.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/define/value_level_metadata.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/abstract_factory.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/abstract_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/get_dictionary_terms.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/get_dictionary_terms.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/meddra/meddra_terms_factory.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/meddra/meddra_terms_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/meddra/terms/meddra_term.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/meddra/terms/meddra_term.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/atc_classification.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/atc_classification.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/atc_text.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/atc_text.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/base_whodrug_term.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/base_whodrug_term.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/drug_dict.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/drug_dict.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_terms_factory.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_terms_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/failed_validation_entity.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/failed_validation_entity.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/operation_params.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/operation_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,10 +17,14 @@
     domain: str
     dataset_path: str
     directory_path: str
     datasets: List[dict]
     standard: str
     standard_version: str
     target: str = None
+    original_target: str = None
     meddra_path: str = None
     whodrug_path: str = None
     grouping: List[str] = None
+    key_name: str = None
+    key_value: str = None
+    attribute_name: str = None
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/record_variable.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/record_variable.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,18 +126,19 @@
 
     @classmethod
     def build_condition(cls, condition: dict, variable_function: str) -> dict:
         data = {
             "name": variable_function,
             "operator": condition.get("operator"),
             "value": {
-                "target": condition.get("name"),
                 "comparator": condition.get("value"),
             },
         }
+        if condition.get("name"):
+            data["value"]["target"] = condition.get("name")
         if "variables" in condition:
             data["variables"] = condition["variables"]
         for optional_parameter in OptionalConditionParameters.values():
             if optional_parameter in condition:
                 data["value"][optional_parameter] = condition.get(optional_parameter)
         return data
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_conditions/condition_composite.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_conditions/condition_composite.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_conditions/condition_composite_factory.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_conditions/condition_composite_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_conditions/not_condition_composite.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_conditions/not_condition_composite.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_conditions/single_condition.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_conditions/single_condition.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/rule_validation_result.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/rule_validation_result.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/validation_error_container.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/validation_error_container.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/models/variable_metadata_container.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/models/variable_metadata_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,13 +10,13 @@
         self.labels = contents_metadata["variable_name_to_label_map"].values()
         self.sizes = contents_metadata["variable_name_to_size_map"].values()
         self.data_types = contents_metadata["variable_name_to_data_type_map"].values()
 
     def to_representation(self) -> dict:
         return {
             "variable_name": self.names,
-            "variable_order": self.order,
+            "variable_order_number": self.order,
             "variable_label": self.labels,
             "variable_size": self.sizes,
             "variable_data_type": self.data_types,
             "variable_format": self.formats,
         }
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/base_operation.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/base_operation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+from cdisc_rules_engine.services.cdisc_library_service import CDISCLibraryService
 from cdisc_rules_engine.models.operation_params import OperationParams
 from cdisc_rules_engine.constants.permissibility import (
     REQUIRED,
     PERMISSIBLE,
     REQUIRED_MODEL_VARIABLES,
     SEQ_VARIABLE,
     PERMISSIBILITY_KEY,
@@ -26,14 +27,16 @@
 
 from cdisc_rules_engine.utilities.utils import (
     get_model_details_cache_key,
     get_standard_details_cache_key,
     search_in_list_of_dicts,
     convert_library_class_name_to_ct_class,
 )
+from cdisc_rules_engine import config
+from collections import OrderedDict
 
 
 class BaseOperation:
     def __init__(
         self,
         params: OperationParams,
         original_dataset: pd.DataFrame,
@@ -58,14 +61,18 @@
         if self.params.grouping:
             return self._handle_grouped_result(result)
         elif isinstance(result, dict):
             return self._handle_dictionary_result(result)
         elif isinstance(result, pd.Series):
             self.evaluation_dataset[self.params.operation_id] = result
             return self.evaluation_dataset
+        elif isinstance(result, pd.DataFrame):
+            # Assume that the operation id has been applied and
+            # result matches the length of the evaluation dataset.
+            return pd.concat([self.evaluation_dataset, result], axis=1)
         else:
             # Handle single results
             self.evaluation_dataset[self.params.operation_id] = pd.Series(
                 [result] * len(self.evaluation_dataset)
             )
             return self.evaluation_dataset
 
@@ -105,18 +112,15 @@
             },
             ...
         ]
         """
         # get model details from cache
         if not self.params.standard or not self.params.standard_version:
             raise Exception("Please provide standard and version")
-        cache_key: str = get_standard_details_cache_key(
-            self.params.standard, self.params.standard_version
-        )
-        standard_details: dict = self.cache.get(cache_key) or {}
+        standard_details: dict = self._retrieve_standards_metadata()
         model = standard_details.get("_links", {}).get("model")
         class_details, domain_details = self._get_class_and_domain_metadata(
             standard_details
         )
         model_type, model_version = self._get_model_type_and_version(model)
         model_cache_key = get_model_details_cache_key(model_type, model_version)
         model_details = self.cache.get(model_cache_key) or {}
@@ -196,14 +200,27 @@
             model_version = link.split("/")[-1]
         else:
             # TODO expand to support CDASH and ADAM
             model_type = ""
             model_version = ""
         return model_type, model_version
 
+    def _retrieve_standards_metadata(self):
+        cache_key = get_standard_details_cache_key(
+            self.params.standard, self.params.standard_version
+        )
+        standard_data: dict = self.cache.get(cache_key)
+        if standard_data is None:
+            cdisc_library_service = CDISCLibraryService(config, self.cache)
+            standard_data = cdisc_library_service.get_standard_details(
+                self.params.standard.lower(), self.params.standard_version
+            )
+            self.cache.add(cache_key, standard_data)
+        return standard_data
+
     def _get_class_metadata(
         self,
         model_details: dict,
         dataset_class: str,
     ) -> dict:
         """
         Extracts metadata of a certain class
@@ -246,7 +263,98 @@
         for variable in class_variables:
             role: str = variable.get("role")
             if role == VariableRoles.IDENTIFIER.value:
                 identifier_vars.append(variable)
             elif role == VariableRoles.TIMING.value:
                 timing_vars.append(variable)
         return identifier_vars, timing_vars
+
+    def _get_variable_names_list(self, domain, dataframe):
+        # get variables metadata from the standard model
+        variables_metadata: List[
+            dict
+        ] = self._get_variables_metadata_from_standard_model(domain, dataframe)
+        # create a list of variable names in accordance to the "ordinal" key
+        variable_names_list = self._replace_variable_wildcards(
+            variables_metadata, domain
+        )
+        return list(OrderedDict.fromkeys(variable_names_list))
+
+    def _get_variables_metadata_from_standard_model(
+        self, domain, dataframe
+    ) -> List[dict]:
+        """
+        Gets variables metadata for the given class and domain from cache.
+        The cache stores CDISC Library metadata.
+
+        Return example:
+        [
+            {
+               "label":"Study Identifier",
+               "name":"STUDYID",
+               "ordinal":"1",
+               "role":"Identifier",
+               ...
+            },
+            {
+               "label":"Domain Abbreviation",
+               "name":"DOMAIN",
+               "ordinal":"2",
+               "role":"Identifier"
+            },
+            ...
+        ]
+        """
+        # get model details from cache
+        cache_key: str = get_standard_details_cache_key(
+            self.params.standard, self.params.standard_version
+        )
+
+        standard_details: dict = self.cache.get(cache_key) or {}
+        model = standard_details.get("_links", {}).get("model")
+        model_type, model_version = self._get_model_type_and_version(model)
+        model_cache_key = get_model_details_cache_key(model_type, model_version)
+        model_details = self.cache.get(model_cache_key) or {}
+        domain_details = self._get_model_domain_metadata(model_details, domain)
+        variables_metadata = []
+
+        if domain_details:
+            # Domain found in the model
+            class_name = convert_library_class_name_to_ct_class(
+                domain_details["_links"]["parentClass"]["title"]
+            )
+            class_details = self._get_class_metadata(model_details, class_name)
+            variables_metadata = domain_details.get("datasetVariables", [])
+            variables_metadata.sort(key=lambda item: item["ordinal"])
+        else:
+            # Domain not found in the model. Detect class name from data
+            class_name = self.data_service.get_dataset_class(
+                dataframe, self.params.dataset_path, self.params.datasets
+            )
+            class_name = convert_library_class_name_to_ct_class(class_name)
+            class_details = self._get_class_metadata(model_details, class_name)
+
+        if class_name in DETECTABLE_CLASSES:
+            (
+                identifiers_metadata,
+                variables_metadata,
+                timing_metadata,
+            ) = self.get_allowed_class_variables(model_details, class_details)
+            # Identifiers are added to the beginning and Timing to the end
+            if identifiers_metadata:
+                variables_metadata = identifiers_metadata + variables_metadata
+            if timing_metadata:
+                variables_metadata = variables_metadata + timing_metadata
+
+        return variables_metadata
+
+    def _get_model_domain_metadata(self, model_details, domain_name) -> Tuple:
+        # Get domain metadata from model
+        domain_details: Optional[dict] = search_in_list_of_dicts(
+            model_details.get("datasets", []), lambda item: item["name"] == domain_name
+        )
+
+        return domain_details
+
+    @staticmethod
+    def _replace_variable_wildcards(variables_metadata, domain):
+        return [var["name"].replace("--", domain) for var in variables_metadata]
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/day_data_validator.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/day_data_validator.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/distinct.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/distinct.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/domain_label.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/domain_is_custom.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 from cdisc_rules_engine.operations.base_operation import BaseOperation
 from cdisc_rules_engine.utilities.utils import (
     get_standard_details_cache_key,
-    search_in_list_of_dicts,
 )
 from cdisc_rules_engine.services.cdisc_library_service import CDISCLibraryService
 from cdisc_rules_engine import config
 
 
-class DomainLabel(BaseOperation):
+class DomainIsCustom(BaseOperation):
     def _execute_operation(self):
         """
-        Return the domain label for the currently executing domain
+        Gets standard details from cache and checks if
+        given domain is in standard domains.
+        If no -> the domain is custom.
         """
         cache_key = get_standard_details_cache_key(
             self.params.standard, self.params.standard_version
         )
         standard_data: dict = self.cache.get(cache_key)
         if standard_data is None:
             cdisc_library_service = CDISCLibraryService(config, self.cache)
-            standard_data = set(
-                cdisc_library_service.get_standard(
-                    self.params.standard.lower(), self.params.standard_version
-                )
+            standard_data = cdisc_library_service.get_standard_details(
+                self.params.standard.lower(), self.params.standard_version
             )
-            self.cache.set(cache_key, standard_data)
-        domain_details = None
-        for c in standard_data.get("classes", []):
-            domain_details = search_in_list_of_dicts(
-                c.get("datasets", []), lambda item: item["name"] == self.params.domain
-            )
-            if domain_details:
-                return domain_details.get("label", "")
-        return ""
+            self.cache.add(cache_key, standard_data)
+        return self.params.domain not in standard_data.get("domains", {})
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/expected_variables.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/expected_variables.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/library_column_order.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/library_column_order.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/max_date.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/max_date.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/meddra_code_references_validator.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/meddra_code_references_validator.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/meddra_code_term_pairs_validator.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/meddra_code_term_pairs_validator.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/meddra_term_references_validator.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/meddra_term_references_validator.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/min_date.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/min_date.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/operations_factory.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/operations_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 from cdisc_rules_engine.operations.library_column_order import LibraryColumnOrder
 from cdisc_rules_engine.operations.library_model_column_order import (
     LibraryModelColumnOrder,
 )
 from cdisc_rules_engine.operations.parent_library_model_column_order import (
     ParentLibraryModelColumnOrder,
 )
+from cdisc_rules_engine.operations.get_model_filtered_variables import (
+    LibraryModelVariablesFilter,
+)
 from cdisc_rules_engine.operations.max_date import MaxDate
 from cdisc_rules_engine.operations.maximum import Maximum
 from cdisc_rules_engine.operations.mean import Mean
+from cdisc_rules_engine.operations.domain_is_custom import DomainIsCustom
 from cdisc_rules_engine.operations.domain_label import DomainLabel
 from cdisc_rules_engine.operations.meddra_code_references_validator import (
     MedDRACodeReferencesValidator,
 )
 from cdisc_rules_engine.operations.meddra_code_term_pairs_validator import (
     MedDRACodeTermPairsValidator,
 )
@@ -34,56 +38,72 @@
 from cdisc_rules_engine.operations.variable_value_count import VariableValueCount
 from cdisc_rules_engine.operations.whodrug_references_validator import (
     WhodrugReferencesValidator,
 )
 from cdisc_rules_engine.operations.whodrug_hierarchy_validator import (
     WhodrugHierarchyValidator,
 )
-from cdisc_rules_engine.operations.variable_permissibility import VariablePermissibility
+from cdisc_rules_engine.operations.variable_library_metadata import (
+    VariableLibraryMetadata,
+)
 from cdisc_rules_engine.operations.variable_count import VariableCount
 from cdisc_rules_engine.operations.variable_is_null import VariableIsNull
 from cdisc_rules_engine.operations.required_variables import RequiredVariables
 from cdisc_rules_engine.operations.expected_variables import ExpectedVariables
 from cdisc_rules_engine.operations.permissible_variables import PermissibleVariables
 from cdisc_rules_engine.operations.study_domains import StudyDomains
 from cdisc_rules_engine.operations.valid_codelist_dates import ValidCodelistDates
+from cdisc_rules_engine.operations.label_referenced_variable_metadata import (
+    LabelReferencedVariableMetadata,
+)
+from cdisc_rules_engine.operations.name_referenced_variable_metadata import (
+    NameReferencedVariableMetadata,
+)
+from cdisc_rules_engine.operations.define_variable_metadata import (
+    DefineVariableMetadata,
+)
 
 
 class OperationsFactory(FactoryInterface):
     _operations_map = {
         "distinct": Distinct,
         "dy": DayDataValidator,
         "extract_metadata": ExtractMetadata,
         "get_column_order_from_dataset": DatasetColumnOrder,
         "get_column_order_from_library": LibraryColumnOrder,
         "get_model_column_order": LibraryModelColumnOrder,
+        "get_model_filtered_variables": LibraryModelVariablesFilter,
         "get_parent_model_column_order": ParentLibraryModelColumnOrder,
         "max": Maximum,
         "max_date": MaxDate,
         "mean": Mean,
         "min": Minimum,
         "min_date": MinDate,
         "record_count": RecordCount,
         "valid_meddra_code_references": MedDRACodeReferencesValidator,
         "valid_whodrug_references": WhodrugReferencesValidator,
         "whodrug_code_hierarchy": WhodrugHierarchyValidator,
         "valid_meddra_term_references": MedDRATermReferencesValidator,
         "valid_meddra_code_term_pairs": MedDRACodeTermPairsValidator,
         "variable_exists": VariableExists,
         "variable_names": VariableNames,
-        "variable_permissibilities": VariablePermissibility,
+        "variable_library_metadata": VariableLibraryMetadata,
         "variable_value_count": VariableValueCount,
         "variable_count": VariableCount,
         "variable_is_null": VariableIsNull,
+        "domain_is_custom": DomainIsCustom,
         "domain_label": DomainLabel,
         "required_variables": RequiredVariables,
         "expected_variables": ExpectedVariables,
         "permissible_variables": PermissibleVariables,
         "study_domains": StudyDomains,
         "valid_codelist_dates": ValidCodelistDates,
+        "label_referenced_variable_metadata": LabelReferencedVariableMetadata,
+        "name_referenced_variable_metadata": NameReferencedVariableMetadata,
+        "define_variable_metadata": DefineVariableMetadata,
     }
 
     @classmethod
     def register_service(cls, name: str, operation: Type[BaseOperation]) -> None:
         """
         Save mapping of operation name and it's implementation
         """
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/parent_library_model_column_order.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/parent_library_model_column_order.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/permissible_variables.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/permissible_variables.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/required_variables.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/required_variables.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/valid_codelist_dates.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/valid_codelist_dates.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/variable_count.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/variable_count.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+import os
 from cdisc_rules_engine.operations.base_operation import BaseOperation
 import asyncio
 from collections import Counter
 from typing import List
 
 
 class VariableCount(BaseOperation):
@@ -30,11 +31,11 @@
         ]
         dataset_variable_value_counts: List[int] = await asyncio.gather(*coroutines)
         return sum(dataset_variable_value_counts)
 
     async def _get_dataset_variable_count(self, dataset: dict) -> Counter:
         domain = dataset.get("domain", "")
         data: pd.DataFrame = self.data_service.get_dataset(
-            f"{self.params.directory_path}/{dataset.get('filename')}"
+            os.path.join(self.params.directory_path, dataset.get("filename"))
         )
-        target_variable = self.params.target.replace("--", domain, 1)
+        target_variable = self.params.original_target.replace("--", domain, 1)
         return 1 if target_variable in data else 0
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/variable_names.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/variable_library_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from cdisc_rules_engine.operations.base_operation import BaseOperation
-from cdisc_rules_engine.utilities.utils import get_library_variables_metadata_cache_key
 from cdisc_rules_engine.services.cdisc_library_service import CDISCLibraryService
+from cdisc_rules_engine.utilities.utils import get_library_variables_metadata_cache_key
 from cdisc_rules_engine import config
 
 
-class VariableNames(BaseOperation):
+class VariableLibraryMetadata(BaseOperation):
     def _execute_operation(self):
         """
-        Return the set of variable names for the given standard
+        Get the variable permissibility values for all data in the current
+        dataset.
         """
         cache_key = get_library_variables_metadata_cache_key(
             self.params.standard, self.params.standard_version
         )
         variable_details: dict = self.cache.get(cache_key)
-        if variable_details is not None:
-            variable_names = set(variable_details.keys())
-        else:
+        if variable_details is None:
             cdisc_library_service = CDISCLibraryService(config, self.cache)
-            variable_names = set(
-                cdisc_library_service.get_variables_details(
-                    self.params.standard, self.params.standard_version
-                ).keys()
+            variable_details = cdisc_library_service.get_variables_details(
+                self.params.standard, self.params.standard_version
             )
-        return variable_names
+        dataset_variable_details = variable_details.get(self.params.domain, {})
+        variable_metadata = {
+            key: dataset_variable_details[key].get(self.params.target)
+            for key in dataset_variable_details.keys()
+        }
+        return variable_metadata
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/variable_permissibility.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/variable_names.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from cdisc_rules_engine.operations.base_operation import BaseOperation
-from cdisc_rules_engine.services.cdisc_library_service import CDISCLibraryService
 from cdisc_rules_engine.utilities.utils import get_library_variables_metadata_cache_key
+from cdisc_rules_engine.services.cdisc_library_service import CDISCLibraryService
 from cdisc_rules_engine import config
 
 
-class VariablePermissibility(BaseOperation):
+class VariableNames(BaseOperation):
     def _execute_operation(self):
         """
-        Get the variable permissibility values for all data in the current
-        dataset.
+        Return the set of variable names for the given standard
         """
         cache_key = get_library_variables_metadata_cache_key(
             self.params.standard, self.params.standard_version
         )
         variable_details: dict = self.cache.get(cache_key)
         if variable_details is None:
             cdisc_library_service = CDISCLibraryService(config, self.cache)
             variable_details = cdisc_library_service.get_variables_details(
                 self.params.standard, self.params.standard_version
             )
-        variable_permissibilities = {
-            key: variable_details[key].get("core") for key in variable_details.keys()
-        }
-        return variable_permissibilities
+        all_variables = [
+            list(variable_details[dataset].values()) for dataset in variable_details
+        ]
+
+        return set(
+            [variable["name"] for variables in all_variables for variable in variables]
+        )
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/variable_value_count.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/variable_value_count.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pandas as pd
 from cdisc_rules_engine.operations.base_operation import BaseOperation
 import asyncio
+import os
 from collections import Counter
 from typing import List
 from cdisc_rules_engine.utilities.utils import (
     get_corresponding_datasets,
     is_split_dataset,
 )
 
@@ -30,22 +31,22 @@
         dataset_variable_value_counts: List[Counter] = await asyncio.gather(*coroutines)
         return dict(sum(dataset_variable_value_counts, Counter()))
 
     async def _get_dataset_variable_value_count(self, dataset: dict) -> Counter:
         domain = dataset.get("domain")
         if is_split_dataset(self.params.datasets, domain):
             files = [
-                f"{self.params.directory_path}/{dataset.get('filename')}"
+                os.path.join(self.params.directory_path, dataset.get("filename"))
                 for dataset in get_corresponding_datasets(self.params.datasets, domain)
             ]
             data: pd.DataFrame = self.data_service.join_split_datasets(
                 self.data_service.get_dataset, files
             )
         else:
             data: pd.DataFrame = self.data_service.get_dataset(
-                f"{self.params.directory_path}/{dataset.get('filename')}"
+                os.path.join(self.params.directory_path, dataset.get("filename"))
             )
-        target_variable = self.params.target.replace("--", domain, 1)
+        target_variable = self.params.original_target.replace("--", domain, 1)
         if target_variable in data:
             return Counter(data[target_variable].unique())
         else:
             return Counter()
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/whodrug_hierarchy_validator.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/whodrug_hierarchy_validator.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/operations/whodrug_references_validator.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/operations/whodrug_references_validator.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/plugin_loader.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/rules_engine.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/rules_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from copy import deepcopy
 from typing import List, Union
 
 import pandas as pd
 from business_rules import export_rule_data
 from business_rules.engine import run
-
+import os
 from cdisc_rules_engine.config import config as default_config
 from cdisc_rules_engine.constants.define_xml_constants import DEFINE_XML_FILE_NAME
 from cdisc_rules_engine.dummy_models.dummy_dataset import DummyDataset
 from cdisc_rules_engine.enums.execution_status import ExecutionStatus
 from cdisc_rules_engine.enums.rule_types import RuleTypes
 from cdisc_rules_engine.exceptions.custom_exceptions import (
     DatasetNotFoundError,
@@ -26,23 +26,24 @@
 from cdisc_rules_engine.models.failed_validation_entity import FailedValidationEntity
 from cdisc_rules_engine.models.validation_error_container import (
     ValidationErrorContainer,
 )
 from cdisc_rules_engine.services import logger
 from cdisc_rules_engine.services.cache import CacheServiceFactory, InMemoryCacheService
 from cdisc_rules_engine.services.data_services import DataServiceFactory
-from cdisc_rules_engine.services.define_xml_reader import DefineXMLReader
+from cdisc_rules_engine.services.define_xml.define_xml_reader_factory import (
+    DefineXMLReaderFactory,
+)
 from cdisc_rules_engine.utilities.data_processor import DataProcessor
 from cdisc_rules_engine.utilities.dataset_preprocessor import DatasetPreprocessor
 from cdisc_rules_engine.utilities.rule_processor import RuleProcessor
 from cdisc_rules_engine.utilities.utils import (
     get_directory_path,
     get_library_variables_metadata_cache_key,
     get_standard_codelist_cache_key,
-    get_standard_details_cache_key,
     is_split_dataset,
     serialize_rule,
 )
 from cdisc_rules_engine.dataset_builders import builder_factory
 
 
 class RulesEngine:
@@ -234,23 +235,30 @@
             rule.get("rule_type")
             == RuleTypes.DATASET_CONTENTS_CHECK_AGAINST_DEFINE_AND_LIBRARY.value
         ):
             library_metadata: dict = self.cache.get(
                 get_library_variables_metadata_cache_key(
                     self.standard, self.standard_version
                 )
-            )
+            ).get(domain, {})
             define_metadata: List[dict] = builder.get_define_xml_variables_metadata()
             targets: List[
                 str
             ] = self.data_processor.filter_dataset_columns_by_metadata_and_rule(
                 dataset.columns.tolist(), define_metadata, library_metadata, rule
             )
-            rule["conditions"] = RuleProcessor.duplicate_conditions_for_all_targets(
-                rule["conditions"], targets
+            rule_copy = deepcopy(rule)
+            updated_conditions = RuleProcessor.duplicate_conditions_for_all_targets(
+                rule_copy["conditions"], targets
+            )
+            rule_copy["conditions"].set_conditions(updated_conditions)
+            # When duplicating conditions,
+            # rule should be copied to prevent updates to concurrent rule executions
+            return self.execute_rule(
+                rule_copy, dataset, dataset_path, datasets, domain, **kwargs
             )
 
         logger.info(f"Using dataset build by: {builder.__class__}")
         return self.execute_rule(
             rule, dataset, dataset_path, datasets, domain, **kwargs
         )
 
@@ -272,51 +280,53 @@
             value_level_metadata = []
         if variable_codelist_map is None:
             variable_codelist_map = {}
         if codelist_term_maps is None:
             codelist_term_maps = []
         # Add conditions to rule for all variables if variables: all appears
         # in condition
-        rule["conditions"] = RuleProcessor.duplicate_conditions_for_all_targets(
+        rule_copy = deepcopy(rule)
+        updated_conditions = RuleProcessor.duplicate_conditions_for_all_targets(
             rule["conditions"], dataset.columns.to_list()
         )
+        rule_copy["conditions"].set_conditions(updated_conditions)
         # Adding copy for now to avoid updating cached dataset
         dataset = deepcopy(dataset)
         # preprocess dataset
         dataset_preprocessor = DatasetPreprocessor(
             dataset, domain, dataset_path, self.data_service, self.cache
         )
-        dataset = dataset_preprocessor.preprocess(rule, datasets)
+        dataset = dataset_preprocessor.preprocess(rule_copy, datasets)
         dataset = self.rule_processor.perform_rule_operations(
-            rule,
+            rule_copy,
             dataset,
             domain,
             datasets,
             dataset_path,
             standard=self.standard,
             standard_version=self.standard_version,
             meddra_path=self.meddra_path,
             whodrug_path=self.whodrug_path,
         )
         relationship_data = {}
         if self.rule_processor.is_relationship_dataset(domain):
             relationship_data = self.data_processor.preprocess_relationship_dataset(
-                dataset_path.rsplit("/", 1)[0], dataset, datasets
+                os.path.dirname(dataset_path), dataset, datasets
             )
         dataset_variable = DatasetVariable(
             dataset,
             column_prefix_map={"--": domain},
             relationship_data=relationship_data,
             value_level_metadata=value_level_metadata,
             column_codelist_map=variable_codelist_map,
             codelist_term_maps=codelist_term_maps,
         )
         results = []
         run(
-            serialize_rule(rule),  # engine expects a JSON serialized dict
+            serialize_rule(rule_copy),  # engine expects a JSON serialized dict
             defined_variables=dataset_variable,
             defined_actions=COREActions(
                 results,
                 variable=dataset_variable,
                 domain=domain,
                 rule=rule,
                 value_level_metadata=value_level_metadata,
@@ -327,52 +337,35 @@
     def get_define_xml_metadata_for_domain(
         self, dataset_path: str, domain_name: str
     ) -> dict:
         """
         Gets Define XML metadata and returns it as dict.
         """
         directory_path = get_directory_path(dataset_path)
-        define_xml_path: str = f"{directory_path}/{DEFINE_XML_FILE_NAME}"
+        define_xml_path: str = os.path.join(directory_path, DEFINE_XML_FILE_NAME)
         define_xml_contents: bytes = self.data_service.get_define_xml_contents(
             dataset_name=define_xml_path
         )
-        define_xml_reader = DefineXMLReader.from_file_contents(
+        define_xml_reader = DefineXMLReaderFactory.from_file_contents(
             define_xml_contents, cache_service_obj=self.cache
         )
         return define_xml_reader.extract_domain_metadata(domain_name=domain_name)
 
-    def is_custom_domain(self, domain: str) -> bool:
-        """
-        Gets standard details from cache and checks if
-        given domain is in standard domains.
-        If no -> the domain is custom.
-        """
-        # request standard details from cache
-        standard_details: dict = (
-            self.cache.get(
-                get_standard_details_cache_key(self.standard, self.standard_version)
-            )
-            or {}
-        )
-
-        # check if domain is in standard details
-        return domain not in standard_details.get("domains", {})
-
     def get_define_xml_value_level_metadata(
         self, dataset_path: str, domain_name: str
     ) -> List[dict]:
         """
         Gets Define XML variable metadata and returns it as dataframe.
         """
         directory_path = get_directory_path(dataset_path)
-        define_xml_path: str = f"{directory_path}/{DEFINE_XML_FILE_NAME}"
+        define_xml_path: str = os.path.join(directory_path, DEFINE_XML_FILE_NAME)
         define_xml_contents: bytes = self.data_service.get_define_xml_contents(
             dataset_name=define_xml_path
         )
-        define_xml_reader = DefineXMLReader.from_file_contents(
+        define_xml_reader = DefineXMLReaderFactory.from_file_contents(
             define_xml_contents, cache_service_obj=self.cache
         )
         return define_xml_reader.extract_value_level_metadata(domain_name=domain_name)
 
     def handle_validation_exceptions(
         self, exception, dataset_path, file_name
     ) -> ValidationErrorContainer:
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/__init__.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/dataset_metadata_serializer.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/dataset_metadata_serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,11 +39,11 @@
                 and isinstance(metadata_obj.modification_date, str)
                 and isinstance(metadata_obj.filename, str)
                 and isinstance(metadata_obj.full_path, str)
                 and (
                     isinstance(metadata_obj.size, int)
                     or isinstance(metadata_obj.size, float)
                 )
-                and isinstance(metadata_obj.records, str)
+                and isinstance(metadata_obj.records, int)
             ):
                 return False
         return True
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/rule_serializer.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/rule_serializer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/term_serializers/atc_classification_serializer.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/term_serializers/atc_classification_serializer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/term_serializers/atc_text_serializer.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/term_serializers/atc_text_serializer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/term_serializers/drug_dictionary_serializer.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/term_serializers/drug_dictionary_serializer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/serializers/term_serializers/meddra_term_serializer.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/serializers/term_serializers/meddra_term_serializer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/adam_variable_reader.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/adam_variable_reader.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/cache/cache_populator_service.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/cache/cache_populator_service.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/cache/cache_service_factory.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/cache/cache_service_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/cache/in_memory_cache_service.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/cache/in_memory_cache_service.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/cache/redis_cache_service.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/cache/redis_cache_service.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/cdisc_library_service.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/cdisc_library_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,15 +329,17 @@
                 "variables_key": "analysisVariables",
             },
         }
         standard_keys: dict = keys[standard_name]
         for cls in standard_data.get(standard_keys["classes_key"], []):
             for dataset in cls.get(standard_keys["datasets_key"], []):
                 for variable in dataset.get(standard_keys["variables_key"], []):
-                    output[variable["name"]] = variable
+                    if dataset.get("name") not in output:
+                        output[dataset.get("name")] = {}
+                    output[dataset.get("name")][variable["name"]] = variable
         return output
 
     def _get_tabulation_ig_codelists(self, data: dict) -> dict:
         """
         Extract the codelists for each variable in a cdashig.
         This dictionary of terms is then merged with the terms gathered from the
         implementation guides models.
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_readers/data_reader_factory.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_readers/data_reader_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_readers/xpt_reader.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_readers/xpt_reader.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_services/base_data_service.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_services/base_data_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from abc import ABC
 from functools import wraps, partial
 from typing import Callable, List, Optional, Iterable, Iterator
 from concurrent.futures import ThreadPoolExecutor
-
+import os
 import numpy as np
 import pandas as pd
 
 from cdisc_rules_engine.constants.domains import AP_DOMAIN_LENGTH
 from cdisc_rules_engine.interfaces import (
     CacheServiceInterface,
     ConfigInterface,
@@ -172,15 +172,15 @@
         directory_path = get_directory_path(file_path)
         if len(datasets) > 1:
             domain_details: dict = search_in_list_of_dicts(
                 datasets, lambda item: item.get("domain") == ap_suffix
             )
             if domain_details:
                 file_name = domain_details["filename"]
-                new_file_path = f"{directory_path}/{file_name}"
+                new_file_path = os.path.join(directory_path, file_name)
                 new_domain_dataset = self.get_dataset(dataset_name=new_file_path)
             else:
                 raise ValueError("Filename for domain doesn't exist")
             if self._is_associated_persons(new_domain_dataset):
                 raise ValueError("Nested Associated Persons domain reference")
             return self.get_dataset_class(new_domain_dataset, new_file_path, datasets)
         else:
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_services/data_service_factory.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_services/data_service_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_services/dummy_data_service.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_services/dummy_data_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,33 +71,34 @@
         return DatasetMetadata(
             name=dataset_metadata["dataset_name"][0],
             domain_name=dataset_metadata["dataset_name"][0],
             label=dataset_metadata["dataset_label"][0],
             modification_date=datetime.now().isoformat(),
             filename=dataset_metadata["filename"][0],
             size=dataset_metadata["dataset_size"][0],
-            records="",
+            full_path=dataset_metadata["filename"][0],
+            records=dataset_metadata["length"][0],
         )
 
     def get_variables_metadata(self, dataset_name: str, **params) -> pd.DataFrame:
         metadata_to_return = {
             "variable_name": [],
-            "variable_order": [],
+            "variable_order_number": [],
             "variable_label": [],
             "variable_size": [],
             "variable_data_type": [],
             "variable_format": [],
         }
         dataset: DummyDataset = self.get_dataset_data(dataset_name)
         for i, variable in enumerate(dataset.variables):
             metadata_to_return["variable_name"] = metadata_to_return[
                 "variable_name"
             ] + [variable.name]
-            metadata_to_return["variable_order"] = metadata_to_return[
-                "variable_order"
+            metadata_to_return["variable_order_number"] = metadata_to_return[
+                "variable_order_number"
             ] + [i + 1]
             metadata_to_return["variable_label"] = metadata_to_return[
                 "variable_label"
             ] + [variable.label]
             metadata_to_return["variable_size"] = metadata_to_return[
                 "variable_size"
             ] + [variable.length]
@@ -123,15 +124,15 @@
 
     def get_define_xml_contents(self, dataset_name: str) -> bytes:
         if not self.define_xml:
             # Search for define xml locally
             with open(dataset_name, "rb") as f:
                 return f.read()
 
-        return bytes(self.define_xml)
+        return self.define_xml.encode()
 
     def has_all_files(self, prefix: str, file_names: List[str]) -> bool:
         return True
 
     def read_data(self, file_path: str) -> IOBase:
         pass
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/data_services/local_data_service.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/data_services/local_data_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             name=contents_metadata["dataset_name"],
             domain_name=contents_metadata["domain_name"],
             label=contents_metadata["dataset_label"],
             modification_date=contents_metadata["dataset_modification_date"],
             filename=file_metadata["name"],
             full_path=file_metadata["path"],
             size=file_metadata["size"],
-            records="",
+            records=contents_metadata["dataset_length"],
         )
 
     @cached_dataset(DatasetTypes.VARIABLES_METADATA.value)
     def get_variables_metadata(self, dataset_name: str, **params) -> pandas.DataFrame:
         """
         Gets dataset from blob storage and returns metadata of a certain variable.
         """
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/dataset_metadata_reader.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/dataset_metadata_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
                 dataset.contents.Type.values, index=dataset.contents.Variable
             ).to_dict(),
             "variable_name_to_size_map": pd.Series(
                 dataset.contents.Length.values, index=dataset.contents.Variable
             ).to_dict(),
             "number_of_variables": len(dataset.columns),
             "dataset_label": dataset.dataset_label,
+            "dataset_length": dataset.shape[0],
             "domain_name": self._domain_name,
             "dataset_name": self._dataset_name,
             "dataset_modification_date": dataset.modified.isoformat(),
         }
         self._domain_name = self._extract_domain_name(dataset)
         self._convert_variable_types()
         self._metadata_container["adam_info"] = self._extract_adam_info(
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/logging/console_logger.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/logging/console_logger.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/logging/logging_service_factory.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/logging/logging_service_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/reporting/base_report.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/reporting/base_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 class BaseReport(ABC):
     """
     Generates a base report for a given set of validation results.
     """
 
     def __init__(
         self,
+        datasets: Iterable[dict],
         dataset_paths: Iterable[str],
         validation_results: List[RuleValidationResult],
         elapsed_time: float,
         args: Validation_args,
         template: Optional[IOBase] = None,
     ):
+        self._datasets = datasets
         self._dataset_paths: Iterable[str] = dataset_paths
         self._elapsed_time: float = elapsed_time
         self._results: List[RuleValidationResult] = validation_results
         self._item_type = ""
         self._args = args
         self._template = template
         self._output_name: str = f"{self._args.output}.{self._file_format}"
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/reporting/excel_report.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/reporting/excel_report.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,31 +13,33 @@
     excel_open_workbook,
     excel_update_worksheet,
     excel_workbook_to_stream,
 )
 from cdisc_rules_engine.utilities.reporting_utilities import (
     get_define_version,
 )
+from pathlib import Path
 
 
 class ExcelReport(BaseReport):
     """
     Generates an excel report for a given set of validation results.
     """
 
     def __init__(
         self,
+        datasets: Iterable[dict],
         dataset_paths: Iterable[str],
         validation_results: List[RuleValidationResult],
         elapsed_time: float,
         args: Validation_args,
         template: Optional[BinaryIO] = None,
     ):
         super().__init__(
-            dataset_paths, validation_results, elapsed_time, args, template
+            datasets, dataset_paths, validation_results, elapsed_time, args, template
         )
         self._item_type = "list"
 
     @property
     def _file_format(self):
         return ReportTypes.XLSX.value.lower()
 
@@ -55,14 +57,31 @@
         )
         # write conformance data
         wb["Conformance Details"]["B2"] = (
             datetime.now().replace(microsecond=0).isoformat()
         )
         wb["Conformance Details"]["B3"] = f"{round(self._elapsed_time, 2)} seconds"
         wb["Conformance Details"]["B4"] = __version__
+
+        # write dataset metadata
+        datasets_data = [
+            [
+                dataset.get("filename"),
+                dataset.get("label"),
+                str(Path(dataset.get("full_path", "")).parent),
+                dataset.get("modification_date"),
+                dataset.get("size", 0) / 1000,
+                dataset.get("length"),
+            ]
+            for dataset in self._datasets
+        ]
+        excel_update_worksheet(
+            wb["Dataset Details"], datasets_data, dict(wrap_text=True)
+        )
+
         # write standards details
         wb["Conformance Details"]["B7"] = standard.upper()
         wb["Conformance Details"]["B8"] = f"V{version}"
         wb["Conformance Details"]["B9"] = ", ".join(cdiscCt)
         wb["Conformance Details"]["B10"] = define_version
         if self._args.meddra:
             wb["Conformance Details"]["B13"] = self._args.meddra
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/reporting/excel_writer.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/reporting/excel_writer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/reporting/json_report.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/reporting/json_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 class JsonReport(BaseReport):
     """
     Generates a json report for a given set of validation results.
     """
 
     def __init__(
         self,
+        datasets: Iterable[dict],
         dataset_paths: Iterable[str],
         validation_results: List[RuleValidationResult],
         elapsed_time: float,
         args: Validation_args,
         template: Optional[BinaryIO] = None,
     ):
         super().__init__(
-            dataset_paths, validation_results, elapsed_time, args, template
+            datasets, dataset_paths, validation_results, elapsed_time, args, template
         )
         self._item_type = "dict"
 
     @property
     def _file_format(self) -> str:
         return ReportTypes.JSON.value.lower()
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/services/reporting/report_factory.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/services/reporting/report_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,22 @@
     elapsed_time -- time spent on validation
     args -- CLI arguments for the validate command
     data_service -- instance of engine data service to read file contents
     """
 
     def __init__(
         self,
-        dataset_paths: Iterable[str],
+        datasets: Iterable[dict],
         results: List[RuleValidationResult],
         elapsed_time: float,
         args: Validation_args,
         data_service: DataServiceInterface,
     ):
-        self._dataset_paths = dataset_paths
+        self._datasets = datasets
+        self._dataset_paths = [dataset.get("full_path") for dataset in datasets]
         self._results = results
         self._elapsed_time = elapsed_time
         self._args = args
         self._data_service = data_service
         self._output_type_service_map: Dict[str, Type[BaseReport]] = {
             ReportTypes.XLSX.value: ExcelReport,
             ReportTypes.JSON.value: JsonReport,
@@ -43,14 +44,15 @@
 
     def get_report_services(self) -> List[BaseReport]:
         services: List[BaseReport] = []
         for output_type in self._args.output_format:
             output_type: str = output_type.upper()
             service_class: Type[BaseReport] = self._output_type_service_map[output_type]
             instance: BaseReport = service_class(
+                self._datasets,
                 self._dataset_paths,
                 self._results,
                 self._elapsed_time,
                 self._args,
                 self._data_service.read_data(self._args.report_template),
             )
             services.append(instance)
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/data_processor.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/data_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     DataServiceInterface,
 )
 from cdisc_rules_engine.services.data_services import (
     DataServiceFactory,
     DummyDataService,
 )
 from cdisc_rules_engine.utilities.utils import search_in_list_of_dicts
+import os
 
 
 class DataProcessor:
     def __init__(self, data_service=None, cache: CacheServiceInterface = None):
         self.cache = cache or CacheServiceFactory(config).get_cache_service()
         self.data_service = (
             data_service or DataServiceFactory(config, self.cache).get_data_service()
@@ -81,15 +82,15 @@
         self, dataset_path: str, datasets: List[dict], columns: list, domain: str
     ):
         reference_data = {}
         domain_details: dict = search_in_list_of_dicts(
             datasets, lambda item: item.get("domain") == domain
         )
         if domain_details:
-            data_filename = f"{dataset_path}/{domain_details['filename']}"
+            data_filename = os.path.join(dataset_path, domain_details["filename"])
             new_data = self.data_service.get_dataset(dataset_name=data_filename)
             reference_data[domain] = self.get_columns(new_data, columns)
         return reference_data
 
     async def async_get_column_data(self, dataset_path, datasets, columns, domain):
         loop = asyncio.get_event_loop()
         return await loop.run_in_executor(
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/dataset_preprocessor.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/dataset_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 )
 from cdisc_rules_engine.utilities.data_processor import DataProcessor
 from cdisc_rules_engine.utilities.rule_processor import RuleProcessor
 from cdisc_rules_engine.utilities.utils import (
     replace_pattern_in_list_of_strings,
     search_in_list_of_dicts,
 )
+import os
 
 
 class DatasetPreprocessor:
     """
     The class is responsible for preprocessing the dataset
     before starting the validation.
 
@@ -88,15 +89,15 @@
         return result
 
     def _is_split_domain(self, domain: str) -> bool:
         return domain == self._dataset_domain
 
     def _download_dataset(self, filename: str) -> pd.DataFrame:
         return self._data_service.get_dataset(
-            dataset_name=f'{self._dataset_path.rsplit("/", 1)[0]}/{filename}'
+            dataset_name=os.path.join(os.path.dirname(self._dataset_path), filename)
         )
 
     def _merge_datasets(
         self,
         left_dataset: pd.DataFrame,
         left_dataset_domain_name: str,
         right_dataset: pd.DataFrame,
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/decorators.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/progress_displayers.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/progress_displayers.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/reporting_utilities.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/reporting_utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import os
 from typing import List, Optional
 
 from cdisc_rules_engine.constants.define_xml_constants import DEFINE_XML_FILE_NAME
-from cdisc_rules_engine.services.define_xml_reader import DefineXMLReader
+from cdisc_rules_engine.services.define_xml.define_xml_reader_factory import (
+    DefineXMLReaderFactory,
+)
 
 
 def get_define_version(dataset_paths: List[str]) -> Optional[str]:
     """
     Method used to extract define version from xml file located
      in the same directory with datasets
     """
     if not dataset_paths:
         return None
     path_to_data = os.path.dirname(dataset_paths[0])
     if not path_to_data or DEFINE_XML_FILE_NAME not in os.listdir(path_to_data):
         return None
-    path_to_define = "/".join([path_to_data, DEFINE_XML_FILE_NAME])
-    define_xml_reader = DefineXMLReader.from_filename(path_to_define)
+    path_to_define = os.path.join(path_to_data, DEFINE_XML_FILE_NAME)
+    define_xml_reader = DefineXMLReaderFactory.from_filename(path_to_define)
     return define_xml_reader.get_define_version()
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/rule_processor.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/rule_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,46 +221,50 @@
         if not operations:
             # stop function execution if no operations have been provided
             return dataset
 
         dataset_copy = dataset.copy()
         for operation in operations:
             # change -- pattern to domain name
-            target: str = operation.get("name")
+            original_target: str = operation.get("name")
+            target: str = original_target
             domain: str = operation.get("domain", domain)
             if target and target.startswith("--") and domain:
                 # Not a study wide operation
                 target = target.replace("--", domain)
                 domain = domain.replace("--", domain)
 
             # get necessary operation
             operation_params = OperationParams(
                 operation_id=operation.get("id"),
                 operation_name=operation.get("operator"),
                 dataframe=dataset_copy,
                 target=target,
+                original_target=original_target,
                 domain=domain,
                 dataset_path=dataset_path,
                 directory_path=get_directory_path(dataset_path),
                 datasets=datasets,
                 grouping=operation.get("group", []),
                 standard=standard,
                 standard_version=standard_version,
                 meddra_path=kwargs.get("meddra_path"),
                 whodrug_path=kwargs.get("whodrug_path"),
+                attribute_name=operation.get("attribute_name", ""),
+                key_name=operation.get("key_name", ""),
+                key_value=operation.get("key_value", ""),
             )
 
             # execute operation
             dataset_copy = self._execute_operation(operation_params, dataset_copy)
 
             logger.info(
                 f"Processed rule operation. "
                 f"operation={operation_params.operation_name}, rule={rule}"
             )
-
         return dataset_copy
 
     def _execute_operation(
         self, operation_params: OperationParams, dataset: pd.DataFrame
     ):
         """
         Internal method that executes the given operation.
@@ -393,15 +397,15 @@
             f"Added comparator to rule conditions. "
             f"comparator={comparator}, conditions={rule['conditions']}"
         )
 
     @staticmethod
     def duplicate_conditions_for_all_targets(
         conditions: ConditionInterface, targets: List[str]
-    ) -> ConditionInterface:
+    ) -> dict:
         """
         Given a list of conditions duplicates the condition for all targets as necessary
         """
         conditions_dict = conditions.get_conditions()
         new_conditions_dict = {}
         for key, conditions_list in conditions_dict.items():
             new_conditions_list = []
@@ -409,16 +413,15 @@
                 if condition.should_copy():
                     new_conditions_list.extend(
                         [condition.copy().set_target(target) for target in targets]
                     )
                 else:
                     new_conditions_list.append(condition)
             new_conditions_dict[key] = new_conditions_list
-        conditions.set_conditions(new_conditions_dict)
-        return conditions
+        return new_conditions_dict
 
     def is_suitable_for_validation(
         self,
         rule: dict,
         dataset_domain: str,
         file_path: str,
         is_split_domain: bool,
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/utils.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine/utilities/validation_output_container.py` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine/utilities/validation_output_container.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine.egg-info/PKG-INFO` & `cdisc-rules-engine-0.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,21 @@
-Metadata-Version: 2.1
-Name: cdisc-rules-engine
-Version: 0.6.1
-Summary: Open source offering of the cdisc rules engine
-Home-page: https://github.com/cdisc-org/cdisc-rules-engine
-Author: cdisc-org
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ### Supported python versions
+
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-orange.svg)](https://www.python.org/downloads/release/python-380)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-green.svg)](https://www.python.org/downloads/release/python-390)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-310)
+
 # cdisc-rules-engine
+
 Open source offering of the cdisc rules engine
 
 ### Quick start
 
-To quickly get up and running with CORE, users can download the latest executable version of the engine for their operating system from here: https://github.com/cdisc-org/cdisc-rules-engine/releases
+To quickly get up and running with CORE, users can download the latest executable version of the engine for their operating system from here: <https://github.com/cdisc-org/cdisc-rules-engine/releases>
 
 Once downloaded, simply unzip the file and run the following command based on your Operating System:
 
 Windows:
 
 ```
 .\core.exe validate -s <standard> -v <standard_version> -d path/to/datasets
@@ -34,52 +26,58 @@
 Linux/Mac:
 
 ```
 ./core validate -s <standard> -v <standard_version> -d path/to/datasets
 
 # ex: ./core validate -s sdtmig -v 3-4 -d .\xpt\
 ```
+
 ### Code formatter
-This project uses the `black` code formatter and `flake8` linter for python.
-It also uses `pre-commit` to run `black` and `flake8` when you commit.
-Both dependencies are added to *requirements.txt*.
+
+This project uses the `black` code formatter, `flake8` linter for python and `prettier` for JSON, YAML and MD.
+It also uses `pre-commit` to run `black`, `flake8` and `prettier` when you commit.
+Both dependencies are added to _requirements.txt_.
 
 **Required**
 
 Setting up `pre-commit` requires one extra step. After installing it you have to run
 
 `pre-commit install`
 
 This installs `pre-commit` in your `.git/hooks` directory.
 
-### Installing dependencies.
+### Installing dependencies
+
 These steps should be run before running any tests or core commands using the non compiled version.
 
-* Create a virtual environment:
-`python -m venv <virtual_environment_name>`
-* Activate the virtual environment:
+- Create a virtual environment:
+  `python -m venv <virtual_environment_name>`
+- Activate the virtual environment:
 
 `./<virtual_environment_name>/bin/activate` -- on linux/mac </br>
 `.\<virtual_environment_name>\Scripts\Activate` -- on windows
 
-* Install the requirements.
+- Install the requirements.
 
 `python -m pip install -r requirements.txt` # From the root directory
 
 ### Running The Tests
+
 From the root of the project run the following command:
 
 `python -m pytest tests/unit/`
+
 ### Running a validation
 
 #### From the command line
 
 Clone the repository and run `python core.py --help` to see the full list of commands.
 
 Run `python core.py validate --help` to see the list of validation options.
+
 ```
   -ca, --cache TEXT               Relative path to cache files containing pre
                                   loaded metadata and rules
   -ps, --pool-size INTEGER         Number of parallel processes for validation
   -d, --data TEXT                 Path to directory containing data files
   -dp, --dataset-path TEXT        Absolute path to dataset file. Can be specified multiple times.
   -l, --log-level [info|debug|error|critical|disabled|warn]
@@ -114,55 +112,58 @@
                                   "[████████████████████████████--------]
                                   78%"is printed.
   --help                          Show this message and exit.
 ```
 
 ##### Available log levels
 
-* `debug` - Display all logs
-* `info` - Display info, warnings, and error logs
-* `warn` - Display warnings and errors
-* `error` - Display only error logs
-* `critical` - Display critical logs
+- `debug` - Display all logs
+- `info` - Display info, warnings, and error logs
+- `warn` - Display warnings and errors
+- `error` - Display only error logs
+- `critical` - Display critical logs
 
 ##### Validate folder
+
 To validate a folder using rules for SDTM-IG version 3.4 use the following command:
 
 `python core.py validate -s sdtmig -v 3-4 -d path/to/datasets`
 
 ##### Understanding the Rules Report
+
 The rules report tab displays the run status of each rule selected for validation
 
 The possible rule run statuses are:
 
-* `SUCCESS` - The rule ran and data was validated against the rule. May or may not produce results
-* `SKIPPED` - The rule was unable to be run. Usually due to missing required data, but could also be cause by rule execution errors.
+- `SUCCESS` - The rule ran and data was validated against the rule. May or may not produce results
+- `SKIPPED` - The rule was unable to be run. Usually due to missing required data, but could also be cause by rule execution errors.
 
 ##### Additional Core Commands
 
-* update-cache - update locally stored cache data (Requires an environment variable - `CDISC_LIBRARY_API_KEY`)
+- update-cache - update locally stored cache data (Requires an environment variable - `CDISC_LIBRARY_API_KEY`)
+
+  `python core.py update-cache`
 
-    `python core.py update-cache`
-    
-    To obtain an api key, please follow the instructions found here: https://wiki.cdisc.org/display/LIBSUPRT/Getting+Started%3A+Access+to+CDISC+Library+API+using+API+Key+Authentication. Please note it can take up to an hour after sign up to have an api key issued
+  To obtain an api key, please follow the instructions found here: <https://wiki.cdisc.org/display/LIBSUPRT/Getting+Started%3A+Access+to+CDISC+Library+API+using+API+Key+Authentication>. Please note it can take up to an hour after sign up to have an api key issued
 
-* list-rules - list rules available in the cache
+- list-rules - list rules available in the cache
 
-    * list all rules:
+  - list all rules:
 
     `python core.py list-rules`
 
-    * list rules for standard:
+  - list rules for standard:
 
     `python core.py list-rules -s sdtmig -v 3-4`
 
-* list-rule-sets - lists all standards and versions for which rules are available:
-    `python core.py list-rule-sets`
+- list-rule-sets - lists all standards and versions for which rules are available:
+  `python core.py list-rule-sets`
+
+- test - Test authored rule given dataset in json format
 
-* test - Test authored rule given dataset in json format
 ```
   -ca, --cache TEXT               Relative path to cache files containing pre
                                   loaded metadata and rules
   -dp, --dataset-path TEXT        Absolute path to dataset file
   -s, --standard TEXT             CDISC standard to validate against
                                   [required]
   -v, --version TEXT              Standard version to validate against
@@ -176,15 +177,15 @@
   --meddra TEXT                   Path to directory with MedDRA dictionary
                                   files
   -r, --rule TEXT                 Path to rule json file.
   --help                          Show this message and exit.
 ```
 
 EX: `python core.py test -s sdtmig -v 3-4 -dp <path to dataset json file> -r <path to rule json file> --meddra ./meddra/ --whodrug ./whodrug/`
-Note: JSON dataset should match the format provided by the rule editor: 
+Note: JSON dataset should match the format provided by the rule editor:
 
 ```
 {
     "datasets": [{
       "filename": "cm.xpt",
       "label": "Concomitant/Concurrent medications",
       "domain": "CM",
@@ -205,14 +206,29 @@
         ],
       }
     }
   ]
 }
 ```
 
+- list-ct - list ct packages available in the cache
+
+```
+Usage: python core.py list-ct [OPTIONS]
+
+  Command to list the ct packages available in the cache.
+
+Options:
+  -c, --cache_path TEXT  Relative path to cache files containing pre loaded
+                         metadata and rules
+  -s, --subsets TEXT     CT package subset type. Ex: sdtmct. Multiple values
+                         allowed
+  --help                 Show this message and exit.
+```
+
 #### PyPI Quickstart: Validate data within python
 
 An alternative to running the validation from the command line is to instead import the rules engine library in python and run rules against data directly (without needing your data to be in `.xpt` format).
 
 ##### Step 0: Install the library
 
 ```
@@ -231,15 +247,15 @@
 
 from multiprocessing.managers import SyncManager
 from cdisc_rules_engine.services.cache import InMemoryCacheService
 
 class CacheManager(SyncManager):
     pass
 
-# If you're working from a terminal you may need to 
+# If you're working from a terminal you may need to
 # use SyncManager directly rather than define CacheManager
 CacheManager.register("InMemoryCacheService", InMemoryCacheService)
 
 
 def load_rules_cache(path_to_rules_cache):
   cache_path = pathlib.Path(path_to_rules_cache)
   manager = CacheManager()
@@ -247,15 +263,15 @@
   cache = manager.InMemoryCacheService()
 
   files = next(os.walk(cache_path), (None, None, []))[2]
 
   for fname in files:
       with open(cache_path / fname, "rb") as f:
           cache.add_all(pickle.load(f))
-  
+
   return cache
 ```
 
 Rules in this cache can be accessed by standard and version using the `get_rules_cache_key` function.
 
 ```python
 from cdisc_rules_engine.utilities.utils import get_rules_cache_key
@@ -264,31 +280,31 @@
 # Note that the standard version is separated by a dash, not a period
 cache_key_prefix = get_rules_cache_key("sdtmig", "3-4")
 rules = cache.get_all_by_prefix(cache_key_prefix)
 ```
 
 `rules` will now be a list of dictionaries the following keys
 
- - `core_id`
-   - e.g. "CORE-000252"
- - `domains`
-   - e.g. `{'Include': ['DM'], 'Exclude': []}` or `{'Include': ['ALL']}`
- - `author`
- - `reference`
- - `sensitivity`
- - `executability`
- - `description`
- - `authorities`
- - `standards`
- - `classes`
- - `rule_type`
- - `conditions`
- - `actions`
- - `datasets`
- - `output_variables`
+- `core_id`
+  - e.g. "CORE-000252"
+- `domains`
+  - e.g. `{'Include': ['DM'], 'Exclude': []}` or `{'Include': ['ALL']}`
+- `author`
+- `reference`
+- `sensitivity`
+- `executability`
+- `description`
+- `authorities`
+- `standards`
+- `classes`
+- `rule_type`
+- `conditions`
+- `actions`
+- `datasets`
+- `output_variables`
 
 ##### Step 2: Prepare your data
 
 In order to pass your data through the rules engine, it must be a pandas dataframe of an SDTM dataset. For example:
 
 ```
 >>> data
@@ -310,15 +326,15 @@
 
 Next, we need to actually run the rules. We can select which rules we want to run based on the domain of the data we're checking and the `"Include"` and `"Exclude"` domains of the rule.
 
 ```python
 # Get the rules for the domain AE
 # (Note: we're ignoring ALL domain rules here)
 ae_rules = [
-  rule for rule in rules 
+  rule for rule in rules
   if "AE" in rule["domains"].get("Include", [])
 ]
 ```
 
 There's one last thing we need before we can actually run the rule, and that's a `COREActions` object. This object will handle generating error messages should the rule fail.
 
 To instantiate a `COREActions` object, we need to pass in the following:
@@ -352,14 +368,15 @@
   defined_actions=core_actions,
 )
 ```
 
 ##### Step 5: Interpret the results
 
 The return value of run will tell us if the rule was triggered.
+
 - A `False` value means that there were no errors
 - A `True` value means that there were errors
 
 If there were errors, they will have been appended to the results array passed into your `COREActions` instance. Here's an example error:
 
 ```python
 {
```

### Comparing `cdisc-rules-engine-0.6.1/cdisc_rules_engine.egg-info/SOURCES.txt` & `cdisc-rules-engine-0.6.2/cdisc_rules_engine.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,27 +23,29 @@
 cdisc_rules_engine/constants/patterns.py
 cdisc_rules_engine/constants/permissibility.py
 cdisc_rules_engine/constants/rule_constants.py
 cdisc_rules_engine/dataset_builders/__init__.py
 cdisc_rules_engine/dataset_builders/base_dataset_builder.py
 cdisc_rules_engine/dataset_builders/content_metadata_dataset_builder.py
 cdisc_rules_engine/dataset_builders/contents_dataset_builder.py
+cdisc_rules_engine/dataset_builders/contents_define_variables_dataset_builder.py
+cdisc_rules_engine/dataset_builders/contents_define_vlm_dataset_builder.py
 cdisc_rules_engine/dataset_builders/dataset_builder_factory.py
 cdisc_rules_engine/dataset_builders/define_item_group_dataset_builder.py
 cdisc_rules_engine/dataset_builders/define_variables_dataset_builder.py
 cdisc_rules_engine/dataset_builders/domain_list_dataset_builder.py
+cdisc_rules_engine/dataset_builders/values_dataset_builder.py
 cdisc_rules_engine/dataset_builders/variables_metadata_dataset_builder.py
 cdisc_rules_engine/dataset_builders/variables_metadata_with_define_dataset_builder.py
 cdisc_rules_engine/dummy_models/__init__.py
 cdisc_rules_engine/dummy_models/dummy_dataset.py
 cdisc_rules_engine/dummy_models/dummy_variable.py
 cdisc_rules_engine/enums/__init__.py
 cdisc_rules_engine/enums/base_enum.py
 cdisc_rules_engine/enums/default_file_paths.py
-cdisc_rules_engine/enums/define_xml_versions.py
 cdisc_rules_engine/enums/execution_status.py
 cdisc_rules_engine/enums/library_endpoints.py
 cdisc_rules_engine/enums/optional_condition_parameters.py
 cdisc_rules_engine/enums/progress_parameter_options.py
 cdisc_rules_engine/enums/report_types.py
 cdisc_rules_engine/enums/rule_types.py
 cdisc_rules_engine/enums/sensitivity.py
@@ -105,40 +107,45 @@
 cdisc_rules_engine/models/rule_conditions/condition_composite_factory.py
 cdisc_rules_engine/models/rule_conditions/not_condition_composite.py
 cdisc_rules_engine/models/rule_conditions/single_condition.py
 cdisc_rules_engine/operations/__init__.py
 cdisc_rules_engine/operations/base_operation.py
 cdisc_rules_engine/operations/dataset_column_order.py
 cdisc_rules_engine/operations/day_data_validator.py
+cdisc_rules_engine/operations/define_variable_metadata.py
 cdisc_rules_engine/operations/distinct.py
+cdisc_rules_engine/operations/domain_is_custom.py
 cdisc_rules_engine/operations/domain_label.py
 cdisc_rules_engine/operations/expected_variables.py
 cdisc_rules_engine/operations/extract_metadata.py
+cdisc_rules_engine/operations/get_model_filtered_variables.py
+cdisc_rules_engine/operations/label_referenced_variable_metadata.py
 cdisc_rules_engine/operations/library_column_order.py
 cdisc_rules_engine/operations/library_model_column_order.py
 cdisc_rules_engine/operations/max_date.py
 cdisc_rules_engine/operations/maximum.py
 cdisc_rules_engine/operations/mean.py
 cdisc_rules_engine/operations/meddra_code_references_validator.py
 cdisc_rules_engine/operations/meddra_code_term_pairs_validator.py
 cdisc_rules_engine/operations/meddra_term_references_validator.py
 cdisc_rules_engine/operations/min_date.py
 cdisc_rules_engine/operations/minimum.py
+cdisc_rules_engine/operations/name_referenced_variable_metadata.py
 cdisc_rules_engine/operations/operations_factory.py
 cdisc_rules_engine/operations/parent_library_model_column_order.py
 cdisc_rules_engine/operations/permissible_variables.py
 cdisc_rules_engine/operations/record_count.py
 cdisc_rules_engine/operations/required_variables.py
 cdisc_rules_engine/operations/study_domains.py
 cdisc_rules_engine/operations/valid_codelist_dates.py
 cdisc_rules_engine/operations/variable_count.py
 cdisc_rules_engine/operations/variable_exists.py
 cdisc_rules_engine/operations/variable_is_null.py
+cdisc_rules_engine/operations/variable_library_metadata.py
 cdisc_rules_engine/operations/variable_names.py
-cdisc_rules_engine/operations/variable_permissibility.py
 cdisc_rules_engine/operations/variable_value_count.py
 cdisc_rules_engine/operations/whodrug_hierarchy_validator.py
 cdisc_rules_engine/operations/whodrug_references_validator.py
 cdisc_rules_engine/serializers/__init__.py
 cdisc_rules_engine/serializers/base_serializer.py
 cdisc_rules_engine/serializers/dataset_metadata_serializer.py
 cdisc_rules_engine/serializers/rule_serializer.py
@@ -148,15 +155,14 @@
 cdisc_rules_engine/serializers/term_serializers/base_whodrug_term_serializer.py
 cdisc_rules_engine/serializers/term_serializers/drug_dictionary_serializer.py
 cdisc_rules_engine/serializers/term_serializers/meddra_term_serializer.py
 cdisc_rules_engine/services/__init__.py
 cdisc_rules_engine/services/adam_variable_reader.py
 cdisc_rules_engine/services/cdisc_library_service.py
 cdisc_rules_engine/services/dataset_metadata_reader.py
-cdisc_rules_engine/services/define_xml_reader.py
 cdisc_rules_engine/services/cache/__init__.py
 cdisc_rules_engine/services/cache/cache_populator_service.py
 cdisc_rules_engine/services/cache/cache_service_factory.py
 cdisc_rules_engine/services/cache/in_memory_cache_service.py
 cdisc_rules_engine/services/cache/redis_cache_service.py
 cdisc_rules_engine/services/data_readers/__init__.py
 cdisc_rules_engine/services/data_readers/data_reader_factory.py
```

### Comparing `cdisc-rules-engine-0.6.1/setup.py` & `cdisc-rules-engine-0.6.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     url="https://github.com/cdisc-org/cdisc-rules-engine",
     packages=setuptools.find_packages(exclude=["scripts", "tests"]),
     license="MIT",
     include_package_data=True,
     python_requires=">=3.8",
     install_requires=[
         "pandas>=1.3.5",
-        "business-rules-enhanced==1.3.4",
+        "business-rules-enhanced==1.3.6",
         "python-dotenv==0.20.0",
         "cdisc-library-client==0.1.4",
         "odmlib==0.1.4",
         "xport==3.6.1",
         "redis==4.0.2",
         "openpyxl==3.0.10",
         "importlib-metadata==5.0.0",
```

