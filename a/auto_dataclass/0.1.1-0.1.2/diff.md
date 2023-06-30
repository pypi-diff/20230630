# Comparing `tmp/auto_dataclass-0.1.1.tar.gz` & `tmp/auto_dataclass-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_dataclass-0.1.1.tar", last modified: Mon Jun 26 13:57:22 2023, max compression
+gzip compressed data, was "auto_dataclass-0.1.2.tar", last modified: Fri Jun 30 06:09:11 2023, max compression
```

## Comparing `auto_dataclass-0.1.1.tar` & `auto_dataclass-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      733 2023-06-26 10:45:19.360030 auto_dataclass-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0       34 2023-06-26 13:42:13.912977 auto_dataclass-0.1.1/.gitignore
--rw-r--r--   0        0        0     1083 2023-06-26 10:54:50.375568 auto_dataclass-0.1.1/LICENSE
--rw-r--r--   0        0        0     2218 2023-06-26 13:31:25.809415 auto_dataclass-0.1.1/README.md
--rw-r--r--   0        0        0      103 2023-06-26 13:31:37.913407 auto_dataclass-0.1.1/auto_dataclass/__init__.py
--rw-r--r--   0        0        0     5339 2023-06-26 08:31:31.487573 auto_dataclass-0.1.1/auto_dataclass/dj_model_to_dataclass.py
--rw-r--r--   0        0        0     4582 2023-06-26 10:25:32.846753 auto_dataclass-0.1.1/poetry.lock
--rw-r--r--   0        0        0      682 2023-06-26 13:56:04.307932 auto_dataclass-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6156 2023-06-26 13:25:12.313667 auto_dataclass-0.1.1/tests/tests_errors.py
--rw-r--r--   0        0        0     3299 2023-06-26 13:25:12.265667 auto_dataclass-0.1.1/tests/tests_to_dto_func.py
--rw-r--r--   0        0        0     3462 2023-06-26 13:25:12.281667 auto_dataclass-0.1.1/tests/tests_to_dto_func_with_recursive.py
--rw-r--r--   0        0        0     2577 1970-01-01 00:00:00.000000 auto_dataclass-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      733 2023-06-26 10:45:19.360030 auto_dataclass-0.1.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       34 2023-06-26 13:42:13.912977 auto_dataclass-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1083 2023-06-26 10:54:50.375568 auto_dataclass-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3398 2023-06-30 05:52:53.057973 auto_dataclass-0.1.2/README.md
+-rw-r--r--   0        0        0      106 2023-06-30 06:05:54.881375 auto_dataclass-0.1.2/auto_dataclass/__init__.py
+-rw-r--r--   0        0        0     4911 2023-06-30 06:04:30.217816 auto_dataclass-0.1.2/auto_dataclass/dj_model_to_dataclass.py
+-rw-r--r--   0        0        0     4582 2023-06-26 10:25:32.846753 auto_dataclass-0.1.2/poetry.lock
+-rw-r--r--   0        0        0      682 2023-06-26 13:56:04.307932 auto_dataclass-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6722 2023-06-30 06:05:16.597558 auto_dataclass-0.1.2/tests/tests_errors.py
+-rw-r--r--   0        0        0     3299 2023-06-26 13:25:12.265667 auto_dataclass-0.1.2/tests/tests_to_dto_func.py
+-rw-r--r--   0        0        0     3400 2023-06-29 21:34:19.675579 auto_dataclass-0.1.2/tests/tests_to_dto_func_with_recursive.py
+-rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 auto_dataclass-0.1.2/PKG-INFO
```

### Comparing `auto_dataclass-0.1.1/.github/workflows/tests.yml` & `auto_dataclass-0.1.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.1/LICENSE` & `auto_dataclass-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.1/auto_dataclass/dj_model_to_dataclass.py` & `auto_dataclass-0.1.2/auto_dataclass/dj_model_to_dataclass.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
+from dataclasses import dataclass, is_dataclass
 from typing import Type, ForwardRef, List, get_origin, Union
 from django.db.models.manager import Manager
 from django.db.models import Model
 
 
 T = Type["T"]
 
@@ -14,40 +14,37 @@
     def to_dto(self, data, dc: dataclass):
         pass
 
 
 class FromOrmToDataclass(ToDTOConverter):
 
     def __init__(self):
