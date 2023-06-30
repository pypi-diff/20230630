# Comparing `tmp/safe_ds-0.8.0.tar.gz` & `tmp/safe_ds-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_ds-0.8.0.tar", max compression
+gzip compressed data, was "safe_ds-0.9.0.tar", max compression
```

## Comparing `safe_ds-0.8.0.tar` & `safe_ds-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,50 @@
--rw-r--r--   0        0        0     1069 2023-03-31 18:30:33.205872 safe_ds-0.8.0/LICENSE
--rw-r--r--   0        0        0     1843 2023-03-31 18:30:33.205872 safe_ds-0.8.0/docs/README.md
--rw-r--r--   0        0        0     1160 2023-03-31 18:31:09.383415 safe_ds-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/__init__.py
--rw-r--r--   0        0        0      115 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/containers/__init__.py
--rw-r--r--   0        0        0    15954 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/containers/_column.py
--rw-r--r--   0        0        0     5847 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/containers/_row.py
--rw-r--r--   0        0        0    36393 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/containers/_table.py
--rw-r--r--   0        0        0     3408 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/containers/_tagged_table.py
--rw-r--r--   0        0        0      132 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/transformation/__init__.py
--rw-r--r--   0        0        0     5652 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/transformation/_imputer.py
--rw-r--r--   0        0        0     4210 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/transformation/_label_encoder.py
--rw-r--r--   0        0        0     4656 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/transformation/_one_hot_encoder.py
--rw-r--r--   0        0        0     3221 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/transformation/_table_transformer.py
--rw-r--r--   0        0        0      113 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/typing/__init__.py
--rw-r--r--   0        0        0     6244 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/typing/_column_type.py
--rw-r--r--   0        0        0     3643 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/data/tabular/typing/_schema.py
--rw-r--r--   0        0        0      350 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/exceptions/__init__.py
--rw-r--r--   0        0        0     2937 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/exceptions/_data_exceptions.py
--rw-r--r--   0        0        0     1106 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/exceptions/_learning_exceptions.py
--rw-r--r--   0        0        0        0 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/__init__.py
--rw-r--r--   0        0        0     2623 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/_util_sklearn.py
--rw-r--r--   0        0        0      320 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/classification/__init__.py
--rw-r--r--   0        0        0     2544 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/classification/_ada_boost.py
--rw-r--r--   0        0        0     2446 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/classification/_classifier.py
--rw-r--r--   0        0        0     2572 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/classification/_decision_tree.py
--rw-r--r--   0        0        0     2653 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/classification/_gradient_boosting_classification.py
--rw-r--r--   0        0        0     2818 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/classification/_k_nearest_neighbors.py
--rw-r--r--   0        0        0     2604 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/classification/_logistic_regression.py
--rw-r--r--   0        0        0     2555 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/classification/_random_forest.py
--rw-r--r--   0        0        0      462 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/regression/__init__.py
--rw-r--r--   0        0        0     2519 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/regression/_ada_boost.py
--rw-r--r--   0        0        0     2551 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/regression/_decision_tree.py
--rw-r--r--   0        0        0     2544 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/regression/_elastic_net_regression.py
--rw-r--r--   0        0        0     2591 2023-03-31 18:30:33.213875 safe_ds-0.8.0/src/safeds/ml/regression/_gradient_boosting_regression.py
--rw-r--r--   0        0        0     2800 2023-03-31 18:30:33.217876 safe_ds-0.8.0/src/safeds/ml/regression/_k_nearest_neighbors.py
--rw-r--r--   0        0        0     2499 2023-03-31 18:30:33.217876 safe_ds-0.8.0/src/safeds/ml/regression/_lasso_regression.py
--rw-r--r--   0        0        0     2557 2023-03-31 18:30:33.217876 safe_ds-0.8.0/src/safeds/ml/regression/_linear_regression.py
--rw-r--r--   0        0        0     2526 2023-03-31 18:30:33.217876 safe_ds-0.8.0/src/safeds/ml/regression/_random_forest.py
--rw-r--r--   0        0        0     4002 2023-03-31 18:30:33.217876 safe_ds-0.8.0/src/safeds/ml/regression/_regressor.py
--rw-r--r--   0        0        0     2499 2023-03-31 18:30:33.217876 safe_ds-0.8.0/src/safeds/ml/regression/_ridge_regression.py
--rw-r--r--   0        0        0     2738 1970-01-01 00:00:00.000000 safe_ds-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-04 17:08:02.202271 safe_ds-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1843 2023-04-04 17:08:02.202271 safe_ds-0.9.0/docs/README.md
+-rw-r--r--   0        0        0     1178 2023-04-04 17:08:28.462272 safe_ds-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/__init__.py
+-rw-r--r--   0        0        0       41 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/__init__.py
+-rw-r--r--   0        0        0       28 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/image/__init__.py
+-rw-r--r--   0        0        0       96 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/image/containers/__init__.py
+-rw-r--r--   0        0        0     3927 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/image/containers/_image.py
+-rw-r--r--   0        0        0      131 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/image/typing/__init__.py
+-rw-r--r--   0        0        0      126 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/image/typing/_image_format.py
+-rw-r--r--   0        0        0       30 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/tabular/__init__.py
+-rw-r--r--   0        0        0      231 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/tabular/containers/__init__.py
+-rw-r--r--   0        0        0    16877 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/tabular/containers/_column.py
+-rw-r--r--   0        0        0     5879 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/tabular/containers/_row.py
+-rw-r--r--   0        0        0    37161 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/tabular/containers/_table.py
+-rw-r--r--   0        0        0     3430 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/tabular/containers/_tagged_table.py
+-rw-r--r--   0        0        0      367 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/tabular/transformation/__init__.py
+-rw-r--r--   0        0        0     5997 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/tabular/transformation/_imputer.py
+-rw-r--r--   0        0        0     4223 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/tabular/transformation/_label_encoder.py
+-rw-r--r--   0        0        0     4646 2023-04-04 17:08:02.206271 safe_ds-0.9.0/src/safeds/data/tabular/transformation/_one_hot_encoder.py
+-rw-r--r--   0        0        0     3100 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/data/tabular/transformation/_table_transformer.py
+-rw-r--r--   0        0        0      369 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/data/tabular/typing/__init__.py
+-rw-r--r--   0        0        0     6288 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/data/tabular/typing/_column_type.py
+-rw-r--r--   0        0        0      454 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/data/tabular/typing/_imputer_strategy.py
+-rw-r--r--   0        0        0     3706 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/data/tabular/typing/_schema.py
+-rw-r--r--   0        0        0      971 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/exceptions/__init__.py
+-rw-r--r--   0        0        0     3054 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/exceptions/_data_exceptions.py
+-rw-r--r--   0        0        0     1786 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/exceptions/_ml_exceptions.py
+-rw-r--r--   0        0        0       36 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/__init__.py
+-rw-r--r--   0        0        0     2923 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/_util_sklearn.py
+-rw-r--r--   0        0        0      525 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/classification/__init__.py
+-rw-r--r--   0        0        0     2704 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/classification/_ada_boost.py
+-rw-r--r--   0        0        0     2679 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/classification/_classifier.py
+-rw-r--r--   0        0        0     2736 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/classification/_decision_tree.py
+-rw-r--r--   0        0        0     2776 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/classification/_gradient_boosting_classification.py
+-rw-r--r--   0        0        0     3080 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/classification/_k_nearest_neighbors.py
+-rw-r--r--   0        0        0     2764 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/classification/_logistic_regression.py
+-rw-r--r--   0        0        0     2749 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/classification/_random_forest.py
+-rw-r--r--   0        0        0      733 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/regression/__init__.py
+-rw-r--r--   0        0        0     2680 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/regression/_ada_boost.py
+-rw-r--r--   0        0        0     2712 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/regression/_decision_tree.py
+-rw-r--r--   0        0        0     2706 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/regression/_elastic_net_regression.py
+-rw-r--r--   0        0        0     2752 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/regression/_gradient_boosting_regression.py
+-rw-r--r--   0        0        0     3058 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/regression/_k_nearest_neighbors.py
+-rw-r--r--   0        0        0     2660 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/regression/_lasso_regression.py
+-rw-r--r--   0        0        0     2718 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/regression/_linear_regression.py
+-rw-r--r--   0        0        0     2725 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/regression/_random_forest.py
+-rw-r--r--   0        0        0     4247 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/regression/_regressor.py
+-rw-r--r--   0        0        0     2660 2023-04-04 17:08:02.210271 safe_ds-0.9.0/src/safeds/ml/regression/_ridge_regression.py
+-rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 safe_ds-0.9.0/PKG-INFO
```

### Comparing `safe_ds-0.8.0/LICENSE` & `safe_ds-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_ds-0.8.0/docs/README.md` & `safe_ds-0.9.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `safe_ds-0.8.0/pyproject.toml` & `safe_ds-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "safe-ds"
-version = "0.8.0"
+version = "0.9.0"
 description = "A user-friendly library for Data Science in Python."
 authors = ["Lars Reimann <mail@larsreimann.com>"]
 license = "MIT"
 readme = "docs/README.md"
 repository = "https://github.com/Safe-DS/Stdlib"
 documentation = "https://safe-ds-stdlib.readthedocs.io"
 keywords = ["data science", "machine learning", "usability", "learnability"]
 packages = [
     { include = "safeds", from = "src"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+ipython = "^8.8.0"
+matplotlib = "^3.6.3"
 pandas = "^1.5.3"
+pillow = "^9.5.0"
 scikit-learn = "^1.2.0"
 seaborn = "^0.12.2"
-ipython = "^8.8.0"
-matplotlib = "^3.6.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.docs.dependencies]
 jupyter = "^1.0.0"
```

### Comparing `safe_ds-0.8.0/src/safeds/data/tabular/containers/_column.py` & `safe_ds-0.9.0/src/safeds/data/tabular/containers/_column.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from __future__ import annotations
 
+import io
 from numbers import Number
-from typing import Any, Callable, Iterable, Iterator, Optional
+from typing import TYPE_CHECKING, Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from IPython.core.display_functions import DisplayHandle, display
+
+from safeds.data.image.containers import Image
+from safeds.data.image.typing import ImageFormat
 from safeds.data.tabular.typing import ColumnType
 from safeds.exceptions import (
     ColumnLengthMismatchError,
     ColumnSizeError,
     IndexOutOfBoundsError,
     NonNumericColumnError,
 )
 
+if TYPE_CHECKING:
+    from collections.abc import Callable, Iterable, Iterator
+
 
 class Column:
     """
     A column is a named collection of values.
 
     Parameters
     ----------
@@ -31,15 +38,15 @@
         The type of the column. If not specified, the type will be inferred from the data.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Dunder methods
     # ------------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, name: str, data: Iterable, type_: Optional[ColumnType] = None) -> None:
+    def __init__(self, name: str, data: Iterable, type_: ColumnType | None = None) -> None:
         self._name: str = name
         self._data: pd.Series = data if isinstance(data, pd.Series) else pd.Series(data)
         # noinspection PyProtectedMember
         self._type: ColumnType = type_ if type_ is not None else ColumnType._from_numpy_dtype(self._data.dtype)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Column):
@@ -163,18 +170,15 @@
 
         Returns
         -------
         result : bool
             True if all match.
 
         """
-        for value in self._data:
-            if not predicate(value):
-                return False
-        return True
+        return all(predicate(value) for value in self._data)
 
     def any(self, predicate: Callable[[Any], bool]) -> bool:
         """
         Check if any value has a given property.
 
         Parameters
         ----------
@@ -183,18 +187,15 @@
 
         Returns
         -------
         result : bool
             True if any match.
 
         """
-        for value in self._data:
-            if predicate(value):
-                return True
-        return False
+        return any(predicate(value) for value in self._data)
 
     def none(self, predicate: Callable[[Any], bool]) -> bool:
         """
         Check if no values has a given property.
 
         Parameters
         ----------
@@ -203,18 +204,15 @@
 
         Returns
         -------
         result : bool
             True if none match.
 
         """
-        for value in self._data:
-            if predicate(value):
-                return False
-        return True
+        return all(not predicate(value) for value in self._data)
 
     def has_missing_values(self) -> bool:
         """
         Return whether the column has missing values.
 
         Returns
         -------
@@ -260,29 +258,29 @@
         ------
         TypeError
             If one of the columns is not numerical.
         """
         if not self._type.is_numeric() or not other_column._type.is_numeric():
             raise NonNumericColumnError(
                 f"Columns must be numerical. {self.name} is {self._type}, "
-                f"{other_column.name} is {other_column._type}."
+                f"{other_column.name} is {other_column._type}.",
             )
         if self._data.size != other_column._data.size:
             raise ColumnLengthMismatchError(
                 f"{self.name} is of size {self._data.size}, "
-                f"{other_column.name} is of size {other_column._data.size}."
+                f"{other_column.name} is of size {other_column._data.size}.",
             )
         return self._data.corr(other_column._data)
 
     def idness(self) -> float:
-        """
-        Calculate the idness of this column, which we define as
+        r"""
+        Calculate the idness of this column, which we define as.
 
         $$
-        \\frac{\\text{number of different values}}{\\text{number of rows}}
+        \frac{\text{number of different values}}{\text{number of rows}}
         $$
 
         Returns
         -------
         idness : float
             The idness of the column.
 
@@ -365,15 +363,15 @@
         """
         if not self._type.is_numeric():
             raise NonNumericColumnError(f"{self.name} is of type {self._type}.")
         return self._data.min()
 
     def missing_value_ratio(self) -> float:
         """
-        Return the ratio of null values to the total number of elements in the column
+        Return the ratio of null values to the total number of elements in the column.
 
         Returns
         -------
         ratio : float
             The ratio of null values to the total number of elements in the column.
         """
         if self._data.size == 0:
@@ -388,19 +386,19 @@
         -------
         List :
             Returns a list with the most common values.
         """
         return self._data.mode().tolist()
 
     def stability(self) -> float:
-        """
-        Calculate the stability of this column, which we define as
+        r"""
+        Calculate the stability of this column, which we define as.
 
         $$
-        \\frac{\\text{number of occurrences of most common non-null value}}{\\text{number of non-null values}}
+        \frac{\text{number of occurrences of most common non-null value}}{\text{number of non-null values}}
         $$
 
         Returns
         -------
         stability : float
             The stability of the column.
 
@@ -419,15 +417,15 @@
 
         Returns
         -------
         sum : float
             The standard deviation of all values.
 
         Raises
-        ---
+        ------
         NonNumericColumnError
             If the data contains non-numerical data.
 
         """
         if not self.type.is_numeric():
             raise NonNumericColumnError(f"{self.name} is of type {self._type}.")
         return self._data.std()
@@ -438,15 +436,15 @@
 
         Returns
         -------
         sum : float
             The sum of all values.
 
         Raises
-        ---
+        ------
         NonNumericColumnError
             If the data contains non-numerical data.
 
         """
         if not self.type.is_numeric():
             raise NonNumericColumnError(f"{self.name} is of type {self._type}.")
         return self._data.sum()
@@ -457,86 +455,114 @@
 
         Returns
         -------
         sum : float
             The variance of all values.
 
         Raises
-        ---
+        ------
         NonNumericColumnError
             If the data contains non-numerical data.
 
         """
         if not self.type.is_numeric():
             raise NonNumericColumnError(f"{self.name} is of type {self._type}.")
 
         return self._data.var()
 
     # ------------------------------------------------------------------------------------------------------------------
     # Plotting
     # ------------------------------------------------------------------------------------------------------------------
 
-    def boxplot(self) -> None:
+    def boxplot(self) -> Image:
         """
         Plot this column in a boxplot. This function can only plot real numerical data.
 
-        Raises
+        Returns
         -------
+        plot: Image
+            The plot as an image.
+
+        Raises
+        ------
         TypeError
             If the column contains non-numerical data or complex data.
         """
         for data in self._data:
             if not isinstance(data, int) and not isinstance(data, float) and not isinstance(data, complex):
                 raise NonNumericColumnError(self.name)
             if isinstance(data, complex):
                 raise TypeError(
                     "The column contains complex data. Boxplots cannot plot the imaginary part of complex "
-                    "data. Please provide a Column with only real numbers"
+                    "data. Please provide a Column with only real numbers",
                 )
+
+        fig = plt.figure()
         ax = sns.boxplot(data=self._data)
         ax.set(xlabel=self.name)
         plt.tight_layout()
-        plt.show()
 
-    def histogram(self) -> None:
+        buffer = io.BytesIO()
+        fig.savefig(buffer, format="png")
+        plt.close()  # Prevents the figure from being displayed directly
+        buffer.seek(0)
+        return Image(buffer, ImageFormat.PNG)
+
+    def histogram(self) -> Image:
         """
         Plot a column in a histogram.
-        """
 
+        Returns
+        -------
+        plot: Image
+            The plot as an image.
+        """
+        fig = plt.figure()
         ax = sns.histplot(data=self._data)
         ax.set_xticks(ax.get_xticks())
         ax.set(xlabel=self.name)
         ax.set_xticklabels(
-            ax.get_xticklabels(), rotation=45, horizontalalignment="right"
+            ax.get_xticklabels(),
+            rotation=45,
+            horizontalalignment="right",
         )  # rotate the labels of the x Axis to prevent the chance of overlapping of the labels
         plt.tight_layout()
-        plt.show()
+
+        buffer = io.BytesIO()
+        fig.savefig(buffer, format="png")
+        plt.close()  # Prevents the figure from being displayed directly
+        buffer.seek(0)
+        return Image(buffer, ImageFormat.PNG)
 
     # ------------------------------------------------------------------------------------------------------------------
-    # Other
+    # IPython integration
     # ------------------------------------------------------------------------------------------------------------------
 
-    def _count_missing_values(self) -> int:
-        """
-        Return the number of null values in the column.
-
-        Returns
-        -------
-        count : int
-            The number of null values.
-        """
-        return self._data.isna().sum()
-
     def _ipython_display_(self) -> DisplayHandle:
         """
         Return a display object for the column to be used in Jupyter Notebooks.
 
         Returns
         -------
         output : DisplayHandle
             Output object.
         """
         tmp = self._data.to_frame()
         tmp.columns = [self.name]
 
         with pd.option_context("display.max_rows", tmp.shape[0], "display.max_columns", tmp.shape[1]):
             return display(tmp)
+
+    # ------------------------------------------------------------------------------------------------------------------
+    # Other
+    # ------------------------------------------------------------------------------------------------------------------
+
+    def _count_missing_values(self) -> int:
+        """
+        Return the number of null values in the column.
+
+        Returns
+        -------
+        count : int
+            The number of null values.
+        """
+        return self._data.isna().sum()
```

### Comparing `safe_ds-0.8.0/src/safeds/data/tabular/containers/_row.py` & `safe_ds-0.9.0/src/safeds/data/tabular/containers/_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from collections.abc import Iterable, Iterator
 from hashlib import md5
-from typing import Any, Iterable, Iterator, Optional
+from typing import Any
 
 import pandas as pd
 from IPython.core.display_functions import DisplayHandle, display
 from pandas.core.util.hashing import hash_pandas_object
+
 from safeds.data.tabular.typing import ColumnType, Schema
 from safeds.exceptions import UnknownColumnNameError
 
 
 class Row:
     """
     A row is a collection of values, where each value is associated with a column name.
@@ -20,15 +22,15 @@
         The schema of the row.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Dunder methods
     # ------------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, data: Iterable, schema: Optional[Schema] = None):
+    def __init__(self, data: Iterable, schema: Schema | None = None):
         self._data: pd.Series = data if isinstance(data, pd.Series) else pd.Series(data)
         self._data = self._data.reset_index(drop=True)
 
         self.schema: Schema
         if schema is not None:
             self.schema = schema
         else:
@@ -92,14 +94,15 @@
             raise UnknownColumnNameError([column_name])
         # noinspection PyProtectedMember
         return self._data[self.schema._get_column_index_by_name(column_name)]
 
     def has_column(self, column_name: str) -> bool:
         """
         Return whether the row contains a given column.
+
         Alias for self.schema.hasColumn(column_name: str) -> bool.
 
         Parameters
         ----------
         column_name : str
             The name of the column.
 
@@ -109,26 +112,28 @@
             True, if row contains the column.
         """
         return self.schema.has_column(column_name)
 
     def get_column_names(self) -> list[str]:
         """
         Return a list of all column names saved in this schema.
+
         Alias for self.schema.get_column_names() -> list[str].
 
         Returns
         -------
         column_names : list[str]
             The column names.
         """
         return self.schema.get_column_names()
 
     def get_type_of_column(self, column_name: str) -> ColumnType:
         """
         Return the type of a specified column.
+
         Alias for self.schema.get_type_of_column(column_name: str) -> ColumnType.
 
         Parameters
         ----------
         column_name : str
             The name of the column.
 
@@ -156,15 +161,15 @@
         -------
         count : int
             The number of columns.
         """
         return len(self._data)
 
     # ------------------------------------------------------------------------------------------------------------------
-    # Other
+    # IPython integration
     # ------------------------------------------------------------------------------------------------------------------
 
     def _ipython_display_(self) -> DisplayHandle:
         """
         Return a display object for the column to be used in Jupyter Notebooks.
 
         Returns
```

### Comparing `safe_ds-0.8.0/src/safeds/data/tabular/containers/_table.py` & `safe_ds-0.9.0/src/safeds/data/tabular/containers/_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 from __future__ import annotations
 
 import functools
-import os.path
+import io
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional, Union
+from typing import TYPE_CHECKING, Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from IPython.core.display_functions import DisplayHandle, display
 from pandas import DataFrame, Series
+from scipy import stats
+
+from safeds.data.image.containers import Image
+from safeds.data.image.typing import ImageFormat
 from safeds.data.tabular.typing import ColumnType, Schema
 from safeds.exceptions import (
     ColumnLengthMismatchError,
     ColumnSizeError,
     DuplicateColumnNameError,
     IndexOutOfBoundsError,
     MissingDataError,
     NonNumericColumnError,
     SchemaMismatchError,
     UnknownColumnNameError,
 )
-from scipy import stats
 
 from ._column import Column
 from ._row import Row
 
 if TYPE_CHECKING:
+    from collections.abc import Callable, Iterable
+
     from ._tagged_table import TaggedTable
 
 
 # noinspection PyProtectedMember
 class Table:
     """
     A table is a two-dimensional collection of data. It can either be seen as a list of rows or as a list of columns.
@@ -40,15 +45,15 @@
     ----------
     data : typing.Iterable
         The data.
     schema : Optional[Schema]
         The schema of the table. If not specified, the schema will be inferred from the data.
 
     Raises
-    ----------
+    ------
     MissingSchemaError
         If the table is empty and no schema is specified.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Creation
     # ------------------------------------------------------------------------------------------------------------------
@@ -71,21 +76,18 @@
         Raises
         ------
         FileNotFoundError
             If the specified file does not exist.
         ValueError
             If the file could not be read.
         """
-
         try:
             return Table(pd.read_csv(path))
         except FileNotFoundError as exception:
             raise FileNotFoundError(f'File "{path}" does not exist') from exception
-        except Exception as exception:
-            raise ValueError(f'Could not read file from "{path}" as CSV') from exception
 
     @staticmethod
     def from_json_file(path: str) -> Table:
         """
         Read data from a JSON file into a table.
 
         Parameters
@@ -101,21 +103,18 @@
         Raises
         ------
         FileNotFoundError
             If the specified file does not exist.
         ValueError
             If the file could not be read.
         """
-
         try:
             return Table(pd.read_json(path))
         except FileNotFoundError as exception:
             raise FileNotFoundError(f'File "{path}" does not exist') from exception
-        except Exception as exception:
-            raise ValueError(f'Could not read file from "{path}" as JSON') from exception
 
     @staticmethod
     def from_columns(columns: list[Column]) -> Table:
         """
         Return a table created from a list of columns.
 
         Parameters
@@ -139,15 +138,15 @@
             raise MissingDataError("This function requires at least one column.")
 
         dataframe: DataFrame = pd.DataFrame()
 
         for column in columns:
             if column._data.size != columns[0]._data.size:
                 raise ColumnLengthMismatchError(
-                    "\n".join([f"{column.name}: {column._data.size}" for column in columns])
+                    "\n".join([f"{column.name}: {column._data.size}" for column in columns]),
                 )
             dataframe[column.name] = column._data
 
         return Table(dataframe)
 
     @staticmethod
     def from_rows(rows: list[Row]) -> Table:
@@ -175,26 +174,26 @@
             raise MissingDataError("This function requires at least one row.")
 
         schema_compare: Schema = rows[0].schema
         row_array: list[Series] = []
 
         for row in rows:
             if schema_compare != row.schema:
-                raise SchemaMismatchError()
+                raise SchemaMismatchError
             row_array.append(row._data)
 
         dataframe: DataFrame = pd.DataFrame(row_array)
         dataframe.columns = schema_compare.get_column_names()
         return Table(dataframe)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Dunder methods
     # ------------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, data: Iterable, schema: Optional[Schema] = None):
+    def __init__(self, data: Iterable, schema: Schema | None = None):
         self._data: pd.Dataframe = data if isinstance(data, pd.DataFrame) else pd.DataFrame(data)
         self._schema: Schema = Schema._from_dataframe(self._data) if schema is None else schema
 
         if self._data.empty:
             self._data = pd.DataFrame(columns=self._schema.get_column_names())
 
         self._data = self._data.reset_index(drop=True)
@@ -270,14 +269,15 @@
             return output_column
 
         raise UnknownColumnNameError([column_name])
 
     def has_column(self, column_name: str) -> bool:
         """
         Return whether the table contains a given column.
