# Comparing `tmp/dataclasses-json-0.5.7.tar.gz` & `tmp/dataclasses-json-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dataclasses-json-0.5.7.tar", last modified: Mon Mar 21 14:49:30 2022, max compression
+gzip compressed data, was "dataclasses-json-0.5.8.tar", last modified: Sun Jun 11 18:43:06 2023, max compression
```

## Comparing `dataclasses-json-0.5.7.tar` & `dataclasses-json-0.5.8.tar`

### file list

```diff
@@ -1,24 +1,44 @@
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2022-03-21 14:49:30.307501 dataclasses-json-0.5.7/
--rw-r--r--   0 charlie    (501) staff       (20)     1084 2019-06-16 15:23:27.000000 dataclasses-json-0.5.7/LICENSE
--rw-r--r--   0 charlie    (501) staff       (20)       16 2021-08-26 01:55:32.000000 dataclasses-json-0.5.7/MANIFEST.in
--rw-r--r--   0 charlie    (501) staff       (20)    27348 2022-03-21 14:49:30.307096 dataclasses-json-0.5.7/PKG-INFO
--rw-r--r--   0 charlie    (501) staff       (20)    21719 2022-03-21 14:47:36.000000 dataclasses-json-0.5.7/README.md
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2022-03-21 14:49:30.303676 dataclasses-json-0.5.7/dataclasses_json/
--rw-r--r--   0 charlie    (501) staff       (20)      441 2022-03-21 14:47:36.000000 dataclasses-json-0.5.7/dataclasses_json/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     5147 2022-03-21 14:47:36.000000 dataclasses-json-0.5.7/dataclasses_json/api.py
--rw-r--r--   0 charlie    (501) staff       (20)     3365 2022-03-21 14:47:36.000000 dataclasses-json-0.5.7/dataclasses_json/cfg.py
--rw-r--r--   0 charlie    (501) staff       (20)    13995 2022-03-21 14:47:44.000000 dataclasses-json-0.5.7/dataclasses_json/core.py
--rw-r--r--   0 charlie    (501) staff       (20)    13904 2021-08-26 01:55:32.000000 dataclasses-json-0.5.7/dataclasses_json/mm.py
--rw-r--r--   0 charlie    (501) staff       (20)     3307 2021-08-26 02:01:26.000000 dataclasses-json-0.5.7/dataclasses_json/stringcase.py
--rw-r--r--   0 charlie    (501) staff       (20)    10110 2021-06-03 10:39:20.000000 dataclasses-json-0.5.7/dataclasses_json/undefined.py
--rw-r--r--   0 charlie    (501) staff       (20)     4499 2021-08-26 01:55:32.000000 dataclasses-json-0.5.7/dataclasses_json/utils.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2022-03-21 14:49:30.306227 dataclasses-json-0.5.7/dataclasses_json.egg-info/
--rw-r--r--   0 charlie    (501) staff       (20)    27348 2022-03-21 14:49:30.000000 dataclasses-json-0.5.7/dataclasses_json.egg-info/PKG-INFO
--rw-r--r--   0 charlie    (501) staff       (20)      475 2022-03-21 14:49:30.000000 dataclasses-json-0.5.7/dataclasses_json.egg-info/SOURCES.txt
--rw-r--r--   0 charlie    (501) staff       (20)        1 2022-03-21 14:49:30.000000 dataclasses-json-0.5.7/dataclasses_json.egg-info/dependency_links.txt
--rw-r--r--   0 charlie    (501) staff       (20)      246 2022-03-21 14:49:30.000000 dataclasses-json-0.5.7/dataclasses_json.egg-info/requires.txt
--rw-r--r--   0 charlie    (501) staff       (20)       17 2022-03-21 14:49:30.000000 dataclasses-json-0.5.7/dataclasses_json.egg-info/top_level.txt
--rw-r--r--   0 charlie    (501) staff       (20)      645 2021-08-26 19:33:00.000000 dataclasses-json-0.5.7/publish.py
--rw-r--r--   0 charlie    (501) staff       (20)       46 2020-02-23 14:06:06.000000 dataclasses-json-0.5.7/pyproject.toml
--rw-r--r--   0 charlie    (501) staff       (20)       38 2022-03-21 14:49:30.307613 dataclasses-json-0.5.7/setup.cfg
--rw-r--r--   0 charlie    (501) staff       (20)     1161 2022-03-21 14:48:28.000000 dataclasses-json-0.5.7/setup.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-06-11 18:43:06.793468 dataclasses-json-0.5.8/
+-rw-r--r--   0 charlie    (501) staff       (20)     1084 2019-06-16 15:23:27.000000 dataclasses-json-0.5.8/LICENSE
+-rw-r--r--   0 charlie    (501) staff       (20)       16 2021-08-26 01:55:32.000000 dataclasses-json-0.5.8/MANIFEST.in
+-rw-r--r--   0 charlie    (501) staff       (20)    27356 2023-06-11 18:43:06.793309 dataclasses-json-0.5.8/PKG-INFO
+-rw-r--r--   0 charlie    (501) staff       (20)    21727 2023-06-11 01:41:14.000000 dataclasses-json-0.5.8/README.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-06-11 18:43:06.788593 dataclasses-json-0.5.8/dataclasses_json/
+-rw-r--r--   0 charlie    (501) staff       (20)      441 2022-03-21 14:47:36.000000 dataclasses-json-0.5.8/dataclasses_json/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     5113 2023-06-11 01:41:14.000000 dataclasses-json-0.5.8/dataclasses_json/api.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3365 2022-03-21 14:47:36.000000 dataclasses-json-0.5.8/dataclasses_json/cfg.py
+-rw-r--r--   0 charlie    (501) staff       (20)    14748 2023-06-11 01:41:14.000000 dataclasses-json-0.5.8/dataclasses_json/core.py
+-rw-r--r--   0 charlie    (501) staff       (20)    13904 2021-08-26 01:55:32.000000 dataclasses-json-0.5.8/dataclasses_json/mm.py
+-rw-r--r--   0 charlie    (501) staff       (20)        0 2020-02-23 14:06:06.000000 dataclasses-json-0.5.8/dataclasses_json/py.typed
+-rw-r--r--   0 charlie    (501) staff       (20)     3307 2021-08-26 02:01:26.000000 dataclasses-json-0.5.8/dataclasses_json/stringcase.py
+-rw-r--r--   0 charlie    (501) staff       (20)    10110 2021-06-03 10:39:20.000000 dataclasses-json-0.5.8/dataclasses_json/undefined.py
+-rw-r--r--   0 charlie    (501) staff       (20)     5464 2022-08-14 20:35:15.000000 dataclasses-json-0.5.8/dataclasses_json/utils.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-06-11 18:43:06.789352 dataclasses-json-0.5.8/dataclasses_json.egg-info/
+-rw-r--r--   0 charlie    (501) staff       (20)    27356 2023-06-11 18:43:06.000000 dataclasses-json-0.5.8/dataclasses_json.egg-info/PKG-INFO
+-rw-r--r--   0 charlie    (501) staff       (20)      931 2023-06-11 18:43:06.000000 dataclasses-json-0.5.8/dataclasses_json.egg-info/SOURCES.txt
+-rw-r--r--   0 charlie    (501) staff       (20)        1 2023-06-11 18:43:06.000000 dataclasses-json-0.5.8/dataclasses_json.egg-info/dependency_links.txt
+-rw-r--r--   0 charlie    (501) staff       (20)      246 2023-06-11 18:43:06.000000 dataclasses-json-0.5.8/dataclasses_json.egg-info/requires.txt
+-rw-r--r--   0 charlie    (501) staff       (20)       17 2023-06-11 18:43:06.000000 dataclasses-json-0.5.8/dataclasses_json.egg-info/top_level.txt
+-rw-r--r--   0 charlie    (501) staff       (20)      645 2023-06-11 02:35:27.000000 dataclasses-json-0.5.8/publish.py
+-rw-r--r--   0 charlie    (501) staff       (20)       46 2020-02-23 14:06:06.000000 dataclasses-json-0.5.8/pyproject.toml
+-rw-r--r--   0 charlie    (501) staff       (20)       38 2023-06-11 18:43:06.793519 dataclasses-json-0.5.8/setup.cfg
+-rw-r--r--   0 charlie    (501) staff       (20)     1159 2023-06-11 18:38:05.000000 dataclasses-json-0.5.8/setup.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-06-11 18:43:06.792880 dataclasses-json-0.5.8/tests/
+-rw-r--r--   0 charlie    (501) staff       (20)     3960 2023-03-18 13:15:21.000000 dataclasses-json-0.5.8/tests/test_annotations.py
+-rw-r--r--   0 charlie    (501) staff       (20)     9918 2022-03-21 14:47:44.000000 dataclasses-json-0.5.8/tests/test_api.py
+-rw-r--r--   0 charlie    (501) staff       (20)     9681 2022-08-14 20:35:15.000000 dataclasses-json-0.5.8/tests/test_collections.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2989 2020-02-23 14:06:56.000000 dataclasses-json-0.5.8/tests/test_dict.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6420 2023-06-11 01:41:14.000000 dataclasses-json-0.5.8/tests/test_enum.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1448 2019-07-08 15:52:19.000000 dataclasses-json-0.5.8/tests/test_examples.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1451 2020-05-29 19:49:41.000000 dataclasses-json-0.5.8/tests/test_exclude.py
+-rw-r--r--   0 charlie    (501) staff       (20)      896 2020-02-23 14:12:41.000000 dataclasses-json-0.5.8/tests/test_global_config.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1241 2019-08-12 00:04:35.000000 dataclasses-json-0.5.8/tests/test_invariants.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3081 2021-06-03 10:39:20.000000 dataclasses-json-0.5.8/tests/test_letter_case.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1141 2020-02-23 14:06:06.000000 dataclasses-json-0.5.8/tests/test_metadata.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1207 2021-06-05 01:16:21.000000 dataclasses-json-0.5.8/tests/test_nested.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1744 2020-02-23 14:06:06.000000 dataclasses-json-0.5.8/tests/test_recursive.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1618 2021-06-03 10:39:20.000000 dataclasses-json-0.5.8/tests/test_schema.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3790 2020-04-21 23:35:26.000000 dataclasses-json-0.5.8/tests/test_time.py
+-rw-r--r--   0 charlie    (501) staff       (20)    12269 2021-06-03 10:39:20.000000 dataclasses-json-0.5.8/tests/test_undefined_parameters.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3904 2020-02-23 14:06:06.000000 dataclasses-json-0.5.8/tests/test_union.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1414 2022-08-14 20:35:15.000000 dataclasses-json-0.5.8/tests/test_unsupported_generics.py
```

### Comparing `dataclasses-json-0.5.7/LICENSE` & `dataclasses-json-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.7/PKG-INFO` & `dataclasses-json-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclasses-json
-Version: 0.5.7
+Version: 0.5.8
 Summary: Easily serialize dataclasses to and from JSON
 Home-page: https://github.com/lidatong/dataclasses-json
 Author: lidatong
 Author-email: charles.dt.li@gmail.com
 License: MIT
 Description: # Dataclasses JSON
         