-        self._is_recursive = False
-        self._current_dataclass = None
-        self._future_dataclasses = None
+        self._future_dataclasses = []
 
-    def to_dto(self, data: Model, dc: dataclass, is_recursive: bool = False,
+    def to_dto(self, data: Model, dc: dataclass,
                future_dataclasses: List[dataclass] = None) -> dataclass:
-        self._is_recursive = is_recursive
         checked_dc = self._check_dataclass_arg(dc)
-        self._current_dataclass = checked_dc
-        self._future_dataclasses = self._check_future_dataclasses_arg(future_dataclasses)
+        self._future_dataclasses.append(checked_dc)
+        self._check_future_dataclasses_arg(future_dataclasses)
         checked_data = self._is_data_dj_model_type(data)
         return self._to_dataclass_obj(checked_data, checked_dc)
 
     def _to_dataclass_obj(self, data: Model, dc: dataclass) -> dataclass:
         obj_for_dataclass = {}
         for field in dataclasses.fields(dc):
             if self._is_field_name_exists_in_data(data, field.name):
 
                 field_data = getattr(data, field.name)
                 origin_type, is_list = self._get_origin_field_type(field.type)
 
-                if is_list and dataclasses.is_dataclass(origin_type) and field_data is not None:
+                if is_list and is_dataclass(origin_type) and field_data is not None:
                     obj_for_dataclass[field.name] = self._get_list_of_dataclass_objects(
                         field_data, origin_type
                     )
-                elif dataclasses.is_dataclass(origin_type) and field_data is not None:
+                elif is_dataclass(origin_type) and field_data is not None:
                     obj_for_dataclass[field.name] = self._get_dataclass_object(
                         field_data, origin_type
                     )
                 else:
                     obj_for_dataclass[field.name] = field_data
         return dc(**obj_for_dataclass)
 
@@ -76,56 +73,51 @@
     def _get_dataclass_object(self, field_data: Model, field_type: type) -> dataclass:
         return self._to_dataclass_obj(field_data, field_type)
 
     def _get_list_of_dataclass_objects(
         self, field_data: Manager, field_type: T
     ) -> List[dataclass]:
         values_lst = []
-        for orm_obj in field_data.all():
-            values_lst.append(self._to_dataclass_obj(orm_obj, field_type))
+        try:
+            for orm_obj in field_data.all():
+                values_lst.append(self._to_dataclass_obj(orm_obj, field_type))
+        except AttributeError:
+            raise TypeError(f"The {field_data} is not iterable, but specified type is List[{field_type}]")
         return values_lst
 
     def _get_future_object_type(self, obj_type: str) -> dataclass:
-        if self._is_recursive:
-            return self._current_dataclass
         if self._future_dataclasses:
             for dc in self._future_dataclasses:
                 if dc.__name__ == obj_type:
                     return dc
             raise TypeError(
                 f"The 'future_dataclasses' arguments must be defined for future reference '{obj_type}'."
             )
-        raise TypeError(
-            f"The dataclass {self._current_dataclass} has recursive or future relation"
-            f" that was not defined. Please define argument 'is_recursive' for recursive relation or "
-            f"'future_dataclasses' for future relations"
-        )
 
     @staticmethod
     def _check_dataclass_arg(dc: dataclass) -> dataclass:
         if dataclasses.is_dataclass(dc):
             return dc
         raise TypeError(f"The 'dc' arg should be dataclass type, not {type(dc)} type")
 
-    @staticmethod
-    def _check_future_dataclasses_arg(future_dataclasses: List[dataclass] | None) -> List[dataclass] | None:
+    def _check_future_dataclasses_arg(self, future_dataclasses: List[dataclass]) -> None:
         if future_dataclasses is None:
-            return future_dataclasses
+            return
         if not isinstance(future_dataclasses, list):
             raise TypeError(
                 f"The 'future_dataclasses' arguments should be a list of 'dataclass' classes or "
                 f"None type, not {type(future_dataclasses)}."
             )
         for dc in future_dataclasses:
-            if not dataclasses.is_dataclass(dc):
+            if not is_dataclass(dc):
                 raise TypeError(
                     f"The 'future_dataclasses' arguments should be a list of 'dataclass' classes. "
                     f"Received {dc} with type {type(dc)}."
                 )
-        return future_dataclasses
+            self._future_dataclasses.append(dc)
 
     @staticmethod
     def _is_data_dj_model_type(data: Model):
         if isinstance(data, Model):
             return data
         raise TypeError(
             f"Data must be a django.db.models.Model type. Instead, received '{type(data)}'"
```

### Comparing `auto_dataclass-0.1.1/poetry.lock` & `auto_dataclass-0.1.2/poetry.lock`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.1/pyproject.toml` & `auto_dataclass-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.1/tests/tests_errors.py` & `auto_dataclass-0.1.2/tests/tests_errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,40 +60,45 @@
         with self.assertRaises(AttributeError) as cm:
             self.converter.to_dto(mock_model, OuterTestDataclass)
         self.assertEqual(
             f"Field name 'non_existed_field_name' doesn't exist in {mock_model}",
             str(cm.exception)
         )
 
-    def test_error_to_dto_not_checked_is_recursive_arg(self):
+    def test_error_to_dto_incorrect_future_dataclasses_arg_type(self):
         @dataclass
         class RecursiveTestDataclass:
             id: int
-            dc: 'RecursiveTestDataclass'
+            dc: 'FutureTestDataclass'
+
+        @dataclass
+        class FutureTestDataclass:
+            id: int
 
         outer_mock_model = Mock(spec=Model)
         inner_mock_model = Mock(spec=Model)
         inner_mock_model.id = 2
         inner_mock_model.dc = None
         outer_mock_model.id = 1
         outer_mock_model.dc = inner_mock_model
 
+        future_dataclass = "future_dataclasses"
+
         with self.assertRaises(TypeError) as cm:
             self.converter.to_dto(
                 outer_mock_model,
-                RecursiveTestDataclass
+                RecursiveTestDataclass,
+                future_dataclasses=future_dataclass
             )
         self.assertEqual(
-            f"The dataclass {RecursiveTestDataclass} has recursive or future relation"
-            f" that was not defined. Please define argument 'is_recursive' for recursive relation or "
-            f"'future_dataclasses' for future relations",
-            str(cm.exception)
+            f"The 'future_dataclasses' arguments should be a list of 'dataclass' classes or "
+            f"None type, not {type(future_dataclass)}.", str(cm.exception)
         )
 
-    def test_error_to_dto_incorrect_future_dataclasses_arg_type(self):
+    def test_error_incorrect_future_dataclasses_arg_type_value(self):
         @dataclass
         class RecursiveTestDataclass:
             id: int
             dc: 'FutureTestDataclass'
 
         @dataclass
         class FutureTestDataclass:
@@ -108,81 +113,98 @@
 
         future_dataclass = "future_dataclasses"
 
         with self.assertRaises(TypeError) as cm:
             self.converter.to_dto(
                 outer_mock_model,
                 RecursiveTestDataclass,
-                future_dataclasses=future_dataclass
+                future_dataclasses=[future_dataclass]
             )
         self.assertEqual(
-            f"The 'future_dataclasses' arguments should be a list of 'dataclass' classes or "
-            f"None type, not {type(future_dataclass)}.", str(cm.exception)
+            "The 'future_dataclasses' arguments should be a list of 'dataclass' classes. "
+            f"Received {future_dataclass} with type {type(future_dataclass)}.", str(cm.exception)
         )
 
-    def test_error_incorrect_future_dataclasses_arg_type_value(self):
+    def test_error_to_dto_incorrect_future_dataclasses_arg_value(self):
         @dataclass
         class RecursiveTestDataclass:
             id: int
             dc: 'FutureTestDataclass'
 
-        @dataclass
-        class FutureTestDataclass:
+        class FutureTestClass:
             id: int
 
         outer_mock_model = Mock(spec=Model)
         inner_mock_model = Mock(spec=Model)
         inner_mock_model.id = 2
         inner_mock_model.dc = None
         outer_mock_model.id = 1
         outer_mock_model.dc = inner_mock_model
 
-        future_dataclass = "future_dataclasses"
-
         with self.assertRaises(TypeError) as cm:
             self.converter.to_dto(
                 outer_mock_model,
                 RecursiveTestDataclass,
-                future_dataclasses=[future_dataclass]
+                future_dataclasses=[FutureTestClass]
             )
         self.assertEqual(
             "The 'future_dataclasses' arguments should be a list of 'dataclass' classes. "
-            f"Received {future_dataclass} with type {type(future_dataclass)}.", str(cm.exception)
+            f"Received {FutureTestClass} with type {type(FutureTestClass)}.", str(cm.exception)
         )
 
-    def test_error_to_dto_incorrect_future_dataclasses_arg_value(self):
+    def test_error_missed_future_dataclasses_arg(self):
         @dataclass
         class RecursiveTestDataclass:
             id: int
             dc: 'FutureTestDataclass'
 
-        class FutureTestClass:
+        @dataclass
+        class FutureTestDataclass:
             id: int
 
         outer_mock_model = Mock(spec=Model)
         inner_mock_model = Mock(spec=Model)
         inner_mock_model.id = 2
         inner_mock_model.dc = None
         outer_mock_model.id = 1
         outer_mock_model.dc = inner_mock_model
 
         with self.assertRaises(TypeError) as cm:
             self.converter.to_dto(
                 outer_mock_model,
-                RecursiveTestDataclass,
-                future_dataclasses=[FutureTestClass]
+                RecursiveTestDataclass
             )
         self.assertEqual(
-            "The 'future_dataclasses' arguments should be a list of 'dataclass' classes. "
-            f"Received {FutureTestClass} with type {type(FutureTestClass)}.", str(cm.exception)
+            f"The 'future_dataclasses' arguments must be defined for future reference 'FutureTestDataclass'.",
+            str(cm.exception)
+        )
+
+    def test_error_to_dto_incorrect_field_type(self) -> None:
+
+        InnerTestDataclass = self.TestDataclass
+
+        @dataclass
+        class OuterTestDataclass:
+            id: int
+            dc: List[InnerTestDataclass]
+
+        mock_model = Mock(spec=Model)
+        mock_model.id = 1
+        mock_model.dc = self.get_list_db_model_objects()[0]
+
+        with self.assertRaises(TypeError) as cm:
+            self.converter.to_dto(mock_model, OuterTestDataclass)
+        self.assertEqual(
+            f"The {mock_model.dc} is not iterable, but specified type is List[{InnerTestDataclass}]",
+            str(cm.exception)
         )
 
     @staticmethod
     def get_list_db_model_objects():
         model_instance_1 = Mock(spec=Model)
         model_instance_1.id = 1
         model_instance_1.name = "first"
         model_instance_2 = Mock(spec=Model)
         model_instance_2.id = 2
         model_instance_2.name = "second"
 
-        return [model_instance_1, model_instance_2]
+        return [model_instance_1, model_instance_2]
```

### Comparing `auto_dataclass-0.1.1/tests/tests_to_dto_func.py` & `auto_dataclass-0.1.2/tests/tests_to_dto_func.py`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.1/tests/tests_to_dto_func_with_recursive.py` & `auto_dataclass-0.1.2/tests/tests_to_dto_func_with_recursive.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         inner_mock_model.id = 2
         inner_mock_model.dc = None
         outer_mock_model.id = 1
         outer_mock_model.dc = inner_mock_model
 
         result = self.converter.to_dto(
             outer_mock_model,
-            RecursiveTestDataclass,
-            is_recursive=True
+            RecursiveTestDataclass
         )
 
         self.assertIsInstance(result, RecursiveTestDataclass)
         self.assertEqual(result.id, 1)
         self.assertEqual(result.dc, RecursiveTestDataclass(id=2, dc=None))
 
     def test_to_dto_list_recursive_relation(self) -> None:
@@ -54,16 +53,15 @@
 
         outer_mock_model = Mock(spec=Model)
         outer_mock_model.id = 1
         outer_mock_model.dc = mock_related_manager
 
         result = self.converter.to_dto(
             outer_mock_model,
-            RecursiveTestDataclass,
-            is_recursive=True)
+            RecursiveTestDataclass)
 
         self.assertIsInstance(result, RecursiveTestDataclass)
         self.assertEqual(result.id, 1)
         self.assertEqual(result.dc[1], RecursiveTestDataclass(id=2, dc=None))
 
     def test_to_dto_list_future_relations(self) -> None:
         @dataclass
```

