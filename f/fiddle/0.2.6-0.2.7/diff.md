# Comparing `tmp/fiddle-0.2.6.tar.gz` & `tmp/fiddle-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddle-0.2.6.tar", last modified: Fri Mar 31 01:02:45 2023, max compression
+gzip compressed data, was "fiddle-0.2.7.tar", last modified: Fri Jun 30 20:02:14 2023, max compression
```

## Comparing `fiddle-0.2.6.tar` & `fiddle-0.2.7.tar`

### file list

```diff
@@ -1,204 +1,218 @@
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.862523 fiddle-0.2.6/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11357 2022-02-19 00:33:27.000000 fiddle-0.2.6/LICENSE
--rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-03-31 01:02:45.862523 fiddle-0.2.6/PKG-INFO
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      603 2023-03-31 01:01:33.000000 fiddle-0.2.6/README.md
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.846523 fiddle-0.2.6/fiddle/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1610 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.850523 fiddle-0.2.6/fiddle/_src/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.850523 fiddle-0.2.6/fiddle/_src/absl_flags/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      907 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/absl_flags/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    18876 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/absl_flags/flags.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1021 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/absl_flags/sample_module_for_flags_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16567 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/arg_factory.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15484 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/arg_factory_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5026 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/building.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.850523 fiddle-0.2.6/fiddle/_src/codegen/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.854523 fiddle-0.2.6/fiddle/_src/codegen/auto_config/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6529 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/code_ir.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2212 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/code_ir_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5271 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/complex_to_variables.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4327 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/complex_to_variables_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3124 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/experimental_top_level_api.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3794 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1626 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/init_task.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1181 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/init_task_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4582 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/ir_printer.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3223 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/ir_printer_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5474 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/ir_to_cst.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3028 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/ir_to_cst_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5682 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/make_symbolic_references.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5919 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6114 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/naming.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8402 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/naming_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4183 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/parents_first_traversal.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2322 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4225 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/shared_to_variables.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3292 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/shared_to_variables_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2047 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/split_arg_factories.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2335 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/split_arg_factories_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4540 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/auto_config/test_fixtures.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11220 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/codegen.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    17067 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/codegen_diff.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9050 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/codegen_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1930 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/formatting_utilities.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8776 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/import_manager.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5074 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/import_manager_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4206 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/mini_ast.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3471 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/namespace.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2204 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/namespace_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15665 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/py_val_to_cst_converter.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5918 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/py_val_to_cst_converter_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3500 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/special_value_codegen.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.854523 fiddle-0.2.6/fiddle/_src/codegen/test_submodule/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/test_submodule/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      810 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/test_submodule/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/codegen/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    47424 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    53285 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    25253 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/daglish.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    18772 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/daglish_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    41201 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/diffing.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    46194 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/diffing_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.858523 fiddle-0.2.6/fiddle/_src/experimental/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    36699 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/auto_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5694 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/auto_config_policy.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    36582 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/auto_config_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.858523 fiddle-0.2.6/fiddle/_src/experimental/autobuilders/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/autobuilders/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11256 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/autobuilders/autobuilders.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6512 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/autobuilders/autobuilders_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      922 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3585 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/configurator.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12374 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/daglish_legacy.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16195 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/daglish_legacy_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4811 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/dataclasses.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12383 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/dataclasses_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1173 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/dict_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2706 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/dict_config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2069 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/fixture_node.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2970 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/fixture_node_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1264 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/namespace_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2678 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/namespace_config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    30108 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/serialization.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2705 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/tied_value.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4556 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/tied_value_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3228 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/transform.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4743 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/transform_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9174 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/visualize.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3089 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/yaml_serialization.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5119 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/experimental/yaml_serialization_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.858523 fiddle-0.2.6/fiddle/_src/extensions/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/extensions/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1324 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/extensions/flax_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4476 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/extensions/jax.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1408 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/extensions/seqio.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1465 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/extensions/seqio_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3433 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/extensions/tf.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4569 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/extensions/tf_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1633 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/field_metadata.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    36961 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/graphviz.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8910 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/history.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5216 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/history_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2380 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/materialize.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1760 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/materialize_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3111 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/module_reflection.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2768 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/module_reflection_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1420 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/module_reflection_test_module.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1795 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/mutate_buildable.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1615 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/mutate_buildable_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12318 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/printing.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14967 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/printing_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2879 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/reraised_exception.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2235 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/reraised_exception_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9305 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/selectors.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11178 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/selectors_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3757 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/signatures.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6539 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/signatures_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1011 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/signatures_test_helper.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4267 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/tag_type.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8360 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/tagging.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    13335 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/tagging_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1275 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/tagging_test_module.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.858523 fiddle-0.2.6/fiddle/_src/testing/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/testing/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5543 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/testing/autotest.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.858523 fiddle-0.2.6/fiddle/_src/testing/example/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/testing/example/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      925 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/testing/example/demo_configs.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2460 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/testing/example/fake_encoder_decoder.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1235 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/testing/example/person_friend_toy.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5419 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/testing/nested_values.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3155 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/testing/nested_values_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9369 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/testing/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9185 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/_src/testing/test_util_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.858523 fiddle-0.2.6/fiddle/absl_flags/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      907 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/absl_flags/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.858523 fiddle-0.2.6/fiddle/absl_flags/example/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/absl_flags/example/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1342 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/absl_flags/example/business_logic.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3453 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/absl_flags/example/configs.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1446 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/absl_flags/example/example.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      906 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/absl_flags/example/tags.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3528 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/arg_factory.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      792 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/building.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.862523 fiddle-0.2.6/fiddle/codegen/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/codegen/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.862523 fiddle-0.2.6/fiddle/codegen/auto_config/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/codegen/auto_config/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      852 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/codegen/auto_config/experimental_top_level_api.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      933 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/codegen/codegen.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/codegen/codegen_diff.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1296 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/codegen/py_val_to_cst_converter.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1052 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1002 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1951 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/daglish.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1705 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/diffing.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.862523 fiddle-0.2.6/fiddle/examples/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/examples/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.862523 fiddle-0.2.6/fiddle/examples/colabs/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/examples/colabs/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.862523 fiddle-0.2.6/fiddle/experimental/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1601 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/auto_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1236 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/auto_config_policy.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.862523 fiddle-0.2.6/fiddle/experimental/autobuilders/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/autobuilders/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1025 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/configurator.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1367 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/dataclasses.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/dict_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1059 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/fixture_node.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      781 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/namespace_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1910 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/serialization.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      894 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/tied_value.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      860 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/transform.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1327 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/visualize.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1043 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/experimental/yaml_serialization.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.862523 fiddle-0.2.6/fiddle/extensions/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/extensions/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      824 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/extensions/jax.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      868 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/extensions/seqio.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      840 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/extensions/tf.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      914 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/graphviz.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1139 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/history.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      812 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/printing.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1049 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/selectors.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/signatures.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      847 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/tag_type.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2682 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/tagging.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.862523 fiddle-0.2.6/fiddle/testing/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/testing/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1300 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/testing/autotest.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      762 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/testing/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      676 2023-03-31 01:01:34.000000 fiddle-0.2.6/fiddle/version.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-03-31 01:02:45.846523 fiddle-0.2.6/fiddle.egg-info/
--rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-03-31 01:02:45.000000 fiddle-0.2.6/fiddle.egg-info/PKG-INFO
--rw-r-----   0 dhr      (201437) primarygroup (89939)     6559 2023-03-31 01:02:45.000000 fiddle-0.2.6/fiddle.egg-info/SOURCES.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)        1 2023-03-31 01:02:45.000000 fiddle-0.2.6/fiddle.egg-info/dependency_links.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)      151 2023-03-31 01:02:45.000000 fiddle-0.2.6/fiddle.egg-info/requires.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)        7 2023-03-31 01:02:45.000000 fiddle-0.2.6/fiddle.egg-info/top_level.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)       38 2023-03-31 01:02:45.862523 fiddle-0.2.6/setup.cfg
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3554 2023-03-31 01:01:34.000000 fiddle-0.2.6/setup.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.370883 fiddle-0.2.7/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11357 2022-02-19 00:33:27.000000 fiddle-0.2.7/LICENSE
+-rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-06-30 20:02:14.370883 fiddle-0.2.7/PKG-INFO
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      603 2023-06-30 20:02:00.000000 fiddle-0.2.7/README.md
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.350883 fiddle-0.2.7/fiddle/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1610 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.354883 fiddle-0.2.7/fiddle/_src/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.354883 fiddle-0.2.7/fiddle/_src/absl_flags/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      907 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/absl_flags/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    21439 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/absl_flags/flags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1021 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/absl_flags/sample_module_for_flags_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16567 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/arg_factory.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15484 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/arg_factory_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5939 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/building.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2483 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/building_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.358883 fiddle-0.2.7/fiddle/_src/codegen/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.362883 fiddle-0.2.7/fiddle/_src/codegen/auto_config/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6997 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/code_ir.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2212 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/code_ir_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5371 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/complex_to_variables.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4327 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/complex_to_variables_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8540 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/experimental_top_level_api.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9800 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2445 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/get_history_comments.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2187 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/get_history_comments_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1605 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/init_task.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1181 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/init_task_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4499 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_printer.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2940 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_printer_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7694 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_to_cst.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5162 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_to_cst_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7708 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/make_symbolic_references.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6819 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6743 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/naming.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8402 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/naming_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4183 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/parents_first_traversal.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2322 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4052 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/shared_to_variables.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3586 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/shared_to_variables_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2047 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/split_arg_factories.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2335 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/split_arg_factories_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11018 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/sub_fixture.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3467 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/sub_fixture_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5499 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/test_fixtures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    17067 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/codegen_diff.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1951 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/formatting_utilities.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8776 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/import_manager.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5074 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/import_manager_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11220 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/legacy_codegen.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9134 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/legacy_codegen_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4206 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/mini_ast.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3471 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/namespace.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2204 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/namespace_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5207 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/new_codegen.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3653 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/new_codegen_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4057 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/newcg_symbolic_references.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5783 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/newcg_symbolic_references_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15928 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/py_val_to_cst_converter.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6189 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/py_val_to_cst_converter_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3500 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/special_value_codegen.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.362883 fiddle-0.2.7/fiddle/_src/codegen/test_submodule/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/test_submodule/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      810 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/test_submodule/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    49485 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    52963 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    26463 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/daglish.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5349 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/daglish_extensions.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3241 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/daglish_extensions_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    20078 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/daglish_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    41201 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/diffing.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    45929 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/diffing_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.362883 fiddle-0.2.7/fiddle/_src/experimental/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    42932 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/auto_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5668 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/auto_config_policy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    43562 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/auto_config_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.362883 fiddle-0.2.7/fiddle/_src/experimental/autobuilders/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/autobuilders/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11256 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/autobuilders/autobuilders.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6512 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/autobuilders/autobuilders_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      922 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3585 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/configurator.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12374 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/daglish_legacy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16195 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/daglish_legacy_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7228 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/dataclasses.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14396 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/dataclasses_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1173 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/dict_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2706 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/dict_config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2069 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/fixture_node.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2970 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/fixture_node_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1264 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/namespace_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2678 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/namespace_config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    30108 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/serialization.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2767 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/tied_value.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6335 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/tied_value_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3228 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/transform.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4743 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/transform_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11539 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/visualize.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2338 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/with_tags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2169 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/with_tags_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3089 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/yaml_serialization.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5119 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/yaml_serialization_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/_src/extensions/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1324 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/flax_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5458 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/jax.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1408 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/seqio.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1479 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/seqio_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3433 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/tf.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4583 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/tf_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1633 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/field_metadata.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    36979 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/graphviz.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2133 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/graphviz_custom_object.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9437 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/history.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5216 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/history_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2380 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/materialize.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1760 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/materialize_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3111 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/module_reflection.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2768 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/module_reflection_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1420 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/module_reflection_test_module.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1795 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/mutate_buildable.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1615 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/mutate_buildable_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12318 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/printing.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14648 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/printing_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2879 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/reraised_exception.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2235 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/reraised_exception_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9305 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/selectors.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11178 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/selectors_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4274 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/signatures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6539 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/signatures_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1011 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/signatures_test_helper.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4267 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/tag_type.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7368 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/tagging.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14083 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/tagging_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1275 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/tagging_test_module.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/_src/testing/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5543 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/autotest.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/_src/testing/example/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/example/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      925 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/example/demo_configs.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2533 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/example/fake_encoder_decoder.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1235 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/example/person_friend_toy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5419 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/nested_values.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3155 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/nested_values_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9562 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9805 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/test_util_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/absl_flags/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      967 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/absl_flags/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/absl_flags/example/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/absl_flags/example/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1342 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/absl_flags/example/business_logic.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3451 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/absl_flags/example/configs.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1444 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/absl_flags/example/example.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      906 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/absl_flags/example/tags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3528 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/arg_factory.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      792 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/building.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/codegen/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/codegen/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/codegen/auto_config/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/codegen/auto_config/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1828 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/codegen/auto_config/experimental_top_level_api.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      961 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/codegen/codegen.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/codegen/codegen_diff.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1296 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/codegen/py_val_to_cst_converter.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1052 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1002 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2119 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/daglish.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1705 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/diffing.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/examples/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/examples/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/examples/colabs/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/examples/colabs/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/experimental/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1658 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/auto_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1210 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/auto_config_policy.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/experimental/autobuilders/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/autobuilders/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1025 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/configurator.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1523 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/dataclasses.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/dict_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1059 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/fixture_node.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      781 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/namespace_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1910 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/serialization.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      901 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/tied_value.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      860 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/transform.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1327 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/visualize.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1043 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/yaml_serialization.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.370883 fiddle-0.2.7/fiddle/extensions/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/extensions/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      824 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/extensions/jax.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      868 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/extensions/seqio.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      840 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/extensions/tf.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      942 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/graphviz.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1184 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/history.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      812 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/printing.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1049 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/selectors.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/signatures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      847 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/tag_type.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2682 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/tagging.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.370883 fiddle-0.2.7/fiddle/testing/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/testing/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1300 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/testing/autotest.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      762 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/testing/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      676 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/version.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.350883 fiddle-0.2.7/fiddle.egg-info/
+-rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-06-30 20:02:14.000000 fiddle-0.2.7/fiddle.egg-info/PKG-INFO
+-rw-r-----   0 dhr      (201437) primarygroup (89939)     7188 2023-06-30 20:02:14.000000 fiddle-0.2.7/fiddle.egg-info/SOURCES.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)        1 2023-06-30 20:02:14.000000 fiddle-0.2.7/fiddle.egg-info/dependency_links.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)      151 2023-06-30 20:02:14.000000 fiddle-0.2.7/fiddle.egg-info/requires.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)        7 2023-06-30 20:02:14.000000 fiddle-0.2.7/fiddle.egg-info/top_level.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)       38 2023-06-30 20:02:14.370883 fiddle-0.2.7/setup.cfg
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3554 2023-06-30 20:02:01.000000 fiddle-0.2.7/setup.py
```

### Comparing `fiddle-0.2.6/LICENSE` & `fiddle-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/PKG-INFO` & `fiddle-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddle
-Version: 0.2.6
+Version: 0.2.7
 Summary: Fiddle: A Python-first configuration library
 Home-page: https://github.com/google/fiddle
 Author: The Fiddle Team
 Author-email: noreply@google.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/google/fiddle/docs
 Project-URL: Bug Reports, https://github.com/google/fiddle/issues
```

### Comparing `fiddle-0.2.6/README.md` & `fiddle-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/__init__.py` & `fiddle-0.2.7/fiddle/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/__init__.py` & `fiddle-0.2.7/fiddle/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/absl_flags/__init__.py` & `fiddle-0.2.7/fiddle/_src/absl_flags/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/absl_flags/flags.py` & `fiddle-0.2.7/fiddle/_src/absl_flags/flags.py`

 * *Files 13% similar despite different names*

```diff
@@ -113,38 +113,43 @@
 import enum
 import importlib
 import inspect
 import re
 import sys
 import textwrap
 import typing
-from typing import Any, List, Optional, Sequence, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple
 
 from absl import app
 from absl import flags
 from absl import logging
 from etils import epath
 from fiddle import printing
 from fiddle import selectors
 from fiddle._src import config
+from fiddle._src import daglish
+from fiddle._src import daglish_extensions
 from fiddle._src import module_reflection
 from fiddle._src import tagging
 from fiddle._src.experimental import auto_config
 from fiddle._src.experimental import serialization
 
 
 _FDL_CONFIG = flags.DEFINE_string(
     'fdl_config',
     default=None,
     help='The name of a function to construct a base Fiddle config.')
 _FDL_CONFIG_FILE = epath.DEFINE_path(
     'fdl_config_file',
     default=None,
-    help='The path to a file containing a serialized base Fiddle config in '
-    'JSON format.')
+    help=(
+        'The path to a file containing a serialized base Fiddle config in '
+        'JSON format. '
+    ),
+)
 _FIDDLER = flags.DEFINE_multi_string(
     'fiddler',
     default=[],
     help='The name of a fiddler. Fiddlers are functions that modify a config.')
 _FDL_SET = flags.DEFINE_multi_string(
     'fdl_set',
     default=[],
@@ -158,69 +163,24 @@
 _FDL_HELP = flags.DEFINE_bool(
     'fdl_help',
     default=False,
     help='Print out Fiddle-specific help (including '
     'information on any loaded configuration) and exit.')
 
 
-@dataclasses.dataclass
-class _IndexKey:
-  """Wraps a string or integer index into a dictionary or list/tuple."""
-  key: Union[str, int]
-
-  def __post_init__(self):
-    try:
-      self.key = ast.literal_eval(self.key)
-    except Exception:  # pylint: disable=broad-except
-      pass  # leave self as-is.
-
-  def __call__(self, obj):
-    return obj[self.key]
-
-  def update(self, obj, new_value):
-    """Updates `obj`'s `self.key` to `new_value`."""
-    obj[self.key] = new_value
-
-
-@dataclasses.dataclass
-class _AttributeKey:
-  """Wraps the name of an attribute."""
-  __slots__ = ('name',)
-  name: str
-
-  def __call__(self, obj):
-    return getattr(obj, self.name)
-
-  def update(self, obj, new_value):
-    setattr(obj, self.name, new_value)
-
-
-_PATH_COMPONENT_REGEX = re.compile(r'(?:\.([A-Za-z_][^\.\[]*))|\[([^]]+)\]')
-
-
 def _print_stderr(*args, **kwargs):
   print(*args, **kwargs, file=sys.stderr)
 
 
-def _parse_path(path: str) -> List[Union[_AttributeKey, _IndexKey]]:
+def _parse_path(path: str) -> daglish.Path:
   """Parses a path into a list of either attributes or index lookups."""
-  path = f'.{path}'  # Add a leading `.` to make parsing work properly.
-  result = []
-  curr_index = 0
-  while curr_index < len(path):
-    match = _PATH_COMPONENT_REGEX.match(path, curr_index)
-    if match is None:
-      raise ValueError(
-          f'Could not parse {path[1:]!r} (failed index: {curr_index - 1}).')
-    curr_index = match.end(0)  # Advance
-    if match[1] is not None:
-      result.append(_AttributeKey(match[1]))
-    else:
-      result.append(_IndexKey(match[2]))
-  return result
+  if not path.startswith('[') and not path.startswith('.'):
+    path = f'.{path}'  # Add a leading `.` to make parsing work properly.
+
+  return daglish_extensions.parse_path(path)
 
 
 class _ImportDottedNameDebugContext(enum.Enum):
   """Context of importing a sumbol, for error messages."""
 
   BASE_CONFIG = 1
   FIDDLER = 2
@@ -300,29 +260,116 @@
         f'Could not parse literal value "{value}" while trying to set '
         f'"{path}". Does a string need to be quoted? For example, you might '
         f"want to pass --fdl_set={path}='{value}' instead of "
         f'--fdl_set={path}={value}.'
     ) from e
 
 
+@dataclasses.dataclass(frozen=True)
+class CallExpression:
+  """Parsed components of a call expression (or bare function name).
+
+  Examples:
+
+  >>> CallExpression.parse("fn('foo', False, x=[1, 2])")
+  CallExpression(func_name='fn', args=('foo', False'), kwargs={'x': [1, 2]})
+  >>> CallExpression.parse("fn")  # Bare function name: empty args/kwargs.
+  CallExpression(func_name='fn', args=()), kwargs={})
+
+  Attributes:
+    func_name: The name fo the function that should be called.
+    args: Parsed values of positional arguments for the function.
+    kwargs: Parsed values of keyword arguments for the function.
+  """
+
+  func_name: str
+  args: Optional[Tuple[Any, ...]]
+  kwargs: Optional[Dict[str, Any]]
+
+  _PARSE_RE = re.compile(r'(?P<func_name>[\w\.]+)(?:\((?P<args>.*)\))?')
+
+  @classmethod
+  def parse(cls, value: str) -> 'CallExpression':
+    """Returns a CallExpression parsed from a string.
+
+    Args:
+      value: A string containing positional and keyword arguments for a
+        function.  Must consist of an open paren followed by comma-separated
+        argument values followed by a close paren.  Argument values must be
+        literal constants (i.e., must be parsable with `ast.literal_eval`).
+        var-positional and var-keyword arguments are not supported.
+
+    Raises:
+      SyntaxError: If `value` is not a simple call expression with literal
+        arguments.
+    """
+    m = re.fullmatch(cls._PARSE_RE, value)
+    if m is None:
+      raise SyntaxError(
+          f'Expected a function name or call expression; got: {value!r}'
+      )
+    if m.group('args') is None:  # Bare function name
+      return CallExpression(m.group('func_name'), (), {})
+
+    node = ast.parse(value)  # Can raise SyntaxError.
+    if not (
+        isinstance(node, ast.Module)
+        and len(node.body) == 1
+        and isinstance(node.body[0], ast.Expr)
+        and isinstance(node.body[0].value, ast.Call)
+    ):
+      raise SyntaxError(
+          f'Expected a function name or call expression; got: {value!r}'
+      )
+    call_node = node.body[0].value
+    args = []
+    for arg in call_node.args:
+      if isinstance(arg, ast.Starred):
+        raise SyntaxError('*args is not supported.')
+      try:
+        args.append(ast.literal_eval(arg))
+      except ValueError as exc:
+        raise SyntaxError(
+            'Expected arguments to be simple literals; got '
+            f'{ast.unparse(arg)!r} (while parsing {value!r})'
+        ) from exc
+    kwargs = {}
+    for kwarg in call_node.keywords:
+      if kwarg.arg is None:
+        raise SyntaxError('**kwargs is not supported.')
+      try:
+        kwargs[kwarg.arg] = ast.literal_eval(kwarg.value)
+      except ValueError as exc:
+        raise SyntaxError(
+            'Expected arguments to be simple literals; got '
+            f'{ast.unparse(kwarg.value)!r} (while parsing {value!r})'
+        ) from exc
+    return CallExpression(m.group('func_name'), tuple(args), kwargs)
+
+
 def apply_overrides_to(cfg: config.Buildable):
   """Applies all command line flags to `cfg`."""
   for flag in _FDL_SET.value:
     path, value = flag.split('=', maxsplit=1)
     *parents, last = _parse_path(path)
     walk = typing.cast(Any, cfg)
     try:
       for parent in parents:
-        walk = parent(walk)
+        walk = parent.follow(walk)
     except Exception as e:
       raise ValueError(f'Invalid path "{path}".') from e
 
     literal_value = parse_value(value=value, path=path)
     try:
-      last.update(walk, literal_value)
+      if isinstance(last, daglish.Attr):
+        setattr(walk, last.name, literal_value)
+      elif isinstance(last, daglish.Key):
+        walk[last.key] = literal_value
+      else:
+        raise ValueError(f'Unexpected path element {last}.')
     except Exception as e:
       raise ValueError(f'Could not set "{path}" to "{value}".') from e
 
 
 def _rewrite_fdl_args(args: Sequence[str]) -> List[str]:
   """Rewrites short-form Fiddle flags.
 
@@ -400,15 +447,17 @@
             value=parse_value(value=value, path=str(matching_tags[0])))
 
 
 def apply_fiddlers_to(cfg: config.Buildable,
                       source_module: Any,
                       allow_imports=False):
   """Applies fiddlers to `cfg`."""
-  for fiddler_name in _FIDDLER.value:
+  for fiddler_value in _FIDDLER.value:
+    call_expr = CallExpression.parse(fiddler_value)
+    fiddler_name = call_expr.func_name
     if hasattr(source_module, fiddler_name):
       fiddler = getattr(source_module, fiddler_name)
     elif allow_imports:
       try:
         fiddler = _import_dotted_name(
             fiddler_name, mode=_ImportDottedNameDebugContext.FIDDLER
         )
@@ -416,15 +465,15 @@
         raise ValueError(f'Could not load fiddler {fiddler_name!r}: {e}') from e
     else:
       available_fiddlers = ', '.join(
           module_reflection.find_fiddler_like_things(source_module))
       raise ValueError(
           f'No fiddler named {fiddler_name!r} found; available fiddlers: '
           f'{available_fiddlers}.')
-    fiddler(cfg)
+    fiddler(cfg, *call_expr.args, **call_expr.kwargs)
 
 
 def _print_help(module, allow_imports):
   """Prints flag help, including available symbols in `module`."""
   flags_help_text = flags.FLAGS.module_help(sys.modules[__name__])
   flags_help_text = '\n'.join(flags_help_text.splitlines()[2:])
   _print_stderr('Fiddle-specific command line flags:')
@@ -447,22 +496,30 @@
         docstring = f' - {obj_doc}'
       else:
         docstring = ''
       _print_stderr(f'  {name}{docstring}')
 
   if allow_imports:
     _print_stderr()
-    _print_stderr('Base configs and fiddlers may be specified using '
-                  'fully-qualified dotted names.')
+    _print_stderr(
+        'Base configs and fiddlers may be specified using '
+        'fully-qualified dotted names.'
+    )
+
+
+def fdl_flags_supplied() -> bool:
+  """Returns True if if required Fiddle flags are defined."""
+  config_defined = bool(_FDL_CONFIG.value or _FDL_CONFIG_FILE.value)
+  return config_defined or _FDL_HELP.value
 
 
 def create_buildable_from_flags(
     module: Optional[Any],
     allow_imports=False,
-    pyref_policy: Optional[serialization.PyrefPolicy] = None
+    pyref_policy: Optional[serialization.PyrefPolicy] = None,
 ) -> config.Buildable:
   """Returns a fdl.Buildable based on standardized flags.
 
   Args:
     module: A common namespace to use as the basis for finding configs and
       fiddlers. May be `None`; if `None`, only fully qualified Fiddler imports
       will be used (or alternatively a base configuration can be specified using
@@ -492,15 +549,16 @@
         '`{flag}` flag unless `allow_imports` is `True`.')
     if _FDL_CONFIG.value:
       raise ValueError(err_msg.format(flag='--fdl_config'))
     if _FIDDLER.value:
       raise ValueError(err_msg.format(flag='--fiddler'))
 
   if _FDL_CONFIG.value:
-    base_name = _FDL_CONFIG.value
+    call_expr = CallExpression.parse(_FDL_CONFIG.value)
+    base_name = call_expr.func_name
     if hasattr(module, base_name):
       base_fn = getattr(module, base_name)
     elif allow_imports:
       try:
         base_fn = _import_dotted_name(
             base_name, mode=_ImportDottedNameDebugContext.BASE_CONFIG
         )
@@ -509,17 +567,17 @@
             f'Could not init a buildable from {base_name!r}: {e}') from e
     else:
       available_names = module_reflection.find_base_config_like_things(module)
       raise ValueError(f'Could not init a buildable from {base_name!r}; '
                        f'available names: {", ".join(available_names)}.')
 
     if auto_config.is_auto_config(base_fn):
-      buildable = base_fn.as_buildable()
+      buildable = base_fn.as_buildable(*call_expr.args, **call_expr.kwargs)
     else:
-      buildable = base_fn()
+      buildable = base_fn(*call_expr.args, **call_expr.kwargs)
   elif _FDL_CONFIG_FILE.value:
     with _FDL_CONFIG_FILE.value.open() as f:
       buildable = serialization.load_json(f.read(), pyref_policy=pyref_policy)
   else:
     raise AssertionError('This should be unreachable.')
 
   apply_fiddlers_to(
```

### Comparing `fiddle-0.2.6/fiddle/_src/absl_flags/sample_module_for_flags_test.py` & `fiddle-0.2.7/fiddle/_src/absl_flags/sample_module_for_flags_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/arg_factory.py` & `fiddle-0.2.7/fiddle/_src/arg_factory.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/arg_factory_test.py` & `fiddle-0.2.7/fiddle/_src/arg_factory_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/building.py` & `fiddle-0.2.7/fiddle/_src/building.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Implements Fiddle's build() function."""
 
 import contextlib
 import functools
+import logging
 import threading
 from typing import Any, Callable, Dict, TypeVar, overload
 
 from fiddle._src import config as config_lib
 from fiddle._src import daglish
 from fiddle._src import reraised_exception
 
@@ -65,43 +66,49 @@
   fn_or_cls = config_lib.get_callable(buildable)
   try:
     fn_or_cls_name = fn_or_cls.__qualname__
   except AttributeError:
     fn_or_cls_name = str(fn_or_cls)  # callable instances, etc.
   kwargs_str = ', '.join(
       f'{name}={_format_arg(value)}' for name, value in arguments.items())
-  return ('\n\nFiddle context: failed to construct or call '
-          f'{fn_or_cls_name} at {path_str} '
-          f'with arguments ({kwargs_str})')
+
+  tag_information = ''
+  bound_args = buildable.__signature__.bind_partial(**arguments)
+  bound_args.apply_defaults()
+  unset_arg_tags = []
+  for param in buildable.__signature__.parameters:
+    if param in bound_args.arguments:
+      continue  # User supplied it, all good.
+    tags = buildable.__argument_tags__.get(param, None)
+    if tags:
+      tag_str = ' '.join(sorted(str(tag) for tag in tags))
+      unset_arg_tags.append(f' - {param}: {tag_str}')
+  if unset_arg_tags:
+    tag_details = '\n'.join(unset_arg_tags)
+    tag_information = f'\nTags for unset arguments:\n{tag_details}'
+
+  return (
+      '\n\nFiddle context: failed to construct or call '
+      f'{fn_or_cls_name} at {path_str} '
+      f'with arguments ({kwargs_str}){tag_information}'
+  )
 
 
 def call_buildable(
     buildable: config_lib.Buildable,
     arguments: Dict[str, Any],
     *,
     current_path: daglish.Path,
 ) -> Any:
   make_message = functools.partial(_make_message, current_path, buildable,
                                    arguments)
   with reraised_exception.try_with_lazy_message(make_message):
     return buildable.__build__(**arguments)
 
 
-def _build(value: Any, state: daglish.State) -> Any:
-  """Inner method / implementation of build()."""
-
-  if isinstance(value, config_lib.Buildable):
-    sub_traversal = state.flattened_map_children(value)
-    metadata: config_lib.BuildableTraverserMetadata = sub_traversal.metadata
-    arguments = metadata.arguments(sub_traversal.values)
-    return call_buildable(value, arguments, current_path=state.current_path)
-  else:
-    return state.map_children(value)
-
-
 # Define typing overload for `build(Partial[T])`
 @overload
 def build(buildable: config_lib.Partial[T]) -> Callable[..., T]:
   ...
 
 
 # Define typing overload for `build(Config[T])`
@@ -141,10 +148,33 @@
   Args:
     buildable: A ``Buildable`` instance to build, or a nested structure of
       ``Buildable`` objects.
 
   Returns:
     The built version of ``buildable``.
   """
+  is_built = False
+
+  def _build(value: Any, state: daglish.State) -> Any:
+    """Inner method / implementation of build()."""
+    nonlocal is_built
+    if isinstance(value, config_lib.Buildable):
+      sub_traversal = state.flattened_map_children(value)
+      metadata: config_lib.BuildableTraverserMetadata = sub_traversal.metadata
+      arguments = metadata.arguments(sub_traversal.values)
+      is_built = True
+      return call_buildable(value, arguments, current_path=state.current_path)
+    else:
+      return state.map_children(value)
 
   with _in_build():
-    return daglish.MemoizedTraversal.run(_build, buildable)
+    result = daglish.MemoizedTraversal.run(_build, buildable)
+
+  if not is_built:
+    logging.warning(
+        'No Buildables found in value passed to `fdl.build()`: '
+        '%s with type %s.',
+        str(buildable),
+        type(buildable),
+    )
+
+  return result
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/__init__.py` & `fiddle-0.2.7/fiddle/_src/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/__init__.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/code_ir.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/code_ir.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         path_elements_fn=lambda x: x.__path_elements__(),
     )
 
 
 @dataclasses.dataclass
 class Parameter(CodegenNode):
   name: Name
-  value_type: Type[Any]
+  value_type: Optional[Type[Any]] = None
 
 
 @dataclasses.dataclass
 class VariableReference(CodegenNode):
   """Reference to a variable or parameter."""
 
   name: Name
@@ -122,31 +122,48 @@
   need a way of tagging it as such.
   """
 
   expression: Any  # Wrapped expression, can involve VariableReference's
 
 
 @dataclasses.dataclass
-class Call(CodegenNode):
-  name: Name
-  arg_expressions: Dict[Name, Any]  # Value that can involve VariableReference's
+class HistoryComments:
+  """Brief assignment history, currently for buildables.
+
+  Note: This is intentionally a plain dataclass and not traversed by daglish
+  by default.
+  """
+
+  # For fdl.Config-like objects, attr name --> history string.
+  per_field: Dict[str, str] = dataclasses.field(default_factory=dict)
 
 
 @dataclasses.dataclass
-class SymbolCall(CodegenNode):
-  """Reference to a call of a library symbol, like MyEncoderLayer()."""
+class SymbolOrFixtureCall(CodegenNode):
+  """Reference to a call of a library symbol/fixture, like MyEncoderLayer()."""
 
   symbol_expression: str
   # Values for args can involve VariableReference's, Calls, etc.
   positional_arg_expressions: List[Any]
   arg_expressions: Dict[str, Any]
+  history_comments: HistoryComments = dataclasses.field(
+      default_factory=HistoryComments
+  )
+
+
+@dataclasses.dataclass
+class WithTagsCall(CodegenNode):
+  """Represents a call to auto_config.with_tags()."""
+
+  tag_symbol_expressions: List[str]
+  item_to_tag: Any
 
 
 @dataclasses.dataclass
-class FunctoolsPartialCall(SymbolCall):
+class FunctoolsPartialCall(SymbolOrFixtureCall):
   pass
 
 
 @dataclasses.dataclass
 class VariableDeclaration(CodegenNode):
   name: Name
   expression: Any  # Value that can involve VariableReference's
@@ -183,17 +200,16 @@
   This is more of a dataflow node than an expression of calling a function, i.e.
   it represents a call to a function at a particular point in the auto_config
   fixture's execution.
   """
 
   fn: FixtureFunction
   parent: Optional[CallInstance]
-  children: Dict[Call, CallInstance]
+  children: List[CallInstance]
   parameter_values: Dict[Name, Any]
-  output_value: Any
 
   def __hash__(self) -> int:
     return id(self)
 
   def to_stack(self) -> List[CallInstance]:
     current = self
     result = [self]
@@ -203,15 +219,15 @@
     return list(reversed(result))
 
   @arg_factory.supply_defaults
   def all_fixture_functions(
       self, seen=arg_factory.default_factory(set)
   ) -> List[FixtureFunction]:
     result = [] if self.fn in seen else [self.fn]
-    for child in self.children.values():
+    for child in self.children:
       result.extend(child.all_fixture_functions(seen))
     return result
 
 
 def _init_import_manager() -> import_manager_lib.ImportManager:
   return import_manager_lib.ImportManager(namespace=namespace_lib.Namespace())
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/code_ir_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/code_ir_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/complex_to_variables.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/complex_to_variables.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,32 +78,36 @@
     is_complex: Function used to determine when a node should be moved to a
       variable.
     make_namer: Function that will create a Namer, used for assigning new names
       to extracted variables. Note: Each path is relative to a FixtureFunction,
       not the overall config.
   """
 
-  global_in_use_names = copy.copy(task.global_namespace.names)
-  global_in_use_names.update(
-      fn.name.value for fn in task.top_level_call.all_fixture_functions()
-  )
+  task_existing_names = naming.get_task_existing_names(task)
 
   def _process_fn(fn: code_ir.FixtureFunction) -> None:
-    names = copy.copy(global_in_use_names)
-    names.update(parameter.name.value for parameter in fn.parameters)
-    names.update(variable.name.value for variable in fn.variables)
+    names = copy.copy(task_existing_names)
+    names.update(naming.get_fn_existing_names(fn))
     namer = make_namer(namespace_lib.Namespace(names))
 
     new_variables = []
 
     def traverse(value, state: daglish.State):
       """Extracts complex values to variables."""
       if not state.is_traversable(value):
         return value
 
+      if isinstance(value, code_ir.SymbolOrFixtureCall):
+        value.arg_expressions = state.map_children(value.arg_expressions)
+        return value
+
+      if isinstance(value, code_ir.VariableDeclaration):
+        value.expression = state.map_children(value.expression)
+        return value
+
       value = state.map_children(value)
 
       if isinstance(
           value, (code_ir.VariableDeclaration, code_ir.ArgFactoryExpr)
       ):
         # If something is already a variable, don't create another variable.
         # Likewise, if it is an ArgFactoryExpr, keep it inline with its parent
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/complex_to_variables_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/complex_to_variables_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     task = init_task.init_task(config)
     self.assertEmpty(task.top_level_call.fn.variables)
     shared_to_variables.move_shared_nodes_to_variables(task)
     self.assertLen(task.top_level_call.fn.variables, 1)
     complex_to_variables.move_complex_nodes_to_variables(
         task, is_complex=lambda x: True
     )
-    self.assertLen(task.top_level_call.fn.variables, 14)
+    self.assertLen(task.top_level_call.fn.variables, 13)
     code = ir_printer.format_task(task)
     self.assertIn("self_attention =", code)
     self.assertIn("cross_attention =", code)
     self.assertIn("sharding_axes =", code)
     self.assertIn("sharding_axes_2 =", code)
 
   def test_doesnt_fail_if_cant_name(self):
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/init_task.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/init_task.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,10 +42,10 @@
           is_generated=top_level_fixture_name == "config_fixture",
       ),
       parameters=[],
       variables=[],
       output_value=config,
   )
   call_instance = code_ir.CallInstance(
-      fn, parent=None, children={}, parameter_values={}, output_value=config
+      fn, parent=None, children=[], parameter_values={}
   )
   return code_ir.CodegenTask(config, top_level_call=call_instance)
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/init_task_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/init_task_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/ir_printer.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,25 +75,22 @@
     elif isinstance(value, dict):
       value = state.map_children(value)
       return (
           "{"
           + ", ".join(f'"{key}": {value}' for key, value in value.items())
           + "}"
       )
-    elif isinstance(value, code_ir.Call):
-      args_str = ", ".join(
-          f"{key}={value}"
-          for key, value in state.map_children(value.arg_expressions).items()
-      )
-      return f"{value.name.value}({args_str})"
     elif isinstance(value, code_ir.VariableReference):
       return value.name.value
     elif isinstance(value, code_ir.ArgFactoryExpr):
       sub_value = state.map_children(value).expression
       return f"ArgFactoryExpr[{sub_value}]"
+    elif isinstance(value, code_ir.WithTagsCall):
+      sub_value = state.map_children(value).expression
+      return f"WithTagsCall[{sub_value}]"
     elif isinstance(value, code_ir.Name):
       return value.value
     elif isinstance(value, type):
       return value.__name__
     elif value in typing_consts or type(value) in typing_consts:
       return str(value)
     else:
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/ir_printer_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_printer_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 """Tests for ir_printer."""
 
 import textwrap
 
 from typing import Any, Optional
 
 from absl.testing import absltest
-from fiddle._src.codegen.auto_config import code_ir
 from fiddle._src.codegen.auto_config import ir_printer
 from fiddle._src.codegen.auto_config import test_fixtures
 
 
 class A:
 
   def __str__(self):
@@ -59,21 +58,14 @@
     example_tuple = (3, 2.5, str)
     self.assertEqual(ir_printer.format_expr(example_tuple), "(3, 2.5, str)")
     example_tuple = ()
     self.assertEqual(ir_printer.format_expr(example_tuple), "()")
     example_tuple = (3,)
     self.assertEqual(ir_printer.format_expr(example_tuple), "(3,)")
 
