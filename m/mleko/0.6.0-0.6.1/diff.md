# Comparing `tmp/mleko-0.6.0.tar.gz` & `tmp/mleko-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-0.6.0.tar", max compression
+gzip compressed data, was "mleko-0.6.1.tar", max compression
```

## Comparing `mleko-0.6.0.tar` & `mleko-0.6.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1073 2023-06-26 21:28:47.298938 mleko-0.6.0/LICENSE
--rw-r--r--   0        0        0     2561 2023-06-26 21:28:47.298938 mleko-0.6.0/README.md
--rw-r--r--   0        0        0     1323 2023-06-26 21:29:23.071188 mleko-0.6.0/mleko/__init__.py
--rw-r--r--   0        0        0      584 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/__init__.py
--rw-r--r--   0        0        0    13234 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/cache_mixin.py
--rw-r--r--   0        0        0      805 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/fingerprinters/__init__.py
--rw-r--r--   0        0        0     1167 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/fingerprinters/base_fingerprinter.py
--rw-r--r--   0        0        0     2843 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/fingerprinters/csv_fingerprinter.py
--rw-r--r--   0        0        0     1233 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
--rw-r--r--   0        0        0      398 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/format/__init__.py
--rw-r--r--   0        0        0     1938 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/format/vaex_cache_format_mixin.py
--rw-r--r--   0        0        0     6957 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/lru_cache_mixin.py
--rw-r--r--   0        0        0      740 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/__init__.py
--rw-r--r--   0        0        0      491 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/convert/__init__.py
--rw-r--r--   0        0        0     1530 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/convert/base_converter.py
--rw-r--r--   0        0        0    11709 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/convert/csv_to_vaex_converter.py
--rw-r--r--   0        0        0     1613 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/__init__.py
--rw-r--r--   0        0        0     5979 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/base_feature_selector.py
--rw-r--r--   0        0        0     5332 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/composite_feature_selector.py
--rw-r--r--   0        0        0     5134 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/invariance_feature_selector.py
--rw-r--r--   0        0        0     5387 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
--rw-r--r--   0        0        0     7212 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
--rw-r--r--   0        0        0     5717 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/variance_feature_selector.py
--rw-r--r--   0        0        0      877 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/ingest/__init__.py
--rw-r--r--   0        0        0     2261 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/ingest/base_ingester.py
--rw-r--r--   0        0        0    18020 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/ingest/kaggle_ingester.py
--rw-r--r--   0        0        0     9637 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/ingest/s3_ingester.py
--rw-r--r--   0        0        0      679 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/split/__init__.py
--rw-r--r--   0        0        0     1489 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/split/base_splitter.py
--rw-r--r--   0        0        0     3947 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/split/expression_splitter.py
--rw-r--r--   0        0        0     6066 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/split/random_splitter.py
--rw-r--r--   0        0        0     1611 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/__init__.py
--rw-r--r--   0        0        0     3168 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/base_transformer.py
--rw-r--r--   0        0        0     4556 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/composite_transformer.py
--rw-r--r--   0        0        0     4521 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/frequency_encoder_transformer.py
--rw-r--r--   0        0        0     4153 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/label_encoder_transformer.py
--rw-r--r--   0        0        0     3809 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/max_abs_scaler_transformer.py
--rw-r--r--   0        0        0     4185 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/min_max_scaler_transformer.py
--rw-r--r--   0        0        0      644 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1420 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4496 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     3711 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      697 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     2482 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/steps/convert_step.py
--rw-r--r--   0        0        0     2302 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/steps/feature_select_step.py
--rw-r--r--   0        0        0     2148 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/steps/ingest_step.py
--rw-r--r--   0        0        0     2372 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/steps/split_step.py
--rw-r--r--   0        0        0     2211 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/steps/transform_step.py
--rw-r--r--   0        0        0        0 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/py.typed
--rw-r--r--   0        0        0      765 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/utils/__init__.py
--rw-r--r--   0        0        0     4497 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     3430 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/utils/decorators.py
--rw-r--r--   0        0        0      742 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1413 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/utils/tqdm_helpers.py
--rw-r--r--   0        0        0     2836 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/utils/vaex_helpers.py
--rw-r--r--   0        0        0     2839 2023-06-26 21:29:23.175189 mleko-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 mleko-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-30 10:51:03.036693 mleko-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2561 2023-06-30 10:51:03.036693 mleko-0.6.1/README.md
+-rw-r--r--   0        0        0     1323 2023-06-30 10:51:33.460752 mleko-0.6.1/mleko/__init__.py
+-rw-r--r--   0        0        0      584 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    13234 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0      805 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1167 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     2843 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1233 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0      398 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/format/__init__.py
+-rw-r--r--   0        0        0     1938 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/format/vaex_cache_format_mixin.py
+-rw-r--r--   0        0        0     6957 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      740 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1530 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    12019 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     1613 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0     5979 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     5332 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     5134 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5387 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     7212 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5717 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      877 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     2261 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    18020 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0     9768 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      679 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1489 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     3931 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     6038 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0     1611 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/__init__.py
+-rw-r--r--   0        0        0     3168 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/base_transformer.py
+-rw-r--r--   0        0        0     4556 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/composite_transformer.py
+-rw-r--r--   0        0        0     4521 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/frequency_encoder_transformer.py
+-rw-r--r--   0        0        0     4153 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/label_encoder_transformer.py
+-rw-r--r--   0        0        0     3809 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/max_abs_scaler_transformer.py
+-rw-r--r--   0        0        0     4185 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/min_max_scaler_transformer.py
+-rw-r--r--   0        0        0      644 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1420 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4496 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3711 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      697 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     2482 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     2302 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     2148 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     2372 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0     2211 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/steps/transform_step.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/py.typed
+-rw-r--r--   0        0        0      765 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     4497 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3430 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      742 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1413 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     2836 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2501 2023-06-30 10:51:33.516752 mleko-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 mleko-0.6.1/PKG-INFO
```

### Comparing `mleko-0.6.0/LICENSE` & `mleko-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/README.md` & `mleko-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/__init__.py` & `mleko-0.6.1/mleko/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 Each subpackage is designed to be modular and extensible, making it easy to customize and adapt the library to a wide
 range of model building processes and requirements.
 """
 from __future__ import annotations
 
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
```

### Comparing `mleko-0.6.0/mleko/cache/__init__.py` & `mleko-0.6.1/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/cache/cache_mixin.py` & `mleko-0.6.1/mleko/cache/cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/cache/fingerprinters/__init__.py` & `mleko-0.6.1/mleko/cache/fingerprinters/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/cache/fingerprinters/base_fingerprinter.py` & `mleko-0.6.1/mleko/cache/fingerprinters/base_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/cache/fingerprinters/csv_fingerprinter.py` & `mleko-0.6.1/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/cache/fingerprinters/vaex_fingerprinter.py` & `mleko-0.6.1/mleko/cache/fingerprinters/vaex_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/cache/format/vaex_cache_format_mixin.py` & `mleko-0.6.1/mleko/cache/format/vaex_cache_format_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/cache/lru_cache_mixin.py` & `mleko-0.6.1/mleko/cache/lru_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/__init__.py` & `mleko-0.6.1/mleko/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/convert/base_converter.py` & `mleko-0.6.1/mleko/dataset/convert/base_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/convert/csv_to_vaex_converter.py` & `mleko-0.6.1/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 from __future__ import annotations
 
 import multiprocessing
 from concurrent import futures
 from itertools import repeat
 from pathlib import Path
 
+import pyarrow as pa
 import vaex
 from pyarrow import csv as arrow_csv
 from tqdm.auto import tqdm
 
 from mleko.cache.fingerprinters import CSVFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.file_helpers import clear_directory
+from mleko.utils.vaex_helpers import get_column
 
 from .base_converter import BaseConverter
 
 
 logger = CustomLogger()
 """A module-level logger instance."""
 
@@ -218,14 +220,18 @@
                     "%Y-%m-%d %H:%M:%S.%f",
                     "%Y-%m-%dT%H:%M:%S",
                     "%Y-%m-%dT%H:%M:%S.%f",
                 ],
             ),
         ).drop(drop_columns)
 
+        for column_name in df_chunk.get_column_names():
+            if get_column(df_chunk, column_name).dtype in (pa.date32(), pa.date64()):
+                df_chunk[column_name] = get_column(df_chunk, column_name).astype("datetime64[s]")
+
         output_path = output_directory / f"df_chunk_{file_path.stem}.{dataframe_suffix}"
         df_chunk.export(output_path, chunk_size=100_000, parallel=False)
         df_chunk.close()
 
     def _convert(self, file_paths: list[Path] | list[str]) -> vaex.DataFrame:
         """Converts a list of CSV files to Arrow format using parallel processing.
