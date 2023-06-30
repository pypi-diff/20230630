# Comparing `tmp/dagster_polars-0.0.2.tar.gz` & `tmp/dagster_polars-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_polars-0.0.2.tar", max compression
+gzip compressed data, was "dagster_polars-0.0.3a0.tar", max compression
```

## Comparing `dagster_polars-0.0.2.tar` & `dagster_polars-0.0.3a0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11344 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/LICENSE
--rw-r--r--   0        0        0     2443 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/README.md
--rw-r--r--   0        0        0      324 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/__init__.py
--rw-r--r--   0        0        0       76 2023-06-25 09:30:38.628701 dagster_polars-0.0.2/dagster_polars/_version.py
--rw-r--r--   0        0        0        0 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/io_managers/__init__.py
--rw-r--r--   0        0        0     5977 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/io_managers/base.py
--rw-r--r--   0        0        0     7200 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/io_managers/bigquery.py
--rw-r--r--   0        0        0     1278 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/io_managers/parquet.py
--rw-r--r--   0        0        0     3936 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/io_managers/utils.py
--rw-r--r--   0        0        0        0 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/py.typed
--rw-r--r--   0        0        0     2806 2023-06-25 09:30:38.624701 dagster_polars-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 dagster_polars-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/LICENSE
+-rw-r--r--   0        0        0     3070 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/README.md
+-rw-r--r--   0        0        0      358 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/__init__.py
+-rw-r--r--   0        0        0       78 2023-06-30 10:34:57.257820 dagster_polars-0.0.3a0/dagster_polars/_version.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/io_managers/__init__.py
+-rw-r--r--   0        0        0     7896 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/io_managers/base.py
+-rw-r--r--   0        0        0     7200 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/io_managers/bigquery.py
+-rw-r--r--   0        0        0     3074 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/io_managers/delta.py
+-rw-r--r--   0        0        0     2143 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/io_managers/parquet.py
+-rw-r--r--   0        0        0     3936 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/io_managers/utils.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/py.typed
+-rw-r--r--   0        0        0     2880 2023-06-30 10:34:57.257820 dagster_polars-0.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 dagster_polars-0.0.3a0/PKG-INFO
```

### Comparing `dagster_polars-0.0.2/LICENSE` & `dagster_polars-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.2/README.md` & `dagster_polars-0.0.3a0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,16 +6,17 @@
  - All IOManagers log various metadata about the DataFrame - size, schema, sample, stats, ...
  - For all IOManagers the `"columns"` input metadata key can be used to select a subset of columns to load
  - `BasePolarsUPathIOManager` is a base class for IO managers that work with Polars DataFrames. Shouldn't be used directly unless you want to implement your own `IOManager`.
    - returns the correct type (`polars.DataFrame` or `polars.LazyFrame`) based on the type annotation
    - inherits all the features of the `UPathIOManager` - works with local and remote filesystems (like S3),
        supports loading multiple partitions (use `dict[str, pl.DataFrame]` type annotation), ...
    - Implemented serialization formats:
-     - `PolarsParquetIOManager` - for reading and writing files in Apache Parquet format. Supports reading partitioned Parquet datasets (for example, often produced by Spark).
- - `BigQueryPolarsIOManager` - for reading and writing data from/to [BigQuery](https://cloud.google.com/bigquery). Supports writing partitioned tables (`"partition_expr"` input metadata key must be specified).
+     - `PolarsParquetIOManager` - for reading and writing files in Apache Parquet format. Supports reading partitioned Parquet datasets (for example, often produced by Spark). All read/write options can be set via metadata values.
+     - `PolarsDeltaIOManager` - for reading and writing Delta Lake. All read/write options can be set via metadata values. `"partition_by"` metadata value can be set to use native Delta Lake partitioning (it's passed to `delta_write_options` of `write_delta`). In this case, all the asset partitions will be stored in the same Delta Table directory. You are responsible for filtering correct partitions when reading the data in the downstream assets. Extra dependencies can be installed with `pip install 'dagster-polars[deltalake]'`.
+ - `BigQueryPolarsIOManager` - for reading and writing data from/to [BigQuery](https://cloud.google.com/bigquery). Supports writing partitioned tables (`"partition_expr"` input metadata key must be specified). Extra dependencies can be installed with `pip install 'dagster-polars[gcp]'`.
 
 ## Quickstart
 
 ### Installation
 
 ```shell
 pip install dagster-polars
@@ -63,11 +64,10 @@
 ```
 
 ### Testing
 ```shell
 poetry run pytest
 ```
 
-## TODO
- - [ ] Add `PolarsDeltaIOManager`
- - [ ] Data validation like in [dagster-pandas](https://docs.dagster.io/integrations/pandas#validating-pandas-dataframes-with-dagster-types)
- - [ ] Maybe use `DagsterTypeLoader` ?
+## Ideas
+ - Data validation like in [dagster-pandas](https://docs.dagster.io/integrations/pandas#validating-pandas-dataframes-with-dagster-types)
+ - Maybe use `DagsterTypeLoader` ?
```

### Comparing `dagster_polars-0.0.2/dagster_polars/io_managers/base.py` & `dagster_polars-0.0.3a0/dagster_polars/io_managers/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import polars as pl
 from dagster import (
     ConfigurableIOManager,
     InitResourceContext,
     InputContext,
     MetadataValue,
+    MultiPartitionKey,
     OutputContext,
     TableColumn,
     TableMetadataValue,
     TableRecord,
     TableSchema,
     UPathIOManager,
 )
@@ -174,7 +175,54 @@
         elif context.dagster_type.typing_type in POLARS_LAZY_FRAME_ANNOTATIONS:
             return ldf
         else:
             raise NotImplementedError(f"Can't load object for type annotation {context.dagster_type.typing_type}")
 
     def get_metadata(self, context: OutputContext, obj: pl.DataFrame) -> Dict[str, MetadataValue]:
         return get_polars_metadata(context, obj)
+
+    @staticmethod
+    def get_storage_options(path: UPath) -> dict:
+        storage_options = {}
+
+        try:
+            storage_options.update(path._kwargs.copy())
+        except AttributeError:
+            pass
+
+        return storage_options
+
+    def get_path_for_partition(self, context: Union[InputContext, OutputContext], path: UPath, partition: str) -> UPath:
+        """
+        Override this method if you want to use a different partitioning scheme
+        (for example, if the saving function handles partitioning instead).
+        The extension will be added later.
+        :param context:
+        :param path: asset path before partitioning
+        :param partition: formatted partition key
+        :return:
+        """
+        return path / partition
+
+    def _get_paths_for_partitions(self, context: Union[InputContext, OutputContext]) -> Dict[str, "UPath"]:
+        """Returns a dict of partition_keys into I/O paths for a given context."""
+        if not context.has_asset_partitions:
+            raise TypeError(
+                f"Detected {context.dagster_type.typing_type} input type " "but the asset is not partitioned"
+            )
+
+        def _formatted_multipartitioned_path(partition_key: MultiPartitionKey) -> str:
+            ordered_dimension_keys = [
+                key[1] for key in sorted(partition_key.keys_by_dimension.items(), key=lambda x: x[0])
+            ]
+            return "/".join(ordered_dimension_keys)
+
+        formatted_partition_keys = [
+            _formatted_multipartitioned_path(pk) if isinstance(pk, MultiPartitionKey) else pk
+            for pk in context.asset_partition_keys
+        ]
+
+        asset_path = self._get_path_without_extension(context)
+        return {
+            partition: self._with_extension(self.get_path_for_partition(context, asset_path, partition))
+            for partition in formatted_partition_keys
+        }
```

### Comparing `dagster_polars-0.0.2/dagster_polars/io_managers/bigquery.py` & `dagster_polars-0.0.3a0/dagster_polars/io_managers/bigquery.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.2/dagster_polars/io_managers/utils.py` & `dagster_polars-0.0.3a0/dagster_polars/io_managers/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.2/pyproject.toml` & `dagster_polars-0.0.3a0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dagster-polars"
-version = "0.0.2"
+version = "0.0.3a0"
 description = "Dagster integration library for Polars"
 authors = [
     "Daniel Gafni <danielgafni16@gmail.com>"
 ]
 readme = "README.md"
 packages = [{include = "dagster_polars"}]
 repository = "https://github.com/danielgafni/dagster-polars"
@@ -26,34 +26,36 @@
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dagster = "^1.3.5"
 polars = ">=0.17.0"
 pyarrow = ">=8.0.0"
+deltalake = "^0.10.0"
 dagster-gcp = "^0.19.5"
 
 
 [tool.poetry.extras]
 gcp = ["dagster-gcp"]
-
+deltalake = ["deltalake"]
 
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "^6.77.0"
 pytest = "^7.3.1"
 deepdiff = "^6.3.0"
 isort = "^5.12.0"
 ruff = "^0.0.272"
 pyright = "^1.1.313"
 tox = "^4.6.0"
 tox-gh = "^1.0.0"
 pre-commit = "^3.3.2"
 dagit = "^1.3.9"
 black = "^23.3.0"
+pytest-cases = "^3.6.14"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `dagster_polars-0.0.2/PKG-INFO` & `dagster_polars-0.0.3a0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-polars
-Version: 0.0.2
+Version: 0.0.3a0
 Summary: Dagster integration library for Polars
 Home-page: https://github.com/danielgafni/dagster-polars
 License: Apache-2.0
 Keywords: dagster,polars,ETL,dataframe
 Author: Daniel Gafni
 Author-email: danielgafni16@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -16,17 +16,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: deltalake
 Provides-Extra: gcp
 Requires-Dist: dagster (>=1.3.5,<2.0.0)
 Requires-Dist: dagster-gcp (>=0.19.5,<0.20.0) ; extra == "gcp"
+Requires-Dist: deltalake (>=0.10.0,<0.11.0) ; extra == "deltalake"
 Requires-Dist: polars (>=0.17.0)
 Requires-Dist: pyarrow (>=8.0.0)
 Project-URL: Repository, https://github.com/danielgafni/dagster-polars
 Description-Content-Type: text/markdown
 
 # `dagster-polars`
 
@@ -36,16 +38,17 @@
  - All IOManagers log various metadata about the DataFrame - size, schema, sample, stats, ...
  - For all IOManagers the `"columns"` input metadata key can be used to select a subset of columns to load
  - `BasePolarsUPathIOManager` is a base class for IO managers that work with Polars DataFrames. Shouldn't be used directly unless you want to implement your own `IOManager`.
    - returns the correct type (`polars.DataFrame` or `polars.LazyFrame`) based on the type annotation
    - inherits all the features of the `UPathIOManager` - works with local and remote filesystems (like S3),
        supports loading multiple partitions (use `dict[str, pl.DataFrame]` type annotation), ...
    - Implemented serialization formats:
-     - `PolarsParquetIOManager` - for reading and writing files in Apache Parquet format. Supports reading partitioned Parquet datasets (for example, often produced by Spark).
- - `BigQueryPolarsIOManager` - for reading and writing data from/to [BigQuery](https://cloud.google.com/bigquery). Supports writing partitioned tables (`"partition_expr"` input metadata key must be specified).
+     - `PolarsParquetIOManager` - for reading and writing files in Apache Parquet format. Supports reading partitioned Parquet datasets (for example, often produced by Spark). All read/write options can be set via metadata values.
+     - `PolarsDeltaIOManager` - for reading and writing Delta Lake. All read/write options can be set via metadata values. `"partition_by"` metadata value can be set to use native Delta Lake partitioning (it's passed to `delta_write_options` of `write_delta`). In this case, all the asset partitions will be stored in the same Delta Table directory. You are responsible for filtering correct partitions when reading the data in the downstream assets. Extra dependencies can be installed with `pip install 'dagster-polars[deltalake]'`.
+ - `BigQueryPolarsIOManager` - for reading and writing data from/to [BigQuery](https://cloud.google.com/bigquery). Supports writing partitioned tables (`"partition_expr"` input metadata key must be specified). Extra dependencies can be installed with `pip install 'dagster-polars[gcp]'`.
 
 ## Quickstart
 
 ### Installation
 
 ```shell
 pip install dagster-polars
@@ -93,12 +96,11 @@
 ```
 
 ### Testing
 ```shell
 poetry run pytest
 ```
 
-## TODO
- - [ ] Add `PolarsDeltaIOManager`
- - [ ] Data validation like in [dagster-pandas](https://docs.dagster.io/integrations/pandas#validating-pandas-dataframes-with-dagster-types)
- - [ ] Maybe use `DagsterTypeLoader` ?
+## Ideas
+ - Data validation like in [dagster-pandas](https://docs.dagster.io/integrations/pandas#validating-pandas-dataframes-with-dagster-types)
+ - Maybe use `DagsterTypeLoader` ?
```