+
         Alias for self.schema.hasColumn(column_name: str) -> bool.
 
         Parameters
         ----------
         column_name : str
             The name of the column.
 
@@ -287,26 +287,28 @@
             True if the column exists.
         """
         return self._schema.has_column(column_name)
 
     def get_column_names(self) -> list[str]:
         """
         Return a list of all column names in this table.
+
         Alias for self.schema.get_column_names() -> list[str].
 
         Returns
         -------
         column_names : list[str]
             The list of the column names.
         """
         return self._schema.get_column_names()
 
     def get_type_of_column(self, column_name: str) -> ColumnType:
         """
         Return the type of the given column.
+
         Alias for self.schema.get_type_of_column(column_name: str) -> ColumnType.
 
         Parameters
         ----------
         column_name : str
             The name of the column to be queried.
 
@@ -376,15 +378,14 @@
         Return a table with a number of statistical key values.
 
         Returns
         -------
         result : Table
             The table with statistics.
         """
-
         columns = self.to_columns()
         result = pd.DataFrame()
         statistics = {}
 
         for column in columns:
             statistics = {
                 "maximum": column.maximum,
@@ -406,15 +407,15 @@
                     values.append(str(function()))
                 except NonNumericColumnError:
                     values.append("-")
 
             result = pd.concat([result, pd.DataFrame(values)], axis=1)
 
         result = pd.concat([pd.DataFrame(list(statistics.keys())), result], axis=1)
-        result.columns = ["metrics"] + self.get_column_names()
+        result.columns = ["metrics", *self.get_column_names()]
 
         return Table(result)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Transformations
     # ------------------------------------------------------------------------------------------------------------------
 
@@ -443,30 +444,30 @@
             raise ColumnSizeError(str(self.count_rows()), str(column._data.size))
 
         result = self._data.copy()
         result.columns = self._schema.get_column_names()
         result[column.name] = column._data
         return Table(result)
 
-    def add_columns(self, columns: Union[list[Column], Table]) -> Table:
+    def add_columns(self, columns: list[Column] | Table) -> Table:
         """
         Add multiple columns to the table.
 
         Parameters
         ----------
         columns : list[Column] or Table
             The columns to be added.
 
         Returns
         -------
         result: Table
             A new table combining the original table and the given columns.
 
         Raises
-        --------
+        ------
         ColumnSizeError
             If at least one of the column sizes from the provided column list does not match the table.
         DuplicateColumnNameError
             If at least one column name from the provided column list already exists in the table.
         """
         if isinstance(columns, Table):
             columns = columns.to_columns()
@@ -494,20 +495,20 @@
         Returns
         -------
         table : Table
             A new table with the added row at the end.
 
         """
         if self._schema != row.schema:
-            raise SchemaMismatchError()
+            raise SchemaMismatchError
         new_df = pd.concat([self._data, row._data.to_frame().T]).infer_objects()
         new_df.columns = self._schema.get_column_names()
         return Table(new_df)
 
-    def add_rows(self, rows: Union[list[Row], Table]) -> Table:
+    def add_rows(self, rows: list[Row] | Table) -> Table:
         """
         Add multiple rows to a table.
 
         Parameters
         ----------
         rows : list[Row] or Table
             The rows to be added.
@@ -518,15 +519,15 @@
             A new table which combines the original table and the given rows.
         """
         if isinstance(rows, Table):
             rows = rows.to_rows()
         result = self._data
         for row in rows:
             if self._schema != row.schema:
-                raise SchemaMismatchError()
+                raise SchemaMismatchError
         result = pd.concat([result, *[row._data.to_frame().T for row in rows]]).infer_objects()
         result.columns = self._schema.get_column_names()
         return Table(result)
 
     def filter_rows(self, query: Callable[[Row], bool]) -> Table:
         """
         Return a table with rows filtered by Callable (e.g. lambda function).
@@ -573,15 +574,15 @@
             if not self._schema.has_column(name):
                 invalid_columns.append(name)
             else:
                 column_indices.append(self._schema._get_column_index_by_name(name))
         if len(invalid_columns) != 0:
             raise UnknownColumnNameError(invalid_columns)
         transformed_data = self._data[column_indices]
-        transformed_data.columns = list(name for name in self._schema.get_column_names() if name in column_names)
+        transformed_data.columns = [name for name in self._schema.get_column_names() if name in column_names]
         return Table(transformed_data)
 
     def remove_columns(self, column_names: list[str]) -> Table:
         """
         Return a table without the given column(s).
 
         Parameters
@@ -605,15 +606,15 @@
             if not self._schema.has_column(name):
                 invalid_columns.append(name)
             else:
                 column_indices.append(self._schema._get_column_index_by_name(name))
         if len(invalid_columns) != 0:
             raise UnknownColumnNameError(invalid_columns)
         transformed_data = self._data.drop(labels=column_indices, axis="columns")
-        transformed_data.columns = list(name for name in self._schema.get_column_names() if name not in column_names)
+        transformed_data.columns = [name for name in self._schema.get_column_names() if name not in column_names]
         return Table(transformed_data)
 
     def remove_columns_with_missing_values(self) -> Table:
         """
         Return a table without the columns that contain missing values.
 
         Returns
@@ -640,17 +641,17 @@
         Return a copy of the table with every duplicate row removed.
 
         Returns
         -------
         result : Table
             The table with the duplicate rows removed.
         """
-        df = self._data.drop_duplicates(ignore_index=True)
-        df.columns = self._schema.get_column_names()
-        return Table(df)
+        result = self._data.drop_duplicates(ignore_index=True)
+        result.columns = self._schema.get_column_names()
+        return Table(result)
 
     def remove_rows_with_missing_values(self) -> Table:
         """
         Return a table without the rows that contain missing values.
 
         Returns
         -------
@@ -776,16 +777,16 @@
         """
         new_df = self._data.sample(frac=1.0)
         new_df.columns = self._schema.get_column_names()
         return Table(new_df)
 
     def slice_rows(
         self,
-        start: Optional[int] = None,
-        end: Optional[int] = None,
+        start: int | None = None,
+        end: int | None = None,
         step: int = 1,
     ) -> Table:
         """
         Slice a part of the table into a new table.
 
         Parameters
         ----------
@@ -798,42 +799,41 @@
 
         Returns
         -------
         result : Table
             The resulting table.
 
         Raises
-        -------
+        ------
         ValueError
             If the index is out of bounds.
         """
-
         if start is None:
             start = 0
 
         if end is None:
             end = self.count_rows()
 
         if start < 0 or end < 0 or start >= self.count_rows() or end > self.count_rows() or end < start:
-            raise ValueError("the given index is out of bounds")
+            raise ValueError("The given index is out of bounds")
 
         new_df = self._data.iloc[start:end:step]
         new_df.columns = self._schema.get_column_names()
         return Table(new_df)
 
     def sort_columns(
         self,
         comparator: Callable[[Column, Column], int] = lambda col1, col2: (col1.name > col2.name)
         - (col1.name < col2.name),
     ) -> Table:
         """
-        Sort the columns of a `Table` with the given comparator and return a new `Table`. The original table is not
-        modified.
+        Sort the columns of a `Table` with the given comparator and return a new `Table`.
 
-        The comparator is a function that takes two columns `col1` and `col2` and returns an integer:
+        The original table is not modified. The comparator is a function that takes two columns `col1` and `col2` and
+        returns an integer:
 
         * If `col1` should be ordered before `col2`, the function should return a negative number.
         * If `col1` should be ordered after `col2`, the function should return a positive number.
         * If the original order of `col1` and `col2` should be kept, the function should return 0.
 
         If no comparator is given, the columns will be sorted alphabetically by their name.
 
@@ -849,18 +849,18 @@
         """
         columns = self.to_columns()
         columns.sort(key=functools.cmp_to_key(comparator))
         return Table.from_columns(columns)
 
     def sort_rows(self, comparator: Callable[[Row, Row], int]) -> Table:
         """
-        Sort the rows of a `Table` with the given comparator and return a new `Table`. The original table is not
-        modified.
+        Sort the rows of a `Table` with the given comparator and return a new `Table`.
 
-        The comparator is a function that takes two rows `row1` and `row2` and returns an integer:
+        The original table is not modified. The comparator is a function that takes two rows `row1` and `row2` and
+        returns an integer:
 
         * If `row1` should be ordered before `row2`, the function should return a negative number.
         * If `row1` should be ordered after `row2`, the function should return a positive number.
         * If the original order of `row1` and `row2` should be kept, the function should return 0.
 
         Parameters
         ----------
@@ -877,15 +877,15 @@
         return Table.from_rows(rows)
 
     def split(self, percentage_in_first: float) -> tuple[Table, Table]:
         """
         Split the table into two new tables.
 
         Parameters
-        -------
+        ----------
         percentage_in_first : float
             The desired size of the first table in percentage to the given table.
 
         Returns
         -------
         result : (Table, Table)
             A tuple containing the two resulting tables. The first table has the specified size, the second table
@@ -896,15 +896,15 @@
         if percentage_in_first <= 0 or percentage_in_first >= 1:
             raise ValueError("the given percentage is not in range")
         return (
             self.slice_rows(0, round(percentage_in_first * self.count_rows())),
             self.slice_rows(round(percentage_in_first * self.count_rows())),
         )
 
-    def tag_columns(self, target_name: str, feature_names: Optional[list[str]] = None) -> TaggedTable:
+    def tag_columns(self, target_name: str, feature_names: list[str] | None = None) -> TaggedTable:
         """
         Mark the columns of the table as target column or feature columns. The original table is not modified.
 
         Parameters
         ----------
         target_name : str
             Name of the target column.
@@ -912,15 +912,14 @@
             Names of the feature columns. If None, all columns except the target column are used.
 
         Returns
         -------
         tagged_table : TaggedTable
             A new tagged table with the given target and feature names.
         """
-        # pylint: disable=import-outside-toplevel
         from ._tagged_table import TaggedTable
 
         return TaggedTable(self._data, target_name, feature_names, self._schema)
 
     def transform_column(self, name: str, transformer: Callable[[Row], Any]) -> Table:
         """
         Transform provided column by calling provided transformer.
@@ -942,133 +941,173 @@
             return self.replace_column(name, result)
         raise UnknownColumnNameError([name])
 
     # ------------------------------------------------------------------------------------------------------------------
     # Plotting
     # ------------------------------------------------------------------------------------------------------------------
 
-    def correlation_heatmap(self) -> None:
+    def correlation_heatmap(self) -> Image:
         """
         Plot a correlation heatmap for all numerical columns of this `Table`.
+
+        Returns
+        -------
+        plot: Image
+            The plot as an image.
         """
         only_numerical = self.remove_columns_with_non_numerical_values()
 
+        fig = plt.figure()
         sns.heatmap(
             data=only_numerical._data.corr(),
             vmin=-1,
             vmax=1,
             xticklabels=only_numerical.get_column_names(),
             yticklabels=only_numerical.get_column_names(),
             cmap="vlag",
         )
         plt.tight_layout()
-        plt.show()
 
-    def lineplot(self, x_column_name: str, y_column_name: str) -> None:
+        buffer = io.BytesIO()
+        fig.savefig(buffer, format="png")
+        plt.close()  # Prevents the figure from being displayed directly
+        buffer.seek(0)
+        return Image(buffer, format_=ImageFormat.PNG)
+
+    def lineplot(self, x_column_name: str, y_column_name: str) -> Image:
         """
-        Plot two columns against each other in a lineplot. If there are multiple x-values for a y-value,
-        the resulting plot will consist of a line representing the mean and the lower-transparency area around the line
-        representing the 95% confidence interval.
+        Plot two columns against each other in a lineplot.
+
+        If there are multiple x-values for a y-value, the resulting plot will consist of a line representing the mean
+        and the lower-transparency area around the line representing the 95% confidence interval.
 
         Parameters
         ----------
         x_column_name : str
             The column name of the column to be plotted on the x-Axis.
         y_column_name : str
             The column name of the column to be plotted on the y-Axis.
 
+        Returns
+        -------
+        plot: Image
+            The plot as an image.
+
         Raises