@@ -526,23 +526,23 @@
         
         ```python
         from dataclasses import dataclass, field
         from dataclasses_json import dataclass_json, config
         from datetime import date
         from marshmallow import fields
         
+        dataclasses_json.cfg.global_config.encoders[date] = date.isoformat
+        dataclasses_json.cfg.global_config.decoders[date] = date.fromisoformat
+        
         @dataclass_json
         @dataclass
         class DataClassWithIsoDatetime:
-            created_at: date = field(
-                metadata=config(
-                    encoder= date.isoformat,
-                    decoder= date.fromisoformat,
-                    mm_field= fields.DateTime(format='iso')
-                ))
+            created_at: date
+            modified_at: date
+            accessed_at: date
         ```
         
         As you can see, you can **override** or **extend** the default codecs by providing a "hook" via a 
         callable:
         - `encoder`: a callable, which will be invoked to convert the field value when encoding to JSON
         - `decoder`: a callable, which will be invoked to convert the JSON value when decoding from JSON
         - `mm_field`: a marshmallow field, which will affect the behavior of any operations involving `.schema()`
```

### Comparing `dataclasses-json-0.5.7/README.md` & `dataclasses-json-0.5.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -518,23 +518,23 @@
 
 ```python
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from datetime import date
 from marshmallow import fields
 
+dataclasses_json.cfg.global_config.encoders[date] = date.isoformat
+dataclasses_json.cfg.global_config.decoders[date] = date.fromisoformat
+
 @dataclass_json
 @dataclass
 class DataClassWithIsoDatetime:
-    created_at: date = field(
-        metadata=config(
-            encoder= date.isoformat,
-            decoder= date.fromisoformat,
-            mm_field= fields.DateTime(format='iso')
-        ))
+    created_at: date
+    modified_at: date
+    accessed_at: date
 ```
 
 As you can see, you can **override** or **extend** the default codecs by providing a "hook" via a 
 callable:
 - `encoder`: a callable, which will be invoked to convert the field value when encoding to JSON
 - `decoder`: a callable, which will be invoked to convert the JSON value when decoding from JSON
 - `mm_field`: a marshmallow field, which will affect the behavior of any operations involving `.schema()`
