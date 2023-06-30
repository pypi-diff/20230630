# Comparing `tmp/lamin_logger-0.7.2.tar.gz` & `tmp/lamin_logger-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.7.2.tar` & `lamin_logger-0.7.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.2/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.2/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.2/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.2/docs/api.md
--rw-r--r--   0        0        0     4471 2023-06-22 14:21:14.438600 lamin_logger-0.7.2/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.2/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.2/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.2/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-06-29 16:03:54.672354 lamin_logger-0.7.2/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.2/lamin_logger/_core.py
--rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.7.2/lamin_logger/_inspect.py
--rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.7.2/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.7.2/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     7160 2023-06-22 14:19:30.503212 lamin_logger-0.7.2/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.2/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     3139 2023-06-19 17:49:41.483432 lamin_logger-0.7.2/lamin_logger/_search.py
--rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.2/noxfile.py
--rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.2/tests/test_base.py
--rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.7.2/tests/test_inspect.py
--rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.2/tests/test_lookup.py
--rw-r--r--   0        0        0     5769 2023-06-22 14:19:30.503907 lamin_logger-0.7.2/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.2/tests/test_notebooks.py
--rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.2/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.3/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.3/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.3/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.3/docs/api.md
+-rw-r--r--   0        0        0     4628 2023-06-30 14:11:53.021008 lamin_logger-0.7.3/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.3/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.3/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.3/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-06-30 14:11:44.881763 lamin_logger-0.7.3/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.3/lamin_logger/_core.py
+-rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.7.3/lamin_logger/_inspect.py
+-rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.7.3/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.7.3/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     7294 2023-06-30 14:10:22.361261 lamin_logger-0.7.3/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.3/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     3139 2023-06-19 17:49:41.483432 lamin_logger-0.7.3/lamin_logger/_search.py
+-rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.3/noxfile.py
+-rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.3/tests/test_base.py
+-rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.7.3/tests/test_inspect.py
+-rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.3/tests/test_lookup.py
+-rw-r--r--   0        0        0     5965 2023-06-30 14:10:22.361575 lamin_logger-0.7.3/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.3/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.3/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.3/PKG-INFO
```

### Comparing `lamin_logger-0.7.2/.github/workflows/build.yml` & `lamin_logger-0.7.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/.github/workflows/latest-changes.yml` & `lamin_logger-0.7.3/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/.gitignore` & `lamin_logger-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/.pre-commit-config.yaml` & `lamin_logger-0.7.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/LICENSE` & `lamin_logger-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/docs/changelog.md` & `lamin_logger-0.7.3/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚑️ Handles categorical input | [32](https://github.com/laminlabs/lamin-logger/pull/32) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-30 | 0.7.3
 🐛 Fix case sensitivity in map_synonyms | [31](https://github.com/laminlabs/lamin-logger/pull/31) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-22 | 0.7.1
 🚚 Moved inspect from bionty | [30](https://github.com/laminlabs/lamin-logger/pull/30) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-21 | 0.7.0
 🚑️ Map_synonyms only returns mapped synonyms not names | [29](https://github.com/laminlabs/lamin-logger/pull/29) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-20 | 0.6.2
 🧪 Deal with empty dataframes | [28](https://github.com/laminlabs/lamin-logger/pull/28) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-19 | 0.6.1
 ✨ Add case_sensitive to map_synonyms | [27](https://github.com/laminlabs/lamin-logger/pull/27) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-19 | 0.6.0
 🧪 Test every line of search | [25](https://github.com/laminlabs/lamin-logger/pull/25) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 | 0.5.3
 🚑️ Fix empty string input for `map_synonyms` | [24](https://github.com/laminlabs/lamin-logger/pull/24) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 |
```

### Comparing `lamin_logger-0.7.2/docs/quickstart.ipynb` & `lamin_logger-0.7.3/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/lamin_logger/_core.py` & `lamin_logger-0.7.3/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/lamin_logger/_inspect.py` & `lamin_logger-0.7.3/lamin_logger/_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/lamin_logger/_logger.py` & `lamin_logger-0.7.3/lamin_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/lamin_logger/_lookup.py` & `lamin_logger-0.7.3/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/lamin_logger/_map_synonyms.py` & `lamin_logger-0.7.3/lamin_logger/_map_synonyms.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,18 @@
             ]
         else:
             return mapped_list
 
 
 def to_str(identifiers: Any, case_sensitive: bool = False):
     """Convert a pandas series values to strings with case sensitive option."""
-    values = identifiers.fillna("")
+    if identifiers.dtype.name == "category":
+        values = identifiers.cat.add_categories("").fillna("").astype(str)
+    else:
+        values = identifiers.fillna("")
     if case_sensitive is False:
         values = values.str.lower()
     return values
 
 
 def check_if_ids_in_field_values(
     identifiers: Iterable, field_values: Iterable, case_sensitive: bool = False
```

### Comparing `lamin_logger-0.7.2/lamin_logger/_python_version.py` & `lamin_logger-0.7.3/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/lamin_logger/_search.py` & `lamin_logger-0.7.3/lamin_logger/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/pyproject.toml` & `lamin_logger-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/tests/test_inspect.py` & `lamin_logger-0.7.3/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/tests/test_lookup.py` & `lamin_logger-0.7.3/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/tests/test_map_synonyms.py` & `lamin_logger-0.7.3/tests/test_map_synonyms.py`

 * *Files 5% similar despite different names*

```diff
@@ -206,7 +206,16 @@
             df, agg_col="synonyms", target_col="symbol", keep="last"
         ).get("GCS")
         == "UGCG"
     )
     assert explode_aggregated_column_to_map(
         df, agg_col="synonyms", target_col="symbol", keep=False
     ).get("GCS") == ["GCLC", "UGCG"]
+
+
+def test_to_str_categorical_series():
+    import numpy as np
+
+    df = pd.DataFrame([np.nan, None, "a"])
+    df[0] = df[0].astype("category")
+
+    assert to_str(df[0]).tolist() == ["", "", "a"]
```

### Comparing `lamin_logger-0.7.2/tests/test_search.py` & `lamin_logger-0.7.3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.2/PKG-INFO` & `lamin_logger-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.7.2
+Version: 0.7.3
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