-        ---------
+        ------
         UnknownColumnNameError
             If either of the columns do not exist.
         """
         if not self.has_column(x_column_name):
             raise UnknownColumnNameError([x_column_name])
         if not self.has_column(y_column_name):
             raise UnknownColumnNameError([y_column_name])
 
+        fig = plt.figure()
         ax = sns.lineplot(
             data=self._data,
             x=self._schema._get_column_index_by_name(x_column_name),
             y=self._schema._get_column_index_by_name(y_column_name),
         )
         ax.set(xlabel=x_column_name, ylabel=y_column_name)
         ax.set_xticks(ax.get_xticks())
         ax.set_xticklabels(
-            ax.get_xticklabels(), rotation=45, horizontalalignment="right"
+            ax.get_xticklabels(),
+            rotation=45,
+            horizontalalignment="right",
         )  # rotate the labels of the x Axis to prevent the chance of overlapping of the labels
         plt.tight_layout()
-        plt.show()
 
-    def scatterplot(self, x_column_name: str, y_column_name: str) -> None:
+        buffer = io.BytesIO()
+        fig.savefig(buffer, format="png")
+        plt.close()  # Prevents the figure from being displayed directly
+        buffer.seek(0)
+        return Image(buffer, format_=ImageFormat.PNG)
+
+    def scatterplot(self, x_column_name: str, y_column_name: str) -> Image:
         """
         Plot two columns against each other in a scatterplot.
 
         Parameters
         ----------
         x_column_name : str
             The column name of the column to be plotted on the x-Axis.
         y_column_name : str
             The column name of the column to be plotted on the y-Axis.
 
+        Returns
+        -------
+        plot: Image
+            The plot as an image.
+
         Raises
-        ---------
+        ------
         UnknownColumnNameError
             If either of the columns do not exist.
         """
         if not self.has_column(x_column_name):
             raise UnknownColumnNameError([x_column_name])
         if not self.has_column(y_column_name):
             raise UnknownColumnNameError([y_column_name])
 
+        fig = plt.figure()
         ax = sns.scatterplot(
             data=self._data,
             x=self._schema._get_column_index_by_name(x_column_name),
             y=self._schema._get_column_index_by_name(y_column_name),
         )
         ax.set(xlabel=x_column_name, ylabel=y_column_name)
         ax.set_xticks(ax.get_xticks())
         ax.set_xticklabels(
-            ax.get_xticklabels(), rotation=45, horizontalalignment="right"
+            ax.get_xticklabels(),
+            rotation=45,
+            horizontalalignment="right",
         )  # rotate the labels of the x Axis to prevent the chance of overlapping of the labels
         plt.tight_layout()
-        plt.show()
+
+        buffer = io.BytesIO()
+        fig.savefig(buffer, format="png")
+        plt.close()  # Prevents the figure from being displayed directly
+        buffer.seek(0)
+        return Image(buffer, format_=ImageFormat.PNG)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Conversion
     # ------------------------------------------------------------------------------------------------------------------
 
     def to_csv_file(self, path: str) -> None:
         """
         Write the data from the table into a CSV file.
-        If the file and/or the directories do not exist they will be created.
-        If the file already exists it will be overwritten.
+
+        If the file and/or the directories do not exist they will be created. If the file already exists it will be
+        overwritten.
 
         Parameters
         ----------
         path : str
             The path to the output file.
         """
-        Path(os.path.dirname(path)).mkdir(parents=True, exist_ok=True)
+        Path(path).parent.mkdir(parents=True, exist_ok=True)
         data_to_csv = self._data.copy()
         data_to_csv.columns = self._schema.get_column_names()
         data_to_csv.to_csv(path, index=False)
 
     def to_json_file(self, path: str) -> None:
         """
         Write the data from the table into a JSON file.
-        If the file and/or the directories do not exist, they will be created.
-        If the file already exists it will be overwritten.
+
+        If the file and/or the directories do not exist, they will be created. If the file already exists it will be
+        overwritten.
 
         Parameters
         ----------
         path : str
             The path to the output file.
         """
-        Path(os.path.dirname(path)).mkdir(parents=True, exist_ok=True)
+        Path(path).parent.mkdir(parents=True, exist_ok=True)
         data_to_json = self._data.copy()
         data_to_json.columns = self._schema.get_column_names()
         data_to_json.to_json(path)
 
     def to_columns(self) -> list[Column]:
         """
         Return a list of the columns.
@@ -1088,15 +1127,15 @@
         -------
         rows : list[Row]
             List of rows.
         """
         return [Row(series_row, self._schema) for (_, series_row) in self._data.iterrows()]
 
     # ------------------------------------------------------------------------------------------------------------------
-    # Other
+    # IPython integration
     # ------------------------------------------------------------------------------------------------------------------
 
     def _ipython_display_(self) -> DisplayHandle:
         """
         Return a display object for the column to be used in Jupyter Notebooks.
 
         Returns
```

### Comparing `safe_ds-0.8.0/src/safeds/data/tabular/containers/_tagged_table.py` & `safe_ds-0.9.0/src/safeds/data/tabular/containers/_tagged_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Iterable, Optional
+from collections.abc import Iterable
 
 from IPython.core.display_functions import DisplayHandle
+
 from safeds.data.tabular.containers import Column, Table
 from safeds.data.tabular.typing import Schema
 
 
 class TaggedTable(Table):
     """
     A tagged table is a table that additionally knows which columns are features and which are the target to predict.
@@ -25,16 +26,16 @@
     # Dunder methods
     # ------------------------------------------------------------------------------------------------------------------
 
     def __init__(
         self,
         data: Iterable,
         target_name: str,
-        feature_names: Optional[list[str]] = None,
-        schema: Optional[Schema] = None,
+        feature_names: list[str] | None = None,
+        schema: Schema | None = None,
     ):
         super().__init__(data, schema)
 
         # If no feature names are specified, use all columns except the target column
         if feature_names is None:
             feature_names = self.get_column_names()
             if target_name in feature_names:
@@ -68,23 +69,23 @@
         return self._features
 
     @property
     def target(self) -> Column:
         return self._target
 
     # ------------------------------------------------------------------------------------------------------------------
-    # Other
+    # IPython integration
     # ------------------------------------------------------------------------------------------------------------------
 
     def _ipython_display_(self) -> DisplayHandle:
         """
         Return a display object for the column to be used in Jupyter Notebooks.
 
         Returns
         -------
         output : DisplayHandle
             Output object.
         """
         tmp = self._features.add_column(self._target)
         header_info = "Target Column is '" + self._target.name + "'\n"
-        print(header_info)
+        print(header_info)  # noqa: T201
         return tmp._ipython_display_()
```

### Comparing `safe_ds-0.8.0/src/safeds/data/tabular/transformation/_imputer.py` & `safe_ds-0.9.0/src/safeds/data/tabular/transformation/_imputer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
-from typing import Any, Optional
+from typing import Any
 
 import pandas as pd
-from safeds.data.tabular.containers import Table
-from safeds.data.tabular.transformation._table_transformer import TableTransformer
-from safeds.exceptions import NotFittedError, UnknownColumnNameError
 from sklearn.impute import SimpleImputer as sk_SimpleImputer
 
-
-class ImputerStrategy(ABC):
-    @abstractmethod
-    def _augment_imputer(self, imputer: sk_SimpleImputer) -> None:
-        pass
+from safeds.data.tabular.containers import Table
+from safeds.data.tabular.transformation._table_transformer import TableTransformer
+from safeds.data.tabular.typing import ImputerStrategy
+from safeds.exceptions import TransformerNotFittedError, UnknownColumnNameError
 
 
 class Imputer(TableTransformer):
     """
-    Impute the data for a given Table.
+    Replace missing values with the given strategy.
 
     Parameters
     ----------
     strategy : ImputerStrategy
-        The strategy used to impute missing values.
+        The strategy used to impute missing values. Use the classes nested inside `Imputer.Strategy` to specify it.
+
+    Examples
+    --------
+    >>> from safeds.data.tabular.containers import Column, Table
+    >>> from safeds.data.tabular.transformation import Imputer
+    >>>
+    >>> table = Table.from_columns(
+    ...     [
+    ...         Column("a", [1, 3, None]),
+    ...         Column("b", [None, 2, 3]),
+    ...     ],
+    ... )
+    >>> transformer = Imputer(Imputer.Strategy.Constant(0))
+    >>> transformed_table = transformer.fit_and_transform(table)
     """
 
     class Strategy:
         class Constant(ImputerStrategy):
             """
             An imputation strategy for imputing missing data with given constant values.
 
@@ -44,54 +53,48 @@
                 return f"Constant({self._value})"
 
             def _augment_imputer(self, imputer: sk_SimpleImputer) -> None:
                 imputer.strategy = "constant"
                 imputer.fill_value = self._value
 
         class Mean(ImputerStrategy):
-            """
-            An imputation strategy for imputing missing data with mean values.
-            """
+            """An imputation strategy for imputing missing data with mean values."""
 
             def __str__(self) -> str:
                 return "Mean"
 
             def _augment_imputer(self, imputer: sk_SimpleImputer) -> None:
                 imputer.strategy = "mean"
 
         class Median(ImputerStrategy):
-            """
-            An imputation strategy for imputing missing data with median values.
-            """
+            """An imputation strategy for imputing missing data with median values."""
 
             def __str__(self) -> str:
                 return "Median"
 
             def _augment_imputer(self, imputer: sk_SimpleImputer) -> None:
                 imputer.strategy = "median"
 
         class Mode(ImputerStrategy):
-            """
-            An imputation strategy for imputing missing data with mode values.
-            """
+            """An imputation strategy for imputing missing data with mode values."""
 
             def __str__(self) -> str:
                 return "Mode"
 
             def _augment_imputer(self, imputer: sk_SimpleImputer) -> None:
                 imputer.strategy = "most_frequent"
 
     def __init__(self, strategy: ImputerStrategy):
         self._strategy = strategy
 
-        self._wrapped_transformer: Optional[sk_SimpleImputer] = None
-        self._column_names: Optional[list[str]] = None
+        self._wrapped_transformer: sk_SimpleImputer | None = None
+        self._column_names: list[str] | None = None
 
     # noinspection PyProtectedMember
-    def fit(self, table: Table, column_names: Optional[list[str]] = None) -> Imputer:
+    def fit(self, table: Table, column_names: list[str] | None = None) -> Imputer:
         """
         Learn a transformation for a set of columns in a table.
 
         Parameters
         ----------
         table : Table
             The table used to fit the transformer.
@@ -139,22 +142,21 @@
 
         Returns
         -------
         transformed_table : Table
             The transformed table.
 
         Raises
-        ----------
-        NotFittedError
+        ------
+        TransformerNotFittedError
             If the transformer has not been fitted yet.
         """
-
         # Transformer has not been fitted yet
         if self._wrapped_transformer is None or self._column_names is None:
-            raise NotFittedError()
+            raise TransformerNotFittedError
 
         # Input table does not contain all columns used to fit the transformer
         missing_columns = set(self._column_names) - set(table.get_column_names())
         if len(missing_columns) > 0:
             raise UnknownColumnNameError(list(missing_columns))
 
         data = table._data.copy()
```

### Comparing `safe_ds-0.8.0/src/safeds/data/tabular/transformation/_label_encoder.py` & `safe_ds-0.9.0/src/safeds/data/tabular/transformation/_label_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from __future__ import annotations
 
 import warnings
-from typing import Any, Optional
+from typing import Any
+
+from sklearn.preprocessing import OrdinalEncoder as sk_OrdinalEncoder
 
 from safeds.data.tabular.containers import Table
 from safeds.data.tabular.transformation._table_transformer import (
     InvertibleTableTransformer,
 )
-from safeds.exceptions import NotFittedError, UnknownColumnNameError
-from sklearn.preprocessing import OrdinalEncoder as sk_OrdinalEncoder
+from safeds.exceptions import TransformerNotFittedError, UnknownColumnNameError
 
 
 def warn(*_: Any, **__: Any) -> None:
     pass
 
 
 warnings.warn = warn
 
 
 # noinspection PyProtectedMember
 class LabelEncoder(InvertibleTableTransformer):
-    """
-    The LabelEncoder encodes one or more given columns into labels.
-    """
+    """The LabelEncoder encodes one or more given columns into labels."""
 
     def __init__(self) -> None:
-        self._wrapped_transformer: Optional[sk_OrdinalEncoder] = None
-        self._column_names: Optional[list[str]] = None
+        self._wrapped_transformer: sk_OrdinalEncoder | None = None
+        self._column_names: list[str] | None = None
 
-    def fit(self, table: Table, column_names: Optional[list[str]] = None) -> LabelEncoder:
+    def fit(self, table: Table, column_names: list[str] | None = None) -> LabelEncoder:
         """
         Learn a transformation for a set of columns in a table.
 
         Parameters
         ----------
         table : Table
             The table used to fit the transformer.
@@ -73,22 +72,21 @@
 
         Returns
         -------
         transformed_table : Table
             The transformed table.
 
         Raises
-        ----------
-        NotFittedError
+        ------
+        TransformerNotFittedError
             If the transformer has not been fitted yet.
         """
