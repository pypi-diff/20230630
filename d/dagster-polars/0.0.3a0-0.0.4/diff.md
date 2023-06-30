# Comparing `tmp/dagster_polars-0.0.3a0.tar.gz` & `tmp/dagster_polars-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_polars-0.0.3a0.tar", max compression
+gzip compressed data, was "dagster_polars-0.0.4.tar", max compression
```

## Comparing `dagster_polars-0.0.3a0.tar` & `dagster_polars-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11344 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/LICENSE
--rw-r--r--   0        0        0     3070 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/README.md
--rw-r--r--   0        0        0      358 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/__init__.py
--rw-r--r--   0        0        0       78 2023-06-30 10:34:57.257820 dagster_polars-0.0.3a0/dagster_polars/_version.py
--rw-r--r--   0        0        0        0 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/io_managers/__init__.py
--rw-r--r--   0        0        0     7896 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/io_managers/base.py
--rw-r--r--   0        0        0     7200 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/io_managers/bigquery.py
--rw-r--r--   0        0        0     3074 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/io_managers/delta.py
--rw-r--r--   0        0        0     2143 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/io_managers/parquet.py
--rw-r--r--   0        0        0     3936 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/io_managers/utils.py
--rw-r--r--   0        0        0        0 2023-06-30 10:34:26.557328 dagster_polars-0.0.3a0/dagster_polars/py.typed
--rw-r--r--   0        0        0     2880 2023-06-30 10:34:57.257820 dagster_polars-0.0.3a0/pyproject.toml
--rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 dagster_polars-0.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3158 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/README.md
+-rw-r--r--   0        0        0      358 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/__init__.py
+-rw-r--r--   0        0        0       76 2023-06-30 18:53:16.726448 dagster_polars-0.0.4/dagster_polars/_version.py
+-rw-r--r--   0        0        0        0 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/io_managers/__init__.py
+-rw-r--r--   0        0        0     7896 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/io_managers/base.py
+-rw-r--r--   0        0        0     7200 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/io_managers/bigquery.py
+-rw-r--r--   0        0        0     4417 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/io_managers/delta.py
+-rw-r--r--   0        0        0     2143 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/io_managers/parquet.py
+-rw-r--r--   0        0        0     3936 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/io_managers/utils.py
+-rw-r--r--   0        0        0        0 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/py.typed
+-rw-r--r--   0        0        0     2878 2023-06-30 18:53:16.726448 dagster_polars-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 dagster_polars-0.0.4/PKG-INFO
```

### Comparing `dagster_polars-0.0.3a0/LICENSE` & `dagster_polars-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.3a0/README.md` & `dagster_polars-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  - For all IOManagers the `"columns"` input metadata key can be used to select a subset of columns to load
  - `BasePolarsUPathIOManager` is a base class for IO managers that work with Polars DataFrames. Shouldn't be used directly unless you want to implement your own `IOManager`.
    - returns the correct type (`polars.DataFrame` or `polars.LazyFrame`) based on the type annotation
    - inherits all the features of the `UPathIOManager` - works with local and remote filesystems (like S3),
        supports loading multiple partitions (use `dict[str, pl.DataFrame]` type annotation), ...
    - Implemented serialization formats:
      - `PolarsParquetIOManager` - for reading and writing files in Apache Parquet format. Supports reading partitioned Parquet datasets (for example, often produced by Spark). All read/write options can be set via metadata values.