-  def test_format_call(self):
-    call = code_ir.Call(
-        name=code_ir.Name("foo_fixture"),
-        arg_expressions={code_ir.Name("bar"): 777},
-    )
-    self.assertEqual(ir_printer.format_expr(call), "foo_fixture(bar=777)")
-
   def test_format_simple_ir(self):
     task = test_fixtures.simple_ir()
     code = "\n".join(ir_printer.format_fn(task.top_level_call.fn))
     self.assertEqual(
         code,
         textwrap.dedent(
             """
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/ir_to_cst.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_to_cst.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """Converts from the auto_config codegen representation to LibCST nodes.
 
 Note: We do not generally do a lot of formatting, instead relying on existing
 source code formatters (pyformat, yapf, etc.).
 """
 
-from typing import Any
+from typing import Any, List, Optional
 
 from fiddle import daglish
 from fiddle._src import config as config_lib
 from fiddle._src.codegen import py_val_to_cst_converter
 from fiddle._src.codegen.auto_config import code_ir
 import libcst as cst
 
@@ -35,14 +35,52 @@
     expr: Arbitrary Python value expression to generate code for.
 
   Returns:
     CST node for expression.
   """
 
   def traverse(value, state: daglish.State) -> cst.CSTNode:
+
+    def _prepare_args_helper(
+        names: List[str],
+        values: List[Any],
+        attr: daglish.Attr,
+        *,
+        history: Optional[code_ir.HistoryComments] = None,
+    ) -> List[cst.Arg]:
+      """Prepare code_ir.Arg node based on names and values."""
+      args = []
+      for arg_name, arg_value in zip(names, values):
+        assert isinstance(arg_name, str)
+        arg_value = state.call(arg_value, attr, daglish.Key(arg_name))
+        kwargs = {}
+        if history and arg_name in history.per_field:
+          kwargs["comma"] = cst.Comma(
+              whitespace_after=cst.ParenthesizedWhitespace(
+                  first_line=cst.TrailingWhitespace(
+                      whitespace=cst.SimpleWhitespace("  "),
+                      comment=cst.Comment(f"# {history.per_field[arg_name]}"),
+                      newline=cst.Newline(),
+                  ),
+                  last_line=cst.SimpleWhitespace(" " * 6),
+              )
+          )
+        args.append(
+            cst.Arg(
+                arg_value,
+                keyword=cst.Name(arg_name),
+                equal=cst.AssignEqual(
+                    whitespace_before=cst.SimpleWhitespace(""),
+                    whitespace_after=cst.SimpleWhitespace(""),
+                ),
+                **kwargs,
+            )
+        )
+      return args
+
     if isinstance(value, config_lib.Buildable):
       raise ValueError(
           "Internal Fiddle error: you must run the make_symbolic_reference "
           "passes before CST generation."
       )
     elif isinstance(value, (list, tuple)):
       value = state.map_children(value)
@@ -56,36 +94,54 @@
       for key, sub_value in value.items():
         key_node = state.call(key, daglish.Key(f"__key_{key}"))
         sub_value_node = state.call(sub_value, daglish.Attr(key))
         elements.append(cst.DictElement(key_node, sub_value_node))
       return cst.Dict(elements)
     elif isinstance(value, code_ir.VariableReference):
       return cst.Name(value.name.value)
-    elif isinstance(value, code_ir.SymbolCall):
+    elif isinstance(value, code_ir.SymbolOrFixtureCall):
       attr = daglish.Attr("arg_expressions")
       args = []
       for i, arg_value in enumerate(value.positional_arg_expressions):
         arg_value = state.call(arg_value, attr, daglish.Key(i))
         args.append(cst.Arg(arg_value))
-      for arg_name, arg_value in value.arg_expressions.items():
-        arg_value = state.call(arg_value, attr, daglish.Key(arg_name))
-        args.append(
-            cst.Arg(
-                arg_value,
-                keyword=cst.Name(arg_name),
-                equal=cst.AssignEqual(
-                    whitespace_before=cst.SimpleWhitespace(""),
-                    whitespace_after=cst.SimpleWhitespace(""),
-                ),
+
+      any_args_have_history = False
+      if value.arg_expressions:
+        names, values = zip(*value.arg_expressions.items())
+        any_args_have_history = set(names) & set(
+            value.history_comments.per_field
+        )
+        args.extend(
+            _prepare_args_helper(
+                names, values, attr, history=value.history_comments
             )
         )
+      if any_args_have_history:
+        whitespace_before_args = cst.ParenthesizedWhitespace(
+            first_line=cst.TrailingWhitespace(newline=cst.Newline()),
+            last_line=cst.SimpleWhitespace(" " * 6),
+        )
+      else:
+        whitespace_before_args = cst.SimpleWhitespace("")
       return cst.Call(
           cst.parse_expression(value.symbol_expression),
           args=args,
+          whitespace_before_args=whitespace_before_args,
       )
+    elif isinstance(value, code_ir.WithTagsCall):
+      attr = daglish.Attr("item_to_tag")
+      item_to_tag = state.call(value.item_to_tag, attr)
+      call_args = [cst.Arg(item_to_tag)]
+      sorted_tags = sorted([tag for tag in value.tag_symbol_expressions])
+      for tag in sorted_tags:
+        tag_name = cst.parse_expression(tag)
+        call_args.append(cst.Arg(tag_name))
+      with_tags = cst.parse_expression("auto_config.with_tags")
+      return cst.Call(with_tags, args=call_args)
     elif isinstance(value, code_ir.SymbolReference):
       return cst.parse_expression(value.expression)
     elif state.is_traversable(value):
       raise NotImplementedError(
           f"Expression generation is not implemented for {value!r}"
       )
     else:
@@ -108,17 +164,20 @@
   Args:
     fn: Fixture function to generate code for.
     task: Codegen task.
 
   Returns:
     LibCST FunctionDef node.
   """
-  auto_config_expr = cst.parse_expression(
-      task.import_manager.add(task.auto_config_fn)
-  )
+  if task.auto_config_fn:
+    auto_config_expr = cst.parse_expression(
+        task.import_manager.add(task.auto_config_fn)
+    )
+  else:
+    auto_config_expr = None
   params = cst.Parameters(
       params=[
           cst.Param(name=cst.Name(param.name.value)) for param in fn.parameters
       ]
   )
   variable_lines = []
   for variable_decl in fn.variables:
@@ -144,15 +203,15 @@
     )
   else:
     whitespace_before_params = cst.SimpleWhitespace("")
   return cst.FunctionDef(
       cst.Name(fn.name.value),
       params,
       body,
-      decorators=[cst.Decorator(auto_config_expr)],
+      decorators=[cst.Decorator(auto_config_expr)] if auto_config_expr else [],
       whitespace_before_params=whitespace_before_params,
       leading_lines=[cst.EmptyLine(), cst.EmptyLine()],
   )
 
 
 def code_for_task(
     task: code_ir.CodegenTask,
@@ -162,10 +221,10 @@
   Args:
     task: Codegen task.
 
   Returns:
     LibCST module.
   """
   body = []
-  for fn in reversed(task.top_level_call.all_fixture_functions()):
+  for fn in task.top_level_call.all_fixture_functions():
     body.append(code_for_fn(fn, task=task))
   return cst.Module(body=task.import_manager.sorted_import_lines() + body)
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/make_symbolic_references.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/make_symbolic_references.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 
 """Changes callables to symbol references."""
 
 import enum
 import functools
 import inspect
-from typing import Any
+from typing import Any, Callable
 
 from fiddle import arg_factory
 from fiddle import daglish
 from fiddle._src import config as config_lib
 from fiddle._src.codegen.auto_config import code_ir
 
 
@@ -50,32 +50,52 @@
     task: Codegen task.
   """
 
   task.import_manager.add(task.auto_config_fn)
   for value, _ in daglish.iterate(task.top_level_call.all_fixture_functions()):
     if isinstance(value, config_lib.Buildable):
       task.import_manager.add(config_lib.get_callable(value))
+      # Import the tags too.
+      for arg_tags in value.__argument_tags__.values():
+        for tag in arg_tags:
+          task.import_manager.add(tag)
     elif is_plain_symbol_or_enum_value(value):
       task.import_manager.add(value)
 
 
+def noop_history_comments(unused_buildable):
+  return code_ir.HistoryComments()
+
+
 def replace_callables_and_configs_with_symbols(
     task: code_ir.CodegenTask,
+    *,
+    format_history: Callable[
+        ..., code_ir.HistoryComments
+    ] = noop_history_comments,
 ) -> None:
-  """Replaces callables and Buildables with symbolic versions."""
+  """Replaces callables and Buildables with symbolic versions.
+
+  Args:
+    task: Codegen task.
+    format_history: Function used to format history for a buildable. Set to
+      get_history_comments.format_history_for_buildable (or a functools.partial
+      variant) to populate histories.
+  """
 
   fn_name = None
 
   def _handle_partial(
       value: config_lib.Partial, state: daglish.State, symbol: str
   ):
     """Split-out helper method to handle Partial() nodes."""
     symbol_ref = code_ir.SymbolReference(symbol)
 
     arguments = config_lib.ordered_arguments(value)
+    all_tags = value.__argument_tags__
 
     # Arguments which were config_lib.ArgFactory arguments; these need to be
     # turned into regular calls.
     arg_factory_args = {}
 
     # All other arguments.
     regular_args = {}
@@ -84,54 +104,83 @@
       if isinstance(arg_value, code_ir.ArgFactoryExpr):
         arg_factory_args[name] = state.call(
             arg_value.expression, daglish.Attr(name)
         )
       else:
         regular_args[name] = state.call(arg_value, daglish.Attr(name))
 
+    for dict_of_args in (arg_factory_args, regular_args):
+      for arg in dict_of_args:
+        if arg in all_tags:
+          tags = all_tags[arg]
+          tags_expr = [task.import_manager.add(tag) for tag in tags]
+          dict_of_args[arg] = code_ir.WithTagsCall(
+              tag_symbol_expressions=tags_expr,
+              item_to_tag=dict_of_args[arg],
+          )
+
     def _arg_factory_partial():
-      return code_ir.SymbolCall(
+      return code_ir.SymbolOrFixtureCall(
           task.import_manager.add(arg_factory.partial),
           positional_arg_expressions=[symbol_ref],
           arg_expressions=arg_factory_args,
+          history_comments=format_history(value),
       )
 
     if not arg_factory_args:
       # The common case: there are no arg_factory's, so just emit a functools
       # partial. We currently emit a functools partial even if there are no
       # arguments, because this will mean there's a fdl.Partial when we call
       # the auto_config fixture's as_buildable() method. If we got rid of the
       # functools.partial, then we couldn't configure any attributes.
-      return code_ir.SymbolCall(
+      return code_ir.SymbolOrFixtureCall(
           task.import_manager.add(functools.partial),
           positional_arg_expressions=[symbol_ref],
           arg_expressions=regular_args,
+          history_comments=format_history(value),
       )
     elif not regular_args:
       # There are only arg_factory args, so we can emit an arg_factory.partial.
       return _arg_factory_partial()
     else:
       # We have both functools.partial and arg_factory args. It doesn't matter
       # which order, but we need to emit both decorators. Go with functools
       # on the outer level.
-      return code_ir.SymbolCall(
+      return code_ir.SymbolOrFixtureCall(
           task.import_manager.add(functools.partial),
           positional_arg_expressions=[_arg_factory_partial()],
           arg_expressions=regular_args,
+          history_comments=format_history(value),
       )
 
   def traverse(value, state: daglish.State):
     if isinstance(value, config_lib.Buildable):
       symbol = task.import_manager.add(config_lib.get_callable(value))
       if isinstance(value, config_lib.Config):
+        all_tags = value.__argument_tags__
         value = state.map_children(value)
-        return code_ir.SymbolCall(
+        for arg, arg_tags in all_tags.items():
+          tag_expr = [task.import_manager.add(tag) for tag in arg_tags]
+          if arg not in value.__arguments__:
+            raise ValueError(
+                f"Tagged field '{arg}' of {value!r} is not found in its"
+                f" arguments: {value.__arguments__}. This is likely because the"
+                " tagged field doesn't yet have a value. Consider assigning a"
+                " value to the field first or removing field tags from your"
+                " config, for example using `fdl.clear_tags`."
+            )
+          value.__arguments__[arg] = code_ir.WithTagsCall(
+              tag_symbol_expressions=tag_expr,
+              item_to_tag=value.__arguments__[arg],
+          )
+        return code_ir.SymbolOrFixtureCall(
             symbol_expression=symbol,
             positional_arg_expressions=[],
             arg_expressions=config_lib.ordered_arguments(value),
+            history_comments=format_history(value),
         )
       elif isinstance(value, config_lib.Partial):
         return _handle_partial(value, state, symbol)
       elif isinstance(value, config_lib.ArgFactory):
         paths = " , ".join(
             daglish.path_str(path) for path in state.get_all_paths()
         )
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/newcg_symbolic_references_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,150 +9,150 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for make_symbolic_references pass."""
+"""Tests for newcg_symbolic_references pass."""
+
+import inspect
 
 from absl.testing import absltest
 import fiddle as fdl
+from fiddle._src.codegen import newcg_symbolic_references
 from fiddle._src.codegen.auto_config import code_ir
 from fiddle._src.codegen.auto_config import complex_to_variables
+from fiddle._src.codegen.auto_config import get_history_comments
 from fiddle._src.codegen.auto_config import init_task
 from fiddle._src.codegen.auto_config import ir_to_cst
-from fiddle._src.codegen.auto_config import make_symbolic_references
-from fiddle._src.codegen.auto_config import split_arg_factories
 from fiddle._src.codegen.auto_config import test_fixtures
 
 
 class MakeSymbolicReferencesTest(absltest.TestCase):
 
   def test_import_symbols(self):
     task = test_fixtures.simple_ir()
 
     # By default, this contains a bunch of builtins.
     task.import_manager.namespace.names = set()
 
-    make_symbolic_references.import_symbols(task)
+    newcg_symbolic_references.import_symbols(task)
 
     # The imported symbols are auto_config, and the fixture module, since it
     # contains the `foo` function.
     self.assertEqual(
-        task.import_manager.namespace.names, {'auto_config', 'test_fixtures'}
+        task.import_manager.namespace.names, {'fdl', 'test_fixtures'}
     )
 
   def test_import_symbols_empty(self):
     task = init_task.init_task(config=[])
     task.import_manager.namespace.names = set()
-    make_symbolic_references.import_symbols(task)
-    self.assertEqual(task.import_manager.namespace.names, {'auto_config'})
+    newcg_symbolic_references.import_symbols(task)
+    self.assertEqual(task.import_manager.namespace.names, set())
 
   def test_replace_config_callable(self):
     task = test_fixtures.simple_ir()
-    make_symbolic_references.import_symbols(task)
-    make_symbolic_references.replace_callables_and_configs_with_symbols(task)
+    newcg_symbolic_references.import_symbols(task)
+    newcg_symbolic_references.replace_callables_and_configs_with_symbols(
+        task, format_history=get_history_comments.format_history_for_buildable
+    )
+    (base_line,) = (
+        i
+        for i, line in enumerate(inspect.getsource(test_fixtures).splitlines())
+        if 'def simple_ir(' in line
+    )
+    line = base_line + 9  # Feel free to adjust if the test fixture is changed.
     self.assertEqual(
         task.top_level_call.fn,
         code_ir.FixtureFunction(
             name=code_ir.Name(
                 value='simple_ir_fixture', is_generated=False, previous=None
             ),
             parameters=[],
             variables=[],
-            output_value=code_ir.SymbolCall(
-                symbol_expression='test_fixtures.foo',
-                positional_arg_expressions=[],
+            output_value=code_ir.SymbolOrFixtureCall(
+                symbol_expression='fdl.Config',
+                positional_arg_expressions=[
+                    code_ir.SymbolReference('test_fixtures.foo')
+                ],
                 arg_expressions={'x': 4},
+                history_comments=code_ir.HistoryComments(
+                    per_field={
+                        '__fn_or_cls__': (
+                            f'Set in .../auto_config/test_fixtures.py:{line}'
+                            ':simple_ir'
+                        ),
+                        'x': (
+                            f'Set in .../auto_config/test_fixtures.py:{line}'
+                            ':simple_ir'
+                        ),
+                    }
+                ),
             ),
         ),
     )
 
   def test_replaces_arg_factory_partial(self):
-    # This test goes from auto_config to a config object and back again.
+    # Tests arg factories.
 
     config = test_fixtures.auto_config_arg_factory_fn.as_buildable()
     task = init_task.init_task(config=config)
-    make_symbolic_references.import_symbols(task)
-    split_arg_factories.lower_arg_factories(task)
-    make_symbolic_references.replace_callables_and_configs_with_symbols(task)
+    task.auto_config_fn = None
+    newcg_symbolic_references.import_symbols(task)
+    newcg_symbolic_references.replace_callables_and_configs_with_symbols(task)
     code = ir_to_cst.code_for_task(task).code
 
     expected = """
+    import fiddle as fdl
     from fiddle._src.codegen.auto_config import test_fixtures
-    from fiddle import arg_factory
-    from fiddle.experimental import auto_config
-    import functools
 
-
-    @auto_config.auto_config
     def config_fixture():
-        return functools.partial(arg_factory.partial(test_fixtures.SharedType,
-            x=functools.partial(test_fixtures.count, increment=3)), z=4.7)
-    """
+      return fdl.Partial(test_fixtures.SharedType, x=fdl.ArgFactory(test_fixtures.count, increment=3), z=4.7)
+   """
     self.assertEqual(code.split(), expected.split(), msg=code)
 
-  def test_forget_to_lower_reasonable_error(self):
-    # This probably won't be very user-facing, but for our own ease of
-    # development, make sure error messages are reasonable if we forget to
-    # call lower_arg_factories().
-    config = test_fixtures.auto_config_arg_factory_fn.as_buildable()
-    task = init_task.init_task(config=config)
-    make_symbolic_references.import_symbols(task)
-    with self.assertRaisesRegex(
-        TypeError,
-        r'Path to misformed object in codegen DAG: \.output_value\.x\.',
-    ):
-      make_symbolic_references.replace_callables_and_configs_with_symbols(task)
-
   def test_two_arg_factories(self):
     config = fdl.Partial(
         test_fixtures.SharedType,
         x=fdl.ArgFactory(test_fixtures.foo, x=7),
         z=fdl.ArgFactory(test_fixtures.foo, x=3.2),
     )
     task = init_task.init_task(config=config)
-    make_symbolic_references.import_symbols(task)
-    split_arg_factories.lower_arg_factories(task)
-    make_symbolic_references.replace_callables_and_configs_with_symbols(task)
+    newcg_symbolic_references.import_symbols(task)
+    newcg_symbolic_references.replace_callables_and_configs_with_symbols(task)
     code = ir_to_cst.code_for_task(task).code
     self.assertIn('7', code)
     self.assertIn('3.2', code)
 
   def test_nested_arg_factories(self):
     config = fdl.Partial(
         test_fixtures.Attention,
         kernel_init=fdl.ArgFactory(
             test_fixtures.initializer, name='const', dtype='float32'
         ),
     )
     task = init_task.init_task(config=config)
-    make_symbolic_references.import_symbols(task)
-    split_arg_factories.lower_arg_factories(task)
+    task.auto_config_fn = None
+    newcg_symbolic_references.import_symbols(task)
     complex_to_variables.move_complex_nodes_to_variables(
         task,
         is_complex=complex_to_variables.more_complex_than(2),
     )
-    make_symbolic_references.replace_callables_and_configs_with_symbols(task)
+    newcg_symbolic_references.replace_callables_and_configs_with_symbols(task)
     code = ir_to_cst.code_for_task(task).code
 
     # Note: Wrapped some lines on spaces, since we don't compare whitespace.
     expected = """
+    import fiddle as fdl
     from fiddle._src.codegen.auto_config import test_fixtures
-    from fiddle import arg_factory
-    from fiddle.experimental import auto_config
-    import functools
-
 
-    @auto_config.auto_config
     def config_fixture():
-        initializer = functools.partial(test_fixtures.initializer,
+        initializer = fdl.ArgFactory(test_fixtures.initializer,
             name='const', dtype='float32')
-        return arg_factory.partial(test_fixtures.Attention,
-            kernel_init=initializer)
+        return fdl.Partial(test_fixtures.Attention, kernel_init=initializer)
     """
     self.assertEqual(code.split(), expected.split(), msg=code)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/naming.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/naming.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """API and default implementation for naming objects."""
 
 import abc
+import copy
 import dataclasses
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Set
 
 from fiddle import daglish
 from fiddle._src import config as config_lib
 from fiddle._src.codegen import namespace as namespace_lib
+from fiddle._src.codegen.auto_config import code_ir
 
 
 _camel_to_snake = namespace_lib.camel_to_snake  # pylint: disable=protected-access
 
 
 class NameGenerationError(ValueError):
   """Error thrown when a namer cannot deduce a name for a value."""
@@ -177,7 +179,24 @@
       candidates.append("root")
     if not candidates:
       raise NameGenerationError(
           f"Could not generate any candidate names for {value!r} with "
           f"paths {paths!r}"
       )
     return self.name_from_candidates(candidates)
+
+
+def get_task_existing_names(task: code_ir.CodegenTask) -> Set[str]:
+  """Get existing names from a CodegenTask."""
+  names = copy.copy(task.global_namespace.names)
+  names.update(
+      fn.name.value for fn in task.top_level_call.all_fixture_functions()
+  )
+  return names
+
+
+def get_fn_existing_names(fn: code_ir.FixtureFunction) -> Set[str]:
+  """Get existing names from a FixtureFunction."""
+  names = set()
+  names.update(parameter.name.value for parameter in fn.parameters)
+  names.update(variable.name.value for variable in fn.variables)
+  return names
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/naming_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/naming_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/parents_first_traversal.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/parents_first_traversal.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/shared_to_variables.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/shared_to_variables.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,26 +21,22 @@
 from fiddle import daglish
 from fiddle._src.codegen import namespace as namespace_lib
 from fiddle._src.codegen.auto_config import code_ir
 from fiddle._src.codegen.auto_config import naming
 from fiddle._src.codegen.auto_config import parents_first_traversal
 
 
-def _strip_paths(
-    paths: List[daglish.Path], depth: int = 1
-) -> List[daglish.Path]:
+def _strip_paths(paths: List[daglish.Path]) -> List[daglish.Path]:
   """Strips prefixes from paths."""
   seen = set()
   cleaned_paths = []
   for path in paths:
-    if len(path) > depth:
-      path = path[depth:]
-      if path not in seen:
-        seen.add(path)
-        cleaned_paths.append(path)
+    if path not in seen:
+      seen.add(path)
+      cleaned_paths.append(path)
   return cleaned_paths
 
 
 def move_shared_nodes_to_variables(
     task: code_ir.CodegenTask,
     *,
     make_namer: Callable[
@@ -52,41 +48,40 @@
   Args:
     task: Codegen task.
     make_namer: Function that will create a Namer, used for assigning new names
       to extracted variables. Note: Each path is relative to a FixtureFunction,
       not the overall config.
   """
 
-  all_fn_names = {
-      fn.name.value for fn in task.top_level_call.all_fixture_functions()
-  }
+  task_existing_names = naming.get_task_existing_names(task)
 
   def _process_fn(fn: code_ir.FixtureFunction) -> None:
     # Object IDs of values to extract into variables.
     to_extract_ids = set()
 
     def find_to_extract(value, parent_results: Any) -> Any:
       """Processes a node in a function definition."""
       if isinstance(
-          value, (code_ir.VariableReference, code_ir.SymbolReference)
+          value,
+          (code_ir.VariableReference, code_ir.SymbolReference, code_ir.Name),
       ):
         # Don't double-extract variables, and repeated symbol references are
         # fine.
         return
       elif len(parent_results) > 1:
         to_extract_ids.add(id(value))
 
-    parents_first_traversal.traverse_parents_first(find_to_extract, fn)
+    parents_first_traversal.traverse_parents_first(
+        find_to_extract, fn.output_value
+    )
 
     # Create a namer for new variables. But don't try to fix pre-existing bugs
     # if there are already conflicting names.
-    names = copy.copy(task.global_namespace.names)
-    names.update(all_fn_names)
-    names.update(parameter.name.value for parameter in fn.parameters)
-    names.update(variable.name.value for variable in fn.variables)
+    names = copy.copy(task_existing_names)
+    names.update(naming.get_fn_existing_names(fn))
     namer = make_namer(namespace_lib.Namespace(names))
 
     new_variables = []
 
     def traverse(value, state: daglish.State):
       """Actually moves shared values to variables."""
       original_value_id = id(value)
@@ -108,13 +103,13 @@
         name = namer.name_for(value, _strip_paths(state.get_all_paths()))
         name = code_ir.Name(name, is_generated=True)
         new_variables.append(code_ir.VariableDeclaration(name, value))
         return code_ir.VariableReference(name)
       else:
         return value
 
-    new_fn = daglish.MemoizedTraversal.run(traverse, fn)
-    new_fn.variables.extend(new_variables)
-    fn.replace_with(new_fn)
+    new_value = daglish.MemoizedTraversal.run(traverse, fn.output_value)
+    fn.output_value = new_value
+    fn.variables.extend(new_variables)
 
   for fn in task.top_level_call.all_fixture_functions():
     _process_fn(fn)
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/shared_to_variables_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/shared_to_variables_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,43 +10,42 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for shared_to_variables."""
-
+import dataclasses
+from typing import Any
 from absl.testing import absltest
+import fiddle as fdl
 from fiddle._src.codegen.auto_config import code_ir
 from fiddle._src.codegen.auto_config import init_task
 from fiddle._src.codegen.auto_config import ir_printer
 from fiddle._src.codegen.auto_config import make_symbolic_references
 from fiddle._src.codegen.auto_config import shared_to_variables
 from fiddle._src.codegen.auto_config import test_fixtures
 from fiddle._src.testing.example import fake_encoder_decoder
 
 
+@dataclasses.dataclass(frozen=True)
+class SampleClass:
+  x: Any
+  y: Any
+
+
 class SharedToVariablesTest(absltest.TestCase):
 
   def test_works_on_toy_example(self):
     task = test_fixtures.unprocessed_shared_config()
     make_symbolic_references.import_symbols(task)
     shared_to_variables.move_shared_nodes_to_variables(task)
     make_symbolic_references.replace_callables_and_configs_with_symbols(task)
     self.assertLen(task.top_level_call.fn.variables, 1)
 
-  def test_fails_on_unnameable_example(self):
-    shared = {"a": 7}
-    config = [shared, shared]
-    task = init_task.init_task(config)
-    with self.assertRaisesRegex(
-        ValueError, r"Could not generate any candidate names for \{'a': 7\}"
-    ):
-      shared_to_variables.move_shared_nodes_to_variables(task)
-
   def test_works_on_toy_example_two_vars(self):
     task = test_fixtures.unprocessed_two_shared_config()
     shared_to_variables.move_shared_nodes_to_variables(task)
     self.assertLen(task.top_level_call.fn.variables, 2)
 
     intermediate_code = ir_printer.format_task(task)
     self.assertIn("foo = ", intermediate_code)
@@ -54,31 +53,44 @@
     self.assertIn("return [shared_type, shared_type, foo]", intermediate_code)
 
   def test_fake_encoder_decoder(self):
     task = init_task.init_task(fake_encoder_decoder.fixture.as_buildable())
     shared_to_variables.move_shared_nodes_to_variables(task)
     self.assertLen(task.top_level_call.fn.variables, 1)
 
+  def test_shared_node_w_one_attr_in_path(self):
+    d = {
+        "map_1d": (("replica", "data"),),
+        "map_2d": (("replica", "data"), None),
+        "map_3d": (("replica", "data"), None, None),
+        "map_4d": (("replica", "data"), None, None, None),
+    }
+    config = fdl.Config(SampleClass, d, 2)
+    task = init_task.init_task(config)
+    shared_to_variables.move_shared_nodes_to_variables(task)
+
   def test_avoids_name_collisions(self):
     task = test_fixtures.unprocessed_shared_config()
 
     # Note: This doesn't strictly respect the API, the key should be a Call.
     # If this is ever required by another part of the code, then make up a
     # fake Call to use as a key.
-    task.top_level_call.children[None] = code_ir.CallInstance(
-        fn=code_ir.FixtureFunction(
-            code_ir.Name("shared_type"),
-            [],
-            [],
-            None,
-        ),
-        parent=None,
-        children={},
-        parameter_values={},
-        output_value=None,
+    task.top_level_call.children = []
+    task.top_level_call.children.append(
+        code_ir.CallInstance(
+            fn=code_ir.FixtureFunction(
+                code_ir.Name("shared_type"),
+                [],
+                [],
+                None,
+            ),
+            parent=None,
+            children=[],
+            parameter_values={},
+        )
     )
     shared_to_variables.move_shared_nodes_to_variables(task)
     intermediate_code = ir_printer.format_task(task)
     self.assertNotIn("shared_type =", intermediate_code)
 
 
 if __name__ == "__main__":
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/split_arg_factories.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/split_arg_factories.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/split_arg_factories_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/split_arg_factories_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/auto_config/test_fixtures.py` & `fiddle-0.2.7/fiddle/_src/codegen/auto_config/test_fixtures.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,14 +26,27 @@
 from fiddle._src.experimental import auto_config
 
 
 def foo(x):
   return x
 
 
+def bar(x, y):
+  del x
+  del y
+
+
+class ATag(fdl.Tag):
+  """Sample tag to test code generation of tags."""
+
+
+class BTag(fdl.Tag):
+  """Sample tag to test code generation of tags."""
+
+
 @dataclasses.dataclass
 class SharedType:
   x: int
   z: float
 
 
 global_counter = {"count": 0}
@@ -83,19 +96,55 @@
   fn = code_ir.FixtureFunction(
       name=code_ir.Name("simple_ir_fixture", is_generated=False),
       parameters=[],
       variables=[],
       output_value=config,
   )
   call_instance = code_ir.CallInstance(
-      fn, parent=None, children={}, parameter_values={}, output_value=config
+      fn, parent=None, children=[], parameter_values={}
   )
   return code_ir.CodegenTask(config, top_level_call=call_instance)
 
 
+def simple_ir_with_tags() -> code_ir.CodegenTask:
+  """Returns a single fixture bound to a config with a tag.
+
+  Code:
+
+  def config_fixture():
+    return fdl.Config(
+        bar,
+        x=ATag.new(1),
+        y=fdl.TaggedValue([ATag, BTag], default=2))
+  """
+  config = fdl.Config(
+      bar, x=ATag.new(1), y=fdl.TaggedValue([ATag, BTag], default=2)
+  )
+  return init_task.init_task(config)
+
+
+def simple_partial_ir_with_tags() -> code_ir.CodegenTask:
+  """Returns a single fixture bound to a Partial with a tag.
+
+  Code:
+
+  def config_fixture():
+    return fdl.Partial(
+        bar,
+        x=ATag.new(1),
+        y=fdl.TaggedValue([ATag, BTag], default=2))
+  """
+  partial = fdl.Partial(
+      bar,
+      x=ATag.new(1),
+      y=fdl.TaggedValue([ATag, BTag], default=2),
+  )
+  return init_task.init_task(partial)
+
+
 def simple_shared_variable_ir() -> code_ir.CodegenTask:
   """Returns a single fixture bound to a config.
 
   Code:
 
   def simple_shared_variable_ir_fixture():
     shared = {"a": 7}
@@ -111,15 +160,15 @@
       variables=[code_ir.VariableDeclaration(shared_name, shared)],
       output_value=[
           code_ir.VariableReference(shared_name),
           code_ir.VariableReference(shared_name),
       ],
   )
   call_instance = code_ir.CallInstance(
-      fn, parent=None, children={}, parameter_values={}, output_value=config
+      fn, parent=None, children=[], parameter_values={}
   )
   return code_ir.CodegenTask(config, top_level_call=call_instance)
 
 
 def unprocessed_shared_config() -> code_ir.CodegenTask:
   """Returns a single fixture bound to a config.
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/codegen.py` & `fiddle-0.2.7/fiddle/_src/codegen/legacy_codegen.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/codegen_diff.py` & `fiddle-0.2.7/fiddle/_src/codegen/codegen_diff.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/codegen_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/legacy_codegen_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """Tests for codegen."""
 import dataclasses
 import functools
 from typing import List
 
 from absl.testing import absltest
 import fiddle as fdl
-from fiddle._src.codegen import codegen
+from fiddle._src.codegen import legacy_codegen
 from fiddle._src.codegen import test_util
 from fiddle._src.codegen.test_submodule import test_util as submodule_test_util
 
 
 def tokens(code: str) -> List[str]:
   return code.strip().split()
 
@@ -102,23 +102,23 @@
 
 # Depending on how the test harness invokes this test, the expected values may
 # or may not include a module name.
 if __name__ == "__main__":
   this_module_import = ""
   this_module_prefix = ""
 else:
-  this_module_import = "from fiddle._src.codegen import codegen_test"
-  this_module_prefix = "codegen_test."
+  this_module_import = "from fiddle._src.codegen import legacy_codegen_test"
+  this_module_prefix = "legacy_codegen_test."
 
 
 class CodegenTest(absltest.TestCase):
 
   def test_codegen_dot_syntax_shared(self):
     cfg = shared_config()
-    result = codegen.codegen_dot_syntax(cfg)
+    result = legacy_codegen.codegen_dot_syntax(cfg)
     expected = f"""
 import fiddle as fdl
 {this_module_import}
 
 
 def build_config():
   shared_foo = fdl.Config({this_module_prefix}Foo)
@@ -137,15 +137,15 @@
     """
     actual_tokens = tokens("\n".join(result.lines()))
     self.assertSequenceEqual(actual_tokens, tokens(expected),
                              "\n".join(result.lines()))
 
   def test_codegen_multi_shared(self):
     cfg = multi_shared_config()
-    result = codegen.codegen_dot_syntax(cfg)
+    result = legacy_codegen.codegen_dot_syntax(cfg)
     expected = f"""
 import fiddle as fdl
 {this_module_import}
 
 
 def build_config():
   shared_foo = fdl.Config({this_module_prefix}Foo)
@@ -170,15 +170,15 @@
     """
     code = "\n".join(result.lines())
     self.assertSequenceEqual(tokens(code), tokens(expected), code)
 
   def test_codegen_import_and_exec(self):
     cfg = fdl.Config(
         test_util.Foo, a=1, leaves=[fdl.Config(test_util.Foo, a=2)])
-    result = codegen.codegen_dot_syntax(cfg)
+    result = legacy_codegen.codegen_dot_syntax(cfg)
     expected = """
 import fiddle as fdl
 from fiddle._src.codegen import test_util
 
 
 def build_config():
   root = fdl.Config(test_util.Foo)
@@ -204,15 +204,15 @@
     self.assertEqual(foo.a, 1)
     self.assertLen(foo.leaves, 1)
     self.assertEqual(foo.leaves[0].a, 2)
     self.assertEmpty(foo.leaves[0].leaves)
 
   def test_codegen_unshared_child_of_shared(self):
     cfg = unshared_child_of_shared()
-    result = codegen.codegen_dot_syntax(cfg)
+    result = legacy_codegen.codegen_dot_syntax(cfg)
     expected = f"""
 import fiddle as fdl
 {this_module_import}
 
 
 def build_config():
   shared_foo = fdl.Config({this_module_prefix}Foo)
@@ -238,15 +238,15 @@
     """
     actual_tokens = tokens("\n".join(result.lines()))
     self.assertSequenceEqual(actual_tokens, tokens(expected),
                              "\n".join(result.lines()))
 
   def test_codegen_partial(self):
     cfg = partial_config()
-    result = codegen.codegen_dot_syntax(cfg)
+    result = legacy_codegen.codegen_dot_syntax(cfg)
     expected = f"""
 import fiddle as fdl
 {this_module_import}
 
 
 def build_config():
   shared_foo = fdl.Partial({this_module_prefix}Foo)
@@ -262,30 +262,30 @@
     """
     actual_tokens = tokens("\n".join(result.lines()))
     self.assertSequenceEqual(actual_tokens, tokens(expected),
                              "\n".join(result.lines()))
 
   def test_codegen_inner_class_name(self):
     cfg = fdl.Config(test_util.NestedParent.Inner, a=4)
-    code = "\n".join(codegen.codegen_dot_syntax(cfg).lines())
+    code = "\n".join(legacy_codegen.codegen_dot_syntax(cfg).lines())
     expected = """
 import fiddle as fdl
 from fiddle._src.codegen import test_util
 
 def build_config():
   root = fdl.Config(test_util.NestedParent.Inner)
   root.a = 4
 
   return root
     """
     self.assertSequenceEqual(tokens(code), tokens(expected), code)
 
   def test_dict_value(self):
     cfg = fdl.Config(identity, x={"foo": fdl.Config(Foo, a=1)})
-    code = "\n".join(codegen.codegen_dot_syntax(cfg).lines())
+    code = "\n".join(legacy_codegen.codegen_dot_syntax(cfg).lines())
     expected = f"""
 import fiddle as fdl
 {this_module_import}
 
 
 def build_config():
   root = fdl.Config({this_module_prefix}identity)
@@ -296,15 +296,15 @@
 
   return root
     """
     self.assertSequenceEqual(tokens(code), tokens(expected), code)
 
   def test_deeply_nested_constant(self):
     cfg = fdl.Config(identity, x={"bar": [3, 4], "foo": [1, 2]})
-    code = "\n".join(codegen.codegen_dot_syntax(cfg).lines())
+    code = "\n".join(legacy_codegen.codegen_dot_syntax(cfg).lines())
     expected = f"""
 import fiddle as fdl
 {this_module_import}
 
 
 def build_config():
   root = fdl.Config({this_module_prefix}identity)
@@ -313,15 +313,15 @@
   return root
     """
     self.assertSequenceEqual(tokens(code), tokens(expected), code)
 
   def test_codegen_submodule(self):
     cfg = fdl.Config(
         submodule_test_util.Foo, a=1, leaves=[fdl.Config(test_util.Foo, a=4)])
-    code = "\n".join(codegen.codegen_dot_syntax(cfg).lines())
+    code = "\n".join(legacy_codegen.codegen_dot_syntax(cfg).lines())
     expected = """
 import fiddle as fdl
 from fiddle._src.codegen.test_submodule import test_util
 from fiddle._src.codegen import test_util as test_util_2
 
 
 def build_config():
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/formatting_utilities.py` & `fiddle-0.2.7/fiddle/_src/codegen/formatting_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 unambiguously by a name that differs from their qualified path. This library
 exposes the pretty-printing functionality that powers the codegen features to
 other string representations, such as graphviz or string serialization.
 """
 
 from typing import Any
 
-from fiddle._src.codegen import codegen
+from fiddle._src.codegen import legacy_codegen
 from fiddle._src.codegen import special_value_codegen
 
 
 class LazyImportManager(special_value_codegen.ImportManagerApi):
   """Import manager for GraphViz & string formatting.
 
   We create an instance of the codegen's import manager on every method call,
   which effectively will alias imports like 'jax.numpy' to 'jnp', but will not
   create new import aliases when two modules of the same name are referenced.
   """
 
   def add_by_name(self, module_name: str) -> str:
     """Returns the usable name generated from an ephemeral import manager."""
-    namespace = codegen.Namespace()
-    import_manager = codegen.ImportManager(namespace)
+    namespace = legacy_codegen.Namespace()
+    import_manager = legacy_codegen.ImportManager(namespace)
     return import_manager.add_by_name(module_name)
 
 
 def pretty_print(value: Any) -> str:
   """Returns the nicest eval-able string representation for `value`."""
   return repr(
       special_value_codegen.transform_py_value(value, LazyImportManager()))
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/import_manager.py` & `fiddle-0.2.7/fiddle/_src/codegen/import_manager.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/import_manager_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/import_manager_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/mini_ast.py` & `fiddle-0.2.7/fiddle/_src/codegen/mini_ast.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/namespace.py` & `fiddle-0.2.7/fiddle/_src/codegen/namespace.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/namespace_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/namespace_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/py_val_to_cst_converter.py` & `fiddle-0.2.7/fiddle/_src/codegen/py_val_to_cst_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Library for converting Python values to `cst` expressions."""
 
 import builtins
+import enum
 import functools
 import inspect
 import types
 from typing import Any, Callable, Union, Type, List, Optional, NamedTuple, Sequence
 
 from fiddle._src import config as config_lib
 from fiddle._src import tagging
@@ -392,7 +393,14 @@
   return cst.Call(
       func=conversion_fn(functools.partial),
       args=([cst.Arg(conversion_fn(value.func))] +
             [cst.Arg(conversion_fn(arg)) for arg in value.args] + [
                 kwarg_to_cst(arg_name, conversion_fn(arg_val))
                 for (arg_name, arg_val) in value.keywords.items()
             ]))
+
+
+@register_py_val_to_cst_converter(lambda value: isinstance(value, enum.Enum))
+def _convert_enum(value: Any, conversion_fn: PyValToCstFunc) -> cst.CSTNode:
+  return cst.Attribute(
+      value=conversion_fn(type(value)), attr=cst.Name(value.name)
+  )
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/py_val_to_cst_converter_test.py` & `fiddle-0.2.7/fiddle/_src/codegen/py_val_to_cst_converter_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for fiddle.codegen.py_val_to_cst_converter."""
 
+import enum
 import functools
 import inspect
 import logging.config
 import re
 import typing
 
 from absl.testing import absltest
@@ -43,14 +44,24 @@
   """Fiddle tag for testing."""
 
 
 def sample_fn(x, y, z):
   return (x, y, z)
 
 
+class MyEnum(enum.Enum):
+  FOO = 'foo'
+  BAR = 'bar'
+
+
+class MyStrEnum(str, enum.Enum):
+  FOO = 'foo'
+  BAR = 'bar'
+
+
 def _get_cst_code(cst_module):
   # Depending on how the tests are run, objects defined in this file might be
   # named "x" or "fiddle.codegen.py_val_to_cst_converter_test.x"; normalize.
   return cst_module.code.replace(
       'fiddle._src.codegen.py_val_to_cst_converter_test.', '')
 
 
@@ -107,14 +118,18 @@
       (slice, 'slice'),
       # Partials:
       (functools.partial(sample_fn), 'functools.partial(sample_fn)'),
       (
           functools.partial(sample_fn, 3, z=4),
           'functools.partial(sample_fn, 3, z=4)',
       ),
+      # Enums:
+      (MyEnum.FOO, 'MyEnum.FOO'),
+      (MyStrEnum.FOO, 'MyStrEnum.FOO'),
+      (re.RegexFlag.DOTALL, 're.RegexFlag.DOTALL'),
   ])
   def test_convert(self, pyval, expected):
     cst_expr = py_val_to_cst_converter.convert_py_val_to_cst(pyval)
     cst_module = cst.Module([cst.SimpleStatementLine([cst.Expr(cst_expr)])])
     self.assertEqual(_get_cst_code(cst_module), expected + '\n')
 
   def test_convert_multiple_tags(self):
```

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/special_value_codegen.py` & `fiddle-0.2.7/fiddle/_src/codegen/special_value_codegen.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/test_submodule/__init__.py` & `fiddle-0.2.7/fiddle/_src/codegen/test_submodule/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/test_submodule/test_util.py` & `fiddle-0.2.7/fiddle/_src/codegen/test_submodule/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/codegen/test_util.py` & `fiddle-0.2.7/fiddle/_src/codegen/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/config.py` & `fiddle-0.2.7/fiddle/_src/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import copy
 import dataclasses
 import functools
 import inspect
 import itertools
 import logging
 import types
-from typing import Any, Callable, Collection, Dict, FrozenSet, Generic, Iterable, Mapping, NamedTuple, Set, Tuple, Type, TypeVar, Union
+from typing import Any, Callable, Collection, Dict, FrozenSet, Generic, Iterable, Mapping, NamedTuple, Optional, Set, Tuple, Type, TypeVar, Union
 
 from fiddle._src import arg_factory
 from fiddle._src import daglish
 from fiddle._src import field_metadata
 from fiddle._src import history
 from fiddle._src import signatures
 from fiddle._src import tag_type
@@ -117,74 +117,78 @@
       fn_or_cls: Union['Buildable[T]', TypeOrCallableProducingT[T]],
       *args,
       **kwargs,
   ):
     """Initialize for ``fn_or_cls``, optionally specifying parameters.
 
     Args:
-      fn_or_cls: The function or class to configure, or a ``Buildable`` to copy.
+      fn_or_cls: A callable to configure. The signature of this callable will
+        determine the parameters this ``Buidlable`` can be used to configure.
       *args: Any positional arguments to configure for ``fn_or_cls``.
       **kwargs: Any keyword arguments to configure for ``fn_or_cls``.
     """
-    if isinstance(fn_or_cls, Buildable):
-      raise ValueError(
-          'Using the Buildable constructor to convert a buildable to a new '
-          'type or to override arguments is forbidden; please use either '
-          '`fdl.cast(new_type, buildable)` (for casting) or '
-          '`fdl.copy_with(buildable, **kwargs)` (for overriding arguments).'
-      )
-
-    # Using `super().__setattr__` here because assigning directly would trigger
-    # our `__setattr__` override. Using `super().__setattr__` instead of special
-    # casing these attribute names in `__setattr__` also has the effect of
-    # making them easily gettable but not as easily settable by user code.
-    super().__setattr__('__fn_or_cls__', fn_or_cls)
-    super().__setattr__('__arguments__', {})
-    signature = signatures.get_signature(fn_or_cls)
-    super().__setattr__('__signature__', signature)
-    has_var_keyword = any(
-        param.kind == param.VAR_KEYWORD
-        for param in signature.parameters.values()
-    )
+    signature = self.__init_callable__(fn_or_cls)
     arg_history = history.History()
     arg_history.add_new_value('__fn_or_cls__', fn_or_cls)
     super().__setattr__('__argument_history__', arg_history)
     super().__setattr__('__argument_tags__', collections.defaultdict(set))
-    super().__setattr__('_has_var_keyword', has_var_keyword)
 
     arguments = signature.bind_partial(*args, **kwargs).arguments
     for name in list(arguments.keys()):  # Make a copy in case we mutate.
       param = signature.parameters[name]
       if param.kind == param.VAR_POSITIONAL:
         # TODO(b/197367863): Add *args support.
         err_msg = (
             'Variable positional arguments (aka `*args`) not supported. '
             f'Found param `{name}` in `{fn_or_cls}`.'
         )
         raise NotImplementedError(err_msg)
       elif param.kind == param.VAR_KEYWORD:
         arguments.update(arguments.pop(param.name))
 
-    if hasattr(fn_or_cls, '__fiddle_init__'):
-      fn_or_cls.__fiddle_init__(self)
-
     if dataclasses.is_dataclass(self.__fn_or_cls__):
       fields = dataclasses.fields(self.__fn_or_cls__)
       _add_dataclass_tags(self, fields)
       _expand_dataclass_default_factories(self, fields, arguments)
 
     for name, value in arguments.items():
       setattr(self, name, value)
 
     for name, tags in tag_type.find_tags_from_annotations(fn_or_cls).items():
       self.__argument_tags__[name].update(tags)
       self.__argument_history__.add_updated_tags(
           name, self.__argument_tags__[name]
       )
 
+  def __init_callable__(
+      self, fn_or_cls: Union['Buildable[T]', TypeOrCallableProducingT[T]]
+  ) -> inspect.Signature:
+    if isinstance(fn_or_cls, Buildable):
+      raise ValueError(
+          'Using the Buildable constructor to convert a buildable to a new '
+          'type or to override arguments is forbidden; please use either '
+          '`fdl.cast(new_type, buildable)` (for casting) or '
+          '`fdl.copy_with(buildable, **kwargs)` (for overriding arguments).'
+      )
+
+    # Using `super().__setattr__` here because assigning directly would trigger
+    # our `__setattr__` override. Using `super().__setattr__` instead of special
+    # casing these attribute names in `__setattr__` also has the effect of
+    # making them easily gettable but not as easily settable by user code.
+    super().__setattr__('__fn_or_cls__', fn_or_cls)
+    super().__setattr__('__arguments__', {})
+    signature = signatures.get_signature(fn_or_cls)
+    super().__setattr__('__signature__', signature)
+    has_var_keyword = any(
+        param.kind == param.VAR_KEYWORD
+        for param in signature.parameters.values()
+    )
+    super().__setattr__('_has_var_keyword', has_var_keyword)
+    return signature
+
   def __init_subclass__(cls):
     daglish.register_node_traverser(
         cls,
         flatten_fn=lambda x: x.__flatten__(),
         unflatten_fn=cls.__unflatten__,
         path_elements_fn=lambda x: x.__path_elements__(),
     )
@@ -194,36 +198,40 @@
     """Builds output for this instance; see subclasses for details."""
     raise NotImplementedError()
 
   def __flatten__(self) -> Tuple[Tuple[Any, ...], BuildableTraverserMetadata]:
     arguments = ordered_arguments(self)
     keys = tuple(arguments.keys())
     values = tuple(arguments.values())
-    tags = {
-        name: frozenset(tags) for name, tags in self.__argument_tags__.items()
+    argument_tags = {
+        name: frozenset(tags)
+        for name, tags in self.__argument_tags__.items()
+        if tags  # Don't include empty sets.
     }
     argument_history = {
         name: tuple(entries)
         for name, entries in self.__argument_history__.items()
     }
     metadata = BuildableTraverserMetadata(
         fn_or_cls=self.__fn_or_cls__,
         argument_names=keys,
-        argument_tags=tags,
+        argument_tags=argument_tags,
         argument_history=argument_history,
     )
     return values, metadata
 
   @classmethod
   def __unflatten__(
       cls, values: Iterable[Any], metadata: BuildableTraverserMetadata
   ):
-    rebuilt = cls(metadata.fn_or_cls, **metadata.arguments(values))  # pytype: disable=not-instantiable
+    rebuilt = cls.__new__(cls)
+    rebuilt.__init_callable__(metadata.fn_or_cls)
     object.__setattr__(rebuilt, '__argument_tags__', metadata.tags())
     object.__setattr__(rebuilt, '__argument_history__', metadata.history())
+    object.__setattr__(rebuilt, '__arguments__', metadata.arguments(values))
     return rebuilt
 
   def __path_elements__(self):
     return tuple(daglish.Attr(name) for name in ordered_arguments(self).keys())
 
   def __getattr__(self, name: str):
     """Get parameter with given ``name``."""
@@ -293,17 +301,30 @@
       raise TypeError(err_msg)
 
   def __setattr__(self, name: str, value: Any):
     """Sets parameter ``name`` to ``value``."""
 
     self.__validate_param_name__(name)
 
+    if isinstance(value, TaggedValueCls):
+      tags = value.__argument_tags__.get('value', ())
+      if tags:
+        self.__argument_tags__[name].update(tags)
+        self.__argument_history__.add_updated_tags(
+            name, self.__argument_tags__[name]
+        )
+      if 'value' in value.__arguments__:
+        # Must pull from underlying dictionary to preserve TiedValue's.
+        value = value.__arguments__['value']
+      else:
+        return
+
     # Actually set the value, handling TiedValue's as a special case.
     current = self.__arguments__.get(name)
-    if isinstance(current, TiedValue):
+    if isinstance(current, TiedValue) and not isinstance(value, TiedValue):
       # This will create a history entry in the TiedValue as well. (Seems
       # reasonable, but not clear what's best?)
       current.value = value
     else:
       self.__arguments__[name] = value
 
     self.__argument_history__.add_new_value(name, value)
@@ -672,43 +693,31 @@
 
       def test_function(arg, kwarg=None):
         return arg, kwarg
 
       fn_config = Config(test_function, 1)
       fn_config.kwarg = 'kwarg'
 
-  A ``Config`` instance may be transformd into instances and function outputs by
-  passing it to the ``build`` function. The ``build`` function invokes each
+  A ``Config`` instance may be transformed into instances and function outputs
+  by passing it to the ``build`` function. The ``build`` function invokes each
   function or class in the configuration tree (appropriately propagating the
   built outputs from nested ``Config``'s). For example, using the
   ``SampleClass`` config from above::
 
       instance = build(class_config)
-      assert instance.arg == 'arg'
+      assert instance.arg == 1
       assert instance.kwarg == 'kwarg'
 
   If the same ``Config`` instance is used in multiple places within the
   configuration tree, its function or class is invoked only once during
   ``build``, and the result shared across all occurences of the ``Config``
   instance. (See ``build`` documentation for further details.) To create a new
   instance of a ``Config`` with the same parameter settings that will yield a
   separate instance during ``build``, ``copy.copy()`` or ``copy.deepcopy()``
   may be used.
-
-  A class or function can customize the Config instance by defining a
-  ``__fiddle_init__`` property. For example::
-
-      class MyClass:
-        def __init__(self, x, y, z):
-          ...
-
-        @staticmethod
-        def __fiddle_init__(cfg):
-          cfg.y = 42
-          cfg.z = Config(MyOtherClass)
   """
 
   # NOTE(b/201159339): We currently need to repeat these annotations for pytype.
   __fn_or_cls__: TypeOrCallableProducingT[T]
   __signature__: inspect.Signature
 
   def __build__(self, *args, **kwargs):
@@ -723,14 +732,64 @@
     Returns:
       The result of calling ``self.__fn_or_cls__`` with the given ``args`` and
       ``kwargs``.
     """
     return self.__fn_or_cls__(*args, **kwargs)
 
 
+def tagged_value_fn(
+    value: Union[T, NoValue], tags: Optional[Set[tag_type.TagType]] = None
+) -> T:
+  """Identity function to return value if set, and raise an error if not.
+
+  Args:
+    value: The value to return.
+    tags: The tags associated with the value. (Used in generating error messages
+      if `value` is not set.)
+
+  Returns:
+    The value `value` passed to it.
+  """
+  if value is NO_VALUE:
+    msg = (
+        'Expected all `TaggedValue`s to be replaced via fdl.set_tagged() '
+        'calls, but one was not set.'
+    )
+    if tags:
+      msg += ' Unset tags: ' + str(tags)
+    raise tag_type.TaggedValueNotFilledError(msg)
+  return value
+
+
+class TaggedValueCls(Generic[T], Config[T]):
+  """Placeholder class for TaggedValue instances.
+
+  Instances of this class are generally transitory; when passed as an argument
+  of a Fiddle Buildable, will be expanded into that argument's values and tags.
+  However, they may survive as stand-alone objects within tuples, lists, and
+  dictionaries.
+  """
+
+  # NOTE(b/201159339): We currently need to repeat these annotations for pytype.
+  __fn_or_cls__: TypeOrCallableProducingT[T]
+  __signature__: inspect.Signature
+
+  @property
+  def tags(self):
+    return self.__argument_tags__['value']
+
+  def __build__(self, *args: Any, **kwargs: Any) -> T:
+    if self.__fn_or_cls__ is not tagged_value_fn:
+      raise RuntimeError(
+          'Unexpected __fn_or_cls__ in TaggedValueCls; found:'
+          f'{self.__fn_or_cls__}'
+      )
+    return self.__fn_or_cls__(tags=self.tags, *args, **kwargs)
+
+
 class TiedValue(Generic[T], Config[T]):
   """Class implementing tied values.
 
   The implementation/declaration is here, so that we can write __getattr__ and
   __setattr__ buildable hooks to eliminate the extra ``.value`` when it is a
   field attribute, but please use ``experimental/tied_value.py`` for the public
   API.
@@ -1149,15 +1208,15 @@
   result = {}
   for name, param in buildable.__signature__.parameters.items():
     if param.kind != param.VAR_KEYWORD:
       if name in buildable.__arguments__:
         value = buildable.__arguments__[name]
         if (not exclude_equal_to_default) or (value != param.default):
           result[name] = value
-      elif param.default != param.empty:
+      elif param.default is not param.empty:
         if include_defaults:
           result[name] = param.default
       elif include_unset:
         result[name] = NO_VALUE
   if include_var_keyword:
     for name, value in buildable.__arguments__.items():
       param = buildable.__signature__.parameters.get(name)
```

### Comparing `fiddle-0.2.6/fiddle/_src/config_test.py` & `fiddle-0.2.7/fiddle/_src/config_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """Tests for the `fiddle.config` module."""
 
 import copy
 import dataclasses
 import functools
 import pickle
 import threading
-from typing import Any, Callable, Dict
+from typing import Any, Callable, Dict, Generic, TypeVar
 
 from absl.testing import absltest
 from absl.testing import parameterized
 import fiddle as fdl
 from fiddle import arg_factory
 from fiddle import daglish
 from fiddle import history
@@ -71,77 +71,14 @@
   return locals()
 
 
 def fn_with_var_args_and_kwargs(arg1, *args, kwarg1=None, **kwargs):  # pylint: disable=unused-argument
   return locals()
 
 
-class FiddleInitStaticMethod:
-
-  def __init__(self, x, y=3, **kwargs):
-    self.x = x
-    self.y = y
-    for key, value in kwargs.items():
-      setattr(self, key, value)
-
-  @staticmethod
-  def __fiddle_init__(cfg):
-    cfg.z = 5
-
-
-class FiddleInitStaticMethodChild(FiddleInitStaticMethod):
-
-  @classmethod
-  def __fiddle_init__(cls, cfg):
-    super().__fiddle_init__(cfg)
-    cfg.w = 42
-
-
-class FiddleInitClassMethod:
-
-  def __init__(self, x, y=3, **kwargs):
-    self.x = x
-    self.y = y
-    for key, value in kwargs.items():
-      setattr(self, key, value)
-
-  @classmethod
-  def __fiddle_init__(cls, cfg):
-    cfg.z = 5
-
-
-class FiddleInitClassMethodChild(FiddleInitClassMethod):
-
-  @classmethod
-  def __fiddle_init__(cls, cfg):
-    super().__fiddle_init__(cfg)
-    cfg.w = 10
-
-
-class FiddleInitIncompatibleChild(FiddleInitClassMethod):
-
-  def __init__(self, a, b):
-    self.a = a
-    self.b = b
-    super().__init__(x=a + 1, y=b - 3, z=a + b)
-
-  @classmethod
-  def __fiddle_init__(cls, cfg):
-    # Since FiddleInitClassMethod has different init arguments, we cannot call
-    # super().__fiddle_init__(cfg).
-    super_cfg = fdl.Config(FiddleInitClassMethod)
-    cfg.b = super_cfg.y + 3  # Demonstrate copying over.
-
-
-class FiddleInitIncompatibleChildBroken(FiddleInitClassMethod):
-
-  def __init__(self, a, b):  # pylint: disable=super-init-not-called
-    pass
-
-
 def make_typed_config() -> fdl.Config[SampleClass]:
   """Helper function which returns a fdl.Config whose type is known."""
   return fdl.Config(SampleClass, arg1=1, arg2=2)
 
 
 def make_untyped_config(arg_to_configure, **kwargs) -> fdl.Config:
   """Helper function which returns an untyped fdl.Config."""
@@ -186,14 +123,22 @@
   three: 'Annotated[float, Tag2]'
 
 
 def raise_error():
   raise ValueError('My fancy exception')
 
 
+_T = TypeVar('_T')
+
+
+@dataclasses.dataclass
+class GenericClass(Generic[_T]):
+  x: _T = 1
+
+
 class ConfigTest(parameterized.TestCase):
 
   def test_config_for_classes(self):
     class_config = fdl.Config(SampleClass, 1, kwarg2='kwarg2')
     pytype_extensions.assert_type(class_config, fdl.Config[SampleClass])
     self.assertEqual(class_config.arg1, 1)
     self.assertEqual(class_config.kwarg2, 'kwarg2')
@@ -281,94 +226,14 @@
 
   def test_config_for_dicts(self):
     dict_config = fdl.Config(dict, a=1, b=2)
     dict_config.c = 3
     instance = fdl.build(dict_config)
     self.assertEqual(instance, {'a': 1, 'b': 2, 'c': 3})
 
-  def test_fiddle_init_config_static(self):
-    cfg = fdl.Config(FiddleInitStaticMethod)
-    self.assertEqual(5, cfg.z)
-    cfg.x = 1
-    obj = fdl.build(cfg)
-    self.assertIsInstance(obj, FiddleInitStaticMethod)
-    self.assertEqual(1, obj.x)
-    self.assertEqual(3, obj.y)
-    self.assertEqual(5, obj.z)  # pytype: disable=attribute-error
-
-  def test_fiddle_init_partial_static(self):
-    cfg = fdl.Partial(FiddleInitStaticMethod)
-    self.assertEqual(5, cfg.z)
-    partial = fdl.build(cfg)
-    obj = partial(x=1)
-    self.assertIsInstance(obj, FiddleInitStaticMethod)
-    self.assertEqual(1, obj.x)
-    self.assertEqual(3, obj.y)
-    self.assertEqual(5, obj.z)  # pytype: disable=attribute-error
-
-  def test_fiddle_init_config_static_subclass(self):
-    cfg = fdl.Config(FiddleInitStaticMethodChild)
-    self.assertEqual(3, cfg.y)
-    self.assertEqual(5, cfg.z)
-    self.assertEqual(42, cfg.w)
-    cfg.x = 1
-    obj = fdl.build(cfg)
-    self.assertIsInstance(obj, FiddleInitStaticMethodChild)
-    self.assertEqual(42, obj.w)  # pytype: disable=attribute-error
-    self.assertEqual(1, obj.x)
-    self.assertEqual(3, obj.y)
-    self.assertEqual(5, cfg.z)  # pytype: disable=attribute-error
-
-  def test_fiddle_init_config_class(self):
-    cfg = fdl.Config(FiddleInitClassMethod, 1)
-    self.assertEqual(5, cfg.z)
-    obj = fdl.build(cfg)
-    self.assertIsInstance(obj, FiddleInitClassMethod)
-    self.assertEqual(1, obj.x)
-    self.assertEqual(3, obj.y)
-    self.assertEqual(5, obj.z)  # pytype: disable=attribute-error
-
-  def test_fiddle_init_partial_class(self):
-    cfg = fdl.Partial(FiddleInitClassMethod, 1)
-    self.assertEqual(5, cfg.z)
-    partial = fdl.build(cfg)
-    obj = partial(x=1)
-    self.assertIsInstance(obj, FiddleInitClassMethod)
-    self.assertEqual(1, obj.x)
-    self.assertEqual(3, obj.y)
-    self.assertEqual(5, obj.z)  # pytype: disable=attribute-error
-
-  def test_fiddle_init_config_subclass(self):
-    cfg = fdl.Config(FiddleInitClassMethodChild, 0)
-    self.assertEqual(5, cfg.z)
-    self.assertEqual(10, cfg.w)
-    obj = fdl.build(cfg)
-    self.assertIsInstance(obj, FiddleInitClassMethodChild)
-    self.assertEqual(0, obj.x)
-    self.assertEqual(3, obj.y)
-    self.assertEqual(5, obj.z)  # pytype: disable=attribute-error
-    self.assertEqual(10, obj.w)  # pytype: disable=attribute-error
-
-  def test_fiddle_init_incompatible_subclass(self):
-    cfg = fdl.Config(FiddleInitIncompatibleChild)
-    self.assertEqual(6, cfg.b)
-    cfg.a = 8
-    obj = fdl.build(cfg)
-    self.assertIsInstance(obj, FiddleInitIncompatibleChild)
-    self.assertEqual(8, obj.a)
-    self.assertEqual(9, obj.x)
-    self.assertEqual(6, obj.b)
-    self.assertEqual(3, obj.y)
-    self.assertEqual(14, obj.z)  # pytype: disable=attribute-error
-
-  def test_fiddle_init_incompatible_broken(self):
-    with self.assertRaisesRegex(
-        TypeError, 'No parameter named.*; valid parameter names: a, b'):
-      _ = fdl.Config(FiddleInitIncompatibleChildBroken)
-
   def test_config_with_default_args(self):
 
     def my_func(x: int = 2, y: str = 'abc'):  # pylint: disable=unused-argument
       return locals()
 
     cfg = fdl.Config(my_func)
     self.assertEqual(2, cfg.x)
@@ -620,14 +485,42 @@
     cfg2 = fdl.Config(SampleClass, 1, 2, None, kwarg2=None)
     self.assertEqual(cfg1, cfg2)
 
     cfg1 = fdl.Config(basic_fn, 1, 2)
     cfg2 = fdl.Config(basic_fn, 1, 2, None, kwarg2=None)
     self.assertEqual(cfg1, cfg2)
 
+  def test_default_value_for_generic_classes(self):
+    self.assertEqual(fdl.Config(GenericClass).x, 1)
+    self.assertEqual(fdl.Config(GenericClass[int]).x, 1)
+
+  def test_config_with_non_comparable_values(self):
+    # This test ensures that fdl.Config and fdl.build work properly with
+    # argument defaults that don't support equality testing. Something related
+    # can come up with NumPy arrays, which test for equality against scalars in
+    # an elementwise fashion, and subsequently can't directly be coerced to a
+    # bool (e.g., used as the condition in an if statement).
+
+    @dataclasses.dataclass(frozen=True, eq=False)
+    class ClassWithDisabledEquality:
+
+      def __eq__(self, _):
+        raise NotImplementedError()
+
+    def fn_with_non_comparable_default(
+        value1, value2=ClassWithDisabledEquality()
+    ):
+      return value1, value2
+
+    cfg = fdl.Config(fn_with_non_comparable_default)
+    cfg.value1 = ClassWithDisabledEquality()
+    value1, value2 = fdl.build(cfg)
+    self.assertIsInstance(value1, ClassWithDisabledEquality)
+    self.assertIsInstance(value2, ClassWithDisabledEquality)
+
   def test_unsetting_argument(self):
     fn_config = fdl.Config(basic_fn)
     fn_config.arg1 = 3
     fn_config.arg2 = 4
 
     del fn_config.arg1
 
@@ -662,14 +555,62 @@
   def test_tag_annotations(self):
     cfg = fdl.Config(DataclassAnnotated)
 
     self.assertEqual(frozenset([Tag1]), fdl.get_tags(cfg, 'one'))
     self.assertEqual(frozenset([Tag1, Tag2]), fdl.get_tags(cfg, 'two'))
     self.assertEqual(frozenset([Tag2]), fdl.get_tags(cfg, 'three'))
 
+  def test_tags_flattening_and_unflattening(self):
+    def flatten_unflatten(config):
+      values, metadata = config.__flatten__()
+      return type(config).__unflatten__(values, metadata)
+
+    with self.subTest('tagged_field_without_value'):
+      cfg = fdl.Config(DataclassAnnotated)
+      self.assertEqual(frozenset([Tag1]), fdl.get_tags(cfg, 'one'))
+      cfg2 = flatten_unflatten(cfg)
+      self.assertEqual(frozenset([Tag1]), fdl.get_tags(cfg2, 'one'))
+
+    with self.subTest('untagged_field_without_value'):
+      cfg = fdl.Config(DataclassAnnotated)
+      fdl.clear_tags(cfg, 'one')
+      self.assertEqual(frozenset([]), fdl.get_tags(cfg, 'one'))
+      cfg2 = flatten_unflatten(cfg)
+      self.assertEqual(frozenset([]), fdl.get_tags(cfg2, 'one'))
+
+    with self.subTest('tagged_field_with_value'):
+      cfg = fdl.Config(DataclassAnnotated)
+      cfg.one = fdl.TaggedValue([Tag2], 3)
+      self.assertEqual(frozenset([Tag1, Tag2]), fdl.get_tags(cfg, 'one'))
+      cfg2 = flatten_unflatten(cfg)
+      self.assertEqual(frozenset([Tag1, Tag2]), fdl.get_tags(cfg2, 'one'))
+
+    with self.subTest('untagged_field_with_value'):
+      cfg = fdl.Config(DataclassAnnotated)
+      cfg.one = 3
+      fdl.clear_tags(cfg, 'one')
+      self.assertEqual(frozenset([]), fdl.get_tags(cfg, 'one'))
+      cfg2 = flatten_unflatten(cfg)
+      self.assertEqual(frozenset([]), fdl.get_tags(cfg2, 'one'))
+
+  def test_setting_tagged_values_with_daglish_traversal(self):
+    cfg = fdl.Config(DataclassAnnotated, one=3)
+
+    def traverse(value, state):
+      if isinstance(value, int):
+        return fdl.TaggedValue([Tag2], value)
+      else:
+        return state.map_children(value)
+
+    # We expect the TaggedValue class *not* to be unwrapped by the constructor
+    # now, because __new__ is called directly.
+    cfg2 = traverse(cfg, daglish.MemoizedTraversal.begin(traverse, cfg))
+    self.assertEqual(frozenset([Tag1]), fdl.get_tags(cfg2, 'one'))
+    self.assertEqual(frozenset([Tag2]), fdl.get_tags(cfg2.one, 'value'))
+
   def test_clear_tags(self):
     cfg = fdl.Config(SampleClass)
     fdl.add_tag(cfg, 'arg1', Tag1)
     fdl.add_tag(cfg, 'arg1', Tag2)
     fdl.clear_tags(cfg, 'arg1')
     self.assertEqual(frozenset([]), fdl.get_tags(cfg, 'arg1'))
 
@@ -1017,19 +958,45 @@
 
   def test_build_raises_nice_error_too_few_args(self):
     cfg = fdl.Config(basic_fn, fdl.Config(SampleClass, 1), 2)
     with self.assertRaisesRegex(
         TypeError, r'.*missing 1 required.*\n\n.*<root>\.arg1.*arg1=1'):
       fdl.build(cfg)
 
-  def test_build_raises_exception_on_call(self):
+  def test_build_reraises_nice_error_with_tag_information(self):
+    cfg = fdl.Config(SampleClass)
+    fdl.add_tag(cfg, 'arg2', Tag1)
+
+    with self.assertRaisesRegex(
+        TypeError,
+        r'.*Tags for unset arguments:\n - arg2: #{module}.Tag1.*'.format(
+            module=__name__
+        ),
+    ):
+      fdl.build(cfg)
 
+  def test_build_reraises_nice_error_multiple_tags(self):
+    cfg = fdl.Config(SampleClass)
+    fdl.add_tag(cfg, 'arg1', Tag2)
+    fdl.add_tag(cfg, 'arg2', Tag1)
+    fdl.add_tag(cfg, 'arg2', Tag2)
+
+    expected_match = (
+        r'.* - arg1: #{module}.Tag2\n - arg2: #{module}.Tag1 #{module}.Tag2.*'
+        .format(module=__name__)
+    )
+    with self.assertRaisesRegex(TypeError, expected_match):
+      fdl.build(cfg)
+
+  def test_build_raises_exception_on_call(self):
     cfg = fdl.Config(raise_error)
-    msg = ('My fancy exception\n\nFiddle context: failed to construct or call '
-           'raise_error at <root> with arguments ()')
+    msg = (
+        'My fancy exception\n\nFiddle context: failed to construct or call '
+        'raise_error at <root> with arguments ()'
+    )
     with self.assertRaisesWithLiteralMatch(ValueError, msg):
       fdl.build(cfg)
 
   def test_build_error_path(self):
     # This will raise an error, because it doesn't have one arg populated.
     sub_cfg = fdl.Config(basic_fn, 1)
     sub_dict = {'a': 0, 'b': 2, 'c': sub_cfg, 'd': 10}
```

### Comparing `fiddle-0.2.6/fiddle/_src/daglish.py` & `fiddle-0.2.7/fiddle/_src/daglish.py`

 * *Files 3% similar despite different names*

```diff
@@ -353,14 +353,17 @@
   apply to are constants, such as booleans, strings, and small integers.
 
   The interning optimization may be applied to (nested) tuples whose
   values are constants.
 
   Args:
     value: any value, it can be a Fiddle buildable or a regular Python value.
+
+  Returns:
+    A bool indicating whether interning optimization is applicable to `value`.
   """
   return not is_memoizable(value) or (
       # We want tuples only and not things like NamedTuples which are not
       # interned by Python.
       # pylint: disable-next=unidiomatic-typecheck
       type(value) is tuple and all(is_internable(e) for e in value))
 
@@ -602,15 +605,16 @@
 
   def all_paths_to_object(self, object_id: int,
                           allow_caching: bool) -> List[Path]:
     if allow_caching and object_id in self.paths_cache:
       return self.paths_cache[object_id]
     else:
       all_paths = self.paths_cache = collect_paths_by_id(
-          self.root_obj, memoizable_only=True)
+          self.root_obj, memoizable_only=True, registry=self.registry
+      )
       return all_paths[object_id]
 
 
 @dataclasses.dataclass
 class MemoizedTraversal(BasicTraversal):
   """Traversal that memoizes results.
 
@@ -620,18 +624,24 @@
       leaf value, by default the traversal will only visit it once, and reuse
       the results. However, if you are writing a traversal that cares about
       paths to the value "4", you might want to set this to False so it is
       visited multiple times.
     memo: Memoization dictionary mapping `id(value)` to the tuple `(value,
       result)`, where `value` is a traversed node and `result` is the value
       returned by `apply` for `value`.
+    _cycle_start: Dictionary used for cycle detection.  When the traversal is
+      applied to a value, `_cycle_start[id(value)]` is temporarily set to the
+      current the `state`.  Once the result has been computed,
+      `_cycle_start[id(value)]` is deleted.  If a cycle is detected during
+      traversal, `MemoizedTraversal` raises a `ValueError`.
   """
 
   memoize_internables: bool = True
   memo: Dict[int, Tuple[Any, Any]] = dataclasses.field(default_factory=dict)
+  _cycle_start: Dict[int, State] = dataclasses.field(default_factory=dict)
 
   @classmethod
   def begin(cls,
             fn: Callable[..., Any],
             root_obj: Any,
             memoize_internables: bool = True) -> State:
     """Creates a new traversal and returns the initial state.
@@ -650,38 +660,54 @@
     """
     return cls(
         traversal_fn=fn,
         root_obj=root_obj,
         memoize_internables=memoize_internables).initial_state()
 
   def apply(self, value, state):
+    value_id = id(value)
     if not self.memoize_internables and is_internable(value):
       return self.traversal_fn(value, state)
-    elif id(value) in self.memo:
-      return self.memo[id(value)][1]
+    elif value_id in self.memo:
+      return self.memo[value_id][1]
+    elif value_id in self._cycle_start:
+      original_state = self._cycle_start[value_id]
+      raise ValueError(
+          "Fiddle detected a cycle while traversing a value: "
+          f"<root>{path_str(original_state.current_path)} is "
+          f"<root>{path_str(state.current_path)}."
+          " Configurations with cycles are not supported."
+      )
     else:
+      self._cycle_start[value_id] = state
       result = self.traversal_fn(value, state)
-      self.memo[id(value)] = (value, result)
+      self.memo[value_id] = (value, result)
+      del self._cycle_start[value_id]
       return result
 
 
-def collect_paths_by_id(structure,
-                        memoizable_only=False) -> Dict[int, List[Path]]:
+def collect_paths_by_id(
+    structure,
+    memoizable_only=False,
+    *,
+    registry: NodeTraverserRegistry = _default_traverser_registry,
+) -> Dict[int, List[Path]]:
   """Returns a dict mapping id(v)->paths for all `v` traversable from structure.
 
   I.e., if `result = collect_paths_by_id(structure)`, then `result[id(v)]` is
   the list of every path `p` such that `follow_path(structure, p) is v`.
 
   This dict only includes values `v` for which `is_memoizable(v)` is true.
 
   Args:
     structure: The structure for which the id->paths mapping should be created.
     memoizable_only: If true, then only include values `v` for which
       `is_memoizable(v)` is true.  Currently required to be True, to avoid bugs
       that can result from Python's interning optimizations.
+    registry: Node traversal registry used to collect paths.
   """
   if not memoizable_only:
     raise ValueError(
         "Including non-memoizable objects when collecting paths by id may "
         "cause problems, because of Python's interning optimizations.  If you "
         "are sure this is what you need, contact the Fiddle team, and we can "
         "look into enabling this flag.")
@@ -689,15 +715,16 @@
 
   def traverse(value, state: State):
     if not memoizable_only or is_memoizable(value):
       paths_by_id.setdefault(id(value), []).append(state.current_path)
     if state.is_traversable(value):
       state.flattened_map_children(value)
 
-  BasicTraversal.run(traverse, structure)
+  traversal = BasicTraversal(traverse, structure, registry=registry)
+  traverse(structure, traversal.initial_state())
   return paths_by_id
 
 
 def iterate(
     value: Any,
     memoized: bool = True,
     registry: NodeTraverserRegistry = _default_traverser_registry,
```

### Comparing `fiddle-0.2.6/fiddle/_src/daglish_test.py` & `fiddle-0.2.7/fiddle/_src/daglish_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 """Tests for daglish."""
 
 import collections
 import dataclasses
 import enum
 import json
 import random
-from typing import Any, List, NamedTuple, Optional, Type, cast
+from typing import Any, List, NamedTuple, Optional, cast
 
 from absl.testing import absltest
 from absl.testing import parameterized
-
 import fiddle as fdl
 from fiddle import daglish
 from fiddle import history
+from fiddle._src.experimental import dataclasses as fdl_dc
 from fiddle._src.testing import nested_values
 from fiddle._src.testing import test_util
 
 
 @dataclasses.dataclass
 class Foo:
   bar: Any
@@ -87,53 +87,14 @@
     return fdl.ordered_arguments(value)
   elif isinstance(value, enum.Enum):
     return str(value)
   else:
     return value
 
 
-# Dataclasses iterator registry
-class DataclassType:
-  """Sentinel class for registry lookup."""
-
-
-class DataclassAwareRegistry(daglish.NodeTraverserRegistry):
-
-  def find_node_traverser(
-      self, node_type: Type[Any]) -> Optional[daglish.NodeTraverser]:
-    if dataclasses.is_dataclass(node_type):
-      node_type = DataclassType
-    return super().find_node_traverser(node_type)
-
-
-dataclass_registry = DataclassAwareRegistry(use_fallback=True)
-
-
-def _flatten_dataclass(value):
-  as_dict = dataclasses.asdict(value)
-  return tuple(as_dict.values()), (tuple(as_dict.keys()), type(value))
-
-
-def _unflatten_dataclass(values, metadata):
-  keys, class_type = metadata
-  return class_type(**dict(zip(keys, values)))
-
-
-def _dataclass_path_elements(value):
-  return [daglish.Attr(field.name) for field in dataclasses.fields(value)]
-
-
-dataclass_registry.register_node_traverser(
-    DataclassType,
-    flatten_fn=_flatten_dataclass,
-    unflatten_fn=_unflatten_dataclass,
-    path_elements_fn=_dataclass_path_elements,
-)
-
-
 class PathTest(parameterized.TestCase):
 
   @parameterized.named_parameters(
       dict(
           testcase_name="exact_match",
           prefix_path=".foo.bar",
           containing_path=".foo.bar",
@@ -506,21 +467,25 @@
             (config, ""),
             (config["dataclass"], "['dataclass']"),
         ])
 
   def test_walk_dataclass_dataclass_aware_traverser(self):
     config = {"dataclass": Foo(3, fdl.Config(sample_fn, "arg"))}
     self.assertEqual(
-        _iterate_path_strings(config, registry=dataclass_registry), [
+        _iterate_path_strings(
+            config, registry=fdl_dc.daglish_dataclass_registry
+        ),
+        [
             (config, ""),
             (config["dataclass"], "['dataclass']"),
             (3, "['dataclass'].bar"),
             (fdl.Config(sample_fn, "arg"), "['dataclass'].baz"),
             ("arg", "['dataclass'].baz.arg"),
-        ])
+        ],
+    )
 
 
 class MemoizedTraversalTest(absltest.TestCase):
 
   def test_unique_traversals_for_different_ids(self):
     # This test generates a bunch of new objects during traversal, which if
     # cached incorrectly will result in false positive cache hits. (This is
@@ -538,10 +503,79 @@
         return result
       else:
         raise AssertionError("Should not be reached, got " + str(value))
 
     result = daglish.MemoizedTraversal.run(traverse, list(range(10_000)))
     self.assertEqual(result, 50_005_000)
 
+  def test_cycle_detection(self):
+    def traverse(value, state: daglish.State):
+      return state.map_children(value)
+
+    x = [1, 2, 3]
+    x.append(x)
+    with self.assertRaisesRegex(
+        ValueError,
+        "Fiddle detected a cycle while traversing a value: "
+        r"<root>\[3\] is <root>\[3\]\[3\]\.",
+    ):
+      daglish.MemoizedTraversal.run(traverse, x)
+
+  def test_cycle_detection_in_fdl_build(self):
+    cfg = fdl.Config(Foo, bar=fdl.Config(Foo))
+    cfg.bar.bar = cfg
+    with self.assertRaisesRegex(
+        ValueError,
+        "Fiddle detected a cycle while traversing a value: "
+        r"<root>\.bar is <root>\.bar\.bar\.bar\.",
+    ):
+      fdl.build(cfg)
+
+  def test_get_all_paths_dataclass_traverser(self):
+    config = {"dataclass": Foo(3, fdl.Config(sample_fn, "arg"))}
+    config["alt"] = config["dataclass"].baz
+
+    def traverse(value, state: daglish.State):
+      if state.is_traversable(value):
+        return {
+            "paths": ", ".join(
+                daglish.path_str(path)
+                for path in state.get_all_paths(allow_caching=True)
+            ),
+            "sub_values": state.flattened_map_children(value).values,
+        }
+      else:
+        return "leaf value"
+
+    traverser = daglish.MemoizedTraversal(
+        traverse, config, fdl_dc.daglish_dataclass_registry
+    )
+    result = traverse(config, traverser.initial_state())
+    self.assertDictEqual(
+        result,
+        {
+            "paths": "",
+            "sub_values": [
+                {
+                    "paths": "['dataclass']",
+                    "sub_values": [
+                        "leaf value",
+                        {
+                            "paths": "['dataclass'].baz, ['alt']",
+                            "sub_values": ["leaf value"],
+                        },
+                    ],
+                },
+                # This one comes from the config['alt']. It is returned as one
+                # of the values from flattened_map_chidlren() but is the same
+                # object as above.
+                {
+                    "paths": "['dataclass'].baz, ['alt']",
+                    "sub_values": ["leaf value"],
+                },
+            ],
+        },
+    )
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `fiddle-0.2.6/fiddle/_src/diffing.py` & `fiddle-0.2.7/fiddle/_src/diffing.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/diffing_test.py` & `fiddle-0.2.7/fiddle/_src/diffing_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,22 +620,18 @@
         z=GreenTag.new(BlueTag.new([20])))
     new = fdl.Config(
         SimpleClass,
         x=BlueTag.new([1]),
         y=GreenTag.new([6]),
         z=BlueTag.new(GreenTag.new({1: 2})))
     expected_changes = (
-        diffing.RemoveTag(parse_path('.x.value'), GreenTag),
-        diffing.AddTag(parse_path('.x.value'), BlueTag),
-        diffing.ModifyValue(parse_path('.y.value[0]'), 6),
-        diffing.RemoveTag(parse_path('.z.value'), GreenTag),
-        diffing.AddTag(parse_path('.z.value'), BlueTag),
-        diffing.RemoveTag(parse_path('.z.value.value'), BlueTag),
-        diffing.AddTag(parse_path('.z.value.value'), GreenTag),
-        diffing.ModifyValue(parse_path('.z.value.value'), {1: 2}),
+        diffing.RemoveTag(parse_path('.x'), GreenTag),
+        diffing.AddTag(parse_path('.x'), BlueTag),
+        diffing.ModifyValue(parse_path('.y[0]'), 6),
+        diffing.ModifyValue(parse_path('.z'), {1: 2}),
     )
     self.check_diff(old, new, expected_changes)
 
   def test_replace_value_with_tags(self):
     tagged_value = BlueTag.new(5)
     self.check_diff(
         old=[tagged_value.tags],
@@ -648,22 +644,26 @@
         expected_changes=(diffing.ModifyValue(
             parse_path('[0]'), tagged_value.tags),))
 
   def test_shared_new_tags(self):
     tagged_value = BlueTag.new([0])
     old = fdl.Config(SimpleClass)
     new = fdl.Config(SimpleClass, x=tagged_value, y=tagged_value)
-    expected_changes = (diffing.SetValue(
-        parse_path('.x'), parse_reference('new_shared_values', '[1]')),
-                        diffing.SetValue(
-                            parse_path('.y'),
-                            parse_reference('new_shared_values', '[1]')))
+    expected_changes = (
+        diffing.AddTag(parse_path('.x'), BlueTag),
+        diffing.AddTag(parse_path('.y'), BlueTag),
+        diffing.SetValue(
+            parse_path('.x'), parse_reference('new_shared_values', '[0]')
+        ),
+        diffing.SetValue(
+            parse_path('.y'), parse_reference('new_shared_values', '[0]')
+        ),
+    )
     expected_new_shared_values = (
         [0],
-        BlueTag.new(parse_reference('new_shared_values', '[0]')),
     )
     self.check_diff(old, new, expected_changes, expected_new_shared_values)
 
   def test_modify_root_tag(self):
     old = GreenTag.new([1])
     new = BlueTag.new([1])
     expected_changes = (
```

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/__init__.py` & `fiddle-0.2.7/fiddle/_src/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/auto_config.py` & `fiddle-0.2.7/fiddle/_src/experimental/auto_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 from fiddle._src import config
 from fiddle._src import mutate_buildable
 from fiddle._src.experimental import auto_config_policy
 from fiddle._src.experimental import daglish_legacy
 import libcst as cst
 
 _CALL_HANDLER_ID = '__auto_config_call_handler__'
+_ATTR_LOAD_HANDLER_ID = '__auto_config_attr_load_handler__'
+_ATTR_SAVE_HANDLER_ID = '__auto_config_attr_save_handler__'
+_ATTR_SAVE_TEMP_VAR_ID = '_attr_save_temp'
 _CLOSURE_WRAPPER_ID = '__auto_config_closure_wrapper__'
 _EMPTY_ARGUMENTS = ast.arguments(
     posonlyargs=[], args=[], kwonlyargs=[], kw_defaults=[], defaults=[])
 _BUILTINS = frozenset([
     builtin for builtin in builtins.__dict__.values()
     if inspect.isroutine(builtin) or inspect.isclass(builtin)
 ])
@@ -129,14 +132,15 @@
     """
     self._lines = source.splitlines()
     self._filename = filename
     self._line_number = line_number
     self._allow_control_flow = allow_control_flow
 
     self._function_def_depth = 0
+    self._temp_var_count = 0
 
   def _location_for(self, node: ast.AST):
     line_number = self._line_number + node.lineno - 1
     line = self._lines[node.lineno - 1]
     return (self._filename, line_number, node.col_offset, line)
 
   def _handle_control_flow(self, node: ast.AST, activatable: bool = False):
@@ -190,14 +194,97 @@
   def visit_Call(self, node: ast.Call):
     return ast.Call(
         func=ast.Name(id=_CALL_HANDLER_ID, ctx=ast.Load()),
         args=[node.func, *(self.visit(arg) for arg in node.args)],
         keywords=[self.visit(keyword) for keyword in node.keywords],
     )
 
+  def visit_Attribute(self, node: ast.Attribute):
+    if isinstance(node.ctx, ast.Load):
+      return ast.Call(
+          func=ast.Name(id=_ATTR_LOAD_HANDLER_ID, ctx=ast.Load()),
+          args=[self.visit(node.value), ast.Str(s=node.attr)],
+          keywords=[],
+      )
+    return self.generic_visit(node)
+
+  def visit_Assign(self, node: ast.Assign):
+    """Handler assignment transformation."""
+
+    def make_expr_call(obj, attr, value):
+      if isinstance(obj, ast.Attribute):
+        obj = self.visit_Attribute(obj)
+      return ast.Expr(
+          ast.Call(
+              func=ast.Name(id=_ATTR_SAVE_HANDLER_ID, ctx=ast.Load()),
+              args=[obj, ast.Str(s=attr), value],
+              keywords=[],
+          )
+      )
+
+    node.value = self.visit(node.value)
+    if len(node.targets) == 1 and isinstance(node.targets[0], ast.Attribute):
+      return make_expr_call(
+          node.targets[0].value, node.targets[0].attr, node.value
+      )
+
+    # Avoid creating temp var for single target ast.Assign expression,
+    # like `a.b = c.d.e`, to improve simplicity.
+    # For multiple targets ast.Assign expression, temporary variables will be
+    # created to facilitate set attribute validation.
+    # For example, `a.b = c.d = foo` will be transformed into:
+    # ```
+    # temp_var_0 = temp_var_1 = foo
+    # __auto_config_attr_save_handler__(a, b, temp_var_0)
+    # __auto_config_attr_save_handler__(c, d, temp_var_1)
+    # ```
+
+    def make_temp_var():
+      temp_var = ast.Name(
+          id=f'{_ATTR_SAVE_TEMP_VAR_ID}_{self._temp_var_count}',
+          ctx=ast.Store(),
+      )
+      return temp_var
+
+    transformed_nodes = []
+    for target in node.targets:
+      if isinstance(target, ast.Tuple) or isinstance(target, ast.List):
+        new_elts = []
+        for elt in target.elts:
+          if isinstance(elt, ast.Attribute):
+            temp_var = make_temp_var()
+            new_elts.append(temp_var)
+            expr_node = make_expr_call(elt.value, elt.attr, temp_var)
+            transformed_nodes.append(expr_node)
+            self._temp_var_count += 1
+          else:
+            new_elts.append(elt)
+        target.elts = new_elts
+      elif isinstance(target, ast.Attribute):
+        temp_var = make_temp_var()
+        expr_node = make_expr_call(target.value, target.attr, temp_var)
+        transformed_nodes.append(expr_node)
+        node.targets[node.targets.index(target)] = temp_var
+        self._temp_var_count += 1
+      elif isinstance(target, ast.Subscript):
+        target.value = self.visit(target.value)
+        target.slice = self.visit(target.slice)
+      elif isinstance(target, ast.Starred):
+        # TODO(b/288479702): Add validation when target is ast.Starred.
+        pass
+      elif isinstance(target, ast.Name):
+        pass
+      else:
+        raise NotImplementedError(
+            f'Cannot handle Assign statement with {target} as target.'
+        )
+
+    transformed_nodes.insert(0, node)
+    return transformed_nodes
+
   def visit_For(self, node: ast.For):
     return self._handle_control_flow(node, activatable=True)
 
   def visit_While(self, node: ast.While):
     return self._handle_control_flow(node, activatable=True)
 
   def visit_If(self, node: ast.If):
@@ -325,15 +412,16 @@
     A new `ast.Module` containing an additional wrapper `ast.FunctionDef` that
     defines dummy closure variables.
   """
   ast_name = lambda name: ast.Name(id=name, ctx=ast.Store())
   ast_none = ast.Constant(value=None)
   closure_var_definitions = [
       ast.Assign(targets=[ast_name(var_name)], value=ast_none)
-      for var_name in fn.__code__.co_freevars + (_CALL_HANDLER_ID,)
+      for var_name in fn.__code__.co_freevars
+      + (_CALL_HANDLER_ID, _ATTR_LOAD_HANDLER_ID, _ATTR_SAVE_HANDLER_ID)
   ]
 
   wrapper_module = ast.Module(
       body=[
           ast.FunctionDef(
               name=_CLOSURE_WRAPPER_ID,
               args=_EMPTY_ARGUMENTS,
@@ -457,56 +545,63 @@
   else:
     return config.Partial(buildable_or_callable, *args, **kwargs)
 
 
 def exempt(fn_or_cls: Callable[..., Any]) -> Callable[..., Any]:
   """Wrap a callable so that it's exempted from auto_config.
 
-  This can be used inside an auto_config function to inline exempt certain calls
-  so that they will be evaluated normally rather than turned into a config
-  object. For example::
+  This can be used either as a decorator to exempt a function, or used inside
+  an auto_config function to inline exempt certain calls to a function.
+  During auto_config transformation, exempted function calls will be evaluated
+  normally rather than turned into a config object. For example::
+
+      @exempt
+      def my_square(x): return x * x
 
       @auto_config
       def build_model():
-        return Model(a=np.square(3), b=exempt(np.square)(3))
+        return Model(a=np.square(3), b=exempt(np.square)(3), c=my_square(3))
 
       config = build_model.as_buildable()
       assert config.a == fdl.Config(np.square, 3)
-      assert config.b == 9
+      assert config.b == config.c == 9
 
   Args:
     fn_or_cls: Any callable.
 
   Returns:
     A wrapped version of the same callable that will not be transformed to
     config if called inside an auto_config function.
   """
   return AutoConfig(
       func=fn_or_cls, buildable_func=fn_or_cls, always_inline=True
   )
 
 
+# TODO(b/286559744): Change allow_dataclass_attribute_access default as False.
 def auto_config(
     fn=None,
     *,
+    experimental_allow_dataclass_attribute_access=True,
     experimental_allow_control_flow: bool = False,
     experimental_always_inline: Optional[bool] = None,
     experimental_exemption_policy: Optional[auto_config_policy.Policy] = None,
     experimental_config_cls=config.Config,
     experimental_result_must_contain_buildable: bool = True,
 ) -> Any:  # TODO(b/272377821): More precise return type.
   """Rewrites the given function to make it generate a ``Config``.
 
   This function creates a new function from ``fn`` by rewriting its AST
   (abstract syntax tree), replacing all ``Call`` nodes with a custom call
   handler. When the rewritten function is run, the call handler intercepts calls
   and applies the following rules:
 
-  - Calls to builtins, methods, callables without an inferrable signature, or
-    other functions that have been ``auto_config``'ed take place as usual.
+  - Calls to builtins, methods, callables without an inferrable signature,
+    callables wrapped by `auto_config.exempt`, or other functions that have
+    been ``auto_config``'ed take place as usual.
   - Calls to ``functools.partial`` are replaced by calling ``fdl.Partial`` with
     the same arguments;
   - All other calls are replaced by calling ``fdl.Config`` with the arguments
     that would have been passed to the called function or class.
 
   This function may be used standalone or as a decorator. The returned function
   is simply a wrapper around ``fn``, but with an additional ``as_buildable``
@@ -557,14 +652,18 @@
 
   Using ``@auto_config`` is compatible with both ``@staticmethod`` and
   ``@classmethod``, however the ``@auto_config`` decorator must appear above the
   ``@classmethod`` or ``@staticmethod`` in the decorator list.
 
   Args:
     fn: The function to create a config-generating function from.
+    experimental_allow_dataclass_attribute_access: Whether to allow attribute
+      access on dataclasses within auto_config. Note that access to dataclass
+      attribute is transformed into access to fdl.Config attributes in the
+      as_buildable path.
     experimental_allow_control_flow: Whether to allow control flow constructs in
       ``fn``. By default, control flow constructs will cause an
       ``UnsupportedLanguageConstructError`` to be thrown.
     experimental_always_inline: If true, this function (when called in an
       ``auto_config`` context) will always be ``inline``'d in-place. See the
       documentation on ``inline`` for an example. The default (if unspecified)
       is currently ``False``, but this may change in the future.
@@ -629,14 +728,40 @@
     if fn_or_cls is exempt:
       return fn_or_cls(*args, **kwargs)
     if experimental_exemption_policy(fn_or_cls):
       return fn_or_cls(*args, **kwargs)
 
     return experimental_config_cls(fn_or_cls, *args, **kwargs)
 
+  def auto_config_attr_load_handler(value, attr, allow_dataclass=True):
+    """Handles attribute access in auto_config'ed functions."""
+    if isinstance(value, config.Buildable):
+      fn_or_cls = value.__fn_or_cls__
+      if allow_dataclass and dataclasses.is_dataclass(fn_or_cls):
+        return getattr(value, attr)
+      raise ValueError(
+          f'Cannot load attribute {attr!r} on object of type {type(value)}'
+          ' within auto_config, as this could lead to inconsistent behavior'
+          ' between the Python and as_buildable code paths.'
+      )
+    return getattr(value, attr)
+
+  def auto_config_attr_save_handler(obj, attr, value, allow_dataclass=True):
+    """Handles saving attributes in auto_config'ed functions."""
+    if isinstance(obj, config.Buildable):
+      fn_or_cls = obj.__fn_or_cls__
+      if allow_dataclass and dataclasses.is_dataclass(fn_or_cls):
+        setattr(obj, attr, value)
+        return
+      raise ValueError(
+          f'Cannot save attribute {attr!r} on object of type {type(obj)}'
+          ' within auto_config, as this could lead to inconsistent behavior'
+          ' between the Python and as_buildable code paths.'
+      )
+
   def make_auto_config(fn):
     if not isinstance(fn, (types.FunctionType, classmethod, staticmethod)):
       raise ValueError('`auto_config` is only compatible with functions, '
                        f'`@classmethod`s, and `@staticmethod`s.  Got {fn!r} '
                        f'with type {type(fn)!r}.')
 
     if isinstance(fn, (classmethod, staticmethod)):
@@ -674,22 +799,43 @@
     # free variables in `fn`.
     node = _wrap_ast_for_fn_with_closure_vars(node, fn)
     # Compile the modified AST, and then find the function code object within
     # the returned module-level code object.
     code = compile(node, inspect.getsourcefile(fn), 'exec')
     code = _unwrap_code_for_fn(code, fn)
 
-    # Insert auto_config_call_handler into `fn.__closure__` at the index where
-    # _CALL_HANDLER_ID occurs in the freevars.  (_CALL_HANDLER_ID was added to
-    # freevars by _wrap_ast_for_fn_with_closure_vars).
+    # Insert auto_config_attr_load_handler, auto_config_attr_save_handler,
+    # auto_config_call_handler into `fn.__closure__` at the index where
+    # _ATTR_LOAD_HANDLER_ID, _ATTR_SAVE_HANDLER_ID, _CALL_HANDLER_ID
+    # occur in the freevars. Both of them were added to freevars by
+    # _wrap_ast_for_fn_with_closure_vars.
     closure = list(fn.__closure__ or ())
+    indexed_handlers = []
+    for handler_id, handler in (
+        (_ATTR_LOAD_HANDLER_ID, auto_config_attr_load_handler),
+        (_ATTR_SAVE_HANDLER_ID, auto_config_attr_save_handler),
+    ):
+      if handler_id in code.co_freevars:
+        handler_idx = code.co_freevars.index(handler_id)
+        handler = _make_closure_cell(
+            functools.partial(
+                handler,
+                allow_dataclass=experimental_allow_dataclass_attribute_access,
+            )
+        )
+        indexed_handlers.append((handler_idx, handler))
     if _CALL_HANDLER_ID in code.co_freevars:
-      closure.insert(
-          code.co_freevars.index(_CALL_HANDLER_ID),
-          _make_closure_cell(auto_config_call_handler))
+      handler_idx = code.co_freevars.index(_CALL_HANDLER_ID)
+      handler = _make_closure_cell(auto_config_call_handler)
+      indexed_handlers.append((handler_idx, handler))
+
+    # Insert handler from small index to ensure the content of closures will
+    # not be mismatched.
+    for handler_idx, handler in sorted(indexed_handlers):
+      closure.insert(handler_idx, handler)
     closure = tuple(closure)
 
     # Then, create a function from the compiled function code object, providing
     # the globals and the original function's closure.
     auto_config_fn = types.FunctionType(code, fn.__globals__, closure=closure)
     auto_config_fn.__defaults__ = fn.__defaults__
     auto_config_fn.__kwdefaults__ = fn.__kwdefaults__
@@ -936,7 +1082,20 @@
     # TODO(b/258671226): If desired, we could narrow down which lambda is
     # used based on the signature (or even fancier things like the checking
     # fn.__code__.co_names).
     raise ValueError(
         'Fiddle auto_config was unable to find the source code for '
         f'{fn}: multiple lambdas found on line {lambda_finder.lineno}; '
         'try moving each lambda to its own line.')
+
+
+def with_buildable_func(
+    buildable_func: Callable[..., Any]
+) -> Callable[..., Any]:
+  """A decorator that adds an auto_config-only code path."""
+
+  def decorator(func):
+    return AutoConfig(
+        func=func, buildable_func=buildable_func, always_inline=True
+    )
+
+  return decorator
```

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/auto_config_policy.py` & `fiddle-0.2.7/fiddle/_src/experimental/auto_config_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# pyformat: mode=midnight
 """A policy of functions to skip representing as `fdl.Config`'s.
 
 When running `auto_config` on a function, some Python functions cannot or, in
 practice, should never be mapped into `fdl.Config`-space. This file defines
 policies (mostly implemented as lists) that enumerates them.
 
 Because either adding or removing a function from this list can cause config
```

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/auto_config_test.py` & `fiddle-0.2.7/fiddle/_src/experimental/auto_config_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for auto_config."""
 
+import ast
 import copy
 import dataclasses
 import functools
 import inspect
 import sys
 from typing import Any
 
 from absl.testing import absltest
 from absl.testing import parameterized
-
 import fiddle as fdl
 from fiddle import arg_factory
 from fiddle._src.experimental import auto_config
 from fiddle._src.experimental import auto_config_policy
 from fiddle._src.experimental import autobuilders as ab
 from fiddle._src.testing import test_util
 
@@ -37,16 +37,29 @@
   return {'arg': arg, 'kwarg': kwarg}
 
 
 def fn_with_kwargs(**kwargs):
   return {'kwargs': kwargs}
 
 
+class NonDataclassSampleClass:
+
+  def __init__(self, arg1, arg2):
+    self.arg1 = arg1
+    self.arg2 = arg2
+
+
+@dataclasses.dataclass(frozen=False)
+class MutableSampleClass:
+  arg1: Any
+  arg2: Any
+
+
 @dataclasses.dataclass(frozen=True)
-class SampleClass:
+class FrozenSampleClass:
   arg1: Any
   arg2: Any
 
   def method(self):
     return 42
 
   @auto_config.auto_config
@@ -78,35 +91,119 @@
   return arg
 
 
 def _line_number():
   return sys._getframe(1).f_lineno
 
 
+class AutoConfigTransformerTest(parameterized.TestCase, test_util.TestCase):
+
+  @parameterized.parameters(
+      (
+          'a.b = x, y',
+          "__auto_config_attr_save_handler__(a, 'b', (x, y))",
+      ),
+      (
+          'x.y.z = v',
+          (
+              '__auto_config_attr_save_handler__('
+              "__auto_config_attr_load_handler__(x, 'y'), 'z', v)"
+          ),
+      ),
+      (
+          'a.b.c = c.d',
+          (
+              '__auto_config_attr_save_handler__('
+              "__auto_config_attr_load_handler__(a, 'b'), 'c', "
+              "__auto_config_attr_load_handler__(c, 'd'))"
+          ),
+      ),
+      (
+          'a, b.c = v',
+          (
+              '(a, _attr_save_temp_0) = v\n'
+              "__auto_config_attr_save_handler__(b, 'c', _attr_save_temp_0)"
+          ),
+      ),
+      (
+          'a = b = c',
+          'a = b = c',
+      ),
+      (
+          'a, b.c = x.y.z = foo.bar',
+          (
+              '(a, _attr_save_temp_0) = _attr_save_temp_1 = '
+              "__auto_config_attr_load_handler__(foo, 'bar')\n"
+              "__auto_config_attr_save_handler__(b, 'c', _attr_save_temp_0)\n"
+              '__auto_config_attr_save_handler__('
+              "__auto_config_attr_load_handler__(x, 'y'), "
+              "'z', _attr_save_temp_1)"
+          ),
+      ),
+      # Test transformations when Assign.value is a function call.
+      # This test will ensure calls to ``functools.partial`` are replaced by
+      # ``fdl.Partial`` properly.
+      (
+          'a.b.c = functools.partial(foo, x.y)',
+          (
+              '__auto_config_attr_save_handler__('
+              "__auto_config_attr_load_handler__(a, 'b'), 'c', "
+              '__auto_config_call_handler__(functools.partial, foo, '
+              "__auto_config_attr_load_handler__(x, 'y')))"
+          ),
+      ),
+      (
+          'a.b.c = bar = functools.partial(foo, x.y)',
+          (
+              '_attr_save_temp_0 = bar = __auto_config_call_handler__('
+              'functools.partial, foo, __auto_config_attr_load_handler__('
+              "x, 'y'))\n"
+              '__auto_config_attr_save_handler__('
+              "__auto_config_attr_load_handler__(a, 'b'), 'c', "
+              '_attr_save_temp_0)'
+          ),
+      ),
+      ('a.b[1] = 123', "__auto_config_attr_load_handler__(a, 'b')[1] = 123"),
+      (
+          # TODO(b/288479702): Add validation for ast.Starred pattern.
+          'a, *a.b = foo.bar',
+          "(a, *a.b) = __auto_config_attr_load_handler__(foo, 'bar')",
+      ),
+  )
+  def test_attribute_save(self, source, expected):
+    version = sys.version_info
+    # ast.unparse is available only after Python 3.9
+    if version.major >= 3 and version.minor >= 9:
+      transfomer = auto_config._AutoConfigNodeTransformer(source, 'dummy.py', 0)
+      node = ast.parse(source)
+      node = transfomer.visit(node)
+      self.assertEqual(ast.unparse(node), expected)
+
+
 class AutoConfigTest(parameterized.TestCase, test_util.TestCase):
 
   def test_create_basic_config(self):
-    expected_config = fdl.Config(SampleClass, 1, arg2=2)
+    expected_config = fdl.Config(FrozenSampleClass, 1, arg2=2)
 
     @auto_config.auto_config
     def test_class_config():
-      return SampleClass(1, 2)
+      return FrozenSampleClass(1, 2)
 
     self.assertEqual(expected_config, test_class_config.as_buildable())
-    self.assertEqual(SampleClass(1, 2), test_class_config())
+    self.assertEqual(FrozenSampleClass(1, 2), test_class_config())
 
   def test_create_basic_config_parents(self):
-    expected_config = fdl.Config(SampleClass, 1, arg2=2)
+    expected_config = fdl.Config(FrozenSampleClass, 1, arg2=2)
 
     @auto_config.auto_config()  # Note the parenthesis!
     def test_class_config():
-      return SampleClass(1, 2)
+      return FrozenSampleClass(1, 2)
 
     self.assertEqual(expected_config, test_class_config.as_buildable())
-    self.assertEqual(SampleClass(1, 2), test_class_config())
+    self.assertEqual(FrozenSampleClass(1, 2), test_class_config())
 
   def test_create_basic_partial(self):
     expected_config = fdl.Partial(basic_fn, 1, kwarg='kwarg')
 
     @auto_config.auto_config
     def test_fn_config():
       return functools.partial(basic_fn, 1, 'kwarg')
@@ -125,15 +222,15 @@
     self.assertEqual(
         fdl.build(test_fn_config.as_buildable())(), {'kwargs': {'a': 1, 'b': 2}}
     )
 
   def test_nested_functools_partial_unsupported_positional_args(self):
     @auto_config.auto_config
     def test_fn_config():
-      return functools.partial(functools.partial(SampleClass, 1), 2)
+      return functools.partial(functools.partial(FrozenSampleClass, 1), 2)
 
     with self.assertRaisesRegex(
         ValueError, 'chained.*partial.*calls.*only.*keyword'
     ):
       test_fn_config.as_buildable()
 
   def test_create_basic_arg_factory(self):
@@ -194,77 +291,85 @@
           a=basic_fn(1),
       )
 
     self.assertEqual(expected_config, test_fn_config_1.as_buildable())
     self.assertEqual(expected_config, test_fn_config_2.as_buildable())
 
   def test_create_config_with_args(self):
-    expected_config = fdl.Config(SampleClass, 'positional', arg2='default')
+    expected_config = fdl.Config(
+        FrozenSampleClass, 'positional', arg2='default'
+    )
 
     @auto_config.auto_config
     def test_class_config(arg1, arg2='default'):
-      return SampleClass(arg1, arg2)
+      return FrozenSampleClass(arg1, arg2)
 
     self.assertEqual(expected_config,
                      test_class_config.as_buildable('positional'))
     self.assertEqual(
-        SampleClass('positional', 'default'), test_class_config('positional'))
+        FrozenSampleClass('positional', 'default'),
+        test_class_config('positional'),
+    )
 
   def test_create_config_with_kwonly_args(self):
-    expected_config = fdl.Config(SampleClass, 'positional', arg2='default')
+    expected_config = fdl.Config(
+        FrozenSampleClass, 'positional', arg2='default'
+    )
 
     @auto_config.auto_config
     def test_class_config(arg1, *, arg2='default'):
-      return SampleClass(arg1, arg2)
+      return FrozenSampleClass(arg1, arg2)
 
     self.assertEqual(expected_config,
                      test_class_config.as_buildable('positional'))
     self.assertEqual(
-        SampleClass('positional', 'default'), test_class_config('positional'))
+        FrozenSampleClass('positional', 'default'),
+        test_class_config('positional'),
+    )
 
   def test_calling_auto_config(self):
     expected_config = fdl.Config(
-        basic_fn, 1, kwarg=fdl.Config(SampleClass, 1, 2))
+        basic_fn, 1, kwarg=fdl.Config(FrozenSampleClass, 1, 2)
+    )
 
     @auto_config.auto_config(experimental_always_inline=True)
     def test_class_config():
-      return SampleClass(1, arg2=2)
+      return FrozenSampleClass(1, arg2=2)
 
     @auto_config.auto_config
     def test_fn_config():
       return basic_fn(1, test_class_config())
 
     self.assertEqual(expected_config, test_fn_config.as_buildable())
-    self.assertEqual({
-        'arg': 1,
-        'kwarg': SampleClass(1, arg2=2)
-    }, test_fn_config())
+    self.assertEqual(
+        {'arg': 1, 'kwarg': FrozenSampleClass(1, arg2=2)}, test_fn_config()
+    )
 
   def test_nested_calls(self):
     expected_config = fdl.Config(
-        SampleClass, 1, arg2=fdl.Config(basic_fn, 2, 'kwarg'))
+        FrozenSampleClass, 1, arg2=fdl.Config(basic_fn, 2, 'kwarg')
+    )
 
     @auto_config.auto_config
     def test_class_config():
-      return SampleClass(1, basic_fn(2, 'kwarg'))
+      return FrozenSampleClass(1, basic_fn(2, 'kwarg'))
 
     self.assertEqual(expected_config, test_class_config.as_buildable())
     self.assertEqual(
-        SampleClass(1, {
-            'arg': 2,
-            'kwarg': 'kwarg'
-        }), test_class_config())
+        FrozenSampleClass(1, {'arg': 2, 'kwarg': 'kwarg'}), test_class_config()
+    )
 
   def test_calling_explicit_function(self):
     expected_config = fdl.Config(
-        SampleClass, 1, arg2=fdl.Config(basic_fn, 5, 10))
+        FrozenSampleClass, 1, arg2=fdl.Config(basic_fn, 5, 10)
+    )
 
     @auto_config.auto_config
     def test_nested_call():
-      return SampleClass(1, explicit_config_building_fn(10))
+      return FrozenSampleClass(1, explicit_config_building_fn(10))
 
     self.assertEqual(expected_config, test_nested_call.as_buildable())
 
   def test_reference_nonlocal(self):
     nonlocal_var = 3
     expected_config = fdl.Config(basic_fn, 1, kwarg=nonlocal_var)
 
@@ -291,67 +396,68 @@
     cfg = inner_fn.as_buildable()
     expected_result = (0, 1, 2)
     self.assertEqual(cfg.arg, expected_result)
     self.assertEqual(expected_result, inner_fn())
     self.assertEqual(expected_result, fdl.build(cfg))
 
   def test_calling_builtins(self):
-    expected_config = fdl.Config(SampleClass, [0, 1, 2], ['a', 'b'])
+    expected_config = fdl.Config(FrozenSampleClass, [0, 1, 2], ['a', 'b'])
 
     @auto_config.auto_config
     def test_config():
-      return SampleClass(list(range(3)), list({'a': 0, 'b': 1}.keys()))
+      return FrozenSampleClass(list(range(3)), list({'a': 0, 'b': 1}.keys()))
 
     self.assertEqual(expected_config, test_config.as_buildable())
 
   def test_auto_config_eligibility(self):
     # Some common types that have no signature.
     for builtin_type in (range, dict):
       self.assertTrue(auto_config_policy.v1(builtin_type))
     # Some common builtins.
     for builtin in (list, tuple, sum, any, all, iter):
       self.assertTrue(auto_config_policy.v1(builtin))
     self.assertTrue(auto_config_policy.v1([].append))
     self.assertTrue(auto_config_policy.v1({}.keys))
     # A method.
-    test_class = SampleClass(1, 2)
+    test_class = FrozenSampleClass(1, 2)
     self.assertFalse(auto_config_policy.v1(test_class.method))
     # Buildable subclasses.
     self.assertTrue(auto_config_policy.v1(fdl.Config))
     self.assertTrue(auto_config_policy.v1(fdl.Partial))
     # Auto-config annotations are not eligible, and this case is tested in
     # `test_calling_auto_config` above.
 
   def test_autobuilders_in_auto_config(self):
     expected_config = fdl.Config(
-        basic_fn, arg=ab.config(SampleClass, require_skeleton=False))
+        basic_fn, arg=ab.config(FrozenSampleClass, require_skeleton=False)
+    )
 
     @auto_config.auto_config
     def autobuilder_using_fn():
-      x = ab.config(SampleClass, require_skeleton=False)
+      x = ab.config(FrozenSampleClass, require_skeleton=False)
       return basic_fn(x)
 
     self.assertEqual(expected_config, autobuilder_using_fn.as_buildable())
 
   def test_auto_configuring_non_function(self):
     with self.assertRaisesRegex(ValueError, 'only compatible with functions'):
       auto_config.auto_config(3)
 
   def test_return_structure(self):
     expected_config = {
-        'test_key1': fdl.Config(SampleClass, 1, arg2=2),
-        'test_key2': [fdl.Config(SampleClass, 3, 4), 5],
+        'test_key1': fdl.Config(FrozenSampleClass, 1, arg2=2),
+        'test_key2': [fdl.Config(FrozenSampleClass, 3, 4), 5],
         'test_key3': (fdl.Partial(pass_through, 'arg'), 6),
     }
 
     @auto_config.auto_config
     def test_config():
       return {
-          'test_key1': SampleClass(1, 2),
-          'test_key2': [SampleClass(3, 4), 5],
+          'test_key1': FrozenSampleClass(1, 2),
+          'test_key2': [FrozenSampleClass(3, 4), 5],
           'test_key3': (functools.partial(pass_through, 'arg'), 6),
       }
 
     buildable = test_config.as_buildable()
     self.assertEqual(expected_config, buildable)
 
   def test_require_buildable_in_return_type(self):
@@ -369,58 +475,64 @@
   def test_experimental_config_cls(self):
 
     class CustomConfig(fdl.Config):
       pass
 
     @auto_config.auto_config(experimental_config_cls=CustomConfig)
     def fn():
-      return SampleClass(arg1=basic_fn(3), arg2=4)
+      return FrozenSampleClass(arg1=basic_fn(3), arg2=4)
 
-    expected = CustomConfig(SampleClass, arg1=CustomConfig(basic_fn, 3), arg2=4)
+    expected = CustomConfig(
+        FrozenSampleClass, arg1=CustomConfig(basic_fn, 3), arg2=4
+    )
     cfg = fn.as_buildable()
     self.assertDagEqual(cfg, expected)
     self.assertIsInstance(cfg, CustomConfig)
     self.assertIsInstance(cfg.arg1, CustomConfig)
 
   def test_staticmethod_nullary(self):
 
     class MyClass:
 
       @auto_config.auto_config
       @staticmethod
       def my_fn():
-        return SampleClass(2, 1)
+        return FrozenSampleClass(2, 1)
 
     self.assertEqual(
-        fdl.Config(SampleClass, 2, 1), MyClass.my_fn.as_buildable())
-    self.assertEqual(SampleClass(2, 1), MyClass.my_fn())
+        fdl.Config(FrozenSampleClass, 2, 1), MyClass.my_fn.as_buildable()
+    )
+    self.assertEqual(FrozenSampleClass(2, 1), MyClass.my_fn())
 
     instance = MyClass()
     self.assertEqual(
-        fdl.Config(SampleClass, 2, 1), instance.my_fn.as_buildable())
-    self.assertEqual(SampleClass(2, 1), instance.my_fn())
+        fdl.Config(FrozenSampleClass, 2, 1), instance.my_fn.as_buildable()
+    )
+    self.assertEqual(FrozenSampleClass(2, 1), instance.my_fn())
 
   def test_staticmethod_arguments(self):
 
     class MyClass:
 
       @auto_config.auto_config
       @staticmethod
       def my_fn(x):
-        return SampleClass(x, x + 1)
+        return FrozenSampleClass(x, x + 1)
 
     self.assertEqual(
-        fdl.Config(SampleClass, 5, 6), MyClass.my_fn.as_buildable(5))
-    self.assertEqual(SampleClass(5, 6), MyClass.my_fn(5))
+        fdl.Config(FrozenSampleClass, 5, 6), MyClass.my_fn.as_buildable(5)
+    )
+    self.assertEqual(FrozenSampleClass(5, 6), MyClass.my_fn(5))
 
     instance = MyClass()
 
     self.assertEqual(
-        fdl.Config(SampleClass, 5, 6), instance.my_fn.as_buildable(5))
-    self.assertEqual(SampleClass(5, 6), instance.my_fn(5))
+        fdl.Config(FrozenSampleClass, 5, 6), instance.my_fn.as_buildable(5)
+    )
+    self.assertEqual(FrozenSampleClass(5, 6), instance.my_fn(5))
 
   def test_staticmethod_on_top(self):
 
     expected_msg = (
         r'@staticmethod placed above @auto_config on function my_fn at '
         r'.+:\d+\. Reorder decorators so that @auto_config is placed above '
         r'@staticmethod.')
@@ -523,15 +635,15 @@
         def my_fn(cls, x, y):
           pass
 
   def test_copy(self):
 
     @auto_config.auto_config
     def test_fn():
-      return SampleClass(1, 2)
+      return FrozenSampleClass(1, 2)
 
     with self.subTest('shallow_copy'):
       shallow_copy = copy.copy(test_fn)
       self.assertIsNot(shallow_copy, test_fn)
       self.assertEqual(shallow_copy.as_buildable(), test_fn.as_buildable())
 
     with self.subTest('deep_copy'):
@@ -565,15 +677,15 @@
       # We don't actually have any additional subfields that should be
       # deepcopied to test, but this at least makes sure things run.
       self.assertEqual(deep_copy.as_buildable(),
                        SomeClass.test_method.as_buildable())
 
   def test_call_super(self):
 
-    class MyClass(SampleClass):  # pylint: disable=unused-variable
+    class MyClass(FrozenSampleClass):  # pylint: disable=unused-variable
 
       def __init__(self):
         super().__init__(1, 2)
 
       @auto_config.auto_config
       def my_fn(self, x):
         return basic_fn(x, kwarg=super().method())
@@ -591,37 +703,38 @@
 
     def custom_policy(fn):
       if fn is make_list:
         return True
       return auto_config_policy.v1(fn)
 
     def make_sample(max_value):
-      return SampleClass(arg1=make_list(max_value), arg2=None)
+      return FrozenSampleClass(arg1=make_list(max_value), arg2=None)
 
     with_policy = auto_config.auto_config(
         experimental_exemption_policy=custom_policy)(
             make_sample)
     without_policy = auto_config.auto_config(make_sample)
 
-    expected_without_policy = fdl.Config(SampleClass, fdl.Config(make_list, 5),
-                                         None)
-    expected_with_policy = fdl.Config(SampleClass, list(range(5)), None)
+    expected_without_policy = fdl.Config(
+        FrozenSampleClass, fdl.Config(make_list, 5), None
+    )
+    expected_with_policy = fdl.Config(FrozenSampleClass, list(range(5)), None)
 
     self.assertEqual(with_policy.as_buildable(5), expected_with_policy)
     self.assertEqual(without_policy.as_buildable(5), expected_without_policy)
 
   def test_inline_exemption(self):
     @auto_config.auto_config
     def make_sample(max_value):
       # Test the case where we first create the function, then call.
       # It produces different AST.
       exempted_func = auto_config.exempt(pass_through)
-      return SampleClass(
+      return FrozenSampleClass(
           arg1=auto_config.exempt(pass_through)(max_value),
-          arg2=SampleClass(
+          arg2=FrozenSampleClass(
               arg1=pass_through(max_value), arg2=exempted_func(max_value)
           ),
       )
 
     cfg = make_sample.as_buildable(5)
     self.assertEqual(cfg.arg1, 5)
     self.assertEqual(cfg.arg2.arg1, fdl.Config(pass_through, 5))
@@ -634,29 +747,30 @@
 
     expected = fdl.Config(dict, arg1=3)
     self.assertEqual(make_sample.as_buildable(), expected)
 
   def test_function_metadata(self):
 
     @auto_config.auto_config
-    def my_helpful_function(x: int, y: str = 'y') -> SampleClass:
+    def my_helpful_function(x: int, y: str = 'y') -> FrozenSampleClass:
       """A docstring."""
-      return SampleClass(x, y)
+      return FrozenSampleClass(x, y)
 
     self.assertEqual('A docstring.', inspect.getdoc(my_helpful_function))
     param_kind = inspect.Parameter.POSITIONAL_OR_KEYWORD
     expected_parameters = (inspect.Parameter(
         'x', kind=param_kind, annotation=int),
                            inspect.Parameter(
                                'y',
                                kind=param_kind,
                                default='y',
                                annotation=str))
     expected_signature = inspect.Signature(
-        expected_parameters, return_annotation=SampleClass)
+        expected_parameters, return_annotation=FrozenSampleClass
+    )
     self.assertEqual(expected_signature, inspect.signature(my_helpful_function))
     self.assertEqual('my_helpful_function', my_helpful_function.__name__)
 
   def test_unhashable_callable(self):
     class UnhashableCallable:
       a: int = 1
 
@@ -708,24 +822,25 @@
     self.assertEqual('false branch', fdl.build(build_config_fn(False)))
 
   def test_control_flow_for(self):
 
     def test_config():
       layers = []
       for i in range(3):
-        layers.append(SampleClass(i, i))
+        layers.append(FrozenSampleClass(i, i))
       return pass_through(layers)
 
     with self.assertRaisesRegex(
         auto_config.UnsupportedLanguageConstructError,
         r'Control flow \(For\) is unsupported by auto_config\.'):
       auto_config.auto_config(test_config)
 
     expected_config = fdl.Config(
-        pass_through, [fdl.Config(SampleClass, i, i) for i in range(3)])
+        pass_through, [fdl.Config(FrozenSampleClass, i, i) for i in range(3)]
+    )
     actual_config = auto_config.auto_config(
         test_config, experimental_allow_control_flow=True).as_buildable()
     self.assertEqual(expected_config, actual_config)
 
   def test_control_flow_while(self):
 
     def test_config():
@@ -851,15 +966,15 @@
         auto_config.UnsupportedLanguageConstructError,
         r'Class definitions are not supported by auto_config\.'):
       auto_config.auto_config(test_config)
 
   def test_disallow_lambda_definitions(self):
 
     def test_config():
-      return pass_through(lambda: SampleClass(1, 2))
+      return pass_through(lambda: FrozenSampleClass(1, 2))
 
     with self.assertRaisesRegex(
         auto_config.UnsupportedLanguageConstructError,
         r'Lambda definitions are not supported by auto_config\.'):
       auto_config.auto_config(test_config)
 
   def test_disallow_async_function_definitions(self):
@@ -871,30 +986,32 @@
         auto_config.UnsupportedLanguageConstructError,
         r'Async function definitions are not supported by auto_config\.'):
       auto_config.auto_config(test_config)
 
   def test_access_autoconfig_method_via_class(self):
     # If we access an autoconfig via an instance, we get a bound method:
     self.assertIsInstance(
-        SampleClass(1, 2).autoconfig_method, auto_config.AutoConfig)
+        FrozenSampleClass(1, 2).autoconfig_method, auto_config.AutoConfig
+    )
 
     # But if we access it via the class, we get the (unbound) AutoConfig:
-    self.assertIsInstance(SampleClass.autoconfig_method, auto_config.AutoConfig)
+    self.assertIsInstance(
+        FrozenSampleClass.autoconfig_method, auto_config.AutoConfig
+    )
 
   @absltest.skip('Enable this after dropping pyhon 3.7 support')
   def test_can_pass_self_as_keyword(self):
-    x = SampleClass(1, 2)
+    x = FrozenSampleClass(1, 2)
     self.assertEqual(
-        SampleClass.autoconfig_method(self=x), {
-            'arg': x,
-            'kwarg': 'test'
-        })
+        FrozenSampleClass.autoconfig_method(self=x), {'arg': x, 'kwarg': 'test'}
+    )
     self.assertDagEqual(
-        SampleClass.autoconfig_method.as_buildable(self=x),
-        fdl.Config(basic_fn, x))
+        FrozenSampleClass.autoconfig_method.as_buildable(self=x),
+        fdl.Config(basic_fn, x),
+    )
 
   def test_globals(self):
     # The following will fail with `NameError: name 'pass_through' is not
     # defined` if the as_buildable globals don't reflect changes made after
     # the auto_config decorator is run.
     globals_test_fn.as_buildable()
 
@@ -927,49 +1044,150 @@
 
     cfg = make_dict.as_buildable(['foo'])
     self.assertEqual(fdl.build(cfg), {'foo': basic_fn('foo')})
 
     cfg = make_dict.as_buildable([])
     self.assertEqual(fdl.build(cfg), {})
 
+  def test_non_dataclass_attribute_load(self):
+    @auto_config.auto_config
+    def fixture():
+      foo = NonDataclassSampleClass(1, 2)
+      _ = foo.arg1
+      return foo
+
+    with self.assertRaisesRegex(ValueError, 'Cannot load attribute'):
+      fixture.as_buildable()
+
+  def test_dataclass_attribute_load(self):
+    def fixture():
+      foo = MutableSampleClass(1, 2)
+      _ = foo.arg1
+      return foo
+
+    fixture_disable = auto_config.auto_config(
+        fixture, experimental_allow_dataclass_attribute_access=False
+    )
+    fixture_enable = auto_config.auto_config(
+        fixture, experimental_allow_dataclass_attribute_access=True
+    )
+
+    with self.subTest('disable'):
+      with self.assertRaisesRegex(ValueError, 'Cannot load attribute'):
+        fixture_disable.as_buildable()
+
+    with self.subTest('enable'):
+      fixture_enable.as_buildable()
+
+  def test_nested_attribute_load(self):
+    @auto_config.auto_config
+    def fixture():
+      foo = NonDataclassSampleClass(1, 'ABC')
+      # To test if inner attribute calls are validated. foo.arg2 is not a
+      # Buildable but foo is. So if the attribute validation only inpsects
+      # the outermost attribute access, the error will not be raised.
+      lower = foo.arg2.lower
+      return NonDataclassSampleClass(2, lower)
+
+    with self.subTest('disable'):
+      with self.assertRaisesRegex(ValueError, 'Cannot load attribute'):
+        fixture.as_buildable()
+
+  def test_non_dataclass_attribute_save(self):
+    @auto_config.auto_config
+    def fixture():
+      foo = NonDataclassSampleClass(1, 2)
+      foo.arg1 = 2
+      return foo
+
+    with self.assertRaisesRegex(ValueError, 'Cannot save attribute'):
+      fixture.as_buildable()
+
+  def test_dataclass_attribute_save(self):
+    def fixture():
+      foo = MutableSampleClass(1, 2)
+      foo.arg1 = 3
+      return foo
+
+    fixture_disable = auto_config.auto_config(
+        fixture, experimental_allow_dataclass_attribute_access=False
+    )
+    fixture_enable = auto_config.auto_config(
+        fixture, experimental_allow_dataclass_attribute_access=True
+    )
+
+    with self.subTest('disable'):
+      with self.assertRaisesRegex(ValueError, 'Cannot save attribute'):
+        fixture_disable.as_buildable()
+
+    with self.subTest('enable'):
+      config = fixture_enable.as_buildable()
+      self.assertEqual(config.arg1, 3)
+      self.assertEqual(config.arg2, 2)
+
+  def test_nested_attribute_save(self):
+    @auto_config.auto_config(experimental_allow_dataclass_attribute_access=True)
+    def fixture():
+      foo = NonDataclassSampleClass(0, 'foo')
+      bar = MutableSampleClass(foo, 'bar')
+      bar.arg1.arg2 = 'baz'
+      return NonDataclassSampleClass(0, bar)
+
+    with self.assertRaisesRegex(ValueError, 'Cannot save attribute'):
+      fixture.as_buildable()
+
+  def test_nested_dataclass_attribute_save(self):
+    @auto_config.auto_config(experimental_allow_dataclass_attribute_access=True)
+    def fixture():
+      foo = MutableSampleClass(0, 'foo')
+      bar = MutableSampleClass(foo, 'bar')
+      bar.arg1.arg2 = 'baz'
+      return MutableSampleClass(0, bar)
+
+    config = fixture.as_buildable()
+    self.assertEqual(config.arg2.arg1.arg2, 'baz')
+
 
 class AutoUnconfigTest(absltest.TestCase):
 
   def test_simple_inline(self):
 
     @auto_config.auto_unconfig(experimental_always_inline=True)
-    def simple(x: int) -> fdl.Config[SampleClass]:
-      cfg = fdl.Config(SampleClass)
+    def simple(x: int) -> fdl.Config[FrozenSampleClass]:
+      cfg = fdl.Config(FrozenSampleClass)
       cfg.arg1 = x
       cfg.arg2 = str(x)
       return cfg
 
     @auto_config.auto_config
     def parent():
-      return SampleClass(arg1=simple(42), arg2=5)
+      return FrozenSampleClass(arg1=simple(42), arg2=5)
 
     expected = fdl.Config(
-        SampleClass, arg1=fdl.Config(SampleClass, 42, '42'), arg2=5)
+        FrozenSampleClass, arg1=fdl.Config(FrozenSampleClass, 42, '42'), arg2=5
+    )
 
     self.assertEqual(expected, parent.as_buildable())
 
   def test_simple_not_inline(self):
 
     @auto_config.auto_unconfig(experimental_always_inline=False)
-    def simple(x: int) -> fdl.Config[SampleClass]:
-      cfg = fdl.Config(SampleClass)
+    def simple(x: int) -> fdl.Config[FrozenSampleClass]:
+      cfg = fdl.Config(FrozenSampleClass)
       cfg.arg1 = x
       cfg.arg2 = str(x)
       return cfg
 
     @auto_config.auto_config
     def parent():
-      return SampleClass(arg1=simple(42), arg2=5)
+      return FrozenSampleClass(arg1=simple(42), arg2=5)
 
-    expected = fdl.Config(SampleClass, arg1=fdl.Config(simple, 42), arg2=5)
+    expected = fdl.Config(
+        FrozenSampleClass, arg1=fdl.Config(simple, 42), arg2=5
+    )
 
     self.assertEqual(expected, parent.as_buildable())
 
   def test_arg_factory_counter(self):
     counter = {'count': 0}
 
     def count():
@@ -988,64 +1206,64 @@
     self.assertEqual(built_from_config(), {'arg': 4, 'kwarg': 'test'})
     self.assertEqual(built_from_config(), {'arg': 5, 'kwarg': 'test'})
     self.assertEqual(built_from_config(), {'arg': 6, 'kwarg': 'test'})
 
   def test_python_execution(self):
 
     @auto_config.auto_unconfig
-    def simple(x: int) -> fdl.Config[SampleClass]:
-      cfg = fdl.Config(SampleClass)
+    def simple(x: int) -> fdl.Config[FrozenSampleClass]:
+      cfg = fdl.Config(FrozenSampleClass)
       cfg.arg1 = x
       cfg.arg2 = str(x)
       return cfg
 
     @auto_config.auto_config
     def parent():
-      return SampleClass(arg1=simple(42), arg2=5)
+      return FrozenSampleClass(arg1=simple(42), arg2=5)
 
-    expected = SampleClass(arg1=SampleClass(42, '42'), arg2=5)
+    expected = FrozenSampleClass(arg1=FrozenSampleClass(42, '42'), arg2=5)
 
     self.assertEqual(expected, parent())
 
   def test_nested_python_execution(self):
 
     @auto_config.auto_unconfig
-    def simple(x: int) -> fdl.Config[SampleClass]:
-      cfg = fdl.Config(SampleClass)
+    def simple(x: int) -> fdl.Config[FrozenSampleClass]:
+      cfg = fdl.Config(FrozenSampleClass)
       cfg.arg1 = x
       cfg.arg2 = str(x)
       return cfg
 
-    def regular_python_wrapper(x) -> SampleClass:
+    def regular_python_wrapper(x) -> FrozenSampleClass:
       return simple(x - 1)
 
     @auto_config.auto_unconfig
-    def parent() -> fdl.Config[SampleClass]:
-      cfg = fdl.Config(SampleClass)
+    def parent() -> fdl.Config[FrozenSampleClass]:
+      cfg = fdl.Config(FrozenSampleClass)
       cfg.arg1 = fdl.Config(regular_python_wrapper, 42)
       cfg.arg2 = 5
       return cfg
 
-    expected = SampleClass(SampleClass(41, '41'), 5)
+    expected = FrozenSampleClass(FrozenSampleClass(41, '41'), 5)
     self.assertEqual(expected, parent())
 
 
 class InlineTest(test_util.TestCase):
 
   def test_simple(self):
 
     @auto_config.auto_config
     def my_fn(x: int, y: str):
-      return SampleClass(basic_fn(x), y)
+      return FrozenSampleClass(basic_fn(x), y)
 
     cfg = fdl.Config(my_fn, x=4, y='y')
     orig = fdl.build(cfg)
     auto_config.inline(cfg)
 
-    self.assertEqual(SampleClass, fdl.get_callable(cfg))
+    self.assertEqual(FrozenSampleClass, fdl.get_callable(cfg))
     self.assertEqual(cfg.arg2, 'y')
     self.assertIsInstance(cfg.arg1, fdl.Config)
     self.assertEqual(basic_fn, fdl.get_callable(cfg.arg1))
     self.assertEqual(4, cfg.arg1.arg)
     self.assertEqual(orig, fdl.build(cfg))
 
   def test_bound_auto_config(self):
@@ -1069,86 +1287,88 @@
     self.assertEqual(cfg.y, 7)
     self.assertEqual(orig, fdl.build(cfg))
 
   def test_always_inline_default_is_true(self):
 
     @auto_config.auto_config
     def inlined_fn():
-      return SampleClass(arg1=1, arg2=2)
+      return FrozenSampleClass(arg1=1, arg2=2)
 
     @auto_config.auto_config
     def calling_fn():
       return inlined_fn()
 
-    expected_config = fdl.Config(SampleClass, arg1=1, arg2=2)
+    expected_config = fdl.Config(FrozenSampleClass, arg1=1, arg2=2)
     actual_config = calling_fn.as_buildable()
     self.assertEqual(expected_config, actual_config)
 
   def test_inlining_nested_config(self):
 
     @auto_config.auto_config(experimental_always_inline=False)
-    def make_library_type(x: int, y: str) -> SampleClass:
+    def make_library_type(x: int, y: str) -> FrozenSampleClass:
       """A function that forms a configuration API boundary.
 
       These functions are often vended by libraries.
 
       Args:
        x: A sample argument to be configured.
        y: An additional argument to be configured.
 
       Returns:
         An instance of the sample class configured per the policy encapsulated
         by this function.
       """
-      return SampleClass(arg1=x + 1, arg2='Hello ' + y)
+      return FrozenSampleClass(arg1=x + 1, arg2='Hello ' + y)
 
     @auto_config.auto_config
     def make_experiment():
       thing1 = basic_fn(arg=5)
       thing2 = make_library_type(5, 'world')
-      return SampleClass(thing1, thing2)
+      return FrozenSampleClass(thing1, thing2)
 
     expected_config = fdl.Config(
-        SampleClass,
+        FrozenSampleClass,
         arg1=fdl.Config(basic_fn, arg=5),
-        arg2=fdl.Config(make_library_type, 5, 'world'))
+        arg2=fdl.Config(make_library_type, 5, 'world'),
+    )
 
     actual_config = make_experiment.as_buildable()
     self.assertEqual(expected_config, actual_config)
 
     auto_config.inline(actual_config.arg2)
 
     inline_expected_config = fdl.Config(
-        SampleClass,
+        FrozenSampleClass,
         arg1=fdl.Config(basic_fn, arg=5),
-        arg2=fdl.Config(SampleClass, 6, 'Hello world'))
+        arg2=fdl.Config(FrozenSampleClass, 6, 'Hello world'),
+    )
 
     self.assertEqual(inline_expected_config, actual_config)
 
   # TODO(b/272374472): Investigate fixing this.
   @absltest.skip('Cannot inline a function that returns a partial currently.')
   def test_inlined_func_returns_partial(self):
 
     @auto_config.auto_config
     def my_fn(x: int):
-      return functools.partial(SampleClass, arg1=x)
+      return functools.partial(FrozenSampleClass, arg1=x)
 
     cfg = fdl.Config(my_fn, x=2)
     auto_config.inline(cfg)
-    expected = fdl.Partial(SampleClass, arg1=2)
+    expected = fdl.Partial(FrozenSampleClass, arg1=2)
 
     self.assertDagEqual(cfg, expected)
-    self.assertEqual(fdl.build(cfg)(4), SampleClass(2, 4))
+    self.assertEqual(fdl.build(cfg)(4), FrozenSampleClass(2, 4))
 
   @absltest.skip('Cannot inline a function that returns a non-buildable.')
   def test_inlined_func_returns_list(self):
 
     @auto_config.auto_config
     def my_fn(x: int):
-      return [SampleClass(x, x), SampleClass(x + 1, x + 2)]
+      return [FrozenSampleClass(x, x), FrozenSampleClass(x + 1, x + 2)]
 
     cfg = fdl.Config(my_fn, x=2)
     auto_config.inline(cfg)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/autobuilders/__init__.py` & `fiddle-0.2.7/fiddle/_src/experimental/autobuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/autobuilders/autobuilders.py` & `fiddle-0.2.7/fiddle/_src/experimental/autobuilders/autobuilders.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/autobuilders/autobuilders_test.py` & `fiddle-0.2.7/fiddle/_src/experimental/autobuilders/autobuilders_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py` & `fiddle-0.2.7/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/configurator.py` & `fiddle-0.2.7/fiddle/_src/experimental/configurator.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/daglish_legacy.py` & `fiddle-0.2.7/fiddle/_src/experimental/daglish_legacy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/daglish_legacy_test.py` & `fiddle-0.2.7/fiddle/_src/experimental/daglish_legacy_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/dataclasses_test.py` & `fiddle-0.2.7/fiddle/_src/experimental/dataclasses_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 # limitations under the License.
 
 """Tests for dataclasses."""
 
 import dataclasses
 import functools
 import types
-from typing import Any, Dict, Callable
+from typing import Any, Callable, Dict
 
 from absl.testing import absltest
 import fiddle as fdl
+from fiddle import daglish
 from fiddle._src.experimental import auto_config
-from fiddle._src.experimental import dataclasses as fdl_dc
 from fiddle._src.testing import test_util
+from fiddle._src.testing.example import fake_encoder_decoder
+from fiddle.experimental import dataclasses as fdl_dc
 
 
 class SampleTag(fdl.Tag):
   """A tag used in testing."""
 
 
 class AdditionalTag(fdl.Tag):
@@ -156,14 +158,25 @@
 
 
 @dataclasses.dataclass
 class E:
   d_factory: Callable[..., D2] = fdl_dc.field(default_factory=D2.factory)
 
 
+@dataclasses.dataclass
+class PostInitDataclass:
+  a: int = 1
+  b: int = 2
+  c: int = dataclasses.field(init=False)
+
+  def __post_init__(self):
+    self.b += 1
+    self.c = self.a + 30
+
+
 class DataclassesTest(test_util.TestCase):
 
   def test_dataclass_tagging(self):
     config = fdl.Config(ATaggedType)
 
     self.assertEqual({SampleTag}, fdl.get_tags(config, 'tagged'))
     self.assertEqual({SampleTag, AdditionalTag},
@@ -365,10 +378,58 @@
     with self.subTest('do_not_delete_configruable_factory'):
       # In this test, we change to a class whose default value for `child` is
       # None; but we leave the fdl.Config built with the configurable factory.
       cfg = fdl.Config(ParentWithATaggedTypeChild)
       fdl.update_callable(cfg, ParentWithOptionalChild)
       self.assertEqual(fdl.get_callable(cfg.child), ATaggedType)
 
+  def test_convert_dataclasses_to_configs(self):
+    model = fake_encoder_decoder.fixture()
+    config = fdl_dc.convert_dataclasses_to_configs(model)
+    self.assertIsInstance(model, fake_encoder_decoder.FakeEncoderDecoder)
+    self.assertIsInstance(config, fdl.Config)
+    self.assertEqual(
+        fdl.get_callable(config), fake_encoder_decoder.FakeEncoderDecoder
+    )
+    self.assertIsInstance(config.encoder.mlp, fdl.Config)
+    self.assertEqual(
+        fdl.get_callable(config.encoder.mlp), fake_encoder_decoder.Mlp
+    )
+    self.assertEqual(model, fdl.build(config))
+
+  def test_post_init_dataclass_conversion(self):
+    dc = PostInitDataclass()
+    with self.assertRaisesRegex(ValueError, 'Dataclasses.*__post_init__.*'):
+      fdl_dc.convert_dataclasses_to_configs(dc)
+
+    config = fdl_dc.convert_dataclasses_to_configs(dc, allow_post_init=True)
+    self.assertNotEqual(dc, fdl.build(config))
+
+  def test_convert_reference_to_dataclass(self):
+    value = {'foo': PostInitDataclass}
+    self.assertEqual(fdl_dc.convert_dataclasses_to_configs(value), value)
+
+  def test_traverse_dataclass_values(self):
+    dc = fake_encoder_decoder.Mlp(
+        dtype=32, use_bias=False, sharding_axes=['foo', 'bar']
+    )
+
+    def traverse(value, state: daglish.State):
+      if isinstance(value, int) and not isinstance(value, bool):
+        return {'value': value}
+      else:
+        return state.map_children(value)
+
+    state = daglish.MemoizedTraversal(
+        traverse, dc, fdl_dc.daglish_dataclass_registry
+    ).initial_state()
+    transformed = traverse(dc, state)
+    self.assertEqual(
+        transformed,
+        fake_encoder_decoder.Mlp(
+            dtype={'value': 32}, use_bias=False, sharding_axes=['foo', 'bar']
+        ),
+    )
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/dict_config.py` & `fiddle-0.2.7/fiddle/_src/experimental/dict_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/dict_config_test.py` & `fiddle-0.2.7/fiddle/_src/experimental/dict_config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/fixture_node.py` & `fiddle-0.2.7/fiddle/_src/experimental/fixture_node.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/fixture_node_test.py` & `fiddle-0.2.7/fiddle/_src/experimental/fixture_node_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/namespace_config.py` & `fiddle-0.2.7/fiddle/_src/experimental/namespace_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/namespace_config_test.py` & `fiddle-0.2.7/fiddle/_src/experimental/namespace_config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/serialization.py` & `fiddle-0.2.7/fiddle/_src/experimental/serialization.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/tied_value.py` & `fiddle-0.2.7/fiddle/_src/experimental/tied_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,23 @@
 
 
 def _identity(value: ValueT) -> ValueT:
   """Returns `value` modified."""
   return value
 
 
-def new(value: ValueT) -> TiedValue[ValueT]:
-  """Returns a new TiedValue (unless value is already a TiedValue).
+def tied_value(value: ValueT) -> TiedValue[ValueT]:
+  """Creates a TiedValue (unless value is already a TiedValue).
 
   Args:
-    value: Value to tie; if it is already a TiedValue it is returned unmodified.
+    value: Value to tie.
+
+  Returns:
+    TiedValue: A new TiedValue, or if argument is already a TiedValue it is
+      returned unmodified.
   """
   return value if isinstance(value, TiedValue) else TiedValue(_identity, value)
 
 
 def untie(parent: config_lib.Buildable, attribute: str) -> None:
   """Unties a configuration value assigned to a parent Buildable field.
```

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/tied_value_test.py` & `fiddle-0.2.7/fiddle/_src/experimental/tied_value_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,54 +11,61 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tied_value."""
 
+import copy
+
 from absl.testing import absltest
+from absl.testing import parameterized
 import fiddle as fdl
 from fiddle._src.experimental import tied_value
 from fiddle._src.testing.example import fake_encoder_decoder
 
 
 class DType(fdl.Tag):
   """Sample dtype tag."""
 
 
 def tied_config():
   config = fake_encoder_decoder.fixture.as_buildable().encoder
-  config.attention.dtype = config.mlp.dtype = tied_value.new(value='float32')
+  config.attention.dtype = config.mlp.dtype = tied_value.tied_value(
+      value='float32'
+  )
   return config
 
 
 def tied_tagged_config():
   """Tests the interaction between TaggedValueCls and TiedValue."""
   config = fake_encoder_decoder.fixture.as_buildable().encoder
-  config.attention.dtype = config.mlp.dtype = tied_value.new(
-      DType.new('float32'))
+  config.attention.dtype = config.mlp.dtype = tied_value.tied_value(
+      DType.new('float32')
+  )
   return config
 
 
 def tagged_tied_config():
   """Tests the interaction between TaggedValueCls and TiedValue."""
   config = fake_encoder_decoder.fixture.as_buildable().encoder
   config.attention.dtype = config.mlp.dtype = DType.new(
-      tied_value.new('float32'))
+      tied_value.tied_value('float32')
+  )
   return config
 
 
-class TiedValueTest(absltest.TestCase):
+class TiedValueTest(parameterized.TestCase):
 
   def test_new_doesnt_rewrap(self):
-    tied = tied_value.new(value='float32')
+    tied = tied_value.tied_value(value='float32')
     self.assertIsInstance(tied, tied_value.TiedValue)
     self.assertEqual(tied.value, 'float32')
 
-    wrapped = tied_value.new(tied)
+    wrapped = tied_value.tied_value(tied)
     self.assertIs(wrapped, tied)
 
   def test_basic_sharing(self):
     config = tied_config()
     encoder = fdl.build(config)
     self.assertEqual(encoder.attention.dtype, 'float32')
     self.assertEqual(encoder.mlp.dtype, 'float32')
@@ -72,25 +79,31 @@
     # Sets the shared field through the other path.
     config = tied_config()
     config.mlp.dtype = 'float64'
     encoder = fdl.build(config)
     self.assertEqual(encoder.attention.dtype, 'float64')
     self.assertEqual(encoder.mlp.dtype, 'float64')
 
-  def test_tagged_and_tied_iteraction(self):
+  @parameterized.named_parameters(
+      ('tied_config', tied_tagged_config()),
+      ('tagged_config', tagged_tied_config()),
+  )
+  def test_tagged_and_tied_iteraction(self, config):
     """Tests interaction between values that are tagged and tied.
 
     Note: This only applies to TaggedValueCls, which is a bit legacy. Usually
     tags attached to fields should be used.
+
+    Args:
+      config: The configuration to check.
     """
-    for config in [tied_tagged_config(), tagged_tied_config()]:
-      config.attention.dtype.value = 'bfloat16'
-      encoder = fdl.build(config)
-      self.assertEqual(encoder.attention.dtype, 'bfloat16')
-      self.assertEqual(encoder.mlp.dtype, 'bfloat16')
+    config.attention.dtype = 'bfloat16'
+    encoder = fdl.build(config)
+    self.assertEqual(encoder.attention.dtype, 'bfloat16')
+    self.assertEqual(encoder.mlp.dtype, 'bfloat16')
 
   def test_untie_and_set_tied(self):
     config = tied_config()
     tied_value.untie(config.attention, 'dtype')
     config.attention.dtype = 'bfloat16'
     encoder = fdl.build(config)
     self.assertEqual(encoder.attention.dtype, 'bfloat16')
@@ -119,14 +132,48 @@
     config.attention.dtype = object_value
     encoder = fdl.build(config)
     self.assertIs(encoder.attention.dtype, object_value)
     self.assertIs(encoder.mlp.dtype, object_value)
 
   def test_works_in_lists(self):
     """TiedValue works in lists, but you need to use `.value` here."""
-    config = [tied_value.new(1)] * 2 + [tied_value.new(2)]
+    config = [tied_value.tied_value(1)] * 2 + [tied_value.tied_value(2)]
     config[0].value = 3
     self.assertEqual(fdl.build(config), [3, 3, 2])
 
+  def test_overwrite_with_new_tied_value_breaks_ties(self):
+    """Overwriting with a new TiedValue breaks existing ties."""
+    config = tied_config()
+    config.attention.dtype = tied_value.tied_value('float64')
+    self.assertEqual(config.mlp.dtype, 'float32')
+    self.assertEqual(config.attention.dtype, 'float64')
+
+  def test_tied_value_preserves_ties_during_copy(self):
+    """Copying a Config with a TiedValue preserves the ties."""
+    config = fdl.Config(fake_encoder_decoder.Mlp)
+    config.dtype = tied_value.tied_value('float32')
+    config_copy = copy.copy(config)
+    config.dtype = 'float64'
+    self.assertEqual(config.dtype, 'float64')
+    self.assertEqual(config_copy.dtype, 'float64')
+
+  def test_tied_value_breaks_ties_during_deepcopy(self):
+    """Copying a Config with a TiedValue preserves the ties."""
+    config = fdl.Config(fake_encoder_decoder.Mlp)
+    config.dtype = tied_value.tied_value('float32')
+    config_copy = copy.deepcopy(config)
+    config_copy.dtype = 'float64'
+    self.assertEqual(config.dtype, 'float32')
+    self.assertEqual(config_copy.dtype, 'float64')
+
+  def test_overwrite_with_new_tied_value_during_copy_breaks_ties(self):
+    """Overwriting with a new TiedValue during copy breaks existing ties."""
+    config = fdl.Config(fake_encoder_decoder.Mlp)
+    config.dtype = tied_value.tied_value('float32')
+    config_copy = copy.copy(config)
+    config_copy.dtype = tied_value.tied_value('float64')
+    self.assertEqual(config.dtype, 'float32')
+    self.assertEqual(config_copy.dtype, 'float64')
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/transform.py` & `fiddle-0.2.7/fiddle/_src/experimental/transform.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/transform_test.py` & `fiddle-0.2.7/fiddle/_src/experimental/transform_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/visualize.py` & `fiddle-0.2.7/fiddle/_src/experimental/visualize.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,45 +20,22 @@
 having a few helper functions for trimming them for interactive demos and such
 can be valuable.
 """
 
 import copy
 import inspect
 import textwrap
-from typing import Any, Dict, Iterable, List, Optional, TypeVar
+from typing import Any, Dict, List, Optional, TypeVar
 
 from fiddle import daglish
 from fiddle import diffing
-from fiddle import graphviz
 from fiddle._src import config as config_lib
-from fiddle._src.experimental import daglish_legacy
+from fiddle._src import graphviz_custom_object
 
-
-def _raise_error():
-  """Helper function for `Trimmed` that raises an error."""
-  raise ValueError('Please do not call fdl.build() on a config tree with '
-                   'Trimmed() nodes. These nodes are for visualization only.')
-
-
-class Trimmed(config_lib.Config[type(None)], graphviz.CustomGraphvizBuildable):
-  """Represents a configuration that has been trimmed."""
-
-  def __init__(self):
-    super().__init__(_raise_error)
-
-  def __render_value__(self, api: graphviz.GraphvizRendererApi) -> Any:
-    return api.tag('i')('(trimmed...)')
-
-  @classmethod
-  def __unflatten__(
-      cls,
-      values: Iterable[Any],
-      metadata: config_lib.BuildableTraverserMetadata,
-  ):
-    return cls()
+Trimmed = graphviz_custom_object.Trimmed
 
 
 _T = TypeVar('_T')
 
 
 def trimmed(config: _T, trim: List[config_lib.Buildable]) -> _T:
   """Returns a deep copy of a Buildable, with certain nodes replaced.
@@ -73,43 +50,127 @@
     config: Root buildable object, or collection of buildables.
     trim: List of sub-buildables that will be replaced by Trimmed() instances.
 
   Returns:
     Copy of the Buildable with nodes replaced.
   """
 
-  return copy.deepcopy(config,
-                       {id(sub_config): Trimmed() for sub_config in trim})
+  return copy.deepcopy(
+      config, {id(sub_config): Trimmed() for sub_config in trim}
+  )
 
 
-def with_defaults_trimmed(config: _T) -> _T:
+def with_defaults_trimmed(config: _T, remove_deep_defaults: bool = False) -> _T:
   """Trims arguments that match their default values.
 
   Args:
     config: Root buildable object, or nested structure of Buildables.
+    remove_deep_defaults: Whether to remove defaults that are equal to
+      dataclass.field(default_factory=auto_config_fn) defaults. If any of these
+      default values have external references, i.e. they are shared, then they
+      will not be removed.
 
   Returns:
     Copy of the Buildable with args matching defaults removed.
   """
 
-  # TODO(b/241261427): Remove args matching dataclasses' default_factory too.
-  def traverse_fn(_, value):
-    new_value = (yield)
+  # We only need to run default initializers once per callable and config class.
+  # (buildable type, id(callable)) --> configuration object.
+  cached_deep_defaults = {}
+
+  def _get_default(buildable: config_lib.Buildable) -> config_lib.Buildable:
+    fn_or_cls = config_lib.get_callable(buildable)
+    key = (type(buildable), id(fn_or_cls))
+    if key in cached_deep_defaults:
+      return cached_deep_defaults[key]
+    result = type(buildable)(fn_or_cls)  # pytype: disable=not-instantiable
+    cached_deep_defaults[key] = result
+    return result
+
+  def can_remove_deep_default(
+      node: Any,
+      attr_name: str,
+      parent_state: daglish.State,
+  ) -> bool:
+    """Returns whether we can safely delete a deep default.
+
+    (This function presumes we've already checked equality with the default, and
+    helps to check that sharing isn't altered.)
+
+    Args:
+      node: Default node to delete.
+      attr_name: Attribute referring to `node`.
+      parent_state: State from the traversal, which should correspond to
+        `parent`.
+    """
+    valid_paths_to_node = [
+        (*parent_path, daglish.Attr(attr_name))
+        for parent_path in parent_state.get_all_paths(allow_caching=True)
+    ]
+
+    def _goes_through_node(path):
+      return any(
+          path[: len(node_path)] == node_path
+          for node_path in valid_paths_to_node
+      )
+
+    def _helper(value, substate: daglish.State) -> bool:
+      if not substate.is_traversable(value) or daglish.is_immutable(value):
+        return True
+
+      for sub_path in substate.get_all_paths():
+        if not _goes_through_node(sub_path):
+          return False
+      return all(substate.flattened_map_children(value).values)
+
+    # Creates a sub-traversal using a different function. We eventually might
+    # make this part of the daglish API.
+    sub_traversal = daglish.MemoizedTraversal(
+        traversal_fn=_helper,
+        root_obj=parent_state.traversal.root_obj,
+        registry=parent_state.traversal.registry,
+        paths_cache=parent_state.traversal.paths_cache,  # pytype: disable=attribute-error
+    )
+    state = daglish.State(
+        sub_traversal,
+        (*parent_state.current_path, daglish.Attr(attr_name)),
+        node,
+        parent_state,
+    )
+    return _helper(node, state)
+
+  def traverse_fn(value, state: daglish.State):
     if isinstance(value, config_lib.Buildable):
-      for name, attr_value in list(new_value.__arguments__.items()):
+      deep_defaults = {}
+      if remove_deep_defaults:
+        deep_defaults = _get_default(value).__arguments__
+
+      should_copy = True
+      for name, attr_value in list(value.__arguments__.items()):
         param = value.__signature__.parameters.get(name, None)
-        if (param is not None and
-            param.kind != inspect.Parameter.VAR_KEYWORD and
-            param.default == attr_value):
-          delattr(new_value, name)
-      return new_value
-    else:
-      return new_value
+        if param is None:
+          continue
+        param_default = (
+            deep_defaults[name] if name in deep_defaults else param.default
+        )
+        if (
+            param.kind != inspect.Parameter.VAR_KEYWORD
+            and param_default == attr_value
+            # All paths must flow through both the parent config (`value`) and
+            # the specific attribute which is being defaulted, in order for us
+            # to safely remove it.
+            and can_remove_deep_default(attr_value, name, state)
+        ):
+          if should_copy:
+            value = copy.copy(value)
+            should_copy = False
+          delattr(value, name)
+    return state.map_children(value)
 
-  return daglish_legacy.memoized_traverse(traverse_fn, config)
+  return daglish.MemoizedTraversal.run(traverse_fn, config)
 
 
 def depth_over(config: Any, depth: int) -> List[config_lib.Buildable]:
   """Returns a list of sub-Buildable objects over a given depth from the root.
 
   If a sub-Buildable has multiple paths from the root to it, its depth is the
   *minimum* distance of those paths.
@@ -123,16 +184,16 @@
     config: Root buildable object, or collection of buildable objects.
     depth: Depth value.
 
   Returns:
     List of all sub-Buildables with depth strictly greater than `depth`.
   """
   node_to_depth: Dict[int, int] = {}  # Buildable hash --> min depth.
-  id_to_node: Dict[int,
-                   config_lib.Buildable] = {}  # Buildable hash --> Buildable.
+  # Buildable hash --> Buildable.
+  id_to_node: Dict[int, config_lib.Buildable] = {}
 
   def _path_len(path: daglish.Path) -> int:
     return sum(1 if isinstance(elt, daglish.Attr) else 0 for elt in path)
 
   def traverse(node, state: daglish.State) -> None:
     if isinstance(node, config_lib.Buildable):
       all_paths = state.get_all_paths(allow_caching=True)
```

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/yaml_serialization.py` & `fiddle-0.2.7/fiddle/_src/experimental/yaml_serialization.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/experimental/yaml_serialization_test.py` & `fiddle-0.2.7/fiddle/_src/experimental/yaml_serialization_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/extensions/__init__.py` & `fiddle-0.2.7/fiddle/_src/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/extensions/flax_test.py` & `fiddle-0.2.7/fiddle/_src/extensions/flax_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/extensions/jax.py` & `fiddle-0.2.7/fiddle/_src/extensions/jax.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # limitations under the License.
 
 """Fiddle extensions to handle JAX code more elegantly.
 
 Currently this just affects codegen, graphviz, and other debugging functions.
 """
 
+from fiddle._src import daglish_extensions
 from fiddle._src.codegen import import_manager
 from fiddle._src.codegen import py_val_to_cst_converter
 from fiddle._src.codegen import special_value_codegen
 import jax
 from jax import numpy as jnp
-
 import libcst as cst
 
 
 def _make_jnp_importable(name: str) -> special_value_codegen.Importable:
   return special_value_codegen.SingleImportable(
       "jax.numpy", lambda jnp_name: f"{jnp_name}.{name}")
 
@@ -46,14 +46,35 @@
     (jnp.float16, _make_jnp_importable("float16")),
     (jnp.float32, _make_jnp_importable("float32")),
     (jnp.float64, _make_jnp_importable("float64")),
     (jnp.complex64, _make_jnp_importable("complex64")),
     (jnp.complex128, _make_jnp_importable("complex128")),
 )
 
+_jax_initializers = (
+    jax.nn.initializers.constant,
+    jax.nn.initializers.delta_orthogonal,
+    jax.nn.initializers.glorot_normal,
+    jax.nn.initializers.glorot_uniform,
+    jax.nn.initializers.he_normal,
+    jax.nn.initializers.he_uniform,
+    jax.nn.initializers.kaiming_normal,
+    jax.nn.initializers.kaiming_uniform,
+    jax.nn.initializers.lecun_normal,
+    jax.nn.initializers.lecun_uniform,
+    jax.nn.initializers.normal,
+    jax.nn.initializers.ones,
+    jax.nn.initializers.orthogonal,
+    jax.nn.initializers.uniform,
+    jax.nn.initializers.variance_scaling,
+    jax.nn.initializers.xavier_normal,
+    jax.nn.initializers.xavier_uniform,
+    jax.nn.initializers.zeros,
+)
+
 _import_aliases = (
     # Rewrite internal import for JAX initializers.
     ("jax._src.nn.initializers", "from jax.nn import initializers"),
     ("jax.numpy", "from jax import numpy as jnp"),
 )
 
 
@@ -110,7 +131,14 @@
   for module_str, import_stmt in _import_aliases:
     import_manager.register_import_alias(module_str, import_stmt)
 
   # The odd calling syntax here ("register(type)(handler)") comes from the fact
   # that register_converter is usually a decorator, but we call it directly.
   py_val_to_cst_converter.register_py_val_to_cst_converter(is_jnp_device_array)(
       convert_jnp_device_array_to_cst)
+
+  for dtype, _ in _jnp_type_importables:
+    daglish_extensions.register_immutable(dtype)
+
+  for init in _jax_initializers:
+    daglish_extensions.register_immutable(init)
+    daglish_extensions.register_function_with_immutable_return_value(init)
```

### Comparing `fiddle-0.2.6/fiddle/_src/extensions/seqio.py` & `fiddle-0.2.7/fiddle/_src/extensions/seqio.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/extensions/seqio_test.py` & `fiddle-0.2.7/fiddle/_src/extensions/seqio_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """Tests for fiddle.extensions.seqio."""
 
 from typing import List
 
 from absl.testing import absltest
 import fiddle as fdl
-from fiddle._src.codegen import codegen
+from fiddle._src.codegen import legacy_codegen
 import fiddle.extensions.seqio
 import seqio
 
 
 def tokens(code: str) -> List[str]:
   return code.strip().split()
 
@@ -31,15 +31,15 @@
 class SeqioTest(absltest.TestCase):
 
   def test_codegen(self):
     fiddle.extensions.seqio.enable()
     cfg = fdl.Config(
         seqio.Evaluator,
         feature_converter=fdl.Config(seqio.DecoderFeatureConverter))
-    code = "\n".join(codegen.codegen_dot_syntax(cfg).lines())
+    code = "\n".join(legacy_codegen.codegen_dot_syntax(cfg).lines())
     expected = """
 import fiddle as fdl
 import seqio
 
 
 def build_config():
   root = fdl.Config(seqio.Evaluator)
```

### Comparing `fiddle-0.2.6/fiddle/_src/extensions/tf.py` & `fiddle-0.2.7/fiddle/_src/extensions/tf.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/extensions/tf_test.py` & `fiddle-0.2.7/fiddle/_src/extensions/tf_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from typing import List
 
 from absl.testing import absltest
 from absl.testing import parameterized
 import fiddle as fdl
 from fiddle import graphviz
 from fiddle import printing
-from fiddle._src.codegen import codegen
 from fiddle._src.codegen import formatting_utilities
+from fiddle._src.codegen import legacy_codegen
 from fiddle._src.codegen import py_val_to_cst_converter
 from fiddle._src.codegen import special_value_codegen
 from fiddle._src.experimental import serialization
 import fiddle.extensions.tf
 import libcst as cst
 import tensorflow as tf
 
@@ -65,15 +65,15 @@
     float32_value = special_value_codegen.transform_py_value(
         tf.float32, import_manager)
     self.assertEqual(import_manager.calls, ["tensorflow"])
     self.assertEqual(repr(float32_value), "tensorflow.float32")
 
   def test_codegen(self):
     config = fdl.Config(foo, dtype=tf.bfloat16)
-    code = "\n".join(codegen.codegen_dot_syntax(config).lines())
+    code = "\n".join(legacy_codegen.codegen_dot_syntax(config).lines())
     if __name__ == "__main__":
       tf_test_import = ""
       foo_name = "foo"
     else:
       # Running via PyTest; tf_test is importable.
       tf_test_import = "from fiddle._src.extensions import tf_test\n"
       foo_name = "tf_test.foo"
```

### Comparing `fiddle-0.2.6/fiddle/_src/field_metadata.py` & `fiddle-0.2.7/fiddle/_src/field_metadata.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/graphviz.py` & `fiddle-0.2.7/fiddle/_src/graphviz.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Provides a renderer to visualize a DAG of `fdl.Buildable`s via Graphviz."""
 
-import abc
 import collections
 import colorsys
 import copy
 import dataclasses
 import functools
 import html
 import itertools
 import types
 
 from typing import Any, Callable, Dict, List, NamedTuple, Optional, Set, Tuple, Type, Union
 
 from fiddle._src import config as config_lib
 from fiddle._src import daglish
 from fiddle._src import diffing
+from fiddle._src import graphviz_custom_object
 from fiddle._src import tag_type
 from fiddle._src import tagging
 from fiddle._src.codegen import formatting_utilities
 from fiddle._src.experimental import daglish_legacy
+from fiddle._src.experimental import visualize
 import graphviz
-import typing_extensions
 
 _BUILDABLE_INSTANCE_COLORS = [
     '#ffc0cb',  # pink
     '#90ee90',  # lightgreen
     '#fff8dc',  # cornsilk
     '#ffa07a',  # lightsalmon
     '#add8e6',  # lightblue
@@ -76,32 +76,14 @@
   number of items that were trimmed.
   """
 
 
 _TRIMMED_SENTINEL = _TrimmedSentinel()
 
 
-class GraphvizRendererApi(typing_extensions.Protocol):
-  """API of _GraphvizRenderer exposed to CustomGraphvizBuildable subclasses."""
-
-  def tag(self, tag: str, **kwargs) -> Callable[[Any], str]:
-    raise NotImplementedError()
-
-
-class CustomGraphvizBuildable(metaclass=abc.ABCMeta):
-  """Mixin class that marks a Buildable has having a custom __render_value__.
-
-  This lets certain special-purpose Buildables customize how they are rendered.
-  """
-
-  @abc.abstractmethod
-  def __render_value__(self, api: GraphvizRendererApi) -> Any:
-    """Renders this Buildable as a value."""
-
-
 @dataclasses.dataclass(frozen=True)
 class _NoValue:
   """Sentinel object used by _ChangedValue to mark missing values."""
 
 
 @dataclasses.dataclass
 class _ChangedValue:
@@ -417,15 +399,15 @@
         key_format_fn=str,
         tags=config.tags)
 
   def _render_value(self, value: Any, color=_DEFAULT_HEADER_COLOR) -> str:
     """Returns an HTML string rendering `value`."""
     if value is tagging.NO_VALUE:
       return self.tag('i')('tagging.NO_VALUE')
-    elif isinstance(value, CustomGraphvizBuildable):
+    elif isinstance(value, graphviz_custom_object.CustomGraphvizBuildable):
       return value.__render_value__(self)
     elif isinstance(value, tagging.TaggedValueCls):
       return self._render_tagged_value(value, color)
     elif isinstance(value, config_lib.Buildable):
       return self._render_config(value, color)
     elif isinstance(value, _ChangedValue):
       return self._render_changed_value(value)
@@ -461,17 +443,18 @@
     Returns:
       The HTML markup for the rectangle (a single-celled table) that is
       connected by an edge to the node for `value`.
     """
     # If this is not a Buildable or shared value, then render it using
     # _render_value.
     buildable_types = (config_lib.Buildable, _ChangedBuildable)
-    if not (id(value) in self._shared_value_ids or
-            (isinstance(value, buildable_types) and
-             not isinstance(value, CustomGraphvizBuildable))):
+    is_standard_buildable = isinstance(
+        value, buildable_types
+    ) and not isinstance(value, graphviz_custom_object.CustomGraphvizBuildable)
+    if not (id(value) in self._shared_value_ids or is_standard_buildable):
       return self._render_value(value)
 
     # First, add the value to the graph. This will add a separate node and
     # render it as a separate table (but is a no-op if it's already added).
     self._add_node_for_value(value)
 
     # Look up the node id for the value, and get a new unique port name to
@@ -609,32 +592,45 @@
     if value.old_value != _NoValue() and value.new_value != _NoValue():
       row.append(td('&rarr;'))
     if value.new_value != _NoValue():
       row.append(td_add(self._render_nested_value(value.new_value)))
     return table(tr(row))
 
 
-def render(config: Any) -> graphviz.Graph:
+def render(
+    config: Any,
+    max_depth: Optional[int] = None,
+    max_str_length: Optional[int] = None,
+) -> graphviz.Graph:
   """Renders the given ``config`` as a ``graphviz.Graph``.
 
   Each config is rendered as a table of keys and values (with a header row).
   Any nested configs get their own separate table, with an edge pointing to
   their location in their parent config. If a config instance is present in
   multiple parent configs, it is only rendered once but will have multiple
   edges to parent configs.
 
   Args:
     config: The ``fdl.Buildable`` (or nested structure of ``fdl.Buildable``'s)
       to render.
+    max_depth: Max depth of nodes to render.
+    max_str_length: Max length of long string fields or object repr's in a
+      config.
 
   Returns:
     A ``graphviz.Graph`` object containing the resulting rendering of
     ``config``. Standard ``graphviz`` methods can then be used to export this to
     a file.
   """
+  if max_depth is not None:
+    config = visualize.trimmed(
+        config, trim=visualize.depth_over(config, depth=max_depth)
+    )
+  if max_str_length is not None:
+    config = visualize.trim_long_fields(config, threshold=max_str_length)
   return _GraphvizRenderer().render(config)
 
 
 def render_diff(diff: Optional[diffing.Diff] = None,
                 *,
                 old: Optional[Any] = None,
                 new: Optional[Any] = None,
```

### Comparing `fiddle-0.2.6/fiddle/_src/history.py` & `fiddle-0.2.7/fiddle/_src/history.py`

 * *Files 4% similar despite different names*

```diff
@@ -237,20 +237,37 @@
 
       with history.suspend_tracking():
         ...  # Modifications made here won't affect Buildable history.
 
   Yields:
     There is no associated yield value.
   """
-  previous_value = _tracking_state.enabled
-  _tracking_state.enabled = False
+  previous_enabled = tracking_enabled()
+  set_tracking(enabled=False)
   try:
     yield
   finally:
-    _tracking_state.enabled = previous_value
+    set_tracking(enabled=previous_enabled)
+
+
+def set_tracking(enabled: bool):
+  """Sets whether Fiddle performs history tracking.
+
+  For performance reasons, it can be valuable to disable history tracking. This
+  function enables callers to imperatively control whether Fiddle tracks
+  mutations to Buildable objects. To disable history tracking::
+
+    history.set_tracking(enabled=False)
+
+  Note: where possible, prefer the context manager ``suspend_tracking`` instead.
+
+  Args:
+    enabled: Whether history tracking should be enabled.
+  """
+  _tracking_state.enabled = enabled
 
 
 def tracking_enabled() -> bool:
   """Returns whether history tracking is currently enabled."""
   return _tracking_state.enabled
```

### Comparing `fiddle-0.2.6/fiddle/_src/history_test.py` & `fiddle-0.2.7/fiddle/_src/history_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/materialize.py` & `fiddle-0.2.7/fiddle/_src/materialize.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/materialize_test.py` & `fiddle-0.2.7/fiddle/_src/materialize_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/module_reflection.py` & `fiddle-0.2.7/fiddle/_src/module_reflection.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/module_reflection_test.py` & `fiddle-0.2.7/fiddle/_src/module_reflection_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/module_reflection_test_module.py` & `fiddle-0.2.7/fiddle/_src/module_reflection_test_module.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/mutate_buildable.py` & `fiddle-0.2.7/fiddle/_src/mutate_buildable.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/mutate_buildable_test.py` & `fiddle-0.2.7/fiddle/_src/mutate_buildable_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/printing.py` & `fiddle-0.2.7/fiddle/_src/printing.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/printing_test.py` & `fiddle-0.2.7/fiddle/_src/printing_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,25 +239,14 @@
     output = printing.as_str_flattened(cfg)
 
     self.check_result(
         output, f"""\
         x = 'cba' {SampleTag} {SampleTag2}
         y = 'cba' {SampleTag} {SampleTag2}""")
 
-  def test_tagged_config(self):
-    cfg = fdl.Config(
-        fn_x_y,
-        x=fdl.TaggedValue(tags=(SampleTag,), default=fdl.Config(SampleClass)),
-    )
-    output = printing.as_str_flattened(cfg)
-    self.check_result(
-        output, f"""\
-        x = <Config[SampleClass()]> {SampleTag}
-        y = <[unset]>""")
-
   def test_argument_tags(self):
     cfg = fdl.Config(fn_x_y, y='abc')
     fdl.add_tag(cfg, 'x', SampleTag)
     fdl.add_tag(cfg, 'y', SampleTag)
     output = printing.as_str_flattened(cfg)
 
     self.check_result(
```

### Comparing `fiddle-0.2.6/fiddle/_src/reraised_exception.py` & `fiddle-0.2.7/fiddle/_src/reraised_exception.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/reraised_exception_test.py` & `fiddle-0.2.7/fiddle/_src/reraised_exception_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/selectors.py` & `fiddle-0.2.7/fiddle/_src/selectors.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/selectors_test.py` & `fiddle-0.2.7/fiddle/_src/selectors_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/signatures.py` & `fiddle-0.2.7/fiddle/_src/signatures.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,23 +13,38 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Module for getting (and caching) inspect.Signature objects."""
 
 import dataclasses
 import inspect
-from typing import Any, Callable, Dict, Type
+from typing import Any, Callable, Dict, Generic, Type
 import weakref
 import typing_extensions
 
 _signature_cache = weakref.WeakKeyDictionary()
 _type_hints_cache = weakref.WeakKeyDictionary()
 
 
 def _get_signature_uncached(fn_or_cls) -> inspect.Signature:
+  """Returns the signature for a function or class.
+
+  This mostly calls inspect.signature, but handles generics and some builtin
+  types better.
+
+  Args:
+    fn_or_cls: Function or class callable.
+  """
+  # TODO(b/285387519): Switch to typing.get_origin after dropping Python 3.8
+  # support.
+  origin = typing_extensions.get_origin(fn_or_cls)
+  fn_or_cls = origin if origin is not None else fn_or_cls
+  if isinstance(fn_or_cls, type) and issubclass(fn_or_cls, Generic):
+    fn_or_cls = fn_or_cls.__init__
+
   try:
     return inspect.signature(fn_or_cls)
   except ValueError:
     if isinstance(fn_or_cls, type) and hasattr(fn_or_cls, '__call__'):
       try:
         return inspect.signature(fn_or_cls.__call__)
       except ValueError:
```

### Comparing `fiddle-0.2.6/fiddle/_src/signatures_test.py` & `fiddle-0.2.7/fiddle/_src/signatures_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/signatures_test_helper.py` & `fiddle-0.2.7/fiddle/_src/signatures_test_helper.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/tag_type.py` & `fiddle-0.2.7/fiddle/_src/tag_type.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/tagging.py` & `fiddle-0.2.7/fiddle/_src/tagging.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,27 +58,29 @@
 """
 
 from __future__ import annotations
 
 import collections
 import inspect
 import typing
-from typing import Any, Collection, FrozenSet, Generic, Optional, Set, TypeVar, Union
+from typing import Any, Collection, FrozenSet, Optional, TypeVar, Union
 
 from fiddle._src import config
 from fiddle._src import daglish
 from fiddle._src import tag_type
 from fiddle._src.experimental import auto_config
 
 TagType = tag_type.TagType
 TaggedValueNotFilledError = tag_type.TaggedValueNotFilledError
 
 NO_VALUE = config.NO_VALUE
 NoValue = config.NoValue
 _NoValue = config.NoValue
+tagged_value_fn = config.tagged_value_fn
+TaggedValueCls = config.TaggedValueCls
 
 
 class Tag(metaclass=TagType):
   """Metadata associated with a Fiddle configurable value.
 
   To see a usage example, please see the documentation on the tagging module.
 
@@ -109,49 +111,14 @@
         auto_config.AutoConfig(
             func=new.__func__, buildable_func=new.__func__, always_inline=True))
 
 
 T = TypeVar('T')
 
 
-def tagged_value_fn(value: Union[T, NoValue] = NO_VALUE,
-                    tags: Optional[Set[TagType]] = None) -> T:
-  """Identity function to return value if set, and raise an error if not.
-
-  Args:
-    value: The value to return.
-    tags: The tags associated with the value. (Used in generating error messages
-      if `value` is not set.)
-
-  Returns:
-    The value `value` passed to it.
-  """
-  if value is NO_VALUE:
-    msg = ('Expected all `TaggedValue`s to be replaced via fdl.set_tagged() '
-           'calls, but one was not set.')
-    if tags:
-      msg += ' Unset tags: ' + str(tags)
-    raise TaggedValueNotFilledError(msg)
-  return value
-
-
-class TaggedValueCls(Generic[T], config.Config[T]):
-  """Placeholder class for TaggedValue instances."""
-
-  @property
-  def tags(self):
-    return self.__argument_tags__['value']
-
-  def __build__(self, *args: Any, **kwargs: Any) -> T:
-    if self.__fn_or_cls__ is not tagged_value_fn:
-      raise RuntimeError('Unexpected __fn_or_cls__ in TaggedValueCls; found:'
-                         f'{self.__fn_or_cls__}')
-    return self.__fn_or_cls__(tags=self.tags, *args, **kwargs)
-
-
 def TaggedValue(  # pylint: disable=invalid-name
     tags: Collection[TagType],
     default: Union[NoValue, T] = NO_VALUE,
 ) -> TaggedValueCls[T]:
   """Declares a value annotated with a set of ``Tag``'s.
 
   This is now basically a fdl.Config(lambda value: value) configuration, since
@@ -163,17 +130,19 @@
 
   Returns:
     Tagged value configuration object.
 
   Raises:
     ValueError: If `tags` is empty.
   """
-  result = TaggedValueCls(tagged_value_fn, value=default)
   if not tags:
     raise ValueError('At least one tag must be provided.')
+  result = TaggedValueCls(tagged_value_fn)
+  if default is not NO_VALUE:
+    result.value = default
   for tag in tags:
     config.add_tag(result, 'value', tag)
   return result
 
 
 def set_tagged(root: config.Buildable, *, tag: TagType, value: Any) -> None:
   """Sets all parameters in `root` tagged with `tag` to `value`.
@@ -229,17 +198,14 @@
 def materialize_tags(
     buildable: AnyBuildable,
     tags: Optional[collections.abc.Set[TagType]] = None,
     clear_field_tags: bool = False,
 ) -> AnyBuildable:
   """Materialize tagged fields with assigned values or default values.
 
-  TODO(b/242574056): Consider supporting tags directly on Config objects, e.g.
-  by removing those tags.
-
   Converts:
   ```foo.bar.baz = MyCustomTag.new(4096)```
 
   Into:
   ```foo.bar.baz = 4096```
 
   Args:
@@ -257,14 +223,19 @@
   """
 
   def transform(value, state: daglish.State):
     value = state.map_children(value)
     if isinstance(value, TaggedValueCls) and value.value != NO_VALUE and (
         tags is None or set(value.tags) & tags):
       return value.value
-    elif isinstance(value, config.Buildable) and clear_field_tags:
-      value.__argument_tags__.clear()
+    elif isinstance(value, config.Buildable):
+      if tags:
+        for tag_set in value.__argument_tags__.values():
+          for tag in tags:
+            tag_set.discard(tag)
+      if clear_field_tags:
+        value.__argument_tags__.clear()
       return value
     else:
       return value
 
   return daglish.MemoizedTraversal.run(transform, buildable)
```

### Comparing `fiddle-0.2.6/fiddle/_src/tagging_test.py` & `fiddle-0.2.7/fiddle/_src/tagging_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 
 from absl.testing import absltest
 import cloudpickle
 import fiddle as fdl
 from fiddle import selectors
 from fiddle._src import tagging
 from fiddle._src import tagging_test_module as tst
+from fiddle.experimental import auto_config
+from fiddle.experimental import dataclasses as fdl_dc
 
 
 @dataclasses.dataclass
 class Foo:
   bar: int
   qux: str
 
@@ -42,14 +44,29 @@
   """A custom tag used for testing."""
 
 
 def return_kwargs(**kwargs):
   return kwargs
 
 
+def sample_function(x, y):
+  return (x, y)
+
+
+@auto_config.auto_config
+def custom_default_factory():
+  return Foo(1, "2")
+
+
+@dataclasses.dataclass
+class Baz:
+  foo: Foo = fdl_dc.field(default_factory=custom_default_factory)
+  baz: int = 2
+
+
 def get_single_tag(tagged_value: tagging.TaggedValueCls) -> tagging.TagType:
   """Gets a single tag from a TaggedValue, errors if there are multiple."""
   assert isinstance(tagged_value, tagging.TaggedValueCls)
   assert len(tagged_value.tags) == 1
   return next(iter(tagged_value.tags))
 
 
@@ -116,50 +133,63 @@
       class Bar(tagging.Tag):  # pylint: disable=unused-variable
         """Bar tag."""
 
   def test_tagged_value_identity_fn_exception(self):
     with self.assertRaisesRegex(
         tagging.TaggedValueNotFilledError,
         "Expected.*TaggedValue.*replaced.*one was not set"):
-      tagging.tagged_value_fn()
+      tagging.tagged_value_fn(fdl.NO_VALUE)
 
   def test_tagged_value_identity_fn_none_value(self):
     # Test that when the value is None, that's OK.
     self.assertIsNone(tagging.tagged_value_fn(value=None))
 
   def test_tagged_value_error_message(self):
-    cfg = tagging.TaggedValue(tags={tst.ParameterDType})
+    cfg = fdl.Config(Foo)
+    cfg.bar = tagging.TaggedValue(tags={tst.ParameterDType})
     with self.assertRaisesRegex(
-        tagging.TaggedValueNotFilledError,
-        r"Unset tags: {fiddle._src.tagging_test_module.ParameterDType}",
+        TypeError,
+        (
+            r"Tags for unset arguments:\n - bar: "
+            r"#fiddle._src.tagging_test_module.ParameterDType"
+        ),
     ):
       fdl.build(cfg)
 
   def test_taggedvalue_default_none(self):
     cfg = tagging.TaggedValue(tags={tst.ParameterDType}, default=None)
     self.assertIsNone(fdl.build(cfg))
 
   def test_one_taggedvalue_unset_in_config(self):
     cfg = fdl.Config(
-        return_kwargs,
-        foo=tst.ParameterDType.new(default=None),
-        bar=tst.ParameterDType.new())
+        sample_function,
+        x=tst.ParameterDType.new(default=None),
+        y=tst.ParameterDType.new(),
+    )
     with self.assertRaisesRegex(
-        tagging.TaggedValueNotFilledError,
-        "Expected.*TaggedValue.*replaced.*one was not set"):
+        TypeError, r" - y: #fiddle._src.tagging_test_module.ParameterDType"
+    ):
       fdl.build(cfg)
 
   def test_set_tagged(self):
     cfg = fdl.Config(
         return_kwargs,
         foo=tst.ParameterDType.new(default=None),
-        bar=tst.LinearParamDType.new())
+        bar=tst.LinearParamDType.new(),
+    )
     tagging.set_tagged(cfg, tag=tst.LinearParamDType, value=1)
     self.assertDictEqual(fdl.build(cfg), {"foo": None, "bar": 1})
 
+  def test_tagging_dataclass_field_defaults(self):
+    cfg = fdl.Config(Baz, foo=RedTag.new())
+    obj = fdl.build(cfg)
+    self.assertEqual(
+        obj.foo.bar, 1, "Default values from dataclass field missing."
+    )
+
   def test_set_two_taggedvalues(self):
     cfg = fdl.Config(
         return_kwargs,
         foo=tst.ParameterDType.new(default=None),
         bar=tst.LinearParamDType.new())
     tagging.set_tagged(cfg, tag=tst.ParameterDType, value=1)
     tagging.set_tagged(cfg, tag=tst.LinearParamDType, value=2)
@@ -273,15 +303,21 @@
     copied.d = 40
 
     tagging.set_tagged(cfg, tag=tst.ParameterDType, value=1)
     tagging.set_tagged(cfg, tag=tst.ActivationDType, value=2)
 
     self.assertEqual(fdl.build(cfg), (1, 2, 1, 4))
 
-    with self.assertRaises(tagging.TaggedValueNotFilledError):
+    with self.assertRaisesRegex(
+        TypeError,
+        (
+            r".*Tags for unset arguments:\n - a:"
+            r" #fiddle._src.tagging_test_module.ParameterDType.*"
+        ),
+    ):
       fdl.build(copied)
 
     tagging.set_tagged(copied, tag=tst.ParameterDType, value=10)
     tagging.set_tagged(copied, tag=tst.ActivationDType, value=20)
     self.assertEqual(fdl.build(copied), (10, 20, 10, 40))
 
   def test_deepcopy_linked_value_object(self):
@@ -293,34 +329,43 @@
     cfg = fdl.Config(
         foo,
         a=fdl.TaggedValue(tags={tst.LinearParamDType}, default=shared_value),
         b=fdl.TaggedValue(tags={tst.LinearParamDType}, default=shared_value),
     )
     copied = copy.deepcopy(cfg)
     self.assertIsNot(copied.a, cfg.a)
-    self.assertIsNot(copied.a.value, cfg.a.value)
 
-    self.assertIs(get_single_tag(copied.a), get_single_tag(cfg.a))
-    self.assertIs(get_single_tag(copied.b), get_single_tag(cfg.b))
-    self.assertIs(cfg.a.value, cfg.b.value)
-    self.assertIs(copied.a.value, copied.b.value)
+    self.assertLen(fdl.get_tags(cfg, "a"), 1)
+    self.assertLen(fdl.get_tags(copied, "a"), 1)
+    self.assertIs(
+        list(fdl.get_tags(cfg, "a"))[0], list(fdl.get_tags(copied, "a"))[0]
+    )
+
+    self.assertLen(fdl.get_tags(cfg, "b"), 1)
+    self.assertLen(fdl.get_tags(copied, "b"), 1)
+    self.assertIs(
+        list(fdl.get_tags(cfg, "b"))[0], list(fdl.get_tags(copied, "b"))[0]
+    )
+
+    self.assertIs(cfg.a, cfg.b)
+    self.assertIs(copied.a, copied.b)
 
   def test_shallow_copy_tagged_values(self):
     cfg = tst.ParameterDType.new()
     copied = copy.copy(cfg)
 
     self.assertIs(get_single_tag(copied), tst.ParameterDType)
-    self.assertIs(copied.value, tagging.NO_VALUE)
+    self.assertFalse(hasattr(copied, "value"))
 
-    with self.assertRaises(tagging.TaggedValueNotFilledError):
+    with self.assertRaises(TypeError):
       fdl.build(copied)
     tagging.set_tagged(cfg, tag=tst.ParameterDType, value=1)
     self.assertEqual(fdl.build(cfg), 1)
 
-    with self.assertRaises(tagging.TaggedValueNotFilledError):
+    with self.assertRaises(TypeError):
       fdl.build(copied)
     tagging.set_tagged(copied, tag=tst.ParameterDType, value=2)
     self.assertEqual(fdl.build(cfg), 1)
     self.assertEqual(fdl.build(copied), 2)
 
   def test_multiple_keys(self):
     cfg = fdl.TaggedValue(
@@ -338,16 +383,15 @@
   def test_materialize_tags_keeps_tag_in_ignore_list(self):
     foo_cfg = fdl.Config(Foo)
     foo_cfg.bar = RedTag.new(5)
     foo_cfg.qux = "abc"
 
     foo_cfg = tagging.materialize_tags(
         foo_cfg, tags=set(tagging.list_tags(foo_cfg) - {RedTag}))
-    self.assertIsInstance(foo_cfg.bar, tagging.TaggedValueCls)
-    self.assertEqual(get_single_tag(foo_cfg.bar), RedTag)
+    self.assertEqual(frozenset([RedTag]), fdl.get_tags(foo_cfg, "bar"))
 
   def test_materialize_tags_removes_tag_when_default_provided(self):
     foo_cfg = fdl.Config(Foo)
     foo_cfg.bar = RedTag.new(5)
     foo_cfg.qux = "abc"
 
     foo_cfg = tagging.materialize_tags(foo_cfg)
@@ -366,16 +410,15 @@
 
   def test_materialize_tags_keeps_tag_when_no_default_provided(self):
     foo_cfg = fdl.Config(Foo)
     foo_cfg.bar = RedTag.new()
     foo_cfg.qux = "abc"
 
     foo_cfg = tagging.materialize_tags(foo_cfg)
-    self.assertIsInstance(foo_cfg.bar, tagging.TaggedValueCls)
-    self.assertEqual(get_single_tag(foo_cfg.bar), RedTag)
+    self.assertEqual(frozenset([RedTag]), fdl.get_tags(foo_cfg, "bar"))
 
   def test_materialize_tags_materializes_tag_in_tags_list(self):
     foo_cfg = fdl.Config(Foo)
     foo_cfg.bar = RedTag.new(5)
     foo_cfg.qux = "abc"
 
     foo_cfg = tagging.materialize_tags(foo_cfg, tags={RedTag})
@@ -384,16 +427,15 @@
 
   def test_materialize_tags_ignores_tag_not_in_tags_list(self):
     foo_cfg = fdl.Config(Foo)
     foo_cfg.bar = RedTag.new(5)
     foo_cfg.qux = "abc"
 
     foo_cfg = tagging.materialize_tags(foo_cfg, tags={BlueTag})
-    self.assertIsInstance(foo_cfg.bar, tagging.TaggedValueCls)
-    self.assertEqual(get_single_tag(foo_cfg.bar), RedTag)
+    self.assertEqual(frozenset([RedTag]), fdl.get_tags(foo_cfg, "bar"))
 
 
 # TODO(b/272077830): Test set_tagged that leverages tag inheritance.
 
 
 class TestWithSelectorMock(TaggingTest):
```

### Comparing `fiddle-0.2.6/fiddle/_src/tagging_test_module.py` & `fiddle-0.2.7/fiddle/_src/tagging_test_module.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/testing/__init__.py` & `fiddle-0.2.7/fiddle/_src/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/testing/autotest.py` & `fiddle-0.2.7/fiddle/_src/testing/autotest.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/testing/example/__init__.py` & `fiddle-0.2.7/fiddle/_src/testing/example/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/testing/example/demo_configs.py` & `fiddle-0.2.7/fiddle/_src/testing/example/demo_configs.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/testing/example/fake_encoder_decoder.py` & `fiddle-0.2.7/fiddle/_src/testing/example/fake_encoder_decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,19 @@
 
 @dataclasses.dataclass
 class FakeEncoderDecoder:
   encoder: FakeEncoder
   decoder: FakeDecoder
 
 
+@dataclasses.dataclass
+class ModelWrapper:
+  model: FakeEncoderDecoder
+
+
 @auto_config.auto_config
 def fixture():
   dtype = "float32"
   kernel_init = "uniform()"
   bias_init = "zeros()"
   shared_token_embedder = TokenEmbedder(dtype)
   return FakeEncoderDecoder(
```

### Comparing `fiddle-0.2.6/fiddle/_src/testing/example/person_friend_toy.py` & `fiddle-0.2.7/fiddle/_src/testing/example/person_friend_toy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/testing/nested_values.py` & `fiddle-0.2.7/fiddle/_src/testing/nested_values.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/testing/nested_values_test.py` & `fiddle-0.2.7/fiddle/_src/testing/nested_values_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/_src/testing/test_util.py` & `fiddle-0.2.7/fiddle/_src/testing/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     A set containing one element for each 'shared' object in `structure` (i.e.,
     each object that is reachable via multiple paths).  The element for each
     object is the set of paths that can be used to reach that object.
   """
   result = set()
 
   def collect_value(paths: daglish.Paths, value: Any):
-    if daglish.is_memoizable(value) and len(paths) > 1:
+    if not daglish.is_internable(value) and len(paths) > 1:
       result.add(frozenset(paths))
     return (yield)
 
   daglish_legacy.memoized_traverse(collect_value, structure)
   return result
 
 
@@ -117,35 +117,42 @@
       # For longer values, it's easier to spot differences if the two
       # values are displayed on separate lines.
       return f'* x{path_str}={x_repr} but\n  y{path_str}={y_repr}'
 
   def find_diffs(x_val, y_val, path):
     """Adds differences between `x_val` and `y_val` to `diffs`."""
 
-    # Compare the sharing structure of x_val and y_val.
+    # Compare the sharing structure of x_val and y_val for x_val and y_val not
+    # immutable literal simple types.
     shared_x_path = x_memo.get(id(x_val))
     shared_y_path = y_memo.get(id(y_val))
     if shared_x_path is not None and shared_x_path == shared_y_path:
       return  # We have already compared x_val with y_val.
 
     if shared_x_path is None:
       x_memo[id(x_val)] = path
     else:
-      path_str = daglish.path_str(path)
-      x_path = daglish.path_str(shared_x_path)
-      diffs.append(f'* Sharing diff: x{path_str} is x{x_path} but '
-                   f'y{path_str} is not y{x_path}')
+      if not daglish.is_internable(x_val):
+        path_str = daglish.path_str(path)
+        x_path = daglish.path_str(shared_x_path)
+        diffs.append(
+            f'* Sharing diff: x{path_str} is x{x_path} but '
+            f'y{path_str} is not y{x_path}'
+        )
 
     if shared_y_path is None:
       y_memo[id(y_val)] = path
     else:
-      path_str = daglish.path_str(path)
-      y_path = daglish.path_str(shared_y_path)
-      diffs.append(f'* Sharing diff: y{path_str} is y{y_path} but '
-                   f'x{path_str} is not x{y_path}')
+      if not daglish.is_internable(y_val):
+        path_str = daglish.path_str(path)
+        y_path = daglish.path_str(shared_y_path)
+        diffs.append(
+            f'* Sharing diff: y{path_str} is y{y_path} but '
+            f'x{path_str} is not x{y_path}'
+        )
 
     # Compare x_val and y_val by type.
     if type(x_val) is not type(y_val):
       path_str = daglish.path_str(path)
       diffs.append(f'* type(x{path_str}) != type(y{path_str}): '
                    f'{type(x_val)} vs {type(y_val)}')
       return  # Don't report any futher differences between x_val and y_val.
```

### Comparing `fiddle-0.2.6/fiddle/_src/testing/test_util_test.py` & `fiddle-0.2.7/fiddle/_src/testing/test_util_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,23 @@
     self.assertEqual(
         test_util.describe_dag_diffs(a, b),
         ['* Sharing diff: x[1] is x[0] but y[1] is not y[0]'])
     self.assertEqual(
         test_util.describe_dag_diffs(b, a),
         ['* Sharing diff: y[1] is y[0] but x[1] is not x[0]'])
 
+  def test_no_sharing_diff_for_internable_value(self):
+    shared_tuple = tuple(range(20))  # To make sure it's not actually interned.
+    a = [shared_tuple, shared_tuple]
+    b = [shared_tuple, tuple(range(20))]
+    self.assertIsNot(b[0], b[1])
+    self.assertEqual(
+        test_util.get_shared_paths(a), test_util.get_shared_paths(b)
+    )
+
   def test_leaf_diff(self):
     x = fdl.Config(sample_fn, a=5)
     y = fdl.Config(sample_fn, a=6)
     self.assertEqual(test_util.describe_dag_diffs(x, y), ['* x.a=5 but y.a=6'])
 
   def test_big_leaf_diff(self):
     x = fdl.Config(sample_fn, a='x' * 40)
@@ -255,14 +264,22 @@
     # There is no NodeTraverser registered for SampleClass, so we don't
     # recurse inside it when looking for shared objects.
     shared_list = [1]
     x = SampleClass(a=shared_list, b=shared_list)
     y = SampleClass(a=shared_list, b=copy.copy(shared_list))
     self.assertEmpty(test_util.describe_dag_diffs(x, y))
 
+  def test_adding_and_removing_tags_is_equivalent(self):
+    config = fdl.Config(SampleClass)
+    fdl.add_tag(config, 'a', SampleTag)
+    fdl.remove_tag(config, 'a', SampleTag)
+    self.assertEmpty(
+        test_util.describe_dag_diffs(config, fdl.Config(SampleClass))
+    )
+
 
 class TestCaseTest(testing.TestCase):
 
   def test_dag_equal(self):
     x = make_test_value()
     y = make_test_value()
     self.assertDagEqual(x, y)
```

### Comparing `fiddle-0.2.6/fiddle/absl_flags/__init__.py` & `fiddle-0.2.7/fiddle/absl_flags/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 # limitations under the License.
 
 """The public API for the absl_flags Fiddle extension."""
 
 from fiddle._src.absl_flags.flags import apply_fiddlers_to
 from fiddle._src.absl_flags.flags import apply_overrides_to
 from fiddle._src.absl_flags.flags import create_buildable_from_flags
+from fiddle._src.absl_flags.flags import fdl_flags_supplied
 from fiddle._src.absl_flags.flags import flags_parser
```

### Comparing `fiddle-0.2.6/fiddle/absl_flags/example/__init__.py` & `fiddle-0.2.7/fiddle/absl_flags/example/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/absl_flags/example/business_logic.py` & `fiddle-0.2.7/fiddle/absl_flags/example/business_logic.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/absl_flags/example/configs.py` & `fiddle-0.2.7/fiddle/absl_flags/example/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A collection of Fiddle-based configurations and fiddlers.
 
 The Fiddle recommended pattern is to define one or more "base" configurations
-(e.g. `simple` in this example). As new experiments are performed, they simply
+(e.g. `base` in this example). As new experiments are performed, they simply
 mutate the base configuration or another experiment. (Fiddle's history tracking
 lets you easily determine which experiment set what value when there's a large
 stack of incremental experiments.)
 
 > Note: This pattern often works well for iterative product launches and/or
 > product versions as well.
```

### Comparing `fiddle-0.2.6/fiddle/absl_flags/example/example.py` & `fiddle-0.2.7/fiddle/absl_flags/example/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 r"""An example demonstrating Fiddle and absl_flags.
 
 Run this example with the following command:
 
 ```sh
 python3 -m fiddle.absl_flags.example.example \
-  --fdl_config=simple \
+  --fdl_config=base \
   --fiddler=swap_weight_and_bias \
   --fdl.model.b=0.73 \
   --fdl.data.filename='"other.txt"'  # Alt syntax: --fdl.data.filename=\"b.txt\"
 ```
 """
 
 from typing import Sequence
```

### Comparing `fiddle-0.2.6/fiddle/absl_flags/example/tags.py` & `fiddle-0.2.7/fiddle/absl_flags/example/tags.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/arg_factory.py` & `fiddle-0.2.7/fiddle/arg_factory.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/building.py` & `fiddle-0.2.7/fiddle/building.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/codegen/__init__.py` & `fiddle-0.2.7/fiddle/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/codegen/auto_config/__init__.py` & `fiddle-0.2.7/fiddle/codegen/auto_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/codegen/auto_config/experimental_top_level_api.py` & `fiddle-0.2.7/fiddle/extensions/jax.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Experimental high-level API for auto_config codegen.
+"""Fiddle extensions to handle JAX code more elegantly.
 
-Do NOT depend on these interfaces for non-experimental code.
+Currently this just affects codegen, graphviz, and other debugging functions.
 """
 
 # pylint: disable=unused-import
-from fiddle._src.codegen.auto_config.experimental_top_level_api import auto_config_codegen
+from fiddle._src.extensions.jax import enable
```

### Comparing `fiddle-0.2.6/fiddle/codegen/codegen.py` & `fiddle-0.2.7/fiddle/codegen/codegen.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Library for generating code from a Config or Partial object."""
 
 # pylint: disable=unused-import
-from fiddle._src.codegen.codegen import assignment_path
-from fiddle._src.codegen.codegen import codegen_dot_syntax
-from fiddle._src.codegen.codegen import mini_ast
-from fiddle._src.codegen.codegen import SharedBuildableManager
+from fiddle._src.codegen.legacy_codegen import assignment_path
+from fiddle._src.codegen.legacy_codegen import codegen_dot_syntax
+from fiddle._src.codegen.legacy_codegen import mini_ast
+from fiddle._src.codegen.legacy_codegen import SharedBuildableManager
```

### Comparing `fiddle-0.2.6/fiddle/codegen/codegen_diff.py` & `fiddle-0.2.7/fiddle/codegen/codegen_diff.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/codegen/py_val_to_cst_converter.py` & `fiddle-0.2.7/fiddle/codegen/py_val_to_cst_converter.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/config.py` & `fiddle-0.2.7/fiddle/config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/config_test.py` & `fiddle-0.2.7/fiddle/config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/daglish.py` & `fiddle-0.2.7/fiddle/daglish.py`

 * *Files 19% similar despite different names*

```diff
@@ -40,7 +40,10 @@
 from fiddle._src.daglish import path_str
 from fiddle._src.daglish import PathElement
 from fiddle._src.daglish import Paths
 from fiddle._src.daglish import register_node_traverser
 from fiddle._src.daglish import State
 from fiddle._src.daglish import SubTraversalResult
 from fiddle._src.daglish import Traversal
+from fiddle._src.daglish_extensions import is_immutable
+from fiddle._src.daglish_extensions import is_unshareable
+from fiddle._src.daglish_extensions import parse_path
```

### Comparing `fiddle-0.2.6/fiddle/diffing.py` & `fiddle-0.2.7/fiddle/diffing.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/examples/__init__.py` & `fiddle-0.2.7/fiddle/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/examples/colabs/__init__.py` & `fiddle-0.2.7/fiddle/examples/colabs/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/experimental/__init__.py` & `fiddle-0.2.7/fiddle/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/experimental/auto_config.py` & `fiddle-0.2.7/fiddle/experimental/auto_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,7 +27,8 @@
 from fiddle._src.experimental.auto_config import auto_config_policy
 from fiddle._src.experimental.auto_config import auto_unconfig
 from fiddle._src.experimental.auto_config import AutoConfig
 from fiddle._src.experimental.auto_config import exempt
 from fiddle._src.experimental.auto_config import inline
 from fiddle._src.experimental.auto_config import is_auto_config
 from fiddle._src.experimental.auto_config import UnsupportedLanguageConstructError
+from fiddle._src.experimental.with_tags import with_tags
```

### Comparing `fiddle-0.2.6/fiddle/experimental/auto_config_policy.py` & `fiddle-0.2.7/fiddle/experimental/auto_config_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# pyformat: mode=midnight
 """A policy of functions to skip representing as `fdl.Config`'s.
 
 When running `auto_config` on a function, some Python functions cannot or, in
 practice, should never be mapped into `fdl.Config`-space. This file defines
 policies (mostly implemented as lists) that enumerates them.
 
 Because either adding or removing a function from this list can cause config
```

### Comparing `fiddle-0.2.6/fiddle/experimental/autobuilders/__init__.py` & `fiddle-0.2.7/fiddle/experimental/autobuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/experimental/configurator.py` & `fiddle-0.2.7/fiddle/experimental/configurator.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/experimental/dataclasses.py` & `fiddle-0.2.7/fiddle/experimental/dataclasses.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,11 +20,13 @@
 choose) to customize Fiddle's behavior to make great user experiences for the
 library's users. Fiddle leverages extension mechanisms within Python's
 dataclasses system to add some additional metadata to control behavior in the
 rest of Fiddle.
 """
 
 # pylint: disable=unused-import
+from fiddle._src.experimental.dataclasses import convert_dataclasses_to_configs
+from fiddle._src.experimental.dataclasses import daglish_dataclass_registry
 from fiddle._src.experimental.dataclasses import field
 from fiddle._src.experimental.dataclasses import field_has_tag
 from fiddle._src.experimental.dataclasses import FieldMetadata
 from fiddle._src.experimental.dataclasses import TagOrTags
```

### Comparing `fiddle-0.2.6/fiddle/experimental/dict_config.py` & `fiddle-0.2.7/fiddle/experimental/dict_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/experimental/fixture_node.py` & `fiddle-0.2.7/fiddle/experimental/fixture_node.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/experimental/namespace_config.py` & `fiddle-0.2.7/fiddle/experimental/namespace_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/experimental/serialization.py` & `fiddle-0.2.7/fiddle/experimental/serialization.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/experimental/tied_value.py` & `fiddle-0.2.7/fiddle/experimental/tied_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Public API for tied values."""
 
 # pylint: disable=unused-import
 from fiddle._src.experimental.tied_value import get_tied
-from fiddle._src.experimental.tied_value import new
+from fiddle._src.experimental.tied_value import tied_value
 from fiddle._src.experimental.tied_value import TiedValue
 from fiddle._src.experimental.tied_value import untie
```

### Comparing `fiddle-0.2.6/fiddle/experimental/transform.py` & `fiddle-0.2.7/fiddle/experimental/transform.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/experimental/visualize.py` & `fiddle-0.2.7/fiddle/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/experimental/yaml_serialization.py` & `fiddle-0.2.7/fiddle/experimental/yaml_serialization.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/extensions/__init__.py` & `fiddle-0.2.7/fiddle/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/extensions/jax.py` & `fiddle-0.2.7/fiddle/extensions/seqio.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Fiddle extensions to handle JAX code more elegantly.
+"""Fiddle extensions to handle SeqIO code more elegantly.
+
+(See https://github.com/google/seqio.)
 
 Currently this just affects codegen, graphviz, and other debugging functions.
 """
 
 # pylint: disable=unused-import
-from fiddle._src.extensions.jax import enable
+from fiddle._src.extensions.seqio import enable
```

### Comparing `fiddle-0.2.6/fiddle/extensions/seqio.py` & `fiddle-0.2.7/fiddle/printing.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,16 +9,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Fiddle extensions to handle SeqIO code more elegantly.
-
-(See https://github.com/google/seqio.)
-
-Currently this just affects codegen, graphviz, and other debugging functions.
-"""
+"""Functions to output representations of `fdl.Buildable`s."""
 
 # pylint: disable=unused-import
-from fiddle._src.extensions.seqio import enable
+from fiddle._src.printing import as_str_flattened
+from fiddle._src.printing import history_per_leaf_parameter
```

### Comparing `fiddle-0.2.6/fiddle/extensions/tf.py` & `fiddle-0.2.7/fiddle/extensions/tf.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/graphviz.py` & `fiddle-0.2.7/fiddle/graphviz.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Provides a renderer to visualize a DAG of `fdl.Buildable`s via Graphviz."""
 
 # pylint: disable=unused-import
 
-from fiddle._src.graphviz import CustomGraphvizBuildable
-from fiddle._src.graphviz import GraphvizRendererApi
 from fiddle._src.graphviz import render
 from fiddle._src.graphviz import render_diff
+from fiddle._src.graphviz_custom_object import CustomGraphvizBuildable
+from fiddle._src.graphviz_custom_object import GraphvizRendererApi
```

### Comparing `fiddle-0.2.6/fiddle/history.py` & `fiddle-0.2.7/fiddle/history.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 from fiddle._src.history import ChangeKind
 from fiddle._src.history import custom_location
 from fiddle._src.history import DELETED
 from fiddle._src.history import History
 from fiddle._src.history import HistoryEntry
 from fiddle._src.history import Location
 from fiddle._src.history import LocationProvider
+from fiddle._src.history import set_tracking
 from fiddle._src.history import suspend_tracking
 from fiddle._src.history import tracking_enabled
```

### Comparing `fiddle-0.2.6/fiddle/printing.py` & `fiddle-0.2.7/fiddle/selectors.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,12 +9,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Functions to output representations of `fdl.Buildable`s."""
+"""Library for manipulating selections of a Buildable DAG.
+
+A common need for configuration libraries is to override settings in some kind
+of base configuration, and these APIs allow such overrides to take place
+imperatively.
+"""
 
 # pylint: disable=unused-import
-from fiddle._src.printing import as_str_flattened
-from fiddle._src.printing import history_per_leaf_parameter
+from fiddle._src.selectors import NodeSelection
+from fiddle._src.selectors import select
+from fiddle._src.selectors import Selection
+from fiddle._src.selectors import TagSelection
```

### Comparing `fiddle-0.2.6/fiddle/selectors.py` & `fiddle-0.2.7/fiddle/signatures.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,19 +9,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Library for manipulating selections of a Buildable DAG.
-
-A common need for configuration libraries is to override settings in some kind
-of base configuration, and these APIs allow such overrides to take place
-imperatively.
-"""
+"""Functions to facilitate getting (and caching) signatures and type hints."""
 
 # pylint: disable=unused-import
-from fiddle._src.selectors import NodeSelection
-from fiddle._src.selectors import select
-from fiddle._src.selectors import Selection
-from fiddle._src.selectors import TagSelection
+from fiddle._src.signatures import get_signature
+from fiddle._src.signatures import get_type_hints
+from fiddle._src.signatures import has_signature
```

### Comparing `fiddle-0.2.6/fiddle/signatures.py` & `fiddle-0.2.7/fiddle/testing/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,13 +9,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Functions to facilitate getting (and caching) signatures and type hints."""
+"""Fiddle testing utilities."""
 
-# pylint: disable=unused-import
-from fiddle._src.signatures import get_signature
-from fiddle._src.signatures import get_type_hints
-from fiddle._src.signatures import has_signature
+from fiddle._src.testing.test_util import parse_path
+from fiddle._src.testing.test_util import parse_reference
+from fiddle._src.testing.test_util import TestCase
```

### Comparing `fiddle-0.2.6/fiddle/tag_type.py` & `fiddle-0.2.7/fiddle/tag_type.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/tagging.py` & `fiddle-0.2.7/fiddle/tagging.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/testing/__init__.py` & `fiddle-0.2.7/fiddle/version.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,12 +9,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Fiddle testing utilities."""
-
-from fiddle._src.testing.test_util import parse_path
-from fiddle._src.testing.test_util import parse_reference
-from fiddle._src.testing.test_util import TestCase
+"""Current Fiddle version at head on Github."""
+__version__ = "0.2.7"
```

### Comparing `fiddle-0.2.6/fiddle/testing/autotest.py` & `fiddle-0.2.7/fiddle/testing/autotest.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle/testing/test_util.py` & `fiddle-0.2.7/fiddle/testing/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.6/fiddle.egg-info/PKG-INFO` & `fiddle-0.2.7/fiddle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddle
-Version: 0.2.6
+Version: 0.2.7
 Summary: Fiddle: A Python-first configuration library
 Home-page: https://github.com/google/fiddle
 Author: The Fiddle Team
 Author-email: noreply@google.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/google/fiddle/docs
 Project-URL: Bug Reports, https://github.com/google/fiddle/issues
```

### Comparing `fiddle-0.2.6/fiddle.egg-info/SOURCES.txt` & `fiddle-0.2.7/fiddle.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,26 @@
 fiddle.egg-info/dependency_links.txt
 fiddle.egg-info/requires.txt
 fiddle.egg-info/top_level.txt
 fiddle/_src/__init__.py
 fiddle/_src/arg_factory.py
 fiddle/_src/arg_factory_test.py
 fiddle/_src/building.py
+fiddle/_src/building_test.py
 fiddle/_src/config.py
 fiddle/_src/config_test.py
 fiddle/_src/daglish.py
+fiddle/_src/daglish_extensions.py
+fiddle/_src/daglish_extensions_test.py
 fiddle/_src/daglish_test.py
 fiddle/_src/diffing.py
 fiddle/_src/diffing_test.py
 fiddle/_src/field_metadata.py
 fiddle/_src/graphviz.py
+fiddle/_src/graphviz_custom_object.py
 fiddle/_src/history.py
 fiddle/_src/history_test.py
 fiddle/_src/materialize.py
 fiddle/_src/materialize_test.py
 fiddle/_src/module_reflection.py
 fiddle/_src/module_reflection_test.py
 fiddle/_src/module_reflection_test_module.py
@@ -55,34 +59,40 @@
 fiddle/_src/tagging.py
 fiddle/_src/tagging_test.py
 fiddle/_src/tagging_test_module.py
 fiddle/_src/absl_flags/__init__.py
 fiddle/_src/absl_flags/flags.py
 fiddle/_src/absl_flags/sample_module_for_flags_test.py
 fiddle/_src/codegen/__init__.py
-fiddle/_src/codegen/codegen.py
 fiddle/_src/codegen/codegen_diff.py
-fiddle/_src/codegen/codegen_test.py
 fiddle/_src/codegen/formatting_utilities.py
 fiddle/_src/codegen/import_manager.py
 fiddle/_src/codegen/import_manager_test.py
+fiddle/_src/codegen/legacy_codegen.py
+fiddle/_src/codegen/legacy_codegen_test.py
 fiddle/_src/codegen/mini_ast.py
 fiddle/_src/codegen/namespace.py
 fiddle/_src/codegen/namespace_test.py
+fiddle/_src/codegen/new_codegen.py
+fiddle/_src/codegen/new_codegen_test.py
+fiddle/_src/codegen/newcg_symbolic_references.py
+fiddle/_src/codegen/newcg_symbolic_references_test.py
 fiddle/_src/codegen/py_val_to_cst_converter.py
 fiddle/_src/codegen/py_val_to_cst_converter_test.py
 fiddle/_src/codegen/special_value_codegen.py
 fiddle/_src/codegen/test_util.py
 fiddle/_src/codegen/auto_config/__init__.py
 fiddle/_src/codegen/auto_config/code_ir.py
 fiddle/_src/codegen/auto_config/code_ir_test.py
 fiddle/_src/codegen/auto_config/complex_to_variables.py
 fiddle/_src/codegen/auto_config/complex_to_variables_test.py
 fiddle/_src/codegen/auto_config/experimental_top_level_api.py
 fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py
+fiddle/_src/codegen/auto_config/get_history_comments.py
+fiddle/_src/codegen/auto_config/get_history_comments_test.py
 fiddle/_src/codegen/auto_config/init_task.py
 fiddle/_src/codegen/auto_config/init_task_test.py
 fiddle/_src/codegen/auto_config/ir_printer.py
 fiddle/_src/codegen/auto_config/ir_printer_test.py
 fiddle/_src/codegen/auto_config/ir_to_cst.py
 fiddle/_src/codegen/auto_config/ir_to_cst_test.py
 fiddle/_src/codegen/auto_config/make_symbolic_references.py
@@ -91,14 +101,16 @@
 fiddle/_src/codegen/auto_config/naming_test.py
 fiddle/_src/codegen/auto_config/parents_first_traversal.py
 fiddle/_src/codegen/auto_config/parents_first_traversal_test.py
 fiddle/_src/codegen/auto_config/shared_to_variables.py
 fiddle/_src/codegen/auto_config/shared_to_variables_test.py
 fiddle/_src/codegen/auto_config/split_arg_factories.py
 fiddle/_src/codegen/auto_config/split_arg_factories_test.py
+fiddle/_src/codegen/auto_config/sub_fixture.py
+fiddle/_src/codegen/auto_config/sub_fixture_test.py
 fiddle/_src/codegen/auto_config/test_fixtures.py
 fiddle/_src/codegen/test_submodule/__init__.py
 fiddle/_src/codegen/test_submodule/test_util.py
 fiddle/_src/experimental/__init__.py
 fiddle/_src/experimental/auto_config.py
 fiddle/_src/experimental/auto_config_policy.py
 fiddle/_src/experimental/auto_config_test.py
@@ -115,14 +127,16 @@
 fiddle/_src/experimental/namespace_config_test.py
 fiddle/_src/experimental/serialization.py
 fiddle/_src/experimental/tied_value.py
 fiddle/_src/experimental/tied_value_test.py
 fiddle/_src/experimental/transform.py
 fiddle/_src/experimental/transform_test.py
 fiddle/_src/experimental/visualize.py
+fiddle/_src/experimental/with_tags.py
+fiddle/_src/experimental/with_tags_test.py
 fiddle/_src/experimental/yaml_serialization.py
 fiddle/_src/experimental/yaml_serialization_test.py
 fiddle/_src/experimental/autobuilders/__init__.py
 fiddle/_src/experimental/autobuilders/autobuilders.py
 fiddle/_src/experimental/autobuilders/autobuilders_test.py
 fiddle/_src/experimental/autobuilders/autobuilders_test_util.py
 fiddle/_src/extensions/__init__.py
```

### Comparing `fiddle-0.2.6/setup.py` & `fiddle-0.2.7/setup.py`

 * *Files identical despite different names*