-
         # Transformer has not been fitted yet
         if self._wrapped_transformer is None or self._column_names is None:
-            raise NotFittedError()
+            raise TransformerNotFittedError
 
         # Input table does not contain all columns used to fit the transformer
         missing_columns = set(self._column_names) - set(table.get_column_names())
         if len(missing_columns) > 0:
             raise UnknownColumnNameError(list(missing_columns))
 
         data = table._data.copy()
@@ -107,22 +105,21 @@
 
         Returns
         -------
         table : Table
             The original table.
 
         Raises
-        ----------
-        NotFittedError
+        ------
+        TransformerNotFittedError
             If the transformer has not been fitted yet.
         """
-
         # Transformer has not been fitted yet
         if self._wrapped_transformer is None or self._column_names is None:
-            raise NotFittedError()
+            raise TransformerNotFittedError
 
         data = transformed_table._data.copy()
         data.columns = transformed_table.get_column_names()
         data[self._column_names] = self._wrapped_transformer.inverse_transform(data[self._column_names])
         return Table(data)
 
     def is_fitted(self) -> bool:
```

### Comparing `safe_ds-0.8.0/src/safeds/data/tabular/transformation/_one_hot_encoder.py` & `safe_ds-0.9.0/src/safeds/data/tabular/transformation/_one_hot_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from __future__ import annotations
 
-from typing import Optional
-
 import pandas as pd
+from sklearn.preprocessing import OneHotEncoder as sk_OneHotEncoder
+
 from safeds.data.tabular.containers import Table
 from safeds.data.tabular.transformation._table_transformer import (
     InvertibleTableTransformer,
 )
-from safeds.exceptions import NotFittedError, UnknownColumnNameError
-from sklearn.preprocessing import OneHotEncoder as sk_OneHotEncoder
+from safeds.exceptions import TransformerNotFittedError, UnknownColumnNameError
 
 
 class OneHotEncoder(InvertibleTableTransformer):
-    """
-    The OneHotEncoder encodes categorical columns to numerical features [0,1] that represent the existence for each value.
-    """
+    """Encodes categorical columns to numerical features [0,1] that represent the existence for each value."""
 
     def __init__(self) -> None:
-        self._wrapped_transformer: Optional[sk_OneHotEncoder] = None
-        self._column_names: Optional[list[str]] = None
+        self._wrapped_transformer: sk_OneHotEncoder | None = None
+        self._column_names: list[str] | None = None
 
     # noinspection PyProtectedMember
-    def fit(self, table: Table, column_names: Optional[list[str]] = None) -> OneHotEncoder:
+    def fit(self, table: Table, column_names: list[str] | None = None) -> OneHotEncoder:
         """
         Learn a transformation for a set of columns in a table.
 
         Parameters
         ----------
         table : Table
             The table used to fit the transformer.
@@ -68,22 +65,21 @@
 
         Returns
         -------
         transformed_table : Table
             The transformed table.
 
         Raises
-        ----------
-        NotFittedError
+        ------
+        TransformerNotFittedError
             If the transformer has not been fitted yet.
         """
-
         # Transformer has not been fitted yet
         if self._wrapped_transformer is None or self._column_names is None:
-            raise NotFittedError()
+            raise TransformerNotFittedError
 
         # Input table does not contain all columns used to fit the transformer
         missing_columns = set(self._column_names) - set(table.get_column_names())
         if len(missing_columns) > 0:
             raise UnknownColumnNameError(list(missing_columns))
 
         original = table._data.copy()
@@ -108,27 +104,28 @@
 
         Returns
         -------
         table : Table
             The original table.
 
         Raises
-        ----------
-        NotFittedError
+        ------
+        TransformerNotFittedError
             If the transformer has not been fitted yet.
         """
         # Transformer has not been fitted yet
         if self._wrapped_transformer is None or self._column_names is None:
-            raise NotFittedError()
+            raise TransformerNotFittedError
 
         data = transformed_table._data.copy()
         data.columns = transformed_table.get_column_names()
 
         decoded = pd.DataFrame(
-            self._wrapped_transformer.inverse_transform(transformed_table._data), columns=self._column_names
+            self._wrapped_transformer.inverse_transform(transformed_table._data),
+            columns=self._column_names,
         )
         unchanged = data.drop(self._wrapped_transformer.get_feature_names_out(), axis=1)
 
         return Table(pd.concat([unchanged, decoded], axis=1))
 
     def is_fitted(self) -> bool:
         """
```

### Comparing `safe_ds-0.8.0/src/safeds/data/tabular/transformation/_table_transformer.py` & `safe_ds-0.9.0/src/safeds/data/tabular/transformation/_table_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from safeds.data.tabular.containers import Table
 
 
 class TableTransformer(ABC):
-    """
-    A `TableTransformer` learns a transformation for a set of columns in a `Table` and can then apply the learned
-    transformation to another `Table` with the same columns.
-    """
+    """Learn a transformation for a set of columns in a `Table` and transform another `Table` with the same columns."""
 
     @abstractmethod
-    def fit(self, table: Table, column_names: Optional[list[str]] = None) -> TableTransformer:
+    def fit(self, table: Table, column_names: list[str] | None = None) -> TableTransformer:
         """
         Learn a transformation for a set of columns in a table.
 
         Parameters
         ----------
         table : Table
             The table used to fit the transformer.
@@ -43,33 +40,34 @@
 
         Returns
         -------
         transformed_table : Table
             The transformed table.
 
         Raises
-        ----------
-        NotFittedError
+        ------
+        TransformerNotFittedError
             If the transformer has not been fitted yet.
         """
 
     @abstractmethod
     def is_fitted(self) -> bool:
         """
         Check if the transformer is fitted.
 
         Returns
         -------
         is_fitted : bool
             Whether the transformer is fitted.
         """
 
-    def fit_and_transform(self, table: Table, column_names: Optional[list[str]] = None) -> Table:
+    def fit_and_transform(self, table: Table, column_names: list[str] | None = None) -> Table:
         """
         Learn a transformation for a set of columns in a table and apply the learned transformation to the same table.
+
         If you also need the fitted transformer, use `fit` and `transform` separately.
 
         Parameters
         ----------
         table : Table
             The table used to fit the transformer. The transformer is then applied to this table.
         column_names : Optional[list[str]]
@@ -80,18 +78,15 @@
         transformed_table : Table
             The transformed table.
         """
         return self.fit(table, column_names).transform(table)
 
 
 class InvertibleTableTransformer(TableTransformer):
-    """
-    An `InvertibleTableTransformer` is a `TableTransformer` that can also undo the learned transformation after it has
-    been applied.
-    """
+    """A `TableTransformer` that can also undo the learned transformation after it has been applied."""
 
     @abstractmethod
     def inverse_transform(self, transformed_table: Table) -> Table:
         """
         Undo the learned transformation.
 
         Parameters
@@ -101,11 +96,11 @@
 
         Returns
         -------
         table : Table
             The original table.
 
         Raises
-        ----------
-        NotFittedError
+        ------
+        TransformerNotFittedError
             If the transformer has not been fitted yet.
         """
```

### Comparing `safe_ds-0.8.0/src/safeds/data/tabular/typing/_column_type.py` & `safe_ds-0.9.0/src/safeds/data/tabular/typing/_column_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
-import numpy as np
+if TYPE_CHECKING:
+    import numpy as np
 
 
 class ColumnType(ABC):
-    """
-    Abstract base class for column types.
-    """
+    """Abstract base class for column types."""
 
     @abstractmethod
     def is_nullable(self) -> bool:
         """
         Return whether the given column type is nullable.
 
         Returns
@@ -45,15 +45,15 @@
 
         Returns
         -------
         column_type : ColumnType
             The ColumnType.
 
         Raises
-        -------
+        ------
         TypeError
             If the given dtype is not supported.
         """
         if dtype.kind in ("u", "i"):
             return Integer()
         if dtype.kind == "b":
             return Boolean()
```

### Comparing `safe_ds-0.8.0/src/safeds/data/tabular/typing/_schema.py` & `safe_ds-0.9.0/src/safeds/data/tabular/typing/_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
-import pandas as pd
 from safeds.data.tabular.typing._column_type import ColumnType
 from safeds.exceptions import UnknownColumnNameError
 
+if TYPE_CHECKING:
+    import pandas as pd
+
 
 @dataclass
 class Schema:
     """
     Store column names and corresponding data types for a `Table` or `Row`.
 
     Parameters
@@ -62,25 +65,24 @@
             raise UnknownColumnNameError([column_name])
         return self._schema[column_name]
 
     def _get_column_index_by_name(self, column_name: str) -> int:
         """
          Return the index of the column with specified column name.
 
-         Parameters
-         ----------
+        Parameters
+        ----------
          column_name : str
              The name of the column.
 
-         Returns
-         -------
+        Returns
+        -------
         index : int
              The index of the column.
         """
-
         return list(self._schema.keys()).index(column_name)
 
     @staticmethod
     def _from_dataframe(dataframe: pd.DataFrame) -> Schema:
         """
         Construct a TableSchema from a Dataframe. This function is not supposed to be exposed to the user.
 
@@ -91,20 +93,19 @@
 
         Returns
         -------
         _from_dataframe: Schema
             The constructed TableSchema.
 
         """
-
         names = dataframe.columns
         # noinspection PyProtectedMember
         types = (ColumnType._from_numpy_dtype(dtype) for dtype in dataframe.dtypes)
 
-        return Schema(dict(zip(names, types)))
+        return Schema(dict(zip(names, types, strict=True)))
 
     def get_column_names(self) -> list[str]:
         """
         Return a list of all column names saved in this schema.
 
         Returns
         -------
```

### Comparing `safe_ds-0.8.0/src/safeds/exceptions/_data_exceptions.py` & `safe_ds-0.9.0/src/safeds/exceptions/_data_exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,22 +9,18 @@
     """
 
     def __init__(self, column_names: list[str]):
         super().__init__(f"Could not find column(s) '{', '.join(column_names)}'")
 
 
 class NonNumericColumnError(Exception):
-    """
-    Exception raised for trying to do numerical operations on a non-numerical column.
-    """
+    """Exception raised for trying to do numerical operations on a non-numerical column."""
 
     def __init__(self, column_info: str) -> None:
-        super().__init__(
-            f"Tried to do a numerical operation on one or multiple non numerical Columns: \n{column_info}"
-        )
+        super().__init__(f"Tried to do a numerical operation on one or multiple non numerical Columns: \n{column_info}")
 
 
 class DuplicateColumnNameError(Exception):
     """
     Exception raised for trying to modify a table resulting in a duplicate column name.
 
     Parameters
@@ -60,46 +56,43 @@
     expected_size : str
         The expected size of the column as an expression (e.g. 2, >0, !=0).
     actual_size : str
         The actual size of the column as an expression (e.g. 2, >0, !=0).
     """
 
     def __init__(self, expected_size: str, actual_size: str):
-        super().__init__(
-            f"Expected a column of size {expected_size} but got column of size {actual_size}."
-        )
+        super().__init__(f"Expected a column of size {expected_size} but got column of size {actual_size}.")
 
 
 class SchemaMismatchError(Exception):
-    """
-    Exception raised when schemas are unequal.
-    """
+    """Exception raised when schemas are unequal."""
 
     def __init__(self) -> None:
         super().__init__("Failed because at least two schemas didn't match.")
 
 
 class MissingSchemaError(Exception):
-    """
-    Exception raised when a required schema is missing.
-    """
+    """Exception raised when a required schema is missing."""
 
     def __init__(self) -> None:
         super().__init__("Failed because a required schema is missing.")
 
 
 class ColumnLengthMismatchError(Exception):
-    """
-    Exception raised when the lengths of two or more columns do not match.
-    """
+    """Exception raised when the lengths of two or more columns do not match."""
 
     def __init__(self, column_info: str):
         super().__init__(f"The length of at least one column differs: \n{column_info}")
 
 
 class MissingDataError(Exception):
-    """
-    Exception raised if a function is not given enough data to succeed.
-    """
+    """Exception raised if a function is not given enough data to succeed."""
 
     def __init__(self, missing_data_info: str):
         super().__init__(f"The function is missing data: \n{missing_data_info}")
+
+
+class TransformerNotFittedError(Exception):
+    """Raised when a transformer is used before fitting it."""
+
+    def __init__(self) -> None:
+        super().__init__("The transformer has not been fitted yet.")
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/_util_sklearn.py` & `safe_ds-0.9.0/src/safeds/ml/_util_sklearn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-from typing import Any, Optional
+from typing import Any
 
 from safeds.data.tabular.containers import Table, TaggedTable