```

### Comparing `dataclasses-json-0.5.7/dataclasses_json/api.py` & `dataclasses-json-0.5.8/dataclasses_json/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,14 @@
                                    _decode_dataclass)
 from dataclasses_json.mm import (JsonData, SchemaType, build_schema)
 from dataclasses_json.undefined import Undefined
 from dataclasses_json.utils import (_handle_undefined_parameters_safe,
                                     _undefined_parameter_action_safe)
 
 A = TypeVar('A', bound="DataClassJsonMixin")
-B = TypeVar('B')
-C = TypeVar('C')
 Fields = List[Tuple[str, Any]]
 
 
 class DataClassJsonMixin(abc.ABC):
     """
     DataClassJsonMixin is an ABC that functions as a Mixin.
```

### Comparing `dataclasses-json-0.5.7/dataclasses_json/cfg.py` & `dataclasses-json-0.5.8/dataclasses_json/cfg.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.7/dataclasses_json/core.py` & `dataclasses-json-0.5.8/dataclasses_json/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,28 @@
                          _is_dataclass_instance,
                          fields,
                          is_dataclass  # type: ignore
                          )
 from datetime import datetime, timezone
 from decimal import Decimal
 from enum import Enum
-from typing import Any, Collection, Mapping, Union, get_type_hints, Tuple
+from typing import (Any, Collection, Mapping, Union, get_type_hints,
+                    Tuple, TypeVar)
 from uuid import UUID
 
 from typing_inspect import is_union_type  # type: ignore
 
 from dataclasses_json import cfg
 from dataclasses_json.utils import (_get_type_cons, _get_type_origin,
                                     _handle_undefined_parameters_safe,
                                     _is_collection, _is_mapping, _is_new_type,
                                     _is_optional, _isinstance_safe,
+                                    _get_type_arg_param,
+                                    _get_type_args,
+                                    _NO_ARGS,
                                     _issubclass_safe)
 
 Json = Union[dict, list, str, int, float, bool, None]
 
 confs = ['encoder', 'decoder', 'mm_field', 'letter_case', 'exclude']
 FieldOverride = namedtuple('FieldOverride', confs)
 
@@ -85,15 +89,20 @@
         field_config.update(field.metadata.get('dataclasses_json', {}))
         overrides[field.name] = FieldOverride(*map(field_config.get, confs))
     return overrides
 
 
 def _encode_json_type(value, default=_ExtendedEncoder().default):
     if isinstance(value, Json.__args__):  # type: ignore
-        return value
+        if isinstance(value, list):
+            return [_encode_json_type(i) for i in value]
+        elif isinstance(value, dict):
+            return {k: _encode_json_type(v) for k, v in value.items()}
+        else:
+            return value
     return default(value)
 
 
 def _encode_overrides(kvs, overrides, encode_json=False):
     override_kvs = {}
     for k, v in kvs.items():
         if k in overrides:
@@ -228,14 +237,16 @@
                else UUID(field_value))
     else:
         res = field_value
     return res
 
 
 def _is_supported_generic(type_):
+    if type_ is _NO_ARGS:
+        return False
     not_str = not _issubclass_safe(type_, str)
     is_enum = _issubclass_safe(type_, Enum)
     return (not_str and _is_collection(type_)) or _is_optional(
         type_) or is_union_type(type_) or is_enum
 
 
 def _decode_generic(type_, value, infer_missing):
@@ -244,35 +255,37 @@
     elif _issubclass_safe(type_, Enum):
         # Convert to an Enum using the type as a constructor.
         # Assumes a direct match is found.
         res = type_(value)
     # FIXME this is a hack to fix a deeper underlying issue. A refactor is due.
     elif _is_collection(type_):
         if _is_mapping(type_):
-            k_type, v_type = getattr(type_, "__args__", (Any, Any))
+            k_type, v_type = _get_type_args(type_, (Any, Any))
             # a mapping type has `.keys()` and `.values()`
             # (see collections.abc)
             ks = _decode_dict_keys(k_type, value.keys(), infer_missing)
             vs = _decode_items(v_type, value.values(), infer_missing)
             xs = zip(ks, vs)
         else:
-            xs = _decode_items(type_.__args__[0], value, infer_missing)
+            xs = _decode_items(_get_type_arg_param(type_, 0),
+                               value, infer_missing)
 
         # get the constructor if using corresponding generic type in `typing`
         # otherwise fallback on constructing using type_ itself
         try:
             res = _get_type_cons(type_)(xs)
         except (TypeError, AttributeError):
             res = type_(xs)
     else:  # Optional or Union
-        if not hasattr(type_, "__args__"):
+        _args = _get_type_args(type_)
+        if _args is _NO_ARGS:
             # Any, just accept
             res = value
-        elif _is_optional(type_) and len(type_.__args__) == 2:  # Optional
-            type_arg = type_.__args__[0]
+        elif _is_optional(type_) and len(_args) == 2:  # Optional
+            type_arg = _get_type_arg_param(type_, 0)
             if is_dataclass(type_arg) or is_dataclass(value):
                 res = _decode_dataclass(type_arg, value, infer_missing)
             elif _is_supported_generic(type_arg):
                 res = _decode_generic(type_arg, value, infer_missing)
             else:
                 res = _support_extended_types(type_arg, value)
         else:  # Union (already decoded or unsupported 'from_json' used)
@@ -284,15 +297,19 @@
     """
     Because JSON object keys must be strs, we need the extra step of decoding
     them back into the user's chosen python type
     """
     decode_function = key_type
     # handle NoneType keys... it's weird to type a Dict as NoneType keys
     # but it's valid...
-    if key_type is None or key_type == Any:
+    # Issue #341 and PR #346:
+    #   This is a special case for Python 3.7 and Python 3.8.
+    #   By some reason, "unbound" dicts are counted
+    #   as having key type parameter to be TypeVar('KT')
+    if key_type is None or key_type == Any or isinstance(key_type, TypeVar):
         decode_function = key_type = (lambda x: x)
     # handle a nested python dict that has tuples for keys. E.g. for
     # Dict[Tuple[int], int], key_type will be typing.Tuple[int], but
     # decode_function should be tuple, so map() doesn't break.
     #
     # Note: _get_type_origin() will return typing.Tuple for python
     # 3.6 and tuple for 3.7 and higher.
```

### Comparing `dataclasses-json-0.5.7/dataclasses_json/mm.py` & `dataclasses-json-0.5.8/dataclasses_json/mm.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.7/dataclasses_json/stringcase.py` & `dataclasses-json-0.5.8/dataclasses_json/stringcase.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.7/dataclasses_json/undefined.py` & `dataclasses-json-0.5.8/dataclasses_json/undefined.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.7/dataclasses_json/utils.py` & `dataclasses-json-0.5.8/dataclasses_json/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 import sys
 from datetime import datetime, timezone
-from typing import Collection, Mapping, Optional, TypeVar, Any
+from typing import (Collection, Mapping, Optional, TypeVar, Any, Type, Tuple,
+                    Union)
 
 
 def _get_type_cons(type_):
     """More spaghetti logic for 3.6 vs. 3.7"""
     if sys.version_info.minor == 6:
         try:
             cons = type_.__extra__
@@ -22,29 +23,36 @@
             except AttributeError:
                 cons = type_
     else:
         cons = type_.__origin__
     return cons
 
 
+_NO_TYPE_ORIGIN = object()
+
+
 def _get_type_origin(type_):
     """Some spaghetti logic to accommodate differences between 3.6 and 3.7 in
     the typing api"""
     try:
         origin = type_.__origin__
     except AttributeError:
-        if sys.version_info.minor == 6:
-            try:
-                origin = type_.__extra__
-            except AttributeError:
-                origin = type_
-            else:
-                origin = type_ if origin is None else origin
-        else:
+        # Issue #341 and PR #346:
+        # For some cases, the type_.__origin__ exists but is set to None
+        origin = _NO_TYPE_ORIGIN
+
+    if sys.version_info.minor == 6:
+        try:
+            origin = type_.__extra__
+        except AttributeError:
             origin = type_
+        else:
+            origin = type_ if origin in (None, _NO_TYPE_ORIGIN) else origin
+    elif origin is _NO_TYPE_ORIGIN:
+        origin = type_
     return origin
 
 
 def _hasargs(type_, *args):
     try:
         res = all(arg in type_.__args__ for arg in args)
     except AttributeError:
@@ -54,14 +62,50 @@
             return False
         else:
             raise
     else:
         return res
 
 
+class _NoArgs(object):
+    def __bool__(self):
+        return False
+
+    def __len__(self):
+        return 0
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        raise StopIteration
+
+
+_NO_ARGS = _NoArgs()
+
+
+def _get_type_args(tp: Type, default: Tuple[Type, ...] = _NO_ARGS) -> \
+        Union[Tuple[Type, ...], _NoArgs]:
+    if hasattr(tp, '__args__'):
+        if tp.__args__ is not None:
+            return tp.__args__
+    return default
+
+
+def _get_type_arg_param(tp: Type, index: int) -> Union[Type, _NoArgs]:
+    _args = _get_type_args(tp)
+    if _args is not _NO_ARGS:
+        try:
+            return _args[index]
+        except (TypeError, IndexError, NotImplementedError):
+            pass
+
+    return _NO_ARGS
+
+
 def _isinstance_safe(o, t):
     try:
         result = isinstance(o, t)
     except Exception:
         return False
     else:
         return result
```

### Comparing `dataclasses-json-0.5.7/dataclasses_json.egg-info/PKG-INFO` & `dataclasses-json-0.5.8/dataclasses_json.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclasses-json
-Version: 0.5.7
+Version: 0.5.8
 Summary: Easily serialize dataclasses to and from JSON
 Home-page: https://github.com/lidatong/dataclasses-json
 Author: lidatong
 Author-email: charles.dt.li@gmail.com
 License: MIT
 Description: # Dataclasses JSON
         
@@ -526,23 +526,23 @@
         
         ```python
         from dataclasses import dataclass, field
         from dataclasses_json import dataclass_json, config
         from datetime import date
         from marshmallow import fields
         
+        dataclasses_json.cfg.global_config.encoders[date] = date.isoformat
+        dataclasses_json.cfg.global_config.decoders[date] = date.fromisoformat
+        
         @dataclass_json
         @dataclass
         class DataClassWithIsoDatetime:
-            created_at: date = field(
-                metadata=config(
-                    encoder= date.isoformat,
-                    decoder= date.fromisoformat,
-                    mm_field= fields.DateTime(format='iso')
-                ))
+            created_at: date
+            modified_at: date
+            accessed_at: date
         ```
         
         As you can see, you can **override** or **extend** the default codecs by providing a "hook" via a 
         callable:
         - `encoder`: a callable, which will be invoked to convert the field value when encoding to JSON
         - `decoder`: a callable, which will be invoked to convert the JSON value when decoding from JSON
         - `mm_field`: a marshmallow field, which will affect the behavior of any operations involving `.schema()`
```

### Comparing `dataclasses-json-0.5.7/publish.py` & `dataclasses-json-0.5.8/publish.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.7/setup.py` & `dataclasses-json-0.5.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as f:
     readme = f.read()
 
 setup(
     name='dataclasses-json',
-    version='0.5.7',
+    version='0.5.8',
     packages=find_packages(exclude=('tests*',)),
     package_data={"dataclasses_json": ["py.typed"]},
     author='lidatong',
     author_email='charles.dt.li@gmail.com',
     description='Easily serialize dataclasses to and from JSON',
     long_description=readme,
     long_description_content_type='text/markdown',
@@ -21,23 +21,21 @@
         'marshmallow>=3.3.0,<4.0.0',
         'marshmallow-enum>=1.5.1,<2.0.0',
         'typing-inspect>=0.4.0'
     ],
     python_requires='>=3.6',
     extras_require={
         'dev': [
-            'pytest>=6.2.3',
+            'pytest>=7.2.0',
             'ipython',
             'mypy>=0.710',
             'hypothesis',
             'portray',
             'flake8',
             'types-dataclasses;python_version=="3.6"',
             'simplejson'
         ]
     },
     include_package_data=True,
     scripts=['publish.py']
 )
 
-
-
```