```

### Comparing `mleko-0.6.0/mleko/dataset/feature_select/__init__.py` & `mleko-0.6.1/mleko/dataset/feature_select/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/feature_select/base_feature_selector.py` & `mleko-0.6.1/mleko/dataset/feature_select/base_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/feature_select/composite_feature_selector.py` & `mleko-0.6.1/mleko/dataset/feature_select/composite_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/feature_select/invariance_feature_selector.py` & `mleko-0.6.1/mleko/dataset/feature_select/invariance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/feature_select/missing_rate_feature_selector.py` & `mleko-0.6.1/mleko/dataset/feature_select/missing_rate_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py` & `mleko-0.6.1/mleko/dataset/feature_select/pearson_correlation_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/feature_select/variance_feature_selector.py` & `mleko-0.6.1/mleko/dataset/feature_select/variance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/ingest/__init__.py` & `mleko-0.6.1/mleko/dataset/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/ingest/base_ingester.py` & `mleko-0.6.1/mleko/dataset/ingest/base_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/ingest/kaggle_ingester.py` & `mleko-0.6.1/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/ingest/s3_ingester.py` & `mleko-0.6.1/mleko/dataset/ingest/s3_ingester.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self,
         destination_directory: str | Path,
         s3_bucket_name: str,
         s3_key_prefix: str,
         aws_profile_name: str | None = None,
         aws_region_name: str = "eu-west-1",
         num_workers: int = 64,