-from safeds.exceptions import LearningError, PredictionError
-from sklearn.exceptions import NotFittedError
+from safeds.exceptions import (
+    DatasetContainsTargetError,
+    DatasetMissesFeaturesError,
+    LearningError,
+    ModelNotFittedError,
+    PredictionError,
+)
 
 
 # noinspection PyProtectedMember
 def fit(model: Any, tagged_table: TaggedTable) -> None:
     """
     Fit a model for a given tagged table.
 
@@ -28,15 +33,15 @@
             tagged_table.target._data,
         )
     except ValueError as exception:
         raise LearningError(str(exception)) from exception
 
 
 # noinspection PyProtectedMember
-def predict(model: Any, dataset: Table, feature_names: Optional[list[str]], target_name: Optional[str]) -> TaggedTable:
+def predict(model: Any, dataset: Table, feature_names: list[str] | None, target_name: str | None) -> TaggedTable:
     """
     Predict a target vector using a dataset containing feature vectors. The model has to be trained first.
 
     Parameters
     ----------
     model
         Classifier or regressor from scikit-learn.
@@ -50,28 +55,37 @@
     Returns
     -------
     table : TaggedTable
         A dataset containing the given features and the predicted target.
 
     Raises
     ------
+    ModelNotFittedError
+        If the model has not been fitted yet.
+    DatasetContainsTargetError
+        If the dataset contains the target column already.
+    DatasetMissesFeaturesError
+        If the dataset misses feature columns.
     PredictionError
         If predicting with the given dataset failed.
     """
-
+    # Validation
     if model is None or target_name is None or feature_names is None:
-        raise PredictionError("The model was not trained")
+        raise ModelNotFittedError
+    if dataset.has_column(target_name):
+        raise DatasetContainsTargetError(target_name)
+    missing_feature_names = [feature_name for feature_name in feature_names if not dataset.has_column(feature_name)]
+    if missing_feature_names:
+        raise DatasetMissesFeaturesError(missing_feature_names)
 
     dataset_df = dataset.keep_only_columns(feature_names)._data
     dataset_df.columns = feature_names
+
+    result_set = dataset._data.copy(deep=True)
+    result_set.columns = dataset.get_column_names()
+
     try:
         predicted_target_vector = model.predict(dataset_df.values)
-        result_set = dataset._data.copy(deep=True)
-        result_set.columns = dataset.get_column_names()
-        if target_name in result_set.columns:
-            raise ValueError(f"Dataset already contains '{target_name}' column. Please rename this column")
         result_set[target_name] = predicted_target_vector
         return Table(result_set).tag_columns(target_name=target_name, feature_names=feature_names)
-    except NotFittedError as exception:
-        raise PredictionError("The model was not trained") from exception
     except ValueError as exception:
         raise PredictionError(str(exception)) from exception
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/classification/_ada_boost.py` & `safe_ds-0.9.0/src/safeds/ml/classification/_ada_boost.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
 
-from safeds.data.tabular.containers import Table, TaggedTable
-from safeds.ml._util_sklearn import fit, predict
 from sklearn.ensemble import AdaBoostClassifier as sk_AdaBoostClassifier
 
+from safeds.ml._util_sklearn import fit, predict
+
 from ._classifier import Classifier
 
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
+
 
 class AdaBoost(Classifier):
-    """
-    This class implements Ada Boost classification. It is used as a classifier model.
-    It can only be trained on a tagged table.
-    """
+    """Ada Boost classification."""
 
     def __init__(self) -> None:
-        self._wrapped_classifier: Optional[sk_AdaBoostClassifier] = None
-        self._feature_names: Optional[list[str]] = None
-        self._target_name: Optional[str] = None
+        self._wrapped_classifier: sk_AdaBoostClassifier | None = None
+        self._feature_names: list[str] | None = None
+        self._target_name: str | None = None
 
     def fit(self, training_set: TaggedTable) -> AdaBoost:
         """
-        Create a new classifier based on this one and fit it with the given training data. This classifier is not
-        modified.
+        Create a copy of this classifier and fit it with the given training data.
+
+        This classifier is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
@@ -36,15 +37,14 @@
             The fitted classifier.
 
         Raises
         ------
         LearningError
             If the training data contains invalid values or if the training failed.
         """
-
         wrapped_classifier = sk_AdaBoostClassifier()
         fit(wrapped_classifier, training_set)
 
         result = AdaBoost()
         result._wrapped_classifier = wrapped_classifier
         result._feature_names = training_set.features.get_column_names()
         result._target_name = training_set.target.name
@@ -63,22 +63,28 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
         return predict(self._wrapped_classifier, dataset, self._feature_names, self._target_name)
 
     def is_fitted(self) -> bool:
         """
-        Checks if the classifier is fitted.
+        Check if the classifier is fitted.
 
         Returns
         -------
         is_fitted : bool
             Whether the classifier is fitted.
         """
         return self._wrapped_classifier is not None
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/classification/_classifier.py` & `safe_ds-0.9.0/src/safeds/ml/classification/_classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING
 
-from safeds.data.tabular.containers import Table, TaggedTable
 from sklearn.metrics import accuracy_score as sk_accuracy_score
 
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
+
 
 class Classifier(ABC):
-    """
-    Abstract base class for all classifiers.
-    """
+    """Abstract base class for all classifiers."""
 
     @abstractmethod
     def fit(self, training_set: TaggedTable) -> Classifier:
         """
-        Create a new classifier based on this one and fit it with the given training data. This classifier is not
-        modified.
+        Create a copy of this classifier and fit it with the given training data.
+
+        This classifier is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
@@ -46,43 +48,47 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
 
     @abstractmethod
     def is_fitted(self) -> bool:
         """
-        Checks if the classifier is fitted.
+        Check if the classifier is fitted.
 
         Returns
         -------
         is_fitted : bool
             Whether the classifier is fitted.
         """
 
     # noinspection PyProtectedMember
     def accuracy(self, validation_or_test_set: TaggedTable) -> float:
         """
-        Predicts the target values for the features in the validation or test set and compares it to the expected
-        results.
+        Compute the accuracy of the classifier on the given data.
 
         Parameters
         ----------
         validation_or_test_set : TaggedTable
             The validation or test set.
 
         Returns
         -------
         accuracy : float
             The calculated accuracy score, i.e. the percentage of equal data.
         """
-
         expected = validation_or_test_set.target
         predicted = self.predict(validation_or_test_set.features).target
 
         return sk_accuracy_score(expected._data, predicted._data)
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/classification/_decision_tree.py` & `safe_ds-0.9.0/src/safeds/ml/classification/_gradient_boosting_classification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
+
+from sklearn.ensemble import GradientBoostingClassifier as sk_GradientBoostingClassifier
 
-from safeds.data.tabular.containers import Table, TaggedTable
 from safeds.ml._util_sklearn import fit, predict
-from sklearn.tree import DecisionTreeClassifier as sk_DecisionTreeClassifier
 
 from ._classifier import Classifier
 
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
+
 
-class DecisionTree(Classifier):
-    """
-    This class implements decision tree regression. It is used as a classifier model.
-    It can only be trained on a tagged table.
-    """
+class GradientBoosting(Classifier):
+    """Gradient boosting classification."""
 
     def __init__(self) -> None:
-        self._wrapped_classifier: Optional[sk_DecisionTreeClassifier] = None
-        self._feature_names: Optional[list[str]] = None
-        self._target_name: Optional[str] = None
+        self._wrapped_classifier: sk_GradientBoostingClassifier | None = None
+        self._feature_names: list[str] | None = None
+        self._target_name: str | None = None
 
-    def fit(self, training_set: TaggedTable) -> DecisionTree:
+    def fit(self, training_set: TaggedTable) -> GradientBoosting:
         """
-        Create a new classifier based on this one and fit it with the given training data. This classifier is not
-        modified.
+        Create a copy of this classifier and fit it with the given training data.
+
+        This classifier is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
         -------
-        fitted_classifier : DecisionTree
+        fitted_classifier : GradientBoosting
             The fitted classifier.
 
         Raises
         ------
         LearningError
             If the training data contains invalid values or if the training failed.
         """
-
-        wrapped_classifier = sk_DecisionTreeClassifier()
+        wrapped_classifier = sk_GradientBoostingClassifier()
         fit(wrapped_classifier, training_set)
 
-        result = DecisionTree()
+        result = GradientBoosting()
         result._wrapped_classifier = wrapped_classifier
         result._feature_names = training_set.features.get_column_names()
         result._target_name = training_set.target.name
 
         return result
 
     def predict(self, dataset: Table) -> TaggedTable:
@@ -63,22 +63,28 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
         return predict(self._wrapped_classifier, dataset, self._feature_names, self._target_name)
 
     def is_fitted(self) -> bool:
         """
-        Checks if the classifier is fitted.
+        Check if the classifier is fitted.
 
         Returns
         -------
         is_fitted : bool
             Whether the classifier is fitted.
         """
         return self._wrapped_classifier is not None
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/classification/_gradient_boosting_classification.py` & `safe_ds-0.9.0/src/safeds/ml/classification/_logistic_regression.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
+
+from sklearn.linear_model import LogisticRegression as sk_LogisticRegression
 
-from safeds.data.tabular.containers import Table, TaggedTable
 from safeds.ml._util_sklearn import fit, predict
-from sklearn.ensemble import GradientBoostingClassifier as sk_GradientBoostingClassifier
 
 from ._classifier import Classifier
 
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
+
 
-class GradientBoosting(Classifier):
-    """
-    This class implements gradient boosting classification. It is used as a classifier model.
-    It can only be trained on a tagged table.
-    """
+class LogisticRegression(Classifier):
+    """Regularized logistic regression."""
 
     def __init__(self) -> None:
-        self._wrapped_classifier: Optional[sk_GradientBoostingClassifier] = None
-        self._feature_names: Optional[list[str]] = None
-        self._target_name: Optional[str] = None
+        self._wrapped_classifier: sk_LogisticRegression | None = None
+        self._feature_names: list[str] | None = None
+        self._target_name: str | None = None
 
-    def fit(self, training_set: TaggedTable) -> GradientBoosting:
+    def fit(self, training_set: TaggedTable) -> LogisticRegression:
         """
-        Create a new classifier based on this one and fit it with the given training data. This classifier is not
-        modified.
+        Create a copy of this classifier and fit it with the given training data.
+
+        This classifier is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
         -------
-        fitted_classifier : GradientBoosting
+        fitted_classifier : LogisticRegression
             The fitted classifier.
 
         Raises
         ------
         LearningError
             If the training data contains invalid values or if the training failed.
         """
-
-        wrapped_classifier = sk_GradientBoostingClassifier()
+        wrapped_classifier = sk_LogisticRegression(n_jobs=-1)
         fit(wrapped_classifier, training_set)
 
-        result = GradientBoosting()
+        result = LogisticRegression()
         result._wrapped_classifier = wrapped_classifier
         result._feature_names = training_set.features.get_column_names()
         result._target_name = training_set.target.name
 
         return result
 
-    # noinspection PyProtectedMember
     def predict(self, dataset: Table) -> TaggedTable:
         """
         Predict a target vector using a dataset containing feature vectors. The model has to be trained first.
 
         Parameters
         ----------
         dataset : Table
@@ -64,22 +63,28 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
         return predict(self._wrapped_classifier, dataset, self._feature_names, self._target_name)
 
     def is_fitted(self) -> bool:
         """
-        Checks if the classifier is fitted.
+        Check if the classifier is fitted.
 
         Returns
         -------
         is_fitted : bool
             Whether the classifier is fitted.
         """
         return self._wrapped_classifier is not None
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/classification/_k_nearest_neighbors.py` & `safe_ds-0.9.0/src/safeds/ml/classification/_k_nearest_neighbors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
 
-from safeds.data.tabular.containers import Table, TaggedTable
-from safeds.ml._util_sklearn import fit, predict
 from sklearn.neighbors import KNeighborsClassifier as sk_KNeighborsClassifier
 
+from safeds.ml._util_sklearn import fit, predict
+
 from ._classifier import Classifier
 
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
+
 
 class KNearestNeighbors(Classifier):
     """
-    This class implements K-nearest-neighbors classifier. It can only be trained on a tagged table.
+    K-nearest-neighbors classification.
 
     Parameters
     ----------
