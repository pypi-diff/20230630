# Comparing `tmp/pandas_money-0.2.2.tar.gz` & `tmp/pandas_money-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_money-0.2.2.tar", max compression
+gzip compressed data, was "pandas_money-1.0.0a0.tar", max compression
```

## Comparing `pandas_money-0.2.2.tar` & `pandas_money-1.0.0a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-06-09 03:17:36.171096 pandas_money-0.2.2/LICENSE
--rw-r--r--   0        0        0      859 2023-06-12 22:53:26.115878 pandas_money-0.2.2/README.md
--rw-r--r--   0        0        0      207 2023-06-16 17:48:47.618208 pandas_money-0.2.2/pandas_money/__init__.py
--rw-r--r--   0        0        0     9019 2023-06-26 05:54:45.243155 pandas_money-0.2.2/pandas_money/money_dtype.py
--rw-r--r--   0        0        0        0 2023-06-16 17:48:47.622207 pandas_money-0.2.2/pandas_money/tests/__init__.py
--rw-r--r--   0        0        0     1901 2023-06-26 05:54:45.243155 pandas_money-0.2.2/pandas_money/tests/test_indexing.py
--rw-r--r--   0        0        0    13160 2023-06-16 17:48:47.622207 pandas_money-0.2.2/pandas_money/tests/test_money_dtype.py
--rw-r--r--   0        0        0     1434 2023-06-26 05:54:45.243155 pandas_money-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 pandas_money-0.2.2/PKG-INFO
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

### Comparing `pandas_money-0.2.2/LICENSE` & `pandas_money-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_money-0.2.2/README.md` & `pandas_money-1.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `pandas_money-0.2.2/pandas_money/money_dtype.py` & `pandas_money-1.0.0a0/pandas_money/money_dtype.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     ExtensionArray,
     ExtensionScalarOpsMixin,
     register_extension_dtype,
 )
 from pandas.core.dtypes.base import ExtensionDtype
 from pandas.core.dtypes.common import is_dtype_equal, pandas_dtype
 from pandas.core.dtypes.dtypes import PandasExtensionDtype
-from pandas.core.dtypes.inference import is_integer
 
 money_decimals = 2
 money_factor = 10**money_decimals
 decimal_quantize = Decimal(f".{'0'*(money_decimals-1)}1")
 
 
 @register_extension_dtype
@@ -39,14 +38,22 @@
 
     def __hash__(self) -> int:
         # for python>=3.10, different nan objects have different hashes
         # we need to avoid that and thus use hash function with old behavior
         return object_hash(tuple(getattr(self, attr) for attr in self._metadata))
 
 