-        manifest_file_name: str = "manifest",
+        manifest_file_name: str | None = "manifest",
         check_s3_timestamps: bool = True,
     ) -> None:
         """Initializes the S3 bucket client, configures the destination directory, and sets client-related parameters.
 
         Note:
             The S3 bucket client is initialized using the provided AWS profile and region. If no profile is provided,
             the default profile will be used. If no region is provided, the default region will be used.
@@ -107,35 +107,35 @@
 
         if self._check_s3_timestamps:
             modification_dates = {key["LastModified"].day for key in resp["Contents"] if "LastModified" in key}
             if len(modification_dates) != 1:
                 raise Exception(
                     "Files in S3 are from muliples dates. This might mean the data is corrupted/duplicated."
                 )
-
-        manifest_file_key = next(
-            entry["Key"]
-            for entry in resp["Contents"]
-            if "Key" in entry and entry["Key"].endswith(self._manifest_file_name)
-        )
-
-        if not force_recompute and manifest_file_key:
-            self._s3_client.download_file(
-                Bucket=self._s3_bucket_name,
-                Key=manifest_file_key,
-                Filename=str(self._destination_directory / self._manifest_file_name),
+        if self._manifest_file_name is not None:
+            manifest_file_key = next(
+                entry["Key"]
+                for entry in resp["Contents"]
+                if "Key" in entry and entry["Key"].endswith(self._manifest_file_name)
             )
-            with open(self._destination_directory / self._manifest_file_name) as f:
-                manifest: dict[str, Any] = json.load(f)
-                if self._is_local_dataset_fresh(manifest):
-                    logger.info(
-                        "\033[32mCache Hit\033[0m: Local dataset is up to date with S3 bucket contents, "
-                        "skipping download."
-                    )
-                    return self._get_local_filenames(["gz", "csv", "zip"])
+
+            if not force_recompute and manifest_file_key:
+                self._s3_client.download_file(
+                    Bucket=self._s3_bucket_name,
+                    Key=manifest_file_key,
+                    Filename=str(self._destination_directory / self._manifest_file_name),
+                )
+                with open(self._destination_directory / self._manifest_file_name) as f:
+                    manifest: dict[str, Any] = json.load(f)
+                    if self._is_local_dataset_fresh(manifest):
+                        logger.info(
+                            "\033[32mCache Hit\033[0m: Local dataset is up to date with S3 bucket contents, "
+                            "skipping download."
+                        )
+                        return self._get_local_filenames(["gz", "csv", "zip"])
 
         if force_recompute:
             logger.info(
                 f"\033[33mForce Cache Refresh\033[0m: Downloading {self._s3_bucket_name}/{self._s3_key_prefix} to "
                 f"{self._destination_directory} from S3."
             )
         else:
```

### Comparing `mleko-0.6.0/mleko/dataset/split/__init__.py` & `mleko-0.6.1/mleko/dataset/split/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/split/base_splitter.py` & `mleko-0.6.1/mleko/dataset/split/base_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/split/expression_splitter.py` & `mleko-0.6.1/mleko/dataset/split/expression_splitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             dataframe: The dataframe to be split.
             cache_group: The cache group to use.
             force_recompute: Forces recomputation if True, otherwise reads from the cache if available.
 
         Returns:
             A tuple containing the split dataframes.
         """