-    n_neighbors : int
+    number_of_neighbors : int
         The number of neighbors to be interpolated with. Has to be less than or equal to the sample size.
     """
 
-    def __init__(self, n_neighbors: int) -> None:
-        self._n_neighbors = n_neighbors
+    def __init__(self, number_of_neighbors: int) -> None:
+        self._number_of_neighbors = number_of_neighbors
 
-        self._wrapped_classifier: Optional[sk_KNeighborsClassifier] = None
-        self._feature_names: Optional[list[str]] = None
-        self._target_name: Optional[str] = None
+        self._wrapped_classifier: sk_KNeighborsClassifier | None = None
+        self._feature_names: list[str] | None = None
+        self._target_name: str | None = None
 
     def fit(self, training_set: TaggedTable) -> KNearestNeighbors:
         """
-        Create a new classifier based on this one and fit it with the given training data. This classifier is not
-        modified.
+        Create a copy of this classifier and fit it with the given training data.
+
+        This classifier is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
@@ -42,48 +46,54 @@
             The fitted classifier.
 
         Raises
         ------
         LearningError
             If the training data contains invalid values or if the training failed.
         """
-        wrapped_classifier = sk_KNeighborsClassifier(self._n_neighbors, n_jobs=-1)
+        wrapped_classifier = sk_KNeighborsClassifier(self._number_of_neighbors, n_jobs=-1)
         fit(wrapped_classifier, training_set)
 
-        result = KNearestNeighbors(self._n_neighbors)
+        result = KNearestNeighbors(self._number_of_neighbors)
         result._wrapped_classifier = wrapped_classifier
         result._feature_names = training_set.features.get_column_names()
         result._target_name = training_set.target.name
 
         return result
 
     def predict(self, dataset: Table) -> TaggedTable:
         """
-        Predict a target vector using a dataset containing feature vectors. The model has to be trained first
+        Predict a target vector using a dataset containing feature vectors. The model has to be trained first.
 
         Parameters
         ----------
         dataset : Table
             The dataset containing the feature vectors.
 
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
         return predict(self._wrapped_classifier, dataset, self._feature_names, self._target_name)
 
     def is_fitted(self) -> bool:
         """
-        Checks if the classifier is fitted.
+        Check if the classifier is fitted.
 
         Returns
         -------
         is_fitted : bool
             Whether the classifier is fitted.
         """
         return self._wrapped_classifier is not None
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/classification/_logistic_regression.py` & `safe_ds-0.9.0/src/safeds/ml/classification/_decision_tree.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
+
+from sklearn.tree import DecisionTreeClassifier as sk_DecisionTreeClassifier
 
-from safeds.data.tabular.containers import Table, TaggedTable
 from safeds.ml._util_sklearn import fit, predict
-from sklearn.linear_model import LogisticRegression as sk_LogisticRegression
 
 from ._classifier import Classifier
 
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
+
 
-class LogisticRegression(Classifier):
-    """
-    This class implements regularized logistic regression. It is used as a classifier model.
-    It can only be trained on a tagged table.
-    """
+class DecisionTree(Classifier):
+    """Decision tree classification."""
 
     def __init__(self) -> None:
-        self._wrapped_classifier: Optional[sk_LogisticRegression] = None
-        self._feature_names: Optional[list[str]] = None
-        self._target_name: Optional[str] = None
+        self._wrapped_classifier: sk_DecisionTreeClassifier | None = None
+        self._feature_names: list[str] | None = None
+        self._target_name: str | None = None
 
-    def fit(self, training_set: TaggedTable) -> LogisticRegression:
+    def fit(self, training_set: TaggedTable) -> DecisionTree:
         """
-        Create a new classifier based on this one and fit it with the given training data. This classifier is not
-        modified.
+        Create a copy of this classifier and fit it with the given training data.
+
+        This classifier is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
         -------
-        fitted_classifier : LogisticRegression
+        fitted_classifier : DecisionTree
             The fitted classifier.
 
         Raises
         ------
         LearningError
             If the training data contains invalid values or if the training failed.
         """
-
-        wrapped_classifier = sk_LogisticRegression(n_jobs=-1)
+        wrapped_classifier = sk_DecisionTreeClassifier()
         fit(wrapped_classifier, training_set)
 
-        result = LogisticRegression()
+        result = DecisionTree()
         result._wrapped_classifier = wrapped_classifier
         result._feature_names = training_set.features.get_column_names()
         result._target_name = training_set.target.name
 
         return result
 
     def predict(self, dataset: Table) -> TaggedTable:
@@ -63,22 +63,28 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
         return predict(self._wrapped_classifier, dataset, self._feature_names, self._target_name)
 
     def is_fitted(self) -> bool:
         """
-        Checks if the classifier is fitted.
+        Check if the classifier is fitted.
 
         Returns
         -------
         is_fitted : bool
             Whether the classifier is fitted.
         """
         return self._wrapped_classifier is not None
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/classification/_random_forest.py` & `safe_ds-0.9.0/src/safeds/ml/regression/_lasso_regression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
+
+from sklearn.linear_model import Lasso as sk_Lasso
 
-from safeds.data.tabular.containers import Table, TaggedTable
 from safeds.ml._util_sklearn import fit, predict
-from sklearn.ensemble import RandomForestClassifier as sk_RandomForestClassifier
 
-from ._classifier import Classifier
+from ._regressor import Regressor
+
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
 
 
-class RandomForest(Classifier):
-    """
-    This class implements the Random Forest classification. It can only be trained on a tagged table.
-    """
+class LassoRegression(Regressor):
+    """Lasso regression."""
 
     def __init__(self) -> None:
-        self._wrapped_classifier: Optional[sk_RandomForestClassifier] = None
-        self._feature_names: Optional[list[str]] = None
-        self._target_name: Optional[str] = None
+        self._wrapped_regressor: sk_Lasso | None = None
+        self._feature_names: list[str] | None = None
+        self._target_name: str | None = None
 
-    def fit(self, training_set: TaggedTable) -> RandomForest:
+    def fit(self, training_set: TaggedTable) -> LassoRegression:
         """
-        Create a new classifier based on this one and fit it with the given training data. This classifier is not
-        modified.
+        Create a copy of this regressor and fit it with the given training data.
+
+        This regressor is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
         -------
-        fitted_classifier : RandomForest
-            The fitted classifier.
+        fitted_regressor : LassoRegression
+            The fitted regressor.
 
         Raises
         ------
         LearningError
             If the training data contains invalid values or if the training failed.
         """
+        wrapped_regressor = sk_Lasso()
+        fit(wrapped_regressor, training_set)
 
-        wrapped_classifier = sk_RandomForestClassifier(n_jobs=-1)
-        fit(wrapped_classifier, training_set)
-
-        result = RandomForest()
-        result._wrapped_classifier = wrapped_classifier
+        result = LassoRegression()
+        result._wrapped_regressor = wrapped_regressor
         result._feature_names = training_set.features.get_column_names()
         result._target_name = training_set.target.name
 
         return result
 
     def predict(self, dataset: Table) -> TaggedTable:
         """
@@ -62,22 +63,28 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
-        return predict(self._wrapped_classifier, dataset, self._feature_names, self._target_name)
+        return predict(self._wrapped_regressor, dataset, self._feature_names, self._target_name)
 
     def is_fitted(self) -> bool:
         """
-        Checks if the classifier is fitted.
+        Check if the regressor is fitted.
 
         Returns
         -------
         is_fitted : bool
-            Whether the classifier is fitted.
+            Whether the regressor is fitted.
         """
-        return self._wrapped_classifier is not None
+        return self._wrapped_regressor is not None
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/regression/_ada_boost.py` & `safe_ds-0.9.0/src/safeds/ml/regression/_gradient_boosting_regression.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
+
+from sklearn.ensemble import GradientBoostingRegressor as sk_GradientBoostingRegressor
 
-from safeds.data.tabular.containers import Table, TaggedTable
 from safeds.ml._util_sklearn import fit, predict
-from sklearn.ensemble import AdaBoostRegressor as sk_AdaBoostRegressor
 
 from ._regressor import Regressor
 
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
+
 
-class AdaBoost(Regressor):
-    """
-    This class implements Ada Boost regression. It is used as a regression model.
-    It can only be trained on a tagged table.
-    """
+class GradientBoosting(Regressor):
+    """Gradient boosting regression."""
 
     def __init__(self) -> None:
-        self._wrapped_regressor: Optional[sk_AdaBoostRegressor] = None
-        self._feature_names: Optional[list[str]] = None
-        self._target_name: Optional[str] = None
+        self._wrapped_regressor: sk_GradientBoostingRegressor | None = None
+        self._feature_names: list[str] | None = None
+        self._target_name: str | None = None
 
-    def fit(self, training_set: TaggedTable) -> AdaBoost:
+    def fit(self, training_set: TaggedTable) -> GradientBoosting:
         """
-        Create a new regressor based on this one and fit it with the given training data. This regressor is not
-        modified.
+        Create a copy of this regressor and fit it with the given training data.
+
+        This regressor is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
         -------
-        fitted_regressor : AdaBoost
+        fitted_regressor : GradientBoosting
             The fitted regressor.
 
         Raises
         ------
         LearningError
             If the training data contains invalid values or if the training failed.
         """
-
-        wrapped_regressor = sk_AdaBoostRegressor()
+        wrapped_regressor = sk_GradientBoostingRegressor()
         fit(wrapped_regressor, training_set)
 
-        result = AdaBoost()
+        result = GradientBoosting()
         result._wrapped_regressor = wrapped_regressor
         result._feature_names = training_set.features.get_column_names()
         result._target_name = training_set.target.name
 
         return result
 
     def predict(self, dataset: Table) -> TaggedTable:
@@ -63,16 +63,22 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
         return predict(self._wrapped_regressor, dataset, self._feature_names, self._target_name)
 
     def is_fitted(self) -> bool:
         """
         Check if the regressor is fitted.
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/regression/_decision_tree.py` & `safe_ds-0.9.0/src/safeds/ml/regression/_ada_boost.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
+
+from sklearn.ensemble import AdaBoostRegressor as sk_AdaBoostRegressor
 
-from safeds.data.tabular.containers import Table, TaggedTable
 from safeds.ml._util_sklearn import fit, predict
-from sklearn.tree import DecisionTreeRegressor as sk_DecisionTreeRegressor
 
 from ._regressor import Regressor
 
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
+
 
-class DecisionTree(Regressor):
-    """
-    This class implements Decision Tree regression. It is used as a regression model.
-    It can only be trained on a tagged table.
-    """
+class AdaBoost(Regressor):
+    """Ada Boost regression."""
 
     def __init__(self) -> None:
-        self._wrapped_regressor: Optional[sk_DecisionTreeRegressor] = None
-        self._feature_names: Optional[list[str]] = None
-        self._target_name: Optional[str] = None
+        self._wrapped_regressor: sk_AdaBoostRegressor | None = None
+        self._feature_names: list[str] | None = None
+        self._target_name: str | None = None
 
-    def fit(self, training_set: TaggedTable) -> DecisionTree:
+    def fit(self, training_set: TaggedTable) -> AdaBoost:
         """
-        Create a new regressor based on this one and fit it with the given training data. This regressor is not
-        modified.
+        Create a copy of this regressor and fit it with the given training data.
+
+        This regressor is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
         -------
-        fitted_regressor : DecisionTree
+        fitted_regressor : AdaBoost
             The fitted regressor.
 
         Raises
         ------
         LearningError
             If the training data contains invalid values or if the training failed.
         """
-
-        wrapped_regressor = sk_DecisionTreeRegressor()
+        wrapped_regressor = sk_AdaBoostRegressor()
         fit(wrapped_regressor, training_set)
 
-        result = DecisionTree()
+        result = AdaBoost()
         result._wrapped_regressor = wrapped_regressor
         result._feature_names = training_set.features.get_column_names()
         result._target_name = training_set.target.name
 
         return result
 
     def predict(self, dataset: Table) -> TaggedTable:
@@ -63,16 +63,22 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
         return predict(self._wrapped_regressor, dataset, self._feature_names, self._target_name)
 
     def is_fitted(self) -> bool:
         """
         Check if the regressor is fitted.
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/regression/_elastic_net_regression.py` & `safe_ds-0.9.0/src/safeds/ml/regression/_elastic_net_regression.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
 
-from safeds.data.tabular.containers import Table, TaggedTable
-from safeds.ml._util_sklearn import fit, predict
 from sklearn.linear_model import ElasticNet as sk_ElasticNet
 
+from safeds.ml._util_sklearn import fit, predict
+
 from ._regressor import Regressor
 
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
+
 
 class ElasticNetRegression(Regressor):
-    """
-    This class implements elastic net regression. It is used as a regression model.
-    It can only be trained on a tagged table.
-    """
+    """Elastic net regression."""
 
     def __init__(self) -> None:
-        self._wrapped_regressor: Optional[sk_ElasticNet] = None
-        self._feature_names: Optional[list[str]] = None
-        self._target_name: Optional[str] = None
+        self._wrapped_regressor: sk_ElasticNet | None = None
+        self._feature_names: list[str] | None = None
+        self._target_name: str | None = None
 
     def fit(self, training_set: TaggedTable) -> ElasticNetRegression:
         """
