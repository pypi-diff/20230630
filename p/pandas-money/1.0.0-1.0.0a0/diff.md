# Comparing `tmp/pandas_money-1.0.0.tar.gz` & `tmp/pandas_money-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_money-1.0.0.tar", max compression
+gzip compressed data, was "pandas_money-1.0.0a0.tar", max compression
```

## Comparing `pandas_money-1.0.0.tar` & `pandas_money-1.0.0a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-06-30 05:04:36.811032 pandas_money-1.0.0/LICENSE
--rw-r--r--   0        0        0      859 2023-06-30 05:04:36.811032 pandas_money-1.0.0/README.md
--rw-r--r--   0        0        0      205 2023-06-30 05:53:39.553726 pandas_money-1.0.0/pandas_money/__init__.py
--rw-r--r--   0        0        0     9101 2023-06-30 05:53:39.553726 pandas_money-1.0.0/pandas_money/money_dtype.py
--rw-r--r--   0        0        0        0 2023-06-30 05:04:36.811032 pandas_money-1.0.0/pandas_money/tests/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-30 05:53:39.553726 pandas_money-1.0.0/pandas_money/tests/test_indexing.py
--rw-r--r--   0        0        0    13588 2023-06-30 05:53:39.553726 pandas_money-1.0.0/pandas_money/tests/test_money_dtype.py
--rw-r--r--   0        0        0     1434 2023-06-30 05:55:24.209191 pandas_money-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 pandas_money-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-30 05:04:36.811032 pandas_money-1.0.0a0/LICENSE
+-rw-r--r--   0        0        0      859 2023-06-30 05:04:36.811032 pandas_money-1.0.0a0/README.md
+-rw-r--r--   0        0        0      205 2023-06-30 05:18:57.449605 pandas_money-1.0.0a0/pandas_money/__init__.py
+-rw-r--r--   0        0        0     9101 2023-06-30 05:25:35.843642 pandas_money-1.0.0a0/pandas_money/money_dtype.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:04:36.811032 pandas_money-1.0.0a0/pandas_money/tests/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-30 05:35:43.600152 pandas_money-1.0.0a0/pandas_money/tests/test_indexing.py
+-rw-r--r--   0        0        0    13588 2023-06-30 05:37:10.007633 pandas_money-1.0.0a0/pandas_money/tests/test_money_dtype.py
+-rw-r--r--   0        0        0     1436 2023-06-30 05:45:14.148675 pandas_money-1.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1547 1970-01-01 00:00:00.000000 pandas_money-1.0.0a0/PKG-INFO
```

### Comparing `pandas_money-1.0.0/LICENSE` & `pandas_money-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_money-1.0.0/README.md` & `pandas_money-1.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `pandas_money-1.0.0/pandas_money/money_dtype.py` & `pandas_money-1.0.0a0/pandas_money/money_dtype.py`

 * *Files identical despite different names*

### Comparing `pandas_money-1.0.0/pandas_money/tests/test_indexing.py` & `pandas_money-1.0.0a0/pandas_money/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `pandas_money-1.0.0/pandas_money/tests/test_money_dtype.py` & `pandas_money-1.0.0a0/pandas_money/tests/test_money_dtype.py`

 * *Files identical despite different names*

### Comparing `pandas_money-1.0.0/pyproject.toml` & `pandas_money-1.0.0a0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandas-money"
-version = "1.0.0"
+version = "1.0.0a0"
 description = "A Pandas ArrayExtension for handling currency with int64 performance"
 authors = ["Rod Morison <rmorison@users.noreply.github.com>"]
 repository = "https://github.com/rmorison/pandas-money"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandas_money"}]
```

### Comparing `pandas_money-1.0.0/PKG-INFO` & `pandas_money-1.0.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-money
-Version: 1.0.0
+Version: 1.0.0a0
 Summary: A Pandas ArrayExtension for handling currency with int64 performance
 Home-page: https://github.com/rmorison/pandas-money
 License: MIT
 Author: Rod Morison
 Author-email: rmorison@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