-        return self._cached_execute(  # type: ignore
+        return self._cached_execute(
             lambda_func=lambda: self._split(dataframe),
             cache_keys=[
                 self._expression,
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
```

### Comparing `mleko-0.6.0/mleko/dataset/split/random_splitter.py` & `mleko-0.6.1/mleko/dataset/split/random_splitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             dataframe: The dataframe to be split.
             cache_group: The cache group to use.
             force_recompute: Whether to force recompute the split, even if the cache is available.
 
         Returns:
             A tuple containing the split dataframes.
         """
-        return self._cached_execute(  # type: ignore
+        return self._cached_execute(
             lambda_func=lambda: self._split(dataframe),
             cache_keys=[
                 self._idx2_size,
                 self._shuffle,
                 self._stratify,
                 self._random_state,
                 (dataframe, VaexFingerprinter()),
@@ -114,17 +114,18 @@
         Args:
             dataframe: The dataframe to be split.
 
         Returns:
             A tuple containing the split dataframes.
         """
         index_name = "index"
-        dataframe[index_name] = vaex.vrange(0, dataframe.shape[0])
-        index = get_column(dataframe, index_name)
-        target = get_column(dataframe, self._stratify).to_numpy() if self._stratify else None
+        df = dataframe.copy()
+        df[index_name] = vaex.vrange(0, df.shape[0])
+        index = get_column(df, index_name)
+        target = get_column(df, self._stratify).to_numpy() if self._stratify else None
 
         if self._shuffle:
             logger.info("Shuffling data before splitting.")
         if target is None:
             logger.info("Splitting data without stratification.")
         else:
             logger.info(f"Splitting data with stratification on column {self._stratify!r}.")
@@ -133,13 +134,13 @@
             index.values,
             test_size=self._idx2_size,
             random_state=self._random_state,
             shuffle=self._shuffle,
             stratify=target,
         )
 
-        df1 = get_filtered_df(dataframe, index.isin(idx1)).extract()
-        df2 = get_filtered_df(dataframe, index.isin(idx2)).extract()
+        df1 = get_filtered_df(df, index.isin(idx1)).extract()
+        df2 = get_filtered_df(df, index.isin(idx2)).extract()
         logger.info(f"Split dataframe into two dataframes with shapes {df1.shape} and {df2.shape}.")
         df1.delete_virtual_column(index_name)
         df2.delete_virtual_column(index_name)
         return df1, df2
```

### Comparing `mleko-0.6.0/mleko/dataset/transform/__init__.py` & `mleko-0.6.1/mleko/dataset/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/transform/base_transformer.py` & `mleko-0.6.1/mleko/dataset/transform/base_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/transform/composite_transformer.py` & `mleko-0.6.1/mleko/dataset/transform/composite_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/transform/frequency_encoder_transformer.py` & `mleko-0.6.1/mleko/dataset/transform/frequency_encoder_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/transform/label_encoder_transformer.py` & `mleko-0.6.1/mleko/dataset/transform/label_encoder_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/transform/max_abs_scaler_transformer.py` & `mleko-0.6.1/mleko/dataset/transform/max_abs_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/dataset/transform/min_max_scaler_transformer.py` & `mleko-0.6.1/mleko/dataset/transform/min_max_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/pipeline/__init__.py` & `mleko-0.6.1/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/pipeline/data_container.py` & `mleko-0.6.1/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/pipeline/pipeline.py` & `mleko-0.6.1/mleko/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/pipeline/pipeline_step.py` & `mleko-0.6.1/mleko/pipeline/pipeline_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/pipeline/steps/__init__.py` & `mleko-0.6.1/mleko/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/pipeline/steps/convert_step.py` & `mleko-0.6.1/mleko/pipeline/steps/convert_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/pipeline/steps/feature_select_step.py` & `mleko-0.6.1/mleko/pipeline/steps/feature_select_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/pipeline/steps/ingest_step.py` & `mleko-0.6.1/mleko/pipeline/steps/ingest_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/pipeline/steps/split_step.py` & `mleko-0.6.1/mleko/pipeline/steps/split_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/pipeline/steps/transform_step.py` & `mleko-0.6.1/mleko/pipeline/steps/transform_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/utils/__init__.py` & `mleko-0.6.1/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/utils/custom_logger.py` & `mleko-0.6.1/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/utils/decorators.py` & `mleko-0.6.1/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/utils/file_helpers.py` & `mleko-0.6.1/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/utils/tqdm_helpers.py` & `mleko-0.6.1/mleko/utils/tqdm_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/mleko/utils/vaex_helpers.py` & `mleko-0.6.1/mleko/utils/vaex_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.0/pyproject.toml` & `mleko-0.6.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "0.6.0"
+version = "0.6.1"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ErikBavenstrand/mleko"
 repository = "https://github.com/ErikBavenstrand/mleko"
 documentation = "https://mleko.readthedocs.io"
@@ -12,15 +12,15 @@
     "Development Status :: 3 - Alpha",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/ErikBavenstrand/mleko/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = "3.10.* || 3.9.* || 3.8.*"
+python = ">=3.8,<3.11.dev0"
 boto3 = "^1.26.91"
 botocore = "^1.29.91"
 tqdm = "^4.65.0"
 vaex = "^4.16.0"
 scikit-learn = "^1.2.2"
 
 [tool.poetry.group.dev.dependencies]
@@ -33,77 +33,58 @@
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
 flake8-rst-docstrings = ">=0.2.5"
 furo = ">=2021.11.12"
 isort = ">=5.10.1"
 moto = "^4.1.4"
-mypy = ">=0.930"
 pep8-naming = ">=0.12.1"
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
 pytest = ">=6.2.5"
 pytest-mock = "^3.10.0"
 pyupgrade = ">=2.29.1"
 safety = ">=1.10.3"
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 typeguard = ">=2.13.3"
-myst-parser = {version = ">=0.16.1"}
+myst-parser = ">=0.16.1"
 ipykernel = "^6.21.3"
-mypy-boto3-s3 = "^1.26.116"
-nox = "^2023.4.22"
-nox-poetry = "^1.0.2"
 sphinx-autodoc-typehints = "^1.23.0"
 sphinx-autoapi = "^2.1.0"
 python-semantic-release = "^7.33.3"
+pyright = "^1.1.316"
 
 [tool.coverage.paths]
 source = ["mleko", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = false
 source = ["mleko"]
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 100
-exclude_lines = ["pragma: no cover", "raise NotImplementedError", '"""', "self._cached_execute"]
+exclude_lines = ["pragma: no cover", "raise NotImplementedError", '"""']
 
 [tool.isort]
 profile = "black"
 lines_after_imports = 2
 line_length = 120
 use_parentheses = true
 include_trailing_comma = true
 
 [tool.black]
 line-length = 120
 
-[tool.mypy]
-strict = true
-warn_unreachable = true
-pretty = true
-show_column_numbers = true
-show_error_codes = true
-show_error_context = true
-
-
-[[tool.mypy.overrides]]
-module = [
-    "vaex.*",
-    "tqdm.*",
-    "boto3.*",
-    "botocore.*",
-    "pyarrow.*",
-    "requests.*",
-    "sklearn.*",
-]
-ignore_missing_imports = true
+[tool.pyright]
+include = ["mleko"]
+reportMissingImports = true
+reportMissingTypeStubs = false
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 branch = "main"
```

### Comparing `mleko-0.6.0/PKG-INFO` & `mleko-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 0.6.0
+Version: 0.6.1
 Summary: ML-Ekosystem
 Home-page: https://github.com/ErikBavenstrand/mleko
 License: MIT
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
-Requires-Python: >=3.8.0,<3.11.0
+Requires-Python: >=3.8,<3.11.dev0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: boto3 (>=1.26.91,<2.0.0)
```

