# Comparing `tmp/safe_ds_examples-0.9.0.tar.gz` & `tmp/safe_ds_examples-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_ds_examples-0.9.0.tar", max compression
+gzip compressed data, was "safe_ds_examples-0.9.1.tar", max compression
```

## Comparing `safe_ds_examples-0.9.0.tar` & `safe_ds_examples-0.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-03-31 18:58:48.606651 safe_ds_examples-0.9.0/LICENSE
--rw-r--r--   0        0        0      919 2023-03-31 18:58:48.606651 safe_ds_examples-0.9.0/docs/README.md
--rw-r--r--   0        0        0     1220 2023-03-31 18:59:15.471125 safe_ds_examples-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-31 18:58:48.610651 safe_ds_examples-0.9.0/src/safeds_examples/__init__.py
--rw-r--r--   0        0        0       78 2023-03-31 18:58:48.610651 safe_ds_examples-0.9.0/src/safeds_examples/tabular/__init__.py
--rw-r--r--   0        0        0       43 2023-03-31 18:58:48.610651 safe_ds_examples-0.9.0/src/safeds_examples/tabular/_house_sales/__init__.py
--rw-r--r--   0        0        0     2032 2023-03-31 18:58:48.610651 safe_ds_examples-0.9.0/src/safeds_examples/tabular/_house_sales/_house_sales.py
--rw-r--r--   0        0        0  2088210 2023-03-31 18:58:48.618651 safe_ds_examples-0.9.0/src/safeds_examples/tabular/_house_sales/data/house_sales.csv
--rw-r--r--   0        0        0       35 2023-03-31 18:58:48.618651 safe_ds_examples-0.9.0/src/safeds_examples/tabular/_titanic/__init__.py
--rw-r--r--   0        0        0     1129 2023-03-31 18:58:48.618651 safe_ds_examples-0.9.0/src/safeds_examples/tabular/_titanic/_titanic.py
--rw-r--r--   0        0        0   101569 2023-03-31 18:58:48.618651 safe_ds_examples-0.9.0/src/safeds_examples/tabular/_titanic/data/titanic.csv
--rw-r--r--   0        0        0       41 2023-03-31 18:58:48.622652 safe_ds_examples-0.9.0/src/safeds_examples/tabular/containers/__init__.py
--rw-r--r--   0        0        0     2061 2023-03-31 18:58:48.622652 safe_ds_examples-0.9.0/src/safeds_examples/tabular/containers/_example_table.py
--rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 safe_ds_examples-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-04 17:20:52.704336 safe_ds_examples-0.9.1/LICENSE
+-rw-r--r--   0        0        0      919 2023-04-04 17:20:52.704336 safe_ds_examples-0.9.1/docs/README.md
+-rw-r--r--   0        0        0     1221 2023-04-04 17:21:25.400828 safe_ds_examples-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-04-04 17:20:52.708336 safe_ds_examples-0.9.1/src/safeds_examples/__init__.py
+-rw-r--r--   0        0        0      163 2023-04-04 17:20:52.708336 safe_ds_examples-0.9.1/src/safeds_examples/tabular/__init__.py
+-rw-r--r--   0        0        0       75 2023-04-04 17:20:52.708336 safe_ds_examples-0.9.1/src/safeds_examples/tabular/_house_sales/__init__.py
+-rw-r--r--   0        0        0     2035 2023-04-04 17:20:52.708336 safe_ds_examples-0.9.1/src/safeds_examples/tabular/_house_sales/_house_sales.py
+-rw-r--r--   0        0        0  2088210 2023-04-04 17:20:52.720336 safe_ds_examples-0.9.1/src/safeds_examples/tabular/_house_sales/data/house_sales.csv
+-rw-r--r--   0        0        0       63 2023-04-04 17:20:52.720336 safe_ds_examples-0.9.1/src/safeds_examples/tabular/_titanic/__init__.py
+-rw-r--r--   0        0        0     1132 2023-04-04 17:20:52.720336 safe_ds_examples-0.9.1/src/safeds_examples/tabular/_titanic/_titanic.py
+-rw-r--r--   0        0        0   101569 2023-04-04 17:20:52.720336 safe_ds_examples-0.9.1/src/safeds_examples/tabular/_titanic/data/titanic.csv
+-rw-r--r--   0        0        0      113 2023-04-04 17:20:52.720336 safe_ds_examples-0.9.1/src/safeds_examples/tabular/containers/__init__.py
+-rw-r--r--   0        0        0     2100 2023-04-04 17:20:52.720336 safe_ds_examples-0.9.1/src/safeds_examples/tabular/containers/_example_table.py
+-rw-r--r--   0        0        0     1669 1970-01-01 00:00:00.000000 safe_ds_examples-0.9.1/PKG-INFO
```

### Comparing `safe_ds_examples-0.9.0/LICENSE` & `safe_ds_examples-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_ds_examples-0.9.0/docs/README.md` & `safe_ds_examples-0.9.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `safe_ds_examples-0.9.0/pyproject.toml` & `safe_ds_examples-0.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "safe-ds-examples"
-version = "0.9.0"
+version = "0.9.1"
 description = "Ready-to-use examples for the Safe-DS Python library."
 license = "MIT"
 authors = ["Lars Reimann <mail@larsreimann.com>"]
 readme = "docs/README.md"
 repository = "https://github.com/Safe-DS/Stdlib-Examples"
 documentation = "https://stdlib-examples.safe-ds.com"
 keywords = ["data science", "machine learning", "usability", "learnability"]
 packages = [
     { include = "safeds_examples", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-safe-ds = ">=0.8,<0.9"
+safe-ds = ">=0.8,<0.10"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.docs.dependencies]
 jupyter = "^1.0.0"
```