-     - `PolarsDeltaIOManager` - for reading and writing Delta Lake. All read/write options can be set via metadata values. `"partition_by"` metadata value can be set to use native Delta Lake partitioning (it's passed to `delta_write_options` of `write_delta`). In this case, all the asset partitions will be stored in the same Delta Table directory. You are responsible for filtering correct partitions when reading the data in the downstream assets. Extra dependencies can be installed with `pip install 'dagster-polars[deltalake]'`.
+     - `PolarsDeltaIOManager` - for reading and writing Delta Lake. All read/write options can be set via metadata values. `"partition_by"` metadata value can be set to use native Delta Lake partitioning (it's passed to `delta_write_options` of `write_delta`). In this case, all the asset partitions will be stored in the same Delta Table directory. You are responsible for filtering correct partitions when reading the data in the downstream assets. Extra dependencies can be installed with `pip install 'dagster-polars[deltalake]'`. **Warning** [doesn't work good](https://github.com/pola-rs/polars/issues/9635) on MacOS
  - `BigQueryPolarsIOManager` - for reading and writing data from/to [BigQuery](https://cloud.google.com/bigquery). Supports writing partitioned tables (`"partition_expr"` input metadata key must be specified). Extra dependencies can be installed with `pip install 'dagster-polars[gcp]'`.
 
 ## Quickstart
 
 ### Installation
 
 ```shell
```

### Comparing `dagster_polars-0.0.3a0/dagster_polars/io_managers/base.py` & `dagster_polars-0.0.4/dagster_polars/io_managers/base.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.3a0/dagster_polars/io_managers/bigquery.py` & `dagster_polars-0.0.4/dagster_polars/io_managers/bigquery.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.3a0/dagster_polars/io_managers/delta.py` & `dagster_polars-0.0.4/dagster_polars/io_managers/delta.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pprint import pformat
-from typing import Union
+from typing import Dict, Union
 
 import polars as pl
-from dagster import InputContext, OutputContext
+from dagster import InputContext, MetadataValue, OutputContext
 from deltalake import DeltaTable
 from upath import UPath
 
 from dagster_polars.io_managers.base import BasePolarsUPathIOManager
 
 
 class PolarsDeltaIOManager(BasePolarsUPathIOManager):
@@ -15,31 +15,14 @@
     assert BasePolarsUPathIOManager.__doc__ is not None
     __doc__ = (
         BasePolarsUPathIOManager.__doc__
         + """\nWorks with Delta files.
     All read/write arguments can be passed via corresponding metadata values."""
     )
 
-    def get_path_for_partition(self, context: Union[InputContext, OutputContext], path: UPath, partition: str) -> UPath:
-        if isinstance(context, InputContext):
-            if (
-                context.upstream_output is not None
-                and context.upstream_output.metadata is not None
-                and context.upstream_output.metadata.get("partition_by") is not None
-            ):
-                # upstream asset has "partition_by" metadata set, so partitioning for it is handled by DeltaLake itself
-                return path
-
-        if isinstance(context, OutputContext):
-            if context.metadata is not None and context.metadata.get("partition_by") is not None:
-                # this asset has "partition_by" metadata set, so partitioning for it is handled by DeltaLake itself
-                return path
-
-        return path / partition  # partitioning is handled by the IOManager
-
     def dump_df_to_path(self, context: OutputContext, df: pl.DataFrame, path: UPath):
         assert context.metadata is not None
 
         delta_write_options = context.metadata.get("delta_write_options")
 
         if context.has_asset_partitions:
             delta_write_options = delta_write_options or {}
@@ -69,7 +52,56 @@
         return pl.scan_delta(
             str(path),
             version=context.metadata.get("version"),
             delta_table_options=context.metadata.get("delta_table_options"),
             pyarrow_options=context.metadata.get("pyarrow_options"),
             storage_options=self.get_storage_options(path),
         )
+
+    def get_path_for_partition(self, context: Union[InputContext, OutputContext], path: UPath, partition: str) -> UPath:
+        if isinstance(context, InputContext):
+            if (
+                context.upstream_output is not None
+                and context.upstream_output.metadata is not None
+                and context.upstream_output.metadata.get("partition_by") is not None
+            ):
+                # upstream asset has "partition_by" metadata set, so partitioning for it is handled by DeltaLake itself
+                return path
+
+        if isinstance(context, OutputContext):
+            if context.metadata is not None and context.metadata.get("partition_by") is not None:
+                # this asset has "partition_by" metadata set, so partitioning for it is handled by DeltaLake itself
+                return path
+
+        return path / partition  # partitioning is handled by the IOManager
+
+    def get_metadata(self, context: OutputContext, obj: pl.DataFrame) -> Dict[str, MetadataValue]:
+        assert context.metadata is not None
+
+        metadata = super().get_metadata(context, obj)
+
+        if context.has_asset_partitions:
+            partition_by = context.metadata.get("partition_by")
+            if partition_by is not None:
+                metadata["partition_by"] = partition_by
+
+        if context.metadata.get("mode") == "append":
+            # FIXME: what to do if we are appending to a partitioned table?
+            # we should not be using the full table length,
+            # but it's unclear how to get the length of the partition we are appending to
+
+            if context.has_asset_partitions:
+                paths = self._get_paths_for_partitions(context)
+                assert len(paths) == 1
+                path = list(paths.values())[0]
+            else:
+                path = self._get_path(context)
+
+            if not context.has_asset_partitions:
+                # we need to get num_rows from the full table
+                metadata["num_rows"] = MetadataValue.int(
+                    DeltaTable(str(path), storage_options=self.get_storage_options(path))
+                    .to_pyarrow_dataset()
+                    .count_rows()
+                )
+
+        return metadata
```

### Comparing `dagster_polars-0.0.3a0/dagster_polars/io_managers/parquet.py` & `dagster_polars-0.0.4/dagster_polars/io_managers/parquet.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.3a0/dagster_polars/io_managers/utils.py` & `dagster_polars-0.0.4/dagster_polars/io_managers/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.3a0/pyproject.toml` & `dagster_polars-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dagster-polars"
-version = "0.0.3a0"
+version = "0.0.4"
 description = "Dagster integration library for Polars"
 authors = [
     "Daniel Gafni <danielgafni16@gmail.com>"
 ]
 readme = "README.md"
 packages = [{include = "dagster_polars"}]
 repository = "https://github.com/danielgafni/dagster-polars"
```

### Comparing `dagster_polars-0.0.3a0/PKG-INFO` & `dagster_polars-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-polars
-Version: 0.0.3a0
+Version: 0.0.4
 Summary: Dagster integration library for Polars
 Home-page: https://github.com/danielgafni/dagster-polars
 License: Apache-2.0
 Keywords: dagster,polars,ETL,dataframe
 Author: Daniel Gafni
 Author-email: danielgafni16@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -39,15 +39,15 @@
  - For all IOManagers the `"columns"` input metadata key can be used to select a subset of columns to load
  - `BasePolarsUPathIOManager` is a base class for IO managers that work with Polars DataFrames. Shouldn't be used directly unless you want to implement your own `IOManager`.
    - returns the correct type (`polars.DataFrame` or `polars.LazyFrame`) based on the type annotation
    - inherits all the features of the `UPathIOManager` - works with local and remote filesystems (like S3),
        supports loading multiple partitions (use `dict[str, pl.DataFrame]` type annotation), ...
    - Implemented serialization formats:
      - `PolarsParquetIOManager` - for reading and writing files in Apache Parquet format. Supports reading partitioned Parquet datasets (for example, often produced by Spark). All read/write options can be set via metadata values.
-     - `PolarsDeltaIOManager` - for reading and writing Delta Lake. All read/write options can be set via metadata values. `"partition_by"` metadata value can be set to use native Delta Lake partitioning (it's passed to `delta_write_options` of `write_delta`). In this case, all the asset partitions will be stored in the same Delta Table directory. You are responsible for filtering correct partitions when reading the data in the downstream assets. Extra dependencies can be installed with `pip install 'dagster-polars[deltalake]'`.
+     - `PolarsDeltaIOManager` - for reading and writing Delta Lake. All read/write options can be set via metadata values. `"partition_by"` metadata value can be set to use native Delta Lake partitioning (it's passed to `delta_write_options` of `write_delta`). In this case, all the asset partitions will be stored in the same Delta Table directory. You are responsible for filtering correct partitions when reading the data in the downstream assets. Extra dependencies can be installed with `pip install 'dagster-polars[deltalake]'`. **Warning** [doesn't work good](https://github.com/pola-rs/polars/issues/9635) on MacOS
  - `BigQueryPolarsIOManager` - for reading and writing data from/to [BigQuery](https://cloud.google.com/bigquery). Supports writing partitioned tables (`"partition_expr"` input metadata key must be specified). Extra dependencies can be installed with `pip install 'dagster-polars[gcp]'`.
 
 ## Quickstart
 
 ### Installation
 
 ```shell
```