+def MoneySeries(
+    data=None, index=None, dtype: Dtype | None = None, **kwargs
+) -> pd.Series:
+    assert dtype is None, "Set dtype in MoneySeries not allowed"
+    dtype = MoneyDtype()
+    return pd.Series(data, index, dtype, **kwargs)
+
+
 class MoneyArray(ExtensionScalarOpsMixin, ExtensionArray):
     """A Pandas ExtensionArray of int64 for fixed decimal currency math
 
     Operator type rules
 
     MoneyArray ± (MoneyArray | Money) = MoneyArray
     MoneyArray * (int | float | Decimal | Iterable[int | float | Decimal]) = MoneyArray
@@ -258,11 +265,7 @@
 ops_overrides_patches = {
     f"__{op}__": getattr(MoneyArray, f"__{op}__") for op in ops_overrides
 }
 MoneyArray._add_arithmetic_ops()
 MoneyArray._add_comparison_ops()
 for attr, patch in ops_overrides_patches.items():
     setattr(MoneyArray, attr, patch)
-
-
-def money_series(data, **kwargs) -> pd.Series:
-    return pd.Series(data, dtype=MoneyDtype(), **kwargs)
```

### Comparing `pandas_money-0.2.2/pandas_money/tests/test_indexing.py` & `pandas_money-1.0.0a0/pandas_money/tests/test_indexing.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 @pytest.fixture
 def money_multidict(multi_tuples):
     return {idx: np.random.randint(1, 100) for idx in multi_tuples}
 
 
 @pytest.fixture
 def money_series(money_dict):
-    return pm.money_series(money_dict)
+    return pd.Series(money_dict, dtype="Money64")
 
 
 def test_loc(money_dict, money_series):
     assert money_series.loc["a"] == money_dict["a"]
     assert money_series.loc["b"] == money_dict["b"]
 
 
@@ -58,14 +58,7 @@
     index = list(money_dict.keys())
     s = pd.Series(index=index, dtype="Money64")
     assert all(list(pd.isna(s)))
     for i, idx in enumerate(index):
         s.iloc[i] = money_dict[idx]
     for i, idx in enumerate(index):
         assert s.iloc[i] == money_dict[idx]
-
-
-@pytest.mark.skip(reason="not supported yet")
-def test_no_data_isha(money_dict):
-    index = list(money_dict.keys())
-    s = pm.series(index=index)
-    assert all(list(pd.isna(s)))
```

### Comparing `pandas_money-0.2.2/pandas_money/tests/test_money_dtype.py` & `pandas_money-1.0.0a0/pandas_money/tests/test_money_dtype.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     m = pd.Series(money_scalar, dtype="Money64")
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == money_scalar
 
 
 def test_money_series_in_dataframe(money_scalar):
     df = pd.DataFrame(index=range(2))
-    df["m"] = pm.money_series(money_scalar)
+    df["m"] = pd.Series(money_scalar, dtype="Money64")
     assert isinstance(df["m"].dtype, pm.MoneyDtype)
     assert df["m"].iloc[0] == money_scalar
     assert pd.isna(df["m"].iloc[1])
 
 
 def test_decimal_scalar(decimal_scalar):
     m = pd.Series(decimal_scalar, dtype="Money64")
@@ -280,15 +280,15 @@
     # DeprecationWarning: Multiplying Money instances with floats is deprecated
     # so cast floats to Decimal
     assert m.iloc[0] == (money_list[0] / Decimal(float_scalar)).round(pm.money_decimals)
     assert m.iloc[1] == (money_list[1] / Decimal(float_scalar)).round(pm.money_decimals)
 
 
 def test_truediv_by_zero(money_list):
-    m1 = pm.money_series(money_list)
+    m1 = pd.Series(money_list, dtype="Money64")
     m = m1 / [0, 1]
     assert pd.isna(m.iloc[0])
     assert m.iloc[1] == money_list[1]
 
 
 def test_badscalar():
     with pytest.raises(InvalidOperation):
@@ -438,7 +438,24 @@
 
     lines = f.getvalue().splitlines()
     # adjust for slightly different formatting in GH Actions container
     assert re.match(r"\d\s+\$\s*3.14\s*", lines[0])
     assert re.match(r"\d\s+\$\s*2.72\s*", lines[1])
     assert re.match(r"\d\s+\<NA\>\s*", lines[2])
     assert "dtype: Money64" in lines[3]
+
+
+def test_no_data_isha(money_dict):
+    index = list(money_dict.keys())
+    s = pd.Series(index=index, dtype="Money64")
+    assert all(list(pd.isna(s)))
+
+
+def test_money_series(money_dict):
+    m1 = pd.Series(money_dict, dtype="Money64")
+    m2 = pm.MoneySeries(money_dict)
+    assert all(m1 == m2)
+
+
+def test_dtype_not_allowed():
+    with pytest.raises(AssertionError):
+        pm.MoneySeries(dtype=int)
```

### Comparing `pandas_money-0.2.2/pyproject.toml` & `pandas_money-1.0.0a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandas-money"
-version = "0.2.2"
+version = "1.0.0a0"
 description = "A Pandas ArrayExtension for handling currency with int64 performance"
 authors = ["Rod Morison <rmorison@users.noreply.github.com>"]
 repository = "https://github.com/rmorison/pandas-money"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandas_money"}]
```

### Comparing `pandas_money-0.2.2/PKG-INFO` & `pandas_money-1.0.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-money
-Version: 0.2.2
+Version: 1.0.0a0
 Summary: A Pandas ArrayExtension for handling currency with int64 performance
 Home-page: https://github.com/rmorison/pandas-money
 License: MIT
 Author: Rod Morison
 Author-email: rmorison@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