### Comparing `safe_ds_examples-0.9.0/src/safeds_examples/tabular/_house_sales/_house_sales.py` & `safe_ds_examples-0.9.1/src/safeds_examples/tabular/_house_sales/_house_sales.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import os
+from pathlib import Path
 
 from safeds.data.tabular.containers import Table
+
 from safeds_examples.tabular.containers import ExampleTable
 
-_path = os.path.join(os.path.dirname(__file__), "data", "house_sales.csv")
+_path = Path(__file__).parent / "data" / "house_sales.csv"
 
 
 def load_house_sales() -> ExampleTable:
     """
-    Loads the "House Sales" dataset.
+    Load the "House Sales" dataset.
 
     Returns
     -------
     ExampleTable
         The "House Sales" dataset.
     """
-
     return ExampleTable(
-        Table.from_csv_file(_path),
+        Table.from_csv_file(str(_path)),
         column_descriptions={
             "id": "A unique identifier",
             "year": "Year of sale",
             "month": "Month of sale",
             "day": "Day of sale",
             "zipcode": "Zipcode",
             "latitude": "Latitude",
```

### Comparing `safe_ds_examples-0.9.0/src/safeds_examples/tabular/_house_sales/data/house_sales.csv` & `safe_ds_examples-0.9.1/src/safeds_examples/tabular/_house_sales/data/house_sales.csv`

 * *Files identical despite different names*

### Comparing `safe_ds_examples-0.9.0/src/safeds_examples/tabular/_titanic/_titanic.py` & `safe_ds_examples-0.9.1/src/safeds_examples/tabular/_titanic/_titanic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import os
+from pathlib import Path
 
 from safeds.data.tabular.containers import Table
+
 from safeds_examples.tabular.containers import ExampleTable
 
-_path = os.path.join(os.path.dirname(__file__), "data", "titanic.csv")
+_path = Path(__file__).parent / "data" / "titanic.csv"
 
 
 def load_titanic() -> ExampleTable:
     """
-    Loads the "Titanic" dataset.
+    Load the "Titanic" dataset.
 
     Returns
     -------
     ExampleTable
         The "Titanic" dataset.
     """
-
     return ExampleTable(
-        Table.from_csv_file(_path),
+        Table.from_csv_file(str(_path)),
         column_descriptions={
             "id": "A unique identifier",
             "name": "Name of the passenger",
             "sex": "Sex of the passenger",
             "age": "Age of the passenger at the time of the accident",
             "siblings_spouses": "Number of siblings or spouses aboard",
             "parents_children": "Number of parents or children aboard",
```

### Comparing `safe_ds_examples-0.9.0/src/safeds_examples/tabular/_titanic/data/titanic.csv` & `safe_ds_examples-0.9.1/src/safeds_examples/tabular/_titanic/data/titanic.csv`

 * *Files identical despite different names*

### Comparing `safe_ds_examples-0.9.0/src/safeds_examples/tabular/containers/_example_table.py` & `safe_ds_examples-0.9.1/src/safeds_examples/tabular/containers/_example_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 
         super().__init__(table._data, table.schema)
         self._descriptions = column_descriptions
 
     @property
     def column_descriptions(self) -> Table:
         """
-        Returns a `Table` with two columns `"Name"` and `"Description"`, containing the name of a column and its
-        description respectively.
-        """
+        Return a `Table` contain the name of a column and its description.
 
+        The name is stored in a column called `"Name"` and the description in a column called `"Description"`.
+        """
         return Table(
             [
                 {"Name": column_name, "Description": self.get_column_description(column_name)}
                 for column_name in self.get_column_names()
-            ]
+            ],
         )
 
     def get_column_description(self, column_name: str) -> str:
         """
         Get the description of a column. If no description exists, an empty string is returned.
 
         Parameters
@@ -57,12 +57,11 @@
             The description of the column.
 
         Raises
         ------
         UnknownColumnNameError
             If no column with the given name exists.
         """
-
         if column_name not in self.get_column_names():
             raise UnknownColumnNameError([column_name])
 
         return self._descriptions.get(column_name, "")
```

### Comparing `safe_ds_examples-0.9.0/PKG-INFO` & `safe_ds_examples-0.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: safe-ds-examples
-Version: 0.9.0
+Version: 0.9.1
 Summary: Ready-to-use examples for the Safe-DS Python library.
 Home-page: https://github.com/Safe-DS/Stdlib-Examples
 License: MIT
 Keywords: data science,machine learning,usability,learnability
 Author: Lars Reimann
 Author-email: mail@larsreimann.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: safe-ds (>=0.8,<0.9)
+Requires-Dist: safe-ds (>=0.8,<0.10)
 Project-URL: Documentation, https://stdlib-examples.safe-ds.com
 Project-URL: Repository, https://github.com/Safe-DS/Stdlib-Examples
 Description-Content-Type: text/markdown
 
 # Safe-DS Python Library - Examples
 
 [![PyPI](https://img.shields.io/pypi/v/safe-ds-examples)](https://pypi.org/project/safe-ds-examples)
```