-        Create a new regressor based on this one and fit it with the given training data. This regressor is not
-        modified.
+        Create a copy of this regressor and fit it with the given training data.
+
+        This regressor is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
@@ -36,15 +37,14 @@
             The fitted regressor.
 
         Raises
         ------
         LearningError
             If the training data contains invalid values or if the training failed.
         """
-
         wrapped_regressor = sk_ElasticNet()
         fit(wrapped_regressor, training_set)
 
         result = ElasticNetRegression()
         result._wrapped_regressor = wrapped_regressor
         result._feature_names = training_set.features.get_column_names()
         result._target_name = training_set.target.name
@@ -63,16 +63,22 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed
+            If predicting with the given dataset failed.
         """
         return predict(self._wrapped_regressor, dataset, self._feature_names, self._target_name)
 
     def is_fitted(self) -> bool:
         """
         Check if the regressor is fitted.
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/regression/_k_nearest_neighbors.py` & `safe_ds-0.9.0/src/safeds/ml/regression/_k_nearest_neighbors.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
 
-from safeds.data.tabular.containers import Table, TaggedTable
-from safeds.ml._util_sklearn import fit, predict
 from sklearn.neighbors import KNeighborsRegressor as sk_KNeighborsRegressor
 
+from safeds.ml._util_sklearn import fit, predict
+
 from ._regressor import Regressor
 
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
+
 
 class KNearestNeighbors(Regressor):
     """
-    This class implements K-nearest-neighbors regressor. It can only be trained on a tagged table.
+    K-nearest-neighbors regression.
 
     Parameters
     ----------
-    n_neighbors : int
+    number_of_neighbors : int
         The number of neighbors to be interpolated with. Has to be less than or equal than the sample size.
     """
 
-    def __init__(self, n_neighbors: int) -> None:
-        self._n_neighbors = n_neighbors
+    def __init__(self, number_of_neighbors: int) -> None:
+        self._number_of_neighbors = number_of_neighbors
 
-        self._wrapped_regressor: Optional[sk_KNeighborsRegressor] = None
-        self._feature_names: Optional[list[str]] = None
-        self._target_name: Optional[str] = None
+        self._wrapped_regressor: sk_KNeighborsRegressor | None = None
+        self._feature_names: list[str] | None = None
+        self._target_name: str | None = None
 
     def fit(self, training_set: TaggedTable) -> KNearestNeighbors:
         """
-        Create a new regressor based on this one and fit it with the given training data. This regressor is not
-        modified.
+        Create a copy of this regressor and fit it with the given training data.
+
+        This regressor is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
@@ -42,19 +46,18 @@
             The fitted regressor.
 
         Raises
         ------
         LearningError
             If the training data contains invalid values or if the training failed.
         """
-
-        wrapped_regressor = sk_KNeighborsRegressor(self._n_neighbors, n_jobs=-1)
+        wrapped_regressor = sk_KNeighborsRegressor(self._number_of_neighbors, n_jobs=-1)
         fit(wrapped_regressor, training_set)
 
-        result = KNearestNeighbors(self._n_neighbors)
+        result = KNearestNeighbors(self._number_of_neighbors)
         result._wrapped_regressor = wrapped_regressor
         result._feature_names = training_set.features.get_column_names()
         result._target_name = training_set.target.name
 
         return result
 
     def predict(self, dataset: Table) -> TaggedTable:
@@ -69,16 +72,22 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
         return predict(self._wrapped_regressor, dataset, self._feature_names, self._target_name)
 
     def is_fitted(self) -> bool:
         """
         Check if the regressor is fitted.
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/regression/_lasso_regression.py` & `safe_ds-0.9.0/src/safeds/ml/regression/_linear_regression.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
+
+from sklearn.linear_model import LinearRegression as sk_LinearRegression
 
-from safeds.data.tabular.containers import Table, TaggedTable
 from safeds.ml._util_sklearn import fit, predict
-from sklearn.linear_model import Lasso as sk_Lasso
 
 from ._regressor import Regressor
 
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
+
 
-class LassoRegression(Regressor):
-    """
-    This class implements lasso regression. It is used as a regression model.
-    It can only be trained on a tagged table.
-    """
+class LinearRegression(Regressor):
+    """Linear regression."""
 
     def __init__(self) -> None:
-        self._wrapped_regressor: Optional[sk_Lasso] = None
-        self._feature_names: Optional[list[str]] = None
-        self._target_name: Optional[str] = None
+        self._wrapped_regressor: sk_LinearRegression | None = None
+        self._feature_names: list[str] | None = None
+        self._target_name: str | None = None
 
-    def fit(self, training_set: TaggedTable) -> LassoRegression:
+    def fit(self, training_set: TaggedTable) -> LinearRegression:
         """
-        Create a new regressor based on this one and fit it with the given training data. This regressor is not
-        modified.
+        Create a copy of this regressor and fit it with the given training data.
+
+        This regressor is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
         -------
-        fitted_regressor : LassoRegression
+        fitted_regressor : LinearRegression
             The fitted regressor.
 
         Raises
         ------
         LearningError
             If the training data contains invalid values or if the training failed.
         """
-
-        wrapped_regressor = sk_Lasso()
+        wrapped_regressor = sk_LinearRegression(n_jobs=-1)
         fit(wrapped_regressor, training_set)
 
-        result = LassoRegression()
+        result = LinearRegression()
         result._wrapped_regressor = wrapped_regressor
         result._feature_names = training_set.features.get_column_names()
         result._target_name = training_set.target.name
 
         return result
 
     def predict(self, dataset: Table) -> TaggedTable:
@@ -63,16 +63,22 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
         return predict(self._wrapped_regressor, dataset, self._feature_names, self._target_name)
 
     def is_fitted(self) -> bool:
         """
         Check if the regressor is fitted.
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/regression/_linear_regression.py` & `safe_ds-0.9.0/src/safeds/ml/regression/_ridge_regression.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
+
+from sklearn.linear_model import Ridge as sk_Ridge
 
-from safeds.data.tabular.containers import Table, TaggedTable
 from safeds.ml._util_sklearn import fit, predict
-from sklearn.linear_model import LinearRegression as sk_LinearRegression
 
 from ._regressor import Regressor
 
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Table, TaggedTable
+
 
-class LinearRegression(Regressor):
-    """
-    This class implements linear regression. It is used as a regression model.
-    It can only be trained on a tagged table.
-    """
+class RidgeRegression(Regressor):
+    """Ridge regression."""
 
     def __init__(self) -> None:
-        self._wrapped_regressor: Optional[sk_LinearRegression] = None
-        self._feature_names: Optional[list[str]] = None
-        self._target_name: Optional[str] = None
+        self._wrapped_regressor: sk_Ridge | None = None
+        self._feature_names: list[str] | None = None
+        self._target_name: str | None = None
 
-    def fit(self, training_set: TaggedTable) -> LinearRegression:
+    def fit(self, training_set: TaggedTable) -> RidgeRegression:
         """
-        Create a new regressor based on this one and fit it with the given training data. This regressor is not
-        modified.
+        Create a copy of this regressor and fit it with the given training data.
+
+        This regressor is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
         -------
-        fitted_regressor : LinearRegression
+        fitted_regressor : RidgeRegression
             The fitted regressor.
 
         Raises
         ------
         LearningError
             If the training data contains invalid values or if the training failed.
         """
-
-        wrapped_regressor = sk_LinearRegression(n_jobs=-1)
+        wrapped_regressor = sk_Ridge()
         fit(wrapped_regressor, training_set)
 
-        result = LinearRegression()
+        result = RidgeRegression()
         result._wrapped_regressor = wrapped_regressor
         result._feature_names = training_set.features.get_column_names()
         result._target_name = training_set.target.name
 
         return result
 
     def predict(self, dataset: Table) -> TaggedTable:
@@ -63,16 +63,22 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
         return predict(self._wrapped_regressor, dataset, self._feature_names, self._target_name)
 
     def is_fitted(self) -> bool:
         """
         Check if the regressor is fitted.
```

### Comparing `safe_ds-0.8.0/src/safeds/ml/regression/_regressor.py` & `safe_ds-0.9.0/src/safeds/ml/regression/_regressor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING
 
-from safeds.data.tabular.containers import Column, Table, TaggedTable
-from safeds.exceptions import ColumnLengthMismatchError
 from sklearn.metrics import mean_absolute_error as sk_mean_absolute_error
 from sklearn.metrics import mean_squared_error as sk_mean_squared_error
 
+from safeds.exceptions import ColumnLengthMismatchError
+
+if TYPE_CHECKING:
+    from safeds.data.tabular.containers import Column, Table, TaggedTable
+
 
 class Regressor(ABC):
-    """
-    Abstract base class for all regressors.
-    """
+    """Abstract base class for all regressors."""
 
     @abstractmethod
     def fit(self, training_set: TaggedTable) -> Regressor:
         """
-        Create a new regressor based on this one and fit it with the given training data. This regressor is not
-        modified.
+        Create a copy of this regressor and fit it with the given training data.
+
+        This regressor is not modified.
 
         Parameters
         ----------
         training_set : TaggedTable
             The training data containing the feature and target vectors.
 
         Returns
@@ -48,67 +51,71 @@
         Returns
         -------
         table : TaggedTable
             A dataset containing the given feature vectors and the predicted target vector.
 
         Raises
         ------
+        ModelNotFittedError
+            If the model has not been fitted yet.
+        DatasetContainsTargetError
+            If the dataset contains the target column already.
+        DatasetMissesFeaturesError
+            If the dataset misses feature columns.
         PredictionError
-            If prediction with the given dataset failed.
+            If predicting with the given dataset failed.
         """
 
     @abstractmethod
     def is_fitted(self) -> bool:
         """
-        Checks if the regressor is fitted.
+        Check if the classifier is fitted.
 
         Returns
         -------
         is_fitted : bool
             Whether the regressor is fitted.
         """
 
     # noinspection PyProtectedMember
     def mean_squared_error(self, validation_or_test_set: TaggedTable) -> float:
         """
-        Return the mean squared error, calculated from a given known truth and a column to compare.
+        Compute the mean squared error (MSE) on the given data.
 
         Parameters
         ----------
         validation_or_test_set : TaggedTable
             The validation or test set.
 
         Returns
         -------
         mean_squared_error : float
             The calculated mean squared error (the average of the distance of each individual row squared).
         """
-
         expected = validation_or_test_set.target
         predicted = self.predict(validation_or_test_set.features).target
 
         _check_metrics_preconditions(predicted, expected)
         return sk_mean_squared_error(expected._data, predicted._data)
 
     # noinspection PyProtectedMember
     def mean_absolute_error(self, validation_or_test_set: TaggedTable) -> float:
         """
-        Return the mean absolute error, calculated from a given known truth and a column to compare.
+        Compute the mean absolute error (MAE) of the regressor on the given data.
 
         Parameters
         ----------
         validation_or_test_set : TaggedTable
             The validation or test set.
 
         Returns
         -------
         mean_absolute_error : float
             The calculated mean absolute error (the average of the distance of each individual row).
         """
-
         expected = validation_or_test_set.target
         predicted = self.predict(validation_or_test_set.features).target
 
         _check_metrics_preconditions(predicted, expected)
         return sk_mean_absolute_error(expected._data, predicted._data)
 
 
@@ -117,9 +124,9 @@
     if not actual.type.is_numeric():
         raise TypeError(f"Column 'actual' is not numerical but {actual.type}.")
     if not expected.type.is_numeric():
         raise TypeError(f"Column 'expected' is not numerical but {expected.type}.")
 
     if actual._data.size != expected._data.size:
         raise ColumnLengthMismatchError(
-            "\n".join([f"{column.name}: {column._data.size}" for column in [actual, expected]])
+            "\n".join([f"{column.name}: {column._data.size}" for column in [actual, expected]]),
         )
```

### Comparing `safe_ds-0.8.0/PKG-INFO` & `safe_ds-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: safe-ds
-Version: 0.8.0
+Version: 0.9.0
 Summary: A user-friendly library for Data Science in Python.
 Home-page: https://github.com/Safe-DS/Stdlib
 License: MIT
 Keywords: data science,machine learning,usability,learnability
 Author: Lars Reimann
 Author-email: mail@larsreimann.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipython (>=8.8.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.6.3,<4.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Project-URL: Documentation, https://safe-ds-stdlib.readthedocs.io
 Project-URL: Repository, https://github.com/Safe-DS/Stdlib
 Description-Content-Type: text/markdown
 
 # Safe-DS Python Library
```

