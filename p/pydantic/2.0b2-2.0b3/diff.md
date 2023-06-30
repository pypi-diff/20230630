# Comparing `tmp/pydantic-2.0b2.tar.gz` & `tmp/pydantic-2.0b3.tar.gz`

## Comparing `pydantic-2.0b2.tar` & `pydantic-2.0b3.tar`

### file list

```diff
@@ -1,202 +1,208 @@
--rw-r--r--   0        0        0    79910 2020-02-02 00:00:00.000000 pydantic-2.0b2/HISTORY.md
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 pydantic-2.0b2/Makefile
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 pydantic-2.0b2/README.md
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/__init__.py
--rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_migration.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/alias_generators.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/class_validators.py
--rw-r--r--   0        0        0    21146 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/color.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/config.py
--rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/dataclasses.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/datetime_parse.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/decorator.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/env_settings.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/error_wrappers.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/errors.py
--rw-r--r--   0        0        0    37298 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/fields.py
--rw-r--r--   0        0        0     8882 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/functional_serializers.py
--rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/functional_validators.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/generics.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/json.py
--rw-r--r--   0        0        0    70692 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/json_schema.py
--rw-r--r--   0        0        0    54924 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/main.py
--rw-r--r--   0        0        0    38603 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/mypy.py
--rw-r--r--   0        0        0    10944 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/networks.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/py.typed
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/schema.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/tools.py
--rw-r--r--   0        0        0    15617 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/type_adapter.py
--rw-r--r--   0        0        0    37702 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/types.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/typing.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/utils.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/validate_call.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/validators.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/__init__.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_annotated_handlers.py
--rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_config.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_core_metadata.py
--rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_core_utils.py
--rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_dataclasses.py
--rw-r--r--   0        0        0    24182 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_decorators.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_decorators_v1.py
--rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_discriminated_union.py
--rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_fields.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_forward_ref.py
--rw-r--r--   0        0        0    65337 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_generate_schema.py
--rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_generics.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_internal_dataclass.py
--rw-r--r--   0        0        0     8225 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_known_annotated_metadata.py
--rw-r--r--   0        0        0    23972 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_model_construction.py
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_repr.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_schema_generation_shared.py
--rw-r--r--   0        0        0    37641 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_std_types_schema.py
--rw-r--r--   0        0        0    16535 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_typing_extra.py
--rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_utils.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_validate_call.py
--rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/__init__.py
--rw-r--r--   0        0        0     9379 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/class_validators.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/config.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/copy_internals.py
--rw-r--r--   0        0        0    10595 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/decorator.py
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/json.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/parse.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/tools.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/__init__.py
--rw-r--r--   0        0        0    14586 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/_hypothesis_plugin.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/annotated_types.py
--rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/class_validators.py
--rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/color.py
--rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/config.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/dataclasses.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/datetime_parse.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/decorator.py
--rw-r--r--   0        0        0    13893 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/env_settings.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/error_wrappers.py
--rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/errors.py
--rw-r--r--   0        0        0    50418 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/fields.py
--rw-r--r--   0        0        0    17424 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/generics.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/json.py
--rw-r--r--   0        0        0    44378 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/main.py
--rw-r--r--   0        0        0    38097 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/mypy.py
--rw-r--r--   0        0        0    21826 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/networks.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/py.typed
--rw-r--r--   0        0        0    47615 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/schema.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/tools.py
--rw-r--r--   0        0        0    35219 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/types.py
--rw-r--r--   0        0        0    19358 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/typing.py
--rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/utils.py
--rw-r--r--   0        0        0    21874 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/validators.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/__init__.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/conftest.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_abc.py
--rw-r--r--   0        0        0    14786 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_aliases.py
--rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_annotated.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_assert_in_validators.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_callable.py
--rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_color.py
--rw-r--r--   0        0        0    16774 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_computed_fields.py
--rw-r--r--   0        0        0    21049 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_config.py
--rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_construction.py
--rw-r--r--   0        0        0    15857 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_create_model.py
--rw-r--r--   0        0        0    63792 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_dataclasses.py
--rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_datetime.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_decorators.py
--rw-r--r--   0        0        0    20818 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_deprecated.py
--rw-r--r--   0        0        0    12182 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_deprecated_validate_arguments.py
--rw-r--r--   0        0        0    40531 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_discriminated_union.py
--rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_docs.py
--rw-r--r--   0        0        0    76384 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_edge_cases.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_errors.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_exports.py
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_fastapi.sh
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_fastapi_json_schema.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_fields.py
--rw-r--r--   0        0        0    26896 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_forward_ref.py
--rw-r--r--   0        0        0    71997 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_generics.py
--rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_internal.py
--rw-r--r--   0        0        0    13165 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_json.py
--rw-r--r--   0        0        0   140193 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_json_schema.py
--rw-r--r--   0        0        0    68360 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_main.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_migration.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_model_signature.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_model_validator.py
--rw-r--r--   0        0        0    29249 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_networks.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_networks_ipaddress.py
--rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_parse.py
--rw-r--r--   0        0        0     8039 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_prepare_annotations.py
--rw-r--r--   0        0        0     8610 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_private_attributes.py
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_pydantic_settings.sh
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_rich_repr.py
--rw-r--r--   0        0        0    10497 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_root_model.py
--rw-r--r--   0        0        0    29452 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_serialize.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_strict.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_structural_pattern_matching.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_tools.py
--rw-r--r--   0        0        0     8494 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_type_adapter.py
--rw-r--r--   0        0        0    10667 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_type_alias_type.py
--rw-r--r--   0        0        0   178255 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_types.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_types_namedtuple.py
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_types_payment_card_number.py
--rw-r--r--   0        0        0    25240 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_types_typeddict.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_typing.py
--rw-r--r--   0        0        0    21503 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_utils.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_v1.py
--rw-r--r--   0        0        0    19653 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_validate_call.py
--rw-r--r--   0        0        0    72997 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_validators.py
--rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_validators_dataclass.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/__init__.py
--rw-r--r--   0        0        0    10878 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/test_mypy.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/mypy-default.ini
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/mypy-plugin-strict-no-any.ini
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/mypy-plugin-strict.ini
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/mypy-plugin.ini
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/pyproject-default.toml
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/pyproject-plugin-bad-param.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/pyproject-plugin-strict.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/pyproject-plugin.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/computed_fields.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/custom_constructor.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/dataclass_no_any.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/fail1.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/fail2.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/fail3.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/fail4.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/fail_defaults.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/plugin_default_factory.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/plugin_fail.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/plugin_success.py
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     7416 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/success.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/computed_fields.txt
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/custom_constructor.txt
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/fail1.txt
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/fail2.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/fail3.txt
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/fail4.txt
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/fail_defaults.txt
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail-strict.txt
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin-success-strict-baseConfig.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin-success-strict.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin_default_factory.txt
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin_success.txt
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin_success_baseConfig.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/v1.0.1/fail1.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/v1.0.1/fail2.txt
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/v1.0.1/plugin_success.txt
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/v1.0.1/plugin_success_baseConfig.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/pyright/pyproject.toml
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/pyright/pyright_example.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pydantic-2.0b2/.gitignore
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.0b2/LICENSE
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 pydantic-2.0b2/pyproject.toml
--rw-r--r--   0        0        0   115211 2020-02-02 00:00:00.000000 pydantic-2.0b2/PKG-INFO
+-rw-r--r--   0        0        0    80833 2020-02-02 00:00:00.000000 pydantic-2.0b3/HISTORY.md
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 pydantic-2.0b3/Makefile
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 pydantic-2.0b3/README.md
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/__init__.py
+-rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_migration.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/alias_generators.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/class_validators.py
+-rw-r--r--   0        0        0    21393 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/color.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/config.py
+-rw-r--r--   0        0        0    10962 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/dataclasses.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/datetime_parse.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/decorator.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/env_settings.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/error_wrappers.py
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/errors.py
+-rw-r--r--   0        0        0    36931 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/fields.py
+-rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/functional_serializers.py
+-rw-r--r--   0        0        0    18035 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/functional_validators.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/generics.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/json.py
+-rw-r--r--   0        0        0    77382 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/json_schema.py
+-rw-r--r--   0        0        0    52973 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/main.py
+-rw-r--r--   0        0        0    38471 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/mypy.py
+-rw-r--r--   0        0        0    13385 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/networks.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/py.typed
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/root_model.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/schema.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/tools.py
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/type_adapter.py
+-rw-r--r--   0        0        0    43122 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/types.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/typing.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/utils.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/validate_call.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/validators.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_annotated_handlers.py
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_config.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_core_metadata.py
+-rw-r--r--   0        0        0    23968 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_core_utils.py
+-rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_dataclasses.py
+-rw-r--r--   0        0        0    28054 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_decorators.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_decorators_v1.py
+-rw-r--r--   0        0        0    23146 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_discriminated_union.py
+-rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_fields.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_forward_ref.py
+-rw-r--r--   0        0        0    73188 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_generate_schema.py
+-rw-r--r--   0        0        0    20979 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_generics.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_internal_dataclass.py
+-rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_known_annotated_metadata.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_mock_validator.py
+-rw-r--r--   0        0        0    24454 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_model_construction.py
+-rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_repr.py
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_schema_generation_shared.py
+-rw-r--r--   0        0        0    37093 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_std_types_schema.py
+-rw-r--r--   0        0        0    16212 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_typing_extra.py
+-rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_utils.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_validate_call.py
+-rw-r--r--   0        0        0     9942 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/_internal/_validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/deprecated/__init__.py
+-rw-r--r--   0        0        0     9631 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/deprecated/class_validators.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/deprecated/config.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/deprecated/copy_internals.py
+-rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/deprecated/decorator.py
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/deprecated/json.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/deprecated/parse.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/deprecated/tools.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/__init__.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/_hypothesis_plugin.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/annotated_types.py
+-rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/class_validators.py
+-rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/color.py
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/config.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/dataclasses.py
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/datetime_parse.py
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/decorator.py
+-rw-r--r--   0        0        0    13893 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/env_settings.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/error_wrappers.py
+-rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/errors.py
+-rw-r--r--   0        0        0    50418 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/fields.py
+-rw-r--r--   0        0        0    17424 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/generics.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/json.py
+-rw-r--r--   0        0        0    44378 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/main.py
+-rw-r--r--   0        0        0    38641 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/mypy.py
+-rw-r--r--   0        0        0    21826 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/networks.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/py.typed
+-rw-r--r--   0        0        0    47615 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/schema.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/tools.py
+-rw-r--r--   0        0        0    35380 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/types.py
+-rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/typing.py
+-rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/utils.py
+-rw-r--r--   0        0        0    21874 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/validators.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pydantic-2.0b3/pydantic/v1/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/__init__.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/conftest.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_abc.py
+-rw-r--r--   0        0        0    16305 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_aliases.py
+-rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_annotated.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_assert_in_validators.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_callable.py
+-rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_color.py
+-rw-r--r--   0        0        0    18991 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_computed_fields.py
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_config.py
+-rw-r--r--   0        0        0    13697 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_construction.py
+-rw-r--r--   0        0        0    15684 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_create_model.py
+-rw-r--r--   0        0        0    64815 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_dataclasses.py
+-rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_datetime.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_decorators.py
+-rw-r--r--   0        0        0    21307 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_deprecated.py
+-rw-r--r--   0        0        0    12182 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_deprecated_validate_arguments.py
+-rw-r--r--   0        0        0    42743 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_discriminated_union.py
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_docs.py
+-rw-r--r--   0        0        0    76384 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_edge_cases.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_errors.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_exports.py
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_fastapi.sh
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_fastapi_json_schema.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_fields.py
+-rw-r--r--   0        0        0    27967 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_forward_ref.py
+-rw-r--r--   0        0        0    71551 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_generics.py
+-rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_internal.py
+-rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_json.py
+-rw-r--r--   0        0        0   148663 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_json_schema.py
+-rw-r--r--   0        0        0    74048 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_main.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_migration.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_model_signature.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_model_validator.py
+-rw-r--r--   0        0        0    29484 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_networks.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_networks_ipaddress.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_parse.py
+-rw-r--r--   0        0        0     8039 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_prepare_annotations.py
+-rw-r--r--   0        0        0     8901 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_private_attributes.py
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_pydantic_settings.sh
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_rich_repr.py
+-rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_root_model.py
+-rw-r--r--   0        0        0    27615 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_serialize.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_strict.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_structural_pattern_matching.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_tools.py
+-rw-r--r--   0        0        0     8494 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_type_adapter.py
+-rw-r--r--   0        0        0    10462 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_type_alias_type.py
+-rw-r--r--   0        0        0   179814 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_types.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_types_namedtuple.py
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_types_payment_card_number.py
+-rw-r--r--   0        0        0    26066 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_types_typeddict.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_typing.py
+-rw-r--r--   0        0        0    21561 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_utils.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_v1.py
+-rw-r--r--   0        0        0    19653 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_validate_call.py
+-rw-r--r--   0        0        0    73667 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_validators.py
+-rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_validators_dataclass.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/__init__.py
+-rw-r--r--   0        0        0    11044 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/test_mypy.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/configs/mypy-default.ini
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/configs/mypy-plugin-strict-no-any.ini
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/configs/mypy-plugin-strict.ini
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/configs/mypy-plugin-very-strict.ini
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/configs/mypy-plugin.ini
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/configs/pyproject-default.toml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/configs/pyproject-plugin-bad-param.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/configs/pyproject-plugin-strict.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/configs/pyproject-plugin.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/computed_fields.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/custom_constructor.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/dataclass_no_any.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/fail1.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/fail2.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/fail3.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/fail4.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/fail_defaults.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/metaclass_args.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/plugin_default_factory.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/plugin_fail.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/plugin_success.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     7416 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/modules/success.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/computed_fields.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/custom_constructor.txt
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/fail1.txt
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/fail2.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/fail3.txt
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/fail4.txt
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/fail_defaults.txt
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/metaclass_args_no_plugin.txt
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/metaclass_args_plugin.txt
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/plugin-fail-strict.txt
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/plugin-fail.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/plugin-success-strict-baseConfig.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/plugin-success-strict.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/plugin_default_factory.txt
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/plugin_success.txt
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/latest/plugin_success_baseConfig.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/v1.0.1/fail1.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/v1.0.1/fail2.txt
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/v1.0.1/plugin_success.txt
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/mypy/outputs/v1.0.1/plugin_success_baseConfig.txt
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/pyright/pyproject.toml
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.0b3/tests/pyright/pyright_example.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pydantic-2.0b3/.gitignore
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.0b3/LICENSE
+-rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 pydantic-2.0b3/pyproject.toml
+-rw-r--r--   0        0        0   116843 2020-02-02 00:00:00.000000 pydantic-2.0b3/PKG-INFO
```

### Comparing `pydantic-2.0b2/HISTORY.md` & `pydantic-2.0b3/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v2.0b3 (2023-06-16)
+
+Third beta pre-release of Pydantic V2
+
+See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0b3)
+
 ## v2.0b2 (2023-06-03)
 
 Add `from_attributes` runtime flag to `TypeAdapter.validate_python` and `BaseModel.model_validate`.
 
 See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0b2)
 
 ## v2.0b1 (2023-06-01)
@@ -30,14 +36,28 @@
 
 ## v2.0a1 (2023-04-03)
 
 First pre-release of Pydantic V2!
 
 See [this post](https://docs.pydantic.dev/blog/pydantic-v2-alpha/) for more details.
 
+## v1.10.9 (2023-06-07)
+
+* Fix trailing zeros not ignored in Decimal validation, #5968 by @hramezani
+* Fix mypy plugin for v1.4.0, #5928 by @cdce8p
+* Add future and past date hypothesis strategies, #5850 by @bschoenmaeckers
+* Discourage usage of Cython 3 with Pydantic 1.x, #5845 by @lig
+
+## v1.10.8 (2023-05-23)
+
+* Fix a bug in `Literal` usage with `typing-extension==4.6.0`, #5826 by @hramezani
+* This solves the (closed) issue #3849 where aliased fields that use discriminated union fail to validate when the data contains the non-aliased field name, #5736 by @benwah
+* Update email-validator dependency to >=2.0.0post2, #5627 by @adriangb
+* update `AnyClassMethod` for changes in [python/typeshed#9771](https://github.com/python/typeshed/issues/9771), #5505 by @ITProKyle
+
 ## v1.10.7 (2023-03-22)
 
 * Fix creating schema from model using `ConstrainedStr` with `regex` as dict key, #5223 by @matejetz
 * Address bug in mypy plugin caused by explicit_package_bases=True, #5191 by @dmontagu
 * Add implicit defaults in the mypy plugin for Field with no default argument, #5190 by @dmontagu
 * Fix schema generated for Enum values used as Literals in discriminated unions, #5188 by @javibookline
 * Fix mypy failures caused by the pydantic mypy plugin when users define `from_orm` in their own classes, #5187 by @dmontagu
@@ -311,15 +331,15 @@
 * Fix mypy plugin issue with self field declaration, #2743 by @uriyyo
 * The colon at the end of the line "The fields which were supplied when user was initialised:" suggests that the code following it is related.
   Changed it to a period, #2733 by @krisaoe
 * Renamed variable `schema` to `schema_` to avoid shadowing of global variable name, #2724 by @shahriyarr
 * Add support for autocomplete in VS Code via `__dataclass_transform__`, #2721 by @tiangolo
 * add missing type annotations in `BaseConfig` and handle `max_length = 0`, #2719 by @PrettyWood
 * Change `orm_mode` checking to allow recursive ORM mode parsing with dicts, #2718 by @nuno-andre
-* Add episode 313 of the *Talk Python To Me* podcast, where Michael Kennedy and Samuel Colvin discuss *pydantic*, to the docs, #2712 by @RatulMaharaj
+* Add episode 313 of the *Talk Python To Me* podcast, where Michael Kennedy and Samuel Colvin discuss Pydantic, to the docs, #2712 by @RatulMaharaj
 * fix JSON schema generation when a field is of type `NamedTuple` and has a default value, #2707 by @PrettyWood
 * `Enum` fields now properly support extra kwargs in schema generation, #2697 by @sammchardy
 * **Breaking Change, see #3780**: Make serialization of referenced pydantic models possible, #2650 by @PrettyWood
 * Add `uniqueItems` option to `ConstrainedList`, #2618 by @nuno-andre
 * Try to evaluate forward refs automatically at model creation, #2588 by @uriyyo
 * Switch docs preview and coverage display to use [smokeshow](https://smokeshow.helpmanual.io/), #2580 by @samuelcolvin
 * Add `__version__` attribute to pydantic module, #2572 by @paxcodes
@@ -562,15 +582,15 @@
 * Add private attributes support, #1679 by @Bobronium
 * add `config` to `@validate_arguments`, #1663 by @samuelcolvin
 * Allow descendant Settings models to override env variable names for the fields defined in parent Settings models with
   `env` in their `Config`. Previously only `env_prefix` configuration option was applicable, #1561 by @ojomio
 * Support `ref_template` when creating schema `$ref`s, #1479 by @kilo59
 * Add a `__call__` stub to `PyObject` so that mypy will know that it is callable, #1352 by @brianmaissy
 * `pydantic.dataclasses.dataclass` decorator now supports built-in `dataclasses.dataclass`.
-  It is hence possible to convert an existing `dataclass` easily to add *pydantic* validation.
+  It is hence possible to convert an existing `dataclass` easily to add Pydantic validation.
   Moreover nested dataclasses are also supported, #744 by @PrettyWood
 
 ## v1.6.2 (2021-05-11)
 
 * **Security fix:** Fix `date` and `datetime` parsing so passing either `'infinity'` or `float('inf')`
   (or their negative values) does not cause an infinite loop,
   See security advisory [CVE-2021-29510](https://github.com/pydantic/pydantic/security/advisories/GHSA-5jqp-qgf6-3pvh)
@@ -586,15 +606,15 @@
 * Modify validators for `conlist` and `conset` to not have `always=True`, #1682 by @samuelcolvin
 * add port check to `AnyUrl` (can't exceed 65536) ports are 16 insigned bits: `0 <= port <= 2**16-1` src: [rfc793 header format](https://tools.ietf.org/html/rfc793#section-3.1), #1654 by @flapili
 * Document default `regex` anchoring semantics, #1648 by @yurikhan
 * Use `chain.from_iterable` in class_validators.py. This is a faster and more idiomatic way of using `itertools.chain`.
   Instead of computing all the items in the iterable and storing them in memory, they are computed one-by-one and never
   stored as a huge list. This can save on both runtime and memory space, #1642 by @cool-RR
 * Add `conset()`, analogous to `conlist()`, #1623 by @patrickkwang
-* make *pydantic* errors (un)pickable, #1616 by @PrettyWood
+* make Pydantic errors (un)pickable, #1616 by @PrettyWood
 * Allow custom encoding for `dotenv` files, #1615 by @PrettyWood
 * Ensure `SchemaExtraCallable` is always defined to get type hints on BaseConfig, #1614 by @PrettyWood
 * Update datetime parser to support negative timestamps, #1600 by @mlbiche
 * Update mypy, remove `AnyType` alias for `Type[Any]`, #1598 by @samuelcolvin
 * Adjust handling of root validators so that errors are aggregated from _all_ failing root validators, instead of reporting on only the first root validator to fail, #1586 by @beezee
 * Make `__modify_schema__` on Enums apply to the enum schema rather than fields that use the enum, #1581 by @therefromhere
 * Fix behavior of `__all__` key when used in conjunction with index keys in advanced include/exclude of fields that are sequences, #1579 by @xspirus
@@ -1092,15 +1112,15 @@
 
 ## v0.11.0 (2018-06-28)
 
 * make `list`, `tuple` and `set` types stricter #86
 * **breaking change**: remove msgpack parsing #201
 * add `FilePath` and `DirectoryPath` types #10
 * model schema generation #190
-* JSON serialisation of models and schemas #133
+* JSON serialization of models and schemas #133
 
 ## v0.10.0 (2018-06-11)
 
 * add `Config.allow_population_by_alias` #160, thanks @bendemaree
 * **breaking change**: new errors format #179, thanks @Gr1N
 * **breaking change**: removed `Config.min_number_size` and `Config.max_number_size` #183, thanks @Gr1N
 * **breaking change**: correct behaviour of `lt` and `gt` arguments to `conint` etc. #188
```

### Comparing `pydantic-2.0b2/Makefile` & `pydantic-2.0b3/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 .PHONY: install  ## Install the package, dependencies, and pre-commit for local development
 install: .pdm .pre-commit
 	pdm install --group :all
 	pre-commit install --install-hooks
 
 .PHONY: refresh-lockfiles  ## Sync lockfiles with requirements files.
 refresh-lockfiles: .pdm
-	pdm lock --refresh --dev --group :all
+	pdm update --update-reuse --group :all
 
 .PHONY: rebuild-lockfiles  ## Rebuild lockfiles from scratch, updating all dependencies
 rebuild-lockfiles: .pdm
-	pdm lock --dev --group :all
+	pdm update --update-eager --group :all
 
 .PHONY: format  ## Auto-format python source files
 format: .pdm
 	pdm run black --exclude 'pydantic/v1' $(sources)
 	pdm run ruff --fix $(sources)
 
 .PHONY: lint  ## Lint python source files
```

### Comparing `pydantic-2.0b2/README.md` & `pydantic-2.0b3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 [![CondaForge](https://img.shields.io/conda/v/conda-forge/pydantic.svg)](https://anaconda.org/conda-forge/pydantic)
 [![downloads](https://pepy.tech/badge/pydantic/month)](https://pepy.tech/project/pydantic)
 [![versions](https://img.shields.io/pypi/pyversions/pydantic.svg)](https://github.com/pydantic/pydantic)
 [![license](https://img.shields.io/github/license/pydantic/pydantic.svg)](https://github.com/pydantic/pydantic/blob/main/LICENSE)
 
 Data validation using Python type hints.
 
-Fast and extensible, *pydantic* plays nicely with your linters/IDE/brain.
-Define how data should be in pure, canonical Python 3.7+; validate it with *pydantic*.
+Fast and extensible, Pydantic plays nicely with your linters/IDE/brain.
+Define how data should be in pure, canonical Python 3.7+; validate it with Pydantic.
 
 ## Pydantic Company :rocket:
 
 We've started a company based on the principles that I believe have led to Pydantic's success.
 Learning more from the [Company Announcement](https://pydantic.dev/announcement/).
 
 ## Pydantic V1.10 vs. V2
@@ -29,15 +29,15 @@
 ## Help
 
 See [documentation](https://docs.pydantic.dev/) for more details.
 
 ## Installation
 
 Install using `pip install -U pydantic` or `conda install pydantic -c conda-forge`.
-For more installation options to make *pydantic* even faster,
+For more installation options to make Pydantic even faster,
 see the [Install](https://docs.pydantic.dev/install/) section in the documentation.
 
 ## A Simple Example
 
 ```py
 from datetime import datetime
 from typing import List, Optional
@@ -56,13 +56,13 @@
 print(user.id)
 #> 123
 ```
 
 ## Contributing
 
 For guidance on setting up a development environment and how to make a
-contribution to *pydantic*, see
+contribution to Pydantic, see
 [Contributing to Pydantic](https://docs.pydantic.dev/contributing/).
 
 ## Reporting a Security Vulnerability
 
 See our [security policy](https://github.com/pydantic/pydantic/security/policy).
```

### Comparing `pydantic-2.0b2/pydantic/__init__.py` & `pydantic-2.0b3/pydantic/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing
+
 import pydantic_core
 from pydantic_core.core_schema import (
     FieldSerializationInfo,
     FieldValidationInfo,
     SerializationInfo,
     SerializerFunctionWrapHandler,
     ValidationInfo,
@@ -18,16 +20,26 @@
 from ._migration import getattr_migration
 from .config import ConfigDict, Extra
 from .deprecated.class_validators import root_validator, validator
 from .deprecated.config import BaseConfig  # type: ignore
 from .deprecated.tools import *
 from .errors import *
 from .fields import AliasChoices, AliasPath, Field, PrivateAttr, computed_field
-from .functional_serializers import PlainSerializer, WrapSerializer, field_serializer, model_serializer
-from .functional_validators import field_validator, model_validator
+from .functional_serializers import PlainSerializer, SerializeAsAny, WrapSerializer, field_serializer, model_serializer
+from .functional_validators import (
+    AfterValidator,
+    BeforeValidator,
+    InstanceOf,
+    PlainValidator,
+    SkipValidation,
+    WrapValidator,
+    field_validator,
+    model_validator,
+)
+from .json_schema import WithJsonSchema
 from .main import *
 from .networks import *
 from .type_adapter import TypeAdapter
 from .types import *
 from .validate_call import validate_call
 from .version import VERSION
 
@@ -43,48 +55,53 @@
     'dataclasses',
     # functional validators
     'ValidationInfo',
     'FieldValidationInfo',
     'ValidatorFunctionWrapHandler',
     'field_validator',
     'model_validator',
+    'AfterValidator',
+    'BeforeValidator',
+    'PlainValidator',
+    'WrapValidator',
     # deprecated V1 functional validators
     'root_validator',
     'validator',
     # functional serializers
     'field_serializer',
     'model_serializer',
     'PlainSerializer',
+    'SerializeAsAny',
     'WrapSerializer',
     'FieldSerializationInfo',
     'SerializationInfo',
     'SerializerFunctionWrapHandler',
     # config
     'BaseConfig',
     'ConfigDict',
     'Extra',
     # validate_call
     'validate_call',
     # pydantic_core errors
     'ValidationError',
     # errors
+    'PydanticErrorCodes',
     'PydanticUserError',
     'PydanticSchemaGenerationError',
     'PydanticImportError',
     'PydanticUndefinedAnnotation',
     'PydanticInvalidForJsonSchema',
     # fields
     'AliasPath',
     'AliasChoices',
     'Field',
     'computed_field',
     # main
     'BaseModel',
     'create_model',
-    'RootModel',
     # network
     'AnyUrl',
     'AnyHttpUrl',
     'FileUrl',
     'HttpUrl',
     'UrlConstraints',
     'EmailStr',
@@ -97,14 +114,16 @@
     'AmqpDsn',
     'RedisDsn',
     'MongoDsn',
     'KafkaDsn',
     'MySQLDsn',
     'MariaDBDsn',
     'validate_email',
+    # root_model
+    'RootModel',
     # tools
     'parse_obj_as',
     'schema_of',
     'schema_json_of',
     # types
     'Strict',
     'StrictStr',
@@ -131,15 +150,14 @@
     'UUID3',
     'UUID4',
     'UUID5',
     'FilePath',
     'DirectoryPath',
     'NewPath',
     'Json',
-    'SecretField',
     'SecretStr',
     'SecretBytes',
     'StrictBool',
     'StrictBytes',
     'StrictInt',
     'StrictFloat',
     'PaymentCardNumber',
@@ -166,9 +184,24 @@
     # version
     'VERSION',
     # annotated handlers
     'GetCoreSchemaHandler',
     'GetJsonSchemaHandler',
 ]
 
+# A mapping of {<member name>: <module name>} defining dynamic imports
+_dynamic_imports = {'RootModel': '.root_model'}
+if typing.TYPE_CHECKING:
+    from .root_model import RootModel
+
+_getattr_migration = getattr_migration(__name__)
+
+
+def __getattr__(attr_name: str) -> object:
+    dynamic_attr = _dynamic_imports.get(attr_name)
+    if dynamic_attr is None:
+        return _getattr_migration(attr_name)
+
+    from importlib import import_module
 
-__getattr__ = getattr_migration(__name__)
+    module = import_module(_dynamic_imports[attr_name], package=__package__)
+    return getattr(module, attr_name)
```

### Comparing `pydantic-2.0b2/pydantic/_migration.py` & `pydantic-2.0b3/pydantic/_migration.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/alias_generators.py` & `pydantic-2.0b3/pydantic/alias_generators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-"""Generators for converting between different naming conventions."""
+"""Alias generators for converting between different capitalization conventions."""
 import re
 
 __all__ = ('to_pascal', 'to_camel', 'to_snake')
 
 
 def to_pascal(snake: str) -> str:
     """Convert a snake_case string to PascalCase.
 
     Args:
-        snake: The snake_case string to convert.
+        snake: The string to convert.
 
     Returns:
-        str: The PascalCase string.
+        The PascalCase string.
     """
     camel = snake.title()
     return re.sub('([0-9A-Za-z])_(?=[0-9A-Z])', lambda m: m.group(1), camel)
 
 
 def to_camel(snake: str) -> str:
     """Convert a snake_case string to camelCase.
 
     Args:
-        snake: The snake_case string to convert.
+        snake: The string to convert.
 
     Returns:
-        str: The converted camelCase string.
+        The converted camelCase string.
     """
     camel = to_pascal(snake)
     return re.sub('(^_*[A-Z])', lambda m: m.group(1).lower(), camel)
 
 
 def to_snake(camel: str) -> str:
     """Convert a PascalCase or camelCase string to snake_case.
 
     Args:
         camel: The string to convert.
 
     Returns:
-        str: The converted string in snake_case.
+        The converted string in snake_case.
     """
     snake = re.sub(r'([a-zA-Z])([0-9])', lambda m: f'{m.group(1)}_{m.group(2)}', camel)
     snake = re.sub(r'([a-z0-9])([A-Z])', lambda m: f'{m.group(1)}_{m.group(2)}', snake)
     return snake.lower()
```

### Comparing `pydantic-2.0b2/pydantic/color.py` & `pydantic-2.0b3/pydantic/color.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-"""
-Color definitions are used as per the CSS3
+"""Color definitions are used as per the CSS3
 [CSS Color Module Level 3](http://www.w3.org/TR/css3-color/#svg-color) specification.
 
 A few colors have multiple names referring to the sames colors, eg. `grey` and `gray` or `aqua` and `cyan`.
 
 In these cases the _last_ color when sorted alphabetically takes preferences,
 eg. `Color((0, 255, 255)).as_named() == 'cyan'` because "cyan" comes after "aqua".
+
+Warning: Deprecated
+    The `Color` class is deprecated, use `pydantic_extra_types` instead.
+    See more about it [here](/usage/types/extra_types/color_types/).
 """
 import math
 import re
 from colorsys import hls_to_rgb, rgb_to_hls
 from typing import Any, Callable, Optional, Tuple, Type, Union, cast
 
 from pydantic_core import CoreSchema, PydanticCustomError, core_schema
+from typing_extensions import deprecated
 
 from ._internal import _repr, _utils
 from ._internal._schema_generation_shared import GetJsonSchemaHandler as _GetJsonSchemaHandler
 from .json_schema import JsonSchemaValue
 
 ColorTuple = Union[Tuple[int, int, int], Tuple[int, int, int, float]]
 ColorType = Union[ColorTuple, str]
 HslColorTuple = Union[Tuple[float, float, float], Tuple[float, float, float, float]]
 
 
 class RGBA:
-    """
-    Internal use only as a representation of a color.
-    """
+    """Internal use only as a representation of a color."""
 
     __slots__ = 'r', 'g', 'b', 'alpha', '_tuple'
 
     def __init__(self, r: float, g: float, b: float, alpha: Optional[float]):
         self.r = r
         self.g = g
         self.b = b
@@ -60,18 +62,20 @@
 r_hsl_v4_style = fr'\s*hsla?\(\s*{_r_h}\s+{_r_sl}\s+{_r_sl}(?:\s*/\s*{_r_alpha})?\s*\)\s*'
 
 # colors where the two hex characters are the same, if all colors match this the short version of hex colors can be used
 repeat_colors = {int(c * 2, 16) for c in '0123456789abcdef'}
 rads = 2 * math.pi
 
 
+@deprecated(
+    'The `Color` class is deprecated, use `pydantic_extra_types` instead. '
+    'See https://pydantic-docs.helpmanual.io/usage/types/extra_types/color_types/.'
+)
 class Color(_repr.Representation):
-    """
-    Represents a color.
-    """
+    """Represents a color."""
 
     __slots__ = '_original', '_rgba'
 
     def __init__(self, value: ColorType) -> None:
         self._rgba: RGBA
         self._original: ColorType
         if isinstance(value, (tuple, list)):
@@ -94,22 +98,19 @@
         cls, core_schema: core_schema.CoreSchema, handler: _GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         field_schema = {}
         field_schema.update(type='string', format='color')
         return field_schema
 
     def original(self) -> ColorType:
-        """
-        Original value passed to `Color`.
-        """
+        """Original value passed to `Color`."""
         return self._original
 
     def as_named(self, *, fallback: bool = False) -> str:
-        """
-        Returns the name of the color if it can be found in `COLORS_BY_VALUE` dictionary,
+        """Returns the name of the color if it can be found in `COLORS_BY_VALUE` dictionary,
         otherwise returns the hexadecimal representation of the color or raises `ValueError`.
 
         Args:
             fallback: If True, falls back to returning the hexadecimal representation of
                 the color instead of raising a ValueError when no named color is found.
 
         Returns:
@@ -145,28 +146,25 @@
 
         as_hex = ''.join(f'{v:02x}' for v in values)
         if all(c in repeat_colors for c in values):
             as_hex = ''.join(as_hex[c] for c in range(0, len(as_hex), 2))
         return '#' + as_hex
 
     def as_rgb(self) -> str:
-        """
-        Color as an `rgb(<r>, <g>, <b>)` or `rgba(<r>, <g>, <b>, <a>)` string.
-        """
+        """Color as an `rgb(<r>, <g>, <b>)` or `rgba(<r>, <g>, <b>, <a>)` string."""
         if self._rgba.alpha is None:
             return f'rgb({float_to_255(self._rgba.r)}, {float_to_255(self._rgba.g)}, {float_to_255(self._rgba.b)})'
         else:
             return (
                 f'rgba({float_to_255(self._rgba.r)}, {float_to_255(self._rgba.g)}, {float_to_255(self._rgba.b)}, '
                 f'{round(self._alpha_float(), 2)})'
             )
 
     def as_rgb_tuple(self, *, alpha: Optional[bool] = None) -> ColorTuple:
-        """
-        Returns the color as an RGB or RGBA tuple.
+        """Returns the color as an RGB or RGBA tuple.
 
         Args:
             alpha: Whether to include the alpha channel. There are three options for this input:
 
                 - `None` (default): Include alpha only if it's set. (e.g. not `None`)
                 - `True`: Always include alpha.
                 - `False`: Always omit alpha.
@@ -184,27 +182,24 @@
         elif alpha:
             return r, g, b, self._alpha_float()
         else:
             # alpha is False
             return r, g, b
 
     def as_hsl(self) -> str:
-        """
-        Color as an `hsl(<h>, <s>, <l>)` or `hsl(<h>, <s>, <l>, <a>)` string.
-        """
+        """Color as an `hsl(<h>, <s>, <l>)` or `hsl(<h>, <s>, <l>, <a>)` string."""
         if self._rgba.alpha is None:
             h, s, li = self.as_hsl_tuple(alpha=False)  # type: ignore
             return f'hsl({h * 360:0.0f}, {s:0.0%}, {li:0.0%})'
         else:
             h, s, li, a = self.as_hsl_tuple(alpha=True)  # type: ignore
             return f'hsl({h * 360:0.0f}, {s:0.0%}, {li:0.0%}, {round(a, 2)})'
 
     def as_hsl_tuple(self, *, alpha: Optional[bool] = None) -> HslColorTuple:
-        """
-        Returns the color as an HSL or HSLA tuple.
+        """Returns the color as an HSL or HSLA tuple.
 
         Args:
             alpha: Whether to include the alpha channel.
 
                 - `None` (default): Include the alpha channel only if it's set (e.g. not `None`).
                 - `True`: Always include alpha.
                 - `False`: Always omit alpha.
@@ -275,16 +270,15 @@
         r, g, b = (parse_color_value(v) for v in value[:3])
         return RGBA(r, g, b, parse_float_alpha(value[3]))
     else:
         raise PydanticCustomError('color_error', 'value is not a valid color: tuples must have length 3 or 4')
 
 
 def parse_str(value: str) -> RGBA:
-    """
-    Parse a string representing a color to an RGBA tuple.
+    """Parse a string representing a color to an RGBA tuple.
 
     Possible formats for the input string include:
 
     * named color, see `COLORS_BY_NAME`
     * hex short eg. `<prefix>fff` (prefix can be `#`, `0x` or nothing)
     * hex long eg. `<prefix>ffffff` (prefix can be `#`, `0x` or nothing)
     * `rgb(<r>, <g>, <b>)`
@@ -335,32 +329,30 @@
     if m:
         return parse_hsl(*m.groups())  # type: ignore
 
     raise PydanticCustomError('color_error', 'value is not a valid color: string not recognised as a valid color')
 
 
 def ints_to_rgba(r: Union[int, str], g: Union[int, str], b: Union[int, str], alpha: Optional[float] = None) -> RGBA:
-    """
-    Converts integer or string values for RGB color and an optional alpha value to an `RGBA` object.
+    """Converts integer or string values for RGB color and an optional alpha value to an `RGBA` object.
 
     Args:
         r: An integer or string representing the red color value.
         g: An integer or string representing the green color value.
         b: An integer or string representing the blue color value.
         alpha: A float representing the alpha value. Defaults to None.
 
     Returns:
         An instance of the `RGBA` class with the corresponding color and alpha values.
     """
     return RGBA(parse_color_value(r), parse_color_value(g), parse_color_value(b), parse_float_alpha(alpha))
 
 
 def parse_color_value(value: Union[int, str], max_val: int = 255) -> float:
-    """
-    Parse the color value provided and return a number between 0 and 1.
+    """Parse the color value provided and return a number between 0 and 1.
 
     Args:
         value: An integer or string color value.
         max_val: Maximum range value. Defaults to 255.
 
     Raises:
         PydanticCustomError: If the value is not a valid color.
@@ -379,16 +371,15 @@
             'color_error',
             'value is not a valid color: color values must be in the range 0 to {max_val}',
             {'max_val': max_val},
         )
 
 
 def parse_float_alpha(value: Union[None, str, float, int]) -> Optional[float]:
-    """
-    Parse an alpha value checking it's a valid float in the range 0 to 1.
+    """Parse an alpha value checking it's a valid float in the range 0 to 1.
 
     Args:
         value: The input value to parse.
 
     Returns:
         The parsed value as a float, or `None` if the value was None or equal 1.
 
@@ -410,16 +401,15 @@
     elif 0 <= alpha <= 1:
         return alpha
     else:
         raise PydanticCustomError('color_error', 'value is not a valid color: alpha values must be in the range 0 to 1')
 
 
 def parse_hsl(h: str, h_units: str, sat: str, light: str, alpha: Optional[float] = None) -> RGBA:
-    """
-    Parse raw hue, saturation, lightness, and alpha values and convert to RGBA.
+    """Parse raw hue, saturation, lightness, and alpha values and convert to RGBA.
 
     Args:
         h: The hue value.
         h_units: The unit for hue value.
         sat: The saturation value.
         light: The lightness value.
         alpha: Alpha value.
@@ -439,16 +429,15 @@
         h_value = h_value % 1
 
     r, g, b = hls_to_rgb(h_value, l_value, s_value)
     return RGBA(r, g, b, parse_float_alpha(alpha))
 
 
 def float_to_255(c: float) -> int:
-    """
-    Converts a float value between 0 and 1 (inclusive) to an integer between 0 and 255 (inclusive).
+    """Converts a float value between 0 and 1 (inclusive) to an integer between 0 and 255 (inclusive).
 
     Args:
         c: The float value to be converted. Must be between 0 and 1 (inclusive).
 
     Returns:
         The integer equivalent of the given float value rounded to the nearest whole number.
```

### Comparing `pydantic-2.0b2/pydantic/dataclasses.py` & `pydantic-2.0b3/pydantic/dataclasses.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Provide an enhanced dataclass that performs validation.
-"""
+"""Provide an enhanced dataclass that performs validation."""
 from __future__ import annotations as _annotations
 
 import dataclasses
 import sys
 import types
 from typing import TYPE_CHECKING, Any, Callable, Generic, NoReturn, TypeVar, overload
 
@@ -36,15 +34,14 @@
         unsafe_hash: bool = False,
         frozen: bool = False,
         config: ConfigDict | type[object] | None = None,
         validate_on_init: bool | None = None,
         kw_only: bool = ...,
         slots: bool = ...,
     ) -> Callable[[type[_T]], type[PydanticDataclass]]:  # type: ignore
-        """Overload for `dataclass`."""
         ...
 
     @dataclass_transform(field_specifiers=(dataclasses.field, Field))
     @overload
     def dataclass(
         _cls: type[_T],  # type: ignore
         *,
@@ -55,15 +52,14 @@
         unsafe_hash: bool = False,
         frozen: bool = False,
         config: ConfigDict | type[object] | None = None,
         validate_on_init: bool | None = None,
         kw_only: bool = ...,
         slots: bool = ...,
     ) -> type[PydanticDataclass]:
-        """Overload for `dataclass`."""
         ...
 
 else:
 
     @dataclass_transform(field_specifiers=(dataclasses.field, Field))
     @overload
     def dataclass(
@@ -73,15 +69,14 @@
         eq: bool = True,
         order: bool = False,
         unsafe_hash: bool = False,
         frozen: bool = False,
         config: ConfigDict | type[object] | None = None,
         validate_on_init: bool | None = None,
     ) -> Callable[[type[_T]], type[PydanticDataclass]]:  # type: ignore
-        """Overload for `dataclass`."""
         ...
 
     @dataclass_transform(field_specifiers=(dataclasses.field, Field))
     @overload
     def dataclass(
         _cls: type[_T],  # type: ignore
         *,
@@ -90,15 +85,14 @@
         eq: bool = True,
         order: bool = False,
         unsafe_hash: bool = False,
         frozen: bool = False,
         config: ConfigDict | type[object] | None = None,
         validate_on_init: bool | None = None,
     ) -> type[PydanticDataclass]:
-        """Overload for `dataclass`."""
         ...
 
 
 @dataclass_transform(field_specifiers=(dataclasses.field, Field))
 def dataclass(
     _cls: type[_T] | None = None,
     *,
@@ -109,80 +103,69 @@
     unsafe_hash: bool = False,
     frozen: bool = False,
     config: ConfigDict | type[object] | None = None,
     validate_on_init: bool | None = None,
     kw_only: bool = False,
     slots: bool = False,
 ) -> Callable[[type[_T]], type[PydanticDataclass]] | type[PydanticDataclass]:
-    """
-    A decorator used to create a Pydantic-enhanced dataclass, similar to the standard Python `dataclasses`,
+    """A decorator used to create a Pydantic-enhanced dataclass, similar to the standard Python `dataclasses`,
     but with added validation.
 
-    Args:
-        _cls (type[_T] | None): The target dataclass.
-        init (Literal[False]): If set to `False`, the `dataclass` will not generate an `__init__`,
-            and you will need to provide one. Defaults to `False`.
-        repr (bool): Determines if a `__repr__` should be generated for the class. Defaults to `True`.
-        eq (bool): Determines if a `__eq__` should be generated for the class. Defaults to `True`.
-        order (bool): Determines if comparison magic methods should be generated, such as `__lt__`, but
-            not `__eq__`. Defaults to `False`.
-        unsafe_hash (bool): Determines if an unsafe hashing function should be included in the class.
-        frozen (bool): Determines if the generated class should be a 'frozen' dataclass, which does not allow its
-            attributes to be modified from its constructor. Defaults to `False`.
-        config (ConfigDict | type[object] | None): A configuration for the `dataclass` generation. Defaults to `None`.
-        validate_on_init (bool | None): Determines whether the `dataclass` will be validated upon creation.
-        kw_only (bool): Determines if keyword-only parameters should be used on the `__init__` method. Defaults
-            to `False`.
+    This function should be used similarly to `dataclasses.dataclass`.
 
     Args:
         _cls: The target dataclass.
-        init: If set to `False`, the dataclass will not generate an `__init__`,
-            and you will need to provide one. Defaults to `False`.
-        repr: Determines if a `__repr__` should be generated for the class. Defaults to `True`.
-        eq: Determines if a `__eq__` should be generated for the class. Defaults to `True`.
-        order: Determines if comparison magic methods should be generated, such as` __lt__`, but
-            not `__eq__`. Defaults to `False`.
+        init: Included for signature compatibility with `dataclasses.dataclass`, and is passed through to
+            `dataclasses.dataclass` when appropriate. If specified, must be set to `False`, as pydantic inserts its
+            own  `__init__` function.
+        repr: A boolean indicating whether or not to include the field in the __repr__ output.
+        eq: Determines if a `__eq__` should be generated for the class.
+        order: Determines if comparison magic methods should be generated, such as` __lt__`, but not `__eq__`.
         unsafe_hash: Determines if an unsafe hashing function should be included in the class.
         frozen: Determines if the generated class should be a 'frozen' dataclass, which does not allow its
-            attributes to be modified from its constructor. Defaults to `False`.
-        config: A configuration for the dataclass generation. Defaults to `None`.
-        validate_on_init: Determines whether the dataclass will be validated upon creation.
-        kw_only: Determines if keyword-only parameters should be used on the `__init__` method. Defaults
-            to `False`.
+            attributes to be modified from its constructor.
+        config: A configuration for the dataclass generation.
+        validate_on_init: A deprecated parameter included for backwards compatibility; in V2, all pydantic dataclasses
+            are validated on init.
+        kw_only: Determines if `__init__` method parameters must be specified by keyword only. Defaults to `False`.
+        slots: Determines if the generated class should be a 'slots' dataclass, which does not allow the addition of
+            new attributes after instantiation.
 
     Returns:
-        A callable that takes a `type` as its argument, and returns a `type` of `PydanticDataclass`. This can
-        also return a `tyoe` of `PydanticDataclass` directly.
+        A decorator that accepts a class as its argument and returns a Pydantic dataclass.
 
     Raises:
-        AssertionError: Raised if `init` is not `False`.
+        AssertionError: Raised if `init` is not `False` or `validate_on_init` is `False`.
     """
     assert init is False, 'pydantic.dataclasses.dataclass only supports init=False'
+    assert validate_on_init is not False, 'validate_on_init=False is no longer supported'
 
     if sys.version_info >= (3, 10):
         kwargs = dict(kw_only=kw_only, slots=slots)
     else:
         kwargs = {}
 
     def create_dataclass(cls: type[Any]) -> type[PydanticDataclass]:
         """Create a Pydantic dataclass from a regular dataclass.
 
         Args:
             cls: The class to create the Pydantic dataclass from.
 
         Returns:
             A Pydantic dataclass.
-
-        Raises:
-            TypeError: If a non-class value is provided.
         """
-
         original_cls = cls
 
-        config_wrapper = _config.ConfigWrapper(config)
+        config_dict = config
+        if config_dict is None:
+            # if not explicitly provided, read from the type
+            cls_config = getattr(cls, '__pydantic_config__', None)
+            if cls_config is not None:
+                config_dict = cls_config
+        config_wrapper = _config.ConfigWrapper(config_dict)
         decorators = _decorators.DecoratorInfos.build(cls)
 
         # Keep track of the original __doc__ so that we can restore it after applying the dataclasses decorator
         # Otherwise, classes with no __doc__ will have their signature added into the JSON schema description,
         # since dataclasses.dataclass will set this as the __doc__
         original_doc = cls.__doc__
 
@@ -230,16 +213,15 @@
 __getattr__ = getattr_migration(__name__)
 
 if (3, 8) <= sys.version_info < (3, 11):
     # Monkeypatch dataclasses.InitVar so that typing doesn't error if it occurs as a type when evaluating type hints
     # Starting in 3.11, typing.get_type_hints will not raise an error if the retrieved type hints are not callable.
 
     def _call_initvar(*args: Any, **kwargs: Any) -> NoReturn:
-        """
-        This function does nothing but raise an error that is as similar as possible to what you'd get
+        """This function does nothing but raise an error that is as similar as possible to what you'd get
         if you were to try calling `InitVar[int]()` without this monkeypatch. The whole purpose is just
         to ensure typing._type_check does not error if the type hint evaluates to `InitVar[<parameter>]`.
         """
         raise TypeError("'InitVar' object is not callable")
 
     dataclasses.InitVar.__call__ = _call_initvar  # type: ignore
 
@@ -248,29 +230,31 @@
     cls: type[PydanticDataclass],
     *,
     force: bool = False,
     raise_errors: bool = True,
     _parent_namespace_depth: int = 2,
     _types_namespace: dict[str, Any] | None = None,
 ) -> bool | None:
-    """
-    Try to rebuild or reconstruct the dataclass core schema.
+    """Try to rebuild the pydantic-core schema for the dataclass.
+
+    This may be necessary when one of the annotations is a ForwardRef which could not be resolved during
+    the initial attempt to build the schema, and automatic rebuilding fails.
 
     This is analogous to `BaseModel.model_rebuild`.
 
     Args:
         cls: The class to build the dataclass core schema for.
         force: Whether to force the rebuilding of the model schema, defaults to `False`.
         raise_errors: Whether to raise errors, defaults to `True`.
         _parent_namespace_depth: The depth level of the parent namespace, defaults to 2.
         _types_namespace: The types namespace, defaults to `None`.
 
     Returns:
-        Returns `None` if model schema is complete and no rebuilding is required.
-            If rebuilding _is_ required, returns `True` if rebuilding was successful, otherwise `False`.
+        Returns `None` if the schema is already "complete" and rebuilding was not required.
+        If rebuilding _was_ required, returns `True` if rebuilding was successful, otherwise `False`.
     """
     if not force and cls.__pydantic_complete__:
         return None
     else:
         if _types_namespace is not None:
             types_namespace: dict[str, Any] | None = _types_namespace.copy()
         else:
```

### Comparing `pydantic-2.0b2/pydantic/errors.py` & `pydantic-2.0b3/pydantic/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Pydantic errors.
-"""
+"""Pydantic-specific errors."""
 from __future__ import annotations as _annotations
 
 import re
 
 from typing_extensions import Literal, Self
 
 from ._migration import getattr_migration
@@ -12,14 +10,15 @@
 
 __all__ = (
     'PydanticUserError',
     'PydanticUndefinedAnnotation',
     'PydanticImportError',
     'PydanticSchemaGenerationError',
     'PydanticInvalidForJsonSchema',
+    'PydanticErrorCodes',
 )
 
 # We use this URL to allow for future flexibility about how we host the docs, while allowing for Pydantic
 # code in the while with "old" URLs to still work.
 # 'u' refers to "user errors" - e.g. errors caused by developers using pydantic, as opposed to validation errors.
 DEV_ERROR_DOCS_URL = f'https://errors.pydantic.dev/{VERSION}/u/'
 PydanticErrorCodes = Literal[
@@ -30,15 +29,15 @@
     'discriminator-alias-type',
     'discriminator-needs-literal',
     'discriminator-alias',
     'typed-dict-version',
     'model-field-overridden',
     'model-field-missing-annotation',
     'config-both',
-    'deprecated-kwargs',
+    'removed-kwargs',
     'invalid-for-json-schema',
     'json-schema-already-used',
     'base-model-instantiated',
     'undefined-annotation',
     'schema-for-unknown-type',
     'import-error',
     'create-model-field-definitions',
@@ -56,55 +55,51 @@
     'multiple-field-serializers',
     'invalid_annotated_type',
     'type-adapter-config-unused',
 ]
 
 
 class PydanticErrorMixin:
-    """
-    A mixin class for common functionality shared by all Pydantic-specific errors.
+    """A mixin class for common functionality shared by all Pydantic-specific errors.
 
     Attributes:
-        message (str): A message describing the error.
-        code (PydanticErrorCodes | None): An optional error code from PydanticErrorCodes enum.
+        message: A message describing the error.
+        code: An optional error code from PydanticErrorCodes enum.
     """
 
     def __init__(self, message: str, *, code: PydanticErrorCodes | None) -> None:
         self.message = message
         self.code = code
 
     def __str__(self) -> str:
         if self.code is None:
             return self.message
         else:
             return f'{self.message}\n\nFor further information visit {DEV_ERROR_DOCS_URL}{self.code}'
 
 
 class PydanticUserError(PydanticErrorMixin, TypeError):
-    """
-    Error raised due to incorrect use of Pydantic.
-    """
+    """An error raised due to incorrect use of Pydantic."""
 
 
 class PydanticUndefinedAnnotation(PydanticErrorMixin, NameError):
     """A subclass of `NameError` raised when handling undefined annotations during `CoreSchema` generation.
 
     Attributes:
-        name (str): Name of the error.
-        message (str): Description of the error.
+        name: Name of the error.
+        message: Description of the error.
     """
 
     def __init__(self, name: str, message: str) -> None:
         self.name = name
         super().__init__(message=message, code='undefined-annotation')
 
     @classmethod
     def from_name_error(cls, name_error: NameError) -> Self:
-        """
-        Convert a `NameError` to a `PydanticUndefinedAnnotation` error.
+        """Convert a `NameError` to a `PydanticUndefinedAnnotation` error.
 
         Args:
             name_error: `NameError` to be converted.
 
         Returns:
             Converted `PydanticUndefinedAnnotation` error.
         """
@@ -112,43 +107,40 @@
             name = name_error.name  # type: ignore  # python > 3.10
         except AttributeError:
             name = re.search(r".*'(.+?)'", str(name_error)).group(1)  # type: ignore[union-attr]
         return cls(name=name, message=str(name_error))
 
 
 class PydanticImportError(PydanticErrorMixin, ImportError):
-    """
-    Error raised when an import fails due to module changes between V1 and V2.
+    """An error raised when an import fails due to module changes between V1 and V2.
 
     Attributes:
-        message (str): Description of the error.
+        message: Description of the error.
     """
 
     def __init__(self, message: str) -> None:
         super().__init__(message, code='import-error')
 
 
 class PydanticSchemaGenerationError(PydanticUserError):
-    """
-    Error raised during failures to generate a `CoreSchema` for some type.
+    """An error raised during failures to generate a `CoreSchema` for some type.
 
     Attributes:
-        message (str): Description of the error.
+        message: Description of the error.
     """
 
     def __init__(self, message: str) -> None:
         super().__init__(message, code='schema-for-unknown-type')
 
 
 class PydanticInvalidForJsonSchema(PydanticUserError):
-    """
-    Error raised during failures to generate a JSON schema for some `CoreSchema`.
+    """An error raised during failures to generate a JSON schema for some `CoreSchema`.
 
     Attributes:
-        message (str): Description of the error.
+        message: Description of the error.
     """
 
     def __init__(self, message: str) -> None:
         super().__init__(message, code='invalid-for-json-schema')
 
 
 __getattr__ = getattr_migration(__name__)
```

### Comparing `pydantic-2.0b2/pydantic/fields.py` & `pydantic-2.0b3/pydantic/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-"""
-Defining fields on models.
-"""
+"""Defining fields on models."""
 from __future__ import annotations as _annotations
 
 import dataclasses
 import inspect
 import sys
 import typing
 from copy import copy
 from dataclasses import Field as DataclassField
 from typing import Any
 from warnings import warn
 
 import annotated_types
 import typing_extensions
+from typing_extensions import Unpack
 
 from . import types
 from ._internal import _decorators, _fields, _generics, _internal_dataclass, _repr, _typing_extra, _utils
 from .errors import PydanticUserError
 
 if typing.TYPE_CHECKING:
     from ._internal._repr import ReprArgs
 
 _Undefined = _fields.Undefined
 
 
 class _FromFieldInfoInputs(typing_extensions.TypedDict, total=False):
-    """
-    This class exists solely to add type checking for the `**kwargs` in `FieldInfo.from_field`.
-    """
+    """This class exists solely to add type checking for the `**kwargs` in `FieldInfo.from_field`."""
 
     annotation: type[Any] | None
     default_factory: typing.Callable[[], Any] | None
     alias: str | None
     alias_priority: int | None
     validation_alias: str | AliasPath | AliasChoices | None
     serialization_alias: str | None
@@ -60,24 +57,21 @@
     validate_default: bool | None
     repr: bool
     init_var: bool | None
     kw_only: bool | None
 
 
 class _FieldInfoInputs(_FromFieldInfoInputs, total=False):
-    """
-    This class exists solely to add type checking for the `**kwargs` in `FieldInfo.__init__`.
-    """
+    """This class exists solely to add type checking for the `**kwargs` in `FieldInfo.__init__`."""
 
     default: Any
 
 
 class FieldInfo(_repr.Representation):
-    """
-    This class holds information about a field.
+    """This class holds information about a field.
 
     `FieldInfo` is used for any field definition regardless of whether the `Field()` function is explicitly used.
 
     Attributes:
         annotation: The type annotation of the field.
         default: The default value of the field.
         default_factory: The factory function used to construct the default for the field.
@@ -160,17 +154,16 @@
         'max_length': annotated_types.MaxLen,
         'pattern': None,
         'allow_inf_nan': None,
         'max_digits': None,
         'decimal_places': None,
     }
 
-    def __init__(self, **kwargs: typing_extensions.Unpack[_FieldInfoInputs]) -> None:
-        """
-        This class should generally not be initialized directly; instead, use the `pydantic.fields.Field` function
+    def __init__(self, **kwargs: Unpack[_FieldInfoInputs]) -> None:
+        """This class should generally not be initialized directly; instead, use the `pydantic.fields.Field` function
         or one of the constructor classmethods.
 
         See the signature of `pydantic.fields.Field` for more details about the expected arguments.
         """
         self.annotation, annotation_metadata = self._extract_metadata(kwargs.get('annotation'))
 
         default = kwargs.pop('default', _Undefined)
@@ -180,19 +173,20 @@
             self.default = default
 
         self.default_factory = kwargs.pop('default_factory', None)
 
         if self.default is not _Undefined and self.default_factory is not None:
             raise TypeError('cannot specify both default and default_factory')
 
-        self.alias = kwargs.pop('alias', None)
-        self.alias_priority = kwargs.pop('alias_priority', None) or 2 if self.alias is not None else None
         self.title = kwargs.pop('title', None)
+        self.alias = kwargs.pop('alias', None)
         self.validation_alias = kwargs.pop('validation_alias', None)
         self.serialization_alias = kwargs.pop('serialization_alias', None)
+        alias_is_set = any(alias is not None for alias in (self.alias, self.validation_alias, self.serialization_alias))
+        self.alias_priority = kwargs.pop('alias_priority', None) or 2 if alias_is_set else None
         self.description = kwargs.pop('description', None)
         self.examples = kwargs.pop('examples', None)
         self.exclude = kwargs.pop('exclude', None)
         self.include = kwargs.pop('include', None)
         self.discriminator = kwargs.pop('discriminator', None)
         self.repr = kwargs.pop('repr', True)
         self.json_schema_extra = kwargs.pop('json_schema_extra', None)
@@ -202,19 +196,16 @@
         # currently only used on dataclasses
         self.init_var = kwargs.pop('init_var', None)
         self.kw_only = kwargs.pop('kw_only', None)
 
         self.metadata = self._collect_metadata(kwargs) + annotation_metadata  # type: ignore
 
     @classmethod
-    def from_field(
-        cls, default: Any = _Undefined, **kwargs: typing_extensions.Unpack[_FromFieldInfoInputs]
-    ) -> typing_extensions.Self:
-        """
-        Create a new `FieldInfo` object with the `Field` function.
+    def from_field(cls, default: Any = _Undefined, **kwargs: Unpack[_FromFieldInfoInputs]) -> typing_extensions.Self:
+        """Create a new `FieldInfo` object with the `Field` function.
 
         Args:
             default: The default value for the field. Defaults to Undefined.
             **kwargs: Additional arguments dictionary.
 
         Raises:
             TypeError: If 'annotation' is passed as a keyword argument.
@@ -234,16 +225,15 @@
         """
         if 'annotation' in kwargs:
             raise TypeError('"annotation" is not permitted as a Field keyword argument')
         return cls(default=default, **kwargs)
 
     @classmethod
     def from_annotation(cls, annotation: type[Any]) -> typing_extensions.Self:
-        """
-        Creates a `FieldInfo` instance from a bare annotation.
+        """Creates a `FieldInfo` instance from a bare annotation.
 
         Args:
             annotation: An annotation object.
 
         Returns:
             An instance of the field metadata.
 
@@ -286,16 +276,15 @@
                 new_field_info.metadata += [a for a in extra_args if not isinstance(a, FieldInfo)]
                 return new_field_info
 
         return cls(annotation=annotation, final=final)
 
     @classmethod
     def from_annotated_attribute(cls, annotation: type[Any], default: Any) -> typing_extensions.Self:
-        """
-        Create `FieldInfo` from an annotation with a default value.
+        """Create `FieldInfo` from an annotation with a default value.
 
         Args:
             annotation: The type annotation of the field.
             default: The default value of the field.
 
         Returns:
             A field object with the passed values.
@@ -352,16 +341,15 @@
                     new_field_info.metadata += [a for a in extra_args if not isinstance(a, FieldInfo)]
                     return new_field_info
 
             return cls(annotation=annotation, default=default, final=final)
 
     @classmethod
     def _from_dataclass_field(cls, dc_field: DataclassField[Any]) -> typing_extensions.Self:
-        """
-        Return a new `FieldInfo` instance from a `dataclasses.Field` instance.
+        """Return a new `FieldInfo` instance from a `dataclasses.Field` instance.
 
         Args:
             dc_field: The `dataclasses.Field` instance to convert.
 
         Returns:
             The corresponding `FieldInfo` instance.
 
@@ -404,29 +392,27 @@
                     raise TypeError('Field may not be used twice on the same field')
                 return first_arg, list(extra_args)
 
         return annotation, []
 
     @staticmethod
     def _find_field_info_arg(args: Any) -> FieldInfo | None:
-        """
-        Find an instance of `FieldInfo` in the provided arguments.
+        """Find an instance of `FieldInfo` in the provided arguments.
 
         Args:
             args: The argument list to search for `FieldInfo`.
 
         Returns:
             An instance of `FieldInfo` if found, otherwise `None`.
         """
         return next((a for a in args if isinstance(a, FieldInfo)), None)
 
     @classmethod
     def _collect_metadata(cls, kwargs: dict[str, Any]) -> list[Any]:
-        """
-        Collect annotations from kwargs.
+        """Collect annotations from kwargs.
 
         The return type is actually `annotated_types.BaseMetadata | PydanticMetadata`,
         but it gets combined with `list[Any]` from `Annotated[T, ...]`, hence types.
 
         Args:
             kwargs: Keyword arguments passed to the function.
 
@@ -449,16 +435,15 @@
                 else:
                     metadata.append(marker(value))
         if general_metadata:
             metadata.append(_fields.PydanticGeneralMetadata(**general_metadata))
         return metadata
 
     def get_default(self, *, call_default_factory: bool = False) -> Any:
-        """
-        Get the default value.
+        """Get the default value.
 
         We expose an option for whether to call the default_factory (if present), as calling it may
         result in side effects that we want to avoid. However, there are times when it really should
         be called (namely, when instantiating a model via `model_construct`).
 
         Args:
             call_default_factory: Whether to call the default_factory or not. Defaults to `False`.
@@ -478,31 +463,30 @@
 
         Returns:
             `True` if the argument is required, `False` otherwise.
         """
         return self.default is _Undefined and self.default_factory is None
 
     def rebuild_annotation(self) -> Any:
-        """
-        Rebuilds the original annotation for use in function signatures.
+        """Rebuilds the original annotation for use in function signatures.
 
         If metadata is present, it adds it to the original annotation using an
         `AnnotatedAlias`. Otherwise, it returns the original annotation as is.
 
         Returns:
             The rebuilt annotation.
         """
         if not self.metadata:
             return self.annotation
         else:
-            return typing_extensions._AnnotatedAlias(self.annotation, self.metadata)
+            # Annotated arguments must be a tuple
+            return typing_extensions.Annotated[(self.annotation, *self.metadata)]  # type: ignore
 
     def apply_typevars_map(self, typevars_map: dict[Any, Any] | None, types_namespace: dict[str, Any] | None) -> None:
-        """
-        Apply a `typevars_map` to the annotation.
+        """Apply a `typevars_map` to the annotation.
 
         This method is used when analyzing parametrized generic types to replace typevars with their concrete types.
 
         This method applies the `typevars_map` to the annotation in place.
 
         Args:
             typevars_map: A dictionary mapping type variables to their concrete types.
@@ -540,75 +524,67 @@
                 value = getattr(self, s)
                 if value is not None and value is not _Undefined:
                     yield s, value
 
 
 @_internal_dataclass.slots_dataclass
 class AliasPath:
-    """
-    A data class used by `validation_alias` as a convenience to create aliases.
+    """A data class used by `validation_alias` as a convenience to create aliases.
 
     Attributes:
         path: A list of string or integer aliases.
     """
 
     path: list[int | str]
 
     def __init__(self, first_arg: str, *args: str | int) -> None:
         self.path = [first_arg] + list(args)
 
     def convert_to_aliases(self) -> list[str | int]:
-        """
-        Converts arguments to a list of string or integer aliases.
+        """Converts arguments to a list of string or integer aliases.
 
         Returns:
             The list of aliases.
         """
         return self.path
 
 
 @_internal_dataclass.slots_dataclass
 class AliasChoices:
-    """
-    A data class used by `validation_alias` as a convenience to create aliases.
+    """A data class used by `validation_alias` as a convenience to create aliases.
 
     Attributes:
         choices: A list containing a string or `AliasPath`.
     """
 
     choices: list[str | AliasPath]
 
     def __init__(self, first_choice: str | AliasPath, *choices: str | AliasPath) -> None:
         self.choices = [first_choice] + list(choices)
 
     def convert_to_aliases(self) -> list[list[str | int]]:
-        """
-        Converts arguments to a list of lists containing string or integer aliases.
+        """Converts arguments to a list of lists containing string or integer aliases.
 
         Returns:
             The list of aliases.
         """
         aliases: list[list[str | int]] = []
         for c in self.choices:
             if isinstance(c, AliasPath):
                 aliases.append(c.convert_to_aliases())
             else:
                 aliases.append([c])
         return aliases
 
 
 class _EmptyKwargs(typing_extensions.TypedDict):
-    """
-    This class exists solely to ensure that type checking warns about passing `**extra` in `Field`.
-    """
-
-    pass
+    """This class exists solely to ensure that type checking warns about passing `**extra` in `Field`."""
 
 
-def Field(  # noqa C901
+def Field(  # C901
     default: Any = _Undefined,
     *,
     default_factory: typing.Callable[[], Any] | None = None,
     alias: str | None = None,
     alias_priority: int | None = None,
     validation_alias: str | AliasPath | AliasChoices | None = None,
     serialization_alias: str | None = None,
@@ -633,18 +609,17 @@
     le: float | None = None,
     multiple_of: float | None = None,
     allow_inf_nan: bool | None = None,
     max_digits: int | None = None,
     decimal_places: int | None = None,
     min_length: int | None = None,
     max_length: int | None = None,
-    **extra: typing_extensions.Unpack[_EmptyKwargs],
+    **extra: Unpack[_EmptyKwargs],
 ) -> Any:
-    """
-    Create a field for objects that can be configured.
+    """Create a field for objects that can be configured.
 
     Used to provide extra information about a field, either for the model schema or complex validation. Some arguments
     apply only to number fields (`int`, `float`, `Decimal`) and some apply only to `str`.
 
     Args:
         default: Default value if the field is not set.
         default_factory: A callable to generate the default value, such as :func:`~datetime.utcnow`.
@@ -660,37 +635,41 @@
         exclude: Whether to exclude the field from the model schema.
         include: Whether to include the field in the model schema.
         discriminator: Field name for discriminating the type in a tagged union.
         json_schema_extra: Any additional JSON schema data for the schema property.
         frozen: Whether the field is frozen.
         final: Whether the field is final.
         validate_default: Run validation that isn't only checking existence of defaults. `True` by default.
-        repr: If `True` (the default), return a string representation of the field.
+        repr: A boolean indicating whether to include the field in the `__repr__` output.
         init_var: Whether the field should be included in the constructor of the dataclass.
         kw_only: Whether the field should be a keyword-only argument in the constructor of the dataclass.
         strict: If `True` (the default is `None`), the field should be validated strictly.
         gt: Greater than. If set, value must be greater than this. Only applicable to numbers.
         ge: Greater than or equal. If set, value must be greater than or equal to this. Only applicable to numbers.
         lt: Less than. If set, value must be less than this. Only applicable to numbers.
         le: Less than or equal. If set, value must be less than or equal to this. Only applicable to numbers.
         multiple_of: Value must be a multiple of this. Only applicable to numbers.
         min_length: Minimum length for strings.
         max_length: Maximum length for strings.
         pattern: Pattern for strings.
         allow_inf_nan: Allow `inf`, `-inf`, `nan`. Only applicable to numbers.
         max_digits: Maximum number of allow digits for strings.
         decimal_places: Maximum number of decimal places allowed for numbers.
+        extra: Include extra fields used by the JSON schema.
+
+            !!! warning Deprecated
+                The `extra` kwargs is deprecated. Use `json_schema_extra` instead.
 
     Returns:
         The generated `FieldInfo` object
     """
     # Check deprecated and removed params from V1. This logic should eventually be removed.
     const = extra.pop('const', None)  # type: ignore
     if const is not None:
-        raise PydanticUserError('`const` is removed, use `Literal` instead', code='deprecated-kwargs')
+        raise PydanticUserError('`const` is removed, use `Literal` instead', code='removed-kwargs')
 
     min_items = extra.pop('min_items', None)  # type: ignore
     if min_items is not None:
         warn('`min_items` is deprecated and will be removed, use `min_length` instead', DeprecationWarning)
         if min_length is None:
             min_length = min_items  # type: ignore
 
@@ -703,38 +682,37 @@
     unique_items = extra.pop('unique_items', None)  # type: ignore
     if unique_items is not None:
         raise PydanticUserError(
             (
                 '`unique_items` is removed, use `Set` instead'
                 '(this feature is discussed in https://github.com/pydantic/pydantic-core/issues/296)'
             ),
-            code='deprecated-kwargs',
+            code='removed-kwargs',
         )
 
     allow_mutation = extra.pop('allow_mutation', None)  # type: ignore
     if allow_mutation is not None:
         warn('`allow_mutation` is deprecated and will be removed. use `frozen` instead', DeprecationWarning)
         if allow_mutation is False:
             frozen = True
 
     regex = extra.pop('regex', None)  # type: ignore
     if regex is not None:
-        raise PydanticUserError('`regex` is removed. use `pattern` instead', code='deprecated-kwargs')
+        raise PydanticUserError('`regex` is removed. use `pattern` instead', code='removed-kwargs')
 
     if extra:
         warn(
             'Extra keyword arguments on `Field` is deprecated and will be removed. use `json_schema_extra` instead',
             DeprecationWarning,
         )
         if not json_schema_extra:
             json_schema_extra = extra  # type: ignore
 
-    if validation_alias:
-        if not isinstance(validation_alias, (str, AliasChoices, AliasPath)):
-            raise TypeError('Invalid `validation_alias` type. it should be `str`, `AliasChoices`, or `AliasPath`')
+    if validation_alias and not isinstance(validation_alias, (str, AliasChoices, AliasPath)):
+        raise TypeError('Invalid `validation_alias` type. it should be `str`, `AliasChoices`, or `AliasPath`')
 
     if serialization_alias is None and isinstance(alias, str):
         serialization_alias = alias
 
     return FieldInfo.from_field(
         default,
         default_factory=default_factory,
@@ -770,49 +748,46 @@
     )
 
 
 class ModelPrivateAttr(_repr.Representation):
     """A descriptor for private attributes in class models.
 
     Attributes:
-        default (Any): The default value of the attribute if not provided.
-        default_factory (typing.Callable[[], Any]): A callable function that generates the default value of the
+        default: The default value of the attribute if not provided.
+        default_factory: A callable function that generates the default value of the
             attribute if not provided.
     """
 
     __slots__ = 'default', 'default_factory'
 
     def __init__(self, default: Any = _Undefined, *, default_factory: typing.Callable[[], Any] | None = None) -> None:
         self.default = default
         self.default_factory = default_factory
 
     def __getattr__(self, item: str) -> Any:
-        """
-        This function improves compatibility with custom descriptors by ensuring delegation happens
+        """This function improves compatibility with custom descriptors by ensuring delegation happens
         as expected when the default value of a private attribute is a descriptor.
         """
         if item in {'__get__', '__set__', '__delete__'}:
             if hasattr(self.default, item):
                 return getattr(self.default, item)
         raise AttributeError(f'{type(self).__name__!r} object has no attribute {item!r}')
 
     def __set_name__(self, cls: type[Any], name: str) -> None:
-        """
-        Preserve `__set_name__` protocol defined in https://peps.python.org/pep-0487.
-        """
+        """Preserve `__set_name__` protocol defined in https://peps.python.org/pep-0487."""
         if self.default is _Undefined:
             return
         if not hasattr(self.default, '__set_name__'):
             return
         set_name = self.default.__set_name__
         if callable(set_name):
             set_name(cls, name)
 
     def get_default(self) -> Any:
-        """Returns the default value for the object.
+        """Retrieve the default value of the object.
 
         If `self.default_factory` is `None`, the method will return a deep copy of the `self.default` object.
 
         If `self.default_factory` is not `None`, it will call `self.default_factory` and return the value returned.
 
         Returns:
             The default value of the object.
@@ -827,20 +802,19 @@
 
 
 def PrivateAttr(
     default: Any = _Undefined,
     *,
     default_factory: typing.Callable[[], Any] | None = None,
 ) -> Any:
-    """
-    Indicates that attribute is only used internally and never mixed with regular fields.
+    """Indicates that attribute is only used internally and never mixed with regular fields.
 
     Private attributes are not checked by Pydantic, so it's up to you to maintain their accuracy.
 
-    Private attributes are stored in the model `__slots__`.
+    Private attributes are stored in `__private_attributes__` on the model.
 
     Args:
         default: The attribute's default value. Defaults to Undefined.
         default_factory: Callable that will be
             called when a default value is needed for this attribute.
             If both `default` and `default_factory` are set, an error will be raised.
 
@@ -857,16 +831,15 @@
         default,
         default_factory=default_factory,
     )
 
 
 @_internal_dataclass.slots_dataclass
 class ComputedFieldInfo:
-    """
-    A container for data from `@computed_field` so that we can access it while building the pydantic-core schema.
+    """A container for data from `@computed_field` so that we can access it while building the pydantic-core schema.
 
     Attributes:
         decorator_repr: A class variable representing the decorator string, '@computed_field'.
         wrapped_property: The wrapped computed field property.
         return_type: The type of the computed field property's return value.
         alias: The alias of the property to be used during encoding and decoding.
         alias_priority: priority of the alias. This affects whether an alias generator is used
@@ -884,32 +857,14 @@
     description: str | None
     repr: bool
 
 
 # this should really be `property[T], cached_proprety[T]` but property is not generic unlike cached_property
 # See https://github.com/python/typing/issues/985 and linked issues
 PropertyT = typing.TypeVar('PropertyT')
-"""
-`TypeVar` that can be used to specify the type of a property.
-
-This can be used in combination with the `@property` decorator to specify the type
-of the property.
-
-Example:
-    ```py
-    class MyClass:
-        @property
-        def my_property(self) -> PropertyT:
-            return self._my_property
-
-        @my_property.setter
-        def my_property(self, value: PropertyT) -> None:
-            self._my_property = value
-    ```
-"""
 
 
 @typing.overload
 def computed_field(
     *,
     return_type: Any = None,
     alias: str | None = None,
@@ -932,29 +887,28 @@
     alias: str | None = None,
     alias_priority: int | None = None,
     title: str | None = None,
     description: str | None = None,
     repr: bool = True,
     return_type: Any = None,
 ) -> PropertyT | typing.Callable[[PropertyT], PropertyT]:
-    """
-    Decorate to include `property` and `cached_property` when serialising models.
+    """Decorate to include `property` and `cached_property` when serializing models.
 
     If applied to functions not yet decorated with `@property` or `@cached_property`, the function is
     automatically wrapped with `property`.
 
     Args:
         __f: the function to wrap.
         alias: alias to use when serializing this computed field, only used when `by_alias=True`
         alias_priority: priority of the alias. This affects whether an alias generator is used
         title: Title to used when including this computed field in JSON Schema, currently unused waiting for #4697
         description: Description to used when including this computed field in JSON Schema, defaults to the functions
             docstring, currently unused waiting for #4697
         repr: whether to include this computed field in model repr
-        return_type: optional return for serialization logic to expect when serialising to JSON, if included
+        return_type: optional return for serialization logic to expect when serializing to JSON, if included
             this must be correct, otherwise a `TypeError` is raised.
             If you don't include a return type Any is used, which does runtime introspection to handle arbitrary
             objects.
 
     Returns:
         A proxy wrapper for the property.
     """
```

### Comparing `pydantic-2.0b2/pydantic/functional_serializers.py` & `pydantic-2.0b3/pydantic/functional_serializers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,39 @@
+"""This module contains related classes and functions for serialization."""
 from __future__ import annotations
 
 from functools import partialmethod
 from typing import TYPE_CHECKING, Any, Callable, TypeVar, Union, overload
 
 from pydantic_core import core_schema
 from pydantic_core import core_schema as _core_schema
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import Annotated, Literal, TypeAlias
 
 from ._internal import _annotated_handlers, _decorators, _internal_dataclass
 
 
 @_internal_dataclass.slots_dataclass(frozen=True)
 class PlainSerializer:
-    """
-    Plain serializers use a function to modify the output of serialization.
+    """Plain serializers use a function to modify the output of serialization.
 
     Attributes:
-        func (core_schema.SerializerFunction): The serializer function.
+        func: The serializer function.
         return_type: Optional return type for the function, if omitted it will be inferred from the type annotation.
-        when_used (Literal['always', 'unless-none', 'json', 'json-unless-none'], optional): The serialization condition.
-            Defaults to 'always'.
+        when_used: The serialization condition. Accepts a string with values `'always'`, `'unless-none'`, `'json'`,
+            and `'json-unless-none'`. Defaults to 'always'.
     """
 
     func: core_schema.SerializerFunction
     return_type: Any = None
     when_used: Literal['always', 'unless-none', 'json', 'json-unless-none'] = 'always'
 
     def __get_pydantic_core_schema__(
         self, source_type: Any, handler: _annotated_handlers.GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
-        """
-        Gets the Pydantic core schema.
+        """Gets the Pydantic core schema.
 
         Args:
             source_type: The source type.
             handler: The `GetCoreSchemaHandler` instance.
 
         Returns:
             The Pydantic core schema.
@@ -49,33 +48,32 @@
             when_used=self.when_used,
         )
         return schema
 
 
 @_internal_dataclass.slots_dataclass(frozen=True)
 class WrapSerializer:
-    """
-    Wrap serializers receive the raw inputs along with a handler function that applies the standard serialization logic,
-    and can modify the resulting value before returning it as the final output of serialization.
+    """Wrap serializers receive the raw inputs along with a handler function that applies the standard serialization
+    logic, and can modify the resulting value before returning it as the final output of serialization.
 
     Attributes:
-        func (core_schema.WrapSerializerFunction): The function to be wrapped.
-        return_type: Optional return type for the function, if omitted it will be inferred from the type annotation.
-        when_used: Determines the serializer will be used for serialization.
+        func: The function to be wrapped.
+        return_type: The return type for the function, if omitted it will be inferred from the type annotation.
+        when_used: Determines when this serializer should be used. Accepts a string with values `'always'`,
+            `'unless-none'`, `'json'`, and `'json-unless-none'`. Defaults to 'always'.
     """
 
     func: core_schema.WrapSerializerFunction
     return_type: Any = None
     when_used: Literal['always', 'unless-none', 'json', 'json-unless-none'] = 'always'
 
     def __get_pydantic_core_schema__(
         self, source_type: Any, handler: _annotated_handlers.GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
-        """
-        This method is used to get the Pydantic core schema of the class.
+        """This method is used to get the Pydantic core schema of the class.
 
         Args:
             source_type: Source type.
             handler: Core schema handler.
 
         Returns:
             The generated core schema of the class.
@@ -138,16 +136,15 @@
 def field_serializer(
     *fields: str,
     mode: Literal['plain', 'wrap'] = 'plain',
     return_type: Any = None,
     when_used: Literal['always', 'unless-none', 'json', 'json-unless-none'] = 'always',
     check_fields: bool | None = None,
 ) -> Callable[[Any], Any]:
-    """
-    Decorate methods on the class indicating that they should be used to serialize fields.
+    """Decorate methods on the class indicating that they should be used to serialize fields.
 
     Four signatures are supported:
 
     - `(self, value: Any, info: FieldSerializationInfo)`
     - `(self, value: Any, nxt: SerializerFunctionWrapHandler, info: FieldSerializationInfo)`
     - `(value: Any, info: SerializationInfo)`
     - `(value: Any, nxt: SerializerFunctionWrapHandler, info: SerializationInfo)`
@@ -155,15 +152,15 @@
     Args:
         fields: Which field(s) the method should be called on.
         mode: `plain` means the function will be called instead of the default serialization logic,
             `wrap` means the function will be called with an argument to optionally call the
             default serialization logic.
         return_type: Optional return type for the function, if omitted it will be inferred from the type annotation.
         when_used: Determines the serializer will be used for serialization.
-        check_fields (bool): Whether to check that the fields actually exist on the model.
+        check_fields: Whether to check that the fields actually exist on the model.
 
     Returns:
         A decorator that can be used to decorate a function to be used as a field serializer.
     """
 
     def dec(
         f: Callable[..., Any] | staticmethod[Any, Any] | classmethod[Any, Any, Any]
@@ -201,26 +198,24 @@
 def model_serializer(
     __f: Callable[..., Any] | None = None,
     *,
     mode: Literal['plain', 'wrap'] = 'plain',
     when_used: Literal['always', 'unless-none', 'json', 'json-unless-none'] = 'always',
     return_type: Any = None,
 ) -> Callable[[Any], Any]:
-    """
-    Decorate a function which will be called to serialize the model.
-
-    (`when_used` is not permitted here since it makes no sense.)
+    """Decorate a function which will be called to serialize the model.
 
     Args:
         __f: The function to be decorated.
         mode: The serialization mode. `'plain'` means the function will be called
             instead of the default serialization logic, `'wrap'` means the function will be called with an argument
             to optionally call the default serialization logic.
-        when_used: Determines the serializer will be be used for serialization.
-        return_type: Optional return type for the function, if omitted it will be inferred from the type annotation.
+        when_used: Determines when this serializer should be used. Accepts a string with values `'always'`,
+            `'unless-none'`, `'json'`, `'json-unless-none'`. Defaults to `'always'`.
+        return_type: The return type for the function, if omitted it will be inferred from the type annotation.
 
     Returns:
         A decorator that can be used to decorate a function to be used as a model serializer.
     """
 
     def dec(f: Callable[..., Any]) -> _decorators.PydanticDescriptorProxy[Any]:
         dec_info = _decorators.ModelSerializerDecoratorInfo(
@@ -228,7 +223,38 @@
         )
         return _decorators.PydanticDescriptorProxy(f, dec_info)
 
     if __f is None:
         return dec
     else:
         return dec(__f)  # type: ignore
+
+
+AnyType = TypeVar('AnyType')
+
+
+if TYPE_CHECKING:
+    SerializeAsAny = Annotated[AnyType, ...]  # SerializeAsAny[list[str]] will be treated by type checkers as list[str]
+    """Force serialization to ignore whatever is defined in the schema and instead ask the object
+    itself how it should be serialized.
+    In particular, this means that when model subclasses are serialized, fields present in the subclass
+    but not in the original schema will be included.
+    """
+else:
+
+    @_internal_dataclass.slots_dataclass
+    class SerializeAsAny:  # noqa: D101
+        def __class_getitem__(cls, item: Any) -> Any:
+            return Annotated[item, SerializeAsAny()]
+
+        def __get_pydantic_core_schema__(
+            self, source_type: Any, handler: _annotated_handlers.GetCoreSchemaHandler
+        ) -> core_schema.CoreSchema:
+            schema = handler(source_type)
+            schema_to_update = schema
+            while schema_to_update['type'] == 'definitions':
+                schema_to_update = schema_to_update.copy()
+                schema_to_update = schema_to_update['schema']
+            schema_to_update['serialization'] = core_schema.wrap_serializer_function_ser_schema(
+                lambda x, h: h(x), schema=core_schema.any_schema()
+            )
+            return schema
```

### Comparing `pydantic-2.0b2/pydantic/json_schema.py` & `pydantic-2.0b3/pydantic/json_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,29 @@
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
 import pydantic_core
-from pydantic_core import CoreSchema, PydanticOmit, core_schema
+from pydantic_core import CoreConfig, CoreSchema, PydanticOmit, core_schema, to_jsonable_python
 from pydantic_core.core_schema import ComputedField
 from typing_extensions import Literal, assert_never
 
+from pydantic._internal import _annotated_handlers, _internal_dataclass
+
 from ._internal import _core_metadata, _core_utils, _schema_generation_shared, _typing_extra
 from .config import JsonSchemaExtraCallable
 from .errors import PydanticInvalidForJsonSchema, PydanticUserError
 
 if TYPE_CHECKING:
     from . import ConfigDict
     from ._internal._core_utils import CoreSchemaField, CoreSchemaOrField
     from ._internal._dataclasses import PydanticDataclass
+    from ._internal._schema_generation_shared import GetJsonSchemaFunction, GetJsonSchemaHandler
     from .main import BaseModel
 
 
 CoreSchemaOrFieldType = Literal[core_schema.CoreSchemaType, core_schema.CoreSchemaFieldType]
 """
 A type alias for defined schema types that represents a union of `core_schema.CoreSchemaType` and
 `core_schema.CoreSchemaFieldType`.
@@ -60,16 +63,15 @@
 for validation inputs, or that will be matched by serialization outputs.
 """
 
 _MODE_TITLE_MAPPING: dict[JsonSchemaMode, str] = {'validation': 'Input', 'serialization': 'Output'}
 
 
 def update_json_schema(schema: JsonSchemaValue, updates: dict[str, Any]) -> JsonSchemaValue:
-    """
-    Update a JSON schema by providing a dictionary of updates.
+    """Update a JSON schema by providing a dictionary of updates.
 
     This function sets the provided key-value pairs in the schema and returns the updated schema.
 
     Args:
         schema (JsonSchemaValue): The JSON schema to update.
         updates (dict[str, Any]): A dictionary of key-value pairs to set in the schema.
 
@@ -85,23 +87,23 @@
 A type alias representing the kinds of warnings that can be emitted during JSON schema generation.
 
 See `GenerateJsonSchema.render_warning_message` for more details.
 """
 
 
 class PydanticJsonSchemaWarning(UserWarning):
-    """
-    This class is used to emit warnings produced during JSON schema generation.
+    """This class is used to emit warnings produced during JSON schema generation.
     See the `GenerateJsonSchema.emit_warning` and `GenerateJsonSchema.render_warning_message`
     methods for more details; these can be overridden to control warning behavior.
     """
 
 
 # ##### JSON Schema Generation #####
 DEFAULT_REF_TEMPLATE = '#/$defs/{model}'
+"""The default format string used to generate reference names."""
 
 # There are three types of references relevant to building JSON schemas:
 #   1. core_schema "ref" values; these are not exposed as part of the JSON schema
 #       * these might look like the fully qualified path of a model, its id, or something similar
 CoreRef = NewType('CoreRef', str)
 #   2. keys of the "definitions" object that will eventually go into the JSON schema
 #       * by default, these look like "MyModel", though may change in the presence of collisions
@@ -112,16 +114,15 @@
 JsonRef = NewType('JsonRef', str)
 
 CoreModeRef = Tuple[CoreRef, JsonSchemaMode]
 JsonSchemaKeyT = TypeVar('JsonSchemaKeyT', bound=Hashable)
 
 
 class GenerateJsonSchema:
-    """
-    A class for generating JSON schemas.
+    """A class for generating JSON schemas.
 
     This class generates JSON schemas based on configured parameters. The default schema dialect
     is 'https://json-schema.org/draft/2020-12/schema'. The class uses `by_alias` to configure how fields with
     multiple names are handled and `ref_template` to format reference names.
 
     Attributes:
         schema_dialect (str): The JSON schema dialect used to generate the schema. See
@@ -180,19 +181,26 @@
 
         # This changes to True after generating a schema, to prevent issues caused by accidental re-use
         # of a single instance of a schema generator
         self._used = False
 
         self.mode: JsonSchemaMode = 'validation'
 
+        # When we encounter definitions we need to try to build them immediately
+        # so that they are available schemas that reference them
+        # But it's possible that that CoreSchema was never going to be used
+        # (e.g. because the CoreSchema that references short circuits is JSON schema generation without needing
+        #  the reference) so instead of failing altogether if we can't build a definition we
+        # store the error raised and re-throw it if we end up needing that def
+        self.core_defs_invalid_for_json_schema: dict[DefsRef, PydanticInvalidForJsonSchema] = {}
+
     def build_schema_type_to_method(
         self,
     ) -> dict[CoreSchemaOrFieldType, Callable[[CoreSchemaOrField], JsonSchemaValue]]:
-        """
-        Builds a dictionary mapping `CoreSchemaOrFieldType` to a callable method that generates a `JsonSchema` value
+        """Builds a dictionary mapping `CoreSchemaOrFieldType` to a callable method that generates a `JsonSchema` value
         for a given `CoreSchemaOrField`.
 
         Returns:
             dict: A dictionary containing the mapping of `CoreSchemaOrFieldType` to a callable method.
 
         Raises:
             TypeError: If no method has been defined for generating a JSON schema for a given pydantic core schema type.
@@ -211,16 +219,15 @@
                     f'(expected: {type(self).__name__}.{method_name})'
                 ) from e
         return mapping
 
     def generate_definitions(
         self, inputs: Sequence[tuple[JsonSchemaKeyT, JsonSchemaMode, core_schema.CoreSchema]]
     ) -> tuple[dict[tuple[JsonSchemaKeyT, JsonSchemaMode], DefsRef], dict[DefsRef, JsonSchemaValue]]:
-        """
-        Given a list of core_schema, generates all JSON schema definitions from a list of core schemas, and
+        """Given a list of core_schema, generates all JSON schema definitions from a list of core schemas, and
         returns the generated definitions paired with a mapping from the input keys to the definition references.
 
         Args:
             inputs: A sequence of tuples, where:
 
                 - `JsonSchemaKeyT` will be paired with `JsonSchemaMode` to form the keys of the first returned
                     dictionary.
@@ -257,19 +264,18 @@
             if '$ref' in json_schema:
                 json_ref = cast(JsonRef, json_schema['$ref'])
                 defs_ref = self.json_to_defs_refs.get(json_ref)
                 if defs_ref is not None:
                     refs_map[(key, mode)] = defs_ref
 
         self._used = True
-        return refs_map, self.definitions
+        return refs_map, _sort_json_schema(self.definitions)  # type: ignore
 
     def generate(self, schema: CoreSchema, mode: JsonSchemaMode = 'validation') -> JsonSchemaValue:
-        """
-        Generates a JSON schema for a specified schema in a specified mode.
+        """Generates a JSON schema for a specified schema in a specified mode.
 
         Args:
             schema: A Pydantic model.
             mode: The mode in which to generate the schema. Defaults to 'validation'.
 
         Returns:
             A JSON schema representing the specified schema.
@@ -314,19 +320,18 @@
             json_schema['$defs'] = self.definitions
 
         # For now, we will not set the $schema key. However, if desired, this can be easily added by overriding
         # this method and adding the following line after a call to super().generate(schema):
         # json_schema['$schema'] = self.schema_dialect
 
         self._used = True
-        return json_schema
+        return _sort_json_schema(json_schema)
 
     def generate_inner(self, schema: CoreSchemaOrField) -> JsonSchemaValue:
-        """
-        Generates a JSON schema for a given `CoreSchemaOrField`.
+        """Generates a JSON schema for a given `CoreSchemaOrField`.
 
         Args:
             schema: The given `CoreSchemaOrField` to generate JSON schema for.
 
         Returns:
             The generated JSON schema.
         """
@@ -338,17 +343,37 @@
             core_mode_ref = (core_ref, self.mode)
             if core_mode_ref in self.core_to_defs_refs and self.core_to_defs_refs[core_mode_ref] in self.definitions:
                 return {'$ref': self.core_to_json_refs[core_mode_ref]}
 
         # Generate the JSON schema, accounting for the json_schema_override and core_schema_override
         metadata_handler = _core_metadata.CoreMetadataHandler(schema)
 
+        def populate_defs(core_schema: CoreSchema, json_schema: JsonSchemaValue) -> JsonSchemaValue:
+            if 'ref' in core_schema:
+                core_ref = CoreRef(core_schema['ref'])  # type: ignore[typeddict-item]
+                defs_ref, ref_json_schema = self.get_cache_defs_ref_schema(core_ref)
+                json_ref = JsonRef(ref_json_schema['$ref'])
+                self.json_to_defs_refs[json_ref] = defs_ref
+                # Replace the schema if it's not a reference to itself
+                # What we want to avoid is having the def be just a ref to itself
+                # which is what would happen if we blindly assigned any
+                if json_schema.get('$ref', None) != json_ref:
+                    self.definitions[defs_ref] = json_schema
+                    self.core_defs_invalid_for_json_schema.pop(defs_ref, None)
+                json_schema = ref_json_schema
+            if '$ref' in json_schema and len(json_schema.keys()) > 1:
+                # technically you can't have any other keys next to a "$ref"
+                # but it's an easy mistake to make and not hard to correct automatically here
+                json_schema = json_schema.copy()
+                ref = json_schema.pop('$ref')
+                json_schema = {'allOf': [{'$ref': ref}], **json_schema}
+            return json_schema
+
         def handler_func(schema_or_field: CoreSchemaOrField) -> JsonSchemaValue:
-            """
-            Generate a JSON schema based on the input schema.
+            """Generate a JSON schema based on the input schema.
 
             Args:
                 schema_or_field: The schema data to generate a JSON schema from.
 
             Returns:
                 The generated JSON schema.
 
@@ -357,185 +382,172 @@
             """
             # Generate the core-schema-type-specific bits of the schema generation:
             if _core_utils.is_core_schema(schema_or_field) or _core_utils.is_core_schema_field(schema_or_field):
                 generate_for_schema_type = self._schema_type_to_method[schema_or_field['type']]
                 json_schema = generate_for_schema_type(schema_or_field)
             else:
                 raise TypeError(f'Unexpected schema type: schema={schema_or_field}')
-            # Populate the definitions
-            if 'ref' in schema:
-                core_ref = CoreRef(schema['ref'])  # type: ignore[typeddict-item]
-                defs_ref, ref_json_schema = self.get_cache_defs_ref_schema(core_ref)
-                self.definitions[defs_ref] = json_schema
-                json_schema = ref_json_schema
+            if _core_utils.is_core_schema(schema_or_field):
+                json_schema = populate_defs(schema_or_field, json_schema)
             return json_schema
 
         current_handler = _schema_generation_shared.GenerateJsonSchemaHandler(self, handler_func)
 
         for js_modify_function in metadata_handler.metadata.get('pydantic_js_functions', ()):
 
             def new_handler_func(
                 schema_or_field: CoreSchemaOrField,
-                current_handler: _core_metadata.GetJsonSchemaHandler = current_handler,
-                js_modify_function: _core_metadata.GetJsonSchemaFunction = js_modify_function,
+                current_handler: GetJsonSchemaHandler = current_handler,
+                js_modify_function: GetJsonSchemaFunction = js_modify_function,
             ) -> JsonSchemaValue:
-                return js_modify_function(schema_or_field, current_handler)
+                json_schema = js_modify_function(schema_or_field, current_handler)
+                if _core_utils.is_core_schema(schema_or_field):
+                    json_schema = populate_defs(schema_or_field, json_schema)
+                return json_schema
 
             current_handler = _schema_generation_shared.GenerateJsonSchemaHandler(self, new_handler_func)
 
         return current_handler(schema)
 
     # ### Schema generation methods
     def any_schema(self, schema: core_schema.AnySchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches any value.
+        """Returns a schema that matches any value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         return {}
 
     def none_schema(self, schema: core_schema.NoneSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a `None` value.
+        """Returns a schema that matches a `None` value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         return {'type': 'null'}
 
     def bool_schema(self, schema: core_schema.BoolSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a Boolean value.
+        """Returns a schema that matches a Boolean value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         return {'type': 'boolean'}
 
     def int_schema(self, schema: core_schema.IntSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches an int value.
+        """Returns a schema that matches an int value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         json_schema: dict[str, Any] = {'type': 'integer'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.numeric)
         json_schema = {k: v for k, v in json_schema.items() if v not in {math.inf, -math.inf}}
         return json_schema
 
     def float_schema(self, schema: core_schema.FloatSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a Float value.
+        """Returns a schema that matches a Float value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         json_schema: dict[str, Any] = {'type': 'number'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.numeric)
         json_schema = {k: v for k, v in json_schema.items() if v not in {math.inf, -math.inf}}
         return json_schema
 
     def str_schema(self, schema: core_schema.StringSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a string value.
+        """Returns a schema that matches a string value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         json_schema = {'type': 'string'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.string)
         return json_schema
 
     def bytes_schema(self, schema: core_schema.BytesSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a bytes value.
+        """Returns a schema that matches a bytes value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         json_schema = {'type': 'string', 'format': 'binary'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.bytes)
         return json_schema
 
     def date_schema(self, schema: core_schema.DateSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a date value.
+        """Returns a schema that matches a date value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         json_schema = {'type': 'string', 'format': 'date'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.date)
         return json_schema
 
     def time_schema(self, schema: core_schema.TimeSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a time value.
+        """Returns a schema that matches a time value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         return {'type': 'string', 'format': 'time'}
 
     def datetime_schema(self, schema: core_schema.DatetimeSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a `datetime` value.
+        """Returns a schema that matches a `datetime` value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         return {'type': 'string', 'format': 'date-time'}
 
     def timedelta_schema(self, schema: core_schema.TimedeltaSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a `timedelta` value.
+        """Returns a schema that matches a `timedelta` value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         return {'type': 'string', 'format': 'duration'}
 
     def literal_schema(self, schema: core_schema.LiteralSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a `Literal` value.
+        """Returns a schema that matches a `Literal` value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
@@ -543,68 +555,64 @@
 
         if len(expected) == 1:
             return {'const': expected[0]}
         else:
             return {'enum': expected}
 
     def is_instance_schema(self, schema: core_schema.IsInstanceSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that checks if a value is an instance of a class, equivalent to Python's `isinstance` method.
+        """Returns a schema that checks if a value is an instance of a class, equivalent to Python's `isinstance`
+        method.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         return self.handle_invalid_for_json_schema(schema, f'core_schema.IsInstanceSchema ({schema["cls"]})')
 
     def is_subclass_schema(self, schema: core_schema.IsSubclassSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that checks if a value is a subtype of a class, equivalent to Python's `issubclass` method.
+        """Returns a schema that checks if a value is a subtype of a class, equivalent to Python's `issubclass` method.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         # Note: This is for compatibility with V1; you can override if you want different behavior.
         return {}
 
     def callable_schema(self, schema: core_schema.CallableSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that checks if a value is callable, equivalent to Python's `callable` method.
+        """Returns a schema that checks if a value is callable, equivalent to Python's `callable` method.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         return self.handle_invalid_for_json_schema(schema, 'core_schema.CallableSchema')
 
     def list_schema(self, schema: core_schema.ListSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a `List` value.
+        """Returns a schema that matches a `List` value.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         items_schema = {} if 'items_schema' not in schema else self.generate_inner(schema['items_schema'])
         json_schema = {'type': 'array', 'items': items_schema}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.array)
         return json_schema
 
     def tuple_positional_schema(self, schema: core_schema.TuplePositionalSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a tuple of schemas.
+        """Returns a schema that matches a tuple of schemas.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
@@ -617,45 +625,40 @@
             json_schema['items'] = self.generate_inner(schema['extra_schema'])
         else:
             json_schema['maxItems'] = len(schema['items_schema'])
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.array)
         return json_schema
 
     def tuple_variable_schema(self, schema: core_schema.TupleVariableSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a tuple of a given schema.
+        """Returns a schema that matches a tuple of a given schema.
 
         Args:
             schema: The schema.
 
         Returns:
             JsonSchemaValue: The generated JSON schema.
         """
-        # NOTE: The `items_schema` is always added, even when we explicitly create a
-        # tuple variable schema without an `items_schema`.
-        items = self.generate_inner(schema['items_schema'])  # type: ignore
-        json_schema: JsonSchemaValue = {'type': 'array', 'items': items}
+        items_schema = {} if 'items_schema' not in schema else self.generate_inner(schema['items_schema'])
+        json_schema = {'type': 'array', 'items': items_schema}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.array)
         return json_schema
 
     def set_schema(self, schema: core_schema.SetSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a `Set` schema.
+        """Returns a schema that matches a `Set` schema.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         return self._common_set_schema(schema)
 
     def frozenset_schema(self, schema: core_schema.FrozenSetSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a `frozenset` schema.
+        """Returns a schema that matches a `frozenset` schema.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
@@ -664,31 +667,29 @@
     def _common_set_schema(self, schema: core_schema.SetSchema | core_schema.FrozenSetSchema) -> JsonSchemaValue:
         items_schema = {} if 'items_schema' not in schema else self.generate_inner(schema['items_schema'])
         json_schema = {'type': 'array', 'uniqueItems': True, 'items': items_schema}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.array)
         return json_schema
 
     def generator_schema(self, schema: core_schema.GeneratorSchema) -> JsonSchemaValue:
-        """
-        Returns a JSON schema that represents the provided GeneratorSchema.
+        """Returns a JSON schema that represents the provided GeneratorSchema.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
         items_schema = {} if 'items_schema' not in schema else self.generate_inner(schema['items_schema'])
         json_schema = {'type': 'array', 'items': items_schema}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.array)
         return json_schema
 
     def dict_schema(self, schema: core_schema.DictSchema) -> JsonSchemaValue:
-        """
-        Returns a schema that matches a dict schema.
+        """Returns a schema that matches a dict schema.
 
         Args:
             schema: The schema.
 
         Returns:
             The generated JSON schema.
         """
@@ -731,20 +732,25 @@
 
     def function_wrap_schema(self, schema: core_schema.WrapValidatorFunctionSchema) -> JsonSchemaValue:
         return self._function_schema(schema)
 
     def default_schema(self, schema: core_schema.WithDefaultSchema) -> JsonSchemaValue:
         json_schema = self.generate_inner(schema['schema'])
 
-        if 'default' in schema:
-            default = schema['default']
-        elif 'default_factory' in schema:
-            default = schema['default_factory']()
-        else:  # pragma: no cover
-            raise ValueError('`schema` has neither default nor default_factory')
+        if 'default' not in schema:
+            return json_schema
+        default = schema['default']
+        # Note: if you want to include the value returned by the default_factory,
+        # override this method and replace the code above with:
+        # if 'default' in schema:
+        #     default = schema['default']
+        # elif 'default_factory' in schema:
+        #     default = schema['default_factory']()
+        # else:
+        #     return json_schema
 
         try:
             encoded_default = self.encode_default(default)
         except pydantic_core.PydanticSerializationError:
             self.emit_warning(
                 'non-serializable-default',
                 f'Default value {default} is not JSON serializable; excluding default from JSON schema',
@@ -782,14 +788,16 @@
         if len(generated) == 1:
             return generated[0]
         return self.get_flattened_anyof(generated)
 
     def tagged_union_schema(self, schema: core_schema.TaggedUnionSchema) -> JsonSchemaValue:
         generated: dict[str, JsonSchemaValue] = {}
         for k, v in schema['choices'].items():
+            if isinstance(k, Enum):
+                k = k.value
             if not isinstance(v, (str, int)):
                 try:
                     # Use str(k) since keys must be strings for json; while not technically correct,
                     # it's the closest that can be represented in valid JSON
                     generated[str(k)] = self.generate_inner(v).copy()
                 except PydanticInvalidForJsonSchema as exc:
                     self.emit_warning('skipped-choice', exc.message)
@@ -817,17 +825,16 @@
             }
 
         return json_schema
 
     def _extract_discriminator(
         self, schema: core_schema.TaggedUnionSchema, one_of_choices: list[_JsonDict]
     ) -> str | None:
-        """
-        Extract a compatible OpenAPI discriminator from the schema and one_of choices that end up in the final schema.
-        """
+        """Extract a compatible OpenAPI discriminator from the schema and one_of choices that end up in the final
+        schema."""
         openapi_discriminator: str | None = None
 
         if isinstance(schema['discriminator'], str):
             return schema['discriminator']
 
         if isinstance(schema['discriminator'], list):
             # If the discriminator is a single item list containing a string, that is equivalent to the string case
@@ -861,42 +868,48 @@
 
     def chain_schema(self, schema: core_schema.ChainSchema) -> JsonSchemaValue:
         # Note: If we wanted to generate a schema for the _serialization_, would want to use the _last_ step:
         # There are always more than zero steps, since the ChainSchema is validated on the pydantic-core side.
         return self.generate_inner(schema['steps'][0])
 
     def lax_or_strict_schema(self, schema: core_schema.LaxOrStrictSchema) -> JsonSchemaValue:
-        """
-        LaxOrStrict will use the strict branch for serialization internally,
+        """LaxOrStrict will use the strict branch for serialization internally,
         unless it was overridden here.
         """
         # TODO: Need to read the default value off of model config or whatever
         use_strict = schema.get('strict', False)  # TODO: replace this default False
         # If your JSON schema fails to generate it is probably
         # because one of the following two branches failed.
         if use_strict:
             return self.generate_inner(schema['strict_schema'])
         else:
             return self.generate_inner(schema['lax_schema'])
 
     def json_or_python_schema(self, schema: core_schema.JsonOrPythonSchema) -> JsonSchemaValue:
-        """
-        Always uses the json schema
-        """
+        """Always uses the json schema."""
         return self.generate_inner(schema['json_schema'])
 
     def typed_dict_schema(self, schema: core_schema.TypedDictSchema) -> JsonSchemaValue:
         named_required_fields: list[tuple[str, bool, CoreSchemaField]] = [
             (name, self.field_is_required(field), field)
             for name, field in schema['fields'].items()
             if self.field_is_present(field)
         ]
         if self.mode == 'serialization':
             named_required_fields.extend(self._name_required_computed_fields(schema.get('computed_fields', [])))
-        return self._named_required_fields_schema(named_required_fields)
+        json_schema = self._named_required_fields_schema(named_required_fields)
+        config: CoreConfig | None = schema.get('config', None)
+
+        extra = (config or {}).get('extra_fields_behavior', 'ignore')
+        if extra == 'forbid':
+            json_schema['additionalProperties'] = False
+        elif extra == 'allow':
+            json_schema['additionalProperties'] = True
+
+        return json_schema
 
     @staticmethod
     def _name_required_computed_fields(
         computed_fields: list[ComputedField],
     ) -> list[tuple[str, bool, core_schema.ComputedField]]:
         return [(field['property_name'], True, field) for field in computed_fields]
 
@@ -962,41 +975,42 @@
         # We do not use schema['model'].model_json_schema() here
         # because it could lead to inconsistent refs handling, etc.
         json_schema = self.generate_inner(schema['schema'])
 
         cls = cast('type[BaseModel]', schema['cls'])
         config = cls.model_config
         title = config.get('title')
-        forbid_additional_properties = config.get('extra') == 'forbid'
+
         json_schema_extra = config.get('json_schema_extra')
-        json_schema = self._update_class_schema(
-            json_schema, title, forbid_additional_properties, cls, json_schema_extra
-        )
+        json_schema = self._update_class_schema(json_schema, title, config.get('extra', None), cls, json_schema_extra)
 
         return json_schema
 
     def _update_class_schema(
         self,
         json_schema: JsonSchemaValue,
         title: str | None,
-        forbid_additional_properties: bool,
+        extra: Literal['allow', 'ignore', 'forbid'] | None,
         cls: type[Any],
         json_schema_extra: dict[str, Any] | JsonSchemaExtraCallable | None,
     ) -> JsonSchemaValue:
         if '$ref' in json_schema:
             schema_to_update = self.get_schema_from_definitions(JsonRef(json_schema['$ref'])) or json_schema
         else:
             schema_to_update = json_schema
 
         if title is not None:
             # referenced_schema['title'] = title
             schema_to_update.setdefault('title', title)
 
-        if forbid_additional_properties:
-            schema_to_update['additionalProperties'] = False
+        if 'additionalProperties' not in schema_to_update:
+            if extra == 'allow':
+                schema_to_update['additionalProperties'] = True
+            elif extra == 'forbid':
+                schema_to_update['additionalProperties'] = False
 
         if isinstance(json_schema_extra, (staticmethod, classmethod)):
             # In older versions of python, this is necessary to ensure staticmethod/classmethods are callable
             json_schema_extra = json_schema_extra.__get__(cls)
 
         if isinstance(json_schema_extra, dict):
             schema_to_update.update(json_schema_extra)
@@ -1008,43 +1022,56 @@
         elif json_schema_extra is not None:
             raise ValueError(
                 f"model_config['json_schema_extra']={json_schema_extra} should be a dict, callable, or None"
             )
 
         return json_schema
 
+    def resolve_schema_to_update(self, json_schema: JsonSchemaValue) -> JsonSchemaValue:
+        """Resolve a JsonSchemaValue to the non-ref schema if it is a $ref schema"""
+        if '$ref' in json_schema:
+            schema_to_update = self.get_schema_from_definitions(JsonRef(json_schema['$ref']))
+            if schema_to_update is None:
+                raise RuntimeError(f'Cannot update undefined schema for $ref={json_schema["$ref"]}')
+            return self.resolve_schema_to_update(schema_to_update)
+        else:
+            schema_to_update = json_schema
+        return schema_to_update
+
     def model_fields_schema(self, schema: core_schema.ModelFieldsSchema) -> JsonSchemaValue:
         named_required_fields: list[tuple[str, bool, CoreSchemaField]] = [
             (name, self.field_is_required(field), field)
             for name, field in schema['fields'].items()
             if self.field_is_present(field)
         ]
         if self.mode == 'serialization':
             named_required_fields.extend(self._name_required_computed_fields(schema.get('computed_fields', [])))
-        return self._named_required_fields_schema(named_required_fields)
+        json_schema = self._named_required_fields_schema(named_required_fields)
+        extra_validator = schema.get('extra_validator', None)
+        if extra_validator is not None:
+            schema_to_update = self.resolve_schema_to_update(json_schema)
+            schema_to_update['additionalProperties'] = self.generate_inner(extra_validator)
+        return json_schema
 
     def field_is_present(self, field: CoreSchemaField) -> bool:
-        """
-        Whether the field should be included in the generated JSON schema
-        """
+        """Whether the field should be included in the generated JSON schema."""
         if self.mode == 'serialization':
             # If you still want to include the field in the generated JSON schema,
             # override this method and return True
             return not field.get('serialization_exclude')
         elif self.mode == 'validation':
             return True
         else:
             assert_never(self.mode)
 
     def field_is_required(
         self, field: core_schema.ModelField | core_schema.DataclassField | core_schema.TypedDictField
     ) -> bool:
-        """
-        Whether the field should be marked as required in the generated JSON schema.
-        (Note that this is irrelevant if the field is not present in the JSON schema.)
+        """Whether the field should be marked as required in the generated JSON schema.
+        (Note that this is irrelevant if the field is not present in the JSON schema.).
         """
         if self.mode == 'serialization':
             return not field.get('serialization_exclude')
         elif self.mode == 'validation':
             if field['type'] == 'typed-dict-field':
                 return field['required']  # type: ignore  # required is always populated
             else:
@@ -1065,19 +1092,17 @@
     def dataclass_schema(self, schema: core_schema.DataclassSchema) -> JsonSchemaValue:
         json_schema = self.generate_inner(schema['schema']).copy()
 
         cls = schema['cls']
         config: ConfigDict = getattr(cls, '__pydantic_config__', cast('ConfigDict', {}))
 
         title = config.get('title') or cls.__name__
-        forbid_additional_properties = config.get('extra') == 'forbid'
+
         json_schema_extra = config.get('json_schema_extra')
-        json_schema = self._update_class_schema(
-            json_schema, title, forbid_additional_properties, cls, json_schema_extra
-        )
+        json_schema = self._update_class_schema(json_schema, title, config.get('extra', None), cls, json_schema_extra)
 
         # Dataclass-specific handling of description
         if is_dataclass(cls) and not hasattr(cls, '__pydantic_validator__'):
             # vanilla dataclass; don't use cls.__doc__ as it will contain the class signature by default
             description = None
         else:
             description = None if cls.__doc__ is None else inspect.cleandoc(cls.__doc__)
@@ -1212,30 +1237,35 @@
         # Note: 'multi-host-uri' is a custom/pydantic-specific format, not part of the JSON Schema spec
         json_schema = {'type': 'string', 'format': 'multi-host-uri', 'minLength': 1}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.string)
         return json_schema
 
     def definitions_schema(self, schema: core_schema.DefinitionsSchema) -> JsonSchemaValue:
         for definition in schema['definitions']:
-            self.generate_inner(definition)
-        return self.generate_inner(schema['schema'])
+            try:
+                self.generate_inner(definition)
+            except PydanticInvalidForJsonSchema as e:
+                core_ref: CoreRef = CoreRef(definition['ref'])  # type: ignore
+                self.core_defs_invalid_for_json_schema[self.get_defs_ref((core_ref, self.mode))] = e
+                continue
+        res = self.generate_inner(schema['schema'])
+        return res
 
     def definition_ref_schema(self, schema: core_schema.DefinitionReferenceSchema) -> JsonSchemaValue:
         core_ref = CoreRef(schema['schema_ref'])
         _, ref_json_schema = self.get_cache_defs_ref_schema(core_ref)
         return ref_json_schema
 
     # ### Utility methods
 
     def get_title_from_name(self, name: str) -> str:
         return name.title().replace('_', ' ')
 
     def field_title_should_be_set(self, schema: CoreSchemaOrField) -> bool:
-        """
-        Returns true if a field with the given schema should have a title set based on the field name.
+        """Returns true if a field with the given schema should have a title set based on the field name.
 
         Intuitively, we want this to return true for schemas that wouldn't otherwise provide their own title
         (e.g., int, float, str), and false for those that would (e.g., BaseModel subclasses).
         """
         if _core_utils.is_core_schema_field(schema):
             if schema['type'] == 'computed-field':
                 field_schema = schema['return_schema']
@@ -1259,17 +1289,15 @@
         else:
             raise PydanticInvalidForJsonSchema(f'Unexpected schema type: schema={schema}')  # pragma: no cover
 
     def normalize_name(self, name: str) -> str:
         return re.sub(r'[^a-zA-Z0-9.\-_]', '_', name).replace('.', '__')
 
     def get_defs_ref(self, core_mode_ref: CoreModeRef) -> DefsRef:
-        """
-        Override this method to change the way that definitions keys are generated from a core reference.
-        """
+        """Override this method to change the way that definitions keys are generated from a core reference."""
         # Split the core ref into "components"; generic origins and arguments are each separate components
         core_ref, mode = core_mode_ref
         components = re.split(r'([\][,])', core_ref)
         # Remove IDs from each component
         components = [x.split(':')[0] for x in components]
         core_ref_no_id = ''.join(components)
         # Remove everything before the last period from each "component"
@@ -1296,16 +1324,15 @@
                 return choice
             else:
                 self.collisions.add(choice)
 
         return choices[-1]  # should never get here if the final choice is guaranteed unique
 
     def resolve_collisions(self, json_schema: JsonSchemaValue) -> JsonSchemaValue:
-        """
-        This function ensures that any defs_ref's that were involved in collisions
+        """This function ensures that any defs_ref's that were involved in collisions
         (due to simplification of the core_ref) get updated, even if they were the
         first occurrence of the colliding defs_ref.
 
         This is intended to prevent confusion where the type that gets the "shortened"
         ref depends on the order in which the types were visited.
         """
         made_changes = True
@@ -1346,17 +1373,15 @@
         self.defs_to_core_refs[new] = self.defs_to_core_refs.pop(old)
         assert self.json_to_defs_refs.pop(old_json_ref) == old
         self.json_to_defs_refs[new_json_ref] = new
         self.core_to_defs_refs[core_mode_ref] = new
         self.core_to_json_refs[core_mode_ref] = new_json_ref
 
         def walk_replace_json_schema_ref(item: Any) -> Any:
-            """
-            Recursively update the JSON schema to use the new defs_ref.
-            """
+            """Recursively update the JSON schema to use the new defs_ref."""
             if isinstance(item, list):
                 return [walk_replace_json_schema_ref(item) for item in item]
             elif isinstance(item, dict):
                 ref = item.get('$ref')
                 if ref == old_json_ref:
                     item['$ref'] = new_json_ref
                 return {k: walk_replace_json_schema_ref(v) for k, v in item.items()}
@@ -1365,16 +1390,15 @@
 
         for k, v in self.definitions.items():
             self.definitions[k] = walk_replace_json_schema_ref(v)
 
         return walk_replace_json_schema_ref(json_schema)
 
     def get_cache_defs_ref_schema(self, core_ref: CoreRef) -> tuple[DefsRef, JsonSchemaValue]:
-        """
-        This method wraps the get_defs_ref method with some cache-lookup/population logic,
+        """This method wraps the get_defs_ref method with some cache-lookup/population logic,
         and returns both the produced defs_ref and the JSON schema that will refer to the right definition.
         """
         core_mode_ref = (core_ref, self.mode)
         maybe_defs_ref = self.core_to_defs_refs.get(core_mode_ref)
         if maybe_defs_ref is not None:
             json_ref = self.core_to_json_refs[core_mode_ref]
             return maybe_defs_ref, {'$ref': json_ref}
@@ -1388,16 +1412,15 @@
         json_ref = JsonRef(self.ref_template.format(model=defs_ref))
         self.core_to_json_refs[core_mode_ref] = json_ref
         self.json_to_defs_refs[json_ref] = defs_ref
         ref_json_schema = {'$ref': json_ref}
         return defs_ref, ref_json_schema
 
     def handle_ref_overrides(self, json_schema: JsonSchemaValue) -> JsonSchemaValue:
-        """
-        It is not valid for a schema with a top-level $ref to have sibling keys.
+        """It is not valid for a schema with a top-level $ref to have sibling keys.
 
         During our own schema generation, we treat sibling keys as overrides to the referenced schema,
         but this is not how the official JSON schema spec works.
 
         Because of this, we first remove any sibling keys that are redundant with the referenced schema, then if
         any remain, we transform the schema from a top-level '$ref' to use allOf to move the $ref out of the top level.
         (See bottom of https://swagger.io/docs/specification/using-ref/ for a reference about this behavior)
@@ -1430,33 +1453,34 @@
                 del json_schema['$ref']
                 assert 'allOf' not in json_schema  # this should never happen, but just in case
                 json_schema['allOf'] = [{'$ref': json_ref}]
 
         return json_schema
 
     def get_schema_from_definitions(self, json_ref: JsonRef) -> JsonSchemaValue | None:
-        return self.definitions.get(self.json_to_defs_refs[json_ref])
+        def_ref = self.json_to_defs_refs[json_ref]
+        if def_ref in self.core_defs_invalid_for_json_schema:
+            raise self.core_defs_invalid_for_json_schema[def_ref]
+        return self.definitions.get(def_ref, None)
 
     def encode_default(self, dft: Any) -> Any:
         return pydantic_core.to_jsonable_python(dft)
 
     def update_with_validations(
         self, json_schema: JsonSchemaValue, core_schema: CoreSchema, mapping: dict[str, str]
     ) -> None:
-        """
-        Update the json_schema with the corresponding validations specified in the core_schema,
+        """Update the json_schema with the corresponding validations specified in the core_schema,
         using the provided mapping to translate keys in core_schema to the appropriate keys for a JSON schema.
         """
         for core_key, json_schema_key in mapping.items():
             if core_key in core_schema:
                 json_schema[json_schema_key] = core_schema[core_key]  # type: ignore[literal-required]
 
     class ValidationsMapping:
-        """
-        This class just contains mappings from core_schema attribute names to the corresponding
+        """This class just contains mappings from core_schema attribute names to the corresponding
         JSON schema attribute names. While I suspect it is unlikely to be necessary, you can in
         principle override this class in a subclass of GenerateJsonSchema (by inheriting from
         GenerateJsonSchema.ValidationsMapping) to change these mappings.
         """
 
         numeric = {
             'multiple_of': 'multipleOf',
@@ -1498,51 +1522,49 @@
                 members.append(schema)
         members = _deduplicate_schemas(members)
         if len(members) == 1:
             return members[0]
         return {'anyOf': members}
 
     def get_json_ref_counts(self, json_schema: JsonSchemaValue) -> dict[JsonRef, int]:
-        """
-        Get all values corresponding to the key '$ref' anywhere in the json_schema
-        """
+        """Get all values corresponding to the key '$ref' anywhere in the json_schema."""
         json_refs: dict[JsonRef, int] = Counter()
 
         def _add_json_refs(schema: Any) -> None:
             if isinstance(schema, dict):
                 if '$ref' in schema:
                     json_ref = JsonRef(schema['$ref'])
                     already_visited = json_ref in json_refs
                     json_refs[json_ref] += 1
                     if already_visited:
                         return  # prevent recursion on a definition that was already visited
-                    _add_json_refs(self.definitions[self.json_to_defs_refs[json_ref]])
+                    def_ref = self.json_to_defs_refs[json_ref]
+                    if def_ref in self.core_defs_invalid_for_json_schema:
+                        raise self.core_defs_invalid_for_json_schema[def_ref]
+                    _add_json_refs(self.definitions[def_ref])
                 for v in schema.values():
                     _add_json_refs(v)
             elif isinstance(schema, list):
                 for v in schema:
                     _add_json_refs(v)
 
         _add_json_refs(json_schema)
         return json_refs
 
     def handle_invalid_for_json_schema(self, schema: CoreSchemaOrField, error_info: str) -> JsonSchemaValue:
         raise PydanticInvalidForJsonSchema(f'Cannot generate a JsonSchema for {error_info}')
 
     def emit_warning(self, kind: JsonSchemaWarningKind, detail: str) -> None:
-        """
-        This method simply emits PydanticJsonSchemaWarnings based on handling in the `warning_message` method.
-        """
+        """This method simply emits PydanticJsonSchemaWarnings based on handling in the `warning_message` method."""
         message = self.render_warning_message(kind, detail)
         if message is not None:
             warnings.warn(message, PydanticJsonSchemaWarning)
 
     def render_warning_message(self, kind: JsonSchemaWarningKind, detail: str) -> str | None:
-        """
-        This method is responsible for ignoring warnings as desired, and for formatting the warning messages.
+        """This method is responsible for ignoring warnings as desired, and for formatting the warning messages.
 
         You can override the value of `ignored_warning_kinds` in a subclass of GenerateJsonSchema
         to modify what warnings are generated. If you want more control, you can override this method;
         just return None in situations where you don't want warnings to be emitted.
         """
         if kind in self.ignored_warning_kinds:
             return None
@@ -1619,7 +1641,78 @@
 def _make_json_hashable(value: _Json) -> _HashableJson:
     if isinstance(value, dict):
         return tuple(sorted((k, _make_json_hashable(v)) for k, v in value.items()))
     elif isinstance(value, list):
         return tuple(_make_json_hashable(v) for v in value)
     else:
         return value
+
+
+def _sort_json_schema(value: JsonSchemaValue) -> JsonSchemaValue:
+    if isinstance(value, dict):  # type: ignore
+        sorted_dict: dict[str, JsonSchemaValue] = {}
+        for key in sorted(value.keys()):
+            sorted_dict[key] = _sort_json_schema(value[key])
+        return sorted_dict  # type: ignore
+    elif isinstance(value, list):  # type: ignore
+        sorted_list: list[JsonSchemaValue] = []
+        for item in value:  # type: ignore
+            sorted_list.append(_sort_json_schema(item))
+        return sorted_list  # type: ignore
+    else:
+        return value
+
+
+@_internal_dataclass.slots_dataclass
+class WithJsonSchema:
+    """Add this as an annotation on a field to override the (base) JSON schema that would be generated for that field.
+    This provides a way to set a JSON schema for types that would otherwise raise errors when producing a JSON schema,
+    such as Callable, or types that have an is-instance core schema, without needing to go so far as creating a
+    custom subclass of pydantic.json_schema.GenerateJsonSchema.
+    Note that any _modifications_ to the schema that would normally be made (such as setting the title for model fields)
+    will still be performed.
+
+    If `mode` is set this will only apply to that schema generation mode, allowing you
+    to set different json schemas for validation and serialization.
+    """
+
+    json_schema: JsonSchemaValue | None
+    mode: Literal['validation', 'serialization'] | None = None
+
+    def __get_pydantic_json_schema__(
+        self, core_schema: core_schema.CoreSchema, handler: _annotated_handlers.GetJsonSchemaHandler
+    ) -> JsonSchemaValue:
+        mode = self.mode or handler.mode
+        if mode != handler.mode:
+            return handler(core_schema)
+        if self.json_schema is None:
+            # This exception is handled in pydantic.json_schema.GenerateJsonSchema._named_required_fields_schema
+            raise PydanticOmit
+        else:
+            return self.json_schema
+
+
+@_internal_dataclass.slots_dataclass
+class Examples:
+    """Add examples to a JSON schema.
+
+    Examples should be a map of example names (strings)
+    to example values (any valid JSON).
+
+    If `mode` is set this will only apply to that schema generation mode,
+    allowing you to add different examples for validation and serialization.
+    """
+
+    examples: dict[str, Any]
+    mode: Literal['validation', 'serialization'] | None = None
+
+    def __get_pydantic_json_schema__(
+        self, core_schema: core_schema.CoreSchema, handler: _annotated_handlers.GetJsonSchemaHandler
+    ) -> JsonSchemaValue:
+        mode = self.mode or handler.mode
+        json_schema = handler(core_schema)
+        if mode != handler.mode:
+            return json_schema
+        examples = json_schema.get('examples', {})
+        examples.update(to_jsonable_python(self.examples))
+        json_schema['examples'] = examples
+        return json_schema
```

### Comparing `pydantic-2.0b2/pydantic/main.py` & `pydantic-2.0b3/pydantic/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Logic for creating models.
-"""
+"""Logic for creating models."""
 from __future__ import annotations as _annotations
 
 import types
 import typing
 import warnings
 from copy import copy, deepcopy
 from typing import Any
@@ -15,14 +13,15 @@
 from ._internal import (
     _annotated_handlers,
     _config,
     _decorators,
     _fields,
     _forward_ref,
     _generics,
+    _mock_validator,
     _model_construction,
     _repr,
     _typing_extra,
     _utils,
 )
 from ._migration import getattr_migration
 from .config import ConfigDict
@@ -50,46 +49,48 @@
 
     AnyClassMethod = classmethod[Any, Any, Any]
     TupleGenerator = typing.Generator[typing.Tuple[str, Any], None, None]
     Model = typing.TypeVar('Model', bound='BaseModel')
     # should be `set[int] | set[str] | dict[int, IncEx] | dict[str, IncEx] | None`, but mypy can't cope
     IncEx: typing_extensions.TypeAlias = 'set[int] | set[str] | dict[int, Any] | dict[str, Any] | None'
 
-__all__ = 'BaseModel', 'RootModel', 'create_model'
+__all__ = 'BaseModel', 'create_model'
 
 _object_setattr = _model_construction.object_setattr
 _Undefined = _fields.Undefined
 
 
 class BaseModel(metaclass=_model_construction.ModelMetaclass):
-    """
-    A base model class for creating Pydantic models.
+    """A base model class for creating Pydantic models.
 
     * `model_fields` is a class attribute that contains the fields defined on the model in Pydantic V2.
         This replaces `Model.__fields__` from Pydantic V1.
     *  `__pydantic_decorators__` contains the decorators defined on the model in Pydantic V2. This replaces
         `Model.__validators__` and `Model.__root_validators__` from Pydantic V1.
 
     Attributes:
+        model_fields: Fields in the model.
+        model_config: Configuration settings for the model.
         __pydantic_validator__: Validator for checking schema validity.
         __pydantic_core_schema__: Schema for representing the model's core.
         __pydantic_serializer__: Serializer for the schema.
         __pydantic_decorators__: Metadata for `@field_validator`, `@root_validator`,
             and `@serializer` decorators.
-        model_fields: Fields in the model.
         __signature__: Signature for instantiating the model.
         __private_attributes__: Private attributes of the model.
         __class_vars__: Class variables of the model.
         __pydantic_fields_set__: Set of fields in the model.
         __pydantic_extra__: Extra fields in the model.
         __pydantic_private__: Private fields in the model.
         __pydantic_generic_metadata__: Metadata for generic models.
         __pydantic_parent_namespace__: Parent namespace of the model.
         __pydantic_custom_init__: Custom init of the model.
         __pydantic_post_init__: Post init of the model.
+        __pydantic_complete__: Whether model building is completed.
+        __pydantic_root_model__: Whether the model is a RootModel.
     """
 
     if typing.TYPE_CHECKING:
         # populated by the metaclass, defined here to help IDEs only
         __pydantic_validator__: typing.ClassVar[SchemaValidator]
         __pydantic_core_schema__: typing.ClassVar[CoreSchema]
         __pydantic_serializer__: typing.ClassVar[SchemaSerializer]
@@ -111,27 +112,26 @@
         __pydantic_custom_init__: typing.ClassVar[bool]
         __pydantic_post_init__: typing.ClassVar[None | Literal['model_post_init']]
     else:
         # `model_fields` and `__pydantic_decorators__` must be set for
         # pydantic._internal._generate_schema.GenerateSchema.model_schema to work for a plain BaseModel annotation
         model_fields = {}
         __pydantic_decorators__ = _decorators.DecoratorInfos()
-        __pydantic_validator__ = _model_construction.MockValidator(
+        __pydantic_validator__ = _mock_validator.MockValidator(
             'Pydantic models should inherit from BaseModel, BaseModel cannot be instantiated directly',
             code='base-model-instantiated',
         )
 
     model_config = ConfigDict()
     __slots__ = '__dict__', '__pydantic_fields_set__', '__pydantic_extra__', '__pydantic_private__'
     __pydantic_complete__ = False
     __pydantic_root_model__: typing.ClassVar[bool] = False
 
     def __init__(__pydantic_self__, **data: Any) -> None:  # type: ignore
-        """
-        Create a new model by parsing and validating input data from keyword arguments.
+        """Create a new model by parsing and validating input data from keyword arguments.
 
         Raises ValidationError if the input data cannot be parsed to form a valid model.
 
         Uses something other than `self` for the first arg to allow "self" as a field name.
         """
         # `__tracebackhide__` tells pytest and some other tools to omit this function from tracebacks
         __tracebackhide__ = True
@@ -189,16 +189,15 @@
             A JSON schema, as a Python object.
         """
         return __handler(__core_schema)
 
     if typing.TYPE_CHECKING:
 
         def __init_subclass__(cls, **kwargs: Unpack[ConfigDict]):
-            """
-            This signature is included purely to help type-checkers check arguments to class declaration, which
+            """This signature is included purely to help type-checkers check arguments to class declaration, which
             provides a way to conveniently set model_config key/value pairs:
 
             ```py
             class MyModel(BaseModel, extra='allow'):
                 ...
             ```
 
@@ -208,16 +207,15 @@
 
             Args:
                 **kwargs: Keyword arguments passed to the class definition, which set model_config
             """
 
     @classmethod
     def __pydantic_init_subclass__(cls, **kwargs: Any) -> None:
-        """
-        This is intended to behave just like `__init_subclass__`, but is called by `ModelMetaclass`
+        """This is intended to behave just like `__init_subclass__`, but is called by `ModelMetaclass`
         only after the class is actually fully initialized. In particular, attributes like `model_fields` will
         be present when this is called.
 
         This is necessary because `__init_subclass__` will always be called by `type.__new__`,
         and it would require a prohibitively large refactor to the `ModelMetaclass` to ensure that
         `type.__new__` was called in such a manner that the class would already be sufficiently initialized.
 
@@ -238,19 +236,18 @@
         strict: bool | None = None,
         from_attributes: bool | None = None,
         context: dict[str, Any] | None = None,
     ) -> Model:
         """Validate a pydantic model instance.
 
         Args:
-            cls: The model class to use.
             obj: The object to validate.
-            strict: Whether to raise an exception on invalid fields. Defaults to None.
-            from_attributes: Whether to extract data from object attributes. Defaults to None.
-            context: Additional context to pass to the validator. Defaults to None.
+            strict: Whether to raise an exception on invalid fields.
+            from_attributes: Whether to extract data from object attributes.
+            context: Additional context to pass to the validator.
 
         Raises:
             ValidationError: If the object could not be validated.
 
         Returns:
             The validated model instance.
         """
@@ -258,83 +255,78 @@
         __tracebackhide__ = True
         return cls.__pydantic_validator__.validate_python(
             obj, strict=strict, from_attributes=from_attributes, context=context
         )
 
     @property
     def model_fields_set(self) -> set[str]:
-        """
-        Returns the set of fields that have been set on this model instance.
+        """Returns the set of fields that have been set on this model instance.
 
         Returns:
             A set of strings representing the fields that have been set,
                 i.e. that were not filled from defaults.
         """
         return self.__pydantic_fields_set__
 
     @property
     def model_extra(self) -> dict[str, Any] | None:
-        """
-        Get extra fields set during validation.
+        """Get extra fields set during validation.
 
         Returns:
             A dictionary of extra fields, or `None` if `config.extra` is not set to `"allow"`.
         """
         return self.__pydantic_extra__
 
     @property
     def model_computed_fields(self) -> dict[str, ComputedFieldInfo]:
-        """
-        Get the computed fields of this model instance.
+        """Get the computed fields of this model instance.
 
         Returns:
             A dictionary of computed field names and their corresponding `ComputedFieldInfo` objects.
         """
         return {k: v.info for k, v in self.__pydantic_decorators__.computed_fields.items()}
 
     @classmethod
     def model_validate_json(
         cls: type[Model],
         json_data: str | bytes | bytearray,
         *,
         strict: bool | None = None,
         context: dict[str, Any] | None = None,
     ) -> Model:
-        """
-        Validate the given JSON data against the Pydantic model.
+        """Validate the given JSON data against the Pydantic model.
 
         Args:
             json_data: The JSON data to validate.
-            strict: Whether to enforce types strictly (default: `None`).
-            context: Extra variables to pass to the validator (default: `None`).
+            strict: Whether to enforce types strictly.
+            context: Extra variables to pass to the validator.
 
         Returns:
             The validated Pydantic model.
 
         Raises:
             ValueError: If `json_data` is not a JSON string.
         """
         # `__tracebackhide__` tells pytest and some other tools to omit this function from tracebacks
         __tracebackhide__ = True
         return cls.__pydantic_validator__.validate_json(json_data, strict=strict, context=context)
 
     def model_post_init(self, __context: Any) -> None:
-        """
-        Override this method to perform additional initialization after `__init__` and `model_construct`.
+        """Override this method to perform additional initialization after `__init__` and `model_construct`.
         This is useful if you want to do some validation that requires the entire model to be initialized.
         """
         pass
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name in self.__class_vars__:
             raise AttributeError(
                 f'"{name}" is a ClassVar of `{self.__class__.__name__}` and cannot be set on an instance. '
                 f'If you want to set a value on the class, use `{self.__class__.__name__}.{name} = value`.'
             )
-        elif name.startswith('_'):
+        elif not _fields.is_valid_field_name(name):
             if self.__pydantic_private__ is None or name not in self.__private_attributes__:
                 _object_setattr(self, name, value)
             else:
                 attribute = self.__private_attributes__[name]
                 if hasattr(attribute, '__set__'):
                     attribute.__set__(self, value)  # type: ignore
                 else:
@@ -386,27 +378,26 @@
         by_alias: bool = False,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
         round_trip: bool = False,
         warnings: bool = True,
     ) -> dict[str, Any]:
-        """
-        Generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
+        """Generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
 
         Args:
             mode: The mode in which `to_python` should run.
                 If mode is 'json', the dictionary will only contain JSON serializable types.
                 If mode is 'python', the dictionary may contain any Python objects.
             include: A list of fields to include in the output.
             exclude: A list of fields to exclude from the output.
             by_alias: Whether to use the field's alias in the dictionary key if defined.
             exclude_unset: Whether to exclude fields that are unset or None from the output.
             exclude_defaults: Whether to exclude fields that are set to their default value from the output.
-            exclude_none: Whether to exclude fields that have a value of None from the output.
+            exclude_none: Whether to exclude fields that have a value of `None` from the output.
             round_trip: Whether to enable serialization and deserialization round-trip support.
             warnings: Whether to log warnings when invalid fields are encountered.
 
         Returns:
             A dictionary representation of the model.
         """
         return self.__pydantic_serializer__.to_python(
@@ -431,27 +422,26 @@
         by_alias: bool = False,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
         round_trip: bool = False,
         warnings: bool = True,
     ) -> str:
-        """
-        Generates a JSON representation of the model using Pydantic's `to_json` method.
+        """Generates a JSON representation of the model using Pydantic's `to_json` method.
 
         Args:
             indent: Indentation to use in the JSON output. If None is passed, the output will be compact.
             include: Field(s) to include in the JSON output. Can take either a string or set of strings.
             exclude: Field(s) to exclude from the JSON output. Can take either a string or set of strings.
-            by_alias: Whether to serialize using field aliases. Defaults to False.
-            exclude_unset: Whether to exclude fields that have not been explicitly set. Defaults to False.
-            exclude_defaults: Whether to exclude fields that have the default value. Defaults to False.
-            exclude_none: Whether to exclude fields that have a value of None. Defaults to False.
-            round_trip: Whether to use serialization/deserialization between JSON and class instance. Defaults to False.
-            warnings: Whether to show any warnings that occurred during serialization. Defaults to True.
+            by_alias: Whether to serialize using field aliases.
+            exclude_unset: Whether to exclude fields that have not been explicitly set.
+            exclude_defaults: Whether to exclude fields that have the default value.
+            exclude_none: Whether to exclude fields that have a value of `None`.
+            round_trip: Whether to use serialization/deserialization between JSON and class instance.
+            warnings: Whether to show any warnings that occurred during serialization.
 
         Returns:
             A JSON string representation of the model.
         """
         return self.__pydantic_serializer__.to_json(
             self,
             indent=indent,
@@ -463,48 +453,49 @@
             exclude_none=exclude_none,
             round_trip=round_trip,
             warnings=warnings,
         ).decode()
 
     @classmethod
     def model_construct(cls: type[Model], _fields_set: set[str] | None = None, **values: Any) -> Model:
-        """
-        Creates a new instance of the `Model` class with validated data.
+        """Creates a new instance of the `Model` class with validated data.
 
         Creates a new model setting `__dict__` and `__pydantic_fields_set__` from trusted or pre-validated data.
         Default values are respected, but no other validation is performed.
         Behaves as if `Config.extra = 'allow'` was set since it adds all passed values
 
         Args:
-            cls: The `Model` class.
             _fields_set: The set of field names accepted for the Model instance.
             values: Trusted or pre-validated data dictionary.
 
         Returns:
             A new instance of the `Model` class with validated data.
         """
         m = cls.__new__(cls)
         fields_values: dict[str, Any] = {}
+        defaults: dict[str, Any] = {}  # keeping this separate from `fields_values` helps us compute `_fields_set`
         for name, field in cls.model_fields.items():
             if field.alias and field.alias in values:
-                fields_values[name] = values[field.alias]
+                fields_values[name] = values.pop(field.alias)
             elif name in values:
-                fields_values[name] = values[name]
+                fields_values[name] = values.pop(name)
             elif not field.is_required():
-                fields_values[name] = field.get_default(call_default_factory=True)
+                defaults[name] = field.get_default(call_default_factory=True)
+        if _fields_set is None:
+            _fields_set = set(fields_values.keys())
+        fields_values.update(defaults)
+
         _extra: dict[str, Any] | None = None
         if cls.model_config.get('extra') == 'allow':
             _extra = {}
             for k, v in values.items():
                 _extra[k] = v
         else:
             fields_values.update(values)
         _object_setattr(m, '__dict__', fields_values)
-        if _fields_set is None:
-            _fields_set = set(values.keys())
         _object_setattr(m, '__pydantic_fields_set__', _fields_set)
         _object_setattr(m, '__pydantic_extra__', _extra)
 
         if cls.__pydantic_post_init__:
             m.model_post_init(None)
         else:
             # Note: if there are any private attributes, cls.__pydantic_post_init__ would exist
@@ -517,54 +508,55 @@
     def model_json_schema(
         cls,
         by_alias: bool = True,
         ref_template: str = DEFAULT_REF_TEMPLATE,
         schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
         mode: JsonSchemaMode = 'validation',
     ) -> dict[str, Any]:
-        """
-        Generates a JSON schema for a model class.
+        """Generates a JSON schema for a model class.
 
         To override the logic used to generate the JSON schema, you can create a subclass of `GenerateJsonSchema`
         with your desired modifications, then override this method on a custom base class and set the default
         value of `schema_generator` to be your subclass.
 
         Args:
-            by_alias: Whether to use attribute aliases or not. Defaults to `True`.
-            ref_template: The reference template. Defaults to `DEFAULT_REF_TEMPLATE`.
-            schema_generator: The JSON schema generator. Defaults to `GenerateJsonSchema`.
+            by_alias: Whether to use attribute aliases or not.
+            ref_template: The reference template.
+            schema_generator: The JSON schema generator.
 
         Returns:
-            The JSON schema for the given `cls` model class.
+            The JSON schema for the given model class.
         """
         return model_json_schema(
             cls, by_alias=by_alias, ref_template=ref_template, schema_generator=schema_generator, mode=mode
         )
 
     @classmethod
     def model_rebuild(
         cls,
         *,
         force: bool = False,
         raise_errors: bool = True,
         _parent_namespace_depth: int = 2,
         _types_namespace: dict[str, Any] | None = None,
     ) -> bool | None:
-        """
-        Tries to rebuild or reconstruct the model core schema.
+        """Try to rebuild the pydantic-core schema for the model.
+
+        This may be necessary when one of the annotations is a ForwardRef which could not be resolved during
+        the initial attempt to build the schema, and automatic rebuilding fails.
 
         Args:
             force: Whether to force the rebuilding of the model schema, defaults to `False`.
             raise_errors: Whether to raise errors, defaults to `True`.
             _parent_namespace_depth: The depth level of the parent namespace, defaults to 2.
             _types_namespace: The types namespace, defaults to `None`.
 
         Returns:
-            Returns `None` if model schema is complete and no rebuilding is required.
-                If rebuilding _is_ required, returns `True` if rebuilding was successful, otherwise `False`.
+            Returns `None` if the schema is already "complete" and rebuilding was not required.
+            If rebuilding _was_ required, returns `True` if rebuilding was successful, otherwise `False`.
         """
         if not force and cls.__pydantic_complete__:
             return None
         else:
             if _types_namespace is not None:
                 types_namespace: dict[str, Any] | None = _types_namespace.copy()
             else:
@@ -581,17 +573,15 @@
                 cls.__name__,
                 _config.ConfigWrapper(cls.model_config, check=False),
                 raise_errors=raise_errors,
                 types_namespace=types_namespace,
             )
 
     def __iter__(self) -> TupleGenerator:
-        """
-        so `dict(model)` works
-        """
+        """So `dict(model)` works."""
         yield from self.__dict__.items()
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, BaseModel):
             # When comparing instances of generic types for equality, as long as all field values are equal,
             # only require their generic origin types to be equal, rather than exact type equality.
             # This prevents headaches like MyGeneric(x=1) != MyGeneric[Any](x=1).
@@ -604,16 +594,15 @@
                 and self.__pydantic_private__ == other.__pydantic_private__
                 and self.__pydantic_extra__ == other.__pydantic_extra__
             )
         else:
             return NotImplemented  # delegate to the other item in the comparison
 
     def model_copy(self: Model, *, update: dict[str, Any] | None = None, deep: bool = False) -> Model:
-        """
-        Returns a copy of the model.
+        """Returns a copy of the model.
 
         Args:
             update: Values to change/add in the new model. Note: the data is not validated
                 before creating the new model. You should trust this data.
             deep: Set to `True` to make a deep copy of the model.
 
         Returns:
@@ -631,17 +620,15 @@
                         copied.__pydantic_extra__[k] = v
             else:
                 copied.__dict__.update(update)
             copied.__pydantic_fields_set__.update(update.keys())
         return copied
 
     def __copy__(self: Model) -> Model:
-        """
-        Returns a shallow copy of the model
-        """
+        """Returns a shallow copy of the model."""
         cls = type(self)
         m = cls.__new__(cls)
         _object_setattr(m, '__dict__', copy(self.__dict__))
         _object_setattr(m, '__pydantic_extra__', copy(self.__pydantic_extra__))
         _object_setattr(m, '__pydantic_fields_set__', copy(self.__pydantic_fields_set__))
 
         if self.__pydantic_private__ is None:
@@ -650,17 +637,15 @@
             _object_setattr(
                 m, '__pydantic_private__', {k: v for k, v in self.__pydantic_private__.items() if v is not _Undefined}
             )
 
         return m
 
     def __deepcopy__(self: Model, memo: dict[int, Any] | None = None) -> Model:
-        """
-        Returns a deep copy of the model
-        """
+        """Returns a deep copy of the model."""
         cls = type(self)
         m = cls.__new__(cls)
         _object_setattr(m, '__dict__', deepcopy(self.__dict__, memo=memo))
         _object_setattr(m, '__pydantic_extra__', deepcopy(self.__pydantic_extra__, memo=memo))
         # This next line doesn't need a deepcopy because __pydantic_fields_set__ is a set[str],
         # and attempting a deepcopy would be marginally slower.
         _object_setattr(m, '__pydantic_fields_set__', copy(self.__pydantic_fields_set__))
@@ -673,19 +658,18 @@
                 '__pydantic_private__',
                 deepcopy({k: v for k, v in self.__pydantic_private__.items() if v is not _Undefined}, memo=memo),
             )
 
         return m
 
     def __repr_args__(self) -> _repr.ReprArgs:
-        yield from (
-            (k, v)
-            for k, v in self.__dict__.items()
-            if not k.startswith('_') and (k not in self.model_fields or self.model_fields[k].repr)
-        )
+        for k, v in self.__dict__.items():
+            field = self.model_fields.get(k)
+            if field and field.repr:
+                yield k, v
         pydantic_extra = self.__pydantic_extra__
         if pydantic_extra is not None:
             yield from ((k, v) for k, v in pydantic_extra.items())
         yield from ((k, getattr(self, k)) for k, v in self.model_computed_fields.items() if v.repr)
 
     # take logic from `_repr.Representation` without the side effects of inheritance, see #5740
     __repr_name__ = _repr.Representation.__repr_name__
@@ -761,16 +745,15 @@
                 # Update cache
                 _generics.set_cached_generic_type(cls, typevar_values, submodel, origin, args)
 
         return submodel
 
     @classmethod
     def model_parametrized_name(cls, params: tuple[type[Any], ...]) -> str:
-        """
-        Compute the class name for parametrizations of generic classes.
+        """Compute the class name for parametrizations of generic classes.
 
         This method can be overridden to achieve a custom naming scheme for generic BaseModels.
 
         Args:
             params: Tuple of types of the class. Given a generic class
                 `Model` with 2 type variables and a concrete model `Model[str, int]`,
                 the value `(str, int)` would be passed to `params`.
@@ -969,16 +952,15 @@
         self: Model,
         *,
         include: AbstractSetIntStr | MappingIntStrAny | None = None,
         exclude: AbstractSetIntStr | MappingIntStrAny | None = None,
         update: typing.Dict[str, Any] | None = None,  # noqa UP006
         deep: bool = False,
     ) -> Model:  # pragma: no cover
-        """
-        Returns a copy of the model.
+        """Returns a copy of the model.
 
         This method is now deprecated; use `model_copy` instead. If you need `include` or `exclude`, use:
 
         ```py
         data = self.model_dump(include=include, exclude=exclude, round_trip=True)
         data = {**data, **(update or {})}
         copied = self.model_validate(data)
@@ -991,17 +973,14 @@
                 specifying which fields to exclude in the copied model.
             update: Optional dictionary of field-value pairs to override field values
                 in the copied model.
             deep: If True, the values of fields that are Pydantic models will be deep copied.
 
         Returns:
             A copy of the model with included, excluded and updated fields as specified.
-
-        Raises:
-            DeprecationWarning: The `copy` method is deprecated; use `model_copy` instead.
         """
         warnings.warn(
             'The `copy` method is deprecated; use `model_copy` instead. '
             'See the docstring of `BaseModel.copy` for details about how to handle `include` and `exclude`.',
             DeprecationWarning,
         )
 
@@ -1111,66 +1090,14 @@
     def _calculate_keys(self, *args: Any, **kwargs: Any) -> Any:
         warnings.warn(
             'The private method `_calculate_keys` will be removed and should no longer be used.', DeprecationWarning
         )
         return _deprecated_copy_internals._calculate_keys(self, *args, **kwargs)  # type: ignore
 
 
-RootModelRootType = typing.TypeVar('RootModelRootType')
-
-
-class RootModel(BaseModel, typing.Generic[RootModelRootType]):
-    """
-    A Pydantic `BaseModel` for the root object of the model.
-
-    Attributes:
-        root (RootModelRootType): The root object of the model.
-    """
-
-    __pydantic_root_model__ = True
-    # TODO: Make `__pydantic_fields_set__` logic consistent with `BaseModel`, i.e. it should be `set()` if default value
-    # was used
-    __pydantic_fields_set__ = {'root'}  # It's fine having a set here as it will never change
-    __pydantic_private__ = None
-    __pydantic_extra__ = None
-
-    root: RootModelRootType
-
-    def __init__(__pydantic_self__, root: RootModelRootType) -> None:  # type: ignore
-        __tracebackhide__ = True
-        __pydantic_self__.__pydantic_validator__.validate_python(root, self_instance=__pydantic_self__)
-
-    __init__.__pydantic_base_init__ = True  # type: ignore
-
-    @classmethod
-    def model_construct(cls: type[Model], root: RootModelRootType, _fields_set: set[str] | None = None) -> Model:
-        """
-        Create a new model using the provided root object and update fields set.
-
-        Args:
-            root: The root object of the model.
-            _fields_set: The set of fields to be updated.
-
-        Returns:
-            The new model.
-
-        Raises:
-            NotImplemented: If the model is not a subclass of `RootModel`.
-        """
-        return super().model_construct(root=root, _fields_set=_fields_set)
-
-    def __eq__(self, other: Any) -> bool:
-        if not isinstance(other, RootModel):
-            return NotImplemented
-        return self.model_fields['root'].annotation == other.model_fields['root'].annotation and super().__eq__(other)
-
-    def __repr_args__(self) -> _repr.ReprArgs:
-        yield 'root', self.root
-
-
 @typing.overload
 def create_model(
     __model_name: str,
     *,
     __config__: ConfigDict | None = None,
     __base__: None = None,
     __module__: str = __name__,
@@ -1202,16 +1129,15 @@
     __base__: type[Model] | tuple[type[Model], ...] | None = None,
     __module__: str = __name__,
     __validators__: dict[str, AnyClassMethod] | None = None,
     __cls_kwargs__: dict[str, Any] | None = None,
     __slots__: tuple[str, ...] | None = None,
     **field_definitions: Any,
 ) -> type[Model]:
-    """
-    Dynamically creates and returns a new Pydantic model.
+    """Dynamically creates and returns a new Pydantic model.
 
     Args:
         __model_name: The name of the newly created model.
         __config__: The configuration of the new model.
         __base__: The base class for the new model.
         __module__: The name of the module that the model belongs to.
         __validators__: A dictionary of methods that validate
@@ -1245,15 +1171,15 @@
 
     __cls_kwargs__ = __cls_kwargs__ or {}
 
     fields = {}
     annotations = {}
 
     for f_name, f_def in field_definitions.items():
-        if f_name.startswith('_'):
+        if not _fields.is_valid_field_name(f_name):
             warnings.warn(f'fields may not start with an underscore, ignoring "{f_name}"', RuntimeWarning)
         if isinstance(f_def, tuple):
             f_def = typing.cast('tuple[str, Any]', f_def)
             try:
                 f_annotation, f_value = f_def
             except ValueError as e:
                 raise PydanticUserError(
```

### Comparing `pydantic-2.0b2/pydantic/mypy.py` & `pydantic-2.0b3/pydantic/mypy.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     UnionType,
     get_proper_type,
 )
 from mypy.typevars import fill_typevars
 from mypy.util import get_unique_redefinition_name
 from mypy.version import __version__ as mypy_version
 
+from pydantic._internal import _fields
+
 try:
     from mypy.types import TypeVarDef  # type: ignore[attr-defined]
 except ImportError:  # pragma: no cover
     # Backward-compatible with TypeVarDef from Mypy 0.930.
     from mypy.types import TypeVarType as TypeVarDef
 
 CONFIGFILE_KEY = 'pydantic-mypy'
@@ -98,16 +100,15 @@
 BUILTINS_NAME = 'builtins' if MYPY_VERSION_TUPLE >= (0, 930) else '__builtins__'
 
 # Increment version if plugin changes and mypy caches should be invalidated
 __version__ = 2
 
 
 def plugin(version: str) -> type[Plugin]:
-    """
-    `version` is the mypy version string
+    """`version` is the mypy version string.
 
     We might want to use this to print a warning if the mypy version being used is
     newer, or especially older, than we expect (or need).
     """
     return PydanticPlugin
 
 
@@ -171,16 +172,15 @@
             return
         info_metaclass = ctx.cls.info.declared_metaclass
         assert info_metaclass, "callback not passed from 'get_metaclass_hook'"
         if getattr(info_metaclass.type, 'dataclass_transform_spec', None):
             info_metaclass.type.dataclass_transform_spec = None
 
     def _pydantic_field_callback(self, ctx: FunctionContext) -> Type:
-        """
-        Extract the type of the `default` argument from the Field function, and use it as the return type.
+        """Extract the type of the `default` argument from the Field function, and use it as the return type.
 
         In particular:
         * Check whether the default and default_factory argument is specified.
         * Output an error if both are specified.
         * Retrieve the type of the argument which is specified, and use it as return type for the function.
         """
         default_any_type = ctx.default_return_type
@@ -256,17 +256,15 @@
                 setattr(self, key, setting)
 
     def to_data(self) -> dict[str, Any]:
         return {key: getattr(self, key) for key in self.__slots__}
 
 
 def from_attributes_callback(ctx: MethodContext) -> Type:
-    """
-    Raise an error if from_attributes is not enabled
-    """
+    """Raise an error if from_attributes is not enabled."""
     model_type: Instance
     ctx_type = ctx.type
     if isinstance(ctx_type, TypeType):
         ctx_type = ctx_type.item
     if isinstance(ctx_type, CallableType) and isinstance(ctx_type.ret_type, Instance):
         model_type = ctx_type.ret_type  # called on the class
     elif isinstance(ctx_type, Instance):
@@ -294,16 +292,15 @@
     }
 
     def __init__(self, ctx: ClassDefContext, plugin_config: PydanticPluginConfig) -> None:
         self._ctx = ctx
         self.plugin_config = plugin_config
 
     def transform(self) -> None:
-        """
-        Configures the BaseModel subclass according to the plugin settings.
+        """Configures the BaseModel subclass according to the plugin settings.
 
         In particular:
         * determines the model config and fields,
         * adds a fields-aware signature for the initializer and construct methods
         * freezes the class if frozen = True
         * stores the fields, config, and if the class is settings in the mypy metadata for access by subclasses
         """
@@ -318,16 +315,15 @@
         self.set_frozen(fields, frozen=config.frozen is True)
         info.metadata[METADATA_KEY] = {
             'fields': {field.name: field.serialize() for field in fields},
             'config': config.set_values_dict(),
         }
 
     def adjust_validator_signatures(self) -> None:
-        """
-        When we decorate a function `f` with `pydantic.validator(...)`, `pydantic.field_validator`
+        """When we decorate a function `f` with `pydantic.validator(...)`, `pydantic.field_validator`
         or `pydantic.serializer(...)`, mypy sees `f` as a regular method taking a `self` instance,
         even though pydantic internally wraps `f` with `classmethod` if necessary.
 
         Teach mypy this by marking any function whose outermost decorator is a `validator()`,
         `field_validator()` or `serializer()` call as a `classmethod`.
         """
         for name, sym in self._ctx.cls.info.names.items():
@@ -337,17 +333,15 @@
                     isinstance(first_dec, CallExpr)
                     and isinstance(first_dec.callee, NameExpr)
                     and first_dec.callee.fullname in DECORATOR_FULLNAMES
                 ):
                     sym.node.func.is_class = True
 
     def collect_config(self) -> ModelConfigData:  # noqa: C901 (ignore complexity)
-        """
-        Collects the values of the config attributes that are used by the plugin, accounting for parent classes.
-        """
+        """Collects the values of the config attributes that are used by the plugin, accounting for parent classes."""
         ctx = self._ctx
         cls = ctx.cls
         config = ModelConfigData()
 
         has_config_kwargs = False
         has_config_from_namespace = False
 
@@ -404,17 +398,15 @@
             # Each class depends on the set of fields in its ancestors
             ctx.api.add_plugin_dependency(make_wildcard_trigger(get_fullname(info)))
             for name, value in info.metadata[METADATA_KEY]['config'].items():
                 config.setdefault(name, value)
         return config
 
     def collect_fields(self, model_config: ModelConfigData) -> list[PydanticModelField]:
-        """
-        Collects the fields for the model, accounting for parent classes
-        """
+        """Collects the fields for the model, accounting for parent classes."""
         # First, collect fields belonging to the current class.
         ctx = self._ctx
         cls = self._ctx.cls
         fields: list[PydanticModelField] = []
         known_fields: set[str] = set()
         for stmt in cls.defs.body:
             maybe_field = self.collect_field_from_stmt(stmt, model_config)
@@ -446,15 +438,15 @@
     def collect_field_from_stmt(self, stmt: Statement, model_config: ModelConfigData) -> PydanticModelField | None:
         ctx = self._ctx
         cls = self._ctx.cls
         if not isinstance(stmt, AssignmentStmt):
             return None
 
         lhs = stmt.lvalues[0]
-        if not isinstance(lhs, NameExpr) or lhs.name.startswith('_') or lhs.name == 'model_config':
+        if not isinstance(lhs, NameExpr) or not _fields.is_valid_field_name(lhs.name) or lhs.name == 'model_config':
             return None
 
         if not stmt.new_syntax:
             if (
                 isinstance(stmt.rvalue, CallExpr)
                 and isinstance(stmt.rvalue.callee, CallExpr)
                 and isinstance(stmt.rvalue.callee.callee, NameExpr)
@@ -500,16 +492,15 @@
             alias=alias,
             has_dynamic_alias=has_dynamic_alias,
             line=stmt.line,
             column=stmt.column,
         )
 
     def add_initializer(self, fields: list[PydanticModelField], config: ModelConfigData) -> None:
-        """
-        Adds a fields-aware `__init__` method to the class.
+        """Adds a fields-aware `__init__` method to the class.
 
         The added `__init__` will be annotated with types vs. all `Any` depending on the plugin settings.
         """
         ctx = self._ctx
         typed = self.plugin_config.init_typed
         use_alias = config.populate_by_name is not True
         force_all_optional = bool(config.has_alias_generator and not config.populate_by_name)
@@ -520,16 +511,15 @@
             var = Var('kwargs')
             init_arguments.append(Argument(var, AnyType(TypeOfAny.explicit), None, ARG_STAR2))
 
         if '__init__' not in ctx.cls.info.names:
             add_method(ctx, '__init__', init_arguments, NoneType())
 
     def add_model_construct_method(self, fields: list[PydanticModelField]) -> None:
-        """
-        Adds a fully typed `model_construct` classmethod to the class.
+        """Adds a fully typed `model_construct` classmethod to the class.
 
         Similar to the fields-aware __init__ method, but always uses the field names (not aliases),
         and does not treat settings fields as optional.
         """
         ctx = self._ctx
         set_str = ctx.api.named_type(f'{BUILTINS_NAME}.set', [ctx.api.named_type(f'{BUILTINS_NAME}.str')])
         optional_set_str = UnionType([set_str, NoneType()])
@@ -560,16 +550,15 @@
             return_type=self_type,
             self_type=self_type,
             tvar_def=self_type,
             is_classmethod=True,
         )
 
     def set_frozen(self, fields: list[PydanticModelField], frozen: bool) -> None:
-        """
-        Marks all fields as properties so that attempts to set them trigger mypy errors.
+        """Marks all fields as properties so that attempts to set them trigger mypy errors.
 
         This is the same approach used by the attrs and dataclasses plugins.
         """
         ctx = self._ctx
         info = ctx.cls.info
         for field in fields:
             sym_node = info.names.get(field.name)
@@ -593,16 +582,15 @@
                 var = field.to_var(info, use_alias=False)
                 var.info = info
                 var.is_property = frozen
                 var._fullname = get_fullname(info) + '.' + get_name(var)
                 info.names[get_name(var)] = SymbolTableNode(MDEF, var)
 
     def get_config_update(self, name: str, arg: Expression) -> ModelConfigData | None:
-        """
-        Determines the config update due to a single kwarg in the ConfigDict definition.
+        """Determines the config update due to a single kwarg in the ConfigDict definition.
 
         Warns if a tracked config attribute is set to a value the plugin doesn't know how to interpret (e.g., an int)
         """
         if name not in self.tracked_config_fields:
             return None
         if name == 'extra':
             if isinstance(arg, StrExpr):
@@ -621,17 +609,15 @@
         if isinstance(arg, NameExpr) and arg.fullname in ('builtins.True', 'builtins.False'):
             return ModelConfigData(**{name: arg.fullname == 'builtins.True'})
         error_invalid_config_value(name, self._ctx.api, arg)
         return None
 
     @staticmethod
     def get_is_required(cls: ClassDef, stmt: AssignmentStmt, lhs: NameExpr) -> bool:
-        """
-        Returns a boolean indicating whether the field defined in `stmt` is a required field.
-        """
+        """Returns a boolean indicating whether the field defined in `stmt` is a required field."""
         expr = stmt.rvalue
         if isinstance(expr, TempNode):
             # TempNode means annotation-only, so only non-required if Optional
             value_type = get_proper_type(cls.info[lhs.name].type)
             if isinstance(value_type, UnionType) and any(isinstance(item, NoneType) for item in value_type.items):
                 # Annotated as Optional, or otherwise having NoneType in the union
                 return False
@@ -648,16 +634,15 @@
                     return False
             return True
         # Only required if the "default value" is Ellipsis (i.e., `field_name: Annotation = ...`)
         return isinstance(expr, EllipsisExpr)
 
     @staticmethod
     def get_alias_info(stmt: AssignmentStmt) -> tuple[str | None, bool]:
-        """
-        Returns a pair (alias, has_dynamic_alias), extracted from the declaration of the field defined in `stmt`.
+        """Returns a pair (alias, has_dynamic_alias), extracted from the declaration of the field defined in `stmt`.
 
         `has_dynamic_alias` is True if and only if an alias is provided, but not as a string literal.
         If `has_dynamic_alias` is True, `alias` will be None.
         """
         expr = stmt.rvalue
         if isinstance(expr, TempNode):
             # TempNode means annotation-only
@@ -678,45 +663,42 @@
             else:
                 return None, True
         return None, False
 
     def get_field_arguments(
         self, fields: list[PydanticModelField], typed: bool, force_all_optional: bool, use_alias: bool
     ) -> list[Argument]:
-        """
-        Helper function used during the construction of the `__init__` and `model_construct` method signatures.
+        """Helper function used during the construction of the `__init__` and `model_construct` method signatures.
 
         Returns a list of mypy Argument instances for use in the generated signatures.
         """
         info = self._ctx.cls.info
         arguments = [
             field.to_argument(info, typed=typed, force_optional=force_all_optional, use_alias=use_alias)
             for field in fields
             if not (use_alias and field.has_dynamic_alias)
         ]
         return arguments
 
     def should_init_forbid_extra(self, fields: list[PydanticModelField], config: ModelConfigData) -> bool:
-        """
-        Indicates whether the generated `__init__` should get a `**kwargs` at the end of its signature
+        """Indicates whether the generated `__init__` should get a `**kwargs` at the end of its signature.
 
         We disallow arbitrary kwargs if the extra config setting is "forbid", or if the plugin config says to,
         *unless* a required dynamic alias is present (since then we can't determine a valid signature).
         """
         if not config.populate_by_name:
             if self.is_dynamic_alias_present(fields, bool(config.has_alias_generator)):
                 return False
         if config.forbid_extra:
             return True
         return self.plugin_config.init_forbid_extra
 
     @staticmethod
     def is_dynamic_alias_present(fields: list[PydanticModelField], has_alias_generator: bool) -> bool:
-        """
-        Returns whether any fields on the model have a "dynamic alias", i.e., an alias that cannot be
+        """Returns whether any fields on the model have a "dynamic alias", i.e., an alias that cannot be
         determined during static analysis.
         """
         for field in fields:
             if field.has_dynamic_alias:
                 return True
         if has_alias_generator:
             for field in fields:
@@ -836,16 +818,15 @@
     return_type: Type,
     self_type: Type | None = None,
     tvar_def: TypeVarDef | None = None,
     is_classmethod: bool = False,
     is_new: bool = False,
     # is_staticmethod: bool = False,
 ) -> None:
-    """
-    Adds a new method to a class.
+    """Adds a new method to a class.
 
     This can be dropped if/when https://github.com/python/mypy/issues/7301 is merged
     """
     info = ctx.cls.info
 
     # First remove any previously generated methods with the same name
     # to avoid clashes and problems in the semantic analyzer.
@@ -909,27 +890,23 @@
     sym.plugin_generated = True
 
     info.names[name] = sym
     info.defn.defs.body.append(func)
 
 
 def get_fullname(x: FuncBase | SymbolNode) -> str:
-    """
-    Used for compatibility with mypy 0.740; can be dropped once support for 0.740 is dropped.
-    """
+    """Used for compatibility with mypy 0.740; can be dropped once support for 0.740 is dropped."""
     fn = x.fullname
     if callable(fn):  # pragma: no cover
         return fn()
     return fn
 
 
 def get_name(x: FuncBase | SymbolNode) -> str:
-    """
-    Used for compatibility with mypy 0.740; can be dropped once support for 0.740 is dropped.
-    """
+    """Used for compatibility with mypy 0.740; can be dropped once support for 0.740 is dropped."""
     fn = x.name
     if callable(fn):  # pragma: no cover
         return fn()
     return fn
 
 
 def parse_toml(config_file: str) -> dict[str, Any] | None:
```

### Comparing `pydantic-2.0b2/pydantic/networks.py` & `pydantic-2.0b3/pydantic/networks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""The networks module contains types for common network-related fields."""
 from __future__ import annotations as _annotations
 
 import dataclasses as _dataclasses
 import re
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from typing import TYPE_CHECKING, Any
 
@@ -42,14 +43,25 @@
     'MySQLDsn',
     'MariaDBDsn',
 ]
 
 
 @_dataclasses.dataclass
 class UrlConstraints(_fields.PydanticMetadata):
+    """Url constraints.
+
+    Attributes:
+        max_length: The maximum length of the url. Defaults to `None`.
+        allowed_schemes: The allowed schemes. Defaults to `None`.
+        host_required: Whether the host is required. Defaults to `None`.
+        default_host: The default host. Defaults to `None`.
+        default_port: The default port. Defaults to `None`.
+        default_path: The default path. Defaults to `None`.
+    """
+
     max_length: int | None = None
     allowed_schemes: list[str] | None = None
     host_required: bool | None = None
     default_host: str | None = None
     default_port: int | None = None
     default_path: str | None = None
 
@@ -63,18 +75,21 @@
                 self.default_port,
                 self.default_path,
             )
         )
 
 
 AnyUrl = Url
-# host_required is false because all schemes are "special" so host is required by rust-url automatically
+"""Base type for all URLs."""
 AnyHttpUrl = Annotated[Url, UrlConstraints(allowed_schemes=['http', 'https'])]
+"""A type that will accept any http or https URL."""
 HttpUrl = Annotated[Url, UrlConstraints(max_length=2083, allowed_schemes=['http', 'https'])]
+"""A type that will accept any http or https URL with a max length of 2083 characters."""
 FileUrl = Annotated[Url, UrlConstraints(allowed_schemes=['file'])]
+"""A type that will accept any file URL."""
 PostgresDsn = Annotated[
     MultiHostUrl,
     UrlConstraints(
         host_required=True,
         allowed_schemes=[
             'postgres',
             'postgresql',
@@ -84,33 +99,39 @@
             'postgresql+psycopg2',
             'postgresql+psycopg2cffi',
             'postgresql+py-postgresql',
             'postgresql+pygresql',
         ],
     ),
 ]
+"""A type that will accept any Postgres DSN."""
 
 CockroachDsn = Annotated[
     Url,
     UrlConstraints(
         host_required=True,
         allowed_schemes=[
             'cockroachdb',
             'cockroachdb+psycopg2',
             'cockroachdb+asyncpg',
         ],
     ),
 ]
+"""A type that will accept any Cockroach DSN."""
 AmqpDsn = Annotated[Url, UrlConstraints(allowed_schemes=['amqp', 'amqps'])]
+"""A type that will accept any AMQP DSN."""
 RedisDsn = Annotated[
     Url,
     UrlConstraints(allowed_schemes=['redis', 'rediss'], default_host='localhost', default_port=6379, default_path='/0'),
 ]
+"""A type that will accept any Redis DSN."""
 MongoDsn = Annotated[MultiHostUrl, UrlConstraints(allowed_schemes=['mongodb', 'mongodb+srv'], default_port=27017)]
+"""A type that will accept any MongoDB DSN."""
 KafkaDsn = Annotated[Url, UrlConstraints(allowed_schemes=['kafka'], default_host='localhost', default_port=9092)]
+"""A type that will accept any Kafka DSN."""
 MySQLDsn = Annotated[
     Url,
     UrlConstraints(
         allowed_schemes=[
             'mysql',
             'mysql+mysqlconnector',
             'mysql+aiomysql',
@@ -119,21 +140,23 @@
             'mysql+pymysql',
             'mysql+cymysql',
             'mysql+pyodbc',
         ],
         default_port=3306,
     ),
 ]
+"""A type that will accept any MySQL DSN."""
 MariaDBDsn = Annotated[
     Url,
     UrlConstraints(
         allowed_schemes=['mariadb', 'mariadb+mariadbconnector', 'mariadb+pymysql'],
         default_port=3306,
     ),
 ]
+"""A type that will accept any MariaDB DSN."""
 
 
 def import_email_validator() -> None:
     global email_validator
     try:
         import email_validator
     except ImportError as e:
@@ -141,36 +164,68 @@
 
 
 if TYPE_CHECKING:
     EmailStr = Annotated[str, ...]
 else:
 
     class EmailStr:
+        """Validate email addresses.
+
+        Example:
+            ```py
+            from pydantic import BaseModel, EmailStr
+
+            class Model(BaseModel):
+                email: EmailStr
+
+            print(Model(email='contact@mail.com'))
+            # > email='contact@mail.com'
+            ```
+        """
+
         @classmethod
         def __get_pydantic_core_schema__(
             cls,
             source: type[Any],
         ) -> core_schema.CoreSchema:
             import_email_validator()
-            return core_schema.general_after_validator_function(cls.validate, core_schema.str_schema())
+            return core_schema.general_after_validator_function(cls._validate, core_schema.str_schema())
 
         @classmethod
         def __get_pydantic_json_schema__(
             cls, core_schema: core_schema.CoreSchema, handler: _schema_generation_shared.GetJsonSchemaHandler
         ) -> JsonSchemaValue:
             field_schema = handler(core_schema)
             field_schema.update(type='string', format='email')
             return field_schema
 
         @classmethod
-        def validate(cls, __input_value: str, _: core_schema.ValidationInfo) -> str:
+        def _validate(cls, __input_value: str, _: core_schema.ValidationInfo) -> str:
             return validate_email(__input_value)[1]
 
 
 class NameEmail(_repr.Representation):
+    """Validate a name and email address combination.
+
+    Example:
+        ```py
+        from pydantic import BaseModel, NameEmail
+
+        class User(BaseModel):
+            email: NameEmail
+
+        print(User(email='John Doe <john.doe@mail.com>'))
+        #> email=NameEmail(name='John Doe', email='john.doe@mail.com')
+        ```
+
+    Attributes:
+        name: The name.
+        email: The email address.
+    """
+
     __slots__ = 'name', 'email'
 
     def __init__(self, name: str, email: str):
         self.name = name
         self.email = email
 
     def __eq__(self, other: Any) -> bool:
@@ -205,17 +260,20 @@
             return cls(name, email)
 
     def __str__(self) -> str:
         return f'{self.name} <{self.email}>'
 
 
 class IPvAnyAddress:
+    """Validate an IPv4 or IPv6 address."""
+
     __slots__ = ()
 
     def __new__(cls, value: Any) -> IPv4Address | IPv6Address:  # type: ignore[misc]
+        """Validate an IPv4 or IPv6 address."""
         try:
             return IPv4Address(value)
         except ValueError:
             pass
 
         try:
             return IPv6Address(value)
@@ -239,17 +297,20 @@
 
     @classmethod
     def _validate(cls, __input_value: Any, _: core_schema.ValidationInfo) -> IPv4Address | IPv6Address:
         return cls(__input_value)  # type: ignore[return-value]
 
 
 class IPvAnyInterface:
+    """Validate an IPv4 or IPv6 interface."""
+
     __slots__ = ()
 
     def __new__(cls, value: NetworkType) -> IPv4Interface | IPv6Interface:  # type: ignore[misc]
+        """Validate an IPv4 or IPv6 interface."""
         try:
             return IPv4Interface(value)
         except ValueError:
             pass
 
         try:
             return IPv6Interface(value)
@@ -273,17 +334,20 @@
 
     @classmethod
     def _validate(cls, __input_value: NetworkType, _: core_schema.ValidationInfo) -> IPv4Interface | IPv6Interface:
         return cls(__input_value)  # type: ignore[return-value]
 
 
 class IPvAnyNetwork:
+    """Validate an IPv4 or IPv6 network."""
+
     __slots__ = ()
 
     def __new__(cls, value: NetworkType) -> IPv4Network | IPv6Network:  # type: ignore[misc]
+        """Validate an IPv4 or IPv6 network."""
         # Assume IP Network is defined with a default value for `strict` argument.
         # Define your own class if you want to specify network address check strictness.
         try:
             return IPv4Network(value)
         except ValueError:
             pass
 
@@ -308,33 +372,43 @@
         return core_schema.general_plain_validator_function(cls._validate)
 
     @classmethod
     def _validate(cls, __input_value: NetworkType, _: core_schema.ValidationInfo) -> IPv4Network | IPv6Network:
         return cls(__input_value)  # type: ignore[return-value]
 
 
-pretty_email_regex = re.compile(r' *([\w ]*?) *<(.+?)> *')
+def _build_pretty_email_regex() -> re.Pattern:
+    name_chars = r'[\w!#$%&\'*+\-/=?^_`{|}~]'
+    unquoted_name_group = fr'((?:{name_chars}+\s+)*{name_chars}+)'
+    quoted_name_group = r'"((?:[^"]|\")+)"'
+    email_group = r'<\s*(.+)\s*>'
+    return re.compile(rf'\s*(?:{unquoted_name_group}|{quoted_name_group})?\s*{email_group}\s*')
+
+
+pretty_email_regex = _build_pretty_email_regex()
 
 
 def validate_email(value: str) -> tuple[str, str]:
-    """
-    Email address validation using https://pypi.org/project/email-validator/
+    """Email address validation using https://pypi.org/project/email-validator/.
+
+    Note:
+        Note that:
 
-    Notes:
-    * raw ip address (literal) domain parts are not allowed.
-    * "John Doe <local_part@domain.com>" style "pretty" email addresses are processed
-    * spaces are striped from the beginning and end of addresses but no error is raised
+        * Raw IP address (literal) domain parts are not allowed.
+        * "John Doe <local_part@domain.com>" style "pretty" email addresses are processed.
+        * Spaces are striped from the beginning and end of addresses, but no error is raised.
     """
     if email_validator is None:
         import_email_validator()
 
     m = pretty_email_regex.fullmatch(value)
     name: str | None = None
     if m:
-        name, value = m.groups()
+        unquoted_name, quoted_name, value = m.groups()
+        name = unquoted_name or quoted_name
 
     email = value.strip()
 
     try:
         parts = email_validator.validate_email(email, check_deliverability=False)
     except email_validator.EmailNotValidError as e:
         raise PydanticCustomError(
```

### Comparing `pydantic-2.0b2/pydantic/type_adapter.py` & `pydantic-2.0b3/pydantic/type_adapter.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 if TYPE_CHECKING:
     # should be `set[int] | set[str] | dict[int, IncEx] | dict[str, IncEx] | None`, but mypy can't cope
     IncEx = Union[Set[int], Set[str], Dict[int, Any], Dict[str, Any]]
 
 
 def _get_schema(type_: Any, config_wrapper: _config.ConfigWrapper, parent_depth: int) -> CoreSchema:
-    """
-    `BaseModel` uses its own `__module__` to find out where it was defined
+    """`BaseModel` uses its own `__module__` to find out where it was defined
     and then look for symbols to resolve forward references in those globals.
     On the other hand this function can be called with arbitrary objects,
     including type aliases where `__module__` (always `typing.py`) is not useful.
     So instead we look at the globals in our parent stack frame.
 
     This works for the case where this function is called in a module that
     has the target of forward references in its scope, but
@@ -72,21 +71,21 @@
 
     But at the very least this behavior is _subtly_ different from `BaseModel`'s.
     """
     local_ns = _typing_extra.parent_frame_namespace(parent_depth=parent_depth)
     global_ns = sys._getframe(max(parent_depth - 1, 1)).f_globals.copy()
     global_ns.update(local_ns or {})
     gen = _generate_schema.GenerateSchema(config_wrapper, types_namespace=global_ns, typevars_map={})
-    return gen.generate_schema(type_)
+    schema = gen.generate_schema(type_)
+    schema = gen.collect_definitions(schema)
+    return schema
 
 
 def _getattr_no_parents(obj: Any, attribute: str) -> Any:
-    """
-    Returns the attribute value without attempting to look up attributes from parent types
-    """
+    """Returns the attribute value without attempting to look up attributes from parent types."""
     if hasattr(obj, '__dict__'):
         try:
             return obj.__dict__[attribute]
         except KeyError:
             pass
 
     slots = getattr(obj, '__slots__', None)
@@ -95,18 +94,23 @@
     else:
         raise AttributeError(attribute)
 
 
 class TypeAdapter(Generic[T]):
     """A class representing the type adapter.
 
+    A `TypeAdapter` instance exposes some of the functionality from `BaseModel` instance methods
+    for types that do not have such methods (such as dataclasses, primitive types, and more).
+
+    Note that `TypeAdapter` is not an actual type, so you cannot use it in type annotations.
+
     Attributes:
-        core_schema (CoreSchema): The core schema for the type.
-        validator (SchemaValidator): The schema validator for the type.
-        serializer (SchemaSerializer): The schema serializer for the type.
+        core_schema: The core schema for the type.
+        validator: The schema validator for the type.
+        serializer: The schema serializer for the type.
     """
 
     if TYPE_CHECKING:
 
         @overload
         def __new__(cls, __type: type[T], *, config: ConfigDict | None = ...) -> TypeAdapter[T]:
             ...
@@ -115,14 +119,15 @@
         # Pyright currently handles this "correctly", but MyPy understands this as TypeAdapter[object]
         # so an explicit type cast is needed
         @overload
         def __new__(cls, __type: T, *, config: ConfigDict | None = ...) -> TypeAdapter[T]:
             ...
 
         def __new__(cls, __type: Any, *, config: ConfigDict | None = ...) -> TypeAdapter[T]:
+            """A class representing the type adapter."""
             raise NotImplementedError
 
     def __init__(self, type: Any, *, config: ConfigDict | None = None, _parent_depth: int = 2) -> None:
         """Initializes the TypeAdapter object."""
         config_wrapper = _config.ConfigWrapper(config)
 
         try:
@@ -170,54 +175,51 @@
         self,
         __object: Any,
         *,
         strict: bool | None = None,
         from_attributes: bool | None = None,
         context: dict[str, Any] | None = None,
     ) -> T:
-        """
-        Validate a Python object against the model.
+        """Validate a Python object against the model.
 
         Args:
-            __object (Any): The Python object to validate against the model.
-            strict (bool | None, optional): Whether to strictly check types. Defaults to None.
-            from_attributes (bool | None, optional): Whether to extract data from object attributes. Defaults to None.
-            context (dict[str, Any] | None, optional): Additional context to use during validation. Defaults to None.
+            __object: The Python object to validate against the model.
+            strict: Whether to strictly check types.
+            from_attributes: Whether to extract data from object attributes.
+            context: Additional context to pass to the validator.
 
         Returns:
-            T: The validated object.
-
+            The validated object.
         """
         return self.validator.validate_python(__object, strict=strict, from_attributes=from_attributes, context=context)
 
     def validate_json(
         self, __data: str | bytes, *, strict: bool | None = None, context: dict[str, Any] | None = None
     ) -> T:
         """Validate a JSON string or bytes against the model.
 
         Args:
-            __data (str | bytes): The JSON data to validate against the model.
-            strict (bool | None, optional): Whether to strictly check types. Defaults to None.
-            context (dict[str, Any] | None, optional): Additional context to use during validation. Defaults to None.
+            __data: The JSON data to validate against the model.
+            strict: Whether to strictly check types.
+            context: Additional context to use during validation.
 
         Returns:
-            T: The validated object.
-
+            The validated object.
         """
         return self.validator.validate_json(__data, strict=strict, context=context)
 
     def get_default_value(self, *, strict: bool | None = None, context: dict[str, Any] | None = None) -> Some[T] | None:
-        """Get the default value for this model / type.
+        """Get the default value for the wrapped type.
 
         Args:
-            strict (bool | None, optional): Whether to strictly check types. Defaults to None.
-            context (dict[str, Any] | None, optional): Additional context to use during validation. Defaults to None.
+            strict: Whether to strictly check types.
+            context: Additional context to pass to the validator.
 
         Returns:
-            Some[T] | None: The default value wrapped in a Some if there is one or None if not.
+            The default value wrapped in a `Some` if there is one or None if not.
         """
         return self.validator.get_default_value(strict=strict, context=context)
 
     def dump_python(
         self,
         __instance: T,
         *,
@@ -227,32 +229,30 @@
         by_alias: bool = False,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
         round_trip: bool = False,
         warnings: bool = True,
     ) -> Any:
-        """Dump a Python object to a serialized format.
+        """Dump an instance of the adapted type to a Python object.
 
         Args:
-            __instance (T): The Python object to serialize.
-            mode (Literal['json', 'python'], optional): The output format. Defaults to 'python'.
-            include (IncEx | None, optional): Fields to include in the output. Defaults to None.
-            exclude (IncEx | None, optional): Fields to exclude from the output. Defaults to None.
-            by_alias (bool, optional): Whether to use alias names for field names. Defaults to False.
-            exclude_unset (bool, optional): Whether to exclude unset fields. Defaults to False.
-            exclude_defaults (bool, optional): Whether to exclude fields with default values. Defaults to False.
-            exclude_none (bool, optional): Whether to exclude fields with None values. Defaults to False.
-            round_trip (bool, optional): Whether to output the serialized data in a way that is compatible with
-                deserialization. Defaults to False.
-            warnings (bool, optional): Whether to display serialization warnings. Defaults to True.
+            __instance: The Python object to serialize.
+            mode: The output format.
+            include: Fields to include in the output.
+            exclude: Fields to exclude from the output.
+            by_alias: Whether to use alias names for field names.
+            exclude_unset: Whether to exclude unset fields.
+            exclude_defaults: Whether to exclude fields with default values.
+            exclude_none: Whether to exclude fields with None values.
+            round_trip: Whether to output the serialized data in a way that is compatible with deserialization.
+            warnings: Whether to display serialization warnings.
 
         Returns:
-            Any: The serialized object.
-
+            The serialized object.
         """
         return self.serializer.to_python(
             __instance,
             mode=mode,
             by_alias=by_alias,
             include=include,
             exclude=exclude,
@@ -273,31 +273,30 @@
         by_alias: bool = False,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
         round_trip: bool = False,
         warnings: bool = True,
     ) -> bytes:
-        """Serialize the given instance to JSON.
+        """Serialize an instance of the adapted type to JSON.
 
         Args:
-            __instance (T): The instance to be serialized.
-            indent (Optional[int]): Number of spaces for JSON indentation (default: None).
-            include (Optional[IncEx]): Fields to include (default: None).
-            exclude (Optional[IncEx]): Fields to exclude (default: None).
-            by_alias (bool): Whether to use alias names (default: False).
-            exclude_unset (bool): Whether to exclude unset fields (default: False).
-            exclude_defaults (bool): Whether to exclude fields with default values (default: False).
-            exclude_none (bool): Whether to exclude fields with a value of None (default: False).
-            round_trip (bool): Whether to serialize and deserialize the instance to ensure
-                round-tripping (default: False).
-            warnings (bool): Whether to emit serialization warnings (default: True).
+            __instance: The instance to be serialized.
+            indent: Number of spaces for JSON indentation.
+            include: Fields to include.
+            exclude: Fields to exclude.
+            by_alias: Whether to use alias names for field names.
+            exclude_unset: Whether to exclude unset fields.
+            exclude_defaults: Whether to exclude fields with default values.
+            exclude_none: Whether to exclude fields with a value of `None`.
+            round_trip: Whether to serialize and deserialize the instance to ensure round-tripping.
+            warnings: Whether to emit serialization warnings.
 
         Returns:
-            bytes: The JSON representation of the given instance as bytes.
+            The JSON representation of the given instance as bytes.
         """
         return self.serializer.to_json(
             __instance,
             indent=indent,
             include=include,
             exclude=exclude,
             by_alias=by_alias,
@@ -312,54 +311,52 @@
         self,
         *,
         by_alias: bool = True,
         ref_template: str = DEFAULT_REF_TEMPLATE,
         schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
         mode: JsonSchemaMode = 'validation',
     ) -> dict[str, Any]:
-        """Generate a JSON schema for the model.
+        """Generate a JSON schema for the adapted type.
 
         Args:
-            by_alias (bool): Whether to use alias names (default: True).
-            ref_template (str): The format string used for generating $ref strings (default: DEFAULT_REF_TEMPLATE).
-            schema_generator (Type[GenerateJsonSchema]): The generator class used for creating the schema
-                (default: GenerateJsonSchema).
+            by_alias: Whether to use alias names for field names.
+            ref_template: The format string used for generating $ref strings.
+            schema_generator: The generator class used for creating the schema.
+            mode: The mode to use for schema generation.
 
         Returns:
-            Dict[str, Any]: The JSON schema for the model as a dictionary.
+            The JSON schema for the model as a dictionary.
         """
         schema_generator_instance = schema_generator(by_alias=by_alias, ref_template=ref_template)
         return schema_generator_instance.generate(self.core_schema, mode=mode)
 
     @staticmethod
     def json_schemas(
         __inputs: Iterable[tuple[JsonSchemaKeyT, JsonSchemaMode, TypeAdapter[Any]]],
         *,
         by_alias: bool = True,
         title: str | None = None,
         description: str | None = None,
         ref_template: str = DEFAULT_REF_TEMPLATE,
         schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
     ) -> tuple[dict[tuple[JsonSchemaKeyT, JsonSchemaMode], DefsRef], JsonSchemaValue]:
-        """Generate JSON schemas for multiple type adapters.
+        """Generate a JSON schema including definitions from multiple type adapters.
 
         Args:
-            __inputs (Iterable[tuple[JsonSchemaKeyT, JsonSchemaMode, TypeAdapter[Any]]]): Inputs to schema generation.
-                The first two items will form the keys of the (first) output mapping; the type adapters will provide
-                the core schemas that get converted into definitions in the output JSON schema.
-            by_alias (bool): Whether to use alias names (default: True).
-            title (Optional[str]): The title for the schema (default: None).
-            description (Optional[str]): The description for the schema (default: None).
-            ref_template (str): The format string used for generating $ref strings (default: DEFAULT_REF_TEMPLATE).
-            schema_generator (Type[GenerateJsonSchema]): The generator class used for creating the
-                schema (default: GenerateJsonSchema).
+            __inputs: Inputs to schema generation. The first two items will form the keys of the (first)
+                output mapping; the type adapters will provide the core schemas that get converted into
+                definitions in the output JSON schema.
+            by_alias: Whether to use alias names.
+            title: The title for the schema.
+            description: The description for the schema.
+            ref_template: The format string used for generating $ref strings.
+            schema_generator: The generator class used for creating the schema.
 
         Returns:
-            tuple[dict[tuple[Hashable, JsonSchemaMode], DefsRef], JsonSchemaValue]:
-                The first item contains the mapping of key + mode to a definitions reference, which will be a key
+            The first item contains the mapping of key + mode to a definitions reference, which will be a key
                 of the $defs mapping in the JSON schema included as the second member of the returned tuple.
         """
         schema_generator_instance = schema_generator(by_alias=by_alias, ref_template=ref_template)
 
         inputs = [(key, mode, adapter.core_schema) for key, mode, adapter in __inputs]
 
         key_map, definitions = schema_generator_instance.generate_definitions(inputs)
```

### Comparing `pydantic-2.0b2/pydantic/types.py` & `pydantic-2.0b3/pydantic/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""The types module contains custom types used by pydantic."""
 from __future__ import annotations as _annotations
 
 import base64
 import dataclasses as _dataclasses
 import re
 from datetime import date, datetime
 from decimal import Decimal
@@ -21,22 +22,20 @@
     Set,
     TypeVar,
     cast,
 )
 from uuid import UUID
 
 import annotated_types
-from pydantic_core import CoreSchema, PydanticCustomError, PydanticKnownError, PydanticOmit, core_schema
-from typing_extensions import Annotated, Literal, Protocol
+from pydantic_core import CoreSchema, PydanticCustomError, PydanticKnownError, core_schema
+from typing_extensions import Annotated, Literal, Protocol, deprecated
 
 from ._internal import (
     _annotated_handlers,
-    _core_metadata,
     _fields,
-    _generics,
     _internal_dataclass,
     _known_annotated_metadata,
     _utils,
     _validators,
 )
 from ._migration import getattr_migration
 from .config import ConfigDict
@@ -68,15 +67,14 @@
     'UUID3',
     'UUID4',
     'UUID5',
     'FilePath',
     'DirectoryPath',
     'NewPath',
     'Json',
-    'SecretField',
     'SecretStr',
     'SecretBytes',
     'StrictBool',
     'StrictBytes',
     'StrictInt',
     'StrictFloat',
     'PaymentCardNumber',
@@ -91,63 +89,83 @@
     'AllowInfNan',
     'EncoderProtocol',
     'EncodedBytes',
     'EncodedStr',
     'Base64Encoder',
     'Base64Bytes',
     'Base64Str',
-    'SkipValidation',
-    'InstanceOf',
-    'WithJsonSchema',
 )
 
 
 @_dataclasses.dataclass
 class Strict(_fields.PydanticMetadata):
+    """A field metadata class to indicate that a field should be validated in strict mode."""
+
     strict: bool = True
 
     def __hash__(self) -> int:
         return hash(self.strict)
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ BOOLEAN TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 StrictBool = Annotated[bool, Strict()]
+"""A boolean that must be either ``True`` or ``False``."""
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ INTEGER TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 def conint(
     *,
     strict: bool | None = None,
     gt: int | None = None,
     ge: int | None = None,
     lt: int | None = None,
     le: int | None = None,
     multiple_of: int | None = None,
 ) -> type[int]:
+    """A wrapper around `int` that allows for additional constraints.
+
+    Args:
+        strict: Whether to validate the integer in strict mode. Defaults to `None`.
+        gt: The value must be greater than this.
+        ge: The value must be greater than or equal to this.
+        lt: The value must be less than this.
+        le: The value must be less than or equal to this.
+        multiple_of: The value must be a multiple of this.
+
+    Returns:
+        The wrapped integer type.
+    """
     return Annotated[  # type: ignore[return-value]
         int,
         Strict(strict) if strict is not None else None,
         annotated_types.Interval(gt=gt, ge=ge, lt=lt, le=le),
         annotated_types.MultipleOf(multiple_of) if multiple_of is not None else None,
     ]
 
 
 PositiveInt = Annotated[int, annotated_types.Gt(0)]
+"""An integer that must be greater than zero."""
 NegativeInt = Annotated[int, annotated_types.Lt(0)]
+"""An integer that must be less than zero."""
 NonPositiveInt = Annotated[int, annotated_types.Le(0)]
+"""An integer that must be less than or equal to zero."""
 NonNegativeInt = Annotated[int, annotated_types.Ge(0)]
+"""An integer that must be greater than or equal to zero."""
 StrictInt = Annotated[int, Strict()]
+"""An integer that must be validated in strict mode."""
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ FLOAT TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 @_dataclasses.dataclass
 class AllowInfNan(_fields.PydanticMetadata):
+    """A field metadata class to indicate that a field should allow ``-inf``, ``inf``, and ``nan``."""
+
     allow_inf_nan: bool = True
 
     def __hash__(self) -> int:
         return hash(self.allow_inf_nan)
 
 
 def confloat(
@@ -156,48 +174,79 @@
     gt: float | None = None,
     ge: float | None = None,
     lt: float | None = None,
     le: float | None = None,
     multiple_of: float | None = None,
     allow_inf_nan: bool | None = None,
 ) -> type[float]:
+    """A wrapper around `float` that allows for additional constraints.
+
+    Args:
+        strict: Whether to validate the float in strict mode.
+        gt: The value must be greater than this.
+        ge: The value must be greater than or equal to this.
+        lt: The value must be less than this.
+        le: The value must be less than or equal to this.
+        multiple_of: The value must be a multiple of this.
+        allow_inf_nan: Whether to allow `-inf`, `inf`, and `nan`.
+
+    Returns:
+        The wrapped float type.
+    """
     return Annotated[  # type: ignore[return-value]
         float,
         Strict(strict) if strict is not None else None,
         annotated_types.Interval(gt=gt, ge=ge, lt=lt, le=le),
         annotated_types.MultipleOf(multiple_of) if multiple_of is not None else None,
         AllowInfNan(allow_inf_nan) if allow_inf_nan is not None else None,
     ]
 
 
 PositiveFloat = Annotated[float, annotated_types.Gt(0)]
+"""A float that must be greater than zero."""
 NegativeFloat = Annotated[float, annotated_types.Lt(0)]
+"""A float that must be less than zero."""
 NonPositiveFloat = Annotated[float, annotated_types.Le(0)]
+"""A float that must be less than or equal to zero.""" ''
 NonNegativeFloat = Annotated[float, annotated_types.Ge(0)]
+"""A float that must be greater than or equal to zero."""
 StrictFloat = Annotated[float, Strict(True)]
+"""A float that must be validated in strict mode."""
 FiniteFloat = Annotated[float, AllowInfNan(False)]
+"""A float that must be finite (not ``-inf``, ``inf``, or ``nan``)."""
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ BYTES TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 def conbytes(
     *,
     min_length: int | None = None,
     max_length: int | None = None,
     strict: bool | None = None,
 ) -> type[bytes]:
+    """A wrapper around `bytes` that allows for additional constraints.
+
+    Args:
+        min_length: The minimum length of the bytes.
+        max_length: The maximum length of the bytes.
+        strict: Whether to validate the bytes in strict mode.
+
+    Returns:
+        The wrapped bytes type.
+    """
     return Annotated[  # type: ignore[return-value]
         bytes,
         Strict(strict) if strict is not None else None,
         annotated_types.Len(min_length or 0, max_length),
     ]
 
 
 StrictBytes = Annotated[bytes, Strict()]
+"""A bytes that must be validated in strict mode."""
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ STRING TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 def constr(
     *,
@@ -205,45 +254,80 @@
     to_upper: bool | None = None,
     to_lower: bool | None = None,
     strict: bool | None = None,
     min_length: int | None = None,
     max_length: int | None = None,
     pattern: str | None = None,
 ) -> type[str]:
+    """A wrapper around `str` that allows for additional constraints.
+
+    Args:
+        strip_whitespace: Whether to strip whitespace from the string.
+        to_upper: Whether to convert the string to uppercase.
+        to_lower: Whether to convert the string to lowercase.
+        strict: Whether to validate the string in strict mode.
+        min_length: The minimum length of the string.
+        max_length: The maximum length of the string.
+        pattern: A regex pattern that the string must match.
+
+    Returns:
+        The wrapped string type.
+    """
     return Annotated[  # type: ignore[return-value]
         str,
         Strict(strict) if strict is not None else None,
         annotated_types.Len(min_length or 0, max_length),
         _fields.PydanticGeneralMetadata(
             strip_whitespace=strip_whitespace,
             to_upper=to_upper,
             to_lower=to_lower,
             pattern=pattern,
         ),
     ]
 
 
 StrictStr = Annotated[str, Strict()]
+"""A string that must be validated in strict mode."""
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~ COLLECTION TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 HashableItemType = TypeVar('HashableItemType', bound=Hashable)
 
 
 def conset(
     item_type: type[HashableItemType], *, min_length: int | None = None, max_length: int | None = None
 ) -> type[set[HashableItemType]]:
+    """A wrapper around `typing.Set` that allows for additional constraints.
+
+    Args:
+        item_type: The type of the items in the set.
+        min_length: The minimum length of the set.
+        max_length: The maximum length of the set.
+
+    Returns:
+        The wrapped set type.
+    """
     return Annotated[  # type: ignore[return-value]
         Set[item_type], annotated_types.Len(min_length or 0, max_length)  # type: ignore[valid-type]
     ]
 
 
 def confrozenset(
     item_type: type[HashableItemType], *, min_length: int | None = None, max_length: int | None = None
 ) -> type[frozenset[HashableItemType]]:
+    """A wrapper around `typing.FrozenSet` that allows for additional constraints.
+
+    Args:
+        item_type: The type of the items in the frozenset.
+        min_length: The minimum length of the frozenset.
+        max_length: The maximum length of the frozenset.
+
+    Returns:
+        The wrapped frozenset type.
+    """
     return Annotated[  # type: ignore[return-value]
         FrozenSet[item_type],  # type: ignore[valid-type]
         annotated_types.Len(min_length or 0, max_length),
     ]
 
 
 AnyItemType = TypeVar('AnyItemType')
@@ -255,29 +339,29 @@
     min_length: int | None = None,
     max_length: int | None = None,
     unique_items: bool | None = None,
 ) -> type[list[AnyItemType]]:
     """A wrapper around typing.List that adds validation.
 
     Args:
-        item_type (type[AnyItemType]): The type of the items in the list.
-        min_length (int | None, optional): The minimum length of the list. Defaults to None.
-        max_length (int | None, optional): The maximum length of the list. Defaults to None.
-        unique_items (bool | None, optional): Whether the items in the list must be unique. Defaults to None.
+        item_type: The type of the items in the list.
+        min_length: The minimum length of the list. Defaults to None.
+        max_length: The maximum length of the list. Defaults to None.
+        unique_items: Whether the items in the list must be unique. Defaults to None.
 
     Returns:
-        type[list[AnyItemType]]: The wrapped list type.
+        The wrapped list type.
     """
     if unique_items is not None:
         raise PydanticUserError(
             (
                 '`unique_items` is removed, use `Set` instead'
                 '(this feature is discussed in https://github.com/pydantic/pydantic-core/issues/296)'
             ),
-            code='deprecated-kwargs',
+            code='removed-kwargs',
         )
     return Annotated[  # type: ignore[return-value]
         List[item_type],  # type: ignore[valid-type]
         annotated_types.Len(min_length or 0, max_length),
     ]
 
 
@@ -285,14 +369,33 @@
 
 AnyType = TypeVar('AnyType')
 if TYPE_CHECKING:
     ImportString = Annotated[AnyType, ...]
 else:
 
     class ImportString:
+        """A type that can be used to import a type from a string.
+
+        Example:
+            ```py
+            from datetime import date
+            from typing import Type
+
+            from pydantic import BaseModel, ImportString
+
+
+            class Foo(BaseModel):
+                call_date: ImportString[Type[date]]
+
+
+            foo = Foo(call_date="datetime.date")
+            assert foo.call_date(2021, 1, 1) == date(2021, 1, 1)
+            ```
+        """
+
         @classmethod
         def __class_getitem__(cls, item: AnyType) -> AnyType:
             return Annotated[item, cls()]
 
         @classmethod
         def __get_pydantic_core_schema__(
             cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
@@ -332,14 +435,27 @@
     lt: int | Decimal | None = None,
     le: int | Decimal | None = None,
     multiple_of: int | Decimal | None = None,
     max_digits: int | None = None,
     decimal_places: int | None = None,
     allow_inf_nan: bool | None = None,
 ) -> type[Decimal]:
+    """A wrapper around Decimal that adds validation.
+
+    Args:
+        strict: Whether to validate the value in strict mode. Defaults to `None`.
+        gt: The value must be greater than this. Defaults to `None`.
+        ge: The value must be greater than or equal to this. Defaults to `None`.
+        lt: The value must be less than this. Defaults to `None`.
+        le: The value must be less than or equal to this. Defaults to `None`.
+        multiple_of: The value must be a multiple of this. Defaults to `None`.
+        max_digits: The maximum number of digits. Defaults to `None`.
+        decimal_places: The number of decimal places. Defaults to `None`.
+        allow_inf_nan: Whether to allow infinity and NaN. Defaults to `None`.
+    """
     return Annotated[  # type: ignore[return-value]
         Decimal,
         Strict(strict) if strict is not None else None,
         annotated_types.Interval(gt=gt, ge=ge, lt=lt, le=le),
         annotated_types.MultipleOf(multiple_of) if multiple_of is not None else None,
         _fields.PydanticGeneralMetadata(max_digits=max_digits, decimal_places=decimal_places),
         AllowInfNan(allow_inf_nan) if allow_inf_nan is not None else None,
@@ -376,17 +492,21 @@
         return value
 
     def __hash__(self) -> int:
         return hash(type(self.uuid_version))
 
 
 UUID1 = Annotated[UUID, UuidVersion(1)]
+"""A UUID1 annotated type."""
 UUID3 = Annotated[UUID, UuidVersion(3)]
+"""A UUID3 annotated type."""
 UUID4 = Annotated[UUID, UuidVersion(4)]
+"""A UUID4 annotated type."""
 UUID5 = Annotated[UUID, UuidVersion(5)]
+"""A UUID5 annotated type."""
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ PATH TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 @_dataclasses.dataclass
 class PathType:
@@ -438,26 +558,31 @@
             return path
 
     def __hash__(self) -> int:
         return hash(type(self.path_type))
 
 
 FilePath = Annotated[Path, PathType('file')]
+"""A path that must point to a file."""
 DirectoryPath = Annotated[Path, PathType('dir')]
+"""A path that must point to a directory."""
 NewPath = Annotated[Path, PathType('new')]
+"""A path for a new file or directory that must not already exist."""
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ JSON TYPE ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 if TYPE_CHECKING:
     Json = Annotated[AnyType, ...]  # Json[list[str]] will be recognized by type checkers as list[str]
 
 else:
 
     class Json:
+        """A special type wrapper which loads JSON before parsing."""
+
         @classmethod
         def __class_getitem__(cls, item: AnyType) -> AnyType:
             return Annotated[item, cls()]
 
         @classmethod
         def __get_pydantic_core_schema__(
             cls, source: Any, handler: _annotated_handlers.GetCoreSchemaHandler
@@ -478,19 +603,24 @@
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ SECRET TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 SecretType = TypeVar('SecretType', str, bytes)
 
 
-class SecretField(Generic[SecretType]):
+class _SecretField(Generic[SecretType]):
     def __init__(self, secret_value: SecretType) -> None:
         self._secret_value: SecretType = secret_value
 
     def get_secret_value(self) -> SecretType:
+        """Get the secret value.
+
+        Returns:
+            The secret value.
+        """
         return self._secret_value
 
     @classmethod
     def __prepare_pydantic_annotations__(
         cls, source: type[Any], annotations: tuple[Any, ...], _config: ConfigDict
     ) -> tuple[Any, Iterable[Any]]:
         metadata, remaining_annotations = _known_annotated_metadata.collect_known_metadata(annotations)
@@ -526,36 +656,36 @@
     if isinstance(value, bytes):
         value = value.decode()
     return '**********' if value else ''
 
 
 @_internal_dataclass.slots_dataclass
 class _SecretFieldValidator:
-    field_type: type[SecretField[Any]]
+    field_type: type[_SecretField[Any]]
     min_length: int | None = None
     max_length: int | None = None
     inner_schema: CoreSchema = _dataclasses.field(init=False)
 
-    def validate(self, value: SecretField[SecretType] | SecretType, _: core_schema.ValidationInfo) -> Any:
+    def validate(self, value: _SecretField[SecretType] | SecretType, _: core_schema.ValidationInfo) -> Any:
         error_prefix: Literal['string', 'bytes'] = 'string' if self.field_type is SecretStr else 'bytes'
         if self.min_length is not None and len(value) < self.min_length:
             short_kind: core_schema.ErrorType = f'{error_prefix}_too_short'  # type: ignore[assignment]
             raise PydanticKnownError(short_kind, {'min_length': self.min_length})
         if self.max_length is not None and len(value) > self.max_length:
             long_kind: core_schema.ErrorType = f'{error_prefix}_too_long'  # type: ignore[assignment]
             raise PydanticKnownError(long_kind, {'max_length': self.max_length})
 
         if isinstance(value, self.field_type):
             return value
         else:
             return self.field_type(value)  # type: ignore[arg-type]
 
     def serialize(
-        self, value: SecretField[SecretType], info: core_schema.SerializationInfo
-    ) -> str | SecretField[SecretType]:
+        self, value: _SecretField[SecretType], info: core_schema.SerializationInfo
+    ) -> str | _SecretField[SecretType]:
         if info.mode == 'json':
             # we want the output to always be string without the `b'` prefix for bytes,
             # hence we just use `secret_display`
             return _secret_display(value.get_secret_value())
         else:
             return value
 
@@ -593,20 +723,41 @@
                 info_arg=True,
                 return_schema=core_schema.str_schema(),
                 when_used='json',
             ),
         )
 
 
-class SecretStr(SecretField[str]):
+class SecretStr(_SecretField[str]):
+    """A string that is displayed as `**********` in reprs and can be used for passwords.
+
+    Example:
+        ```py
+        from pydantic import BaseModel, SecretStr
+
+        class User(BaseModel):
+            username: str
+            password: SecretStr
+
+        user = User(username='scolvin', password='password1')
+
+        print(user)
+        #> username='scolvin' password=SecretStr('**********')
+        print(user.password.get_secret_value())
+        #> password1
+        ```
+    """
+
     def _display(self) -> str:
         return _secret_display(self.get_secret_value())
 
 
-class SecretBytes(SecretField[bytes]):
+class SecretBytes(_SecretField[bytes]):
+    """A bytes that is displayed as `**********` in reprs and can be used for passwords."""
+
     def _display(self) -> bytes:
         return _secret_display(self.get_secret_value()).encode()
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ PAYMENT CARD TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
@@ -616,18 +767,20 @@
     visa = 'Visa'
     other = 'other'
 
     def __str__(self) -> str:
         return self.value
 
 
+@deprecated(
+    'The `PaymentCardNumber` class is deprecated, use `pydantic_extra_types` instead. '
+    'See https://pydantic-docs.helpmanual.io/usage/types/extra_types/payment_cards/.'
+)
 class PaymentCardNumber(str):
-    """
-    Based on: https://en.wikipedia.org/wiki/Payment_card_number
-    """
+    """Based on: https://en.wikipedia.org/wiki/Payment_card_number."""
 
     strip_whitespace: ClassVar[bool] = True
     min_length: ClassVar[int] = 12
     max_length: ClassVar[int] = 19
     bin: str
     last4: str
     brand: PaymentCardBrand
@@ -650,31 +803,36 @@
             core_schema.str_schema(
                 min_length=cls.min_length, max_length=cls.max_length, strip_whitespace=cls.strip_whitespace
             ),
         )
 
     @classmethod
     def validate(cls, __input_value: str, _: core_schema.ValidationInfo) -> PaymentCardNumber:
+        """Validate the card number and return a `PaymentCardNumber` instance."""
         return cls(__input_value)
 
     @property
     def masked(self) -> str:
+        """Mask all but the last 4 digits of the card number.
+
+        Returns:
+            A masked card number string.
+        """
         num_masked = len(self) - 10  # len(bin) + len(last4) == 10
         return f'{self.bin}{"*" * num_masked}{self.last4}'
 
     @classmethod
     def validate_digits(cls, card_number: str) -> None:
+        """Validate that the card number is all digits."""
         if not card_number.isdigit():
             raise PydanticCustomError('payment_card_number_digits', 'Card number is not all digits')
 
     @classmethod
     def validate_luhn_check_digit(cls, card_number: str) -> str:
-        """
-        Based on: https://en.wikipedia.org/wiki/Luhn_algorithm
-        """
+        """Based on: https://en.wikipedia.org/wiki/Luhn_algorithm."""
         sum_ = int(card_number[-1])
         length = len(card_number)
         parity = length % 2
         for i in range(length - 1):
             digit = int(card_number[i])
             if i % 2 == parity:
                 digit *= 2
@@ -684,17 +842,16 @@
         valid = sum_ % 10 == 0
         if not valid:
             raise PydanticCustomError('payment_card_number_luhn', 'Card number is not luhn valid')
         return card_number
 
     @staticmethod
     def validate_brand(card_number: str) -> PaymentCardBrand:
-        """
-        Validate length based on BIN for major brands:
-        https://en.wikipedia.org/wiki/Payment_card_number#Issuer_identification_number_(IIN)
+        """Validate length based on BIN for major brands:
+        https://en.wikipedia.org/wiki/Payment_card_number#Issuer_identification_number_(IIN).
         """
         if card_number[0] == '4':
             brand = PaymentCardBrand.visa
         elif 51 <= int(card_number[:2]) <= 55:
             brand = PaymentCardBrand.mastercard
         elif card_number[:2] in {'34', '37'}:
             brand = PaymentCardBrand.amex
@@ -741,22 +898,24 @@
     'eib': 2**60,
 }
 BYTE_SIZES.update({k.lower()[0]: v for k, v in BYTE_SIZES.items() if 'i' not in k})
 byte_string_re = re.compile(r'^\s*(\d*\.?\d+)\s*(\w+)?', re.IGNORECASE)
 
 
 class ByteSize(int):
+    """Converts a bytes string with units to the number of bytes."""
+
     @classmethod
     def __get_pydantic_core_schema__(
         cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
-        return core_schema.general_plain_validator_function(cls.validate)
+        return core_schema.general_plain_validator_function(cls._validate)
 
     @classmethod
-    def validate(cls, __input_value: Any, _: core_schema.ValidationInfo) -> ByteSize:
+    def _validate(cls, __input_value: Any, _: core_schema.ValidationInfo) -> ByteSize:
         try:
             return cls(int(__input_value))
         except ValueError:
             pass
 
         str_match = byte_string_re.match(str(__input_value))
         if str_match is None:
@@ -770,14 +929,23 @@
             unit_mult = BYTE_SIZES[unit.lower()]
         except KeyError:
             raise PydanticCustomError('byte_size_unit', 'could not interpret byte unit: {unit}', {'unit': unit})
 
         return cls(int(float(scalar) * unit_mult))
 
     def human_readable(self, decimal: bool = False) -> str:
+        """Converts a byte size to a human readable string.
+
+        Args:
+            decimal: If True, use decimal units (e.g. 1000 bytes per KB). If False, use binary units
+                (e.g. 1024 bytes per KiB).
+
+        Returns:
+            A human readable string representation of the byte size.
+        """
         if decimal:
             divisor = 1000
             units = 'B', 'KB', 'MB', 'GB', 'TB', 'PB'
             final_unit = 'EB'
         else:
             divisor = 1024
             units = 'B', 'KiB', 'MiB', 'GiB', 'TiB', 'PiB'
@@ -791,14 +959,23 @@
                 else:
                     return f'{num:0.1f}{unit}'
             num /= divisor
 
         return f'{num:0.1f}{final_unit}'
 
     def to(self, unit: str) -> float:
+        """Converts a byte size to another unit.
+
+        Args:
+            unit: The unit to convert to. Must be one of the following: B, KB, MB, GB, TB, PB, EiB,
+                KiB, MiB, GiB, TiB, PiB, EiB.
+
+        Returns:
+            The byte size in the new unit.
+        """
         try:
             unit_div = BYTE_SIZES[unit.lower()]
         except KeyError:
             raise PydanticCustomError('byte_size_unit', 'Could not interpret byte unit: {unit}', {'unit': unit})
 
         return self / unit_div
 
@@ -813,14 +990,16 @@
 
 if TYPE_CHECKING:
     PastDate = Annotated[date, ...]
     FutureDate = Annotated[date, ...]
 else:
 
     class PastDate:
+        """A date in the past."""
+
         @classmethod
         def __get_pydantic_core_schema__(
             cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
         ) -> core_schema.CoreSchema:
             if cls is source:
                 # used directly as a type
                 return core_schema.date_schema(now_op='past')
@@ -830,14 +1009,16 @@
                 schema['now_op'] = 'past'
                 return schema
 
         def __repr__(self) -> str:
             return 'PastDate'
 
     class FutureDate:
+        """A date in the future."""
+
         @classmethod
         def __get_pydantic_core_schema__(
             cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
         ) -> core_schema.CoreSchema:
             if cls is source:
                 # used directly as a type
                 return core_schema.date_schema(now_op='future')
@@ -855,14 +1036,26 @@
     *,
     strict: bool | None = None,
     gt: date | None = None,
     ge: date | None = None,
     lt: date | None = None,
     le: date | None = None,
 ) -> type[date]:
+    """A wrapper for date that adds constraints.
+
+    Args:
+        strict: Whether to validate the date value in strict mode. Defaults to `None`.
+        gt: The value must be greater than this. Defaults to `None`.
+        ge: The value must be greater than or equal to this. Defaults to `None`.
+        lt: The value must be less than this. Defaults to `None`.
+        le: The value must be less than or equal to this. Defaults to `None`.
+
+    Returns:
+        A date type with the specified constraints.
+    """
     return Annotated[  # type: ignore[return-value]
         date,
         Strict(strict) if strict is not None else None,
         annotated_types.Interval(gt=gt, ge=ge, lt=lt, le=le),
     ]
 
 
@@ -873,14 +1066,16 @@
     NaiveDatetime = Annotated[datetime, ...]
     PastDatetime = Annotated[datetime, ...]
     FutureDatetime = Annotated[datetime, ...]
 
 else:
 
     class AwareDatetime:
+        """A datetime that requires timezone info."""
+
         @classmethod
         def __get_pydantic_core_schema__(
             cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
         ) -> core_schema.CoreSchema:
             if cls is source:
                 # used directly as a type
                 return core_schema.datetime_schema(tz_constraint='aware')
@@ -890,14 +1085,16 @@
                 schema['tz_constraint'] = 'aware'
                 return schema
 
         def __repr__(self) -> str:
             return 'AwareDatetime'
 
     class NaiveDatetime:
+        """A datetime that doesn't require timezone info."""
+
         @classmethod
         def __get_pydantic_core_schema__(
             cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
         ) -> core_schema.CoreSchema:
             if cls is source:
                 # used directly as a type
                 return core_schema.datetime_schema(tz_constraint='naive')
@@ -907,14 +1104,16 @@
                 schema['tz_constraint'] = 'naive'
                 return schema
 
         def __repr__(self) -> str:
             return 'NaiveDatetime'
 
     class PastDatetime:
+        """A datetime that must be in the past."""
+
         @classmethod
         def __get_pydantic_core_schema__(
             cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
         ) -> core_schema.CoreSchema:
             if cls is source:
                 # used directly as a type
                 return core_schema.datetime_schema(now_op='past')
@@ -924,14 +1123,16 @@
                 schema['now_op'] = 'past'
                 return schema
 
         def __repr__(self) -> str:
             return 'PastDatetime'
 
     class FutureDatetime:
+        """A datetime that must be in the future."""
+
         @classmethod
         def __get_pydantic_core_schema__(
             cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
         ) -> core_schema.CoreSchema:
             if cls is source:
                 # used directly as a type
                 return core_schema.datetime_schema(now_op='future')
@@ -945,47 +1146,94 @@
             return 'FutureDatetime'
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ Encoded TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 class EncoderProtocol(Protocol):
+    """Protocol for encoding and decoding data to and from bytes."""
+
     @classmethod
     def decode(cls, data: bytes) -> bytes:
-        """Can throw `PydanticCustomError`"""
+        """Decode the data using the encoder.
+
+        Args:
+            data: The data to decode.
+
+        Returns:
+            The decoded data.
+        """
         ...
 
     @classmethod
     def encode(cls, value: bytes) -> bytes:
+        """Encode the data using the encoder.
+
+        Args:
+            value: The data to encode.
+
+        Returns:
+            The encoded data.
+        """
         ...
 
     @classmethod
     def get_json_format(cls) -> str:
+        """Get the JSON format for the encoded data.
+
+        Returns:
+            The JSON format for the encoded data.
+        """
         ...
 
 
 class Base64Encoder(EncoderProtocol):
+    """Base64 encoder."""
+
     @classmethod
     def decode(cls, data: bytes) -> bytes:
+        """Decode the data from base64 encoded bytes to original bytes data.
+
+        Args:
+            data: The data to decode.
+
+        Returns:
+            The decoded data.
+        """
         try:
             return base64.decodebytes(data)
         except ValueError as e:
             raise PydanticCustomError('base64_decode', "Base64 decoding error: '{error}'", {'error': str(e)})
 
     @classmethod
     def encode(cls, value: bytes) -> bytes:
+        """Encode the data from bytes to a base64 encoded bytes.
+
+        Args:
+            value: The data to encode.
+
+        Returns:
+            The encoded data.
+        """
         return base64.encodebytes(value)
 
     @classmethod
-    def get_json_format(cls) -> str:
+    def get_json_format(cls) -> Literal['base64']:
+        """Get the JSON format for the encoded data.
+
+        Returns:
+            The JSON format for the encoded data.
+        """
         return 'base64'
 
 
 @_internal_dataclass.slots_dataclass
 class EncodedBytes:
+    """A bytes type that is encoded and decoded using the specified encoder."""
+
     encoder: type[EncoderProtocol]
 
     def __get_pydantic_json_schema__(
         self, core_schema: core_schema.CoreSchema, handler: _annotated_handlers.GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         field_schema = handler(core_schema)
         field_schema.update(type='string', format=self.encoder.get_json_format())
@@ -997,138 +1245,84 @@
         return core_schema.general_after_validator_function(
             function=self.decode,
             schema=core_schema.bytes_schema(),
             serialization=core_schema.plain_serializer_function_ser_schema(function=self.encode),
         )
 
     def decode(self, data: bytes, _: core_schema.ValidationInfo) -> bytes:
+        """Decode the data using the specified encoder.
+
+        Args:
+            data: The data to decode.
+
+        Returns:
+            The decoded data.
+        """
         return self.encoder.decode(data)
 
     def encode(self, value: bytes) -> bytes:
+        """Encode the data using the specified encoder.
+
+        Args:
+            value: The data to encode.
+
+        Returns:
+            The encoded data.
+        """
         return self.encoder.encode(value)
 
     def __hash__(self) -> int:
         return hash(self.encoder)
 
 
 class EncodedStr(EncodedBytes):
+    """A str type that is encoded and decoded using the specified encoder."""
+
     def __get_pydantic_core_schema__(
         self, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
     ) -> core_schema.CoreSchema:
         return core_schema.general_after_validator_function(
             function=self.decode_str,
             schema=super().__get_pydantic_core_schema__(source=source, handler=handler),
             serialization=core_schema.plain_serializer_function_ser_schema(function=self.encode_str),
         )
 
     def decode_str(self, data: bytes, _: core_schema.ValidationInfo) -> str:
+        """Decode the data using the specified encoder.
+
+        Args:
+            data: The data to decode.
+
+        Returns:
+            The decoded data.
+        """
         return data.decode()
 
     def encode_str(self, value: str) -> str:
+        """Encode the data using the specified encoder.
+
+        Args:
+            value: The data to encode.
+
+        Returns:
+            The encoded data.
+        """
         return super().encode(value=value.encode()).decode()
 
 
 Base64Bytes = Annotated[bytes, EncodedBytes(encoder=Base64Encoder)]
 Base64Str = Annotated[str, EncodedStr(encoder=Base64Encoder)]
 
 
-if TYPE_CHECKING:
-    # If we add configurable attributes to IsInstance, we'd probably need to stop hiding it from type checkers like this
-    InstanceOf = Annotated[AnyType, ...]  # `IsInstance[Sequence]` will be recognized by type checkers as `Sequence`
-
-else:
-
-    @_internal_dataclass.slots_dataclass
-    class InstanceOf:
-        @classmethod
-        def __class_getitem__(cls, item: AnyType) -> AnyType:
-            return Annotated[item, cls()]
-
-        @classmethod
-        def __get_pydantic_core_schema__(
-            cls, source: Any, handler: _annotated_handlers.GetCoreSchemaHandler
-        ) -> core_schema.CoreSchema:
-            from pydantic import PydanticSchemaGenerationError
-
-            # use the generic _origin_ as the second argument to isinstance when appropriate
-            python_schema = core_schema.is_instance_schema(_generics.get_origin(source) or source)
-
-            try:
-                # Try to generate the "standard" schema, which will be used when loading from JSON
-                json_schema = handler(source)
-            except PydanticSchemaGenerationError:
-                # If that fails, just produce a schema that can validate from python
-                return python_schema
-            else:
-                return core_schema.json_or_python_schema(python_schema=python_schema, json_schema=json_schema)
-
-
 __getattr__ = getattr_migration(__name__)
 
 
 @_internal_dataclass.slots_dataclass
-class WithJsonSchema:
-    """
-    Add this as an annotation on a field to override the (base) JSON schema that would be generated for that field.
-
-    This provides a way to set a JSON schema for types that would otherwise raise errors when producing a JSON schema,
-    such as Callable, or types that have an is-instance core schema, without needing to go so far as creating a
-    custom subclass of pydantic.json_schema.GenerateJsonSchema.
-
-    Note that any _modifications_ to the schema that would normally be made (such as setting the title for model fields)
-    will still be performed.
-    """
-
-    json_schema: JsonSchemaValue | None
-
-    def __get_pydantic_json_schema__(
-        self, _core_schema: core_schema.CoreSchema, handler: _annotated_handlers.GetJsonSchemaHandler
-    ) -> JsonSchemaValue:
-        if self.json_schema is None:
-            # This exception is handled in pydantic.json_schema.GenerateJsonSchema._named_required_fields_schema
-            raise PydanticOmit
-        else:
-            return self.json_schema
-
-
-if TYPE_CHECKING:
-    SkipValidation = Annotated[AnyType, ...]  # SkipValidation[list[str]] will be treated by type checkers as list[str]
-else:
-
-    @_internal_dataclass.slots_dataclass
-    class SkipValidation:
-        """
-        If this is applied as an annotation (e.g., via `x: Annotated[int, SkipValidation]`), validation will be skipped.
-        You can also use `SkipValidation[int]` as a shorthand for `Annotated[int, SkipValidation]`.
-
-        This can be useful if you want to use a type annotation for documentation/IDE/type-checking purposes,
-        and know that it is safe to skip validation for one or more of the fields.
-
-        Because this converts the validation schema to `any_schema`, subsequent annotation-applied transformations
-        may not have the expected effects. Therefore, when used, this annotation should generally be the final
-        annotation applied to a type.
-        """
-
-        def __class_getitem__(cls, item: Any) -> Any:
-            return Annotated[item, SkipValidation()]
-
-        @classmethod
-        def __get_pydantic_core_schema__(
-            cls, source: Any, handler: _annotated_handlers.GetCoreSchemaHandler
-        ) -> core_schema.CoreSchema:
-            original_schema = handler.generate_schema(source)
-            metadata = _core_metadata.build_metadata_dict(js_functions=[lambda _c, h: h(original_schema)])
-            return core_schema.any_schema(metadata=metadata, serialization=original_schema)
-
-
-@_internal_dataclass.slots_dataclass
 class TransformSchema:
-    """
-    An annotation that can be used to apply a transform to a core schema.
-    """
+    """An annotation that can be used to apply a transform to a core schema."""
 
     transform: Callable[[CoreSchema], CoreSchema]
 
     def __get_pydantic_core_schema__(
         self, source_type: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
     ) -> CoreSchema:
         return self.transform(handler(source_type))
```

### Comparing `pydantic-2.0b2/pydantic/validate_call.py` & `pydantic-2.0b3/pydantic/validate_call.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 
 def validate_call(
     __func: AnyCallableT | None = None,
     *,
     config: ConfigDict | None = None,
     validate_return: bool = False,
 ) -> AnyCallableT | Callable[[AnyCallableT], AnyCallableT]:
-    """
-    Decorator to validate the arguments passed to a function and, optionally, the return value.
+    """Returns a decorated version of the function that validates the arguments and, optionally, the return value.
 
     Args:
         __func: The function to be decorated.
         config: The configuration dictionary.
         validate_return: Whether to validate the return value.
 
     Returns:
```

### Comparing `pydantic-2.0b2/pydantic/version.py` & `pydantic-2.0b3/pydantic/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""The `version` module holds the version information for Pydantic."""
 __all__ = 'VERSION', 'version_info'
 
-VERSION = '2.0b2'
+VERSION = '2.0b3'
+"""The version of Pydantic."""
 
 
 def version_info() -> str:
+    """Return complete version information for Pydantic and its dependencies."""
     import platform
     import sys
     from importlib import import_module
     from pathlib import Path
 
     import pydantic_core._pydantic_core as pdc
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_annotated_handlers.py` & `pydantic-2.0b3/pydantic/_internal/_annotated_handlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,18 @@
         core_schema.ComputedField,
     ]
 
 __all__ = 'GetJsonSchemaHandler', 'GetCoreSchemaHandler'
 
 
 class GetJsonSchemaHandler:
-    """
-    Handler to call into the next JSON schema generation function
+    """Handler to call into the next JSON schema generation function.
+
+    Attributes:
+        mode: Json schema mode, can be `validation` or `serialization`.
     """
 
     mode: JsonSchemaMode
 
     def __call__(self, __core_schema: CoreSchemaOrField) -> JsonSchemaValue:
         """Call the inner handler and get the JsonSchemaValue it returns.
         This will call the next JSON schema modifying function up until it calls
@@ -32,65 +34,77 @@
         `pydantic.errors.PydanticInvalidForJsonSchema` error if it cannot generate
         a JSON schema.
 
         Args:
             __core_schema: A `pydantic_core.core_schema.CoreSchema`.
 
         Returns:
-            JsonSchemaValue: the JSON schema generated by the inner JSON schema modify
+            JsonSchemaValue: The JSON schema generated by the inner JSON schema modify
             functions.
         """
         raise NotImplementedError
 
     def resolve_ref_schema(self, __maybe_ref_json_schema: JsonSchemaValue) -> JsonSchemaValue:
         """Get the real schema for a `{"$ref": ...}` schema.
         If the schema given is not a `$ref` schema, it will be returned as is.
         This means you don't have to check before calling this function.
 
         Args:
             __maybe_ref_json_schema: A JsonSchemaValue, ref based or not.
 
         Raises:
-            LookupError: if the ref is not found.
+            LookupError: If the ref is not found.
 
         Returns:
             JsonSchemaValue: A JsonSchemaValue that has no `$ref`.
         """
         raise NotImplementedError
 
 
 class GetCoreSchemaHandler:
-    """
-    Handler to call into the next CoreSchema schema generation function
-    """
+    """Handler to call into the next CoreSchema schema generation function."""
 
     def __call__(self, __source_type: Any) -> core_schema.CoreSchema:
-        """
-        Call the inner handler and get the CoreSchema it returns.
+        """Call the inner handler and get the CoreSchema it returns.
         This will call the next CoreSchema modifying function up until it calls
         into Pydantic's internal schema generation machinery, which will raise a
         `pydantic.errors.PydanticSchemaGenerationError` error if it cannot generate
         a CoreSchema for the given source type.
 
         Args:
             __source_type: The input type.
 
         Returns:
-            CoreSchema: the `pydantic-core` CoreSchema generated.
+            CoreSchema: The `pydantic-core` CoreSchema generated.
         """
         raise NotImplementedError
 
     def generate_schema(self, __source_type: Any) -> core_schema.CoreSchema:
-        """
-        Generate a schema unrelated to the current context.
+        """Generate a schema unrelated to the current context.
         Use this function if e.g. you are handling schema generation for a sequence
         and want to generate a schema for its items.
         Otherwise, you may end up doing something like applying a `min_length` constraint
         that was intended for the sequence itself to it's items!
 
         Args:
             __source_type: The input type.
 
         Returns:
-            CoreSchema: the `pydantic-core` CoreSchema generated.
+            CoreSchema: The `pydantic-core` CoreSchema generated.
+        """
+        raise NotImplementedError
+
+    def resolve_ref_schema(self, __maybe_ref_schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
+        """Get the real schema for a `definition-ref` schema.
+        If the schema given is not a `definition-ref` schema, it will be returned as is.
+        This means you don't have to check before calling this function.
+
+        Args:
+            __maybe_ref_schema: A `CoreSchema`, `ref`-based or not.
+
+        Raises:
+            LookupError: If the `ref` is not found.
+
+        Returns:
+            A concrete `CoreSchema`.
         """
         raise NotImplementedError
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_config.py` & `pydantic-2.0b3/pydantic/_internal/_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from ..config import ConfigDict, ExtraValues, JsonSchemaExtraCallable
 from ..errors import PydanticUserError
 
 DEPRECATION_MESSAGE = 'Support for class-based `config` is deprecated, use ConfigDict instead.'
 
 
 class ConfigWrapper:
-    """
-    Internal wrapper for Config which exposes ConfigDict items as attributes.
-    """
+    """Internal wrapper for Config which exposes ConfigDict items as attributes."""
 
     __slots__ = ('config_dict',)
 
     config_dict: ConfigDict
 
     # all annotations are copied directly from ConfigDict, and should be kept up to date, a test will fail if they
     # stop matching
@@ -60,25 +58,29 @@
         if check:
             self.config_dict = prepare_config(config)
         else:
             self.config_dict = cast(ConfigDict, config)
 
     @classmethod
     def for_model(cls, bases: tuple[type[Any], ...], namespace: dict[str, Any], kwargs: dict[str, Any]) -> Self:
-        """
-        Build a new `ConfigDict` instance for a `BaseModel` based on (from lowest to highest)
-        - options defined in base
-        - options defined in namespace
-        - options defined via kwargs
-
-        :param bases: tuple of base classes
-        :param namespace: namespace of the class being created
-        :param kwargs: kwargs passed to the class being created
-        """
+        """Build a new `ConfigWrapper` instance for a `BaseModel`.
 
+        The config wrapper built based on (in descending order of priority):
+        - options from `kwargs`
+        - options from the `namespace`
+        - options from the base classes (`bases`)
+
+        Args:
+            bases: A tuple of base classes.
+            namespace: The namespace of the class being created.
+            kwargs: The kwargs passed to the class being created.
+
+        Returns:
+            A `ConfigWrapper` instance for `BaseModel`.
+        """
         config_new = ConfigDict()
         for base in bases:
             config = getattr(base, 'model_config', None)
             if config:
                 config_new.update(config.copy())
 
         config_class_from_namespace = namespace.get('Config')
@@ -107,20 +109,25 @@
             except KeyError:
                 try:
                     return config_defaults[name]
                 except KeyError:
                     raise AttributeError(f'Config has no attribute {name!r}') from None
 
     def core_config(self, obj: Any) -> core_schema.CoreConfig:
-        """
-        Create a pydantic-core config, `obj` is just used to populate `title` if not set in config.
+        """Create a pydantic-core config, `obj` is just used to populate `title` if not set in config.
 
         Pass `obj=None` if you do not want to attempt to infer the `title`.
 
         We don't use getattr here since we don't want to populate with defaults.
+
+        Args:
+            obj: An object used to populate `title` if not set in config.
+
+        Returns:
+            A `CoreConfig` object created from config.
         """
         core_config = core_schema.CoreConfig(
             **core_schema.dict_not_none(
                 title=self.config_dict.get('title') or (obj and obj.__name__),
                 extra_fields_behavior=self.config_dict.get('extra'),
                 allow_inf_nan=self.config_dict.get('allow_inf_nan'),
                 populate_by_name=self.config_dict.get('populate_by_name'),
@@ -174,16 +181,21 @@
     validate_return=False,
     protected_namespaces=('model_',),
     hide_input_in_errors=False,
 )
 
 
 def prepare_config(config: ConfigDict | dict[str, Any] | type[Any] | None) -> ConfigDict:
-    """
-    Create a `ConfigDict` instance from an existing dict, a class (e.g. old class-based config) or None.
+    """Create a `ConfigDict` instance from an existing dict, a class (e.g. old class-based config) or None.
+
+    Args:
+        config: The input config.
+
+    Returns:
+        A ConfigDict object created from config.
     """
     if config is None:
         return ConfigDict()
 
     if not isinstance(config, dict):
         warnings.warn(DEPRECATION_MESSAGE, DeprecationWarning)
         config = {k: getattr(config, k) for k in dir(config) if not k.startswith('__')}
@@ -220,16 +232,18 @@
     'orm_mode': 'from_attributes',
     'schema_extra': 'json_schema_extra',
     'validate_all': 'validate_default',
 }
 
 
 def check_deprecated(config_dict: ConfigDict) -> None:
-    """
-    Check for deprecated config keys and warn the user.
+    """Check for deprecated config keys and warn the user.
+
+    Args:
+        config_dict: The input config.
     """
     deprecated_removed_keys = V2_REMOVED_KEYS & config_dict.keys()
     deprecated_renamed_keys = V2_RENAMED_KEYS.keys() & config_dict.keys()
     if deprecated_removed_keys or deprecated_renamed_keys:
         renamings = {k: V2_RENAMED_KEYS[k] for k in sorted(deprecated_renamed_keys)}
         renamed_bullets = [f'* {k!r} has been renamed to {v!r}' for k, v in renamings.items()]
         removed_bullets = [f'* {k!r} has been removed' for k in sorted(deprecated_removed_keys)]
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_core_metadata.py` & `pydantic-2.0b3/pydantic/_internal/_core_metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 from __future__ import annotations as _annotations
 
 import typing
 from typing import Any
 
 import typing_extensions
-from pydantic_core import CoreSchema
 
 if typing.TYPE_CHECKING:
-    from ..json_schema import JsonSchemaValue
     from ._schema_generation_shared import (
         CoreSchemaOrField as CoreSchemaOrField,
     )
     from ._schema_generation_shared import (
         GetJsonSchemaFunction,
-        GetJsonSchemaHandler,
     )
 
 
 class CoreMetadata(typing_extensions.TypedDict, total=False):
+    """A `TypedDict` for holding the metadata dict of the schema.
+
+    Attributes:
+        pydantic_js_functions: List of JSON schema functions.
+        pydantic_js_prefer_positional_arguments: Whether JSON schema generator will
+            prefer positional over keyword arguments for an 'arguments' schema.
+    """
+
     pydantic_js_functions: list[GetJsonSchemaFunction]
 
     # If `pydantic_js_prefer_positional_arguments` is True, the JSON schema generator will
     # prefer positional over keyword arguments for an 'arguments' schema.
     pydantic_js_prefer_positional_arguments: bool | None
 
 
-class UpdateCoreSchemaCallable(typing_extensions.Protocol):
-    def __call__(self, schema: CoreSchema, **kwargs: Any) -> None:
-        ...  # pragma: no cover
-
-
 class CoreMetadataHandler:
-    """
-    Because the metadata field in pydantic_core is of type `Any`, we can't assume much about its contents.
+    """Because the metadata field in pydantic_core is of type `Any`, we can't assume much about its contents.
 
     This class is used to interact with the metadata field on a CoreSchema object in a consistent
     way throughout pydantic.
     """
 
     __slots__ = ('_schema',)
 
@@ -47,44 +46,32 @@
         if metadata is None:
             schema['metadata'] = CoreMetadata()
         elif not isinstance(metadata, dict):
             raise TypeError(f'CoreSchema metadata should be a dict; got {metadata!r}.')
 
     @property
     def metadata(self) -> CoreMetadata:
-        """
-        Retrieves the metadata dict off the schema, initializing it to a dict if it is None
+        """Retrieves the metadata dict from the schema, initializing it to a dict if it is None
         and raises an error if it is not a dict.
         """
         metadata = self._schema.get('metadata')
         if metadata is None:
             self._schema['metadata'] = metadata = CoreMetadata()
         if not isinstance(metadata, dict):
             raise TypeError(f'CoreSchema metadata should be a dict; got {metadata!r}.')
         return metadata  # type: ignore[return-value]
 
-    def get_json_schema(
-        self,
-        core_schema: CoreSchemaOrField,
-        handler: GetJsonSchemaHandler,
-    ) -> JsonSchemaValue:
-        js_function = self.metadata.get('pydantic_js_function')
-        if js_function is None:
-            return handler(core_schema)
-        return js_function(core_schema, handler)
-
 
 def build_metadata_dict(
     *,  # force keyword arguments to make it easier to modify this signature in a backwards-compatible way
     js_functions: list[GetJsonSchemaFunction] | None = None,
     js_prefer_positional_arguments: bool | None = None,
     initial_metadata: Any | None = None,
 ) -> Any:
-    """
-    Builds a dict to use as the metadata field of a CoreSchema object in a manner that is consistent
+    """Builds a dict to use as the metadata field of a CoreSchema object in a manner that is consistent
     with the CoreMetadataHandler class.
     """
     if initial_metadata is not None and not isinstance(initial_metadata, dict):
         raise TypeError(f'CoreSchema metadata should be a dict; got {initial_metadata!r}.')
 
     metadata = CoreMetadata(
         pydantic_js_functions=js_functions or [],
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_core_utils.py` & `pydantic-2.0b3/pydantic/_internal/_core_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from collections import defaultdict
-from typing import Any, Callable, Iterable, TypeVar, Union, cast
+from typing import Any, Callable, Hashable, Iterable, TypeVar, Union, cast
 
 from pydantic_core import CoreSchema, core_schema
 from typing_extensions import TypeAliasType, TypeGuard, get_args
 
 from . import _repr
 
 AnyFunctionSchema = Union[
@@ -63,16 +63,15 @@
 ) -> TypeGuard[
     core_schema.ListSchema | core_schema.TupleVariableSchema | core_schema.SetSchema | core_schema.FrozenSetSchema
 ]:
     return schema['type'] in _LIST_LIKE_SCHEMA_WITH_ITEMS_TYPES
 
 
 def get_type_ref(type_: type[Any], args_override: tuple[type[Any], ...] | None = None) -> str:
-    """
-    Produces the ref to be used for this type by pydantic_core's core schemas.
+    """Produces the ref to be used for this type by pydantic_core's core schemas.
 
     This `args_override` argument was added for the purpose of creating valid recursive references
     when creating generic models without needing to create a concrete class.
     """
     origin = type_
     args = args_override or ()
     generic_metadata = getattr(type_, '__pydantic_generic_metadata__', None)
@@ -97,49 +96,14 @@
             arg_ref = f'{_repr.display_as_type(arg)}:{id(arg)}'
         arg_refs.append(arg_ref)
     if arg_refs:
         type_ref = f'{type_ref}[{",".join(arg_refs)}]'
     return type_ref
 
 
-def consolidate_refs(schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
-    """
-    This function walks a schema recursively, replacing all but the first occurrence of each ref with
-    a definition-ref schema referencing that ref.
-
-    This makes the fundamental assumption that any time two schemas have the same ref, occurrences
-    after the first can safely be replaced.
-
-    In most cases, schemas with the same ref should not actually be produced. However, when building recursive
-    models with multiple references to themselves at some level in the field hierarchy, it is difficult to avoid
-    getting multiple (identical) copies of the same schema with the same ref. This function removes the copied refs,
-    but is safe because the "duplicate" refs refer to the same schema.
-
-    There is one case where we purposely emit multiple (different) schemas with the same ref: when building
-    recursive generic models. In this case, as an implementation detail, recursive generic models will emit
-    a _non_-identical schema deeper in the tree with a re-used ref, with the intent that _that_ schema will
-    be replaced with a recursive reference once the specific generic parametrization to use can be determined.
-    """
-    refs: set[str] = set()
-
-    top_ref = schema.get('ref', None)  # type: ignore[assignment]
-
-    def _replace_refs(s: core_schema.CoreSchema, recurse: Recurse) -> core_schema.CoreSchema:
-        ref: str | None = s.get('ref')  # type: ignore[assignment]
-        if ref:
-            if ref is top_ref:
-                return recurse(s, _replace_refs)
-            if ref in refs:
-                return {'type': 'definition-ref', 'schema_ref': ref}
-            refs.add(ref)
-        return recurse(s, _replace_refs)
-
-    return walk_core_schema(schema, _replace_refs)
-
-
 def collect_definitions(schema: core_schema.CoreSchema) -> dict[str, core_schema.CoreSchema]:
     # Only collect valid definitions. This is equivalent to collecting all definitions for "valid" schemas,
     # but allows us to reuse this logic while removing "invalid" definitions
     valid_definitions = dict()
 
     def _record_valid_refs(s: core_schema.CoreSchema, recurse: Recurse) -> core_schema.CoreSchema:
         ref: str | None = s.get('ref')  # type: ignore[assignment]
@@ -246,16 +210,16 @@
             mapping[key] = getattr(self, method_name, self._handle_other_schemas)
         return mapping
 
     def walk(self, schema: core_schema.CoreSchema, f: Walk) -> core_schema.CoreSchema:
         return f(schema.copy(), self._walk)
 
     def _walk(self, schema: core_schema.CoreSchema, f: Walk) -> core_schema.CoreSchema:
-        ser_schema: core_schema.SerSchema | None = schema.get('serialization', None)  # type: ignore
         schema = self._schema_type_to_method[schema['type']](schema, f)
+        ser_schema: core_schema.SerSchema | None = schema.get('serialization', None)  # type: ignore
         if ser_schema:
             schema['serialization'] = self._handle_ser_schemas(ser_schema.copy(), f)
         return schema
 
     def _handle_other_schemas(self, schema: core_schema.CoreSchema, f: Walk) -> core_schema.CoreSchema:
         if 'schema' in schema:
             schema['schema'] = self.walk(schema['schema'], f)  # type: ignore
@@ -338,15 +302,15 @@
         return schema
 
     def handle_union_schema(self, schema: core_schema.UnionSchema, f: Walk) -> core_schema.CoreSchema:
         schema['choices'] = [self.walk(v, f) for v in schema['choices']]
         return schema
 
     def handle_tagged_union_schema(self, schema: core_schema.TaggedUnionSchema, f: Walk) -> core_schema.CoreSchema:
-        new_choices: dict[str | int, str | int | core_schema.CoreSchema] = {}
+        new_choices: dict[Hashable, core_schema.CoreSchema] = {}
         for k, v in schema['choices'].items():
             new_choices[k] = v if isinstance(v, (str, int)) else self.walk(v, f)
         schema['choices'] = new_choices
         return schema
 
     def handle_chain_schema(self, schema: core_schema.ChainSchema, f: Walk) -> core_schema.CoreSchema:
         schema['steps'] = [self.walk(v, f) for v in schema['steps']]
@@ -362,34 +326,55 @@
         schema['python_schema'] = self.walk(schema['python_schema'], f)
         return schema
 
     def handle_model_fields_schema(self, schema: core_schema.ModelFieldsSchema, f: Walk) -> core_schema.CoreSchema:
         if 'extra_validator' in schema:
             schema['extra_validator'] = self.walk(schema['extra_validator'], f)
         replaced_fields: dict[str, core_schema.ModelField] = {}
+        replaced_computed_fields: list[core_schema.ComputedField] = []
+        for computed_field in schema.get('computed_fields', None) or ():
+            replaced_field = computed_field.copy()
+            replaced_field['return_schema'] = self.walk(computed_field['return_schema'], f)
+            replaced_computed_fields.append(replaced_field)
+        if replaced_computed_fields:
+            schema['computed_fields'] = replaced_computed_fields
         for k, v in schema['fields'].items():
             replaced_field = v.copy()
             replaced_field['schema'] = self.walk(v['schema'], f)
             replaced_fields[k] = replaced_field
         schema['fields'] = replaced_fields
         return schema
 
     def handle_typed_dict_schema(self, schema: core_schema.TypedDictSchema, f: Walk) -> core_schema.CoreSchema:
         if 'extra_validator' in schema:
             schema['extra_validator'] = self.walk(schema['extra_validator'], f)
+        replaced_computed_fields: list[core_schema.ComputedField] = []
+        for computed_field in schema.get('computed_fields', None) or ():
+            replaced_field = computed_field.copy()
+            replaced_field['return_schema'] = self.walk(computed_field['return_schema'], f)
+            replaced_computed_fields.append(replaced_field)
+        if replaced_computed_fields:
+            schema['computed_fields'] = replaced_computed_fields
         replaced_fields: dict[str, core_schema.TypedDictField] = {}
         for k, v in schema['fields'].items():
             replaced_field = v.copy()
             replaced_field['schema'] = self.walk(v['schema'], f)
             replaced_fields[k] = replaced_field
         schema['fields'] = replaced_fields
         return schema
 
     def handle_dataclass_args_schema(self, schema: core_schema.DataclassArgsSchema, f: Walk) -> core_schema.CoreSchema:
         replaced_fields: list[core_schema.DataclassField] = []
+        replaced_computed_fields: list[core_schema.ComputedField] = []
+        for computed_field in schema.get('computed_fields', None) or ():
+            replaced_field = computed_field.copy()
+            replaced_field['return_schema'] = self.walk(computed_field['return_schema'], f)
+            replaced_computed_fields.append(replaced_field)
+        if replaced_computed_fields:
+            schema['computed_fields'] = replaced_computed_fields
         for field in schema['fields']:
             replaced_field = field.copy()
             replaced_field['schema'] = self.walk(field['schema'], f)
             replaced_fields.append(replaced_field)
         schema['fields'] = replaced_fields
         return schema
 
@@ -430,15 +415,16 @@
     Returns:
         core_schema.CoreSchema: A processed CoreSchema.
     """
     return f(schema.copy(), _dispatch)
 
 
 def _simplify_schema_references(schema: core_schema.CoreSchema, inline: bool) -> core_schema.CoreSchema:  # noqa: C901
-    all_defs: dict[str, core_schema.CoreSchema] = {}
+    valid_defs: dict[str, core_schema.CoreSchema] = {}
+    invalid_defs: dict[str, core_schema.CoreSchema] = {}
 
     def make_result(schema: core_schema.CoreSchema, defs: Iterable[core_schema.CoreSchema]) -> core_schema.CoreSchema:
         definitions = list(defs)
         if definitions:
             return core_schema.definitions_schema(schema=schema, definitions=definitions)
         return schema
 
@@ -446,33 +432,47 @@
         return s.get('ref', None)
 
     def collect_refs(s: core_schema.CoreSchema, recurse: Recurse) -> core_schema.CoreSchema:
         if s['type'] == 'definitions':
             for definition in s['definitions']:
                 ref = get_ref(definition)
                 assert ref is not None
-                all_defs[ref] = recurse(definition, collect_refs).copy()
+                def_schema = recurse(definition, collect_refs).copy()
+                if 'invalid' in def_schema.get('metadata', {}):
+                    invalid_defs[ref] = def_schema
+                else:
+                    valid_defs[ref] = def_schema
             return recurse(s['schema'], collect_refs)
         ref = get_ref(s)
         if ref is not None:
-            all_defs[ref] = s
+            if 'invalid' in s.get('metadata', {}):
+                invalid_defs[ref] = s
+            else:
+                valid_defs[ref] = s
         return recurse(s, collect_refs)
 
     schema = walk_core_schema(schema, collect_refs)
 
+    all_defs = {**invalid_defs, **valid_defs}
+
     def flatten_refs(s: core_schema.CoreSchema, recurse: Recurse) -> core_schema.CoreSchema:
         if is_definitions_schema(s):
+            new: dict[str, Any] = dict(s)
             # iterate ourselves, we don't want to flatten the actual defs!
-            s['schema'] = recurse(s['schema'], flatten_refs)
-            for definition in s['definitions']:
+            definitions: list[CoreSchema] = new.pop('definitions')
+            schema = cast(CoreSchema, new.pop('schema'))
+            # remaining keys are optional like 'serialization'
+            schema = cast(CoreSchema, {**schema, **new})
+            s['schema'] = recurse(schema, flatten_refs)
+            for definition in definitions:
                 recurse(definition, flatten_refs)  # don't re-assign here!
-            return s
+            return schema
         s = recurse(s, flatten_refs)
         ref = get_ref(s)
-        if ref and ref in all_defs and ref:
+        if ref and ref in all_defs:
             all_defs[ref] = s
             return core_schema.definition_reference_schema(schema_ref=ref)
         return s
 
     schema = walk_core_schema(schema, flatten_refs)
 
     if not inline:
@@ -505,35 +505,37 @@
             ref = s['schema_ref']
             # Check if the reference is only used once and not involved in recursion
             if ref_counts[ref] <= 1 and not involved_in_recursion.get(ref, False):
                 # Inline the reference by replacing the reference with the actual schema
                 new = all_defs.pop(ref)
                 ref_counts[ref] -= 1  # because we just replaced it!
                 new.pop('ref')  # type: ignore
+                # put all other keys that were on the def-ref schema into the inlined version
+                # in particular this is needed for `serialization`
+                if 'serialization' in s:
+                    new['serialization'] = s['serialization']
                 s = recurse(new, inline_refs)
                 return s
             else:
                 return recurse(s, inline_refs)
         else:
             return recurse(s, inline_refs)
 
     schema = walk_core_schema(schema, inline_refs)
 
     definitions = [d for d in all_defs.values() if ref_counts[d['ref']] > 0]  # type: ignore
     return make_result(schema, definitions)
 
 
 def flatten_schema_defs(schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
-    """
-    Simplify schema references by:
-      1. Grouping all definitions into a single top-level `definitions` schema, similar to a JSON schema's `#/$defs`.
+    """Simplify schema references by:
+    1. Grouping all definitions into a single top-level `definitions` schema, similar to a JSON schema's `#/$defs`.
     """
     return _simplify_schema_references(schema, inline=False)
 
 
 def inline_schema_defs(schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
-    """
-    Simplify schema references by:
-      1. Inlining any definitions that are only referenced in one place and are not involved in a cycle.
-      2. Removing any unused `ref` references from schemas.
+    """Simplify schema references by:
+    1. Inlining any definitions that are only referenced in one place and are not involved in a cycle.
+    2. Removing any unused `ref` references from schemas.
     """
     return _simplify_schema_references(schema, inline=True)
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_dataclasses.py` & `pydantic-2.0b3/pydantic/_internal/_dataclasses.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-"""
-Private logic for creating pydantic dataclasses.
-"""
+"""Private logic for creating pydantic dataclasses."""
 from __future__ import annotations as _annotations
 
 import dataclasses
 import typing
 import warnings
 from functools import partial, wraps
 from typing import Any, Callable, ClassVar
 
 from pydantic_core import ArgsKwargs, SchemaSerializer, SchemaValidator, core_schema
 from typing_extensions import TypeGuard
 
 from ..errors import PydanticUndefinedAnnotation
 from ..fields import FieldInfo
 from . import _config, _decorators, _typing_extra
-from ._core_utils import flatten_schema_defs, inline_schema_defs
+from ._core_utils import collect_invalid_schemas, flatten_schema_defs, inline_schema_defs
 from ._fields import collect_dataclass_fields
 from ._generate_schema import GenerateSchema
 from ._generics import get_standard_typevars_map
-from ._model_construction import MockValidator
+from ._mock_validator import set_dataclass_mock_validator
 from ._schema_generation_shared import CallbackGetCoreSchemaHandler
 
 if typing.TYPE_CHECKING:
     from ..config import ConfigDict
 
     class StandardDataclass(typing.Protocol):
         __dataclass_fields__: ClassVar[dict[str, Any]]
@@ -41,36 +39,50 @@
         """metadata for `@field_validator`, `@root_validator` and `@serializer` decorators"""
         __pydantic_fields__: typing.ClassVar[dict[str, FieldInfo]]
         __pydantic_config__: typing.ClassVar[ConfigDict]
         __pydantic_complete__: typing.ClassVar[bool]
 
 
 def set_dataclass_fields(cls: type[StandardDataclass], types_namespace: dict[str, Any] | None = None) -> None:
-    """
-    Collect and set `cls.__pydantic_fields__`
+    """Collect and set `cls.__pydantic_fields__`.
+
+    Args:
+        cls: The class.
+        types_namespace: The types namespace, defaults to `None`.
     """
     typevars_map = get_standard_typevars_map(cls)
     fields = collect_dataclass_fields(cls, types_namespace, typevars_map=typevars_map)
 
     cls.__pydantic_fields__ = fields  # type: ignore
 
 
 def complete_dataclass(
     cls: type[Any],
     config_wrapper: _config.ConfigWrapper,
     *,
     raise_errors: bool = True,
     types_namespace: dict[str, Any] | None,
 ) -> bool:
-    """
-    Finish building a pydantic dataclass.
+    """Finish building a pydantic dataclass.
 
     This logic is called on a class which is yet to be wrapped in `dataclasses.dataclass()`.
 
     This is somewhat analogous to `pydantic._internal._model_construction.complete_model_class`.
+
+    Args:
+        cls: The class.
+        config_wrapper: The config wrapper instance.
+        raise_errors: Whether to raise errors, defaults to `True`.
+        types_namespace: The types namespace.
+
+    Returns:
+        `True` if building a pydantic dataclass is successfully completed, `False` otherwise.
+
+    Raises:
+        PydanticUndefinedAnnotation: If `raise_error` is `True` and there is an undefined annotations.
     """
     if hasattr(cls, '__post_init_post_parse__'):
         warnings.warn(
             'Support for `__post_init_post_parse__` has been dropped, the method will not be called', DeprecationWarning
         )
 
     if types_namespace is None:
@@ -99,44 +111,34 @@
     get_core_schema = getattr(cls, '__get_pydantic_core_schema__', None)
     try:
         if get_core_schema:
             schema = get_core_schema(
                 cls,
                 CallbackGetCoreSchemaHandler(
                     partial(gen_schema.generate_schema, from_dunder_get_core_schema=False),
-                    gen_schema.generate_schema,
+                    gen_schema,
+                    ref_mode='unpack',
                 ),
             )
         else:
             schema = gen_schema.generate_schema(cls, from_dunder_get_core_schema=False)
     except PydanticUndefinedAnnotation as e:
-        cls_name = cls.__name__
         if raise_errors:
             raise
-        undefined_type_error_message = (
-            f'`{cls_name}` is not fully defined; you should define `{e.name}`,'
-            f' then call `pydantic.dataclasses.rebuild_dataclass({cls_name})`'
-            f' before the first `{cls_name}` instance is created.'
-        )
-
-        def attempt_rebuild() -> SchemaValidator | None:
-            from ..dataclasses import rebuild_dataclass
-
-            if rebuild_dataclass(cls, raise_errors=False, _parent_namespace_depth=5):
-                return cls.__pydantic_validator__  # type: ignore
-            else:
-                return None
-
-        cls.__pydantic_validator__ = MockValidator(  # type: ignore[assignment]
-            undefined_type_error_message, code='class-not-fully-defined', attempt_rebuild=attempt_rebuild
-        )
+        set_dataclass_mock_validator(cls, cls.__name__, f'`{e.name}`')
         return False
 
     core_config = config_wrapper.core_config(cls)
 
+    schema = gen_schema.collect_definitions(schema)
+    schema = flatten_schema_defs(schema)
+    if collect_invalid_schemas(schema):
+        set_dataclass_mock_validator(cls, cls.__name__, 'all referenced types')
+        return False
+
     # We are about to set all the remaining required properties expected for this cast;
     # __pydantic_decorators__ and __pydantic_fields__ should already be set
     cls = typing.cast('type[PydanticDataclass]', cls)
     # debug(schema)
     cls.__pydantic_core_schema__ = schema
     simplified_core_schema = inline_schema_defs(flatten_schema_defs(schema))
     cls.__pydantic_validator__ = validator = SchemaValidator(simplified_core_schema, core_config)
@@ -150,17 +152,16 @@
 
         cls.__setattr__ = validated_setattr.__get__(None, cls)  # type: ignore
 
     return True
 
 
 def is_builtin_dataclass(_cls: type[Any]) -> TypeGuard[type[StandardDataclass]]:
-    """
-    Whether a class is a stdlib dataclass
-    (useful to discriminated a pydantic dataclass that is actually a wrapper around a stdlib dataclass)
+    """Whether a class is a stdlib dataclass
+    (useful to discriminated a pydantic dataclass that is actually a wrapper around a stdlib dataclass).
 
     we check that
     - `_cls` is a dataclass
     - `_cls` is not a processed pydantic dataclass (with a basemodel attached)
     - `_cls` is not a pydantic dataclass inheriting directly from a stdlib dataclass
     e.g.
     ```py
@@ -170,17 +171,31 @@
 
     @pydantic.dataclasses.dataclass
     class B(A):
         y: int
     ```
     In this case, when we first check `B`, we make an extra check and look at the annotations ('y'),
     which won't be a superset of all the dataclass fields (only the stdlib fields i.e. 'x')
+
+    Args:
+        cls: The class.
+
+    Returns:
+        `True` if the class is a stdlib dataclass, `False` otherwise.
     """
     return (
         dataclasses.is_dataclass(_cls)
         and not hasattr(_cls, '__pydantic_validator__')
         and set(_cls.__dataclass_fields__).issuperset(set(getattr(_cls, '__annotations__', {})))
     )
 
 
 def is_pydantic_dataclass(_cls: type[Any]) -> TypeGuard[type[PydanticDataclass]]:
+    """Whether a class is a pydantic dataclass.
+
+    Args:
+        cls: The class.
+
+    Returns:
+        `True` if the class is a pydantic dataclass, `False` otherwise.
+    """
     return dataclasses.is_dataclass(_cls) and '__pydantic_validator__' in _cls.__dict__
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_decorators.py` & `pydantic-2.0b3/pydantic/_internal/_decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Logic related to validators applied to models etc. via the `@field_validator` and `@root_validator` decorators.
-"""
+"""Logic related to validators applied to models etc. via the `@field_validator` and `@root_validator` decorators."""
 from __future__ import annotations as _annotations
 
 from collections import deque
 from dataclasses import dataclass, field
 from functools import partial, partialmethod
 from inspect import Parameter, Signature, isdatadescriptor, ismethoddescriptor, signature
 from itertools import islice
@@ -27,86 +25,119 @@
 except ImportError:
     # python 3.7
     cached_property = None
 
 
 @slots_dataclass
 class ValidatorDecoratorInfo:
-    """
-    A container for data from `@validator` so that we can access it
+    """A container for data from `@validator` so that we can access it
     while building the pydantic-core schema.
+
+    Attributes:
+        decorator_repr: A class variable representing the decorator string, '@validator'.
+        fields: A tuple of field names the validator should be called on.
+        mode: The proposed validator mode.
+        each_item: For complex objects (sets, lists etc.) whether to validate individual
+            elements rather than the whole object.
+        always: Whether this method and other validators should be called even if the value is missing.
+        check_fields: Whether to check that the fields actually exist on the model.
     """
 
     decorator_repr: ClassVar[str] = '@validator'
 
     fields: tuple[str, ...]
     mode: Literal['before', 'after']
     each_item: bool
     always: bool
     check_fields: bool | None
 
 
 @slots_dataclass
 class FieldValidatorDecoratorInfo:
-    """
-    A container for data from `@field_validator` so that we can access it
+    """A container for data from `@field_validator` so that we can access it
     while building the pydantic-core schema.
+
+    Attributes:
+        decorator_repr: A class variable representing the decorator string, '@field_validator'.
+        fields: A tuple of field names the validator should be called on.
+        mode: The proposed validator mode.
+        check_fields: Whether to check that the fields actually exist on the model.
     """
 
     decorator_repr: ClassVar[str] = '@field_validator'
 
     fields: tuple[str, ...]
     mode: FieldValidatorModes
     check_fields: bool | None
 
 
 @slots_dataclass
 class RootValidatorDecoratorInfo:
-    """
-    A container for data from `@root_validator` so that we can access it
+    """A container for data from `@root_validator` so that we can access it
     while building the pydantic-core schema.
+
+    Attributes:
+        decorator_repr: A class variable representing the decorator string, '@root_validator'.
+        mode: The proposed validator mode.
     """
 
     decorator_repr: ClassVar[str] = '@root_validator'
     mode: Literal['before', 'after']
 
 
 @slots_dataclass
 class FieldSerializerDecoratorInfo:
-    """
-    A container for data from `@field_serializer` so that we can access it
+    """A container for data from `@field_serializer` so that we can access it
     while building the pydantic-core schema.
+
+    Attributes:
+        decorator_repr: A class variable representing the decorator string, '@field_serializer'.
+        fields: A tuple of field names the serializer should be called on.
+        mode: The proposed serializer mode.
+        return_type: The type of the serializer's return value.
+        when_used: The serialization condition. Accepts a string with values `'always'`, `'unless-none'`, `'json'`,
+            and `'json-unless-none'`.
+        check_fields: Whether to check that the fields actually exist on the model.
     """
 
     decorator_repr: ClassVar[str] = '@field_serializer'
     fields: tuple[str, ...]
     mode: Literal['plain', 'wrap']
     return_type: Any
     when_used: core_schema.WhenUsed
     check_fields: bool | None
 
 
 @slots_dataclass
 class ModelSerializerDecoratorInfo:
-    """
-    A container for data from `@model_serializer` so that we can access it
+    """A container for data from `@model_serializer` so that we can access it
     while building the pydantic-core schema.
+
+    Attributes:
+        decorator_repr: A class variable representing the decorator string, '@model_serializer'.
+        mode: The proposed serializer mode.
+        return_type: The type of the serializer's return value.
+        when_used: The serialization condition. Accepts a string with values `'always'`, `'unless-none'`, `'json'`,
+            and `'json-unless-none'`.
     """
 
     decorator_repr: ClassVar[str] = '@model_serializer'
     mode: Literal['plain', 'wrap']
     return_type: Any
     when_used: core_schema.WhenUsed
 
 
 @slots_dataclass
 class ModelValidatorDecoratorInfo:
-    """
-    A container for data from `@model_validator` so that we can access it
+    """A container for data from `@model_validator` so that we can access it
     while building the pydantic-core schema.
+
+    Attributes:
+        decorator_repr: A class variable representing the decorator string, '@model_serializer'.
+        mode: The proposed serializer mode.
     """
 
     decorator_repr: ClassVar[str] = '@model_validator'
     mode: Literal['wrap', 'before', 'after']
 
 
 DecoratorInfo = Union[
@@ -123,21 +154,25 @@
 DecoratedType: TypeAlias = (
     'Union[classmethod[Any, Any, ReturnType], staticmethod[Any, ReturnType], Callable[..., ReturnType], property]'
 )
 
 
 @dataclass  # can't use slots here since we set attributes on `__post_init__`
 class PydanticDescriptorProxy(Generic[ReturnType]):
-    """
-    Wrap a classmethod, staticmethod, property or unbound function
+    """Wrap a classmethod, staticmethod, property or unbound function
     and act as a descriptor that allows us to detect decorated items
     from the class' attributes.
 
     This class' __get__ returns the wrapped item's __get__ result,
     which makes it transparent for classmethods and staticmethods.
+
+    Attributes:
+        wrapped: The decorator that has to be wrapped.
+        decorator_info: The decorator info.
+        shim: A wrapper function to wrap V1 style function.
     """
 
     wrapped: DecoratedType[ReturnType]
     decorator_info: DecoratorInfo
     shim: Callable[[Callable[..., Any]], Callable[..., Any]] | None = None
 
     def __post_init__(self):
@@ -158,28 +193,34 @@
             return self.wrapped  # type: ignore[return-value]
 
     def __set_name__(self, instance: Any, name: str) -> None:
         if hasattr(self.wrapped, '__set_name__'):
             self.wrapped.__set_name__(instance, name)
 
     def __getattr__(self, __name: str) -> Any:
-        """Forward checks for __isabstractmethod__ and such"""
+        """Forward checks for __isabstractmethod__ and such."""
         return getattr(self.wrapped, __name)
 
 
 DecoratorInfoType = TypeVar('DecoratorInfoType', bound=DecoratorInfo)
 
 
 @slots_dataclass
 class Decorator(Generic[DecoratorInfoType]):
-    """
-    A generic container class to join together the decorator metadata
+    """A generic container class to join together the decorator metadata
     (metadata from decorator itself, which we have when the
     decorator is called but not when we are building the core-schema)
     and the bound function (which we have after the class itself is created).
+
+    Attributes:
+        cls_ref: The class ref.
+        cls_var_name: The decorated function name.
+        func: The decorated function.
+        shim: A wrapper function to wrap V1 style function.
+        info: The decorator info.
     """
 
     cls_ref: str
     cls_var_name: str
     func: Callable[..., Any]
     shim: Callable[[Any], Any] | None
     info: DecoratorInfoType
@@ -188,50 +229,75 @@
     def build(
         cls_: Any,
         *,
         cls_var_name: str,
         shim: Callable[[Any], Any] | None,
         info: DecoratorInfoType,
     ) -> Decorator[DecoratorInfoType]:
+        """Build a new decorator.
+
+        Args:
+            cls_: The class.
+            cls_var_name: The decorated function name.
+            shim: A wrapper function to wrap V1 style function.
+            info: The decorator info.
+
+        Returns:
+            The new decorator instance.
+        """
         func = get_attribute_from_bases(cls_, cls_var_name)
         if shim is not None:
             func = shim(func)
         return Decorator(
             cls_ref=get_type_ref(cls_),
             cls_var_name=cls_var_name,
             func=func,
             shim=shim,
             info=info,
         )
 
     def bind_to_cls(self, cls: Any) -> Decorator[DecoratorInfoType]:
+        """Bind the decorator to a class.
+
+        Args:
+            cls: the class.
+
+        Returns:
+            The new decorator instance.
+        """
         return self.build(
             cls,
             cls_var_name=self.cls_var_name,
             shim=self.shim,
             info=self.info,
         )
 
 
 def get_bases(tp: type[Any]) -> tuple[type[Any], ...]:
+    """Get the base classes of a class or typeddict.
+
+    Args:
+        tp: The type or class to get the bases.
+
+    Returns:
+        The base classes.
+    """
     if is_typeddict(tp):
         return tp.__orig_bases__  # type: ignore
     try:
         return tp.__bases__
     except AttributeError:
         return ()
 
 
 def mro(tp: type[Any]) -> tuple[type[Any], ...]:
-    """
-    Calculate the Method Resolution Order of bases using the C3 algorithm.
+    """Calculate the Method Resolution Order of bases using the C3 algorithm.
 
     See https://www.python.org/download/releases/2.3/mro/
     """
-
     # try to use the existing mro, for performance mainly
     # but also because it helps verify the implementation below
     if not is_typeddict(tp):
         try:
             return tp.__mro__
         except AttributeError:
             # GenericAlias and some other cases
@@ -264,26 +330,25 @@
     seqs = [deque(mro(base)) for base in bases] + [deque(bases)]
     res = tuple(merge_seqs(seqs))
 
     return (tp,) + res
 
 
 def get_attribute_from_bases(tp: type[Any], name: str) -> Any:
-    """
-    Get the attribute from the next class in the MRO that has it,
+    """Get the attribute from the next class in the MRO that has it,
     aiming to simulate calling the method on the actual class.
 
     The reason for iterating over the mro instead of just getting
     the attribute (which would do that for us) is to support TypedDict,
     which lacks a real __mro__, but can have a virtual one constructed
     from its bases (as done here).
 
     Args:
-        tp (type[Any]): The type or class to search for the attribute.
-        name (str): The name of the attribute to retrieve.
+        tp: The type or class to search for the attribute.
+        name: The name of the attribute to retrieve.
 
     Returns:
         Any: The attribute value, if found.
 
     Raises:
         AttributeError: If the attribute is not found in any class in the MRO.
     """
@@ -294,41 +359,42 @@
             if hasattr(base, name):
                 return getattr(base, name)
         raise e
 
 
 @slots_dataclass
 class DecoratorInfos:
-    # mapping of name in the class namespace to decorator info
-    # note that the name in the class namespace is the function or attribute name
-    # not the field name!
+    """Mapping of name in the class namespace to decorator info.
+
+    note that the name in the class namespace is the function or attribute name
+    not the field name!
+    """
+
     validators: dict[str, Decorator[ValidatorDecoratorInfo]] = field(default_factory=dict)
     field_validators: dict[str, Decorator[FieldValidatorDecoratorInfo]] = field(default_factory=dict)
     root_validators: dict[str, Decorator[RootValidatorDecoratorInfo]] = field(default_factory=dict)
     field_serializers: dict[str, Decorator[FieldSerializerDecoratorInfo]] = field(default_factory=dict)
     model_serializers: dict[str, Decorator[ModelSerializerDecoratorInfo]] = field(default_factory=dict)
     model_validators: dict[str, Decorator[ModelValidatorDecoratorInfo]] = field(default_factory=dict)
     computed_fields: dict[str, Decorator[ComputedFieldInfo]] = field(default_factory=dict)
 
     @staticmethod
     def build(model_dc: type[Any]) -> DecoratorInfos:  # noqa: C901 (ignore complexity)
-        """
-        We want to collect all DecFunc instances that exist as
+        """We want to collect all DecFunc instances that exist as
         attributes in the namespace of the class (a BaseModel or dataclass)
         that called us
         But we want to collect these in the order of the bases
         So instead of getting them all from the leaf class (the class that called us),
         we traverse the bases from root (the oldest ancestor class) to leaf
         and collect all of the instances as we go, taking care to replace
         any duplicate ones with the last one we see to mimic how function overriding
         works with inheritance.
         If we do replace any functions we put the replacement into the position
         the replaced function was in; that is, we maintain the order.
         """
-
         # reminder: dicts are ordered and replacement does not alter the order
         res = DecoratorInfos()
         for base in reversed(mro(model_dc)[1:]):
             existing: DecoratorInfos | None = base.__dict__.get('__pydantic_decorators__')
             if existing is None:
                 existing = DecoratorInfos.build(base)
             res.validators.update({k: v.bind_to_cls(model_dc) for k, v in existing.validators.items()})
@@ -396,16 +462,15 @@
             setattr(model_dc, '__pydantic_decorators__', res)
             for name, value in to_replace:
                 setattr(model_dc, name, value)
         return res
 
 
 def inspect_validator(validator: Callable[..., Any], mode: FieldValidatorModes) -> bool:
-    """
-    Look at a field or model validator function and determine if it whether it takes an info argument.
+    """Look at a field or model validator function and determine if it whether it takes an info argument.
 
     An error is raised if the function has an invalid signature.
 
     Args:
         validator: The validator function to inspect.
         mode: The proposed validator mode.
 
@@ -429,26 +494,25 @@
     raise PydanticUserError(
         f'Unrecognized field_validator function signature for {validator} with `mode={mode}`:{sig}',
         code='validator-signature',
     )
 
 
 def inspect_field_serializer(serializer: Callable[..., Any], mode: Literal['plain', 'wrap']) -> tuple[bool, bool]:
-    """
-    Look at a field serializer function and determine if it is a field serializer,
+    """Look at a field serializer function and determine if it is a field serializer,
     and whether it takes an info argument.
 
     An error is raised if the function has an invalid signature.
 
     Args:
         serializer: The serializer function to inspect.
         mode: The serializer mode, either 'plain' or 'wrap'.
 
     Returns:
-        Tuple of (is_field_serializer, info_arg)
+        Tuple of (is_field_serializer, info_arg).
     """
     sig = signature(serializer)
 
     first = next(iter(sig.parameters.values()), None)
     is_field_serializer = first is not None and first.name == 'self'
 
     n_positional = count_positional_params(sig)
@@ -464,16 +528,15 @@
             code='field-serializer-signature',
         )
     else:
         return is_field_serializer, info_arg
 
 
 def inspect_annotated_serializer(serializer: Callable[..., Any], mode: Literal['plain', 'wrap']) -> bool:
-    """
-    Look at a serializer function used via `Annotated` and determine whether it takes an info argument.
+    """Look at a serializer function used via `Annotated` and determine whether it takes an info argument.
 
     An error is raised if the function has an invalid signature.
 
     Args:
         serializer: The serializer function to check.
         mode: The serializer mode, either 'plain' or 'wrap'.
 
@@ -488,27 +551,25 @@
             code='field-serializer-signature',
         )
     else:
         return info_arg
 
 
 def inspect_model_serializer(serializer: Callable[..., Any], mode: Literal['plain', 'wrap']) -> bool:
-    """
-    Look at a model serializer function and determine whether it takes an info argument.
+    """Look at a model serializer function and determine whether it takes an info argument.
 
     An error is raised if the function has an invalid signature.
 
     Args:
         serializer: The serializer function to check.
         mode: The serializer mode, either 'plain' or 'wrap'.
 
     Returns:
-        `info_arg` - whether the function expects an info argument
+        `info_arg` - whether the function expects an info argument.
     """
-
     if isinstance(serializer, (staticmethod, classmethod)) or not is_instance_method_from_sig(serializer):
         raise PydanticUserError(
             '`@model_serializer` must be applied to instance methods', code='model-serializer-instance-method'
         )
 
     sig = signature(serializer)
     info_arg = _serializer_info_arg(mode, count_positional_params(sig))
@@ -543,22 +604,41 @@
 
 AnyDecoratorCallable: TypeAlias = (
     'Union[classmethod[Any, Any, Any], staticmethod[Any, Any], partialmethod[Any], Callable[..., Any]]'
 )
 
 
 def is_instance_method_from_sig(function: AnyDecoratorCallable) -> bool:
+    """Whether the function is an instance method.
+
+    It will consider a function as instance method if the first parameter of
+    function is `self`.
+
+    Args:
+        function: The function to check.
+
+    Returns:
+        `True` if the function is an instance method, `False` otherwise.
+    """
     sig = signature(unwrap_wrapped_function(function))
     first = next(iter(sig.parameters.values()), None)
     if first and first.name == 'self':
         return True
     return False
 
 
 def ensure_classmethod_based_on_signature(function: AnyDecoratorCallable) -> Any:
+    """Apply the `@classmethod` decorator on the function.
+
+    Args:
+        function: The function to apply the decorator on.
+
+    Return:
+        The `@classmethod` decorator applied function.
+    """
     if not isinstance(
         unwrap_wrapped_function(function, unwrap_class_static_method=False), classmethod
     ) and _is_classmethod_from_sig(function):
         return classmethod(function)  # type: ignore[arg-type]
     return function
 
 
@@ -571,16 +651,15 @@
 
 
 def unwrap_wrapped_function(
     func: Any,
     *,
     unwrap_class_static_method: bool = True,
 ) -> Any:
-    """
-    Recursively unwraps a wrapped function until the underlying function is reached.
+    """Recursively unwraps a wrapped function until the underlying function is reached.
     This handles functools.partial, functools.partialmethod, staticmethod and classmethod.
 
     Args:
         func: The function to unwrap.
         unwrap_class_static_method: If True (default), also unwrap classmethod and staticmethod
             decorators. If False, only unwrap partial and partialmethod decorators.
 
@@ -611,14 +690,26 @@
             assert isinstance(func, cached_property)
             func = func.func  # type: ignore
 
     return func
 
 
 def get_function_return_type(func: Any, explicit_return_type: Any) -> Any:
+    """Get the function return type.
+
+    It gets the return type from the type annotation if `explicit_return_type` is `None`.
+    Otherwise, it returns `explicit_return_type`.
+
+    Args:
+        func: The function to get its return type.
+        explicit_return_type: The explicit return type.
+
+    Returns:
+        The function return type.
+    """
     if explicit_return_type is None:
         # try to get it from the type annotation
         func = unwrap_wrapped_function(func)
         hints = get_function_type_hints(unwrap_wrapped_function(func), include_keys={'return'})
         return hints.get('return', None)
     else:
         return explicit_return_type
@@ -629,21 +720,19 @@
 
 
 def can_be_positional(param: Parameter) -> bool:
     return param.kind in (Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD)
 
 
 def ensure_property(f: Any) -> Any:
-    """
-    Ensure that a function is a `property` or `cached_property`, or is a valid descriptor.
+    """Ensure that a function is a `property` or `cached_property`, or is a valid descriptor.
 
     Args:
         f: The function to check.
 
     Returns:
         The function, or a `property` or `cached_property` instance wrapping the function.
     """
-
     if ismethoddescriptor(f) or isdatadescriptor(f):
         return f
     else:
         return property(f)
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_decorators_v1.py` & `pydantic-2.0b3/pydantic/_internal/_decorators_v1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,77 @@
-"""
-Logic for V1 validators, e.g. `@validator` and `@root_validator`.
-"""
+"""Logic for V1 validators, e.g. `@validator` and `@root_validator`."""
 from __future__ import annotations as _annotations
 
 from inspect import Parameter, signature
 from typing import Any, Dict, Tuple, Union, cast
 
 from pydantic_core import core_schema
 from typing_extensions import Protocol
 
 from ..errors import PydanticUserError
 from ._decorators import can_be_positional
 
 
 class V1OnlyValueValidator(Protocol):
-    """
-    A simple validator, supported for V1 validators and V2 validators
-    """
+    """A simple validator, supported for V1 validators and V2 validators."""
 
     def __call__(self, __value: Any) -> Any:
         ...
 
 
 class V1ValidatorWithValues(Protocol):
+    """A validator with `values` argument, supported for V1 validators and V2 validators."""
+
     def __call__(self, __value: Any, values: dict[str, Any]) -> Any:
         ...
 
 
 class V1ValidatorWithValuesKwOnly(Protocol):
+    """A validator with keyword only `values` argument, supported for V1 validators and V2 validators."""
+
     def __call__(self, __value: Any, *, values: dict[str, Any]) -> Any:
         ...
 
 
 class V1ValidatorWithKwargs(Protocol):
+    """A validator with `kwargs` argument, supported for V1 validators and V2 validators."""
+
     def __call__(self, __value: Any, **kwargs: Any) -> Any:
         ...
 
 
 class V1ValidatorWithValuesAndKwargs(Protocol):
+    """A validator with `values` and `kwargs` arguments, supported for V1 validators and V2 validators."""
+
     def __call__(self, __value: Any, values: dict[str, Any], **kwargs: Any) -> Any:
         ...
 
 
 V1Validator = Union[
     V1ValidatorWithValues, V1ValidatorWithValuesKwOnly, V1ValidatorWithKwargs, V1ValidatorWithValuesAndKwargs
 ]
 
 
 def can_be_keyword(param: Parameter) -> bool:
     return param.kind in (Parameter.POSITIONAL_OR_KEYWORD, Parameter.KEYWORD_ONLY)
 
 
 def make_generic_v1_field_validator(validator: V1Validator) -> core_schema.FieldValidatorFunction:
+    """Wrap a V1 style field validator for V2 compatibility.
+
+    Args:
+        validator: The V1 style field validator.
+
+    Returns:
+        A wrapped V2 style field validator.
+
+    Raises:
+        PydanticUserError: If the signature is not supported or the parameters are
+            not available in Pydantic V2.
+    """
     sig = signature(validator)
 
     needs_values_kw = False
 
     for param_num, (param_name, parameter) in enumerate(sig.parameters.items()):
         if can_be_keyword(parameter) and param_name in ('field', 'config'):
             raise PydanticUserError(
@@ -95,35 +111,47 @@
 
 RootValidatorValues = Dict[str, Any]
 # technically tuple[model_dict, model_extra, fields_set] | tuple[dataclass_dict, init_vars]
 RootValidatorFieldsTuple = Tuple[Any, ...]
 
 
 class V1RootValidatorFunction(Protocol):
+    """A simple root validator, supported for V1 validators and V2 validators."""
+
     def __call__(self, __values: RootValidatorValues) -> RootValidatorValues:
         ...
 
 
 class V2CoreBeforeRootValidator(Protocol):
+    """V2 validator with mode='before'."""
+
     def __call__(self, __values: RootValidatorValues, __info: core_schema.ValidationInfo) -> RootValidatorValues:
         ...
 
 
 class V2CoreAfterRootValidator(Protocol):
+    """V2 validator with mode='after'."""
+
     def __call__(
         self, __fields_tuple: RootValidatorFieldsTuple, __info: core_schema.ValidationInfo
     ) -> RootValidatorFieldsTuple:
         ...
 
 
 def make_v1_generic_root_validator(
     validator: V1RootValidatorFunction, pre: bool
 ) -> V2CoreBeforeRootValidator | V2CoreAfterRootValidator:
-    """
-    Wrap a V1 style root validator for V2 compatibility
+    """Wrap a V1 style root validator for V2 compatibility.
+
+    Args:
+        validator: The V1 style field validator.
+        pre: Whether the validator is a pre validator.
+
+    Returns:
+        A wrapped V2 style validator.
     """
     if pre is True:
         # mode='before' for pydantic-core
         def _wrapper1(values: RootValidatorValues, _: core_schema.ValidationInfo) -> RootValidatorValues:
             return validator(values)
 
         return _wrapper1
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_discriminated_union.py` & `pydantic-2.0b3/pydantic/_internal/_discriminated_union.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,49 @@
 from __future__ import annotations as _annotations
 
-from enum import Enum
-from typing import Sequence
+from typing import Any, Hashable, Sequence
 
 from pydantic_core import core_schema
 
 from ..errors import PydanticUserError
 from . import _core_utils
 from ._core_utils import CoreSchemaField, collect_definitions
 
 
 def apply_discriminator(
     schema: core_schema.CoreSchema, discriminator: str, definitions: dict[str, core_schema.CoreSchema] | None = None
 ) -> core_schema.CoreSchema:
+    """Applies the discriminator and returns a new core schema.
+
+    Args:
+        schema: The input schema.
+        discriminator: The name of the field which will serve as the discriminator.
+        definitions: A mapping of schema ref to schema.
+
+    Returns:
+        The new core schema.
+
+    Raises:
+        TypeError:
+            - If `discriminator` is used with invalid union variant.
+            - If `discriminator` is used with `Union` type with one variant.
+            - If `discriminator` value mapped to multiple choices.
+        ValueError:
+            If the definition for ref is missing.
+        PydanticUserError:
+            - If a model in union doesn't have a discriminator field.
+            - If discriminator field has a non-string alias.
+            - If discriminator fields have different aliases.
+            - If discriminator field not of type `Literal`.
+    """
     return _ApplyInferredDiscriminator(discriminator, definitions or {}).apply(schema)
 
 
 class _ApplyInferredDiscriminator:
-    """
-    This class is used to convert an input schema containing a union schema into one where that union is
+    """This class is used to convert an input schema containing a union schema into one where that union is
     replaced with a tagged-union, with all the associated debugging and performance benefits.
 
     This is done by:
     * Validating that the input schema is compatible with the provided discriminator
     * Introspecting the schema to determine which discriminator values should map to which union choices
     * Handling various edge cases such as 'definitions', 'default', 'nullable' schemas, and more
 
@@ -75,41 +96,59 @@
         # `_choices_to_handle` serves as a stack of choices to add to the tagged union. Initially, choices
         # from the union in the wrapped schema will be appended to this list, and the recursive choice-handling
         # algorithm may add more choices to this stack as (nested) unions are encountered.
         self._choices_to_handle: list[core_schema.CoreSchema] = []
 
         # `_tagged_union_choices` is built during the call to `apply`, and will hold the choices to be included
         # in the output TaggedUnionSchema that will replace the union from the input schema
-        self._tagged_union_choices: dict[str | int, str | int | core_schema.CoreSchema] = {}
+        self._tagged_union_choices: dict[Hashable, core_schema.CoreSchema] = {}
 
         # `_used` is changed to True after applying the discriminator to prevent accidental re-use
         self._used = False
 
     def apply(self, schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
-        """
-        Return a new CoreSchema based on `schema` that uses a tagged-union with the discriminator provided
+        """Return a new CoreSchema based on `schema` that uses a tagged-union with the discriminator provided
         to this class.
+
+        Args:
+            schema: The input schema.
+
+        Returns:
+            The new core schema.
+
+        Raises:
+            TypeError:
+                - If `discriminator` is used with invalid union variant.
+                - If `discriminator` is used with `Union` type with one variant.
+                - If `discriminator` value mapped to multiple choices.
+            ValueError:
+                If the definition for ref is missing.
+            PydanticUserError:
+                - If a model in union doesn't have a discriminator field.
+                - If discriminator field has a non-string alias.
+                - If discriminator fields have different aliases.
+                - If discriminator field not of type `Literal`.
         """
         old_definitions = collect_definitions(schema)
+        self.definitions = {**old_definitions, **self.definitions}
         assert not self._used
         schema = self._apply_to_root(schema)
         if self._should_be_nullable and not self._is_nullable:
             schema = core_schema.nullable_schema(schema)
         self._used = True
         new_definitions = collect_definitions(schema)
 
         missing_definitions = [v for k, v in old_definitions.items() if k not in new_definitions]
         if missing_definitions:
             schema = core_schema.definitions_schema(schema, missing_definitions)
 
         return schema
 
     def _apply_to_root(self, schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
-        """
-        This method handles the outer-most stage of recursion over the input schema:
+        """This method handles the outer-most stage of recursion over the input schema:
         unwrapping nullable or definitions schemas, and calling the `_handle_choice`
         method iteratively on the choices extracted (recursively) from the possibly-wrapped union.
         """
         if schema['type'] == 'nullable':
             self._is_nullable = True
             wrapped = self._apply_to_root(schema['schema'])
             nullable_wrapper = schema.copy()
@@ -155,16 +194,15 @@
             from_attributes=True,
             ref=schema.get('ref'),
             metadata=schema.get('metadata'),
             serialization=schema.get('serialization'),
         )
 
     def _handle_choice(self, choice: core_schema.CoreSchema) -> None:
-        """
-        This method handles the "middle" stage of recursion over the input schema.
+        """This method handles the "middle" stage of recursion over the input schema.
         Specifically, it is responsible for handling each choice of the outermost union
         (and any "coalesced" choices obtained from inner unions).
 
         Here, "handling" entails:
         * Coalescing nested unions and compatible tagged-unions
         * Tracking the presence of 'none' and 'nullable' schemas occurring as choices
         * Validating that each allowed discriminator value maps to a unique choice
@@ -206,31 +244,29 @@
                 self._choices_to_handle.extend(subchoices[::-1])
                 return
 
             inferred_discriminator_values = self._infer_discriminator_values_for_choice(choice, source_name=None)
             self._set_unique_choice_for_values(choice, inferred_discriminator_values)
 
     def _is_discriminator_shared(self, choice: core_schema.TaggedUnionSchema) -> bool:
-        """
-        This method returns a boolean indicating whether the discriminator for the `choice`
+        """This method returns a boolean indicating whether the discriminator for the `choice`
         is the same as that being used for the outermost tagged union. This is used to
         determine whether this TaggedUnionSchema choice should be "coalesced" into the top level,
         or whether it should be treated as a separate (nested) choice.
         """
         inner_discriminator = choice['discriminator']
         return inner_discriminator == self.discriminator or (
             isinstance(inner_discriminator, list)
             and (self.discriminator in inner_discriminator or [self.discriminator] in inner_discriminator)
         )
 
     def _infer_discriminator_values_for_choice(  # noqa C901
         self, choice: core_schema.CoreSchema, source_name: str | None
     ) -> list[str | int]:
-        """
-        This function recurses over `choice`, extracting all discriminator values that should map to this choice.
+        """This function recurses over `choice`, extracting all discriminator values that should map to this choice.
 
         `model_name` is accepted for the purpose of producing useful error messages.
         """
         if choice['type'] == 'definitions':
             return self._infer_discriminator_values_for_choice(choice['schema'], source_name=source_name)
         elif choice['type'] == 'function-plain':
             raise TypeError(
@@ -287,16 +323,15 @@
                 f'{choice["type"]!r} is not a valid discriminated union variant;'
                 ' should be a `BaseModel` or `dataclass`'
             )
 
     def _infer_discriminator_values_for_typed_dict_choice(
         self, choice: core_schema.TypedDictSchema, source_name: str | None = None
     ) -> list[str | int]:
-        """
-        This method just extracts the _infer_discriminator_values_for_choice logic specific to TypedDictSchema
+        """This method just extracts the _infer_discriminator_values_for_choice logic specific to TypedDictSchema
         for the sake of readability.
         """
         source = 'TypedDict' if source_name is None else f'TypedDict {source_name!r}'
         field = choice['fields'].get(self.discriminator)
         if field is None:
             raise PydanticUserError(
                 f'{source} needs a discriminator field for key {self.discriminator!r}', code='discriminator-no-field'
@@ -345,33 +380,25 @@
                 code='discriminator-alias',
             )
         return self._infer_discriminator_values_for_inner_schema(field['schema'], source)
 
     def _infer_discriminator_values_for_inner_schema(
         self, schema: core_schema.CoreSchema, source: str
     ) -> list[str | int]:
-        """
-        When inferring discriminator values for a field, we typically extract the expected values from a literal schema.
-        This function does that, but also handles nested unions and defaults.
+        """When inferring discriminator values for a field, we typically extract the expected values from a literal
+        schema. This function does that, but also handles nested unions and defaults.
         """
         if schema['type'] == 'literal':
-            values = []
-            for v in schema['expected']:
-                if isinstance(v, Enum):
-                    v = v.value
-                if not isinstance(v, (str, int)):
-                    raise TypeError(f'Unsupported value for discriminator field: {v!r}')
-                values.append(v)
-            return values
+            return schema['expected']
 
         elif schema['type'] == 'union':
             # Generally when multiple values are allowed they should be placed in a single `Literal`, but
             # we add this case to handle the situation where a field is annotated as a `Union` of `Literal`s.
             # For example, this lets us handle `Union[Literal['key'], Union[Literal['Key'], Literal['KEY']]]`
-            values = []
+            values: list[Any] = []
             for choice in schema['choices']:
                 choice_values = self._infer_discriminator_values_for_inner_schema(choice, source)
                 values.extend(choice_values)
             return values
 
         elif schema['type'] == 'default':
             # This will happen if the field has a default value; we ignore it while extracting the discriminator values
@@ -380,30 +407,23 @@
         else:
             raise PydanticUserError(
                 f'{source} needs field {self.discriminator!r} to be of type `Literal`',
                 code='discriminator-needs-literal',
             )
 
     def _set_unique_choice_for_values(self, choice: core_schema.CoreSchema, values: Sequence[str | int]) -> None:
-        """
-        This method updates `self.tagged_union_choices` so that all provided (discriminator) `values` map to the
+        """This method updates `self.tagged_union_choices` so that all provided (discriminator) `values` map to the
         provided `choice`, validating that none of these values already map to another (different) choice.
         """
-        primary_value: str | int | None = None
         for discriminator_value in values:
             if discriminator_value in self._tagged_union_choices:
                 # It is okay if `value` is already in tagged_union_choices as long as it maps to the same value.
                 # Because tagged_union_choices may map values to other values, we need to walk the choices dict
                 # until we get to a "real" choice, and confirm that is equal to the one assigned.
                 existing_choice = self._tagged_union_choices[discriminator_value]
-                while isinstance(existing_choice, (str, int)):
-                    existing_choice = self._tagged_union_choices[existing_choice]
                 if existing_choice != choice:
                     raise TypeError(
                         f'Value {discriminator_value!r} for discriminator '
                         f'{self.discriminator!r} mapped to multiple choices'
                     )
-            elif primary_value is None:
-                self._tagged_union_choices[discriminator_value] = choice
-                primary_value = discriminator_value
             else:
-                self._tagged_union_choices[discriminator_value] = primary_value
+                self._tagged_union_choices[discriminator_value] = choice
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_fields.py` & `pydantic-2.0b3/pydantic/_internal/_fields.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Private logic related to fields (the `Field()` function and `FieldInfo` class), and arguments to `Annotated`.
-"""
+"""Private logic related to fields (the `Field()` function and `FieldInfo` class), and arguments to `Annotated`."""
 from __future__ import annotations as _annotations
 
 import dataclasses
 import sys
 from copy import copy
 from typing import TYPE_CHECKING, Any
 
@@ -20,29 +18,40 @@
 
 
 def get_type_hints_infer_globalns(
     obj: Any,
     localns: dict[str, Any] | None = None,
     include_extras: bool = False,
 ) -> dict[str, Any]:
+    """Gets type hints for an object by inferring the global namespace.
+
+    It uses the `typing.get_type_hints`, The only thing that we do here is fetching
+    global namespace from `obj.__module__` if it is not `None`.
+
+    Args:
+        obj: The object to get it's type hints.
+        localns: The local namespaces.
+        include_extras: Whether to recursively include annotation metadata.
+
+    Returns:
+        The object type hints.
+    """
     module_name = getattr(obj, '__module__', None)
     globalns: dict[str, Any] | None = None
     if module_name:
         try:
             globalns = sys.modules[module_name].__dict__
         except KeyError:
             # happens occasionally, see https://github.com/pydantic/pydantic/issues/2363
             pass
     return get_type_hints(obj, globalns=globalns, localns=localns, include_extras=include_extras)
 
 
 class _UndefinedType:
-    """
-    Singleton class to represent an undefined value.
-    """
+    """Singleton class to represent an undefined value."""
 
     def __repr__(self) -> str:
         return 'PydanticUndefined'
 
     def __copy__(self) -> _UndefinedType:
         return self
 
@@ -53,66 +62,82 @@
         return self
 
 
 Undefined = _UndefinedType()
 
 
 class PydanticMetadata(Representation):
-    """
-    Base class for annotation markers like `Strict`.
-    """
+    """Base class for annotation markers like `Strict`."""
 
     __slots__ = ()
 
 
 class PydanticGeneralMetadata(PydanticMetadata):
+    """Pydantic general metada like `max_digits`."""
+
     def __init__(self, **metadata: Any):
         self.__dict__ = metadata
 
 
 def collect_model_fields(  # noqa: C901
     cls: type[BaseModel],
     bases: tuple[type[Any], ...],
     config_wrapper: ConfigWrapper,
     types_namespace: dict[str, Any] | None,
     *,
     typevars_map: dict[Any, Any] | None = None,
 ) -> tuple[dict[str, FieldInfo], set[str]]:
-    """
-    Collect the fields of a nascent pydantic model
+    """Collect the fields of a nascent pydantic model.
 
     Also collect the names of any ClassVars present in the type hints.
 
     The returned value is a tuple of two items: the fields dict, and the set of ClassVar names.
 
-    :param cls: BaseModel or dataclass
-    :param bases: parents of the class, generally `cls.__bases__`
-    :param types_namespace: optional extra namespace to look for types in
+    Args:
+        cls: BaseModel or dataclass.
+        bases: Parents of the class, generally `cls.__bases__`.
+        config_wrapper: The config wrapper instance.
+        types_namespace: Optional extra namespace to look for types in.
+        typevars_map: A dictionary mapping type variables to their concrete types.
+
+    Returns:
+        A tuple contains fields and class variables.
+
+    Raises:
+        NameError:
+            - If there is a conflict between a field name and protected namespaces.
+            - If there is a field other than `root` in `RootModel`.
+            - If a field shadows an attribute in the parent model.
     """
     from ..fields import FieldInfo
 
     type_hints = get_cls_type_hints_lenient(cls, types_namespace)
 
     # https://docs.python.org/3/howto/annotations.html#accessing-the-annotations-dict-of-an-object-in-python-3-9-and-older
     # annotations is only used for finding fields in parent classes
     annotations = cls.__dict__.get('__annotations__', {})
     fields: dict[str, FieldInfo] = {}
 
     class_vars: set[str] = set()
     for ann_name, ann_type in type_hints.items():
+        if ann_name == 'model_config':
+            # We never want to treat `model_config` as a field
+            # Note: we may need to change this logic if/when we introduce a `BareModel` class with no
+            # protected namespaces (where `model_config` might be allowed as a field name)
+            continue
         for protected_namespace in config_wrapper.protected_namespaces:
             if ann_name.startswith(protected_namespace):
                 raise NameError(f'Field "{ann_name}" has conflict with protected namespace "{protected_namespace}"')
         if is_classvar(ann_type):
             class_vars.add(ann_name)
             continue
         if _is_finalvar_with_default_val(ann_type, getattr(cls, ann_name, Undefined)):
             class_vars.add(ann_name)
             continue
-        if ann_name.startswith('_'):
+        if not is_valid_field_name(ann_name):
             continue
         if cls.__pydantic_root_model__ and ann_name != 'root':
             raise NameError(
                 f"Unexpected field with name {ann_name!r}; only 'root' is allowed as a field of a `RootModel`"
             )
 
         # when building a generic model with `MyModel[int]`, the generic_origin check makes sure we don't get
@@ -181,14 +206,24 @@
     else:
         return True
 
 
 def collect_dataclass_fields(
     cls: type[StandardDataclass], types_namespace: dict[str, Any] | None, *, typevars_map: dict[Any, Any] | None = None
 ) -> dict[str, FieldInfo]:
+    """Collect the fields of a dataclass.
+
+    Args:
+        cls: dataclass.
+        types_namespace: Optional extra namespace to look for types in.
+        typevars_map: A dictionary mapping type variables to their concrete types.
+
+    Returns:
+        The dataclass fields.
+    """
     from ..fields import FieldInfo
 
     fields: dict[str, FieldInfo] = {}
     dataclass_fields: dict[str, dataclasses.Field] = cls.__dataclass_fields__
     cls_localns = dict(vars(cls))  # this matches get_cls_type_hints_lenient, but all tests pass with `= None` instead
 
     for ann_name, dataclass_field in dataclass_fields.items():
@@ -198,21 +233,32 @@
 
         if not dataclass_field.init:
             # TODO: We should probably do something with this so that validate_assignment behaves properly
             #   Issue: https://github.com/pydantic/pydantic/issues/5470
             continue
 
         if isinstance(dataclass_field.default, FieldInfo):
+            if dataclass_field.default.init_var:
+                # TODO: same note as above
+                continue
             field_info = FieldInfo.from_annotated_attribute(ann_type, dataclass_field.default)
         else:
             field_info = FieldInfo.from_annotated_attribute(ann_type, dataclass_field)
         fields[ann_name] = field_info
 
         if field_info.default is not Undefined:
             # We need this to fix the default when the "default" from __dataclass_fields__ is a pydantic.FieldInfo
             setattr(cls, ann_name, field_info.default)
 
     if typevars_map:
         for field in fields.values():
             field.apply_typevars_map(typevars_map, types_namespace)
 
     return fields
+
+
+def is_valid_field_name(name: str) -> bool:
+    return not name.startswith('_')
+
+
+def is_valid_privateattr_name(name: str) -> bool:
+    return name.startswith('_') and not name.startswith('__')
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_generate_schema.py` & `pydantic-2.0b3/pydantic/_internal/_generate_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-"""
-Convert python types to pydantic-core schema.
-"""
+"""Convert python types to pydantic-core schema."""
 from __future__ import annotations as _annotations
 
 import collections.abc
 import dataclasses
 import inspect
 import re
 import sys
 import typing
+from contextlib import contextmanager
+from copy import copy
+from enum import Enum
 from functools import partial
 from inspect import Parameter, _ParameterKind, signature
 from itertools import chain
 from operator import attrgetter
 from types import FunctionType, LambdaType, MethodType
-from typing import TYPE_CHECKING, Any, Callable, ForwardRef, Iterable, Mapping, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, Callable, Dict, ForwardRef, Iterable, Iterator, Mapping, TypeVar, Union, cast
 
 from pydantic_core import CoreSchema, core_schema
 from typing_extensions import Annotated, Final, Literal, TypeAliasType, TypedDict, get_args, get_origin, is_typeddict
 
 from ..config import ConfigDict
 from ..errors import PydanticSchemaGenerationError, PydanticUndefinedAnnotation, PydanticUserError
 from ..fields import AliasChoices, AliasPath, FieldInfo
@@ -28,16 +29,16 @@
 from ._config import ConfigWrapper
 from ._core_metadata import (
     CoreMetadataHandler,
     build_metadata_dict,
 )
 from ._core_utils import (
     CoreSchemaOrField,
-    consolidate_refs,
     define_expected_missing_refs,
+    flatten_schema_defs,
     get_type_ref,
     is_list_like_schema_with_items_schema,
     remove_unnecessary_invalid_definitions,
 )
 from ._decorators import (
     ComputedFieldInfo,
     Decorator,
@@ -57,16 +58,14 @@
     collect_dataclass_fields,
     get_type_hints_infer_globalns,
 )
 from ._forward_ref import PydanticRecursiveRef
 from ._generics import get_standard_typevars_map, recursively_defined_type_refs, replace_types
 from ._schema_generation_shared import (
     CallbackGetCoreSchemaHandler,
-    UnpackedRefJsonSchemaHandler,
-    wrap_json_schema_fn_for_model_or_custom_type_with_ref_unpacking,
 )
 from ._typing_extra import is_finalvar
 from ._utils import lenient_issubclass
 
 if TYPE_CHECKING:
     from ..main import BaseModel
     from ..validators import FieldValidatorModes
@@ -87,24 +86,44 @@
 GetCoreSchemaFunction = Callable[[Any, ModifyCoreSchemaWrapHandler], core_schema.CoreSchema]
 
 
 def check_validator_fields_against_field_name(
     info: FieldDecoratorInfo,
     field: str,
 ) -> bool:
+    """Check if field name is in validator fields.
+
+    Args:
+        info: The field info.
+        field: The field name to check.
+
+    Returns:
+        `True` if field name is in validator fields, `False` otherwise.
+    """
     if isinstance(info, (ValidatorDecoratorInfo, FieldValidatorDecoratorInfo)):
         if '*' in info.fields:
             return True
     for v_field_name in info.fields:
         if v_field_name == field:
             return True
     return False
 
 
 def check_decorator_fields_exist(decorators: Iterable[AnyFieldDecorator], fields: Iterable[str]) -> None:
+    """Check if the defined fields in decorators exist in `fields` param.
+
+    It ignores the check for a decorator if the decorator has `*` as field or `check_fields=False`.
+
+    Args:
+        decorators: An iterable of decorators.
+        fields: An iterable of fields name.
+
+    Raises:
+        PydanticUserError: If one of the field names does not exist in `fields` param.
+    """
     fields = set(fields)
     for dec in decorators:
         if isinstance(dec.info, (ValidatorDecoratorInfo, FieldValidatorDecoratorInfo)) and '*' in dec.info.fields:
             continue
         if dec.info.check_fields is False:
             continue
         for field in dec.info.fields:
@@ -151,58 +170,104 @@
         )
     return schema
 
 
 def modify_model_json_schema(
     schema_or_field: CoreSchemaOrField, handler: GetJsonSchemaHandler, *, cls: Any
 ) -> JsonSchemaValue:
-    """Add title and description for model-like classes' JSON schema"""
-    wrapped_handler = UnpackedRefJsonSchemaHandler(handler)
+    """Add title and description for model-like classes' JSON schema.
 
+    Args:
+        schema_or_field: The schema data to generate a JSON schema from.
+        handler: The `GetCoreSchemaHandler` instance.
+        cls: The model-like class.
+
+    Returns:
+        JsonSchemaValue: The updated JSON schema.
+    """
     json_schema = handler(schema_or_field)
-    original_schema = wrapped_handler.resolve_ref_schema(json_schema)
+    original_schema = handler.resolve_ref_schema(json_schema)
+    # Preserve the fact that definitions schemas should never have sibling keys:
+    if '$ref' in original_schema:
+        ref = original_schema['$ref']
+        original_schema.clear()
+        original_schema['allOf'] = [{'$ref': ref}]
     if 'title' not in original_schema:
         original_schema['title'] = cls.__name__
     docstring = cls.__doc__
     if docstring and 'description' not in original_schema:
         original_schema['description'] = docstring
     return json_schema
 
 
 class GenerateSchema:
-    __slots__ = '_config_wrapper_stack', 'types_namespace', 'typevars_map', 'recursion_cache', 'definitions'
+    """Generate core schema for a Pydantic model, dataclass and types like `str`, `datatime`, ... ."""
+
+    __slots__ = '_config_wrapper_stack', 'types_namespace', 'typevars_map', 'recursion_cache', 'definitions', 'defs'
 
     def __init__(
         self,
         config_wrapper: ConfigWrapper,
         types_namespace: dict[str, Any] | None,
         typevars_map: dict[Any, Any] | None = None,
     ):
         # we need a stack for recursing into child models
         self._config_wrapper_stack: list[ConfigWrapper] = [config_wrapper]
         self.types_namespace = types_namespace
         self.typevars_map = typevars_map
 
-        self.recursion_cache: dict[str, core_schema.DefinitionReferenceSchema] = {}
-        self.definitions: dict[str, core_schema.CoreSchema] = {}
+        self.defs = _Definitions()
 
     @property
     def config_wrapper(self) -> ConfigWrapper:
         return self._config_wrapper_stack[-1]
 
     @property
     def arbitrary_types(self) -> bool:
         return self.config_wrapper.arbitrary_types_allowed
 
+    def collect_definitions(self, schema: CoreSchema) -> CoreSchema:
+        ref = cast('str | None', schema.get('ref', None))
+        if ref:
+            self.defs.definitions[ref] = schema
+        return core_schema.definitions_schema(
+            schema,
+            list(self.defs.definitions.values()),
+        )
+
     def generate_schema(
         self,
         obj: Any,
         from_dunder_get_core_schema: bool = True,
         from_prepare_args: bool = True,
     ) -> core_schema.CoreSchema:
+        """Generate core schema.
+
+        Args:
+            obj: The object to generate core schema for.
+            from_dunder_get_core_schema: Whether to generate schema from either the
+                `__get_pydantic_core_schema__` function or `__pydantic_core_schema__` property.
+            from_prepare_args: Whether to generate schema from either the
+                `__prepare_pydantic_annotations__` function or `__prepare_pydantic_annotations__` property.
+
+        Returns:
+            The generated core schema.
+
+        Raises:
+            PydanticUndefinedAnnotation:
+                If it is not possible to evaluate forward reference.
+            PydanticSchemaGenerationError:
+                If it is not possible to generate pydantic-core schema.
+            TypeError:
+                - If `alias_generator` returns a non-string value.
+                - If V1 style validator with `each_item=True` applied on a wrong field.
+            PydanticUserError:
+                - If `typing.TypedDict` is used instead of `typing_extensions.TypedDict` on Python < 3.12.
+                - If `__modify_schema__` method is used instead of `__get_pydantic_json_schema__`.
+        """
         if isinstance(obj, type(Annotated[int, 123])):
             return self._annotated_schema(obj)
         return self._generate_schema_for_type(
             obj, from_dunder_get_core_schema=from_dunder_get_core_schema, from_prepare_args=from_prepare_args
         )
 
     def _generate_schema_for_type(
@@ -222,135 +287,168 @@
                 schema = from_property
 
         if schema is None:
             schema = self._generate_schema(obj)
 
         metadata_js_function = _extract_get_pydantic_json_schema(obj, schema)
         if metadata_js_function is not None:
-            metadata = CoreMetadataHandler(schema).metadata
-            metadata.setdefault('pydantic_js_functions', []).append(metadata_js_function)
-
-        schema = remove_unnecessary_invalid_definitions(schema)
-
-        ref = schema.get('ref', None)
-        if ref:
-            # definitions and definition-ref schemas don't have 'ref', causing the type error ignored on the next line
-            self.definitions[ref] = schema
-
-        return schema
-
-    def model_schema(self, cls: type[BaseModel]) -> core_schema.CoreSchema:
-        """
-        Generate schema for a pydantic model.
-
-        Since models generate schemas for themselves this method is public and can be called
-        from within BaseModel's metaclass.
-        """
-        model_ref, schema = self._get_or_cache_recursive_ref(cls)
-        if schema is not None:
-            return schema
-
-        fields = cls.model_fields
-        decorators = cls.__pydantic_decorators__
-        check_decorator_fields_exist(
-            chain(
-                decorators.field_validators.values(),
-                decorators.field_serializers.values(),
-                decorators.validators.values(),
-            ),
-            fields.keys(),
-        )
-        config_wrapper = ConfigWrapper(cls.model_config, check=False)
-        core_config = config_wrapper.core_config(cls)
-        metadata = build_metadata_dict(js_functions=[partial(modify_model_json_schema, cls=cls)])
-
-        model_validators = decorators.model_validators.values()
-
-        if cls.__pydantic_root_model__:
-            root_field = self._common_field_schema('root', fields['root'], decorators)
-            inner_schema = root_field['schema']
-            inner_schema = apply_model_validators(inner_schema, model_validators, 'inner')
-            model_schema = core_schema.model_schema(
-                cls,
-                inner_schema,
-                custom_init=getattr(cls, '__pydantic_custom_init__', None),
-                root_model=True,
-                post_init=getattr(cls, '__pydantic_post_init__', None),
-                config=core_config,
-                ref=model_ref,
-                metadata={**metadata, **root_field['metadata']},
+            metadata_schema = resolve_original_schema(schema, self.defs.definitions)
+            if metadata_schema:
+                metadata = CoreMetadataHandler(metadata_schema).metadata
+                metadata.setdefault('pydantic_js_functions', []).append(metadata_js_function)
+
+        return remove_unnecessary_invalid_definitions(schema)
+
+    def _model_schema(self, cls: type[BaseModel]) -> core_schema.CoreSchema:
+        """Generate schema for a Pydantic model."""
+        with self.defs.get_schema_or_ref(cls) as (model_ref, maybe_schema):
+            if maybe_schema is not None:
+                return maybe_schema
+
+            fields = cls.model_fields
+            decorators = cls.__pydantic_decorators__
+            check_decorator_fields_exist(
+                chain(
+                    decorators.field_validators.values(),
+                    decorators.field_serializers.values(),
+                    decorators.validators.values(),
+                ),
+                fields.keys(),
             )
-        else:
-            self._config_wrapper_stack.append(config_wrapper)
-            try:
-                fields_schema: core_schema.CoreSchema = core_schema.model_fields_schema(
-                    {k: self._generate_md_field_schema(k, v, decorators) for k, v in fields.items()},
-                    computed_fields=[self._computed_field_schema(d) for d in decorators.computed_fields.values()],
+            config_wrapper = ConfigWrapper(cls.model_config, check=False)
+            core_config = config_wrapper.core_config(cls)
+            metadata = build_metadata_dict(js_functions=[partial(modify_model_json_schema, cls=cls)])
+
+            model_validators = decorators.model_validators.values()
+
+            extra_validator = None
+            if core_config.get('extra_fields_behavior') == 'allow':
+                for tp in (cls, *cls.__mro__):
+                    extras_annotation = cls.__annotations__.get('__pydantic_extra__', None)
+                    if extras_annotation is not None:
+                        tp = get_origin(extras_annotation)
+                        if tp not in (Dict, dict):
+                            raise PydanticSchemaGenerationError(
+                                'The type annotation for `__pydantic_extra__` must be `Dict[str, ...]`'
+                            )
+                        extra_items_type = get_args(cls.__annotations__['__pydantic_extra__'])[1]
+                        if extra_items_type is not Any:
+                            extra_validator = self.generate_schema(extra_items_type)
+                            break
+
+            if cls.__pydantic_root_model__:
+                root_field = self._common_field_schema('root', fields['root'], decorators)
+                inner_schema = root_field['schema']
+                inner_schema = apply_model_validators(inner_schema, model_validators, 'inner')
+                model_schema = core_schema.model_schema(
+                    cls,
+                    inner_schema,
+                    custom_init=getattr(cls, '__pydantic_custom_init__', None),
+                    root_model=True,
+                    post_init=getattr(cls, '__pydantic_post_init__', None),
+                    config=core_config,
+                    ref=model_ref,
+                    metadata=metadata,
                 )
-            finally:
-                self._config_wrapper_stack.pop()
-
-            inner_schema = apply_validators(fields_schema, decorators.root_validators.values())
-            inner_schema = define_expected_missing_refs(inner_schema, recursively_defined_type_refs())
-            inner_schema = apply_model_validators(inner_schema, model_validators, 'inner')
+            else:
+                self._config_wrapper_stack.append(config_wrapper)
+                try:
+                    fields_schema: core_schema.CoreSchema = core_schema.model_fields_schema(
+                        {k: self._generate_md_field_schema(k, v, decorators) for k, v in fields.items()},
+                        computed_fields=[self._computed_field_schema(d) for d in decorators.computed_fields.values()],
+                        extra_validator=extra_validator,
+                    )
+                finally:
+                    self._config_wrapper_stack.pop()
 
-            model_schema = core_schema.model_schema(
-                cls,
-                inner_schema,
-                custom_init=getattr(cls, '__pydantic_custom_init__', None),
-                root_model=False,
-                post_init=getattr(cls, '__pydantic_post_init__', None),
-                config=core_config,
-                ref=model_ref,
-                metadata=metadata,
-            )
+                inner_schema = apply_validators(fields_schema, decorators.root_validators.values())
+                inner_schema = define_expected_missing_refs(inner_schema, recursively_defined_type_refs())
+                inner_schema = apply_model_validators(inner_schema, model_validators, 'inner')
+
+                model_schema = core_schema.model_schema(
+                    cls,
+                    inner_schema,
+                    custom_init=getattr(cls, '__pydantic_custom_init__', None),
+                    root_model=False,
+                    post_init=getattr(cls, '__pydantic_post_init__', None),
+                    config=core_config,
+                    ref=model_ref,
+                    metadata=metadata,
+                )
 
-        model_schema = consolidate_refs(model_schema)
-        schema = self._apply_model_serializers(model_schema, decorators.model_serializers.values())
-        return apply_model_validators(schema, model_validators, 'outer')
+            schema = self._apply_model_serializers(model_schema, decorators.model_serializers.values())
+            schema = apply_model_validators(schema, model_validators, 'outer')
+            self.defs.definitions[model_ref] = schema
+            return core_schema.definition_reference_schema(model_ref)
 
     def _generate_schema_from_prepare_annotations(self, obj: Any) -> core_schema.CoreSchema | None:
-        """
-        Try to generate schema from either the `__get_pydantic_core_schema__` function or
-        `__pydantic_core_schema__` property.
-
-        Note: `__get_pydantic_core_schema__` takes priority so it can
-        decide whether to use a `__pydantic_core_schema__` attribute, or generate a fresh schema.
+        """Try to generate schema from either the `__prepare_pydantic_annotations__` function or
+        `__prepare_pydantic_annotations__` property.
         """
         new_obj, new_annotations = self._prepare_annotations(obj, [])
         if new_obj is not obj or new_annotations:
             return self._apply_annotations(
                 lambda x: x,
                 new_obj,
                 new_annotations,
             )
         return None
 
-    def _generate_schema_from_property(self, obj: Any, source: Any) -> core_schema.CoreSchema | None:
+    def _unpack_refs_defs(self, schema: CoreSchema) -> CoreSchema:
+        """Unpack all 'definitions' schemas into `GenerateSchema.defs.definitions`
+        and return the inner schema.
         """
-        Try to generate schema from either the `__get_pydantic_core_schema__` function or
+
+        def get_ref(s: CoreSchema) -> str:
+            return s['ref']  # type: ignore
+
+        schema = flatten_schema_defs(schema)
+
+        if schema['type'] == 'definitions':
+            self.defs.definitions.update({get_ref(s): s for s in schema['definitions']})
+            schema = schema['schema']
+        return schema
+
+    def _generate_schema_from_property(self, obj: Any, source: Any) -> core_schema.CoreSchema | None:
+        """Try to generate schema from either the `__get_pydantic_core_schema__` function or
         `__pydantic_core_schema__` property.
 
         Note: `__get_pydantic_core_schema__` takes priority so it can
         decide whether to use a `__pydantic_core_schema__` attribute, or generate a fresh schema.
         """
+        # avoid calling `__get_pydantic_core_schema__` if we've already visited this object
+        with self.defs.get_schema_or_ref(obj) as (_, maybe_schema):
+            if maybe_schema is not None:
+                return maybe_schema
+        if obj is source:
+            ref_mode = 'unpack'
+        else:
+            ref_mode = 'to-def'
+
         get_schema = getattr(obj, '__get_pydantic_core_schema__', None)
         if get_schema is None:
             return None
 
+        schema: CoreSchema
         if len(inspect.signature(get_schema).parameters) == 1:
             # (source) -> CoreSchema
-            return get_schema(source)
+            schema = get_schema(source)
+        else:
+            schema = get_schema(source, CallbackGetCoreSchemaHandler(self._generate_schema, self, ref_mode=ref_mode))
+
+        schema = self._unpack_refs_defs(schema)
 
-        return get_schema(source, CallbackGetCoreSchemaHandler(self._generate_schema, self.generate_schema))
+        ref: str | None = schema.get('ref', None)
+        if ref:
+            self.defs.definitions[ref] = schema
+            return core_schema.definition_reference_schema(ref)
+        return schema
 
     def _generate_schema(self, obj: Any) -> core_schema.CoreSchema:  # noqa: C901
-        """
-        Recursively generate a pydantic-core schema for any supported python type.
-        """
+        """Recursively generate a pydantic-core schema for any supported python type."""
         if isinstance(obj, dict):
             # we assume this is already a valid schema
             return obj  # type: ignore[return-value]
 
         if isinstance(obj, str):
             obj = ForwardRef(obj)
 
@@ -375,15 +473,15 @@
                 obj = replace_types(obj, self.typevars_map)
 
             return self.generate_schema(obj)
 
         from ..main import BaseModel
 
         if lenient_issubclass(obj, BaseModel):
-            return self.model_schema(obj)
+            return self._model_schema(obj)
 
         if isinstance(obj, PydanticRecursiveRef):
             return core_schema.definition_reference_schema(schema_ref=obj.type_ref)
 
         try:
             if obj in {bool, int, float, str, bytes, list, set, frozenset, dict}:
                 # Note: obj may fail to be hashable if it has an unhashable annotation
@@ -418,18 +516,27 @@
             return self._unsubstituted_typevar_schema(obj)
         elif is_finalvar(obj):
             if obj is Final:
                 return core_schema.AnySchema(type='any')
             return self.generate_schema(get_args(obj)[0])
         elif isinstance(obj, (FunctionType, LambdaType, MethodType, partial)):
             return self._callable_schema(obj)
+        elif inspect.isclass(obj) and issubclass(obj, Enum):
+            from ._std_types_schema import get_enum_core_schema
+
+            return get_enum_core_schema(obj)
 
         if _typing_extra.is_dataclass(obj):
             return self._dataclass_schema(obj, None)
 
+        res = self._get_prepare_pydantic_annotations_for_known_type(obj, ())
+        if res is not None:
+            source_type, annotations = res
+            return self._apply_annotations(lambda x: x, source_type, annotations)
+
         origin = get_origin(obj)
 
         if isinstance(obj, TypeAliasType) or isinstance(origin, TypeAliasType):
             return self._type_alias_type_schema(obj)
 
         if origin is None:
             return self._arbitrary_type_schema(obj, obj)
@@ -487,17 +594,15 @@
         self,
         name: str,
         field_info: FieldInfo,
         decorators: DecoratorInfos,
         *,
         required: bool = True,
     ) -> core_schema.TypedDictField:
-        """
-        Prepare a TypedDictField to represent a model or typeddict field.
-        """
+        """Prepare a TypedDictField to represent a model or typeddict field."""
         common_field = self._common_field_schema(name, field_info, decorators)
         return core_schema.typed_dict_field(
             common_field['schema'],
             required=False if not field_info.is_required() else required,
             serialization_exclude=common_field['serialization_exclude'],
             validation_alias=common_field['validation_alias'],
             serialization_alias=common_field['serialization_alias'],
@@ -505,20 +610,16 @@
         )
 
     def _generate_md_field_schema(
         self,
         name: str,
         field_info: FieldInfo,
         decorators: DecoratorInfos,
-        *,
-        required: bool = True,
     ) -> core_schema.ModelField:
-        """
-        Prepare a ModelField to represent a model field.
-        """
+        """Prepare a ModelField to represent a model field."""
         common_field = self._common_field_schema(name, field_info, decorators)
         return core_schema.model_field(
             common_field['schema'],
             serialization_exclude=common_field['serialization_exclude'],
             validation_alias=common_field['validation_alias'],
             serialization_alias=common_field['serialization_alias'],
             frozen=common_field['frozen'],
@@ -527,17 +628,15 @@
 
     def _generate_dc_field_schema(
         self,
         name: str,
         field_info: FieldInfo,
         decorators: DecoratorInfos,
     ) -> core_schema.DataclassField:
-        """
-        Prepare a DataclassField to represent the parameter/field, of a dataclass
-        """
+        """Prepare a DataclassField to represent the parameter/field, of a dataclass."""
         common_field = self._common_field_schema(name, field_info, decorators)
         return core_schema.dataclass_field(
             name,
             common_field['schema'],
             init_only=field_info.init_var or None,
             kw_only=None if field_info.kw_only else False,
             serialization_exclude=common_field['serialization_exclude'],
@@ -548,15 +647,17 @@
         )
 
     def _common_field_schema(self, name: str, field_info: FieldInfo, decorators: DecoratorInfos) -> _CommonField:
         assert field_info.annotation is not None, 'field_info.annotation should not be None when generating a schema'
 
         def apply_discriminator(schema: CoreSchema) -> CoreSchema:
             if field_info.discriminator is not None:
-                schema = _discriminated_union.apply_discriminator(schema, field_info.discriminator, self.definitions)
+                schema = _discriminated_union.apply_discriminator(
+                    schema, field_info.discriminator, self.defs.definitions
+                )
             return schema
 
         source_type, annotations = field_info.annotation, field_info.metadata
         schema = self._apply_annotations(
             apply_discriminator,
             source_type,
             annotations,
@@ -622,17 +723,15 @@
             validation_alias=validation_alias,
             serialization_alias=field_info.serialization_alias,
             frozen=field_info.frozen or field_info.final,
             metadata=metadata,
         )
 
     def _union_schema(self, union_type: Any) -> core_schema.CoreSchema:
-        """
-        Generate schema for a Union.
-        """
+        """Generate schema for a Union."""
         args = get_args(union_type)
         choices: list[core_schema.CoreSchema] = []
         nullable = False
         for arg in args:
             if arg is None or arg is _typing_extra.NoneType:
                 nullable = True
             else:
@@ -648,119 +747,111 @@
         return s
 
     def _type_alias_type_schema(
         self,
         obj: Any,  # TypeAliasType
     ) -> CoreSchema:
         origin = get_origin(obj)
-        if origin is not None and _typing_extra.origin_is_type_alias_type(origin):  # type: ignore
-            origin = cast(Any, origin)
-            ref, schema = self._get_or_cache_recursive_ref(origin)
-            if schema is not None:
-                return schema
+        origin = origin or obj
+        with self.defs.get_schema_or_ref(origin) as (ref, maybe_schema):
+            if maybe_schema is not None:
+                return maybe_schema
+
             namespace = (self.types_namespace or {}).copy()
             new_namespace = {**_typing_extra.get_cls_types_namespace(origin), **namespace}
             annotation = origin.__value__
-        else:
-            ref, schema = self._get_or_cache_recursive_ref(obj)
-            if schema is not None:
-                return schema
-            namespace = (self.types_namespace or {}).copy()
-            new_namespace = {**_typing_extra.get_cls_types_namespace(obj), **namespace}
-            annotation = obj.__value__
-        self.types_namespace = new_namespace
-        typevars_map = get_standard_typevars_map(obj)
-        annotation = replace_types(annotation, typevars_map)
-        schema = self.generate_schema(annotation)
-        assert schema['type'] != 'definitions'
-        schema['ref'] = ref  # type: ignore
-        self.types_namespace = namespace or None
-        self.recursion_cache[obj] = schema  # type: ignore
-        self.definitions[ref] = schema
-        return schema
+
+            self.types_namespace = new_namespace
+            typevars_map = get_standard_typevars_map(obj)
+            annotation = replace_types(annotation, typevars_map)
+            schema = self.generate_schema(annotation)
+            assert schema['type'] != 'definitions'
+            schema['ref'] = ref  # type: ignore
+            self.types_namespace = namespace or None
+            self.defs.definitions[ref] = schema
+            return core_schema.definition_reference_schema(ref)
 
     def _literal_schema(self, literal_type: Any) -> core_schema.LiteralSchema:
-        """
-        Generate schema for a Literal.
-        """
+        """Generate schema for a Literal."""
         expected = _typing_extra.all_literal_values(literal_type)
         assert expected, f'literal "expected" cannot be empty, obj={literal_type}'
         return core_schema.literal_schema(expected)
 
     def _typed_dict_schema(self, typed_dict_cls: Any, origin: Any) -> core_schema.CoreSchema:
-        """
-        Generate schema for a TypedDict.
+        """Generate schema for a TypedDict.
 
         It is not possible to track required/optional keys in TypedDict without __required_keys__
         since TypedDict.__new__ erases the base classes (it replaces them with just `dict`)
         and thus we can track usage of total=True/False
         __required_keys__ was added in Python 3.9
         (https://github.com/miss-islington/cpython/blob/1e9939657dd1f8eb9f596f77c1084d2d351172fc/Doc/library/typing.rst?plain=1#L1546-L1548)
         however it is buggy
         (https://github.com/python/typing_extensions/blob/ac52ac5f2cb0e00e7988bae1e2a1b8257ac88d6d/src/typing_extensions.py#L657-L666).
         Hence to avoid creating validators that do not do what users expect we only
         support typing.TypedDict on Python >= 3.11 or typing_extension.TypedDict on all versions
         """
-        typed_dict_ref, schema = self._get_or_cache_recursive_ref(typed_dict_cls)
-        if schema is not None:
-            return schema
-
-        typevars_map = get_standard_typevars_map(typed_dict_cls)
-        if origin is not None:
-            typed_dict_cls = origin
-
-        if not _SUPPORTS_TYPEDDICT and type(typed_dict_cls).__module__ == 'typing':
-            raise PydanticUserError(
-                'Please use `typing_extensions.TypedDict` instead of `typing.TypedDict` on Python < 3.12.',
-                code='typed-dict-version',
-            )
-
-        config: ConfigDict | None = getattr(typed_dict_cls, '__pydantic_config__', None)
-        config_wrapper = ConfigWrapper(config)
-        core_config = config_wrapper.core_config(None)
-
-        required_keys: frozenset[str] = typed_dict_cls.__required_keys__
+        with self.defs.get_schema_or_ref(typed_dict_cls) as (typed_dict_ref, maybe_schema):
+            if maybe_schema is not None:
+                return maybe_schema
+
+            typevars_map = get_standard_typevars_map(typed_dict_cls)
+            if origin is not None:
+                typed_dict_cls = origin
 
-        fields: dict[str, core_schema.TypedDictField] = {}
+            if not _SUPPORTS_TYPEDDICT and type(typed_dict_cls).__module__ == 'typing':
+                raise PydanticUserError(
+                    'Please use `typing_extensions.TypedDict` instead of `typing.TypedDict` on Python < 3.12.',
+                    code='typed-dict-version',
+                )
 
-        decorators = DecoratorInfos.build(typed_dict_cls)
+            config: ConfigDict | None = getattr(typed_dict_cls, '__pydantic_config__', None)
+            config_wrapper = ConfigWrapper(config)
+            core_config = config_wrapper.core_config(None)
+
+            required_keys: frozenset[str] = typed_dict_cls.__required_keys__
+
+            fields: dict[str, core_schema.TypedDictField] = {}
+
+            decorators = DecoratorInfos.build(typed_dict_cls)
+
+            for field_name, annotation in get_type_hints_infer_globalns(
+                typed_dict_cls, localns=self.types_namespace, include_extras=True
+            ).items():
+                annotation = replace_types(annotation, typevars_map)
+                required = field_name in required_keys
+
+                if get_origin(annotation) == _typing_extra.Required:
+                    required = True
+                    annotation = get_args(annotation)[0]
+                elif get_origin(annotation) == _typing_extra.NotRequired:
+                    required = False
+                    annotation = get_args(annotation)[0]
+
+                field_info = FieldInfo.from_annotation(annotation)
+                fields[field_name] = self._generate_td_field_schema(
+                    field_name, field_info, decorators, required=required
+                )
 
-        for field_name, annotation in get_type_hints_infer_globalns(
-            typed_dict_cls, localns=self.types_namespace, include_extras=True
-        ).items():
-            annotation = replace_types(annotation, typevars_map)
-            required = field_name in required_keys
+            metadata = build_metadata_dict(js_functions=[partial(modify_model_json_schema, cls=typed_dict_cls)])
 
-            if get_origin(annotation) == _typing_extra.Required:
-                required = True
-                annotation = get_args(annotation)[0]
-            elif get_origin(annotation) == _typing_extra.NotRequired:
-                required = False
-                annotation = get_args(annotation)[0]
-
-            field_info = FieldInfo.from_annotation(annotation)
-            fields[field_name] = self._generate_td_field_schema(field_name, field_info, decorators, required=required)
-
-        metadata = build_metadata_dict(js_functions=[partial(modify_model_json_schema, cls=typed_dict_cls)])
-
-        td_schema = core_schema.typed_dict_schema(
-            fields,
-            extra_behavior='forbid',
-            ref=typed_dict_ref,
-            metadata=metadata,
-            config=core_config,
-        )
+            td_schema = core_schema.typed_dict_schema(
+                fields,
+                computed_fields=[self._computed_field_schema(d) for d in decorators.computed_fields.values()],
+                ref=typed_dict_ref,
+                metadata=metadata,
+                config=core_config,
+            )
 
-        schema = self._apply_model_serializers(td_schema, decorators.model_serializers.values())
-        return apply_model_validators(schema, decorators.model_validators.values(), 'all')
+            schema = self._apply_model_serializers(td_schema, decorators.model_serializers.values())
+            schema = apply_model_validators(schema, decorators.model_validators.values(), 'all')
+            self.defs.definitions[typed_dict_ref] = schema
+            return core_schema.definition_reference_schema(typed_dict_ref)
 
     def _namedtuple_schema(self, namedtuple_cls: Any) -> core_schema.CallSchema:
-        """
-        Generate schema for a NamedTuple.
-        """
+        """Generate schema for a NamedTuple."""
         annotations: dict[str, Any] = get_type_hints_infer_globalns(
             namedtuple_cls, include_extras=True, localns=self.types_namespace
         )
         if not annotations:
             # annotations is empty, happens if namedtuple_cls defined via collections.namedtuple(...)
             annotations = {k: Any for k in namedtuple_cls._fields}
 
@@ -777,17 +868,15 @@
     def _generate_parameter_schema(
         self,
         name: str,
         annotation: type[Any],
         default: Any = Parameter.empty,
         mode: Literal['positional_only', 'positional_or_keyword', 'keyword_only'] | None = None,
     ) -> core_schema.ArgumentsParameter:
-        """
-        Prepare a ArgumentsParameter to represent a field in a namedtuple or function signature.
-        """
+        """Prepare a ArgumentsParameter to represent a field in a namedtuple or function signature."""
         if default is Parameter.empty:
             field = FieldInfo.from_annotation(annotation)
         else:
             field = FieldInfo.from_annotated_attribute(annotation, default)
         assert field.annotation is not None, 'field.annotation should not be None when generating a schema'
         source_type, annotations = field.annotation, field.metadata
         schema = self._apply_annotations(lambda x: x, source_type, annotations)
@@ -803,17 +892,15 @@
         else:
             alias_generator = self.config_wrapper.alias_generator
             if alias_generator:
                 parameter_schema['alias'] = alias_generator(name)
         return parameter_schema
 
     def _tuple_schema(self, tuple_type: Any) -> core_schema.CoreSchema:
-        """
-        Generate schema for a Tuple, e.g. `tuple[int, str]` or `tuple[int, ...]`.
-        """
+        """Generate schema for a Tuple, e.g. `tuple[int, str]` or `tuple[int, ...]`."""
         params = get_args(tuple_type)
         # NOTE: subtle difference: `tuple[()]` gives `params=()`, whereas `typing.Tuple[()]` gives `params=((),)`
         # This is only true for <3.11, on Python 3.11+ `typing.Tuple[()]` gives `params=()`
         if not params:
             if tuple_type == typing.Tuple:
                 return core_schema.tuple_variable_schema()
             else:
@@ -841,17 +928,15 @@
         return core_schema.custom_error_schema(
             core_schema.is_instance_schema(type),
             custom_error_type='is_type',
             custom_error_message='Input should be a type',
         )
 
     def _subclass_schema(self, type_: Any) -> core_schema.CoreSchema:
-        """
-        Generate schema for a Type, e.g. `Type[int]`.
-        """
+        """Generate schema for a Type, e.g. `Type[int]`."""
         type_param = get_first_arg(type_)
         if type_param == Any:
             return self._type_schema()
         elif isinstance(type_param, typing.TypeVar):
             if type_param.__bound__:
                 return core_schema.is_subclass_schema(type_param.__bound__)
             elif type_param.__constraints__:
@@ -860,17 +945,15 @@
                 )
             else:
                 return self._type_schema()
         else:
             return core_schema.is_subclass_schema(type_param)
 
     def _sequence_schema(self, sequence_type: Any) -> core_schema.CoreSchema:
-        """
-        Generate schema for a Sequence, e.g. `Sequence[int]`.
-        """
+        """Generate schema for a Sequence, e.g. `Sequence[int]`."""
         item_type = get_first_arg(sequence_type)
 
         def json_schema_func(_schema: CoreSchemaOrField, handler: GetJsonSchemaHandler) -> JsonSchemaValue:
             items_schema = self._generate_schema(item_type)
             return handler(core_schema.list_schema(items_schema))
 
         metadata = build_metadata_dict(js_functions=[json_schema_func])
@@ -884,17 +967,15 @@
                 [python_schema, core_schema.no_info_wrap_validator_function(sequence_validator, list_schema)],
             )
         return core_schema.json_or_python_schema(
             json_schema=list_schema, python_schema=python_schema, metadata=metadata
         )
 
     def _iterable_schema(self, type_: Any) -> core_schema.GeneratorSchema:
-        """
-        Generate a schema for an `Iterable`.
-        """
+        """Generate a schema for an `Iterable`."""
         item_type = get_first_arg(type_)
 
         return core_schema.generator_schema(self.generate_schema(item_type))
 
     def _pattern_schema(self, pattern_type: Any) -> core_schema.CoreSchema:
         from . import _validators
 
@@ -926,87 +1007,86 @@
             custom_error_type='is_hashable',
             custom_error_message='Input should be hashable',
         )
 
     def _dataclass_schema(
         self, dataclass: type[StandardDataclass], origin: type[StandardDataclass] | None
     ) -> core_schema.CoreSchema:
-        """
-        Generate schema for a dataclass.
-        """
-        dataclass_ref, schema = self._get_or_cache_recursive_ref(dataclass)
-        if schema is not None:
-            return schema
-
-        typevars_map = get_standard_typevars_map(dataclass)
-        if origin is not None:
-            dataclass = origin
-
-        from ._dataclasses import is_pydantic_dataclass
-
-        if is_pydantic_dataclass(dataclass):
-            fields = dataclass.__pydantic_fields__
-            if typevars_map:
-                for field in fields.values():
-                    field.apply_typevars_map(typevars_map, self.types_namespace)
-        else:
-            fields = collect_dataclass_fields(
-                dataclass,
-                self.types_namespace,
-                typevars_map=typevars_map,
+        """Generate schema for a dataclass."""
+        with self.defs.get_schema_or_ref(dataclass) as (dataclass_ref, maybe_schema):
+            if maybe_schema is not None:
+                return maybe_schema
+
+            typevars_map = get_standard_typevars_map(dataclass)
+            if origin is not None:
+                dataclass = origin
+
+            from ._dataclasses import is_pydantic_dataclass
+
+            if is_pydantic_dataclass(dataclass):
+                fields = dataclass.__pydantic_fields__
+                if typevars_map:
+                    for field in fields.values():
+                        field.apply_typevars_map(typevars_map, self.types_namespace)
+            else:
+                fields = collect_dataclass_fields(
+                    dataclass,
+                    self.types_namespace,
+                    typevars_map=typevars_map,
+                )
+            decorators = dataclass.__dict__.get('__pydantic_decorators__') or DecoratorInfos.build(dataclass)
+            # Move kw_only=False args to the start of the list, as this is how vanilla dataclasses work.
+            # Note that when kw_only is missing or None, it is treated as equivalent to kw_only=True
+            args = sorted(
+                (self._generate_dc_field_schema(k, v, decorators) for k, v in fields.items()),
+                key=lambda a: a.get('kw_only') is not False,
             )
-        decorators = dataclass.__dict__.get('__pydantic_decorators__') or DecoratorInfos.build(dataclass)
-        # Move kw_only=False args to the start of the list, as this is how vanilla dataclasses work.
-        # Note that when kw_only is missing or None, it is treated as equivalent to kw_only=True
-        args = sorted(
-            (self._generate_dc_field_schema(k, v, decorators) for k, v in fields.items()),
-            key=lambda a: a.get('kw_only') is not False,
-        )
-        has_post_init = hasattr(dataclass, '__post_init__')
-        has_slots = hasattr(dataclass, '__slots__')
-
-        config = getattr(dataclass, '__pydantic_config__', None)
-        if config is not None:
-            config_wrapper = ConfigWrapper(config, check=False)
-            self._config_wrapper_stack.append(config_wrapper)
-            core_config = config_wrapper.core_config(dataclass)
-        else:
-            core_config = None
+            has_post_init = hasattr(dataclass, '__post_init__')
+            has_slots = hasattr(dataclass, '__slots__')
 
-        try:
-            args_schema = core_schema.dataclass_args_schema(
-                dataclass.__name__,
-                args,
-                computed_fields=[self._computed_field_schema(d) for d in decorators.computed_fields.values()],
-                collect_init_only=has_post_init,
-            )
-        finally:
+            config = getattr(dataclass, '__pydantic_config__', None)
             if config is not None:
-                self._config_wrapper_stack.pop()
+                config_wrapper = ConfigWrapper(config, check=False)
+                self._config_wrapper_stack.append(config_wrapper)
+                core_config = config_wrapper.core_config(dataclass)
+            else:
+                core_config = None
 
-        inner_schema = apply_validators(args_schema, decorators.root_validators.values())
+            try:
+                args_schema = core_schema.dataclass_args_schema(
+                    dataclass.__name__,
+                    args,
+                    computed_fields=[self._computed_field_schema(d) for d in decorators.computed_fields.values()],
+                    collect_init_only=has_post_init,
+                )
+            finally:
+                if config is not None:
+                    self._config_wrapper_stack.pop()
 
-        model_validators = decorators.model_validators.values()
-        inner_schema = apply_model_validators(inner_schema, model_validators, 'inner')
+            inner_schema = apply_validators(args_schema, decorators.root_validators.values())
 
-        dc_schema = core_schema.dataclass_schema(
-            dataclass,
-            inner_schema,
-            post_init=has_post_init,
-            ref=dataclass_ref,
-            fields=[field.name for field in dataclasses.fields(dataclass)],
-            slots=has_slots,
-            config=core_config,
-        )
-        schema = self._apply_model_serializers(dc_schema, decorators.model_serializers.values())
-        return apply_model_validators(schema, model_validators, 'outer')
+            model_validators = decorators.model_validators.values()
+            inner_schema = apply_model_validators(inner_schema, model_validators, 'inner')
+
+            dc_schema = core_schema.dataclass_schema(
+                dataclass,
+                inner_schema,
+                post_init=has_post_init,
+                ref=dataclass_ref,
+                fields=[field.name for field in dataclasses.fields(dataclass)],
+                slots=has_slots,
+                config=core_config,
+            )
+            schema = self._apply_model_serializers(dc_schema, decorators.model_serializers.values())
+            schema = apply_model_validators(schema, model_validators, 'outer')
+            self.defs.definitions[dataclass_ref] = schema
+            return core_schema.definition_reference_schema(dataclass_ref)
 
     def _callable_schema(self, function: Callable[..., Any]) -> core_schema.CallSchema:
-        """
-        Generate schema for a Callable.
+        """Generate schema for a Callable.
 
         TODO support functional validators once we support them in Config
         """
         sig = signature(function)
 
         type_hints = _typing_extra.get_function_type_hints(function)
 
@@ -1060,22 +1140,14 @@
         if typevar.__bound__:
             return self.generate_schema(typevar.__bound__)
         elif typevar.__constraints__:
             return self._union_schema(typing.Union[typevar.__constraints__])  # type: ignore
         else:
             return core_schema.AnySchema(type='any')
 
-    def _get_or_cache_recursive_ref(self, cls: type[Any]) -> tuple[str, core_schema.DefinitionReferenceSchema | None]:
-        obj_ref = get_type_ref(cls)
-        if obj_ref in self.recursion_cache:
-            return obj_ref, self.recursion_cache[obj_ref]
-        else:
-            self.recursion_cache[obj_ref] = core_schema.definition_reference_schema(obj_ref)
-            return obj_ref, None
-
     def _computed_field_schema(self, d: Decorator[ComputedFieldInfo]) -> core_schema.ComputedField:
         return_type_schema = self.generate_schema(d.info.return_type)
 
         # Handle alias_generator using similar logic to that from
         # pydantic._internal._generate_schema.GenerateSchema._common_field_schema,
         # with field_info -> d.info and name -> d.cls_var_name
         alias_generator = self.config_wrapper.alias_generator
@@ -1085,17 +1157,15 @@
                 raise TypeError(f'alias_generator {alias_generator} must return str, not {alias.__class__}')
             d.info.alias = alias
             d.info.alias_priority = 1
 
         return core_schema.computed_field(d.cls_var_name, return_schema=return_type_schema, alias=d.info.alias)
 
     def _annotated_schema(self, annotated_type: Any) -> core_schema.CoreSchema:
-        """
-        Generate schema for an Annotated type, e.g. `Annotated[int, Field(...)]` or `Annotated[int, Gt(0)]`.
-        """
+        """Generate schema for an Annotated type, e.g. `Annotated[int, Field(...)]` or `Annotated[int, Gt(0)]`."""
         source_type, *annotations = get_args(annotated_type)
         schema = self._apply_annotations(lambda x: x, source_type, annotations)
         # put the default validator last so that TypeAdapter.get_default_value() works
         # even if there are function validators involved
         for annotation in annotations:
             if isinstance(annotation, FieldInfo):
                 schema = wrap_default(annotation, schema)
@@ -1110,21 +1180,20 @@
             res = gen(obj, annotations, self.config_wrapper.config_dict)
             if res is not None:
                 return res
 
         return None
 
     def _prepare_annotations(self, source_type: Any, annotations: Iterable[Any]) -> tuple[Any, list[Any]]:
-        """
-        Call `__prepare_pydantic_annotations__` if it exists and return a tuple of (new_source_type, new_annotations).
+        """Call `__prepare_pydantic_annotations__` if it exists and return a tuple of
+            (new_source_type, new_annotations).
 
         This should be treated conceptually similar to the transformation
         `Annotated[source_type, *annotations]` -> `Annotated[new_source_type, *new_annotations]`
         """
-
         prepare = getattr(source_type, '__prepare_pydantic_annotations__', None)
 
         annotations = tuple(annotations)  # make them immutable to avoid confusion over mutating them
 
         if prepare is not None:
             source_type, annotations = prepare(source_type, tuple(annotations), self.config_wrapper.config_dict)
             annotations = list(annotations)
@@ -1137,16 +1206,15 @@
 
     def _apply_annotations(
         self,
         transform_inner_schema: Callable[[CoreSchema], CoreSchema],
         source_type: Any,
         annotations: list[Any],
     ) -> CoreSchema:
-        """
-        Apply arguments from `Annotated` or from `FieldInfo` to a schema.
+        """Apply arguments from `Annotated` or from `FieldInfo` to a schema.
 
         This gets called by `GenerateSchema._annotated_schema` but differs from it in that it does
         not expect `source_type` to be an `Annotated` object, it expects it to be  the first argument of that
         (in other words, `GenerateSchema._annotated_schema` just unpacks `Annotated`, this process it).
         """
         # expand annotations before we start processing them so that `__prepare_pydantic_annotations` can consume
         # individual items from GroupedMetadata
@@ -1173,15 +1241,15 @@
                 else:
                     schema = from_property
                 metadata_js_function = _extract_get_pydantic_json_schema(obj, schema)
                 if metadata_js_function is not None:
                     pydantic_js_functions.append(metadata_js_function)
             return transform_inner_schema(schema)
 
-        get_inner_schema = CallbackGetCoreSchemaHandler(inner_handler, self.generate_schema)
+        get_inner_schema = CallbackGetCoreSchemaHandler(inner_handler, self)
 
         while True:
             idx += 1
             if idx == len(annotations):
                 break
             annotation = annotations[idx]
             if annotation is None:
@@ -1195,52 +1263,101 @@
                 if new_source_type is not source_type:
                     return self._apply_annotations(
                         transform_inner_schema,
                         new_source_type,
                         annotations,
                     )
             annotation = annotations[idx]
-            get_inner_schema = self._get_wrapped_inner_schema(
-                get_inner_schema, annotation, self.definitions, pydantic_js_functions
-            )
+            get_inner_schema = self._get_wrapped_inner_schema(get_inner_schema, annotation, pydantic_js_functions)
 
         schema = get_inner_schema(source_type)
-        metadata = CoreMetadataHandler(schema).metadata
-        metadata.setdefault('pydantic_js_functions', []).extend(pydantic_js_functions)
+        if pydantic_js_functions:
+            metadata = CoreMetadataHandler(schema).metadata
+            metadata.setdefault('pydantic_js_functions', []).extend(pydantic_js_functions)
         return schema
 
+    def apply_single_annotation(self, schema: core_schema.CoreSchema, metadata: Any) -> core_schema.CoreSchema:
+        if isinstance(metadata, FieldInfo):
+            for field_metadata in metadata.metadata:
+                schema = self.apply_single_annotation(schema, field_metadata)
+            if metadata.discriminator is not None:
+                schema = _discriminated_union.apply_discriminator(
+                    schema,
+                    metadata.discriminator,
+                    self.defs.definitions,
+                )
+            return schema
+
+        if schema['type'] == 'nullable':
+            # for nullable schemas, metadata is automatically applied to the inner schema
+            inner = schema.get('schema', core_schema.any_schema())
+            inner = self.apply_single_annotation(inner, metadata)
+            if inner:
+                schema['schema'] = inner
+            return schema
+
+        original_schema = schema
+        ref = schema.get('ref', None)
+        if ref is not None:
+            schema = schema.copy()
+            new_ref = ref + f'_{repr(metadata)}'
+            if new_ref in self.defs.definitions:
+                return self.defs.definitions[new_ref]
+            schema['ref'] = new_ref  # type: ignore
+        elif schema['type'] == 'definition-ref':
+            ref = schema['schema_ref']
+            if ref in self.defs.definitions:
+                schema = self.defs.definitions[ref].copy()
+                new_ref = ref + f'_{repr(metadata)}'
+                if new_ref in self.defs.definitions:
+                    return self.defs.definitions[new_ref]
+                schema['ref'] = new_ref  # type: ignore
+
+        maybe_updated_schema = _known_annotated_metadata.apply_known_metadata(metadata, schema.copy())
+
+        if maybe_updated_schema is not None:
+            return maybe_updated_schema
+        return original_schema
+
     def _get_wrapped_inner_schema(
         self,
         get_inner_schema: GetCoreSchemaHandler,
         annotation: Any,
-        definitions: dict[str, core_schema.CoreSchema],
         pydantic_js_functions: list[GetJsonSchemaFunction],
     ) -> CallbackGetCoreSchemaHandler:
         metadata_get_schema: GetCoreSchemaFunction = getattr(annotation, '__get_pydantic_core_schema__', None) or (
             lambda source, handler: handler(source)
         )
 
         def new_handler(source: Any) -> core_schema.CoreSchema:
             schema = metadata_get_schema(source, get_inner_schema)
-            schema = apply_single_annotation(schema, annotation, definitions)
+            schema = self.apply_single_annotation(schema, annotation)
 
             metadata_js_function = _extract_get_pydantic_json_schema(annotation, schema)
             if metadata_js_function is not None:
                 pydantic_js_functions.append(metadata_js_function)
             return schema
 
-        return CallbackGetCoreSchemaHandler(new_handler, self.generate_schema)
+        return CallbackGetCoreSchemaHandler(new_handler, self)
 
     def _apply_field_serializers(
         self, schema: core_schema.CoreSchema, serializers: list[Decorator[FieldSerializerDecoratorInfo]]
     ) -> core_schema.CoreSchema:
-        """
-        Apply field serializers to a schema.
-        """
+        """Apply field serializers to a schema."""
         if serializers:
+            schema = copy(schema)
+            if schema['type'] == 'definitions':
+                inner_schema = schema['schema']
+                schema['schema'] = self._apply_field_serializers(inner_schema, serializers)
+                return schema
+            else:
+                ref = typing.cast('str|None', schema.get('ref', None))
+                if ref is not None:
+                    schema = core_schema.definition_reference_schema(ref)
+
             # use the last serializer to make it easy to override a serializer set on a parent model
             serializer = serializers[-1]
             is_field_serializer, info_arg = inspect_field_serializer(serializer.func, serializer.info.mode)
 
             if serializer.info.return_type is None:
                 return_schema = None
             else:
@@ -1264,17 +1381,15 @@
                     when_used=serializer.info.when_used,
                 )
         return schema
 
     def _apply_model_serializers(
         self, schema: core_schema.CoreSchema, serializers: Iterable[Decorator[ModelSerializerDecoratorInfo]]
     ) -> core_schema.CoreSchema:
-        """
-        Apply model serializers to a schema.
-        """
+        """Apply model serializers to a schema."""
         ref: str | None = schema.pop('ref', None)  # type: ignore
         if serializers:
             serializer = list(serializers)[-1]
             info_arg = inspect_model_serializer(serializer.func, serializer.info.mode)
 
             if serializer.info.return_type is None:
                 return_schema = None
@@ -1323,32 +1438,37 @@
 
 def apply_validators(
     schema: core_schema.CoreSchema,
     validators: Iterable[Decorator[RootValidatorDecoratorInfo]]
     | Iterable[Decorator[ValidatorDecoratorInfo]]
     | Iterable[Decorator[FieldValidatorDecoratorInfo]],
 ) -> core_schema.CoreSchema:
-    """
-    Apply validators to a schema.
+    """Apply validators to a schema.
+
+    Args:
+        schema: The schema to apply validators on.
+        validators: An iterable of validators.
+
+    Returns:
+        The updated schema.
     """
     for validator in validators:
         info_arg = inspect_validator(validator.func, validator.info.mode)
         if not info_arg:
             val_type: Literal['no-info', 'general', 'field'] = 'no-info'
         elif isinstance(validator.info, (FieldValidatorDecoratorInfo, ValidatorDecoratorInfo)):
             val_type = 'field'
         else:
             val_type = 'general'
         schema = _VALIDATOR_F_MATCH[(validator.info.mode, val_type)](validator.func, schema)
     return schema
 
 
 def _validators_require_validate_default(validators: Iterable[Decorator[ValidatorDecoratorInfo]]) -> bool:
-    """
-    In v1, if any of the validators for a field had `always=True`, the default value would be validated.
+    """In v1, if any of the validators for a field had `always=True`, the default value would be validated.
 
     This serves as an auxiliary function for re-implementing that logic, by looping over a provided
     collection of (v1-style) ValidatorDecoratorInfo's and checking if any of them have `always=True`.
 
     We should be able to drop this function and the associated logic calling it once we drop support
     for v1-style validator decorators. (Or we can extend it and keep it if we add something equivalent
     to the v1-validator `always` kwarg to `field_validator`.)
@@ -1360,20 +1480,27 @@
 
 
 def apply_model_validators(
     schema: core_schema.CoreSchema,
     validators: Iterable[Decorator[ModelValidatorDecoratorInfo]],
     mode: Literal['inner', 'outer', 'all'],
 ) -> core_schema.CoreSchema:
-    """
-    Apply model validators to a schema.
+    """Apply model validators to a schema.
 
     If mode == 'inner', only "before" validators are applied
     If mode == 'outer', validators other than "before" are applied
     If mode == 'all', all validators are applied
+
+    Args:
+        schema: The schema to apply validators on.
+        validators: An iterable of validators.
+        mode: The validator mode.
+
+    Returns:
+        The updated schema.
     """
     ref: str | None = schema.pop('ref', None)  # type: ignore
     for validator in validators:
         if mode == 'inner' and validator.info.mode != 'before':
             continue
         if mode == 'outer' and validator.info.mode == 'before':
             continue
@@ -1395,60 +1522,46 @@
             else:
                 schema = core_schema.no_info_after_validator_function(function=validator.func, schema=schema)
     if ref:
         schema['ref'] = ref  # type: ignore
     return schema
 
 
-def apply_single_annotation(
-    schema: core_schema.CoreSchema, metadata: Any, definitions: dict[str, core_schema.CoreSchema]
-) -> core_schema.CoreSchema:
-    if isinstance(metadata, FieldInfo):
-        for field_metadata in metadata.metadata:
-            schema = apply_single_annotation(schema, field_metadata, definitions)
-        if metadata.discriminator is not None:
-            schema = _discriminated_union.apply_discriminator(schema, metadata.discriminator, definitions)
-        return schema
-
-    if schema['type'] == 'nullable':
-        # for nullable schemas, metadata is automatically applied to the inner schema
-        inner = schema.get('schema', core_schema.any_schema())
-        inner = apply_single_annotation(inner, metadata, definitions)
-        if inner:
-            schema['schema'] = inner
-        return schema
-
-    return _known_annotated_metadata.apply_known_metadata(metadata, schema.copy())
+def wrap_default(field_info: FieldInfo, schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
+    """Wrap schema with default schema if default value or `default_factory` are available.
 
+    Args:
+        field_info: The field info object.
+        schema: The schema to apply default on.
 
-def wrap_default(field_info: FieldInfo, schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
+    Returns:
+        Updated schema by default value or `default_factory`.
+    """
     if field_info.default_factory:
         return core_schema.with_default_schema(
             schema, default_factory=field_info.default_factory, validate_default=field_info.validate_default
         )
     elif field_info.default is not Undefined:
         return core_schema.with_default_schema(
             schema, default=field_info.default, validate_default=field_info.validate_default
         )
     else:
         return schema
 
 
 def get_first_arg(type_: Any) -> Any:
-    """
-    Get the first argument from a typing object, e.g. `List[int]` -> `int`, or `Any` if no argument.
-    """
+    """Get the first argument from a typing object, e.g. `List[int]` -> `int`, or `Any` if no argument."""
     try:
         return get_args(type_)[0]
     except IndexError:
         return Any
 
 
 def _extract_get_pydantic_json_schema(tp: Any, schema: CoreSchema) -> GetJsonSchemaFunction | None:
-    """Extract `__get_pydantic_json_schema__` from a type, handling the deprecated `__modify_schema__`"""
+    """Extract `__get_pydantic_json_schema__` from a type, handling the deprecated `__modify_schema__`."""
     js_modify_function = getattr(tp, '__get_pydantic_json_schema__', None)
 
     if hasattr(tp, '__modify_schema__'):
         raise PydanticUserError(
             'The `__modify_schema__` method is not supported in Pydantic v2. '
             'Use `__get_pydantic_json_schema__` instead.',
             code='custom-json-schema',
@@ -1457,18 +1570,14 @@
     # handle GenericAlias' but ignore Annotated which "lies" about it's origin (in this case it would be `int`)
     if hasattr(tp, '__origin__') and not isinstance(tp, type(Annotated[int, 'placeholder'])):
         return _extract_get_pydantic_json_schema(tp.__origin__, schema)
 
     if js_modify_function is None:
         return None
 
-    # wrap the schema so that we unpack ref schemas and always call metadata_js_function with the full schema
-    if schema['type'] != 'definition-ref':
-        # we would fail to unpack recursive ref schemas!
-        js_modify_function = wrap_json_schema_fn_for_model_or_custom_type_with_ref_unpacking(js_modify_function)
     return js_modify_function
 
 
 class _CommonField(TypedDict):
     schema: core_schema.CoreSchema
     validation_alias: str | list[str | int] | list[list[str | int]] | None
     serialization_alias: str | None
@@ -1490,7 +1599,55 @@
         'schema': schema,
         'validation_alias': validation_alias,
         'serialization_alias': serialization_alias,
         'serialization_exclude': serialization_exclude,
         'frozen': frozen,
         'metadata': metadata,
     }
+
+
+class _Definitions:
+    """Keeps track of references and definitions."""
+
+    def __init__(self) -> None:
+        self.seen: set[str] = set()
+        self.definitions: dict[str, core_schema.CoreSchema] = {}
+
+    @contextmanager
+    def get_schema_or_ref(self, tp: Any) -> Iterator[tuple[str, None] | tuple[str, CoreSchema]]:
+        """Get a definition for `tp` if one exists.
+
+        If a definition exists, a tuple of `(ref_string, CoreSchema)` is returned.
+        If no definition exists yet, a tuple of `(ref_string, None)` is returned.
+
+        Note that the returned `CoreSchema` will always be a `DefinitionReferenceSchema`,
+        not the actual definition itself.
+
+        This should be called for any type that can be identified by reference.
+        This includes any recursive types.
+
+        At present the following types can be named/recursive:
+
+        - BaseModel
+        - Dataclasses
+        - TypedDict
+        - TypeAliasType
+        """
+        ref = get_type_ref(tp)
+        # return the reference if we're either (1) in a cycle or (2) it was already defined
+        if ref in self.seen or ref in self.definitions:
+            yield (ref, core_schema.definition_reference_schema(ref))
+        else:
+            self.seen.add(ref)
+            try:
+                yield (ref, None)
+            finally:
+                self.seen.discard(ref)
+
+
+def resolve_original_schema(schema: CoreSchema, definitions: dict[str, CoreSchema]) -> CoreSchema | None:
+    if schema['type'] == 'definition-ref':
+        return definitions.get(schema['schema_ref'], None)
+    elif schema['type'] == 'definitions':
+        return schema['schema']
+    else:
+        return schema
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_generics.py` & `pydantic-2.0b3/pydantic/_internal/_generics.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,15 @@
     class LimitedDict(dict, MutableMapping[KT, VT]):  # type: ignore[type-arg]
         def __init__(self, size_limit: int = _LIMITED_DICT_SIZE):
             ...
 
 else:
 
     class LimitedDict(dict):
-        """
-        Limit the size/length of a dict used for caching to avoid unlimited increase in memory usage.
+        """Limit the size/length of a dict used for caching to avoid unlimited increase in memory usage.
 
         Since the dict is ordered, and we always remove elements from the beginning, this is effectively a FIFO cache.
         """
 
         def __init__(self, size_limit: int = _LIMITED_DICT_SIZE):
             self.size_limit = size_limit
             super().__init__()
@@ -77,16 +76,15 @@
 
     class DeepChainMap(ChainMap[KT, VT]):  # type: ignore
         ...
 
 else:
 
     class DeepChainMap(ChainMap):
-        """
-        Variant of ChainMap that allows direct updates to inner scopes
+        """Variant of ChainMap that allows direct updates to inner scopes.
 
         Taken from https://docs.python.org/3/library/collections.html#collections.ChainMap,
         with some light modifications for this use case.
         """
 
         def clear(self) -> None:
             for mapping in self.maps:
@@ -118,23 +116,28 @@
     args: tuple[Any, ...]  # analogous to typing._GenericAlias.__args__
     parameters: tuple[type[Any], ...]  # analogous to typing.Generic.__parameters__
 
 
 def create_generic_submodel(
     model_name: str, origin: type[BaseModel], args: tuple[Any, ...], params: tuple[Any, ...]
 ) -> type[BaseModel]:
-    """
-    Dynamically create a submodel of a provided (generic) BaseModel.
+    """Dynamically create a submodel of a provided (generic) BaseModel.
 
     This is used when producing concrete parametrizations of generic models. This function
     only *creates* the new subclass; the schema/validators/serialization must be updated to
     reflect a concrete parametrization elsewhere.
 
-    :param model_name: name of the newly created model
-    :param origin: base class for the new model to inherit from
+    Args:
+        model_name: The name of the newly created model.
+        origin: The base class for the new model to inherit from.
+        args: A tuple of generic metadata arguments.
+        params: A tuple of generic metadata parameters.
+
+    Returns:
+        The created submodel.
     """
     namespace: dict[str, Any] = {'__module__': origin.__module__}
     bases = (origin,)
     meta, ns, kwds = prepare_class(model_name, bases)
     namespace.update(ns)
     created_model = meta(
         model_name,
@@ -158,18 +161,24 @@
             object_by_reference = reference_module_globals.setdefault(reference_name, created_model)
             reference_name += '_'
 
     return created_model
 
 
 def _get_caller_frame_info(depth: int = 2) -> tuple[str | None, bool]:
-    """
-    Used inside a function to check whether it was called globally
+    """Used inside a function to check whether it was called globally.
+
+    Args:
+        depth: The depth to get the frame.
 
-    :returns Tuple[module_name, called_globally]
+    Returns:
+        A tuple contains `module_nam` and `called_globally`.
+
+    Raises:
+        RuntimeError: If the function is not called inside a function.
     """
     try:
         previous_caller_frame = sys._getframe(depth)
     except ValueError as e:
         raise RuntimeError('This function must be used inside another function') from e
     except AttributeError:  # sys module does not have _getframe function, so there's nothing we can do about it
         return None, False
@@ -177,16 +186,15 @@
     return frame_globals.get('__name__'), previous_caller_frame.f_locals is frame_globals
 
 
 DictValues: type[Any] = {}.values().__class__
 
 
 def iter_contained_typevars(v: Any) -> Iterator[TypeVarType]:
-    """
-    Recursively iterate through all subtypes and type args of `v` and yield any typevars that are found.
+    """Recursively iterate through all subtypes and type args of `v` and yield any typevars that are found.
 
     This is inspired as an alternative to directly accessing the `__parameters__` attribute of a GenericAlias,
     since __parameters__ of (nested) generic BaseModel subclasses won't show up in that list.
     """
     if isinstance(v, TypeVar):
         yield v
     elif is_basemodel(v):
@@ -211,32 +219,30 @@
     pydantic_generic_metadata: PydanticGenericMetadata | None = getattr(v, '__pydantic_generic_metadata__', None)
     if pydantic_generic_metadata:
         return pydantic_generic_metadata.get('origin')
     return typing_extensions.get_origin(v)
 
 
 def get_standard_typevars_map(cls: type[Any]) -> dict[TypeVarType, Any] | None:
-    """
-    Package a generic type's typevars and parametrization (if present) into a dictionary compatible with the
+    """Package a generic type's typevars and parametrization (if present) into a dictionary compatible with the
     `replace_types` function. Specifically, this works with standard typing generics and typing._GenericAlias.
     """
     origin = get_origin(cls)
     if origin is None:
         return None
 
     # In this case, we know that cls is a _GenericAlias, and origin is the generic type
     # So it is safe to access cls.__args__ and origin.__parameters__
     args: tuple[Any, ...] = cls.__args__  # type: ignore
     parameters: tuple[TypeVarType, ...] = origin.__parameters__  # type: ignore
     return dict(zip(parameters, args))
 
 
 def get_model_typevars_map(cls: type[BaseModel]) -> dict[TypeVarType, Any] | None:
-    """
-    Package a generic BaseModel's typevars and concrete parametrization (if present) into a dictionary compatible
+    """Package a generic BaseModel's typevars and concrete parametrization (if present) into a dictionary compatible
     with the `replace_types` function.
 
     Since BaseModel.__class_getitem__ does not produce a typing._GenericAlias, and the BaseModel generic info is
     stored in the __pydantic_generic_metadata__ attribute, we need special handling here.
     """
     # TODO: This could be unified with `get_standard_typevars_map` if we stored the generic metadata
     #   in the __origin__, __args__, and __parameters__ attributes of the model.
@@ -245,22 +251,27 @@
     args = generic_metadata['args']
     return dict(zip(iter_contained_typevars(origin), args))
 
 
 def replace_types(type_: Any, type_map: Mapping[Any, Any] | None) -> Any:
     """Return type with all occurrences of `type_map` keys recursively replaced with their values.
 
-    :param type_: Any type, class or generic alias
-    :param type_map: Mapping from `TypeVar` instance to concrete types.
-    :return: New type representing the basic structure of `type_` with all
-        `typevar_map` keys recursively replaced.
+    Args:
+        type_: The class or generic alias.
+        type_map: Mapping from `TypeVar` instance to concrete types.
 
-    >>> replace_types(Tuple[str, Union[List[str], float]], {str: int})
-    Tuple[int, Union[List[int], float]]
+    Returns:
+        A new type representing the basic structure of `type_` with all
+        `typevar_map` keys recursively replaced.
 
+    Example:
+        ```python
+        replace_types(Tuple[str, Union[List[str], float]], {str: int})
+        #> Tuple[int, Union[List[int], float]]
+        ```
     """
     if not type_map:
         return type_
 
     type_args = get_args(type_)
     origin_type = get_origin(type_)
 
@@ -318,30 +329,38 @@
 
     # If all else fails, we try to resolve the type directly and otherwise just
     # return the input with no modifications.
     return type_map.get(type_, type_)
 
 
 def check_parameters_count(cls: type[BaseModel], parameters: tuple[Any, ...]) -> None:
+    """Check the generic model parameters count is equal.
+
+    Args:
+        cls: The generic model.
+        parameters: A tuple of passed parameters to the generic model.
+
+    Raises:
+        TypeError: If the passed parameters count is not equal to generic model parameters count.
+    """
     actual = len(parameters)
     expected = len(cls.__pydantic_generic_metadata__['parameters'])
     if actual != expected:
         description = 'many' if actual > expected else 'few'
         raise TypeError(f'Too {description} parameters for {cls}; actual {actual}, expected {expected}')
 
 
 _generic_recursion_cache: ContextVar[set[str] | None] = ContextVar('_generic_recursion_cache', default=None)
 
 
 @contextmanager
 def generic_recursion_self_type(
     origin: type[BaseModel], args: tuple[Any, ...]
 ) -> Iterator[PydanticRecursiveRef | None]:
-    """
-    This contextmanager should be placed around the recursive calls used to build a generic type,
+    """This contextmanager should be placed around the recursive calls used to build a generic type,
     and accept as arguments the generic origin type and the type arguments being passed to it.
 
     If the same origin and arguments are observed twice, it implies that a self-reference placeholder
     can be used while building the core schema, and will produce a schema_ref that will be valid in the
     final parent schema.
     """
     previously_seen_type_refs = _generic_recursion_cache.get()
@@ -369,16 +388,15 @@
     if not visited:
         return set()  # not in a generic recursion, so there are no types
 
     return visited.copy()  # don't allow modifications
 
 
 def get_cached_generic_type_early(parent: type[BaseModel], typevar_values: Any) -> type[BaseModel] | None:
-    """
-    The use of a two-stage cache lookup approach was necessary to have the highest performance possible for
+    """The use of a two-stage cache lookup approach was necessary to have the highest performance possible for
     repeated calls to `__class_getitem__` on generic types (which may happen in tighter loops during runtime),
     while still ensuring that certain alternative parametrizations ultimately resolve to the same type.
 
     As a concrete example, this approach was necessary to make Model[List[T]][int] equal to Model[List[int]].
     The approach could be modified to not use two different cache keys at different points, but the
     _early_cache_key is optimized to be as quick to compute as possible (for repeated-access speed), and the
     _late_cache_key is optimized to be as "correct" as possible, so that two types that will ultimately be the
@@ -392,44 +410,40 @@
     """
     return _GENERIC_TYPES_CACHE.get(_early_cache_key(parent, typevar_values))
 
 
 def get_cached_generic_type_late(
     parent: type[BaseModel], typevar_values: Any, origin: type[BaseModel], args: tuple[Any, ...]
 ) -> type[BaseModel] | None:
-    """
-    See the docstring of `get_cached_generic_type_early` for more information about the two-stage cache lookup.
-    """
+    """See the docstring of `get_cached_generic_type_early` for more information about the two-stage cache lookup."""
     cached = _GENERIC_TYPES_CACHE.get(_late_cache_key(origin, args, typevar_values))
     if cached is not None:
         set_cached_generic_type(parent, typevar_values, cached, origin, args)
     return cached
 
 
 def set_cached_generic_type(
     parent: type[BaseModel],
     typevar_values: tuple[Any, ...],
     type_: type[BaseModel],
     origin: type[BaseModel] | None = None,
     args: tuple[Any, ...] | None = None,
 ) -> None:
-    """
-    See the docstring of `get_cached_generic_type_early` for more information about why items are cached with
+    """See the docstring of `get_cached_generic_type_early` for more information about why items are cached with
     two different keys.
     """
     _GENERIC_TYPES_CACHE[_early_cache_key(parent, typevar_values)] = type_
     if len(typevar_values) == 1:
         _GENERIC_TYPES_CACHE[_early_cache_key(parent, typevar_values[0])] = type_
     if origin and args:
         _GENERIC_TYPES_CACHE[_late_cache_key(origin, args, typevar_values)] = type_
 
 
 def _union_orderings_key(typevar_values: Any) -> Any:
-    """
-    This is intended to help differentiate between Union types with the same arguments in different order.
+    """This is intended to help differentiate between Union types with the same arguments in different order.
 
     Thanks to caching internal to the `typing` module, it is not possible to distinguish between
     List[Union[int, float]] and List[Union[float, int]] (and similarly for other "parent" origins besides List)
     because `typing` considers Union[int, float] to be equal to Union[float, int].
 
     However, you _can_ distinguish between (top-level) Union[int, float] vs. Union[float, int].
     Because we parse items as the first Union type that is successful, we get slightly more consistent behavior
@@ -445,29 +459,27 @@
     elif typing_extensions.get_origin(typevar_values) is typing.Union:
         return get_args(typevar_values)
     else:
         return ()
 
 
 def _early_cache_key(cls: type[BaseModel], typevar_values: Any) -> GenericTypesCacheKey:
-    """
-    This is intended for minimal computational overhead during lookups of cached types.
+    """This is intended for minimal computational overhead during lookups of cached types.
 
     Note that this is overly simplistic, and it's possible that two different cls/typevar_values
     inputs would ultimately result in the same type being created in BaseModel.__class_getitem__.
     To handle this, we have a fallback _late_cache_key that is checked later if the _early_cache_key
     lookup fails, and should result in a cache hit _precisely_ when the inputs to __class_getitem__
     would result in the same type.
     """
     return cls, typevar_values, _union_orderings_key(typevar_values)
 
 
 def _late_cache_key(origin: type[BaseModel], args: tuple[Any, ...], typevar_values: Any) -> GenericTypesCacheKey:
-    """
-    This is intended for use later in the process of creating a new type, when we have more information
+    """This is intended for use later in the process of creating a new type, when we have more information
     about the exact args that will be passed. If it turns out that a different set of inputs to
     __class_getitem__ resulted in the same inputs to the generic type creation process, we can still
     return the cached type, and update the cache with the _early_cache_key as well.
     """
     # The _union_orderings_key is placed at the start here to ensure there cannot be a collision with an
     # _early_cache_key, as that function will always produce a BaseModel subclass as the first item in the key,
     # whereas this function will always produce a tuple as the first item in the key.
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_known_annotated_metadata.py` & `pydantic-2.0b3/pydantic/_internal/_known_annotated_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,30 @@
 
 TEXT_SCHEMA_TYPES = ('str', 'bytes', 'url', 'multi-host-url')
 SEQUENCE_SCHEMA_TYPES = ('list', 'tuple', 'set', 'frozenset', 'generator', *TEXT_SCHEMA_TYPES)
 NUMERIC_SCHEMA_TYPES = ('float', 'int', 'date', 'time', 'timedelta', 'datetime')
 
 
 def expand_grouped_metadata(annotations: Iterable[Any]) -> Iterable[Any]:
+    """Expand the annotations.
+
+    Args:
+        annotations: An iterable of annotations.
+
+    Returns:
+        An iterable of expanded annotations.
+
+    Example:
+        ```python
+        from annotated_types import Ge, Len
+
+        print(list(expand_grouped_metadata([Ge(4), Len(5)])))
+        #> [Ge(ge=4), MinLen(min_length=5)]
+        ```
+    """
     from pydantic.fields import FieldInfo  # circular import
 
     for annotation in annotations:
         if isinstance(annotation, at.GroupedMetadata):
             yield from annotation
         elif isinstance(annotation, FieldInfo):
             yield from annotation.metadata
@@ -54,23 +70,32 @@
             annotation = copy(annotation)
             annotation.metadata = []
             yield annotation
         else:
             yield annotation
 
 
-def apply_known_metadata(annotation: Any, schema: CoreSchema) -> CoreSchema:  # noqa: C901
-    """
-    Apply `annotation` to `schema` if it is an annotation we know about (Gt, Le, etc.).
+def apply_known_metadata(annotation: Any, schema: CoreSchema) -> CoreSchema | None:  # noqa: C901
+    """Apply `annotation` to `schema` if it is an annotation we know about (Gt, Le, etc.).
     Otherwise return `None`.
 
     This does not handle all known annotations. If / when it does, it can always
     return a CoreSchema and return the unmodified schema if the annotation should be ignored.
 
     Assumes that GroupedMetadata has already been expanded via `expand_grouped_metadata`.
+
+    Args:
+        annotation: The annotation.
+        schema: The schema.
+
+    Returns:
+        An updated schema with annotation if it is an annotation we know about, `None` otherwise.
+
+    Raises:
+        PydanticCustomError: If `Predicate` fails.
     """
     schema = schema.copy()
     schema_update, _ = collect_known_metadata([annotation])
     if isinstance(annotation, at.Gt):
         if schema['type'] in NUMERIC_SCHEMA_TYPES:
             schema.update(schema_update)  # type: ignore
         else:
@@ -136,27 +161,37 @@
                     'predicate_failed',
                     f'Predicate {predicate_name}failed',  # type: ignore
                     {},
                 )
             return v
 
         return cs.no_info_after_validator_function(val_func, schema)
-
-    # for all other annotations just update the schema
-    # this includes things like `strict` which apply to pretty much every schema
-    schema.update(schema_update)  # type: ignore
+    elif schema_update:
+        # for all other annotations just update the schema
+        # this includes things like `strict` which apply to pretty much every schema
+        schema.update(schema_update)  # type: ignore
+    else:
+        return None
 
     return schema
 
 
 def collect_known_metadata(annotations: Iterable[Any]) -> tuple[dict[str, Any], list[Any]]:
-    """
-    Split `annotations` into known metadata and unknown annotations.
+    """Split `annotations` into known metadata and unknown annotations.
+
+    Args:
+        annotations: An iterable of annotations.
 
-    For example `[Gt(1), Len(42), Unknown()]` -> `({'gt': 1, 'min_length': 42}, [Unknown()])`.
+    Returns:
+        A tuple contains a dict of known metadata and a list of unknown annotations.
+
+    Example:
+        ```python
+        collect_known_metadata([Gt(1), Len(42), Unknown()])  # ({'gt': 1, 'min_length': 42}, [Unknown()])
+        ```
     """
     annotations = expand_grouped_metadata(annotations)
 
     res: dict[str, Any] = {}
     remaining: list[Any] = []
     for annotation in annotations:
         # Do we really want to consume any `BaseMetadata`?
@@ -176,16 +211,23 @@
     # it'd be nice to clean things up so we don't put in None (we probably don't _need_ to, it was just easier)
     # but this is simple enough to kick that can down the road
     res = {k: v for k, v in res.items() if v is not None}
     return res, remaining
 
 
 def check_metadata(metadata: dict[str, Any], allowed: Iterable[str], source_type: Any) -> None:
-    """
-    A small utility function to validate that the given metadata can be applied to the target.
+    """A small utility function to validate that the given metadata can be applied to the target.
     More than saving lines of code, this gives us a consistent error message for all of our internal implementations.
+
+    Args:
+        metadata: A dict of metadata.
+        allowed: An iterable of allowed metadata.
+        source_type: The source type.
+
+    Raises:
+        TypeError: If there is metadatas that can't be applied on source type.
     """
     unknown = metadata.keys() - set(allowed)
     if unknown:
         raise TypeError(
             f'The following constraints cannot be applied to {source_type!r}: {", ".join([f"{k!r}" for k in unknown])}'
         )
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_model_construction.py` & `pydantic-2.0b3/pydantic/_internal/_model_construction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-"""
-Private logic for creating models.
-"""
+"""Private logic for creating models."""
 from __future__ import annotations as _annotations
 
 import typing
 import warnings
 from abc import ABCMeta
 from functools import partial
 from types import FunctionType
 from typing import Any, Callable, Generic, Mapping
 
 from pydantic_core import SchemaSerializer, SchemaValidator
 from typing_extensions import dataclass_transform, deprecated
 
-from ..errors import PydanticErrorCodes, PydanticUndefinedAnnotation, PydanticUserError
+from ..errors import PydanticUndefinedAnnotation, PydanticUserError
 from ..fields import Field, FieldInfo, ModelPrivateAttr, PrivateAttr
 from ._config import ConfigWrapper
-from ._core_utils import flatten_schema_defs, inline_schema_defs
+from ._core_utils import collect_invalid_schemas, flatten_schema_defs, inline_schema_defs
 from ._decorators import ComputedFieldInfo, DecoratorInfos, PydanticDescriptorProxy
-from ._fields import Undefined, collect_model_fields
+from ._fields import Undefined, collect_model_fields, is_valid_field_name, is_valid_privateattr_name
 from ._generate_schema import GenerateSchema
 from ._generics import PydanticGenericMetadata, get_model_typevars_map
+from ._mock_validator import set_basemodel_mock_validator
 from ._schema_generation_shared import CallbackGetCoreSchemaHandler
 from ._typing_extra import get_cls_types_namespace, is_classvar, parent_frame_namespace
 from ._utils import ClassAttribute, is_valid_identifier
 
 if typing.TYPE_CHECKING:
     from inspect import Signature
 
@@ -39,20 +38,16 @@
     PydanticDescriptorProxy,
     ComputedFieldInfo,
 )
 object_setattr = object.__setattr__
 
 
 class _ModelNamespaceDict(dict):  # type: ignore[type-arg]
-    """
-    A dictionary subclass that intercepts attribute setting on model classes and warns about overriding of decorators.
-
-    Args:
-        k (str): The key to be set.
-        v (object): The value to set with the key.
+    """A dictionary subclass that intercepts attribute setting on model classes and
+    warns about overriding of decorators.
     """
 
     def __setitem__(self, k: str, v: object) -> None:
         existing: Any = self.get(k, None)
         if existing and v is not existing and isinstance(existing, PydanticDescriptorProxy):
             warnings.warn(f'`{k}` overrides an existing Pydantic `{existing.decorator_info.decorator_repr}` decorator')
 
@@ -69,23 +64,23 @@
         __pydantic_generic_metadata__: PydanticGenericMetadata | None = None,
         __pydantic_reset_parent_namespace__: bool = True,
         **kwargs: Any,
     ) -> type:
         """Metaclass for creating Pydantic models.
 
         Args:
-            cls_name (str): the name of the class to be created
-            bases (tuple[type[Any], ...]]): the base classes of the class to be created
-            namespace (dict[str, Any]): the attribute dictionary of the class to be created
-            __pydantic_generic_metadata__ (PydanticGenericMetadata | None): metadata for generic models
-            __pydantic_reset_parent_namespace__ (bool): reset parent namespace
-            **kwargs (Any): catch-all for any other keyword arguments
+            cls_name: The name of the class to be created.
+            bases: The base classes of the class to be created.
+            namespace: The attribute dictionary of the class to be created.
+            __pydantic_generic_metadata__: Metadata for generic models.
+            __pydantic_reset_parent_namespace__: Reset parent namespace.
+            **kwargs: Catch-all for any other keyword arguments.
 
         Returns:
-            type: the new class created by the metaclass
+            The new class created by the metaclass.
         """
         # Note `ModelMetaclass` refers to `BaseModel`, but is also used to *create* `BaseModel`, so we rely on the fact
         # that `BaseModel` itself won't have any bases, but any subclass of it will, to determine whether the `__new__`
         # call we're in the middle of is for the `BaseModel` class.
         if bases:
             base_field_names, class_vars, base_private_attributes = mcs._collect_bases_data(bases)
 
@@ -96,16 +91,16 @@
             )
             if private_attributes:
                 if 'model_post_init' in namespace:
                     # if there are private_attributes and a model_post_init function, we handle both
                     original_model_post_init = namespace['model_post_init']
 
                     def wrapped_model_post_init(self: BaseModel, __context: Any) -> None:
-                        """
-                        We need to both initialize private attributes and call the user-defined model_post_init method
+                        """We need to both initialize private attributes and call the user-defined model_post_init
+                        method.
                         """
                         init_private_attributes(self, __context)
                         original_model_post_init(self, __context)
 
                     namespace['model_post_init'] = wrapped_model_post_init
                 else:
                     namespace['model_post_init'] = init_private_attributes
@@ -186,29 +181,26 @@
             super(cls, cls).__pydantic_init_subclass__(**kwargs)  # type: ignore[misc]
             return cls
         else:
             # this is the BaseModel class itself being created, no logic required
             return super().__new__(mcs, cls_name, bases, namespace, **kwargs)
 
     def __getattr__(self, item: str) -> Any:
-        """
-        This is necessary to keep attribute access working for class attribute access
-        """
+        """This is necessary to keep attribute access working for class attribute access."""
         private_attributes = self.__dict__.get('__private_attributes__')
         if private_attributes and item in private_attributes:
             return private_attributes[item]
         raise AttributeError(item)
 
     @classmethod
     def __prepare__(cls, *args: Any, **kwargs: Any) -> Mapping[str, object]:
         return _ModelNamespaceDict()
 
     def __instancecheck__(self, instance: Any) -> bool:
-        """
-        Avoid calling ABC _abc_subclasscheck unless we're pretty sure.
+        """Avoid calling ABC _abc_subclasscheck unless we're pretty sure.
 
         See #3829 and python/cpython#92810
         """
         return hasattr(instance, '__pydantic_validator__') and super().__instancecheck__(instance)
 
     @staticmethod
     def _collect_bases_data(bases: tuple[type[Any], ...]) -> tuple[set[str], set[str], dict[str, ModelPrivateAttr]]:
@@ -229,18 +221,21 @@
     @deprecated('The `__fields__` attribute is deprecated, use `model_fields` instead.')
     def __fields__(self) -> dict[str, FieldInfo]:
         warnings.warn('The `__fields__` attribute is deprecated, use `model_fields` instead.', DeprecationWarning)
         return self.model_fields
 
 
 def init_private_attributes(self: BaseModel, __context: Any) -> None:
-    """
-    This function is meant to behave like a BaseModel method to initialise private attributes.
+    """This function is meant to behave like a BaseModel method to initialise private attributes.
 
     It takes context as an argument since that's what pydantic-core passes when calling it.
+
+    Args:
+        self: The BaseModel instance.
+        __context: The context.
     """
     pydantic_private = {}
     for name, private_attr in self.__private_attributes__.items():
         default = private_attr.get_default()
         if default is not Undefined:
             pydantic_private[name] = default
     object_setattr(self, '__pydantic_private__', pydantic_private)
@@ -248,18 +243,33 @@
 
 def inspect_namespace(  # noqa C901
     namespace: dict[str, Any],
     ignored_types: tuple[type[Any], ...],
     base_class_vars: set[str],
     base_class_fields: set[str],
 ) -> dict[str, ModelPrivateAttr]:
-    """
-    iterate over the namespace and:
+    """Iterate over the namespace and:
     * gather private attributes
-    * check for items which look like fields but are not (e.g. have no annotation) and warn
+    * check for items which look like fields but are not (e.g. have no annotation) and warn.
+
+    Args:
+        namespace: The attribute dictionary of the class to be created.
+        ignored_types: A tuple of ignore types.
+        base_class_vars: A set of base class class variables.
+        base_class_fields: A set of base class fields.
+
+    Returns:
+        A dict contains private attributes info.
+
+    Raises:
+        TypeError: If there is a `__root__` field in model.
+        NameError: If private attribute name is invalid.
+        PydanticUserError:
+            - If a field does not have a type annotation.
+            - If a field on base class was overridden by a non-annotated attribute.
     """
     all_ignored_types = ignored_types + IGNORED_TYPES
 
     private_attributes: dict[str, ModelPrivateAttr] = {}
     raw_annotations = namespace.get('__annotations__', {})
 
     if '__root__' in raw_annotations or '__root__' in namespace:
@@ -281,25 +291,25 @@
             continue
         elif isinstance(value, ModelPrivateAttr):
             if var_name.startswith('__'):
                 raise NameError(
                     f'Private attributes "{var_name}" must not have dunder names; '
                     'use a single underscore prefix instead.'
                 )
-            elif not single_underscore(var_name):
+            elif is_valid_field_name(var_name):
                 raise NameError(
                     f'Private attributes "{var_name}" must not be a valid field name; '
                     f'use sunder names, e.g. "_{var_name}"'
                 )
             private_attributes[var_name] = value
             del namespace[var_name]
         elif var_name.startswith('__'):
             continue
-        elif var_name.startswith('_'):
-            if var_name in raw_annotations and not is_classvar(raw_annotations[var_name]):
+        elif is_valid_privateattr_name(var_name):
+            if var_name not in raw_annotations or not is_classvar(raw_annotations[var_name]):
                 private_attributes[var_name] = PrivateAttr(default=value)
                 del namespace[var_name]
         elif var_name in base_class_vars:
             continue
         elif var_name not in raw_annotations:
             if var_name in base_class_fields:
                 raise PydanticUserError(
@@ -317,35 +327,36 @@
                     f"type annotation; if `{var_name}` is not meant to be a field, you may be able to resolve this "
                     f"error by annotating it as a `ClassVar` or updating `model_config['ignored_types']`.",
                     code='model-field-missing-annotation',
                 )
 
     for ann_name, ann_type in raw_annotations.items():
         if (
-            single_underscore(ann_name)
+            is_valid_privateattr_name(ann_name)
             and ann_name not in private_attributes
             and ann_name not in ignored_names
             and not is_classvar(ann_type)
             and ann_type not in all_ignored_types
             and getattr(ann_type, '__module__', None) != 'functools'
         ):
             private_attributes[ann_name] = PrivateAttr()
 
     return private_attributes
 
 
-def single_underscore(name: str) -> bool:
-    return name.startswith('_') and not name.startswith('__')
-
-
 def set_model_fields(
     cls: type[BaseModel], bases: tuple[type[Any], ...], config_wrapper: ConfigWrapper, types_namespace: dict[str, Any]
 ) -> None:
-    """
-    Collect and set `cls.model_fields` and `cls.__class_vars__`.
+    """Collect and set `cls.model_fields` and `cls.__class_vars__`.
+
+    Args:
+        cls: BaseModel or dataclass.
+        bases: Parents of the class, generally `cls.__bases__`.
+        config_wrapper: The config wrapper instance.
+        types_namespace: Optional extra namespace to look for types in.
     """
     typevars_map = get_model_typevars_map(cls)
     fields, class_vars = collect_model_fields(cls, bases, config_wrapper, types_namespace, typevars_map=typevars_map)
 
     cls.model_fields = fields
     cls.__class_vars__.update(class_vars)
 
@@ -354,59 +365,64 @@
     cls: type[BaseModel],
     cls_name: str,
     config_wrapper: ConfigWrapper,
     *,
     raise_errors: bool = True,
     types_namespace: dict[str, Any] | None,
 ) -> bool:
-    """
-    Finish building a model class.
-
-    Returns `True` if the model is successfully completed, else `False`.
+    """Finish building a model class.
 
     This logic must be called after class has been created since validation functions must be bound
     and `get_type_hints` requires a class object.
+
+    Args:
+        cls: BaseModel or dataclass.
+        cls_name: The model or dataclass name.
+        config_wrapper: The config wrapper instance.
+        raise_errors: Whether to raise errors.
+        types_namespace: Optional extra namespace to look for types in.
+
+    Returns:
+        `True` if the model is successfully completed, else `False`.
+
+    Raises:
+        PydanticUndefinedAnnotation: If `PydanticUndefinedAnnotation` occurs in`__get_pydantic_core_schema__`
+            and `raise_errors=True`.
     """
     typevars_map = get_model_typevars_map(cls)
     gen_schema = GenerateSchema(
         config_wrapper,
         types_namespace,
         typevars_map,
     )
+
     handler = CallbackGetCoreSchemaHandler(
         partial(gen_schema.generate_schema, from_dunder_get_core_schema=False),
-        gen_schema.generate_schema,
+        gen_schema,
+        ref_mode='unpack',
     )
+
     try:
         schema = cls.__get_pydantic_core_schema__(cls, handler)
     except PydanticUndefinedAnnotation as e:
         if raise_errors:
             raise
-        undefined_type_error_message = (
-            f'`{cls_name}` is not fully defined; you should define `{e.name}`, then call `{cls_name}.model_rebuild()` '
-            f'before the first `{cls_name}` instance is created.'
-        )
-
-        def attempt_rebuild() -> SchemaValidator | None:
-            if cls.model_rebuild(raise_errors=False, _parent_namespace_depth=5):
-                return cls.__pydantic_validator__
-            else:
-                return None
-
-        cls.__pydantic_validator__ = MockValidator(  # type: ignore[assignment]
-            undefined_type_error_message, code='class-not-fully-defined', attempt_rebuild=attempt_rebuild
-        )
+        set_basemodel_mock_validator(cls, cls_name, f'`{e.name}`')
         return False
 
     core_config = config_wrapper.core_config(cls)
 
+    schema = gen_schema.collect_definitions(schema)
+    schema = flatten_schema_defs(schema)
+    if collect_invalid_schemas(schema):
+        set_basemodel_mock_validator(cls, cls_name, 'all referenced types')
+        return False
+
     # debug(schema)
     cls.__pydantic_core_schema__ = schema
-
-    schema = flatten_schema_defs(schema)
     simplified_core_schema = inline_schema_defs(schema)
     cls.__pydantic_validator__ = SchemaValidator(simplified_core_schema, core_config)
     cls.__pydantic_serializer__ = SchemaSerializer(simplified_core_schema, core_config)
     cls.__pydantic_complete__ = True
 
     # set __signature__ attr only for model class, but not for its instances
     cls.__signature__ = ClassAttribute(
@@ -414,16 +430,23 @@
     )
     return True
 
 
 def generate_model_signature(
     init: Callable[..., None], fields: dict[str, FieldInfo], config_wrapper: ConfigWrapper
 ) -> Signature:
-    """
-    Generate signature for model based on its fields
+    """Generate signature for model based on its fields.
+
+    Args:
+        init: The class init.
+        fields: The model fields.
+        config_wrapper: The config wrapper instance.
+
+    Returns:
+        The model signature.
     """
     from inspect import Parameter, Signature, signature
     from itertools import islice
 
     present_params = signature(init).parameters.values()
     merged_params: dict[str, Parameter] = {}
     var_kw = None
@@ -484,51 +507,27 @@
         while var_kw_name in fields:
             var_kw_name += '_'
         merged_params[var_kw_name] = var_kw.replace(name=var_kw_name)
 
     return Signature(parameters=list(merged_params.values()), return_annotation=None)
 
 
-class MockValidator:
-    """
-    Mocker for `pydantic_core.SchemaValidator` which just raises an error when one of its methods is accessed.
-    """
-
-    __slots__ = '_error_message', '_code', '_attempt_rebuild'
+def model_extra_private_getattr(self: BaseModel, item: str) -> Any:
+    """This function is used to retrieve unrecognized attribute values from BaseModel subclasses which
+    allow (and store) extra and/or private attributes.
 
-    def __init__(
-        self,
-        error_message: str,
-        *,
-        code: PydanticErrorCodes,
-        attempt_rebuild: Callable[[], SchemaValidator | None] | None = None,
-    ) -> None:
-        """
-        Attempt rebuild
-        """
-        self._error_message = error_message
-        self._code: PydanticErrorCodes = code
-        self._attempt_rebuild = attempt_rebuild
-
-    def __getattr__(self, item: str) -> None:
-        __tracebackhide__ = True
-        if self._attempt_rebuild:
-            validator = self._attempt_rebuild()
-            if validator is not None:
-                return getattr(validator, item)
-
-        # raise an AttributeError if `item` doesn't exist
-        getattr(SchemaValidator, item)
-        raise PydanticUserError(self._error_message, code=self._code)
+    Args:
+        self: The BaseModel instance.
+        item: The extra private attribute name.
 
+    Returns:
+        The extra private attribute value.
 
-def model_extra_private_getattr(self: BaseModel, item: str) -> Any:
-    """
-    This function is used to retrieve unrecognized attribute values from BaseModel subclasses which
-    allow (and store) extra and/or private attributes
+    Raises:
+        AttributeError: If the attribute does not exist in the model.
     """
     if item in self.__private_attributes__:
         attribute = self.__private_attributes__[item]
         if hasattr(attribute, '__get__'):
             return attribute.__get__(self, type(self))  # type: ignore
 
         try:
@@ -541,15 +540,25 @@
             return self.__pydantic_extra__[item]
         except KeyError as exc:
             raise AttributeError(f'{type(self).__name__!r} object has no attribute {item!r}') from exc
     else:
         raise AttributeError(f'{type(self).__name__!r} object has no attribute {item!r}')
 
 
-def model_private_delattr(self: BaseModel, item: str) -> Any:
+def model_private_delattr(self: BaseModel, item: str) -> None:
+    """This function is used to delete unrecognized attribute values from BaseModel subclasses which
+    allow (and store) extra and/or private attributes.
+
+    Args:
+        self: The BaseModel instance.
+        item: The extra private attribute name.
+
+    Raises:
+        AttributeError: If the attribute does not exist in the model.
+    """
     if item in self.__private_attributes__:
         attribute = self.__private_attributes__[item]
         if hasattr(attribute, '__delete__'):
             attribute.__delete__(self)  # type: ignore
             return
 
         try:
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_repr.py` & `pydantic-2.0b3/pydantic/_internal/_repr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Tools to provide pretty/human-readable display of objects.
-"""
+"""Tools to provide pretty/human-readable display of objects."""
 from __future__ import annotations as _annotations
 
 import types
 import typing
 from typing import Any
 
 import typing_extensions
@@ -15,16 +13,15 @@
     ReprArgs: typing_extensions.TypeAlias = 'typing.Iterable[tuple[str | None, Any]]'
     RichReprResult: typing_extensions.TypeAlias = (
         'typing.Iterable[Any | tuple[Any] | tuple[str, Any] | tuple[str, Any, Any]]'
     )
 
 
 class PlainRepr(str):
-    """
-    String class where repr doesn't include quotes. Useful with Representation when you want to return a string
+    """String class where repr doesn't include quotes. Useful with Representation when you want to return a string
     representation of something that is valid (or pseudo-valid) python.
     """
 
     def __repr__(self) -> str:
         return str(self)
 
 
@@ -34,71 +31,63 @@
     # `__rich_repr__` is used by [rich](https://rich.readthedocs.io/en/stable/pretty.html).
     # (this is not a docstring to avoid adding a docstring to classes which inherit from Representation)
 
     # we don't want to use a type annotation here as it can break get_type_hints
     __slots__ = tuple()  # type: typing.Collection[str]
 
     def __repr_args__(self) -> ReprArgs:
-        """
-        Returns the attributes to show in __str__, __repr__, and __pretty__ this is generally overridden.
+        """Returns the attributes to show in __str__, __repr__, and __pretty__ this is generally overridden.
 
         Can either return:
         * name - value pairs, e.g.: `[('foo_name', 'foo'), ('bar_name', ['b', 'a', 'r'])]`
         * or, just values, e.g.: `[(None, 'foo'), (None, ['b', 'a', 'r'])]`
         """
         attrs_names = self.__slots__
         if not attrs_names and hasattr(self, '__dict__'):
             attrs_names = self.__dict__.keys()
         attrs = ((s, getattr(self, s)) for s in attrs_names)
         return [(a, v) for a, v in attrs if v is not None]
 
     def __repr_name__(self) -> str:
-        """
-        Name of the instance's class, used in __repr__.
-        """
+        """Name of the instance's class, used in __repr__."""
         return self.__class__.__name__
 
     def __repr_str__(self, join_str: str) -> str:
         return join_str.join(repr(v) if a is None else f'{a}={v!r}' for a, v in self.__repr_args__())
 
     def __pretty__(self, fmt: typing.Callable[[Any], Any], **kwargs: Any) -> typing.Generator[Any, None, None]:
-        """
-        Used by devtools (https://python-devtools.helpmanual.io/) to pretty print objects.
-        """
+        """Used by devtools (https://python-devtools.helpmanual.io/) to pretty print objects."""
         yield self.__repr_name__() + '('
         yield 1
         for name, value in self.__repr_args__():
             if name is not None:
                 yield name + '='
             yield fmt(value)
             yield ','
             yield 0
         yield -1
         yield ')'
 
     def __rich_repr__(self) -> RichReprResult:
-        """
-        Used by Rich (https://rich.readthedocs.io/en/stable/pretty.html) to pretty print objects.
-        """
+        """Used by Rich (https://rich.readthedocs.io/en/stable/pretty.html) to pretty print objects."""
         for name, field_repr in self.__repr_args__():
             if name is None:
                 yield field_repr
             else:
                 yield name, field_repr
 
     def __str__(self) -> str:
         return self.__repr_str__(' ')
 
     def __repr__(self) -> str:
         return f'{self.__repr_name__()}({self.__repr_str__(", ")})'
 
 
 def display_as_type(obj: Any) -> str:
-    """
-    Pretty representation of a type, should be as close as possible to the original type definition string.
+    """Pretty representation of a type, should be as close as possible to the original type definition string.
 
     Takes some logic from `typing._type_repr`.
     """
     if isinstance(obj, types.FunctionType):
         return obj.__name__
     elif obj is ...:
         return '...'
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_std_types_schema.py` & `pydantic-2.0b3/pydantic/_internal/_std_types_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Logic for generating pydantic-core schemas for standard library types.
+"""Logic for generating pydantic-core schemas for standard library types.
 
 Import of this module is deferred since it contains imports of many standard library modules.
 """
 from __future__ import annotations as _annotations
 
 import collections
 import collections.abc
@@ -51,60 +50,46 @@
     def __get_pydantic_core_schema__(self, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
         return self.get_core_schema(source_type, handler)
 
     def __get_pydantic_json_schema__(self, schema: CoreSchema, handler: GetJsonSchemaHandler) -> JsonSchemaValue:
         return self.get_json_schema(schema, handler)
 
 
-def enum_prepare_pydantic_annotations(
-    source_type: Any, annotations: Iterable[Any], _config: ConfigDict
-) -> tuple[Any, list[Any]] | None:
-    if not (inspect.isclass(source_type) and issubclass(source_type, Enum)):
-        return None
-
-    enum_type = source_type
-
+def get_enum_core_schema(enum_type: type[Enum]) -> CoreSchema:
     cases: list[Any] = list(enum_type.__members__.values())
 
     if not cases:
         # Use an isinstance check for enums with no cases.
         # This won't work with serialization or JSON schema, but that's okay -- the most important
         # use case for this is creating typevar bounds for generics that should be restricted to enums.
         # This is more consistent than it might seem at first, since you can only subclass enum.Enum
         # (or subclasses of enum.Enum) if all parent classes have no cases.
-        schema = core_schema.is_instance_schema(enum_type)
-        return enum_type, [
-            SchemaTransformer(
-                lambda _1, _2: schema,
-                lambda _1, handler: handler(schema),
-            ),
-            *annotations,
-        ]
+        return core_schema.is_instance_schema(enum_type)
 
     if len(cases) == 1:
         expected = repr(cases[0].value)
     else:
         expected = ','.join([repr(case.value) for case in cases[:-1]]) + f' or {cases[-1].value!r}'
 
     def to_enum(__input_value: Any) -> Enum:
         try:
-            return enum_type(__input_value)
+            return enum_type(__input_value)  # type: ignore
         except ValueError:
             # The type: ignore on the next line is to ignore the requirement of LiteralString
             raise PydanticCustomError('enum', f'Input should be {expected}', {'expected': expected})  # type: ignore
 
     enum_ref = get_type_ref(enum_type)
     description = None if not enum_type.__doc__ else inspect.cleandoc(enum_type.__doc__)
     if description == 'An enumeration.':  # This is the default value provided by enum.EnumMeta.__new__; don't use it
         description = None
     updates = {'title': enum_type.__name__, 'description': description}
     updates = {k: v for k, v in updates.items() if v is not None}
 
     def get_json_schema(_, handler: GetJsonSchemaHandler) -> JsonSchemaValue:
-        json_schema = handler(core_schema.literal_schema([x.value for x in cases]))
+        json_schema = handler(core_schema.literal_schema([x.value for x in cases], ref=enum_ref))
         original_schema = handler.resolve_ref_schema(json_schema)
         update_json_schema(original_schema, updates)
         return json_schema
 
     to_enum_validator = core_schema.no_info_plain_validator_function(to_enum)
     if issubclass(enum_type, int):
         # this handles `IntEnum`, and also `Foobar(int, Enum)`
@@ -131,25 +116,18 @@
             python_schema=core_schema.is_instance_schema(enum_type),
         )
     else:
         lax = to_enum_validator
         strict = core_schema.json_or_python_schema(
             json_schema=to_enum_validator, python_schema=core_schema.is_instance_schema(enum_type)
         )
-    outer_schema = core_schema.lax_or_strict_schema(
-        lax_schema=lax,
-        strict_schema=strict,
-        ref=enum_ref,
+    return core_schema.lax_or_strict_schema(
+        lax_schema=lax, strict_schema=strict, ref=enum_ref, metadata={'pydantic_js_functions': [get_json_schema]}
     )
 
-    return enum_type, [
-        SchemaTransformer(lambda _1, _2: outer_schema, lambda _, handler: get_json_schema(_, handler)),
-        *annotations,
-    ]
-
 
 @slots_dataclass
 class DecimalValidator:
     gt: int | decimal.Decimal | None = None
     ge: int | decimal.Decimal | None = None
     lt: int | decimal.Decimal | None = None
     le: int | decimal.Decimal | None = None
@@ -321,15 +299,15 @@
         metadata, {*_known_annotated_metadata.FLOAT_CONSTRAINTS, 'max_digits', 'decimal_places'}, decimal.Decimal
     )
     return source, [DecimalValidator(**metadata), *remaining_annotations]
 
 
 @slots_dataclass
 class InnerSchemaValidator:
-    """Use a fixed CoreSchema, avoiding interference from outward annotations"""
+    """Use a fixed CoreSchema, avoiding interference from outward annotations."""
 
     core_schema: CoreSchema
     js_schema: JsonSchemaValue | None = None
     js_core_schema: CoreSchema | None = None
     js_schema_update: JsonSchemaValue | None = None
 
     def __get_pydantic_json_schema__(self, _schema: CoreSchema, handler: GetJsonSchemaHandler) -> JsonSchemaValue:
@@ -909,11 +887,10 @@
 PREPARE_METHODS: tuple[Callable[[Any, Iterable[Any], ConfigDict], tuple[Any, list[Any]] | None], ...] = (
     decimal_prepare_pydantic_annotations,
     sequence_like_prepare_pydantic_annotations,
     datetime_prepare_pydantic_annotations,
     uuid_prepare_pydantic_annotations,
     path_schema_prepare_pydantic_annotations,
     mapping_like_prepare_pydantic_annotations,
-    enum_prepare_pydantic_annotations,
     ip_prepare_pydantic_annotations,
     url_prepare_pydantic_annotations,
 )
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_typing_extra.py` & `pydantic-2.0b3/pydantic/_internal/_typing_extra.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Logic for interacting with type annotations, mostly extensions, shims and hacks to wrap python's typing module.
-"""
+"""Logic for interacting with type annotations, mostly extensions, shims and hacks to wrap python's typing module."""
 from __future__ import annotations as _annotations
 
 import dataclasses
 import sys
 import types
 import typing
 from collections.abc import Callable
@@ -83,18 +81,17 @@
 
 
 def literal_values(type_: type[Any]) -> tuple[Any, ...]:
     return get_args(type_)
 
 
 def all_literal_values(type_: type[Any]) -> list[Any]:
-    """
-    This method is used to retrieve all Literal values as
+    """This method is used to retrieve all Literal values as
     Literal can be used recursively (see https://www.python.org/dev/peps/pep-0586)
-    e.g. `Literal[Literal[Literal[1, 2, 3], "foo"], 5, None]`
+    e.g. `Literal[Literal[Literal[1, 2, 3], "foo"], 5, None]`.
     """
     if not is_literal_type(type_):
         return [type_]
 
     values = literal_values(type_)
     return list(x for value in values for x in all_literal_values(value))
 
@@ -103,29 +100,27 @@
     from ._utils import lenient_issubclass
 
     origin = get_origin(ann_type)
     return origin is not None and lenient_issubclass(origin, Annotated)
 
 
 def is_namedtuple(type_: type[Any]) -> bool:
-    """
-    Check if a given class is a named tuple.
-    It can be either a `typing.NamedTuple` or `collections.namedtuple`
+    """Check if a given class is a named tuple.
+    It can be either a `typing.NamedTuple` or `collections.namedtuple`.
     """
     from ._utils import lenient_issubclass
 
     return lenient_issubclass(type_, tuple) and hasattr(type_, '_fields')
 
 
 test_new_type = typing.NewType('test_new_type', str)
 
 
 def is_new_type(type_: type[Any]) -> bool:
-    """
-    Check whether type_ was created using typing.NewType.
+    """Check whether type_ was created using typing.NewType.
 
     Can't use isinstance because it fails <3.10.
     """
     return isinstance(type_, test_new_type.__class__) and hasattr(type_, '__supertype__')  # type: ignore[arg-type]
 
 
 def _check_classvar(v: type[Any] | None) -> bool:
@@ -144,30 +139,27 @@
     if ann_type.__class__ == typing.ForwardRef and ann_type.__forward_arg__.startswith('ClassVar['):  # type: ignore
         return True
 
     return False
 
 
 def _check_finalvar(v: type[Any] | None) -> bool:
-    """
-    Check if a given type is a `typing.Final` type.
-    """
+    """Check if a given type is a `typing.Final` type."""
     if v is None:
         return False
 
     return v.__class__ == Final.__class__ and (sys.version_info < (3, 8) or getattr(v, '_name', None) == 'Final')
 
 
 def is_finalvar(ann_type: Any) -> bool:
     return _check_finalvar(ann_type) or _check_finalvar(get_origin(ann_type))
 
 
 def parent_frame_namespace(*, parent_depth: int = 2) -> dict[str, Any] | None:
-    """
-    We allow use of items in parent namespace to get around the issue with `get_type_hints` only looking in the
+    """We allow use of items in parent namespace to get around the issue with `get_type_hints` only looking in the
     global module namespace. See https://github.com/pydantic/pydantic/issues/2678#issuecomment-1008139014 -> Scope
     and suggestion at the end of the next comment by @gvanrossum.
 
     WARNING 1: it matters exactly where this is called. By default, this function will build a namespace from the
     parent of where it is called.
 
     WARNING 2: this only looks in the parent namespace, not other parents since (AFAIK) there's no way to collect a
@@ -203,51 +195,46 @@
 def get_cls_types_namespace(cls: type[Any], parent_namespace: dict[str, Any] | None = None) -> dict[str, Any]:
     ns = add_module_globals(cls, parent_namespace)
     ns[cls.__name__] = cls
     return ns
 
 
 def get_cls_type_hints_lenient(obj: Any, globalns: dict[str, Any] | None = None) -> dict[str, Any]:
-    """
-    Collect annotations from a class, including those from parent classes.
+    """Collect annotations from a class, including those from parent classes.
 
     Unlike `typing.get_type_hints`, this function will not error if a forward reference is not resolvable.
     """
     hints = {}
     for base in reversed(obj.__mro__):
         ann = base.__dict__.get('__annotations__')
         localns = dict(vars(base))
         if ann is not None and ann is not GetSetDescriptorType:
             for name, value in ann.items():
                 hints[name] = eval_type_lenient(value, globalns, localns)
     return hints
 
 
 def eval_type_lenient(value: Any, globalns: dict[str, Any] | None, localns: dict[str, Any] | None) -> Any:
-    """
-    Behaves like typing._eval_type, except it won't raise an error if a forward reference can't be resolved.
-    """
+    """Behaves like typing._eval_type, except it won't raise an error if a forward reference can't be resolved."""
     if value is None:
         value = NoneType
     elif isinstance(value, str):
         value = _make_forward_ref(value, is_argument=False, is_class=True)
 
     try:
         return typing._eval_type(value, globalns, localns)  # type: ignore
     except NameError:
         # the point of this function is to be tolerant to this case
         return value
 
 
 def get_function_type_hints(function: Callable[..., Any], *, include_keys: set[str] | None = None) -> dict[str, Any]:
-    """
-    Like `typing.get_type_hints`, but doesn't convert `X` to `Optional[X]` if the default value is `None`, also
+    """Like `typing.get_type_hints`, but doesn't convert `X` to `Optional[X]` if the default value is `None`, also
     copes with `partial`.
     """
-
     if isinstance(function, partial):
         annotations = function.func.__annotations__
     else:
         annotations = function.__annotations__
 
     globalns = add_module_globals(function)
     type_hints = {}
@@ -268,29 +255,22 @@
 
     def _make_forward_ref(
         arg: Any,
         is_argument: bool = True,
         *,
         is_class: bool = False,
     ) -> typing.ForwardRef:
-        """
-        Wrapper for ForwardRef that accounts for the `is_class` argument missing in older versions.
+        """Wrapper for ForwardRef that accounts for the `is_class` argument missing in older versions.
         The `module` argument is omitted as it breaks <3.9 and isn't used in the calls below.
 
         See https://github.com/python/cpython/pull/28560 for some background
 
         Implemented as EAFP with memory.
         """
-        global _make_forward_ref
-        try:
-            res = typing.ForwardRef(arg, is_argument, is_class=is_class)  # type: ignore
-            _make_forward_ref = typing.ForwardRef  # type: ignore
-            return res
-        except TypeError:
-            return typing.ForwardRef(arg, is_argument)
+        return typing.ForwardRef(arg, is_argument)
 
 else:
     _make_forward_ref = typing.ForwardRef
 
 
 if sys.version_info >= (3, 10):
     get_type_hints = typing.get_type_hints
@@ -304,19 +284,18 @@
     @typing.no_type_check
     def get_type_hints(  # noqa: C901
         obj: Any,
         globalns: dict[str, Any] | None = None,
         localns: dict[str, Any] | None = None,
         include_extras: bool = False,
     ) -> dict[str, Any]:  # pragma: no cover
-        """
-        Taken verbatim from python 3.10.8 unchanged, except:
+        """Taken verbatim from python 3.10.8 unchanged, except:
         * type annotations of the function definition above.
         * prefixing `typing.` where appropriate
-        * Use `_make_forward_ref` instead of `typing.ForwardRef` to handle the `is_class` argument
+        * Use `_make_forward_ref` instead of `typing.ForwardRef` to handle the `is_class` argument.
 
         https://github.com/python/cpython/blob/aaaf5174241496afca7ce4d4584570190ff972fe/Lib/typing.py#L1773-L1875
 
         DO NOT CHANGE THIS METHOD UNLESS ABSOLUTELY NECESSARY.
         ======================================================
 
         Return type hints for an object.
@@ -346,15 +325,14 @@
 
         - If one dict argument is passed, it is used for both globals and
           locals.
 
         - If two dict arguments are passed, they specify globals and
           locals, respectively.
         """
-
         if getattr(obj, '__no_type_check__', None):
             return {}
         # Classes require a special treatment.
         if isinstance(obj, type):
             hints = {}
             for base in reversed(obj.__mro__):
                 if globalns is None:
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_utils.py` & `pydantic-2.0b3/pydantic/_internal/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Bucket of reusable internal utilities.
+"""Bucket of reusable internal utilities.
 
 This should be reduced as much as possible with functions only used in one place, moved to that place.
 """
 from __future__ import annotations as _annotations
 
 import keyword
 import typing
@@ -77,30 +76,28 @@
     except TypeError:
         if isinstance(cls, _typing_extra.WithArgsTypes):
             return False
         raise  # pragma: no cover
 
 
 def is_basemodel(cls: Any) -> TypeGuard[type[BaseModel]]:
-    """
-    We can remove this function and go back to using lenient_issubclass, but this is nice because it
+    """We can remove this function and go back to using lenient_issubclass, but this is nice because it
     ensures that we get proper type-checking, which lenient_issubclass doesn't provide.
 
     Would be nice if there was a lenient_issubclass-equivalent in typing_extensions, or otherwise
     a way to define such a function that would support proper type-checking; maybe we should bring it up
     at the typing summit..
     """
     from ..main import BaseModel
 
     return lenient_issubclass(cls, BaseModel)
 
 
 def is_valid_identifier(identifier: str) -> bool:
-    """
-    Checks that a string is a valid identifier and not a Python keyword.
+    """Checks that a string is a valid identifier and not a Python keyword.
     :param identifier: The identifier to test.
     :return: True if the identifier is valid.
     """
     return identifier.isidentifier() and not keyword.iskeyword(identifier)
 
 
 KeyType = TypeVar('KeyType')
@@ -118,32 +115,29 @@
 
 
 def update_not_none(mapping: dict[Any, Any], **update: Any) -> None:
     mapping.update({k: v for k, v in update.items() if v is not None})
 
 
 def almost_equal_floats(value_1: float, value_2: float, *, delta: float = 1e-8) -> bool:
-    """
-    Return True if two floats are almost equal
-    """
+    """Return True if two floats are almost equal."""
     return abs(value_1 - value_2) <= delta
 
 
 T = TypeVar('T')
 
 
 def unique_list(
     input_list: list[T] | tuple[T, ...],
     *,
     name_factory: typing.Callable[[T], str] = str,
 ) -> list[T]:
-    """
-    Make a list unique while maintaining order.
+    """Make a list unique while maintaining order.
     We update the list if another one with the same name is set
-    (e.g. root validator overridden in subclass)
+    (e.g. root validator overridden in subclass).
     """
     result: list[T] = []
     result_names: list[str] = []
     for v in input_list:
         v_name = name_factory(v)
         if v_name not in result_names:
             result_names.append(v_name)
@@ -151,64 +145,56 @@
         else:
             result[result_names.index(v_name)] = v
 
     return result
 
 
 class ValueItems(_repr.Representation):
-    """
-    Class for more convenient calculation of excluded or included fields on values.
-    """
+    """Class for more convenient calculation of excluded or included fields on values."""
 
     __slots__ = ('_items', '_type')
 
     def __init__(self, value: Any, items: AbstractSetIntStr | MappingIntStrAny) -> None:
         items = self._coerce_items(items)
 
         if isinstance(value, (list, tuple)):
             items = self._normalize_indexes(items, len(value))  # type: ignore
 
         self._items: MappingIntStrAny = items  # type: ignore
 
     def is_excluded(self, item: Any) -> bool:
-        """
-        Check if item is fully excluded.
+        """Check if item is fully excluded.
 
         :param item: key or index of a value
         """
         return self.is_true(self._items.get(item))
 
     def is_included(self, item: Any) -> bool:
-        """
-        Check if value is contained in self._items
+        """Check if value is contained in self._items.
 
         :param item: key or index of value
         """
         return item in self._items
 
     def for_element(self, e: int | str) -> AbstractSetIntStr | MappingIntStrAny | None:
-        """
-        :param e: key or index of element on value
+        """:param e: key or index of element on value
         :return: raw values for element if self._items is dict and contain needed element
         """
-
         item = self._items.get(e)  # type: ignore
         return item if not self.is_true(item) else None
 
     def _normalize_indexes(self, items: MappingIntStrAny, v_length: int) -> dict[int | str, Any]:
-        """
-        :param items: dict or set of indexes which will be normalized
+        """:param items: dict or set of indexes which will be normalized
         :param v_length: length of sequence indexes of which will be
 
         >>> self._normalize_indexes({0: True, -2: True, -1: True}, 4)
         {0: True, 2: True, 3: True}
         >>> self._normalize_indexes({'__all__': True}, 4)
         {0: True, 1: True, 2: True, 3: True}
         """
-
         normalized_items: dict[int | str, Any] = {}
         all_items = None
         for i, v in items.items():
             if not (isinstance(v, typing.Mapping) or isinstance(v, typing.AbstractSet) or self.is_true(v)):
                 raise TypeError(f'Unexpected type of exclude value for index "{i}" {v.__class__}')
             if i == '__all__':
                 all_items = self._coerce_value(v)
@@ -231,16 +217,15 @@
             normalized_item = normalized_items.setdefault(i, {})
             if not self.is_true(normalized_item):
                 normalized_items[i] = self.merge(all_items, normalized_item)
         return normalized_items
 
     @classmethod
     def merge(cls, base: Any, override: Any, intersect: bool = False) -> Any:
-        """
-        Merge a `base` item with an `override` item.
+        """Merge a `base` item with an `override` item.
 
         Both `base` and `override` are converted to dictionaries if possible.
         Sets are converted to dictionaries with the sets entries as keys and
         Ellipsis as values.
 
         Each key-value pair existing in `base` is merged with `override`,
         while the rest of the key-value pairs are updated recursively with this function.
@@ -301,17 +286,15 @@
 
     def ClassAttribute(name: str, value: T) -> T:
         ...
 
 else:
 
     class ClassAttribute:
-        """
-        Hide class attribute from its instances
-        """
+        """Hide class attribute from its instances."""
 
         __slots__ = 'name', 'value'
 
         def __init__(self, name: str, value: Any) -> None:
             self.name = name
             self.value = value
 
@@ -321,20 +304,18 @@
             raise AttributeError(f'{self.name!r} attribute of {owner.__name__!r} is class-only')
 
 
 Obj = TypeVar('Obj')
 
 
 def smart_deepcopy(obj: Obj) -> Obj:
-    """
-    Return type as is for immutable built-in types
+    """Return type as is for immutable built-in types
     Use obj.copy() for built-in empty collections
-    Use copy.deepcopy() for non-empty collections and unknown objects
+    Use copy.deepcopy() for non-empty collections and unknown objects.
     """
-
     obj_type = obj.__class__
     if obj_type in IMMUTABLE_NON_COLLECTIONS_TYPES:
         return obj  # fastest case: obj is immutable and not collection therefore will not be copied anyway
     try:
         if not obj and obj_type in BUILTIN_COLLECTIONS:
             # faster way for empty collections, no need to copy its members
             return obj if obj_type is tuple else obj.copy()  # type: ignore  # tuple doesn't have copy method
@@ -345,16 +326,15 @@
     return deepcopy(obj)  # slowest way when we actually might need a deepcopy
 
 
 _EMPTY = object()
 
 
 def all_identical(left: typing.Iterable[Any], right: typing.Iterable[Any]) -> bool:
-    """
-    Check that the items of `left` are the same objects as those in `right`.
+    """Check that the items of `left` are the same objects as those in `right`.
 
     >>> a, b = object(), object()
     >>> all_identical([a, b, a], [a, b, a])
     True
     >>> all_identical([a, b, [a]], [a, b, [a]])  # new list object, while "equal" is not "identical"
     False
     """
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_validate_call.py` & `pydantic-2.0b3/pydantic/_internal/_validate_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 @dataclass
 class CallMarker:
     function: Callable[..., Any]
     validate_return: bool
 
 
 class ValidateCallWrapper:
-    """
-    This is a wrapper around a function that validates the arguments passed to it, and optionally the return value.
+    """This is a wrapper around a function that validates the arguments passed to it, and optionally the return value.
 
     It's partially inspired by `wraps` which in turn uses `partial`, but extended to be a descriptor so
     these functions can be applied to instance methods, class methods, static methods, as well as normal functions.
     """
 
     __slots__ = (
         'raw_function',
@@ -68,15 +67,13 @@
         simplified_schema = inline_schema_defs(schema)
         self.__pydantic_validator__ = pydantic_core.SchemaValidator(simplified_schema, core_config)
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return self.__pydantic_validator__.validate_python(pydantic_core.ArgsKwargs(args, kwargs))
 
     def __get__(self, obj: Any, objtype: type[Any] | None = None) -> ValidateCallWrapper:
-        """
-        Bind the raw function and return another ValidateCallWrapper wrapping that.
-        """
+        """Bind the raw function and return another ValidateCallWrapper wrapping that."""
         bound_function = self.raw_function.__get__(obj, objtype)
         return self.__class__(bound_function, self._config, self._validate_return)
 
     def __repr__(self) -> str:
         return f'ValidateCallWrapper({self.raw_function})'
```

### Comparing `pydantic-2.0b2/pydantic/_internal/_validators.py` & `pydantic-2.0b3/pydantic/_internal/_validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Validator functions for standard library types.
+"""Validator functions for standard library types.
 
 Import of this module is deferred since it contains imports of many standard library modules.
 """
 
 from __future__ import annotations as _annotations
 
 import re
@@ -15,17 +14,15 @@
 from pydantic_core._pydantic_core import PydanticKnownError
 
 
 def sequence_validator(
     __input_value: typing.Sequence[Any],
     validator: core_schema.ValidatorFunctionWrapHandler,
 ) -> typing.Sequence[Any]:
-    """
-    Validator for `Sequence` types, isinstance(v, Sequence) has already been called.
-    """
+    """Validator for `Sequence` types, isinstance(v, Sequence) has already been called."""
     value_type = type(__input_value)
 
     # We don't accept any plain string as a sequence
     # Relevant issue: https://github.com/pydantic/pydantic/issues/5595
     if issubclass(value_type, (str, bytes)):
         raise PydanticCustomError(
             'sequence_str',
@@ -54,17 +51,16 @@
             raise PydanticCustomError('import_error', 'Invalid python path: {error}', {'error': str(e)})
     else:
         # otherwise we just return the value and let the next validator do the rest of the work
         return value
 
 
 def _import_string_logic(dotted_path: str) -> Any:
-    """
-    Inspired by uvicorn — dotted paths should include a colon before the final item if that item is not a module.
-    (This is necessary to distinguish between a submodule and an attribute when there is a conflict.)
+    """Inspired by uvicorn — dotted paths should include a colon before the final item if that item is not a module.
+    (This is necessary to distinguish between a submodule and an attribute when there is a conflict.).
 
     If the dotted path does not include a colon and the final item is not a valid module, importing as an attribute
     rather than a submodule will be attempted automatically.
 
     So, for example, the following values of `dotted_path` result in the following returned values:
     * 'collections': <module 'collections'>
     * 'collections.abc': <module 'collections.abc'>
@@ -174,32 +170,30 @@
     try:
         return IPv6Address(__input_value)
     except ValueError:
         raise PydanticCustomError('ip_v6_address', 'Input is not a valid IPv6 address')
 
 
 def ip_v4_network_validator(__input_value: Any) -> IPv4Network:
-    """
-    Assume IPv4Network initialised with a default `strict` argument
+    """Assume IPv4Network initialised with a default `strict` argument.
 
     See more:
     https://docs.python.org/library/ipaddress.html#ipaddress.IPv4Network
     """
     if isinstance(__input_value, IPv4Network):
         return __input_value
 
     try:
         return IPv4Network(__input_value)
     except ValueError:
         raise PydanticCustomError('ip_v4_network', 'Input is not a valid IPv4 network')
 
 
 def ip_v6_network_validator(__input_value: Any) -> IPv6Network:
-    """
-    Assume IPv6Network initialised with a default `strict` argument
+    """Assume IPv6Network initialised with a default `strict` argument.
 
     See more:
     https://docs.python.org/library/ipaddress.html#ipaddress.IPv6Network
     """
     if isinstance(__input_value, IPv6Network):
         return __input_value
```

### Comparing `pydantic-2.0b2/pydantic/deprecated/class_validators.py` & `pydantic-2.0b3/pydantic/deprecated/class_validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Old `@validator` and `@root_validator` function validators from V1.
-"""
+"""Old `@validator` and `@root_validator` function validators from V1."""
 
 from __future__ import annotations as _annotations
 
 from functools import partial, partialmethod
 from types import FunctionType
 from typing import TYPE_CHECKING, Any, Callable, TypeVar, Union, overload
 from warnings import warn
@@ -81,16 +79,15 @@
     *fields: str,
     pre: bool = False,
     each_item: bool = False,
     always: bool = False,
     check_fields: bool | None = None,
     allow_reuse: bool = False,
 ) -> Callable[[_V1ValidatorType], _V1ValidatorType]:
-    """
-    Decorate methods on the class indicating that they should be used to validate fields.
+    """Decorate methods on the class indicating that they should be used to validate fields.
 
     Args:
         __field (str): The first field the validator should be called on; this is separate
             from `fields` to ensure an error is raised if you don't pass at least one.
         *fields (str): Additional field(s) the validator should be called on.
         pre (bool, optional): Whether or not this validator should be called before the standard
             validators (else after). Defaults to False.
@@ -184,25 +181,24 @@
     skip_on_failure: Literal[True],
     allow_reuse: bool = ...,
 ) -> Callable[[_V1RootValidatorFunctionType], _V1RootValidatorFunctionType,]:
     ...
 
 
 def root_validator(
-    *,
+    *__args,
     pre: bool = False,
     skip_on_failure: bool = False,
     allow_reuse: bool = False,
 ) -> Any:
-    """
-    Decorate methods on a model indicating that they should be used to validate (and perhaps
+    """Decorate methods on a model indicating that they should be used to validate (and perhaps
     modify) data either before or after standard model parsing/validation is performed.
 
     Args:
-        pre (bool, optional): Whether or not this validator should be called before the standard
+        pre (bool, optional): Whether this validator should be called before the standard
             validators (else after). Defaults to False.
         skip_on_failure (bool, optional): Whether to stop validation and return as soon as a
             failure is encountered. Defaults to False.
         allow_reuse (bool, optional): Whether to track and raise an error if another validator
             refers to the decorated function. Defaults to False.
 
     Returns:
@@ -211,20 +207,26 @@
     warn(
         'Pydantic V1 style `@root_validator` validators are deprecated.'
         ' You should migrate to Pydantic V2 style `@model_validator` validators,'
         ' see the migration guide for more details',
         DeprecationWarning,
         stacklevel=2,
     )
+
+    if __args:
+        # Ensure a nice error is raised if someone attempts to use the bare decorator
+        return root_validator()(*__args)  # type: ignore
+
     if allow_reuse is True:  # pragma: no cover
         warn(_ALLOW_REUSE_WARNING_MESSAGE, DeprecationWarning)
     mode: Literal['before', 'after'] = 'before' if pre is True else 'after'
     if pre is False and skip_on_failure is not True:
         raise PydanticUserError(
-            'If you use `@root_validator` with pre=False (the default) you MUST specify `skip_on_failure=True`.',
+            'If you use `@root_validator` with pre=False (the default) you MUST specify `skip_on_failure=True`.'
+            ' Note that `@root_validator` is deprecated and should be replaced with `@model_validator`.',
             code='root-validator-pre-skip',
         )
 
     wrap = partial(_decorators_v1.make_v1_generic_root_validator, pre=pre)
 
     def dec(f: Callable[..., Any] | classmethod[Any, Any, Any] | staticmethod[Any, Any]) -> Any:
         if _decorators.is_instance_method_from_sig(f):
```

### Comparing `pydantic-2.0b2/pydantic/deprecated/copy_internals.py` & `pydantic-2.0b3/pydantic/deprecated/copy_internals.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/deprecated/decorator.py` & `pydantic-2.0b3/pydantic/deprecated/decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,15 @@
 @overload
 @deprecated('The `validate_arguments` method is deprecated; use `validate_call` instead.')
 def validate_arguments(func: 'AnyCallableT') -> 'AnyCallableT':
     ...
 
 
 def validate_arguments(func: Optional['AnyCallableT'] = None, *, config: 'ConfigType' = None) -> Any:
-    """
-    Decorator to validate the arguments passed to a function.
-    """
+    """Decorator to validate the arguments passed to a function."""
     warnings.warn(
         'The `validate_arguments` method is deprecated; use `validate_call` instead.', DeprecationWarning, stacklevel=2
     )
 
     def validate(_func: 'AnyCallable') -> 'AnyCallable':
         vd = ValidatedFunction(_func, config)
```

### Comparing `pydantic-2.0b2/pydantic/deprecated/json.py` & `pydantic-2.0b3/pydantic/deprecated/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 
 
 def isoformat(o: Union[datetime.date, datetime.time]) -> str:
     return o.isoformat()
 
 
 def decimal_encoder(dec_value: Decimal) -> Union[int, float]:
-    """
-    Encodes a Decimal as int of there's no exponent, otherwise float
+    """Encodes a Decimal as int of there's no exponent, otherwise float.
 
     This is useful when we use ConstrainedDecimal to represent Numeric(x,0)
     where a integer (but not int typed) is used. Encoding this as a float
     results in failed round-tripping between encode and parse.
     Our Id type is a prime example of this.
 
     >>> decimal_encoder(Decimal("1.0"))
@@ -112,14 +111,12 @@
         return encoder(obj)
     else:  # We have exited the for loop without finding a suitable encoder
         return pydantic_encoder(obj)
 
 
 @deprecated('timedelta_isoformat is deprecated.')
 def timedelta_isoformat(td: datetime.timedelta) -> str:
-    """
-    ISO 8601 encoding for Python timedelta object.
-    """
+    """ISO 8601 encoding for Python timedelta object."""
     warnings.warn('timedelta_isoformat is deprecated.', DeprecationWarning, stacklevel=2)
     minutes, seconds = divmod(td.seconds, 60)
     hours, minutes = divmod(minutes, 60)
     return f'{"-" if td.days < 0 else ""}P{abs(td.days)}DT{hours:d}H{minutes:d}M{seconds:d}.{td.microseconds:06d}S'
```

### Comparing `pydantic-2.0b2/pydantic/deprecated/parse.py` & `pydantic-2.0b3/pydantic/deprecated/parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/deprecated/tools.py` & `pydantic-2.0b3/pydantic/deprecated/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     type_: Any,
     *,
     title: NameFactory | None = None,
     by_alias: bool = True,
     ref_template: str = DEFAULT_REF_TEMPLATE,
     schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
 ) -> dict[str, Any]:
-    """Generate a JSON schema (as dict) for the passed model or dynamically generated one"""
+    """Generate a JSON schema (as dict) for the passed model or dynamically generated one."""
     warnings.warn(
         'schema_of is deprecated. Use pydantic.TypeAdapter.json_schema instead.', DeprecationWarning, stacklevel=2
     )
     res = TypeAdapter(type_).json_schema(
         by_alias=by_alias,
         schema_generator=schema_generator,
         ref_template=ref_template,
@@ -70,15 +70,15 @@
     *,
     title: NameFactory | None = None,
     by_alias: bool = True,
     ref_template: str = DEFAULT_REF_TEMPLATE,
     schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
     **dumps_kwargs: Any,
 ) -> str:
-    """Generate a JSON schema (as JSON) for the passed model or dynamically generated one"""
+    """Generate a JSON schema (as JSON) for the passed model or dynamically generated one."""
     warnings.warn(
         'schema_json_of is deprecated. Use pydantic.TypeAdapter.json_schema instead.', DeprecationWarning, stacklevel=2
     )
     return json.dumps(
         schema_of(type_, title=title, by_alias=by_alias, ref_template=ref_template, schema_generator=schema_generator),
         **dumps_kwargs,
     )
```

### Comparing `pydantic-2.0b2/pydantic/v1/__init__.py` & `pydantic-2.0b3/pydantic/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/_hypothesis_plugin.py` & `pydantic-2.0b3/pydantic/v1/_hypothesis_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 #
 # URLs are unsupported because it's easy for users to define their own strategy for
 # "normal" URLs, and hard for us to define a general strategy which includes "weird"
 # URLs but doesn't also have unpredictable performance problems.
 #
 # conlist() and conset() are unsupported for now, because the workarounds for
 # Cython and Hypothesis to handle parametrized generic types are incompatible.
-# Once Cython can support 'normal' generics we'll revisit this.
+# We are rethinking Hypothesis compatibility in Pydantic v2.
 
 # Emails
 try:
     import email_validator
 except ImportError:  # pragma: no cover
     pass
 else:
@@ -164,14 +164,19 @@
 # We hook into the con***() functions and the ConstrainedNumberMeta metaclass,
 # so here we only have to register subclasses for other constrained types which
 # don't go via those mechanisms.  Then there are the registration hooks below.
 st.register_type_strategy(pydantic.StrictBool, st.booleans())
 st.register_type_strategy(pydantic.StrictStr, st.text())
 
 
+# FutureDate, PastDate
+st.register_type_strategy(pydantic.FutureDate, st.dates(min_value=datetime.date.today() + datetime.timedelta(days=1)))
+st.register_type_strategy(pydantic.PastDate, st.dates(max_value=datetime.date.today() - datetime.timedelta(days=1)))
+
+
 # Constrained-type resolver functions
 #
 # For these ones, we actually want to inspect the type in order to work out a
 # satisfying strategy.  First up, the machinery for tracking resolver functions:
 
 RESOLVERS: Dict[type, Callable[[type], st.SearchStrategy]] = {}  # type: ignore[type-arg]
```

### Comparing `pydantic-2.0b2/pydantic/v1/annotated_types.py` & `pydantic-2.0b3/pydantic/v1/annotated_types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/class_validators.py` & `pydantic-2.0b3/pydantic/v1/class_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/color.py` & `pydantic-2.0b3/pydantic/v1/color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/config.py` & `pydantic-2.0b3/pydantic/v1/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 class Extra(str, Enum):
     allow = 'allow'
     ignore = 'ignore'
     forbid = 'forbid'
 
 
 # https://github.com/cython/cython/issues/4003
-# Will be fixed with Cython 3 but still in alpha right now
+# Fixed in Cython 3 and Pydantic v1 won't support Cython 3.
+# Pydantic v2 doesn't depend on Cython at all.
 if not compiled:
     from typing_extensions import TypedDict
 
     class ConfigDict(TypedDict, total=False):
         title: Optional[str]
         anystr_lower: bool
         anystr_strip_whitespace: bool
```

### Comparing `pydantic-2.0b2/pydantic/v1/dataclasses.py` & `pydantic-2.0b3/pydantic/v1/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/datetime_parse.py` & `pydantic-2.0b3/pydantic/v1/datetime_parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/decorator.py` & `pydantic-2.0b3/pydantic/v1/decorator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/env_settings.py` & `pydantic-2.0b3/pydantic/v1/env_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/error_wrappers.py` & `pydantic-2.0b3/pydantic/v1/error_wrappers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/errors.py` & `pydantic-2.0b3/pydantic/v1/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/fields.py` & `pydantic-2.0b3/pydantic/v1/fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/generics.py` & `pydantic-2.0b3/pydantic/v1/generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/json.py` & `pydantic-2.0b3/pydantic/v1/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/main.py` & `pydantic-2.0b3/pydantic/v1/main.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/mypy.py` & `pydantic-2.0b3/pydantic/v1/mypy.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,23 +489,40 @@
         fields_set_argument = Argument(Var('_fields_set', optional_set_str), optional_set_str, None, ARG_OPT)
         construct_arguments = self.get_field_arguments(fields, typed=True, force_all_optional=False, use_alias=False)
         construct_arguments = [fields_set_argument] + construct_arguments
 
         obj_type = ctx.api.named_type(f'{BUILTINS_NAME}.object')
         self_tvar_name = '_PydanticBaseModel'  # Make sure it does not conflict with other names in the class
         tvar_fullname = ctx.cls.fullname + '.' + self_tvar_name
-        tvd = TypeVarDef(self_tvar_name, tvar_fullname, -1, [], obj_type)
-        self_tvar_expr = TypeVarExpr(self_tvar_name, tvar_fullname, [], obj_type)
+        if MYPY_VERSION_TUPLE >= (1, 4):
+            tvd = TypeVarType(
+                self_tvar_name,
+                tvar_fullname,
+                -1,
+                [],
+                obj_type,
+                AnyType(TypeOfAny.from_omitted_generics),  # type: ignore[arg-type]
+            )
+            self_tvar_expr = TypeVarExpr(
+                self_tvar_name,
+                tvar_fullname,
+                [],
+                obj_type,
+                AnyType(TypeOfAny.from_omitted_generics),  # type: ignore[arg-type]
+            )
+        else:
+            tvd = TypeVarDef(self_tvar_name, tvar_fullname, -1, [], obj_type)
+            self_tvar_expr = TypeVarExpr(self_tvar_name, tvar_fullname, [], obj_type)
         ctx.cls.info.names[self_tvar_name] = SymbolTableNode(MDEF, self_tvar_expr)
 
         # Backward-compatible with TypeVarDef from Mypy 0.910.
         if isinstance(tvd, TypeVarType):
             self_type = tvd
         else:
-            self_type = TypeVarType(tvd)  # type: ignore[call-arg]
+            self_type = TypeVarType(tvd)
 
         add_method(
             ctx,
             'construct',
             construct_arguments,
             return_type=self_type,
             self_type=self_type,
```

### Comparing `pydantic-2.0b2/pydantic/v1/networks.py` & `pydantic-2.0b3/pydantic/v1/networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/parse.py` & `pydantic-2.0b3/pydantic/v1/parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/schema.py` & `pydantic-2.0b3/pydantic/v1/schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/tools.py` & `pydantic-2.0b3/pydantic/v1/tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/types.py` & `pydantic-2.0b3/pydantic/v1/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 import math
 import re
 import warnings
 from datetime import date
-from decimal import Decimal
+from decimal import Decimal, InvalidOperation
 from enum import Enum
 from pathlib import Path
 from types import new_class
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
@@ -687,15 +687,19 @@
         yield decimal_validator
         yield number_size_validator
         yield number_multiple_validator
         yield cls.validate
 
     @classmethod
     def validate(cls, value: Decimal) -> Decimal:
-        digit_tuple, exponent = value.as_tuple()[1:]
+        try:
+            normalized_value = value.normalize()
+        except InvalidOperation:
+            normalized_value = value
+        digit_tuple, exponent = normalized_value.as_tuple()[1:]
         if exponent in {'F', 'n', 'N'}:
             raise errors.DecimalIsNotFiniteError()
 
         if exponent >= 0:
             # A positive exponent adds that many trailing zeros.
             digits = len(digit_tuple) + exponent
             decimals = 0
```

### Comparing `pydantic-2.0b2/pydantic/v1/typing.py` & `pydantic-2.0b3/pydantic/v1/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,23 +248,15 @@
 
     def is_union(tp: Optional[Type[Any]]) -> bool:
         return tp is Union or tp is types.UnionType  # noqa: E721
 
     WithArgsTypes = (typing._GenericAlias, types.GenericAlias, types.UnionType)
 
 
-if sys.version_info < (3, 9):
-    StrPath = Union[str, PathLike]
-else:
-    StrPath = Union[str, PathLike]
-    # TODO: Once we switch to Cython 3 to handle generics properly
-    #  (https://github.com/cython/cython/issues/2753), use following lines instead
-    #  of the one above
-    # # os.PathLike only becomes subscriptable from Python 3.9 onwards
-    # StrPath = Union[str, PathLike[str]]
+StrPath = Union[str, PathLike]
 
 
 if TYPE_CHECKING:
     from .fields import ModelField
 
     TupleGenerator = Generator[Tuple[str, Any], None, None]
     DictStrAny = Dict[str, Any]
```

### Comparing `pydantic-2.0b2/pydantic/v1/utils.py` & `pydantic-2.0b3/pydantic/v1/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/validators.py` & `pydantic-2.0b3/pydantic/v1/validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pydantic/v1/version.py` & `pydantic-2.0b3/pydantic/v1/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __all__ = 'compiled', 'VERSION', 'version_info'
 
-VERSION = '1.10.8'
+VERSION = '1.10.9'
 
 try:
     import cython  # type: ignore
 except ImportError:
     compiled: bool = False
 else:  # pragma: no cover
     try:
```

### Comparing `pydantic-2.0b2/tests/conftest.py` & `pydantic-2.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_abc.py` & `pydantic-2.0b3/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_aliases.py` & `pydantic-2.0b3/tests/test_aliases.py`

 * *Files 8% similar despite different names*

```diff
@@ -234,14 +234,63 @@
     assert [f.validation_alias for f in Parent.model_fields.values()] == ['w_val_alias', 'x_val_alias', None]
     assert [f.serialization_alias for f in Parent.model_fields.values()] == ['w_ser_alias', 'x_ser_alias', None]
     assert [f.alias for f in Child.model_fields.values()] == ['w_', 'X', 'Y', 'Z']
     assert [f.validation_alias for f in Child.model_fields.values()] == ['w_val_alias', 'X', 'Y', 'Z']
     assert [f.serialization_alias for f in Child.model_fields.values()] == ['w_ser_alias', 'X', 'Y', 'Z']
 
 
+@pytest.mark.parametrize(
+    'cls_params, field_params, validation_key, serialization_key',
+    [
+        pytest.param(
+            {},
+            {'alias': 'x1', 'validation_alias': 'x2'},
+            'x2',
+            'x1',
+            id='alias-validation_alias',
+        ),
+        pytest.param(
+            {'alias_generator': str.upper},
+            {'alias': 'x'},
+            'x',
+            'x',
+            id='alias_generator-alias',
+        ),
+        pytest.param(
+            {'alias_generator': str.upper},
+            {'alias': 'x1', 'validation_alias': 'x2'},
+            'x2',
+            'x1',
+            id='alias_generator-alias-validation_alias',
+        ),
+        pytest.param(
+            {'alias_generator': str.upper},
+            {'alias': 'x1', 'serialization_alias': 'x2'},
+            'x1',
+            'x2',
+            id='alias_generator-alias-serialization_alias',
+        ),
+        pytest.param(
+            {'alias_generator': str.upper},
+            {'alias': 'x1', 'validation_alias': 'x2', 'serialization_alias': 'x3'},
+            'x2',
+            'x3',
+            id='alias_generator-alias-validation_alias-serialization_alias',
+        ),
+    ],
+)
+def test_aliases_priority(cls_params, field_params, validation_key, serialization_key):
+    class Model(BaseModel, **cls_params):
+        x: int = Field(**field_params)
+
+    model = Model(**{validation_key: 1})
+    assert model.x == 1
+    assert model.model_dump(by_alias=True).get(serialization_key, None) is not None
+
+
 def test_empty_string_alias():
     class Model(BaseModel):
         empty_string_key: int = Field(alias='')
 
     data = {'': 123}
     m = Model(**data)
     assert m.empty_string_key == 123
```

### Comparing `pydantic-2.0b2/tests/test_annotated.py` & `pydantic-2.0b3/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_assert_in_validators.py` & `pydantic-2.0b3/tests/test_assert_in_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_callable.py` & `pydantic-2.0b3/tests/test_callable.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_color.py` & `pydantic-2.0b3/tests/test_color.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 import pytest
 from pydantic_core import PydanticCustomError
 
 from pydantic import BaseModel, ValidationError
 from pydantic.color import Color
 
+pytestmark = pytest.mark.filterwarnings(
+    'ignore:The `Color` class is deprecated, use `pydantic_extra_types` instead.*:DeprecationWarning'
+)
+
 
 @pytest.mark.parametrize(
     'raw_color, as_tuple',
     [
         # named colors
         ('aliceblue', (240, 248, 255)),
         ('Antiquewhite', (250, 235, 215)),
```

### Comparing `pydantic-2.0b2/tests/test_computed_fields.py` & `pydantic-2.0b3/tests/test_computed_fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import random
 import sys
 from abc import ABC, abstractmethod
-from typing import Any, ClassVar, List, Tuple
+from typing import Any, Callable, ClassVar, List, Tuple
 
 import pytest
 from pydantic_core import ValidationError, core_schema
+from typing_extensions import TypedDict
 
 from pydantic import (
     BaseModel,
     Field,
     GetCoreSchemaHandler,
     PrivateAttr,
     TypeAdapter,
@@ -590,7 +591,97 @@
     assert submodel.model_dump(by_alias=True) == {
         'myStandardField': 1,
         'myComputedField': 2,
         'my_alias_none': 3,
         'myAliasedComputedField1': 4,
         'my_alias_2': 5,
     }
+
+
+def make_base_model() -> Any:
+    class CompModel(BaseModel):
+        pass
+
+    class Model(BaseModel):
+        @computed_field
+        @property
+        def comp_1(self) -> CompModel:
+            return CompModel()
+
+        @computed_field
+        @property
+        def comp_2(self) -> CompModel:
+            return CompModel()
+
+    return Model
+
+
+def make_dataclass() -> Any:
+    class CompModel(BaseModel):
+        pass
+
+    @dataclasses.dataclass
+    class Model:
+        @computed_field
+        @property
+        def comp_1(self) -> CompModel:
+            return CompModel()
+
+        @computed_field
+        @property
+        def comp_2(self) -> CompModel:
+            return CompModel()
+
+    return Model
+
+
+def make_typed_dict() -> Any:
+    class CompModel(BaseModel):
+        pass
+
+    class Model(TypedDict):
+        @computed_field  # type: ignore
+        @property
+        def comp_1(self) -> CompModel:
+            return CompModel()
+
+        @computed_field  # type: ignore
+        @property
+        def comp_2(self) -> CompModel:
+            return CompModel()
+
+    return Model
+
+
+@pytest.mark.parametrize(
+    'model_factory',
+    [
+        make_base_model,
+        pytest.param(
+            make_typed_dict,
+            marks=pytest.mark.xfail(
+                reason='computed fields do not work with TypedDict yet. See https://github.com/pydantic/pydantic-core/issues/657'
+            ),
+        ),
+        make_dataclass,
+    ],
+)
+def test_multiple_references_to_schema(model_factory: Callable[[], Any]) -> None:
+    """
+    https://github.com/pydantic/pydantic/issues/5980
+    """
+
+    model = model_factory()
+
+    ta = TypeAdapter(model)
+
+    assert ta.dump_python(model()) == {'comp_1': {}, 'comp_2': {}}
+
+    assert ta.json_schema() == {'type': 'object', 'properties': {}, 'title': 'Model'}
+
+    assert ta.json_schema(mode='serialization') == {
+        'type': 'object',
+        'properties': {'comp_1': {'$ref': '#/$defs/CompModel'}, 'comp_2': {'$ref': '#/$defs/CompModel'}},
+        'required': ['comp_1', 'comp_2'],
+        'title': 'Model',
+        '$defs': {'CompModel': {'type': 'object', 'properties': {}, 'title': 'CompModel'}},
+    }
```

### Comparing `pydantic-2.0b2/tests/test_config.py` & `pydantic-2.0b3/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -618,7 +618,17 @@
 
 def test_config_wrapper_get_item():
     config_wrapper = ConfigWrapper(config=ConfigDict(title='test'))
 
     assert config_wrapper.title == 'test'
     with pytest.raises(AttributeError, match="Config has no attribute 'test'"):
         config_wrapper.test
+
+
+def test_config_inheritance_with_annotations():
+    class Parent(BaseModel):
+        model_config: ConfigDict = {'extra': 'allow'}
+
+    class Child(Parent):
+        model_config: ConfigDict = {'str_to_lower': True}
+
+    assert Child.model_config == {'extra': 'allow', 'str_to_lower': True}
```

### Comparing `pydantic-2.0b2/tests/test_construction.py` & `pydantic-2.0b3/tests/test_construction.py`

 * *Files 2% similar despite different names*

```diff
@@ -496,7 +496,16 @@
     assert m.a == m2.a == 24
     assert isinstance(m2.d, Model)
     assert m.d is m2.d
     assert m.d.a == m2.d.a == 12
 
     m.a = 12
     assert m.a != m2.a
+
+
+def test_pydantic_extra():
+    class Model(BaseModel):
+        model_config = dict(extra='allow')
+        x: int
+
+    m = Model.model_construct(x=1, y=2)
+    assert m.__pydantic_extra__ == {'y': 2}
```

### Comparing `pydantic-2.0b2/tests/test_create_model.py` & `pydantic-2.0b3/tests/test_create_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,19 +306,15 @@
         else:
             _some_func = MyDescriptor(lambda self: self.x)
 
         @property
         def _double_x(self):
             return self.x * 2
 
-    if use_annotation or base is ModelPrivateAttr:
-        assert set(A.__private_attributes__) == {'_some_func'}
-    else:
-        assert set(A.__private_attributes__) == set()
-
+    assert set(A.__private_attributes__) == {'_some_func'}
     assert set_name_calls == [(A, '_some_func')]
 
     a = A(x=2)
 
     assert a._double_x == 4  # Ensure properties with leading underscores work fine and don't become private attributes
 
     assert get_calls == []
@@ -402,16 +398,16 @@
 
     del m.some_field
 
     assert not hasattr(m, 'some_field')
 
 
 @pytest.mark.skipif(
-    platform.python_implementation() == 'PyPy' and platform.python_version_tuple() < ('3', '8'),
-    reason='In this single case `del` behaves weird on pypy 3.7',
+    platform.python_implementation() == 'PyPy',
+    reason='In this single case `del` behaves weird on pypy',
 )
 def test_del_model_attr_error():
     class Model(BaseModel):
         some_field: str
 
     m = Model(some_field='value')
     assert not hasattr(m, 'other_field')
```

### Comparing `pydantic-2.0b2/tests/test_dataclasses.py` & `pydantic-2.0b3/tests/test_dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     TypeAdapter,
     ValidationError,
     computed_field,
     field_serializer,
     field_validator,
     model_validator,
 )
-from pydantic._internal._model_construction import MockValidator
+from pydantic._internal._mock_validator import MockValidator
 from pydantic.dataclasses import rebuild_dataclass
 from pydantic.fields import Field, FieldInfo
 from pydantic.json_schema import model_json_schema
 
 
 def test_simple():
     @pydantic.dataclasses.dataclass
@@ -562,15 +562,14 @@
                 'anyOf': [{'type': 'integer'}, {'type': 'null'}],
                 'default': None,
                 'title': 'The age of the user',
                 'description': 'do not lie!',
             },
             'aliases': {
                 'additionalProperties': {'type': 'string'},
-                'default': {'John': 'Joey'},
                 'title': 'Aliases',
                 'type': 'object',
             },
             'height': {
                 'anyOf': [{'maximum': 300, 'minimum': 50, 'type': 'integer'}, {'type': 'null'}],
                 'default': None,
                 'title': 'The height in cm',
@@ -2306,7 +2305,45 @@
 
     @pydantic.dataclasses.dataclass()
     class MyDataClass1:
         d2: Optional['Foo'] = None  # noqa F821
 
     with pytest.raises(PydanticUndefinedAnnotation, match="name 'Foo' is not defined"):
         rebuild_dataclass(MyDataClass1, _parent_namespace_depth=0)
+
+
+@pytest.mark.parametrize(
+    'dataclass_decorator',
+    [
+        pydantic.dataclasses.dataclass,
+        dataclasses.dataclass,
+    ],
+    ids=['pydantic', 'stdlib'],
+)
+def test_model_config(dataclass_decorator: Any) -> None:
+    @dataclass_decorator
+    class Model:
+        x: str
+        __pydantic_config__ = ConfigDict(str_to_lower=True)
+
+    ta = TypeAdapter(Model)
+    assert ta.validate_python({'x': 'ABC'}).x == 'abc'
+
+
+def test_model_config_override_in_decorator() -> None:
+    @pydantic.dataclasses.dataclass(config=ConfigDict(str_to_lower=False, str_strip_whitespace=True))
+    class Model:
+        x: str
+        __pydantic_config__ = ConfigDict(str_to_lower=True)
+
+    ta = TypeAdapter(Model)
+    assert ta.validate_python({'x': 'ABC '}).x == 'ABC'
+
+
+def test_model_config_override_in_decorator_empty_config() -> None:
+    @pydantic.dataclasses.dataclass(config=ConfigDict())
+    class Model:
+        x: str
+        __pydantic_config__ = ConfigDict(str_to_lower=True)
+
+    ta = TypeAdapter(Model)
+    assert ta.validate_python({'x': 'ABC '}).x == 'ABC '
```

### Comparing `pydantic-2.0b2/tests/test_datetime.py` & `pydantic-2.0b3/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_decorators.py` & `pydantic-2.0b3/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_deprecated.py` & `pydantic-2.0b3/tests/test_deprecated.py`

 * *Files 4% similar despite different names*

```diff
@@ -315,15 +315,15 @@
 
 
 @pytest.mark.parametrize('attribute,value', [('allow', 'allow'), ('ignore', 'ignore'), ('forbid', 'forbid')])
 def test_extra_used_as_enum(
     attribute: str,
     value: str,
 ) -> None:
-    with pytest.raises(
+    with pytest.warns(
         DeprecationWarning,
         match=re.escape("`pydantic.config.Extra` is deprecated, use literal values instead (e.g. `extra='allow'`)"),
     ):
         assert getattr(Extra, attribute) == value
 
 
 def test_field_min_items_deprecation():
@@ -637,7 +637,24 @@
         DeprecationWarning, match='The `validate_arguments` method is deprecated; use `validate_call` instead.'
     ):
 
         def test(a: int, b: int):
             pass
 
         validate_arguments()(test)
+
+
+def test_deprecated_color():
+    from pydantic.color import Color
+
+    with pytest.warns(DeprecationWarning, match='The `Color` class is deprecated, use `pydantic_extra_types` instead.'):
+        Color('red')
+
+
+def test_deprecated_payment():
+    from pydantic import PaymentCardNumber
+
+    with pytest.warns(
+        DeprecationWarning,
+        match='The `PaymentCardNumber` class is deprecated, use `pydantic_extra_types` instead.',
+    ):
+        PaymentCardNumber('4242424242424242')
```

### Comparing `pydantic-2.0b2/tests/test_deprecated_validate_arguments.py` & `pydantic-2.0b3/tests/test_deprecated_validate_arguments.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_discriminated_union.py` & `pydantic-2.0b3/tests/test_discriminated_union.py`

 * *Files 4% similar despite different names*

```diff
@@ -344,18 +344,16 @@
 
 
 class FooStrEnum(str, Enum):
     pass
 
 
 ENUM_TEST_CASES = [
-    pytest.param(Enum, {'a': 1, 'b': 2}, marks=pytest.mark.xfail(reason='Plain Enum discriminator not yet supported')),
-    pytest.param(
-        Enum, {'a': 'v_a', 'b': 'v_b'}, marks=pytest.mark.xfail(reason='Plain Enum discriminator not yet supported')
-    ),
+    pytest.param(Enum, {'a': 1, 'b': 2}),
+    pytest.param(Enum, {'a': 'v_a', 'b': 'v_b'}),
     (FooIntEnum, {'a': 1, 'b': 2}),
     (IntEnum, {'a': 1, 'b': 2}),
     (FooStrEnum, {'a': 'v_a', 'b': 'v_b'}),
 ]
 if sys.version_info >= (3, 11):
     from enum import StrEnum
 
@@ -373,26 +371,28 @@
     class B(BaseModel):
         m: Literal[EnumValue.b]
 
     class Top(BaseModel):
         sub: Union[A, B] = Field(..., discriminator='m')
 
     assert isinstance(Top.model_validate({'sub': {'m': EnumValue.b}}).sub, B)
-    assert isinstance(Top.model_validate({'sub': {'m': EnumValue.b.value}}).sub, B)
+    if isinstance(EnumValue.b, (int, str)):
+        assert isinstance(Top.model_validate({'sub': {'m': EnumValue.b.value}}).sub, B)
     with pytest.raises(ValidationError) as exc_info:
         Top.model_validate({'sub': {'m': 3}})
 
-    expected_tags = f'{EnumValue.a.value!r}, {EnumValue.b.value!r}'
+    expected_tags = f'{EnumValue.a!r}, {EnumValue.b!r}'
+    # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
         {
-            'ctx': {'discriminator': "'m'", 'expected_tags': expected_tags, 'tag': '3'},
-            'input': {'m': 3},
+            'type': 'union_tag_invalid',
             'loc': ('sub',),
             'msg': f"Input tag '3' found using 'm' does not match any of the expected tags: {expected_tags}",
-            'type': 'union_tag_invalid',
+            'input': {'m': 3},
+            'ctx': {'discriminator': "'m'", 'tag': '3', 'expected_tags': expected_tags},
         }
     ]
 
 
 def test_alias_different():
     class Cat(BaseModel):
         pet_type: Literal['cat'] = Field(alias='U')
@@ -613,28 +613,35 @@
     Pet.model_validate({'pet': {'pet_type': 'cat'}})
     Pet.model_validate({'pet': {'pet_type': 'lizard'}})
     Pet.model_validate({'pet': {'pet_type': 'reptile'}})
     Pet.model_validate({'pet': None})
 
     with pytest.raises(ValidationError) as exc_info:
         Pet.model_validate({'pet': {'pet_type': None}})
+    # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
-        {'input': None, 'loc': ('pet',), 'msg': 'Input should be a valid string', 'type': 'string_type'}
+        {
+            'type': 'union_tag_invalid',
+            'loc': ('pet',),
+            'msg': "Input tag 'None' found using 'pet_type' does not match any of the expected tags: 'cat', 'dog', 'lizard', 'reptile'",  # noqa: E501
+            'input': {'pet_type': None},
+            'ctx': {'discriminator': "'pet_type'", 'tag': 'None', 'expected_tags': "'cat', 'dog', 'lizard', 'reptile'"},
+        }
     ]
 
     with pytest.raises(ValidationError) as exc_info:
         Pet.model_validate({'pet': {'pet_type': 'fox'}})
+    # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
         {
-            'ctx': {'discriminator': "'pet_type'", 'expected_tags': "'cat', 'dog', 'lizard', 'reptile'", 'tag': 'fox'},
-            'input': {'pet_type': 'fox'},
-            'loc': ('pet',),
-            'msg': "Input tag 'fox' found using 'pet_type' does not match any of the "
-            "expected tags: 'cat', 'dog', 'lizard', 'reptile'",
             'type': 'union_tag_invalid',
+            'loc': ('pet',),
+            'msg': "Input tag 'fox' found using 'pet_type' does not match any of the expected tags: 'cat', 'dog', 'lizard', 'reptile'",  # noqa: E501
+            'input': {'pet_type': 'fox'},
+            'ctx': {'discriminator': "'pet_type'", 'tag': 'fox', 'expected_tags': "'cat', 'dog', 'lizard', 'reptile'"},
         }
     ]
 
 
 def test_nested_discriminated_union() -> None:
     class Cat(BaseModel):
         pet_type: Literal['cat', 'CAT']
@@ -653,26 +660,26 @@
 
     Pet.model_validate({'pet': {'pet_type': 'dog'}})
     Pet.model_validate({'pet': {'pet_type': 'cat'}})
     Pet.model_validate({'pet': {'pet_type': 'lizard'}})
 
     with pytest.raises(ValidationError) as exc_info:
         Pet.model_validate({'pet': {'pet_type': 'reptile'}})
+    # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
         {
+            'type': 'union_tag_invalid',
+            'loc': ('pet',),
+            'msg': "Input tag 'reptile' found using 'pet_type' does not match any of the expected tags: 'cat', 'CAT', 'dog', 'DOG', 'lizard', 'LIZARD'",  # noqa: E501
+            'input': {'pet_type': 'reptile'},
             'ctx': {
                 'discriminator': "'pet_type'",
-                'expected_tags': "'cat', 'dog', 'lizard', 'CAT', 'DOG', 'LIZARD'",
                 'tag': 'reptile',
+                'expected_tags': "'cat', 'CAT', 'dog', 'DOG', 'lizard', 'LIZARD'",
             },
-            'input': {'pet_type': 'reptile'},
-            'loc': ('pet',),
-            'msg': "Input tag 'reptile' found using 'pet_type' does not match any of the "
-            "expected tags: 'cat', 'dog', 'lizard', 'CAT', 'DOG', 'LIZARD'",
-            'type': 'union_tag_invalid',
         }
     ]
 
 
 def test_unions_of_optionals() -> None:
     class Cat(BaseModel):
         pet_type: Literal['cat'] = Field(alias='typeOfPet')
@@ -707,22 +714,22 @@
         pet: Union[Cat, Dog] = Field(discriminator='pet_type')
 
     assert Model(**{'pet': {'typeOfPet': 'dog'}}).pet.pet_type == 'dog'
     assert Model(**{'pet': {'typeOfPet': 'cat'}}).pet.pet_type == 'cat'
     assert Model(**{'pet': {'typeOfPet': 'CAT'}}).pet.pet_type == 'CAT'
     with pytest.raises(ValidationError) as exc_info:
         Model(**{'pet': {'typeOfPet': 'Cat'}})
+    # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
         {
-            'ctx': {'discriminator': "'pet_type' | 'typeOfPet'", 'expected_tags': "'cat', 'dog', 'CAT'", 'tag': 'Cat'},
-            'input': {'typeOfPet': 'Cat'},
-            'loc': ('pet',),
-            'msg': "Input tag 'Cat' found using 'pet_type' | 'typeOfPet' does not match "
-            "any of the expected tags: 'cat', 'dog', 'CAT'",
             'type': 'union_tag_invalid',
+            'loc': ('pet',),
+            'msg': "Input tag 'Cat' found using 'pet_type' | 'typeOfPet' does not match any of the expected tags: 'cat', 'CAT', 'dog'",  # noqa: E501
+            'input': {'typeOfPet': 'Cat'},
+            'ctx': {'discriminator': "'pet_type' | 'typeOfPet'", 'tag': 'Cat', 'expected_tags': "'cat', 'CAT', 'dog'"},
         }
     ]
 
 
 def test_none_schema() -> None:
     cat_fields = {'kind': core_schema.typed_dict_field(core_schema.literal_schema(['cat']))}
     dog_fields = {'kind': core_schema.typed_dict_field(core_schema.literal_schema(['dog']))}
@@ -844,27 +851,14 @@
     cat = core_schema.typed_dict_schema(cat_fields)
     dog = core_schema.typed_dict_schema(dog_fields)
 
     with pytest.raises(TypeError, match=re.escape("TypedDict needs a discriminator field for key 'kind'")):
         apply_discriminator(core_schema.union_schema([dog, cat]), 'kind')
 
 
-def test_invalid_discriminator_value() -> None:
-    cat_fields = {'kind': core_schema.typed_dict_field(core_schema.literal_schema([None]))}
-    dog_fields = {'kind': core_schema.typed_dict_field(core_schema.literal_schema([1.5]))}
-    cat = core_schema.typed_dict_schema(cat_fields)
-    dog = core_schema.typed_dict_schema(dog_fields)
-
-    with pytest.raises(TypeError, match=re.escape('Unsupported value for discriminator field: None')):
-        apply_discriminator(core_schema.union_schema([cat, dog]), 'kind')
-
-    with pytest.raises(TypeError, match=re.escape('Unsupported value for discriminator field: 1.5')):
-        apply_discriminator(core_schema.union_schema([dog, cat]), 'kind')
-
-
 def test_wrap_function_schema() -> None:
     cat_fields = {'kind': core_schema.typed_dict_field(core_schema.literal_schema(['cat']))}
     dog_fields = {'kind': core_schema.typed_dict_field(core_schema.literal_schema(['dog']))}
     cat = core_schema.general_wrap_validator_function(lambda x, y, z: None, core_schema.typed_dict_schema(cat_fields))
     dog = core_schema.typed_dict_schema(dog_fields)
     schema = core_schema.union_schema([cat, dog])
 
@@ -936,51 +930,70 @@
         [core_schema.int_schema(ref='my-int-definition')],
     )
     dog = core_schema.definitions_schema(
         core_schema.lax_or_strict_schema(lax_schema=lax_dog, strict_schema=strict_dog),
         [core_schema.str_schema(ref='my-str-definition')],
     )
     discriminated_schema = apply_discriminator(core_schema.union_schema([cat, dog]), 'kind')
+    # insert_assert(discriminated_schema)
     assert discriminated_schema == {
-        'definitions': [{'ref': 'my-str-definition', 'type': 'str'}],
+        'type': 'definitions',
         'schema': {
+            'type': 'tagged-union',
             'choices': {
+                'cat': {
+                    'type': 'typed-dict',
+                    'fields': {
+                        'kind': {'type': 'typed-dict-field', 'schema': {'type': 'literal', 'expected': ['cat']}}
+                    },
+                },
                 'DOG': {
+                    'type': 'lax-or-strict',
                     'lax_schema': {
+                        'type': 'typed-dict',
                         'fields': {
-                            'kind': {'schema': {'expected': ['DOG'], 'type': 'literal'}, 'type': 'typed-dict-field'}
+                            'kind': {'type': 'typed-dict-field', 'schema': {'type': 'literal', 'expected': ['DOG']}}
                         },
-                        'type': 'typed-dict',
                     },
                     'strict_schema': {
-                        'definitions': [{'ref': 'my-int-definition', 'type': 'int'}],
+                        'type': 'definitions',
                         'schema': {
+                            'type': 'typed-dict',
                             'fields': {
-                                'kind': {'schema': {'expected': ['dog'], 'type': 'literal'}, 'type': 'typed-dict-field'}
+                                'kind': {'type': 'typed-dict-field', 'schema': {'type': 'literal', 'expected': ['dog']}}
                             },
-                            'type': 'typed-dict',
                         },
-                        'type': 'definitions',
+                        'definitions': [{'type': 'int', 'ref': 'my-int-definition'}],
                     },
-                    'type': 'lax-or-strict',
                 },
-                'cat': {
-                    'fields': {
-                        'kind': {'schema': {'expected': ['cat'], 'type': 'literal'}, 'type': 'typed-dict-field'}
+                'dog': {
+                    'type': 'lax-or-strict',
+                    'lax_schema': {
+                        'type': 'typed-dict',
+                        'fields': {
+                            'kind': {'type': 'typed-dict-field', 'schema': {'type': 'literal', 'expected': ['DOG']}}
+                        },
+                    },
+                    'strict_schema': {
+                        'type': 'definitions',
+                        'schema': {
+                            'type': 'typed-dict',
+                            'fields': {
+                                'kind': {'type': 'typed-dict-field', 'schema': {'type': 'literal', 'expected': ['dog']}}
+                            },
+                        },
+                        'definitions': [{'type': 'int', 'ref': 'my-int-definition'}],
                     },
-                    'type': 'typed-dict',
                 },
-                'dog': 'DOG',
             },
             'discriminator': 'kind',
-            'from_attributes': True,
             'strict': False,
-            'type': 'tagged-union',
+            'from_attributes': True,
         },
-        'type': 'definitions',
+        'definitions': [{'type': 'str', 'ref': 'my-str-definition'}],
     }
 
 
 def test_wrapped_nullable_union() -> None:
     cat = core_schema.typed_dict_schema({'kind': core_schema.typed_dict_field(core_schema.literal_schema(['cat']))})
     dog = core_schema.typed_dict_schema({'kind': core_schema.typed_dict_field(core_schema.literal_schema(['dog']))})
     ant = core_schema.typed_dict_schema({'kind': core_schema.typed_dict_field(core_schema.literal_schema(['ant']))})
@@ -1010,58 +1023,91 @@
             'loc': (),
             'msg': "Input tag 'armadillo' found using 'kind' does not match any of the "
             "expected tags: 'ant', 'cat', 'dog'",
             'type': 'union_tag_invalid',
         }
     ]
 
+    # insert_assert(discriminated_schema)
     assert discriminated_schema == {
+        'type': 'nullable',
         'schema': {
+            'type': 'tagged-union',
             'choices': {
                 'ant': {
+                    'type': 'typed-dict',
                     'fields': {
-                        'kind': {'schema': {'expected': ['ant'], 'type': 'literal'}, 'type': 'typed-dict-field'}
+                        'kind': {'type': 'typed-dict-field', 'schema': {'type': 'literal', 'expected': ['ant']}}
                     },
-                    'type': 'typed-dict',
                 },
                 'cat': {
+                    'type': 'function-wrap',
                     'function': {
-                        'function': HasRepr(IsStr(regex=r'<function [a-z_]*\.<locals>\.<lambda> at 0x[0-9a-fA-F]+>')),
                         'type': 'general',
+                        'function': HasRepr(IsStr(regex=r'<function [a-z_]*\.<locals>\.<lambda> at 0x[0-9a-fA-F]+>')),
                     },
                     'schema': {
+                        'type': 'nullable',
                         'schema': {
+                            'type': 'union',
                             'choices': [
                                 {
+                                    'type': 'typed-dict',
                                     'fields': {
                                         'kind': {
-                                            'schema': {'expected': ['cat'], 'type': 'literal'},
                                             'type': 'typed-dict-field',
+                                            'schema': {'type': 'literal', 'expected': ['cat']},
                                         }
                                     },
+                                },
+                                {
                                     'type': 'typed-dict',
+                                    'fields': {
+                                        'kind': {
+                                            'type': 'typed-dict-field',
+                                            'schema': {'type': 'literal', 'expected': ['dog']},
+                                        }
+                                    },
                                 },
+                            ],
+                        },
+                    },
+                },
+                'dog': {
+                    'type': 'function-wrap',
+                    'function': {
+                        'type': 'general',
+                        'function': HasRepr(IsStr(regex=r'<function [a-z_]*\.<locals>\.<lambda> at 0x[0-9a-fA-F]+>')),
+                    },
+                    'schema': {
+                        'type': 'nullable',
+                        'schema': {
+                            'type': 'union',
+                            'choices': [
                                 {
+                                    'type': 'typed-dict',
                                     'fields': {
                                         'kind': {
-                                            'schema': {'expected': ['dog'], 'type': 'literal'},
                                             'type': 'typed-dict-field',
+                                            'schema': {'type': 'literal', 'expected': ['cat']},
                                         }
                                     },
+                                },
+                                {
                                     'type': 'typed-dict',
+                                    'fields': {
+                                        'kind': {
+                                            'type': 'typed-dict-field',
+                                            'schema': {'type': 'literal', 'expected': ['dog']},
+                                        }
+                                    },
                                 },
                             ],
-                            'type': 'union',
                         },
-                        'type': 'nullable',
                     },
-                    'type': 'function-wrap',
                 },
-                'dog': 'cat',
             },
             'discriminator': 'kind',
-            'from_attributes': True,
             'strict': False,
-            'type': 'tagged-union',
+            'from_attributes': True,
         },
-        'type': 'nullable',
     }
```

### Comparing `pydantic-2.0b2/tests/test_docs.py` & `pydantic-2.0b3/tests/test_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,18 +101,19 @@
     if requires_settings:
         major, minor = map(int, requires_settings.split('.'))
         if sys.version_info < (major, minor):
             pytest.skip(f'requires python {requires_settings}')
 
     group_name = prefix_settings.get('group')
 
+    eval_example.set_config(ruff_ignore=['D'])
     if '# ignore-above' in example.source:
-        eval_example.set_config(ruff_ignore=['E402'])
+        eval_example.set_config(ruff_ignore=['D', 'E402'])
     if group_name:
-        eval_example.set_config(ruff_ignore=['F821'])
+        eval_example.set_config(ruff_ignore=['D', 'F821'])
 
     if not lint_settings.startswith('skip'):
         if eval_example.update_examples:
             eval_example.format(example)
         else:
             eval_example.lint(example)
 
@@ -151,14 +152,16 @@
 @pytest.mark.skipif(bool(skip_reason), reason=skip_reason or 'not skipping')
 @pytest.mark.parametrize(
     'example', find_examples(str(DOCS_ROOT / 'integrations/devtools.md'), skip=sys.platform == 'win32'), ids=str
 )
 def test_docs_devtools_example(example: CodeExample, eval_example: EvalExample, tmp_path: Path):
     from ansi2html import Ansi2HTMLConverter
 
+    eval_example.set_config(ruff_ignore=['D'])
+
     if eval_example.update_examples:
         eval_example.format(example)
     else:
         eval_example.lint(example)
 
     with NamedTemporaryFile(mode='w', suffix='.py') as f:
         f.write(example.source)
```

### Comparing `pydantic-2.0b2/tests/test_edge_cases.py` & `pydantic-2.0b3/tests/test_edge_cases.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_errors.py` & `pydantic-2.0b3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_exports.py` & `pydantic-2.0b3/tests/test_exports.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import importlib
 import importlib.util
+import platform
 import sys
 from pathlib import Path
 from types import ModuleType
 
 import pytest
 
 import pydantic
@@ -18,17 +20,29 @@
             continue
         if isinstance(attr, ModuleType) and name != 'dataclasses':
             continue
         if name == 'getattr_migration':
             continue
         exported.add(name)
 
+    exported.update(pydantic._dynamic_imports)
+
     assert pydantic_all == exported, "pydantic.__all__ doesn't match actual exports"
 
 
+@pytest.mark.parametrize(('attr_name', 'module_name'), list(pydantic._dynamic_imports.items()))
+def test_public_api_dynamic_imports(attr_name, module_name):
+    imported_object = getattr(importlib.import_module(module_name, package='pydantic'), attr_name)
+    assert isinstance(imported_object, object)
+
+
+@pytest.mark.skipif(
+    platform.python_implementation() == 'PyPy' and platform.python_version_tuple() < ('3', '8'),
+    reason='Produces a weird error on pypy<3.8',
+)
 @pytest.mark.filterwarnings('ignore::DeprecationWarning')
 def test_public_internal():
     """
     check we don't make anything from _internal public
     """
     public_internal_attributes = []
     for file in (Path(__file__).parent.parent / 'pydantic').glob('*.py'):
```

### Comparing `pydantic-2.0b2/tests/test_fastapi_json_schema.py` & `pydantic-2.0b3/tests/test_fastapi_json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_fields.py` & `pydantic-2.0b3/tests/test_fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,28 @@
         @pydantic.dataclasses.dataclass
         class Model:
             some_field: InitVar[str]
 
     assert e.value.args == ('InitVar is not supported in Python 3.7 as type information is lost',)
 
 
+def test_init_var_field():
+    @pydantic.dataclasses.dataclass
+    class Foo:
+        bar: str
+        baz: str = Field(init_var=True)
+
+    class Model(BaseModel):
+        foo: Foo
+
+    model = Model(foo=Foo('bar', baz='baz'))
+    assert 'bar' in model.foo.__pydantic_fields__
+    assert 'baz' not in model.foo.__pydantic_fields__
+
+
 def test_root_model_arbitrary_field_name_error():
     with pytest.raises(
         NameError, match="Unexpected field with name 'a_field'; only 'root' is allowed as a field of a `RootModel`"
     ):
 
         class Model(RootModel[int]):
             a_field: str
```

### Comparing `pydantic-2.0b2/tests/test_forward_ref.py` & `pydantic-2.0b3/tests/test_forward_ref.py`

 * *Files 6% similar despite different names*

```diff
@@ -953,7 +953,41 @@
 
             UndefinedType = ForwardRef('UndefinedType')
 
             class Foobar(BaseModel):
                 a: UndefinedType
 
             Foobar(a=1)
+
+
+def test_rebuild_recursive_schema():
+    from typing import ForwardRef, List
+
+    class Expressions_(BaseModel):
+        model_config = dict(undefined_types_warning=False)
+        items: List["types['Expression']"]
+
+    class Expression_(BaseModel):
+        model_config = dict(undefined_types_warning=False)
+        Or: ForwardRef("types['allOfExpressions']")
+        Not: ForwardRef("types['allOfExpression']")
+
+    class allOfExpression_(BaseModel):
+        model_config = dict(undefined_types_warning=False)
+        Not: ForwardRef("types['Expression']")
+
+    class allOfExpressions_(BaseModel):
+        model_config = dict(undefined_types_warning=False)
+        items: List["types['Expression']"]
+
+    types_namespace = {
+        'types': {
+            'Expression': Expression_,
+            'Expressions': Expressions_,
+            'allOfExpression': allOfExpression_,
+            'allOfExpressions': allOfExpressions_,
+        }
+    }
+
+    models = [allOfExpressions_, Expressions_]
+    for m in models:
+        m.model_rebuild(_types_namespace=types_namespace)
```

### Comparing `pydantic-2.0b2/tests/test_generics.py` & `pydantic-2.0b3/tests/test_generics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1107,91 +1107,75 @@
     T = TypeVar('T')
     KT = TypeVar('KT')
     VT = TypeVar('VT')
 
     class CustomCounter(Counter[T]):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
-            return core_schema.no_info_after_validator_function(
-                cls, handler.generate_schema(Counter[get_args(source_type)[0]])
-            )
+            return core_schema.no_info_after_validator_function(cls, handler(Counter[get_args(source_type)[0]]))
 
     class CustomDefaultDict(DefaultDict[KT, VT]):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
             keys_type, values_type = get_args(source_type)
             return core_schema.no_info_after_validator_function(
-                lambda x: cls(x.default_factory, x), handler.generate_schema(DefaultDict[keys_type, values_type])
+                lambda x: cls(x.default_factory, x), handler(DefaultDict[keys_type, values_type])
             )
 
     class CustomDeque(Deque[T]):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
-            return core_schema.no_info_after_validator_function(
-                cls, handler.generate_schema(Deque[get_args(source_type)[0]])
-            )
+            return core_schema.no_info_after_validator_function(cls, handler(Deque[get_args(source_type)[0]]))
 
     class CustomDict(Dict[KT, VT]):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
             keys_type, values_type = get_args(source_type)
-            return core_schema.no_info_after_validator_function(
-                cls, handler.generate_schema(Dict[keys_type, values_type])
-            )
+            return core_schema.no_info_after_validator_function(cls, handler(Dict[keys_type, values_type]))
 
     class CustomFrozenset(FrozenSet[T]):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
-            return core_schema.no_info_after_validator_function(
-                cls, handler.generate_schema(FrozenSet[get_args(source_type)[0]])
-            )
+            return core_schema.no_info_after_validator_function(cls, handler(FrozenSet[get_args(source_type)[0]]))
 
     class CustomIterable(Iterable[T]):
         def __init__(self, iterable):
             self.iterable = iterable
 
         def __iter__(self):
             return self
 
         def __next__(self):
             return next(self.iterable)
 
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
-            return core_schema.no_info_after_validator_function(
-                cls, handler.generate_schema(Iterable[get_args(source_type)[0]])
-            )
+            return core_schema.no_info_after_validator_function(cls, handler(Iterable[get_args(source_type)[0]]))
 
     class CustomList(List[T]):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
-            return core_schema.no_info_after_validator_function(
-                cls, handler.generate_schema(List[get_args(source_type)[0]])
-            )
+            return core_schema.no_info_after_validator_function(cls, handler(List[get_args(source_type)[0]]))
 
     class CustomMapping(Mapping[KT, VT]):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
             keys_type, values_type = get_args(source_type)
-            return handler.generate_schema(Mapping[keys_type, values_type])
+            return handler(Mapping[keys_type, values_type])
 
     class CustomOrderedDict(OrderedDict[KT, VT]):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
             keys_type, values_type = get_args(source_type)
-            return core_schema.no_info_after_validator_function(
-                cls, handler.generate_schema(OrderedDict[keys_type, values_type])
-            )
+            return core_schema.no_info_after_validator_function(cls, handler(OrderedDict[keys_type, values_type]))
 
     class CustomSet(Set[T]):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
-            return core_schema.no_info_after_validator_function(
-                cls, handler.generate_schema(Set[get_args(source_type)[0]])
-            )
+            return core_schema.no_info_after_validator_function(cls, handler(Set[get_args(source_type)[0]]))
 
     class CustomTuple(Tuple[T]):
         pass
 
     class Model(BaseModel, Generic[T, KT, VT]):
         counter_field: CustomCounter[T]
         default_dict_field: CustomDefaultDict[KT, VT]
@@ -1873,17 +1857,15 @@
 
 def test_generic_with_user_defined_generic_field():
     T = TypeVar('T')
 
     class GenericList(List[T]):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
-            return core_schema.no_info_after_validator_function(
-                GenericList, handler.generate_schema(List[get_args(source_type)[0]])
-            )
+            return core_schema.no_info_after_validator_function(GenericList, handler(List[get_args(source_type)[0]]))
 
     class Model(BaseModel, Generic[T]):
         field: GenericList[T]
 
     model = Model[int](field=[5])
     assert model.field[0] == 5
```

### Comparing `pydantic-2.0b2/tests/test_internal.py` & `pydantic-2.0b3/tests/test_internal.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_json.py` & `pydantic-2.0b3/tests/test_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from dataclasses import dataclass as vanilla_dataclass
 from datetime import date, datetime, time, timedelta, timezone
 from decimal import Decimal
 from enum import Enum
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from pathlib import Path
-from typing import Any, Generator, Optional, Pattern
+from typing import Any, Generator, Optional, Pattern, Union
 from uuid import UUID
 
 import pytest
 from pydantic_core import CoreSchema, SchemaSerializer, core_schema
 
 from pydantic import BaseModel, ConfigDict, GetCoreSchemaHandler, GetJsonSchemaHandler, NameEmail
 from pydantic._internal._config import ConfigWrapper
@@ -19,14 +19,15 @@
 from pydantic.color import Color
 from pydantic.dataclasses import dataclass as pydantic_dataclass
 from pydantic.deprecated.json import pydantic_encoder, timedelta_isoformat
 from pydantic.functional_serializers import (
     field_serializer,
 )
 from pydantic.json_schema import JsonSchemaValue
+from pydantic.type_adapter import TypeAdapter
 from pydantic.types import DirectoryPath, FilePath, SecretBytes, SecretStr, condecimal
 
 try:
     import email_validator
 except ImportError:
     email_validator = None
 
@@ -73,19 +74,16 @@
         (Decimal, lambda: Decimal('12.34'), b'"12.34"'),
         (MyModel, lambda: MyModel(), b'{"a":"b","c":"d"}'),
         (MyEnum, lambda: MyEnum.foo, b'"bar"'),
         (Pattern, lambda: re.compile('^regex$'), b'"^regex$"'),
     ],
 )
 def test_json_serialization(ser_type, gen_value, json_output):
-    config_wrapper = ConfigWrapper({'arbitrary_types_allowed': False})
-    gen = GenerateSchema(config_wrapper, None)
-    schema = gen.generate_schema(ser_type)
-    serializer = SchemaSerializer(schema)
-    assert serializer.to_json(gen_value()) == json_output
+    ta: TypeAdapter[Any] = TypeAdapter(ser_type)
+    assert ta.dump_json(gen_value()) == json_output
 
 
 @pytest.mark.skipif(not email_validator, reason='email_validator not installed')
 def test_json_serialization_email():
     config_wrapper = ConfigWrapper({'arbitrary_types_allowed': False})
     gen = GenerateSchema(config_wrapper, None)
     schema = gen.generate_schema(NameEmail)
@@ -130,15 +128,15 @@
 def test_subclass_encoding():
     class SubDate(datetime):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
             def val(v: datetime) -> SubDate:
                 return SubDate.fromtimestamp(v.timestamp())
 
-            return core_schema.no_info_after_validator_function(val, handler.generate_schema(datetime))
+            return core_schema.no_info_after_validator_function(val, handler(datetime))
 
     class Model(BaseModel):
         a: datetime
         b: SubDate
 
     m = Model(a=datetime(2032, 1, 1, 1, 1), b=SubDate(2020, 2, 29, 12, 30))
     assert m.model_dump() == {'a': datetime(2032, 1, 1, 1, 1), 'b': SubDate(2020, 2, 29, 12, 30)}
@@ -148,23 +146,23 @@
 def test_subclass_custom_encoding():
     class SubDt(datetime):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
             def val(v: datetime) -> SubDt:
                 return SubDt.fromtimestamp(v.timestamp())
 
-            return core_schema.no_info_after_validator_function(val, handler.generate_schema(datetime))
+            return core_schema.no_info_after_validator_function(val, handler(datetime))
 
     class SubDelta(timedelta):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
             def val(v: timedelta) -> SubDelta:
                 return cls(seconds=v.total_seconds())
 
-            return core_schema.no_info_after_validator_function(val, handler.generate_schema(timedelta))
+            return core_schema.no_info_after_validator_function(val, handler(timedelta))
 
     class Model(BaseModel):
         a: SubDt
         b: SubDelta
 
         @field_serializer('a', when_used='json')
         def serialize_a(self, v: SubDt, _info):
@@ -355,25 +353,33 @@
 """
     )
     M = module.Model
 
     assert M(value=1, nested=M(value=2)).model_dump_json(exclude_none=True) == '{"value":1,"nested":{"value":2}}'
 
 
-def test_unresolvable_schema_lookup_error():
+def test_resolve_ref_schema_recursive_model():
     class Model(BaseModel):
-        mini_me: 'Model'
+        mini_me: Union['Model', None]
 
         @classmethod
         def __get_pydantic_json_schema__(
             cls, core_schema: CoreSchema, handler: GetJsonSchemaHandler
         ) -> JsonSchemaValue:
             json_schema = super().__get_pydantic_json_schema__(core_schema, handler)
-            return handler.resolve_ref_schema(json_schema)
-
-    with pytest.raises(LookupError) as e:
-        Model.model_json_schema()
-
-    assert e.value.args[0] == (
-        'Could not find a ref for #/$defs/Model.'
-        ' Maybe you tried to call resolve_ref_schema from within a recursive model?'
-    )
+            json_schema = handler.resolve_ref_schema(json_schema)
+            json_schema['examples'] = {'foo': {'mini_me': None}}
+            return json_schema
+
+    # insert_assert(Model.model_json_schema())
+    assert Model.model_json_schema() == {
+        '$defs': {
+            'Model': {
+                'examples': {'foo': {'mini_me': None}},
+                'properties': {'mini_me': {'anyOf': [{'$ref': '#/$defs/Model'}, {'type': 'null'}]}},
+                'required': ['mini_me'],
+                'title': 'Model',
+                'type': 'object',
+            }
+        },
+        'allOf': [{'$ref': '#/$defs/Model'}],
+    }
```

### Comparing `pydantic-2.0b2/tests/test_json_schema.py` & `pydantic-2.0b3/tests/test_json_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,36 +26,40 @@
     Type,
     TypeVar,
     Union,
 )
 from uuid import UUID
 
 import pytest
-from pydantic_core import CoreSchema, core_schema
-from typing_extensions import Annotated, Literal
+from pydantic_core import CoreSchema, core_schema, to_json
+from typing_extensions import Annotated, Literal, TypedDict
 
+import pydantic
 from pydantic import (
     BaseModel,
     Field,
     GetCoreSchemaHandler,
     GetJsonSchemaHandler,
     ImportString,
+    InstanceOf,
     PydanticUserError,
     RootModel,
     ValidationError,
+    WithJsonSchema,
     computed_field,
     field_validator,
 )
 from pydantic._internal._core_metadata import CoreMetadataHandler, build_metadata_dict
 from pydantic.color import Color
 from pydantic.config import ConfigDict
 from pydantic.dataclasses import dataclass
 from pydantic.errors import PydanticInvalidForJsonSchema
 from pydantic.json_schema import (
     DEFAULT_REF_TEMPLATE,
+    Examples,
     GenerateJsonSchema,
     JsonSchemaValue,
     PydanticJsonSchemaWarning,
     model_json_schema,
     models_json_schema,
 )
 from pydantic.networks import AnyUrl, EmailStr, IPvAnyAddress, IPvAnyInterface, IPvAnyNetwork, MultiHostUrl, NameEmail
@@ -63,30 +67,28 @@
 from pydantic.types import (
     UUID1,
     UUID3,
     UUID4,
     UUID5,
     DirectoryPath,
     FilePath,
-    InstanceOf,
     Json,
     NegativeFloat,
     NegativeInt,
     NewPath,
     NonNegativeFloat,
     NonNegativeInt,
     NonPositiveFloat,
     NonPositiveInt,
     PositiveFloat,
     PositiveInt,
     SecretBytes,
     SecretStr,
     StrictBool,
     StrictStr,
-    WithJsonSchema,
     conbytes,
     condate,
     condecimal,
     confloat,
     conint,
     constr,
 )
@@ -110,15 +112,15 @@
         'title': 'Apple Pie',
         'properties': {
             'Snap': {'type': 'number', 'title': 'Snap'},
             'Crackle': {'type': 'integer', 'title': 'Crackle', 'default': 10},
         },
         'required': ['Snap'],
     }
-    assert list(ApplePie.model_json_schema(by_alias=True)['properties'].keys()) == ['Snap', 'Crackle']
+    assert list(ApplePie.model_json_schema(by_alias=True)['properties'].keys()) == ['Crackle', 'Snap']
     assert list(ApplePie.model_json_schema(by_alias=False)['properties'].keys()) == ['a', 'b']
 
 
 def test_ref_template():
     class KeyLimePie(BaseModel):
         x: str = None
 
@@ -244,27 +246,28 @@
         bar = 'b'
 
     class Model(BaseModel):
         foo: FooEnum
         bar: BarEnum
         spam: SpamEnum = Field(None)
 
+    # insert_assert(Model.model_json_schema())
     assert Model.model_json_schema() == {
-        'title': 'Model',
         'type': 'object',
         'properties': {
             'foo': {'$ref': '#/$defs/FooEnum'},
             'bar': {'$ref': '#/$defs/BarEnum'},
             'spam': {'allOf': [{'$ref': '#/$defs/SpamEnum'}], 'default': None},
         },
         'required': ['foo', 'bar'],
+        'title': 'Model',
         '$defs': {
-            'FooEnum': {'title': 'FooEnum', 'enum': ['f', 'b']},
-            'BarEnum': {'title': 'BarEnum', 'type': 'integer', 'enum': [1, 2]},
-            'SpamEnum': {'title': 'SpamEnum', 'type': 'string', 'enum': ['f', 'b']},
+            'BarEnum': {'enum': [1, 2], 'title': 'BarEnum', 'type': 'integer'},
+            'SpamEnum': {'enum': ['f', 'b'], 'title': 'SpamEnum', 'type': 'string'},
+            'FooEnum': {'enum': ['f', 'b'], 'title': 'FooEnum'},
         },
     }
 
 
 def test_enum_modify_schema():
     class SpamEnum(str, Enum):
         """
@@ -275,23 +278,24 @@
         bar = 'b'
 
         @classmethod
         def __get_pydantic_json_schema__(
             cls, core_schema: CoreSchema, handler: GetJsonSchemaHandler
         ) -> JsonSchemaValue:
             field_schema = handler(core_schema)
+            field_schema = handler.resolve_ref_schema(field_schema)
             existing_comment = field_schema.get('$comment', '')
             field_schema['$comment'] = existing_comment + 'comment'  # make sure this function is only called once
-
             field_schema['tsEnumNames'] = [e.name for e in cls]
             return field_schema
 
     class Model(BaseModel):
         spam: Optional[SpamEnum] = Field(None)
 
+    # insert_assert(Model.model_json_schema())
     assert Model.model_json_schema() == {
         '$defs': {
             'SpamEnum': {
                 '$comment': 'comment',
                 'description': 'Spam enum.',
                 'enum': ['f', 'b'],
                 'title': 'SpamEnum',
@@ -311,39 +315,34 @@
         bar = 'bar'
 
     class Model(BaseModel):
         pika: FooBarEnum = Field(alias='pikalias', title='Pikapika!', description='Pika is definitely the best!')
         bulbi: FooBarEnum = Field('foo', alias='bulbialias', title='Bulbibulbi!', description='Bulbi is not...')
         cara: FooBarEnum
 
+    # insert_assert(Model.model_json_schema())
     assert Model.model_json_schema() == {
-        '$defs': {
-            'FooBarEnum': {
-                'enum': ['foo', 'bar'],
-                'title': 'FooBarEnum',
-                'type': 'string',
-            }
-        },
+        'type': 'object',
         'properties': {
             'pikalias': {
-                'allOf': [{'$ref': '#/$defs/FooBarEnum'}],
-                'description': 'Pika is definitely the best!',
                 'title': 'Pikapika!',
+                'description': 'Pika is definitely the best!',
+                'allOf': [{'$ref': '#/$defs/FooBarEnum'}],
             },
             'bulbialias': {
                 'allOf': [{'$ref': '#/$defs/FooBarEnum'}],
-                'description': 'Bulbi is not...',
-                'title': 'Bulbibulbi!',
                 'default': 'foo',
+                'title': 'Bulbibulbi!',
+                'description': 'Bulbi is not...',
             },
             'cara': {'$ref': '#/$defs/FooBarEnum'},
         },
         'required': ['pikalias', 'cara'],
         'title': 'Model',
-        'type': 'object',
+        '$defs': {'FooBarEnum': {'enum': ['foo', 'bar'], 'title': 'FooBarEnum', 'type': 'string'}},
     }
 
 
 def test_enum_and_model_have_same_behaviour():
     class Names(str, Enum):
         rick = 'Rick'
         morty = 'Morty'
@@ -362,45 +361,42 @@
         model: Pika
         titled_model: Pika = Field(
             ...,
             title='Title of model',
             description='Description of model',
         )
 
+    # insert_assert(Foo.model_json_schema())
     assert Foo.model_json_schema() == {
-        '$defs': {
-            'Pika': {
-                'properties': {'a': {'title': 'A', 'type': 'string'}},
-                'required': ['a'],
-                'title': 'Pika',
-                'type': 'object',
-            },
-            'Names': {
-                'enum': ['Rick', 'Morty', 'Summer'],
-                'title': 'Names',
-                'type': 'string',
-            },
-        },
+        'type': 'object',
         'properties': {
             'enum': {'$ref': '#/$defs/Names'},
-            'model': {'$ref': '#/$defs/Pika'},
             'titled_enum': {
-                'allOf': [{'$ref': '#/$defs/Names'}],
-                'description': 'Description of enum',
                 'title': 'Title of enum',
+                'description': 'Description of enum',
+                'allOf': [{'$ref': '#/$defs/Names'}],
             },
+            'model': {'$ref': '#/$defs/Pika'},
             'titled_model': {
-                'allOf': [{'$ref': '#/$defs/Pika'}],
-                'description': 'Description of model',
                 'title': 'Title of model',
+                'description': 'Description of model',
+                'allOf': [{'$ref': '#/$defs/Pika'}],
             },
         },
         'required': ['enum', 'titled_enum', 'model', 'titled_model'],
         'title': 'Foo',
-        'type': 'object',
+        '$defs': {
+            'Names': {'enum': ['Rick', 'Morty', 'Summer'], 'title': 'Names', 'type': 'string'},
+            'Pika': {
+                'type': 'object',
+                'properties': {'a': {'type': 'string', 'title': 'A'}},
+                'required': ['a'],
+                'title': 'Pika',
+            },
+        },
     }
 
 
 def test_enum_includes_extra_without_other_params():
     class Names(str, Enum):
         rick = 'Rick'
         morty = 'Morty'
@@ -632,29 +628,33 @@
                 'maxItems': 4,
             },
         ),
         (Tuple[str], {'prefixItems': [{'type': 'string'}], 'minItems': 1, 'maxItems': 1}),
         (Tuple[()], {'maxItems': 0, 'minItems': 0}),
         (
             Tuple[str, ...],
-            {'items': {'type': 'string'}, 'title': 'A', 'type': 'array'},
+            {'items': {'type': 'string'}, 'type': 'array'},
         ),
     ],
 )
 def test_tuple(field_type, extra_props):
     class Model(BaseModel):
         a: field_type
 
     assert Model.model_json_schema() == {
         'title': 'Model',
         'type': 'object',
         'properties': {'a': {'title': 'A', 'type': 'array', **extra_props}},
         'required': ['a'],
     }
 
+    ta = TypeAdapter(field_type)
+
+    assert ta.json_schema() == {'type': 'array', **extra_props}
+
 
 def test_deque():
     class Model(BaseModel):
         a: Deque[str]
 
     assert Model.model_json_schema() == {
         'title': 'Model',
@@ -1654,14 +1654,30 @@
         },
         'properties': {'inner': {'allOf': [{'$ref': '#/$defs/Inner'}], 'default': {'a': {'.': ''}}}},
         'title': 'Outer',
         'type': 'object',
     }
 
 
+def test_model_subclass_metadata():
+    class A(BaseModel):
+        """A Model docstring"""
+
+    class B(A):
+        pass
+
+    assert A.model_json_schema() == {
+        'title': 'A',
+        'description': 'A Model docstring',
+        'type': 'object',
+        'properties': {},
+    }
+    assert B.model_json_schema() == {'title': 'B', 'type': 'object', 'properties': {}}
+
+
 @pytest.mark.parametrize(
     'kwargs,type_,expected_extra',
     [
         ({'max_length': 5}, str, {'type': 'string', 'maxLength': 5}),
         ({}, constr(max_length=6), {'type': 'string', 'maxLength': 6}),
         ({'min_length': 2}, str, {'type': 'string', 'minLength': 2}),
         ({'max_length': 5}, bytes, {'type': 'string', 'maxLength': 5, 'format': 'binary'}),
@@ -2081,14 +2097,126 @@
         'type': 'object',
         'properties': {'a': {'title': 'A', 'type': 'string'}},
         'required': ['a'],
         'additionalProperties': False,
     }
 
 
+def test_model_with_extra_allow():
+    class Model(BaseModel):
+        model_config = ConfigDict(extra='allow')
+        a: str
+
+    assert Model.model_json_schema() == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {'a': {'title': 'A', 'type': 'string'}},
+        'required': ['a'],
+        'additionalProperties': True,
+    }
+
+
+def test_model_with_extra_ignore():
+    class Model(BaseModel):
+        model_config = ConfigDict(extra='ignore')
+        a: str
+
+    assert Model.model_json_schema() == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {'a': {'title': 'A', 'type': 'string'}},
+        'required': ['a'],
+    }
+
+
+def test_dataclass_with_extra_allow():
+    @pydantic.dataclasses.dataclass
+    class Model:
+        __pydantic_config__ = ConfigDict(extra='allow')
+        a: str
+
+    assert TypeAdapter(Model).json_schema() == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {'a': {'title': 'A', 'type': 'string'}},
+        'required': ['a'],
+        'additionalProperties': True,
+    }
+
+
+def test_dataclass_with_extra_ignore():
+    @pydantic.dataclasses.dataclass
+    class Model:
+        __pydantic_config__ = ConfigDict(extra='ignore')
+        a: str
+
+    assert TypeAdapter(Model).json_schema() == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {'a': {'title': 'A', 'type': 'string'}},
+        'required': ['a'],
+    }
+
+
+def test_dataclass_with_extra_forbid():
+    @pydantic.dataclasses.dataclass
+    class Model:
+        __pydantic_config__ = ConfigDict(extra='ignore')
+        a: str
+
+    assert TypeAdapter(Model).json_schema() == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {'a': {'title': 'A', 'type': 'string'}},
+        'required': ['a'],
+    }
+
+
+def test_typeddict_with_extra_allow():
+    class Model(TypedDict):
+        __pydantic_config__ = ConfigDict(extra='allow')  # type: ignore
+        a: str
+
+    assert TypeAdapter(Model).json_schema() == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {'a': {'title': 'A', 'type': 'string'}},
+        'required': ['a'],
+        'additionalProperties': True,
+    }
+
+
+def test_typeddict_with_extra_ignore():
+    class Model(TypedDict):
+        __pydantic_config__ = ConfigDict(extra='ignore')  # type: ignore
+        a: str
+
+    assert TypeAdapter(Model).json_schema() == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {'a': {'title': 'A', 'type': 'string'}},
+        'required': ['a'],
+    }
+
+
+def test_typeddict_with_extra_forbid():
+    @pydantic.dataclasses.dataclass
+    class Model:
+        __pydantic_config__ = ConfigDict(extra='forbid')
+        a: str
+
+    assert TypeAdapter(Model).json_schema() == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {'a': {'title': 'A', 'type': 'string'}},
+        'required': ['a'],
+        'additionalProperties': False,
+    }
+
+
 @pytest.mark.parametrize(
     'annotation,kwargs,field_schema',
     [
         (int, dict(gt=0), {'title': 'A', 'exclusiveMinimum': 0, 'type': 'integer'}),
         (
             Optional[int],
             dict(gt=0),
@@ -2272,15 +2400,15 @@
     }
 
 
 def test_path_modify_schema():
     class MyPath(Path):
         @classmethod
         def __get_pydantic_core_schema__(cls, _source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
-            return handler.generate_schema(Path)
+            return handler(Path)
 
         @classmethod
         def __get_pydantic_json_schema__(
             cls, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
         ) -> JsonSchemaValue:
             schema = handler(core_schema)
             schema.update(foobar=123)
@@ -2705,61 +2833,53 @@
         # check Tuple because changes in code touch that type
         data3: Tuple
         data4: Tuple[CustomType]
         data5: Tuple[CustomType, str]
 
         model_config = {'arbitrary_types_allowed': True}
 
+    # insert_assert(Model.model_json_schema())
     assert Model.model_json_schema() == {
-        'title': 'Model',
-        'type': 'object',
+        '$defs': {'CustomType': {'enum': ['a', 'b'], 'title': 'CustomType'}},
         'properties': {
             'data0': {
                 'anyOf': [{'type': 'string'}, {'items': {'type': 'string'}, 'type': 'array'}],
                 'title': 'Gen title',
             },
             'data1': {
-                'title': 'Data1 title',
+                'anyOf': [{'$ref': '#/$defs/CustomType'}, {'items': {'$ref': '#/$defs/CustomType'}, 'type': 'array'}],
                 'description': 'Data 1 description',
-                'anyOf': [
-                    {'$ref': '#/$defs/CustomType'},
-                    {'type': 'array', 'items': {'$ref': '#/$defs/CustomType'}},
-                ],
+                'title': 'Data1 title',
             },
             'data2': {
                 'description': 'Data 2',
                 'examples': 'examples',
                 'prefixItems': [{'$ref': '#/$defs/CustomType'}, {'format': 'uuid4', 'type': 'string'}],
                 'title': 'Data2 title',
                 'type': 'array',
             },
-            'data3': {'title': 'Data3', 'type': 'array', 'items': {}},
+            'data3': {'items': {}, 'title': 'Data3', 'type': 'array'},
             'data4': {
+                'maxItems': 1,
+                'minItems': 1,
+                'prefixItems': [{'$ref': '#/$defs/CustomType'}],
                 'title': 'Data4',
                 'type': 'array',
-                'prefixItems': [{'$ref': '#/$defs/CustomType'}],
-                'minItems': 1,
-                'maxItems': 1,
             },
             'data5': {
+                'maxItems': 2,
+                'minItems': 2,
+                'prefixItems': [{'$ref': '#/$defs/CustomType'}, {'type': 'string'}],
                 'title': 'Data5',
                 'type': 'array',
-                'prefixItems': [{'$ref': '#/$defs/CustomType'}, {'type': 'string'}],
-                'minItems': 2,
-                'maxItems': 2,
             },
         },
         'required': ['data0', 'data1', 'data2', 'data3', 'data4', 'data5'],
-        '$defs': {
-            'CustomType': {
-                'title': 'CustomType title',
-                'enum': ['a', 'b'],
-                'type': 'string',
-            }
-        },
+        'title': 'Model',
+        'type': 'object',
     }
 
 
 def test_nested_generic():
     """
     Test a nested BaseModel that is also a Generic
     """
@@ -3157,33 +3277,34 @@
 
     Pet = Annotated[Union[Cat, Dog], Field(discriminator='pet_type')]
 
     class Model(BaseModel):
         pet: Pet
         number: int
 
+    # insert_assert(Model.model_json_schema())
     assert Model.model_json_schema() == {
         '$defs': {
             'BlackCatWithHeight': {
                 'properties': {
-                    'black_infos': {'title': 'Black ' 'Infos', 'type': 'string'},
+                    'black_infos': {'title': 'Black Infos', 'type': 'string'},
                     'color': {'const': 'black', 'title': 'Color'},
                     'info': {'const': 'height', 'title': 'Info'},
-                    'pet_type': {'const': 'cat', 'title': 'Pet ' 'Type'},
+                    'pet_type': {'const': 'cat', 'title': 'Pet Type'},
                 },
                 'required': ['pet_type', 'color', 'info', 'black_infos'],
                 'title': 'BlackCatWithHeight',
                 'type': 'object',
             },
             'BlackCatWithWeight': {
                 'properties': {
-                    'black_infos': {'title': 'Black ' 'Infos', 'type': 'string'},
+                    'black_infos': {'title': 'Black Infos', 'type': 'string'},
                     'color': {'const': 'black', 'title': 'Color'},
                     'info': {'const': 'weight', 'title': 'Info'},
-                    'pet_type': {'const': 'cat', 'title': 'Pet ' 'Type'},
+                    'pet_type': {'const': 'cat', 'title': 'Pet Type'},
                 },
                 'required': ['pet_type', 'color', 'info', 'black_infos'],
                 'title': 'BlackCatWithWeight',
                 'type': 'object',
             },
             'Dog': {
                 'properties': {
@@ -3340,33 +3461,34 @@
 
     Pet = Annotated[Union[Cat, Dog], Field(discriminator='pet_type')]
 
     class Model(BaseModel):
         pet: Pet
         number: int
 
+    # insert_assert(Model.model_json_schema())
     assert Model.model_json_schema() == {
         '$defs': {
             'BlackCatWithHeight': {
                 'properties': {
-                    'black_infos': {'title': 'Black ' 'Infos', 'type': 'string'},
+                    'black_infos': {'title': 'Black Infos', 'type': 'string'},
                     'color': {'const': 'black', 'title': 'Color'},
                     'info': {'const': 0, 'title': 'Info'},
-                    'pet_type': {'const': 'cat', 'title': 'Pet ' 'Type'},
+                    'pet_type': {'const': 'cat', 'title': 'Pet Type'},
                 },
                 'required': ['pet_type', 'color', 'info', 'black_infos'],
                 'title': 'BlackCatWithHeight',
                 'type': 'object',
             },
             'BlackCatWithWeight': {
                 'properties': {
-                    'black_infos': {'title': 'Black ' 'Infos', 'type': 'string'},
+                    'black_infos': {'title': 'Black Infos', 'type': 'string'},
                     'color': {'const': 'black', 'title': 'Color'},
                     'info': {'const': 1, 'title': 'Info'},
-                    'pet_type': {'const': 'cat', 'title': 'Pet ' 'Type'},
+                    'pet_type': {'const': 'cat', 'title': 'Pet Type'},
                 },
                 'required': ['pet_type', 'color', 'info', 'black_infos'],
                 'title': 'BlackCatWithWeight',
                 'type': 'object',
             },
             'Dog': {
                 'properties': {
@@ -3476,41 +3598,30 @@
         },
         'required': ['pet', 'number'],
         'title': 'Model',
         'type': 'object',
     }
 
 
+@pytest.mark.xfail(reason='json schema generation for tagged unions is fundamentally incompatible with references')
 def test_alias_same():
     class Cat(BaseModel):
         pet_type: Literal['cat'] = Field(alias='typeOfPet')
         c: str
 
     class Dog(BaseModel):
         pet_type: Literal['dog'] = Field(alias='typeOfPet')
         d: str
 
     class Model(BaseModel):
         pet: Union[Cat, Dog] = Field(discriminator='pet_type')
         number: int
 
+    # insert_assert(Model.model_json_schema())
     assert Model.model_json_schema() == {
-        'type': 'object',
-        'title': 'Model',
-        'properties': {
-            'number': {'title': 'Number', 'type': 'integer'},
-            'pet': {
-                'discriminator': {
-                    'mapping': {'cat': '#/$defs/Cat', 'dog': '#/$defs/Dog'},
-                    'propertyName': 'typeOfPet',
-                },
-                'oneOf': [{'$ref': '#/$defs/Cat'}, {'$ref': '#/$defs/Dog'}],
-                'title': 'Pet',
-            },
-        },
         '$defs': {
             'Cat': {
                 'properties': {
                     'c': {'title': 'C', 'type': 'string'},
                     'typeOfPet': {'const': 'cat', 'title': 'Typeofpet'},
                 },
                 'required': ['typeOfPet', 'c'],
@@ -3523,15 +3634,25 @@
                     'typeOfPet': {'const': 'dog', 'title': 'Typeofpet'},
                 },
                 'required': ['typeOfPet', 'd'],
                 'title': 'Dog',
                 'type': 'object',
             },
         },
+        'properties': {
+            'number': {'title': 'Number', 'type': 'integer'},
+            'pet': {
+                'oneOf': [{'$ref': '#/$defs/Cat'}, {'$ref': '#/$defs/Dog'}],
+                'title': 'Pet',
+                'discriminator': 'something',
+            },
+        },
         'required': ['pet', 'number'],
+        'title': 'Model',
+        'type': 'object',
     }
 
 
 def test_nested_python_dataclasses():
     """
     Test schema generation for nested python dataclasses
     """
@@ -4258,22 +4379,36 @@
             x: Annotated[ArbitraryClass, WithJsonSchema(field_schema)]
 
     assert Model.model_json_schema() == model_schema
 
 
 def test_root_model():
     class A(RootModel[int]):
-        pass
+        """A Model docstring"""
 
-    assert A.model_json_schema() == {'type': 'integer'}
+    assert A.model_json_schema() == {'title': 'A', 'description': 'A Model docstring', 'type': 'integer'}
 
     class B(RootModel[A]):
         pass
 
-    assert B.model_json_schema() == {'type': 'integer'}
+    assert B.model_json_schema() == {
+        '$defs': {'A': {'description': 'A Model docstring', 'title': 'A', 'type': 'integer'}},
+        'allOf': [{'$ref': '#/$defs/A'}],
+        'title': 'B',
+    }
+
+    class C(RootModel[A]):
+        """C Model docstring"""
+
+    assert C.model_json_schema() == {
+        '$defs': {'A': {'description': 'A Model docstring', 'title': 'A', 'type': 'integer'}},
+        'allOf': [{'$ref': '#/$defs/A'}],
+        'title': 'C',
+        'description': 'C Model docstring',
+    }
 
 
 def test_get_json_schema_is_passed_the_same_schema_handler_was_called_with() -> None:
     class CustomInt(int):
         @classmethod
         def __get_pydantic_core_schema__(cls, _source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
             return handler(int)
@@ -4349,24 +4484,14 @@
 def test_build_metadata_dict_initial_metadata():
     assert build_metadata_dict(initial_metadata={'foo': 'bar'}) == {'foo': 'bar', 'pydantic_js_functions': []}
 
     with pytest.raises(TypeError, match=re.escape("CoreSchema metadata should be a dict; got 'test'.")):
         build_metadata_dict(initial_metadata='test')
 
 
-def test_core_metadata_get_json_schema():
-    core_metadata_handler = CoreMetadataHandler({})
-    assert core_metadata_handler.get_json_schema({}, lambda c: c) == {}
-
-    core_metadata_handler = CoreMetadataHandler(
-        {'metadata': {'pydantic_js_function': lambda c, h: f'schema = {c}, {h.__name__}'}}
-    )
-    assert core_metadata_handler.get_json_schema({'foo': 'bar'}, lambda c: c) == "schema = {'foo': 'bar'}, <lambda>"
-
-
 def test_type_adapter_json_schemas_title_description():
     class Model(BaseModel):
         a: str
 
     _, json_schema = TypeAdapter.json_schemas([(Model, 'validation', TypeAdapter(Model))])
     assert 'title' not in json_schema
     assert 'description' not in json_schema
@@ -4443,7 +4568,170 @@
 
     assert Model.model_json_schema() == {
         'properties': {'a': {'title': 'A', 'type': 'integer'}},
         'required': ['a'],
         'title': 'Model',
         'type': 'object',
     }
+
+
+@pytest.mark.xfail(reason='Need to fix JSON schema customization for Enum')
+def test_override_enum_json_schema():
+    class CustomType(Enum):
+        A = 'a'
+        B = 'b'
+
+        @classmethod
+        def __get_pydantic_json_schema__(
+            cls, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+        ) -> core_schema.CoreSchema:
+            json_schema = handler(core_schema)
+            json_schema.update(title='CustomType title', type='string')
+            return json_schema
+
+    class Model(BaseModel):
+        x: CustomType
+
+    assert Model.model_json_schema() == {
+        'type': 'object',
+        'properties': {'x': {'$ref': '#/$defs/CustomType'}},
+        'required': ['x'],
+        'title': 'Model',
+        '$defs': {
+            'CustomType': {
+                'enum': ['a', 'b'],
+                'title': 'CustomType title',  # <----------- this is not getting set properly
+            }
+        },
+    }
+
+
+def test_json_schema_extras_on_ref() -> None:
+    @dataclass
+    class JsonSchemaExamples:
+        examples: Dict[str, Any]
+
+        def __get_pydantic_json_schema__(
+            self, core_schema: CoreSchema, handler: GetJsonSchemaHandler
+        ) -> JsonSchemaValue:
+            json_schema = handler(core_schema)
+            assert json_schema.keys() == {'$ref'}
+            json_schema['examples'] = to_json(self.examples)
+            return json_schema
+
+    @dataclass
+    class JsonSchemaTitle:
+        title: str
+
+        def __get_pydantic_json_schema__(
+            self, core_schema: CoreSchema, handler: GetJsonSchemaHandler
+        ) -> JsonSchemaValue:
+            json_schema = handler(core_schema)
+            assert json_schema.keys() == {'allOf', 'examples'}
+            json_schema['title'] = self.title
+            return json_schema
+
+    class Model(BaseModel):
+        name: str
+        age: int
+
+    ta = TypeAdapter(
+        Annotated[Model, JsonSchemaExamples({'foo': Model(name='John', age=28)}), JsonSchemaTitle('ModelTitle')]
+    )
+
+    # insert_assert(ta.json_schema())
+    assert ta.json_schema() == {
+        '$defs': {
+            'Model': {
+                'properties': {'age': {'title': 'Age', 'type': 'integer'}, 'name': {'title': 'Name', 'type': 'string'}},
+                'required': ['name', 'age'],
+                'title': 'Model',
+                'type': 'object',
+            }
+        },
+        'allOf': [{'$ref': '#/$defs/Model'}],
+        'examples': b'{"foo":{"name":"John","age":28}}',
+        'title': 'ModelTitle',
+    }
+
+
+def test_inclusion_of_defaults():
+    class Model(BaseModel):
+        x: int = 1
+        y: int = Field(default_factory=lambda: 2)
+
+    assert Model.model_json_schema() == {
+        'properties': {'x': {'default': 1, 'title': 'X', 'type': 'integer'}, 'y': {'title': 'Y', 'type': 'integer'}},
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
+def test_resolve_def_schema_from_core_schema() -> None:
+    class Inner(BaseModel):
+        x: int
+
+    class Marker:
+        def __get_pydantic_json_schema__(
+            self, core_schema: CoreSchema, handler: GetJsonSchemaHandler
+        ) -> JsonSchemaValue:
+            field_schema = handler(core_schema)
+            field_schema['title'] = 'Foo'
+            original_schema = handler.resolve_ref_schema(field_schema)
+            original_schema['title'] = 'Bar'
+            return field_schema
+
+    class Outer(BaseModel):
+        inner: Annotated[Inner, Marker()]
+
+    # insert_assert(Outer.model_json_schema())
+    assert Outer.model_json_schema() == {
+        '$defs': {
+            'Inner': {
+                'properties': {'x': {'title': 'X', 'type': 'integer'}},
+                'required': ['x'],
+                'title': 'Bar',
+                'type': 'object',
+            }
+        },
+        'properties': {'inner': {'allOf': [{'$ref': '#/$defs/Inner'}], 'title': 'Foo'}},
+        'required': ['inner'],
+        'title': 'Outer',
+        'type': 'object',
+    }
+
+
+def test_examples_annotation() -> None:
+    ListWithExamples = Annotated[
+        List[float],
+        Examples({'Fibonacci': [1, 1, 2, 3, 5]}),
+    ]
+
+    ta = TypeAdapter(ListWithExamples)
+
+    # insert_assert(ta.json_schema())
+    assert ta.json_schema() == {
+        'examples': {'Fibonacci': [1, 1, 2, 3, 5]},
+        'items': {'type': 'number'},
+        'type': 'array',
+    }
+
+    ListWithMoreExamples = Annotated[
+        ListWithExamples,
+        Examples(
+            {
+                'Constants': [
+                    3.14,
+                    2.71,
+                ]
+            }
+        ),
+    ]
+
+    ta = TypeAdapter(ListWithMoreExamples)
+
+    # insert_assert(ta.json_schema())
+    assert ta.json_schema() == {
+        'examples': {'Constants': [3.14, 2.71], 'Fibonacci': [1, 1, 2, 3, 5]},
+        'items': {'type': 'number'},
+        'type': 'array',
+    }
```

### Comparing `pydantic-2.0b2/tests/test_main.py` & `pydantic-2.0b3/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import platform
 import re
 import sys
+from collections import defaultdict
 from copy import deepcopy
 from dataclasses import dataclass
 from enum import Enum
 from typing import (
     Any,
     Callable,
     ClassVar,
@@ -18,15 +19,15 @@
     Type,
     TypeVar,
     get_type_hints,
 )
 from uuid import UUID, uuid4
 
 import pytest
-from pydantic_core import CoreSchema
+from pydantic_core import CoreSchema, core_schema
 from typing_extensions import Annotated, Final, Literal
 
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
     GetCoreSchemaHandler,
@@ -35,14 +36,15 @@
     PydanticUserError,
     SecretStr,
     ValidationError,
     ValidationInfo,
     constr,
     field_validator,
 )
+from pydantic.type_adapter import TypeAdapter
 
 
 def test_success():
     # same as below but defined here so class definition occurs inside the test
     class Model(BaseModel):
         a: float
         b: int = 10
@@ -2348,7 +2350,169 @@
             ModelFromAttributesFalse.model_validate(UnrelatedClass(), from_attributes=from_attributes)
         assert exc_info.value.errors(include_url=False) == [
             {'type': 'dict_type', 'loc': (), 'msg': 'Input should be a valid dictionary', 'input': input}
         ]
 
     res = ModelFromAttributesFalse.model_validate(UnrelatedClass(), from_attributes=True)
     assert res == ModelFromAttributesFalse(x=1)
+
+
+def test_model_signature_annotated() -> None:
+    class Model(BaseModel):
+        x: Annotated[int, 123]
+
+    # we used to accidentally convert `__metadata__` to a list
+    # which caused things like `typing.get_args()` to fail
+    assert Model.__signature__.parameters['x'].annotation.__metadata__ == (123,)
+
+
+def test_get_core_schema_unpacks_refs_for_source_type() -> None:
+    # use a list to track since we end up calling `__get_pydantic_core_schema__` multiple times for models
+    # e.g. InnerModel.__get_pydantic_core_schema__ gets called:
+    # 1. When InnerModel is defined
+    # 2. When OuterModel is defined
+    # 3. When we use the TypeAdapter
+    received_schemas: dict[str, list[str]] = defaultdict(list)
+
+    @dataclass
+    class Marker:
+        name: str
+
+        def __get_pydantic_core_schema__(self, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            schema = handler(source_type)
+            received_schemas[self.name].append(schema['type'])
+            return schema
+
+    class InnerModel(BaseModel):
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            schema = handler(source_type)
+            received_schemas['InnerModel'].append(schema['type'])
+            schema['metadata'] = schema.get('metadata', {})
+            schema['metadata']['foo'] = 'inner was here!'
+            return deepcopy(schema)
+
+    class OuterModel(BaseModel):
+        inner: Annotated[InnerModel, Marker('Marker("inner")')]
+
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            schema = handler(source_type)
+            received_schemas['OuterModel'].append(schema['type'])
+            return schema
+
+    ta = TypeAdapter(Annotated[OuterModel, Marker('Marker("outer")')])
+
+    # super hacky check but it works in all cases and avoids a complex and fragile iteration over CoreSchema
+    # the point here is to verify that `__get_pydantic_core_schema__`
+    assert 'inner was here' in str(ta.core_schema)
+
+    assert received_schemas == {
+        'InnerModel': ['model', 'model', 'model'],
+        'Marker("inner")': ['definition-ref', 'definition-ref'],
+        'OuterModel': ['model', 'model'],
+        'Marker("outer")': ['definition-ref'],
+    }
+
+
+def test_get_core_schema_return_new_ref() -> None:
+    class InnerModel(BaseModel):
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            schema = handler(source_type)
+            schema = deepcopy(schema)
+            schema['metadata'] = schema.get('metadata', {})
+            schema['metadata']['foo'] = 'inner was here!'
+            return deepcopy(schema)
+
+    class OuterModel(BaseModel):
+        inner: InnerModel
+        x: int = 1
+
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            schema = handler(source_type)
+
+            def set_x(m: 'OuterModel') -> 'OuterModel':
+                m.x += 1
+                return m
+
+            return core_schema.no_info_after_validator_function(set_x, schema, ref=schema.pop('ref'))
+
+    cs = OuterModel.__pydantic_core_schema__
+    # super hacky check but it works in all cases and avoids a complex and fragile iteration over CoreSchema
+    # the point here is to verify that `__get_pydantic_core_schema__`
+    assert 'inner was here' in str(cs)
+
+    assert OuterModel(inner=InnerModel()).x == 2
+
+
+def test_resolve_def_schema_from_core_schema() -> None:
+    class Inner(BaseModel):
+        x: int
+
+    class Marker:
+        def __get_pydantic_core_schema__(self, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            schema = handler(source_type)
+            resolved = handler.resolve_ref_schema(schema)
+            assert resolved['type'] == 'model'
+            assert resolved['cls'] is Inner
+
+            def modify_inner(v: Inner) -> Inner:
+                v.x += 1
+                return v
+
+            return core_schema.no_info_after_validator_function(modify_inner, schema)
+
+    class Outer(BaseModel):
+        inner: Annotated[Inner, Marker()]
+
+    assert Outer.model_validate({'inner': {'x': 1}}).inner.x == 2
+
+
+def test_extra_validator_scalar() -> None:
+    class Model(BaseModel):
+        model_config = ConfigDict(extra='allow')
+
+    class Child(Model):
+        __pydantic_extra__: Dict[str, int]
+
+    m = Child(a='1')
+    assert m.__pydantic_extra__ == {'a': 1}
+
+    # insert_assert(Child.model_json_schema())
+    assert Child.model_json_schema() == {
+        'additionalProperties': {'type': 'integer'},
+        'properties': {},
+        'title': 'Child',
+        'type': 'object',
+    }
+
+
+def test_extra_validator_named() -> None:
+    class Foo(BaseModel):
+        x: int
+
+    class Model(BaseModel):
+        model_config = ConfigDict(extra='allow')
+
+    class Child(Model):
+        __pydantic_extra__: Dict[str, Foo]
+
+    m = Child(a={'x': '1'})
+    assert m.__pydantic_extra__ == {'a': Foo(x=1)}
+
+    # insert_assert(Child.model_json_schema())
+    assert Child.model_json_schema() == {
+        '$defs': {
+            'Foo': {
+                'properties': {'x': {'title': 'X', 'type': 'integer'}},
+                'required': ['x'],
+                'title': 'Foo',
+                'type': 'object',
+            }
+        },
+        'additionalProperties': {'$ref': '#/$defs/Foo'},
+        'properties': {},
+        'title': 'Child',
+        'type': 'object',
+    }
```

### Comparing `pydantic-2.0b2/tests/test_migration.py` & `pydantic-2.0b3/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_model_signature.py` & `pydantic-2.0b3/tests/test_model_signature.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_model_validator.py` & `pydantic-2.0b3/tests/test_model_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_networks.py` & `pydantic-2.0b3/tests/test_networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -747,14 +747,16 @@
         ('foo.bar@exam-ple.com ', 'foo.bar', 'foo.bar@exam-ple.com'),
         ('ιωάννης@εεττ.gr', 'ιωάννης', 'ιωάννης@εεττ.gr'),
         ('foobar@аррӏе.com', 'foobar', 'foobar@аррӏе.com'),
         ('foobar@xn--80ak6aa92e.com', 'foobar', 'foobar@аррӏе.com'),
         ('аррӏе@example.com', 'аррӏе', 'аррӏе@example.com'),
         ('xn--80ak6aa92e@example.com', 'xn--80ak6aa92e', 'xn--80ak6aa92e@example.com'),
         ('葉士豪@臺網中心.tw', '葉士豪', '葉士豪@臺網中心.tw'),
+        ('"first.last" <first.last@example.com>', 'first.last', 'first.last@example.com'),
+        ("Shaquille O'Neal <shaq@example.com>", "Shaquille O'Neal", 'shaq@example.com'),
     ],
 )
 def test_address_valid(value, name, email):
     assert validate_email(value) == (name, email)
 
 
 @pytest.mark.skipif(not email_validator, reason='email_validator not installed')
@@ -781,14 +783,15 @@
         ('"@example.com', None),
         ('\"@example.com', None),
         (',@example.com', None),
         ('foobar <foobar<@example.com>', None),
         ('foobar <foobar@example.com>>', None),
         ('foobar <<foobar<@example.com>', None),
         ('foobar <>', None),
+        ('first.last <first.last@example.com>', None),
     ],
 )
 def test_address_invalid(value, reason):
     with pytest.raises(PydanticCustomError, match=f'value is not a valid email address: {reason or ""}'):
         validate_email(value)
```

### Comparing `pydantic-2.0b2/tests/test_networks_ipaddress.py` & `pydantic-2.0b3/tests/test_networks_ipaddress.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_parse.py` & `pydantic-2.0b3/tests/test_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import List, Tuple
 
 import pytest
+from pydantic_core import CoreSchema
 
-from pydantic import BaseModel, ValidationError, model_validator, parse_obj_as
+from pydantic import BaseModel, GetJsonSchemaHandler, ValidationError, model_validator, parse_obj_as
 from pydantic.functional_serializers import model_serializer
+from pydantic.json_schema import JsonSchemaValue
 
 
 class Model(BaseModel):
     a: float
     b: int = 10
 
 
@@ -72,17 +74,20 @@
             data = handler(self)
             if info.mode == 'json':
                 return data['root']
             else:
                 return data
 
         @classmethod
-        def __get_pydantic_json_schema__(cls, core_schema, handler):
+        def __get_pydantic_json_schema__(
+            cls, core_schema: CoreSchema, handler: GetJsonSchemaHandler
+        ) -> JsonSchemaValue:
             json_schema = handler(core_schema)
-            return json_schema['properties']['root']
+            root = handler.resolve_ref_schema(json_schema)['properties']['root']
+            return root
 
     # Validation
     m = MyModel.model_validate('a')
     assert m.root == 'a'
 
     # Serialization
     assert m.model_dump() == {'root': 'a'}
```

### Comparing `pydantic-2.0b2/tests/test_prepare_annotations.py` & `pydantic-2.0b3/tests/test_prepare_annotations.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_private_attributes.py` & `pydantic-2.0b3/tests/test_private_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,21 +281,21 @@
         model_config = ConfigDict(ignored_types=(IgnoredType,))
 
         _a = IgnoredType()
         _b: int = IgnoredType()
         _c: IgnoredType
         _d: IgnoredType = IgnoredType()
 
-        # The following are included to document existing behavior, and can be updated
-        # if the current behavior does not match the desired behavior
+        # The following are included to document existing behavior, which is to make them into PrivateAttrs
+        # this can be updated if the current behavior is not the desired behavior
         _e: int
         _f: int = 1
-        _g = 1  # Note: this is completely ignored, in keeping with v1
+        _g = 1
 
-    assert sorted(MyModel.__private_attributes__.keys()) == ['_e', '_f']
+    assert sorted(MyModel.__private_attributes__.keys()) == ['_e', '_f', '_g']
 
 
 @pytest.mark.skipif(not hasattr(functools, 'cached_property'), reason='cached_property is not available')
 def test_ignored_types_are_ignored_cached_property():
     """Demonstrate the members of functools are ignore here as with fields."""
 
     class MyModel(BaseModel):
@@ -335,7 +335,21 @@
     m = NewModel()
     m._mixin_private = 1
     m._private = 2
 
     assert m.__pydantic_private__ == {'_mixin_private': 1, '_private': 2}
     assert m._mixin_private == 1
     assert m._private == 2
+
+
+def test_unannotated_private_attr():
+    from pydantic import BaseModel, PrivateAttr
+
+    class A(BaseModel):
+        _x = PrivateAttr()
+        _y = 52
+
+    a = A()
+    assert a._y == 52
+    assert a.__pydantic_private__ == {'_y': 52}
+    a._x = 1
+    assert a.__pydantic_private__ == {'_x': 1, '_y': 52}
```

### Comparing `pydantic-2.0b2/tests/test_rich_repr.py` & `pydantic-2.0b3/tests/test_rich_repr.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,12 +26,13 @@
         ('id', 22),
         ('name', 'John Doe'),
         ('signup_ts', None),
         ('friends', []),
     ]
 
 
+@pytest.mark.filterwarnings('ignore::DeprecationWarning')
 def test_rich_repr_color(User):
     color = Color((10, 20, 30, 0.1))
     rich_repr = list(color.__rich_repr__())
 
     assert rich_repr == ['#0a141e1a', ('rgb', (10, 20, 30, 0.1))]
```

### Comparing `pydantic-2.0b2/tests/test_root_model.py` & `pydantic-2.0b3/tests/test_root_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, List, Optional
 
 import pytest
+from pydantic_core import CoreSchema
 from pydantic_core.core_schema import SerializerFunctionWrapHandler
 
 from pydantic import (
     Base64Str,
     BaseModel,
     ConfigDict,
     Field,
@@ -35,36 +36,46 @@
                 {'int_field': 42, 'str_field': 'forty two'},
                 id='InnerModel',
             ),
         ],
     )
 
 
+def check_schema(schema: CoreSchema) -> None:
+    # we assume the shape of the core schema here, which is not a guarantee
+    # pydantic makes to it's users but is useful to check here to make sure
+    # we are doing the right thing internally
+    assert schema['type'] == 'definitions'
+    inner = schema['schema']
+    assert inner['type'] == 'definition-ref'
+    ref = inner['schema_ref']  # type: ignore
+    schema = next(s for s in schema['definitions'] if s['ref'] == ref)  # type: ignore
+    assert schema['type'] == 'model'
+    assert schema['root_model'] is True
+    assert schema['custom_init'] is False
+
+
 @parametrize_root_model()
 def test_root_model_specialized(root_type, root_value, dump_value):
     Model = RootModel[root_type]
 
-    assert Model.__pydantic_core_schema__['type'] == 'model'
-    assert Model.__pydantic_core_schema__['root_model'] is True
-    assert Model.__pydantic_core_schema__['custom_init'] is False
+    check_schema(Model.__pydantic_core_schema__)
 
     m = Model(root_value)
 
     assert m.model_dump() == dump_value
     assert dict(m) == {'root': m.root}
 
 
 @parametrize_root_model()
 def test_root_model_inherited(root_type, root_value, dump_value):
     class Model(RootModel[root_type]):
         pass
 
-    assert Model.__pydantic_core_schema__['type'] == 'model'
-    assert Model.__pydantic_core_schema__['root_model'] is True
-    assert Model.__pydantic_core_schema__['custom_init'] is False
+    check_schema(Model.__pydantic_core_schema__)
 
     m = Model(root_value)
 
     assert m.model_dump() == dump_value
     assert dict(m) == {'root': m.root}
 
 
@@ -386,7 +397,24 @@
         root: int = 42
 
     class Model(BaseModel):
         value: Nested = Field(default_factory=Nested)
 
     m = Model()
     assert m.value.root == 42
+
+
+def test_root_model_json_schema_meta():
+    ParametrizedModel = RootModel[int]
+
+    class SubclassedModel(RootModel):
+        """Subclassed Model docstring"""
+
+        root: int
+
+    parametrized_json_schema = ParametrizedModel.model_json_schema()
+    subclassed_json_schema = SubclassedModel.model_json_schema()
+
+    assert parametrized_json_schema.get('title') == 'RootModel[int]'
+    assert parametrized_json_schema.get('description') is None
+    assert subclassed_json_schema.get('title') == 'SubclassedModel'
+    assert subclassed_json_schema.get('description') == 'Subclassed Model docstring'
```

### Comparing `pydantic-2.0b2/tests/test_serialize.py` & `pydantic-2.0b3/tests/test_serialize.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 """
 New tests for v2 of serialization logic.
 """
 import json
 import re
 from functools import partial, partialmethod
-from typing import Any, Callable, Dict, Iterable, Optional, Pattern, Tuple, Type
+from typing import Any, Callable, Dict, Optional, Pattern
 
 import pytest
-from pydantic_core import PydanticSerializationError, SchemaSerializer, core_schema, to_jsonable_python
+from pydantic_core import PydanticSerializationError, core_schema, to_jsonable_python
 from typing_extensions import Annotated, TypedDict
 
 from pydantic import (
     BaseModel,
     Field,
     FieldSerializationInfo,
-    GetCoreSchemaHandler,
-    SecretField,
     SecretStr,
     SerializationInfo,
+    SerializeAsAny,
     SerializerFunctionWrapHandler,
     TypeAdapter,
     errors,
     field_serializer,
     model_serializer,
 )
-from pydantic._internal import _known_annotated_metadata
-from pydantic._internal._config import ConfigWrapper
-from pydantic._internal._generate_schema import GenerateSchema
 from pydantic.config import ConfigDict
 from pydantic.functional_serializers import PlainSerializer, WrapSerializer
-from pydantic.types import _SecretFieldValidator
 
 
 def test_serialize_extra_allow() -> None:
     class Model(BaseModel):
         x: int
         model_config = ConfigDict(extra='allow')
 
@@ -148,51 +143,51 @@
 
 
 def test_serialize_decorator_always():
     class MyModel(BaseModel):
         x: Optional[int]
 
         @field_serializer('x')
-        def customise_x_serialisation(v, _info) -> str:
+        def customise_x_serialization(v, _info) -> str:
             return f'{v:,}'
 
     assert MyModel(x=1234).model_dump() == {'x': '1,234'}
     assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,234'}
     assert MyModel(x=1234).model_dump_json() == '{"x":"1,234"}'
     m = MyModel(x=None)
     # can't use v:, on None, hence error
     error_msg = (
-        'Error calling function `customise_x_serialisation`: '
+        'Error calling function `customise_x_serialization`: '
         'TypeError: unsupported format string passed to NoneType.__format__'
     )
     with pytest.raises(PydanticSerializationError, match=error_msg):
         m.model_dump()
     with pytest.raises(PydanticSerializationError, match=error_msg):
         m.model_dump_json()
 
 
 def test_serialize_decorator_json():
     class MyModel(BaseModel):
         x: int
 
         @field_serializer('x', when_used='json')
-        def customise_x_serialisation(v) -> str:
+        def customise_x_serialization(v) -> str:
             return f'{v:,}'
 
     assert MyModel(x=1234).model_dump() == {'x': 1234}
     assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,234'}
     assert MyModel(x=1234).model_dump_json() == '{"x":"1,234"}'
 
 
 def test_serialize_decorator_unless_none():
     class MyModel(BaseModel):
         x: Optional[int]
 
         @field_serializer('x', when_used='unless-none')
-        def customise_x_serialisation(v):
+        def customise_x_serialization(v):
             return f'{v:,}'
 
     assert MyModel(x=1234).model_dump() == {'x': '1,234'}
     assert MyModel(x=None).model_dump() == {'x': None}
     assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,234'}
     assert MyModel(x=None).model_dump(mode='json') == {'x': None}
     assert MyModel(x=1234).model_dump_json() == '{"x":"1,234"}'
@@ -349,27 +344,27 @@
 
 
 def test_serialize_decorator_self_info():
     class MyModel(BaseModel):
         x: Optional[int]
 
         @field_serializer('x')
-        def customise_x_serialisation(self, v, info) -> str:
+        def customise_x_serialization(self, v, info) -> str:
             return f'{info.mode}:{v:,}'
 
     assert MyModel(x=1234).model_dump() == {'x': 'python:1,234'}
     assert MyModel(x=1234).model_dump(mode='foobar') == {'x': 'foobar:1,234'}
 
 
 def test_serialize_decorator_self_no_info():
     class MyModel(BaseModel):
         x: Optional[int]
 
         @field_serializer('x')
-        def customise_x_serialisation(self, v) -> str:
+        def customise_x_serialization(self, v) -> str:
             return f'{v:,}'
 
     assert MyModel(x=1234).model_dump() == {'x': '1,234'}
 
 
 def test_model_serializer_plain():
     class MyModel(BaseModel):
@@ -795,24 +790,24 @@
     assert to_jsonable_python(AnyModel(x=m)) == {'x': {'m': 'custom:test'}}
     assert AnyModel(x=m).model_dump() == {'x': {'m': 'custom:test'}}
 
 
 def test_invalid_field():
     msg = (
         r'Decorators defined with incorrect fields:'
-        r' tests.test_serialize.test_invalid_field.<locals>.Model:\d+.customise_b_serialisation'
+        r' tests.test_serialize.test_invalid_field.<locals>.Model:\d+.customise_b_serialization'
         r" \(use check_fields=False if you're inheriting from the model and intended this\)"
     )
     with pytest.raises(errors.PydanticUserError, match=msg):
 
         class Model(BaseModel):
             a: str
 
             @field_serializer('b')
-            def customise_b_serialisation(v):
+            def customise_b_serialization(v):
                 return v
 
 
 def test_serialize_with_extra():
     class Inner(BaseModel):
         a: str = 'a'
 
@@ -887,53 +882,25 @@
             return {'x': self['x'] * 2, 'y': self['y'] * 3}
 
     ta = TypeAdapter(Model)
 
     assert ta.dump_json(Model({'x': 1, 'y': 2.5})) == b'{"x":2,"y":7.5}'
 
 
-def test_custom_secret_type_python_serializer():
-    """
-    test for non json serializer in pydantic.types._SecretFieldValidator.serialize.
-    most of the code in this test are just a copy from original implementation.
-    """
-
-    class MySecretFieldValidator(_SecretFieldValidator):
-        def __get_pydantic_core_schema__(
-            self, source: Type[Any], handler: GetCoreSchemaHandler
-        ) -> core_schema.CoreSchema:
-            self.inner_schema = handler(str if self.field_type is SecretStr else bytes)
-            error_kind = 'string_type' if self.field_type is SecretStr else 'bytes_type'
-            return core_schema.general_after_validator_function(
-                self.validate,
-                core_schema.union_schema(
-                    [core_schema.is_instance_schema(self.field_type), self.inner_schema],
-                    strict=True,
-                    custom_error_type=error_kind,
-                ),
-                serialization=core_schema.plain_serializer_function_ser_schema(
-                    self.serialize,
-                    info_arg=True,
-                    return_schema=core_schema.str_schema(),
-                    when_used='always',  # change it to `always` to call `serialize` for python and json
-                ),
-            )
-
-    class MySecretStr(SecretField[str]):
-        @classmethod
-        def __prepare_pydantic_annotations__(
-            cls, source: Type[Any], annotations: Tuple[Any, ...], _config: ConfigDict
-        ) -> Tuple[Any, Iterable[Any]]:
-            metadata, remaining_annotations = _known_annotated_metadata.collect_known_metadata(annotations)
-            _known_annotated_metadata.check_metadata(metadata, {'min_length', 'max_length'}, cls)
-            return (
-                source,
-                (
-                    MySecretFieldValidator(source, **metadata),
-                    *remaining_annotations,
-                ),
-            )
-
-    gen = GenerateSchema(ConfigWrapper({}), None)
-    schema = gen.generate_schema(MySecretStr)
-    serializer = SchemaSerializer(schema)
-    assert serializer.to_python('foo bar') == 'foo bar'
+def test_serialize_as_any() -> None:
+    class User(BaseModel):
+        name: str
+
+    class UserLogin(User):
+        password: SecretStr
+
+    class OuterModel(BaseModel):
+        as_any: SerializeAsAny[User]
+        without: User
+
+    user = UserLogin(name='pydantic', password='password')
+
+    # insert_assert(json.loads(OuterModel(as_any=user, without=user).model_dump_json()))
+    assert json.loads(OuterModel(as_any=user, without=user).model_dump_json()) == {
+        'as_any': {'name': 'pydantic', 'password': '**********'},
+        'without': {'name': 'pydantic'},
+    }
```

### Comparing `pydantic-2.0b2/tests/test_strict.py` & `pydantic-2.0b3/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_structural_pattern_matching.py` & `pydantic-2.0b3/tests/test_structural_pattern_matching.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_tools.py` & `pydantic-2.0b3/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_type_adapter.py` & `pydantic-2.0b3/tests/test_type_adapter.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_type_alias_type.py` & `pydantic-2.0b3/tests/test_type_alias_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,15 +149,14 @@
             'ctx': {'field_type': 'List', 'max_length': 1, 'actual_length': 2},
         }
     ]
 
     assert t.json_schema() == {'type': 'array', 'items': {'type': 'integer'}, 'maxItems': 1}
 
 
-@pytest.mark.xfail(reason='Not working yet, we cannot apply constraints to named/ref types')
 def test_type_alias_annotated_defs() -> None:
     # force use of refs by referencing the schema in multiple places
     t = TypeAdapter(Tuple[ShortMyList[int], ShortMyList[int]])
 
     assert t.validate_python((['1'], ['2'])) == ([1], [2])
 
     with pytest.raises(ValidationError) as exc_info:
@@ -227,15 +226,14 @@
                 'type': 'array',
                 'items': {'anyOf': [{'$ref': '#/$defs/RecursiveGenericAlias'}, {'type': 'integer'}]},
             }
         },
     }
 
 
-@pytest.mark.xfail(reason='Not working yet, we cannot apply constraints to named/ref types')
 def test_recursive_generic_type_alias_annotated() -> None:
     t = TypeAdapter(ShortRecursiveGenericAlias[int])
 
     assert t.validate_python([[]]) == [[]]
 
     with pytest.raises(ValidationError) as exc_info:
         t.validate_python([[], []])
@@ -245,28 +243,28 @@
             'loc': (),
             'msg': 'List should have at most 1 item after validation, not 2',
             'input': [[], []],
             'ctx': {'field_type': 'List', 'max_length': 1, 'actual_length': 2},
         }
     ]
 
+    # insert_assert(t.json_schema())
     assert t.json_schema() == {
         'type': 'array',
         'items': {'anyOf': [{'$ref': '#/$defs/RecursiveGenericAlias'}, {'type': 'integer'}]},
         'maxItems': 1,
         '$defs': {
             'RecursiveGenericAlias': {
                 'type': 'array',
                 'items': {'anyOf': [{'$ref': '#/$defs/RecursiveGenericAlias'}, {'type': 'integer'}]},
             }
         },
     }
 
 
-@pytest.mark.xfail(reason='Not working yet, we cannot apply constraints to named/ref types')
 def test_recursive_generic_type_alias_annotated_defs() -> None:
     # force use of refs by referencing the schema in multiple places
     t = TypeAdapter(Tuple[ShortRecursiveGenericAlias[int], ShortRecursiveGenericAlias[int]])
 
     assert t.validate_python(([[]], [[]])) == ([[]], [[]])
 
     with pytest.raises(ValidationError) as exc_info:
@@ -277,14 +275,15 @@
             'loc': (0,),
             'msg': 'List should have at most 1 item after validation, not 2',
             'input': [[], []],
             'ctx': {'field_type': 'List', 'max_length': 1, 'actual_length': 2},
         }
     ]
 
+    # insert_assert(t.json_schema())
     assert t.json_schema() == {
         'type': 'array',
         'minItems': 2,
         'prefixItems': [
             {'$ref': '#/$defs/RecursiveGenericAlias_MaxLen_max_length_1_'},
             {'$ref': '#/$defs/RecursiveGenericAlias_MaxLen_max_length_1_'},
         ],
```

### Comparing `pydantic-2.0b2/tests/test_types.py` & `pydantic-2.0b3/tests/test_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import math
 import os
 import re
 import sys
 import typing
 import uuid
 from collections import OrderedDict, defaultdict, deque
+from dataclasses import dataclass
 from datetime import date, datetime, time, timedelta, timezone
 from decimal import Decimal
 from enum import Enum, IntEnum
 from pathlib import Path
 from typing import (
     Any,
     Callable,
@@ -58,14 +59,15 @@
     Field,
     FilePath,
     FiniteFloat,
     FutureDate,
     FutureDatetime,
     GetCoreSchemaHandler,
     GetJsonSchemaHandler,
+    InstanceOf,
     Json,
     NaiveDatetime,
     NameEmail,
     NegativeFloat,
     NegativeInt,
     NewPath,
     NonNegativeFloat,
@@ -75,14 +77,15 @@
     PastDate,
     PastDatetime,
     PositiveFloat,
     PositiveInt,
     PydanticInvalidForJsonSchema,
     SecretBytes,
     SecretStr,
+    SkipValidation,
     StrictBool,
     StrictBytes,
     StrictFloat,
     StrictInt,
     StrictStr,
     TypeAdapter,
     ValidationError,
@@ -98,15 +101,15 @@
     field_serializer,
     field_validator,
     validate_call,
 )
 from pydantic.errors import PydanticSchemaGenerationError
 from pydantic.functional_validators import AfterValidator
 from pydantic.json_schema import JsonSchemaValue
-from pydantic.types import AllowInfNan, ImportString, InstanceOf, SecretField, SkipValidation, Strict, TransformSchema
+from pydantic.types import AllowInfNan, ImportString, Strict, TransformSchema
 
 try:
     import email_validator
 except ImportError:
     email_validator = None
 
 # TODO add back tests for Iterator
@@ -3856,18 +3859,14 @@
     assert len(f.empty_password) == 0
 
     # Assert retrieval of secret value is correct
     assert f.password.get_secret_value() == '1234'
     assert f.empty_password.get_secret_value() == ''
 
 
-def test_secretstr_is_secret_field():
-    assert issubclass(SecretStr, SecretField)
-
-
 def test_secretstr_equality():
     assert SecretStr('abc') == SecretStr('abc')
     assert SecretStr('123') != SecretStr('321')
     assert SecretStr('123') != '123'
     assert SecretStr('123') is not SecretStr('123')
 
 
@@ -3897,15 +3896,14 @@
         NonPositiveFloat,
         NonNegativeFloat,
         StrictFloat,
         FiniteFloat,
         conbytes,
         SecretBytes,
         constr,
-        SecretField,
         StrictStr,
         SecretStr,
         ImportString,
         conset,
         confrozenset,
         conlist,
         condecimal,
@@ -4024,18 +4022,14 @@
     # Assert that SecretBytes is equal to SecretBytes if the secret is the same.
     assert f == f.model_copy()
     copied_with_changes = f.model_copy()
     copied_with_changes.password = SecretBytes(b'4321')
     assert f != copied_with_changes
 
 
-def test_secretbytes_is_secret_field():
-    assert issubclass(SecretBytes, SecretField)
-
-
 def test_secretbytes_equality():
     assert SecretBytes(b'abc') == SecretBytes(b'abc')
     assert SecretBytes(b'123') != SecretBytes(b'321')
     assert SecretBytes(b'123') != b'123'
     assert SecretBytes(b'123') is not SecretBytes(b'123')
 
 
@@ -4723,17 +4717,15 @@
 
 def test_custom_generic_containers():
     T = TypeVar('T')
 
     class GenericList(List[T]):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
-            return core_schema.no_info_after_validator_function(
-                GenericList, handler.generate_schema(List[get_args(source_type)[0]])
-            )
+            return core_schema.no_info_after_validator_function(GenericList, handler(List[get_args(source_type)[0]]))
 
     class Model(BaseModel):
         field: GenericList[int]
 
     model = Model(field=['1', '2'])
     assert model.field == [1, 2]
     assert isinstance(model.field, GenericList)
@@ -5073,15 +5065,15 @@
     VT = TypeVar('VT')
 
     class CustomDefaultDict(DefaultDict[KT, VT]):
         @classmethod
         def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
             keys_type, values_type = get_args(source_type)
             return core_schema.no_info_after_validator_function(
-                lambda x: cls(x.default_factory, x), handler.generate_schema(DefaultDict[keys_type, values_type])
+                lambda x: cls(x.default_factory, x), handler(DefaultDict[keys_type, values_type])
             )
 
     ta = TypeAdapter(CustomDefaultDict[str, int])
 
     assert ta.validate_python({'a': 1}) == CustomDefaultDict(int, {'a': 1})
 
 
@@ -5558,7 +5550,61 @@
         (PastDatetime, 'PastDatetime'),
         (FutureDatetime, 'FutureDatetime'),
         (ImportString, 'ImportString'),
     ),
 )
 def test_types_repr(pydantic_type, expected):
     assert repr(pydantic_type()) == expected
+
+
+def test_enum_custom_schema() -> None:
+    class MyEnum(str, Enum):
+        foo = 'FOO'
+        bar = 'BAR'
+        baz = 'BAZ'
+
+        @classmethod
+        def __get_pydantic_core_schema__(
+            cls,
+            source_type: Any,
+            handler: GetCoreSchemaHandler,
+        ) -> CoreSchema:
+            # check that we can still call handler
+            handler(source_type)
+
+            # return a custom unrelated schema so we can test that
+            # it gets used
+            schema = core_schema.union_schema(
+                [
+                    core_schema.str_schema(),
+                    core_schema.is_instance_schema(cls),
+                ]
+            )
+            return core_schema.no_info_after_validator_function(
+                function=lambda x: MyEnum(x.upper()) if isinstance(x, str) else x,
+                schema=schema,
+                serialization=core_schema.plain_serializer_function_ser_schema(
+                    lambda x: x.value, return_schema=core_schema.int_schema()
+                ),
+            )
+
+    ta = TypeAdapter(MyEnum)
+
+    assert ta.validate_python('foo') == MyEnum.foo
+
+
+def test_get_pydantic_core_schema_marker_unrelated_type() -> None:
+    """Test using handler.generate_schema() to generate a schema that ignores
+    the current context of annotations and such
+    """
+
+    @dataclass
+    class Marker:
+        num: int
+
+        def __get_pydantic_core_schema__(self, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            schema = handler.resolve_ref_schema(handler.generate_schema(source_type))
+            return core_schema.no_info_after_validator_function(lambda x: x * self.num, schema)
+
+    ta = TypeAdapter(Annotated[int, Marker(2), Marker(3)])
+
+    assert ta.validate_python('1') == 3
```

### Comparing `pydantic-2.0b2/tests/test_types_namedtuple.py` & `pydantic-2.0b3/tests/test_types_namedtuple.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_types_payment_card_number.py` & `pydantic-2.0b3/tests/test_types_payment_card_number.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
 import pytest
 from pydantic_core import PydanticCustomError
 
 from pydantic import BaseModel, ValidationError
 from pydantic.types import PaymentCardBrand, PaymentCardNumber
 
+pytestmark = pytest.mark.filterwarnings(
+    'ignore:' 'The `PaymentCardNumber` class is deprecated, use `pydantic_extra_types` instead.*' ':DeprecationWarning'
+)
+
+
 VALID_AMEX = '370000000000002'
 VALID_MC = '5100000000000003'
 VALID_VISA_13 = '4050000000001'
 VALID_VISA_16 = '4050000000000001'
 VALID_VISA_19 = '4050000000000000001'
 VALID_OTHER = '2000000000000000008'
 LUHN_INVALID = '4000000000000000'
```

### Comparing `pydantic-2.0b2/tests/test_types_typeddict.py` & `pydantic-2.0b3/tests/test_types_typeddict.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,18 +172,32 @@
 
 
 def test_typeddict_extra_default(TypedDict):
     class User(TypedDict):
         name: str
         age: int
 
-    val = TypeAdapter(User)
+    ta = TypeAdapter(User)
+
+    assert ta.validate_python({'name': 'pika', 'age': 7, 'rank': 1}) == {'name': 'pika', 'age': 7}
+
+    class UserExtraAllow(User):
+        __pydantic_config__ = ConfigDict(extra='allow')
+
+    ta = TypeAdapter(UserExtraAllow)
+
+    assert ta.validate_python({'name': 'pika', 'age': 7, 'rank': 1}) == {'name': 'pika', 'age': 7, 'rank': 1}
+
+    class UserExtraForbid(User):
+        __pydantic_config__ = ConfigDict(extra='forbid')
+
+    ta = TypeAdapter(UserExtraForbid)
 
     with pytest.raises(ValidationError) as exc_info:
-        val.validate_python({'name': 'pika', 'age': 7, 'rank': 1})
+        ta.validate_python({'name': 'pika', 'age': 7, 'rank': 1})
     # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
         {'type': 'extra_forbidden', 'loc': ('rank',), 'msg': 'Extra inputs are not permitted', 'input': 1}
     ]
 
 
 def test_typeddict_schema(TypedDict):
@@ -197,84 +211,86 @@
         b: int
 
         @classmethod
         def __get_pydantic_core_schema__(
             cls, source_type: Any, handler: GetCoreSchemaHandler
         ) -> core_schema.CoreSchema:
             schema = handler(source_type)
-            schema['computed_fields'] = [
-                core_schema.computed_field(property_name='another_b', return_schema=core_schema.int_schema())
-            ]
+            schema = handler.resolve_ref_schema(schema)
+            assert schema['type'] == 'typed-dict'
+            b = schema['fields']['b']['schema']
+            assert b['type'] == 'int'
+            b['gt'] = 0  # type: ignore
             return schema
 
     class Model(BaseModel):
         data: Data
         data_td: DataTD
         custom_td: CustomTD
 
+    # insert_assert(Model.model_json_schema(mode='validation'))
     assert Model.model_json_schema(mode='validation') == {
-        'title': 'Model',
         'type': 'object',
         'properties': {
-            'custom_td': {'$ref': '#/$defs/CustomTD'},
             'data': {'$ref': '#/$defs/Data'},
             'data_td': {'$ref': '#/$defs/DataTD'},
+            'custom_td': {'$ref': '#/$defs/CustomTD'},
         },
         'required': ['data', 'data_td', 'custom_td'],
+        'title': 'Model',
         '$defs': {
+            'DataTD': {
+                'type': 'object',
+                'properties': {'a': {'type': 'integer', 'title': 'A'}},
+                'required': ['a'],
+                'title': 'DataTD',
+            },
             'CustomTD': {
                 'type': 'object',
-                'title': 'CustomTD',
-                'properties': {'b': {'title': 'B', 'type': 'integer'}},
+                'properties': {'b': {'type': 'integer', 'exclusiveMinimum': 0, 'title': 'B'}},
                 'required': ['b'],
+                'title': 'CustomTD',
             },
             'Data': {
                 'type': 'object',
-                'title': 'Data',
-                'properties': {'a': {'title': 'A', 'type': 'integer'}},
-                'required': ['a'],
-            },
-            'DataTD': {
-                'type': 'object',
-                'title': 'DataTD',
-                'properties': {'a': {'title': 'A', 'type': 'integer'}},
+                'properties': {'a': {'type': 'integer', 'title': 'A'}},
                 'required': ['a'],
+                'title': 'Data',
             },
         },
     }
+
+    # insert_assert(Model.model_json_schema(mode='serialization'))
     assert Model.model_json_schema(mode='serialization') == {
-        'title': 'Model',
         'type': 'object',
         'properties': {
-            'custom_td': {'$ref': '#/$defs/CustomTD'},
             'data': {'$ref': '#/$defs/Data'},
             'data_td': {'$ref': '#/$defs/DataTD'},
+            'custom_td': {'$ref': '#/$defs/CustomTD'},
         },
         'required': ['data', 'data_td', 'custom_td'],
+        'title': 'Model',
         '$defs': {
+            'DataTD': {
+                'type': 'object',
+                'properties': {'a': {'type': 'integer', 'title': 'A'}},
+                'required': ['a'],
+                'title': 'DataTD',
+            },
             'CustomTD': {
                 'type': 'object',
+                'properties': {'b': {'type': 'integer', 'exclusiveMinimum': 0, 'title': 'B'}},
+                'required': ['b'],
                 'title': 'CustomTD',
-                'properties': {
-                    'b': {'title': 'B', 'type': 'integer'},
-                    'another_b': {'title': 'Another B', 'type': 'integer'},
-                },
-                'required': ['b', 'another_b'],
             },
             'Data': {
                 'type': 'object',
-                'title': 'Data',
-                'properties': {'a': {'title': 'A', 'type': 'integer'}},
-                'required': ['a'],
-            },
-            'DataTD': {
-                'type': 'object',
-                'title': 'DataTD',
-                'properties': {'a': {'title': 'A', 'type': 'integer'}},
+                'properties': {'a': {'type': 'integer', 'title': 'A'}},
                 'required': ['a'],
+                'title': 'Data',
             },
         },
     }
 
 
 def test_typeddict_postponed_annotation(TypedDict):
     class DataTD(TypedDict):
@@ -825,7 +841,17 @@
         @model_serializer(mode='plain')
         def ser_model(self) -> Dict[str, Any]:
             return {'x': self['x'] * 2, 'y': self['y'] * 3}
 
     ta = TypeAdapter(Model)
 
     assert ta.dump_python(Model({'x': 1, 'y': 2.5})) == {'x': 2, 'y': 7.5}
+
+
+def test_model_config() -> None:
+    class Model(TypedDict):
+        x: str
+        __pydantic_config__ = ConfigDict(str_to_lower=True)  # type: ignore
+
+    ta = TypeAdapter(Model)
+
+    assert ta.validate_python({'x': 'ABC'}) == {'x': 'abc'}
```

### Comparing `pydantic-2.0b2/tests/test_utils.py` & `pydantic-2.0b3/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,14 +283,15 @@
         ',',
         0,
         -1,
         ')',
     ]
 
 
+@pytest.mark.filterwarnings('ignore::DeprecationWarning')
 def test_pretty_color():
     c = Color('red')
     assert str(c) == 'red'
     assert repr(c) == "Color('red', rgb=(255, 0, 0))"
     assert list(c.__pretty__(lambda x: f'fmt: {x!r}')) == [
         'Color(',
         1,
```

### Comparing `pydantic-2.0b2/tests/test_v1.py` & `pydantic-2.0b3/tests/test_v1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_validate_call.py` & `pydantic-2.0b3/tests/test_validate_call.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_validators.py` & `pydantic-2.0b3/tests/test_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from typing_extensions import Annotated, Literal
 
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
     FieldValidationInfo,
+    PydanticUserError,
     ValidationError,
     ValidationInfo,
     ValidatorFunctionWrapHandler,
     errors,
     field_validator,
     model_validator,
     root_validator,
@@ -2522,14 +2523,31 @@
                 assert v == {'x': 2}
                 return {'x': 4}
 
     assert Parent(x=1).model_dump() == {'x': 2}
     assert Child(x=1).model_dump() == {'x': 4}
 
 
+def test_bare_root_validator():
+    with pytest.raises(
+        PydanticUserError,
+        match=re.escape(
+            'If you use `@root_validator` with pre=False (the default) you MUST specify `skip_on_failure=True`.'
+            ' Note that `@root_validator` is deprecated and should be replaced with `@model_validator`.'
+        ),
+    ):
+        with pytest.warns(DeprecationWarning, match='Pydantic V1 style `@root_validator` validators are deprecated.'):
+
+            class Model(BaseModel):
+                @root_validator
+                @classmethod
+                def validate_values(cls, values):
+                    return values
+
+
 def test_validator_with_underscore_name() -> None:
     """
     https://github.com/pydantic/pydantic/issues/5252
     """
 
     def f(name: str) -> str:
         return name.lower()
```

### Comparing `pydantic-2.0b2/tests/test_validators_dataclass.py` & `pydantic-2.0b3/tests/test_validators_dataclass.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/test_version.py` & `pydantic-2.0b3/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/test_mypy.py` & `pydantic-2.0b3/tests/mypy/test_mypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,16 @@
         'computed_fields.py',
         'computed_fields.txt',
         marks=pytest.mark.skipif(
             sys.version_info < (3, 8) or MYPY_VERSION_TUPLE < (0, 982),
             reason='cached_property is only available in Python 3.8+, errors are different with mypy 0.971',
         ),
     ),
+    ('mypy-default.ini', 'metaclass_args.py', 'metaclass_args_no_plugin.txt'),
+    ('mypy-plugin-very-strict.ini', 'metaclass_args.py', 'metaclass_args_plugin.txt'),
 ]
 
 
 def build_executable_modules():
     """
     Iterates over the test cases and returns a list of modules that should be executable.
     Specifically, we include any modules that are not expected to produce any typechecking errors.
```

### Comparing `pydantic-2.0b2/tests/mypy/configs/mypy-plugin-strict-no-any.ini` & `pydantic-2.0b3/tests/mypy/configs/mypy-plugin-strict-no-any.ini`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/configs/pyproject-default.toml` & `pydantic-2.0b3/tests/mypy/configs/pyproject-default.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/configs/pyproject-plugin-bad-param.toml` & `pydantic-2.0b3/tests/mypy/configs/pyproject-plugin-bad-param.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/configs/pyproject-plugin-strict.toml` & `pydantic-2.0b3/tests/mypy/configs/pyproject-plugin-strict.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/configs/pyproject-plugin.toml` & `pydantic-2.0b3/tests/mypy/configs/pyproject-plugin.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/modules/computed_fields.py` & `pydantic-2.0b3/tests/mypy/modules/computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/modules/fail4.py` & `pydantic-2.0b3/tests/mypy/modules/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/modules/plugin_default_factory.py` & `pydantic-2.0b3/tests/mypy/modules/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/modules/plugin_fail.py` & `pydantic-2.0b3/tests/mypy/modules/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/modules/plugin_fail_baseConfig.py` & `pydantic-2.0b3/tests/mypy/modules/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/modules/plugin_success.py` & `pydantic-2.0b3/tests/mypy/modules/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/modules/plugin_success_baseConfig.py` & `pydantic-2.0b3/tests/mypy/modules/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/modules/success.py` & `pydantic-2.0b3/tests/mypy/modules/success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/outputs/latest/fail4.txt` & `pydantic-2.0b3/tests/mypy/outputs/latest/fail4.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt` & `pydantic-2.0b3/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt` & `pydantic-2.0b3/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail-strict.txt` & `pydantic-2.0b3/tests/mypy/outputs/latest/plugin-fail-strict.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail.txt` & `pydantic-2.0b3/tests/mypy/outputs/latest/plugin-fail.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/tests/pyright/pyright_example.py` & `pydantic-2.0b3/tests/pyright/pyright_example.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/.gitignore` & `pydantic-2.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/LICENSE` & `pydantic-2.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b2/pyproject.toml` & `pydantic-2.0b3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet',
 ]
 requires-python = '>=3.7'
 dependencies = [
     'typing-extensions>=4.6.1',
     'annotated-types>=0.4.0',
-    "pydantic-core==0.38.0",
+    "pydantic-core==0.39.0",
 ]
 dynamic = ['version', 'readme']
 
 [project.optional-dependencies]
 email = ['email-validator>=2.0.0']
 
 [tool.pdm.dev-dependencies]
@@ -80,14 +80,16 @@
     "mkdocstrings-python",
     "tomli",
     "pyupgrade",
     "mike @ git+https://github.com/jimporter/mike.git",
     "mkdocs-embed-external-markdown>=2.3.0",
     "black>=23.3.0",
     "pytest-examples>=0.0.9",
+    "pydantic-settings>=2.0b1",
+    "pydantic-extra-types @ git+https://github.com/pydantic/pydantic-extra-types.git@main"
 ]
 linting = [
     "black",
     "ruff",
     "mypy~=1.1.1",
 ]
 testing-extra = [
@@ -152,24 +154,36 @@
 # configuring https://github.com/pydantic/hooky
 [tool.hooky]
 reviewers = ['samuelcolvin', 'adriangb', 'dmontagu', 'hramezani', 'lig', 'Kludex']
 require_change_file = false
 
 [tool.ruff]
 line-length = 120
-extend-select = ['Q', 'RUF100', 'C90', 'UP', 'I']
+extend-select = ['Q', 'RUF100', 'C90', 'UP', 'I', 'D']
+extend-ignore = ['D105', 'D107', 'D205']
 flake8-quotes = {inline-quotes = 'single', multiline-quotes = 'double'}
 mccabe = { max-complexity = 14 }
 isort = { known-first-party = ['pydantic', 'tests'] }
 target-version = "py37"
 exclude=['pydantic/v1']
 
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [tool.ruff.per-file-ignores]
-'pydantic/__init__.py' = ['F405', 'F403']
+'docs/*' = ['D']
+'pydantic/__init__.py' = ['F405', 'F403', 'D']
 'tests/test_forward_ref.py' = ['F821']
+'tests/*' = ['D']
+'pydantic/deprecated/*' = ['D']
+'pydantic/functional_validators.py' = ['D']
+'pydantic/json_schema.py' = ['D']
+'pydantic/main.py' = ['D']
+'pydantic/mypy.py' = ['D']
+'pydantic/root_model.py' = ['D']
 
 [tool.coverage.run]
 source = ['pydantic']
 omit = ['pydantic/deprecated/*', 'pydantic/v1/*']
 branch = true
 context = '${CONTEXT}'
```

### Comparing `pydantic-2.0b2/PKG-INFO` & `pydantic-2.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic
-Version: 2.0b2
+Version: 2.0b3
 Summary: Data validation using Python type hints
 Project-URL: Homepage, https://github.com/pydantic/pydantic
 Project-URL: Documentation, https://docs.pydantic.dev
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic
 Project-URL: Changelog, https://docs.pydantic.dev/changelog
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>, Adrian Garcia Badaracco <1755071+adriangb@users.noreply.github.com>, Terrence Dorsey <terry@pydantic.dev>, David Montague <david@pydantic.dev>
@@ -31,15 +31,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: annotated-types>=0.4.0
-Requires-Dist: pydantic-core==0.38.0
+Requires-Dist: pydantic-core==0.39.0
 Requires-Dist: typing-extensions>=4.6.1
 Provides-Extra: email
 Requires-Dist: email-validator>=2.0.0; extra == 'email'
 Description-Content-Type: text/markdown
 
 # Pydantic
 
@@ -49,16 +49,16 @@
 [![CondaForge](https://img.shields.io/conda/v/conda-forge/pydantic.svg)](https://anaconda.org/conda-forge/pydantic)
 [![downloads](https://pepy.tech/badge/pydantic/month)](https://pepy.tech/project/pydantic)
 [![versions](https://img.shields.io/pypi/pyversions/pydantic.svg)](https://github.com/pydantic/pydantic)
 [![license](https://img.shields.io/github/license/pydantic/pydantic.svg)](https://github.com/pydantic/pydantic/blob/main/LICENSE)
 
 Data validation using Python type hints.
 
-Fast and extensible, *pydantic* plays nicely with your linters/IDE/brain.
-Define how data should be in pure, canonical Python 3.7+; validate it with *pydantic*.
+Fast and extensible, Pydantic plays nicely with your linters/IDE/brain.
+Define how data should be in pure, canonical Python 3.7+; validate it with Pydantic.
 
 ## Pydantic Company :rocket:
 
 We've started a company based on the principles that I believe have led to Pydantic's success.
 Learning more from the [Company Announcement](https://pydantic.dev/announcement/).
 
 ## Pydantic V1.10 vs. V2
@@ -72,15 +72,15 @@
 ## Help
 
 See [documentation](https://docs.pydantic.dev/) for more details.
 
 ## Installation
 
 Install using `pip install -U pydantic` or `conda install pydantic -c conda-forge`.
-For more installation options to make *pydantic* even faster,
+For more installation options to make Pydantic even faster,
 see the [Install](https://docs.pydantic.dev/install/) section in the documentation.
 
 ## A Simple Example
 
 ```py
 from datetime import datetime
 from typing import List, Optional
@@ -99,23 +99,29 @@
 print(user.id)
 #> 123
 ```
 
 ## Contributing
 
 For guidance on setting up a development environment and how to make a
-contribution to *pydantic*, see
+contribution to Pydantic, see
 [Contributing to Pydantic](https://docs.pydantic.dev/contributing/).
 
 ## Reporting a Security Vulnerability
 
 See our [security policy](https://github.com/pydantic/pydantic/security/policy).
 
 ## Changelog
 
+## v2.0b3 (2023-06-16)
+
+Third beta pre-release of Pydantic V2
+
+See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0b3)
+
 ## v2.0b2 (2023-06-03)
 
 Add `from_attributes` runtime flag to `TypeAdapter.validate_python` and `BaseModel.model_validate`.
 
 See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0b2)
 
 ## v2.0b1 (2023-06-01)
@@ -144,14 +150,28 @@
 
 ## v2.0a1 (2023-04-03)
 
 First pre-release of Pydantic V2!
 
 See [this post](https://docs.pydantic.dev/blog/pydantic-v2-alpha/) for more details.
 
+## v1.10.9 (2023-06-07)
+
+* Fix trailing zeros not ignored in Decimal validation, [#5968](https://github.com/pydantic/pydantic/issues/5968) by [@hramezani](https://github.com/hramezani)
+* Fix mypy plugin for v1.4.0, [#5928](https://github.com/pydantic/pydantic/issues/5928) by [@cdce8p](https://github.com/cdce8p)
+* Add future and past date hypothesis strategies, [#5850](https://github.com/pydantic/pydantic/issues/5850) by [@bschoenmaeckers](https://github.com/bschoenmaeckers)
+* Discourage usage of Cython 3 with Pydantic 1.x, [#5845](https://github.com/pydantic/pydantic/issues/5845) by [@lig](https://github.com/lig)
+
+## v1.10.8 (2023-05-23)
+
+* Fix a bug in `Literal` usage with `typing-extension==4.6.0`, [#5826](https://github.com/pydantic/pydantic/issues/5826) by [@hramezani](https://github.com/hramezani)
+* This solves the (closed) issue [#3849](https://github.com/pydantic/pydantic/issues/3849) where aliased fields that use discriminated union fail to validate when the data contains the non-aliased field name, [#5736](https://github.com/pydantic/pydantic/issues/5736) by [@benwah](https://github.com/benwah)
+* Update email-validator dependency to >=2.0.0post2, [#5627](https://github.com/pydantic/pydantic/issues/5627) by [@adriangb](https://github.com/adriangb)
+* update `AnyClassMethod` for changes in [python/typeshed#9771](https://github.com/python/typeshed/issues/9771), [#5505](https://github.com/pydantic/pydantic/issues/5505) by [@ITProKyle](https://github.com/ITProKyle)
+
 ## v1.10.7 (2023-03-22)
 
 * Fix creating schema from model using `ConstrainedStr` with `regex` as dict key, [#5223](https://github.com/pydantic/pydantic/issues/5223) by [@matejetz](https://github.com/matejetz)
 * Address bug in mypy plugin caused by explicit_package_bases=True, [#5191](https://github.com/pydantic/pydantic/issues/5191) by [@dmontagu](https://github.com/dmontagu)
 * Add implicit defaults in the mypy plugin for Field with no default argument, [#5190](https://github.com/pydantic/pydantic/issues/5190) by [@dmontagu](https://github.com/dmontagu)
 * Fix schema generated for Enum values used as Literals in discriminated unions, [#5188](https://github.com/pydantic/pydantic/issues/5188) by [@javibookline](https://github.com/javibookline)
 * Fix mypy failures caused by the pydantic mypy plugin when users define `from_orm` in their own classes, [#5187](https://github.com/pydantic/pydantic/issues/5187) by [@dmontagu](https://github.com/dmontagu)
@@ -425,15 +445,15 @@
 * Fix mypy plugin issue with self field declaration, [#2743](https://github.com/pydantic/pydantic/issues/2743) by [@uriyyo](https://github.com/uriyyo)
 * The colon at the end of the line "The fields which were supplied when user was initialised:" suggests that the code following it is related.
   Changed it to a period, [#2733](https://github.com/pydantic/pydantic/issues/2733) by [@krisaoe](https://github.com/krisaoe)
 * Renamed variable `schema` to `schema_` to avoid shadowing of global variable name, [#2724](https://github.com/pydantic/pydantic/issues/2724) by [@shahriyarr](https://github.com/shahriyarr)
 * Add support for autocomplete in VS Code via `__dataclass_transform__`, [#2721](https://github.com/pydantic/pydantic/issues/2721) by [@tiangolo](https://github.com/tiangolo)
 * add missing type annotations in `BaseConfig` and handle `max_length = 0`, [#2719](https://github.com/pydantic/pydantic/issues/2719) by [@PrettyWood](https://github.com/PrettyWood)
 * Change `orm_mode` checking to allow recursive ORM mode parsing with dicts, [#2718](https://github.com/pydantic/pydantic/issues/2718) by [@nuno-andre](https://github.com/nuno-andre)
-* Add episode 313 of the *Talk Python To Me* podcast, where Michael Kennedy and Samuel Colvin discuss *pydantic*, to the docs, [#2712](https://github.com/pydantic/pydantic/issues/2712) by [@RatulMaharaj](https://github.com/RatulMaharaj)
+* Add episode 313 of the *Talk Python To Me* podcast, where Michael Kennedy and Samuel Colvin discuss Pydantic, to the docs, [#2712](https://github.com/pydantic/pydantic/issues/2712) by [@RatulMaharaj](https://github.com/RatulMaharaj)
 * fix JSON schema generation when a field is of type `NamedTuple` and has a default value, [#2707](https://github.com/pydantic/pydantic/issues/2707) by [@PrettyWood](https://github.com/PrettyWood)
 * `Enum` fields now properly support extra kwargs in schema generation, [#2697](https://github.com/pydantic/pydantic/issues/2697) by [@sammchardy](https://github.com/sammchardy)
 * **Breaking Change, see [#3780](https://github.com/pydantic/pydantic/issues/3780)**: Make serialization of referenced pydantic models possible, [#2650](https://github.com/pydantic/pydantic/issues/2650) by [@PrettyWood](https://github.com/PrettyWood)
 * Add `uniqueItems` option to `ConstrainedList`, [#2618](https://github.com/pydantic/pydantic/issues/2618) by [@nuno-andre](https://github.com/nuno-andre)
 * Try to evaluate forward refs automatically at model creation, [#2588](https://github.com/pydantic/pydantic/issues/2588) by [@uriyyo](https://github.com/uriyyo)
 * Switch docs preview and coverage display to use [smokeshow](https://smokeshow.helpmanual.io/), [#2580](https://github.com/pydantic/pydantic/issues/2580) by [@samuelcolvin](https://github.com/samuelcolvin)
 * Add `__version__` attribute to pydantic module, [#2572](https://github.com/pydantic/pydantic/issues/2572) by [@paxcodes](https://github.com/paxcodes)
@@ -676,15 +696,15 @@
 * Add private attributes support, [#1679](https://github.com/pydantic/pydantic/issues/1679) by [@Bobronium](https://github.com/Bobronium)
 * add `config` to `@validate_arguments`, [#1663](https://github.com/pydantic/pydantic/issues/1663) by [@samuelcolvin](https://github.com/samuelcolvin)
 * Allow descendant Settings models to override env variable names for the fields defined in parent Settings models with
   `env` in their `Config`. Previously only `env_prefix` configuration option was applicable, [#1561](https://github.com/pydantic/pydantic/issues/1561) by [@ojomio](https://github.com/ojomio)
 * Support `ref_template` when creating schema `$ref`s, [#1479](https://github.com/pydantic/pydantic/issues/1479) by [@kilo59](https://github.com/kilo59)
 * Add a `__call__` stub to `PyObject` so that mypy will know that it is callable, [#1352](https://github.com/pydantic/pydantic/issues/1352) by [@brianmaissy](https://github.com/brianmaissy)
 * `pydantic.dataclasses.dataclass` decorator now supports built-in `dataclasses.dataclass`.
-  It is hence possible to convert an existing `dataclass` easily to add *pydantic* validation.
+  It is hence possible to convert an existing `dataclass` easily to add Pydantic validation.
   Moreover nested dataclasses are also supported, [#744](https://github.com/pydantic/pydantic/issues/744) by [@PrettyWood](https://github.com/PrettyWood)
 
 ## v1.6.2 (2021-05-11)
 
 * **Security fix:** Fix `date` and `datetime` parsing so passing either `'infinity'` or `float('inf')`
   (or their negative values) does not cause an infinite loop,
   See security advisory [CVE-2021-29510](https://github.com/pydantic/pydantic/security/advisories/GHSA-5jqp-qgf6-3pvh)
@@ -700,15 +720,15 @@
 * Modify validators for `conlist` and `conset` to not have `always=True`, [#1682](https://github.com/pydantic/pydantic/issues/1682) by [@samuelcolvin](https://github.com/samuelcolvin)
 * add port check to `AnyUrl` (can't exceed 65536) ports are 16 insigned bits: `0 <= port <= 2**16-1` src: [rfc793 header format](https://tools.ietf.org/html/rfc793#section-3.1), [#1654](https://github.com/pydantic/pydantic/issues/1654) by [@flapili](https://github.com/flapili)
 * Document default `regex` anchoring semantics, [#1648](https://github.com/pydantic/pydantic/issues/1648) by [@yurikhan](https://github.com/yurikhan)
 * Use `chain.from_iterable` in class_validators.py. This is a faster and more idiomatic way of using `itertools.chain`.
   Instead of computing all the items in the iterable and storing them in memory, they are computed one-by-one and never
   stored as a huge list. This can save on both runtime and memory space, [#1642](https://github.com/pydantic/pydantic/issues/1642) by [@cool-RR](https://github.com/cool-RR)
 * Add `conset()`, analogous to `conlist()`, [#1623](https://github.com/pydantic/pydantic/issues/1623) by [@patrickkwang](https://github.com/patrickkwang)
-* make *pydantic* errors (un)pickable, [#1616](https://github.com/pydantic/pydantic/issues/1616) by [@PrettyWood](https://github.com/PrettyWood)
+* make Pydantic errors (un)pickable, [#1616](https://github.com/pydantic/pydantic/issues/1616) by [@PrettyWood](https://github.com/PrettyWood)
 * Allow custom encoding for `dotenv` files, [#1615](https://github.com/pydantic/pydantic/issues/1615) by [@PrettyWood](https://github.com/PrettyWood)
 * Ensure `SchemaExtraCallable` is always defined to get type hints on BaseConfig, [#1614](https://github.com/pydantic/pydantic/issues/1614) by [@PrettyWood](https://github.com/PrettyWood)
 * Update datetime parser to support negative timestamps, [#1600](https://github.com/pydantic/pydantic/issues/1600) by [@mlbiche](https://github.com/mlbiche)
 * Update mypy, remove `AnyType` alias for `Type[Any]`, [#1598](https://github.com/pydantic/pydantic/issues/1598) by [@samuelcolvin](https://github.com/samuelcolvin)
 * Adjust handling of root validators so that errors are aggregated from _all_ failing root validators, instead of reporting on only the first root validator to fail, [#1586](https://github.com/pydantic/pydantic/issues/1586) by [@beezee](https://github.com/beezee)
 * Make `__modify_schema__` on Enums apply to the enum schema rather than fields that use the enum, [#1581](https://github.com/pydantic/pydantic/issues/1581) by [@therefromhere](https://github.com/therefromhere)
 * Fix behavior of `__all__` key when used in conjunction with index keys in advanced include/exclude of fields that are sequences, [#1579](https://github.com/pydantic/pydantic/issues/1579) by [@xspirus](https://github.com/xspirus)
```

