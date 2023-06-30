# Comparing `tmp/adpbulk-0.1.3.tar.gz` & `tmp/adpbulk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adpbulk-0.1.3.tar", last modified: Thu Apr 28 15:37:19 2022, max compression
+gzip compressed data, was "adpbulk-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `adpbulk-0.1.3.tar` & `adpbulk-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      971 2022-04-28 15:15:08.678470 adpbulk-0.1.3/.github/workflows/main.yml
--rw-r--r--   0        0        0     1799 2022-04-28 15:15:08.678470 adpbulk-0.1.3/.gitignore
--rw-r--r--   0        0        0     1080 2022-04-28 15:15:08.678470 adpbulk-0.1.3/LICENSE
--rw-r--r--   0        0        0     5434 2022-04-28 15:15:08.678470 adpbulk-0.1.3/README.md
--rw-r--r--   0        0        0       94 2022-04-28 15:31:15.185143 adpbulk-0.1.3/adpbulk/__init__.py
--rw-r--r--   0        0        0     8399 2022-04-28 15:30:24.375142 adpbulk-0.1.3/adpbulk/adpbulk.py
--rw-r--r--   0        0        0      520 2022-04-28 15:31:05.145142 adpbulk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4839 2022-04-28 15:30:54.381809 adpbulk-0.1.3/tests/test_adpbulk.py
--rw-r--r--   0        0        0     5865 1970-01-01 00:00:00.000000 adpbulk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      971 2023-06-29 23:51:02.541824 adpbulk-0.1.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1799 2023-06-29 23:51:02.541824 adpbulk-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1080 2023-06-29 23:51:02.541824 adpbulk-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5434 2023-06-29 23:51:02.541824 adpbulk-0.1.4/README.md
+-rw-r--r--   0        0        0       94 2023-06-30 01:42:53.090919 adpbulk-0.1.4/adpbulk/__init__.py
+-rw-r--r--   0        0        0     9251 2023-06-30 01:42:53.090919 adpbulk-0.1.4/adpbulk/adpbulk.py
+-rw-r--r--   0        0        0      520 2023-06-29 23:51:02.541824 adpbulk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5795 2023-06-30 01:42:53.090919 adpbulk-0.1.4/tests/test_adpbulk.py
+-rw-r--r--   0        0        0     5865 1970-01-01 00:00:00.000000 adpbulk-0.1.4/PKG-INFO
```

### Comparing `adpbulk-0.1.3/.github/workflows/main.yml` & `adpbulk-0.1.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `adpbulk-0.1.3/.gitignore` & `adpbulk-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `adpbulk-0.1.3/LICENSE` & `adpbulk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adpbulk-0.1.3/README.md` & `adpbulk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `adpbulk-0.1.3/adpbulk/adpbulk.py` & `adpbulk-0.1.4/adpbulk/adpbulk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 Class for Pseudobulking
 """
-from typing import Union, List
+from typing import Optional, Union, List
 import itertools as it
 import numpy as np
 import pandas as pd
 import anndata as ad
 from tqdm import tqdm
 
 
 class ADPBulk:
     def __init__(
-            self,
-            adat: ad.AnnData,
-            groupby: Union[List[str], str],
-            method: str = "sum",
-            name_delim: str = "-",
-            group_delim: str = ".",
-            use_raw: bool = False):
+        self,
+        adat: ad.AnnData,
+        groupby: Union[List[str], str],
+        method: str = "sum",
+        name_delim: str = "-",
+        group_delim: str = ".",
+        use_raw: bool = False,
+        layer: Optional[str] = None,
+    ):
         """
         Class of Pseudo-Bulking `AnnData` objects based on categorical variables
         found in the `.obs` attribute
 
         inputs:
             adat: anndata.AnnData
                 The `AnnData` object to process
@@ -34,27 +36,27 @@
                 The delimiter to use when grouping multiple categories together.
                 example: 'cat1{delim}cat2'
             group_delim: str
                 The delimiter to use for adding the value to its category.
                 example: 'cat{delim}value'
             use_raw: bool
                 Whether to use the `.raw` attribute on the `AnnData` object
+            layer: Optional[str]
+                The layer to use for the aggregation. If None, will use `.X`
         """
 
-        self.agg_methods = {
-            "sum": np.sum,
-            "mean": np.mean,
-            "median": np.median}
+        self.agg_methods = {"sum": np.sum, "mean": np.mean, "median": np.median}
 
         self.adat = adat
         self.groupby = groupby
         self.method = method
         self.name_delim = name_delim
         self.group_delim = group_delim
         self.use_raw = use_raw
+        self.layer = layer
 
         self.group_idx = dict()
         self.groupings = list()
         self.grouping_masks = dict()
 
         self.meta = pd.DataFrame([])
         self.matrix = pd.DataFrame([])
@@ -69,14 +71,15 @@
         """
         validates that the input is as expected
         """
         self._validate_anndata()
         self._validate_groups()
         self._validate_method()
         self._validate_raw()
+        self._validate_layer()
 
     def _validate_anndata(self):
         """
         validates that the anndata object is as expected
         """
         if self.adat.X is None:
             raise AttributeError("Provided Matrix is None")
@@ -109,35 +112,52 @@
 
     def _validate_method(self):
         """
         confirms that the method is known
         """
         if self.method not in self.agg_methods.keys():
             raise ValueError(
-                f"Provided method {self.method} not in known methods {''.join(self.agg_methods)}")
+                f"Provided method {self.method} not in known methods {''.join(self.agg_methods)}"
+            )
+
+    def _validate_layer(self):
+        """
+        confirms that the layer is known and of expected size
+        """
+        if self.layer is None:
+            return
+        if self.layer not in self.adat.layers.keys():
+            raise KeyError(
+                f"Provided layer {self.layer} not in known layers {''.join(self.adat.layers)}"
+            )
+        if self.adat.layers[self.layer].shape != self.adat.X.shape:
+            raise ValueError(
+                f"Provided layer {self.layer} is not the same shape as the internal counts matrix"
+            )
 
     def _validate_raw(self):
         """
         if the `use_raw` flag is provided will confirm that
         the raw field is present
         """
         if self.use_raw and self.adat.raw is None:
             raise AttributeError(
-                "use_raw provided, but no raw field is found in AnnData")
-
+                "use_raw provided, but no raw field is found in AnnData"
+            )
 
     def _fit_indices(self):
         """
         determines the indices for each of the provided groups
         """
         for group in self.groupby:
             unique_values = np.unique(self.adat.obs[group].values)
             self.group_idx[group] = {
                 uv: set(np.flatnonzero(self.adat.obs[group].values == uv))
-                    for uv in tqdm(unique_values, desc=f"fitting indices: {group}")}
+                for uv in tqdm(unique_values, desc=f"fitting indices: {group}")
+            }
 
     def _get_mask(self, pairs: tuple) -> np.ndarray:
         """
         retrieve the indices for the provided values from their respective groups
         calculates the global intersection between the sets
         """
         group_indices = []
@@ -146,24 +166,30 @@
         mask = set.intersection(*group_indices)
         return np.array(list(mask))
 
     def _get_name(self, pairs: tuple) -> str:
         """
         create a name for the provided values based on their respective groups
         """
-        name = self.name_delim.join([
-                f"{self.groupby[i]}{self.group_delim}{pairs[i]}" for i in range(len(pairs))])
+        name = self.name_delim.join(
+            [
+                f"{self.groupby[i]}{self.group_delim}{pairs[i]}"
+                for i in range(len(pairs))
+            ]
+        )
         return name
 
     def _get_agg(self, mask: np.ndarray) -> np.ndarray:
         """
         runs the aggregation function with the provided sample mask
         """
         if self.use_raw:
             mat = self.adat.raw.X[mask]
+        elif self.layer is not None:
+            mat = self.adat.layers[self.layer][mask]
         else:
             mat = self.adat.X[mask]
         return self.agg_methods[self.method](mat, axis=0)
 
     def _get_var(self) -> np.ndarray:
         """
         return the var names using the given scheme (normal/raw)
@@ -173,17 +199,15 @@
         else:
             return self.adat.var.index.values
 
     def _prepare_meta(self, pairs: tuple) -> dict:
         """
         defines the meta values for the pairs
         """
-        values = {
-            self.groupby[idx]: pairs[idx] for idx in np.arange(len(self.groupby))
-            }
+        values = {self.groupby[idx]: pairs[idx] for idx in np.arange(len(self.groupby))}
         values["SampleName"] = self._get_name(pairs)
         return values
 
     def _build_groupings(self):
         """
         generate the grouping iterable
         """
@@ -230,22 +254,21 @@
 
         matrix = []
         for pairs in tqdm(self.groupings, desc="Aggregating Samples"):
             if not isinstance(pairs, tuple):
                 pairs = tuple([pairs])
             if pairs in self.grouping_masks:
                 matrix.append(self._get_agg(self.grouping_masks[pairs]))
-        
+
         # stack all observations into single matrix
         matrix = np.vstack(matrix)
 
         self.matrix = pd.DataFrame(
-            matrix,
-            index=self.meta.SampleName.values,
-            columns=self._get_var())
+            matrix, index=self.meta.SampleName.values, columns=self._get_var()
+        )
 
         self._istransform = True
         return self.matrix
 
     def fit_transform(self):
         """
         firs the indices and performs the aggregation based on those indices
```

### Comparing `adpbulk-0.1.3/pyproject.toml` & `adpbulk-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adpbulk-0.1.3/tests/test_adpbulk.py` & `adpbulk-0.1.4/tests/test_adpbulk.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,42 +9,42 @@
 from adpbulk import ADPBulk
 
 SIZE_N = 100
 SIZE_M = 100
 
 np.random.seed(42)
 
+
 def build_adat() -> ad.AnnData:
     """
     creates an anndata for testing
     """
     mat = np.random.random((SIZE_N, SIZE_M))
     raw = np.random.randint(0, 1000, (SIZE_N, SIZE_M))
-    obs = pd.DataFrame({
-        "cell": [f"b{idx}" for idx in np.arange(SIZE_N)],
-        "cA": np.random.choice(np.random.choice(5)+1, SIZE_N),
-        "cB": np.random.choice(np.random.choice(5)+1, SIZE_N),
-        "cC": np.random.choice(np.random.choice(5)+1, SIZE_N),
-        "cD": np.random.choice(np.random.choice(5)+1, SIZE_N),
-        }).set_index("cell")
-    var = pd.DataFrame({
-        "symbol": [f"g{idx}" for idx in np.arange(SIZE_M)],
-        "cA": np.random.choice(np.random.choice(5)+1, SIZE_M),
-        "cB": np.random.choice(np.random.choice(5)+1, SIZE_M),
-        "cC": np.random.choice(np.random.choice(5)+1, SIZE_M),
-        "cD": np.random.choice(np.random.choice(5)+1, SIZE_M),
-        }).set_index("symbol")
-    adat = ad.AnnData(
-            X=mat,
-            obs=obs,
-            var=var)
-    adat_raw = ad.AnnData(
-            X=raw,
-            obs=obs,
-            var=var)
+    obs = pd.DataFrame(
+        {
+            "cell": [f"b{idx}" for idx in np.arange(SIZE_N)],
+            "cA": np.random.choice(np.random.choice(5) + 1, SIZE_N),
+            "cB": np.random.choice(np.random.choice(5) + 1, SIZE_N),
+            "cC": np.random.choice(np.random.choice(5) + 1, SIZE_N),
+            "cD": np.random.choice(np.random.choice(5) + 1, SIZE_N),
+        }
+    ).set_index("cell")
+    var = pd.DataFrame(
+        {
+            "symbol": [f"g{idx}" for idx in np.arange(SIZE_M)],
+            "cA": np.random.choice(np.random.choice(5) + 1, SIZE_M),
+            "cB": np.random.choice(np.random.choice(5) + 1, SIZE_M),
+            "cC": np.random.choice(np.random.choice(5) + 1, SIZE_M),
+            "cD": np.random.choice(np.random.choice(5) + 1, SIZE_M),
+        }
+    ).set_index("symbol")
+    adat = ad.AnnData(X=mat, obs=obs, var=var)
+    adat_raw = ad.AnnData(X=raw, obs=obs, var=var)
+    adat.layers["test"] = mat * 10
     adat.raw = adat_raw
     return adat
 
 
 def test_init():
     """
     tests whether the ADPBulk object can be instantiated correctly
@@ -73,14 +73,51 @@
 
     # tests multiple group conditions
     _ = ADPBulk(adat, groupby=["cA", "cD"], use_raw=True)
 
     assert True
 
 
+def test_init_layer():
+    """
+    tests whether the ADPBulk object can be instantiated correctly
+    """
+    adat = build_adat()
+
+    # tests singular group conditions
+    for group in adat.obs.columns:
+        _ = ADPBulk(adat, groupby=group, layer="test")
+
+    # tests multiple group conditions
+    _ = ADPBulk(adat, groupby=["cA", "cD"], layer="test")
+
+    assert True
+
+
+def test_init_layer_missing():
+    """
+    tests whether the ADPBulk object can be instantiated correctly
+    """
+    adat = build_adat()
+
+    # tests singular group conditions
+    for group in adat.obs.columns:
+        with pytest.raises(KeyError):
+            _ = ADPBulk(adat, groupby=group, layer="missing_layer")
+            assert False
+        assert True
+
+    # tests multiple group conditions
+    with pytest.raises(KeyError):
+        _ = ADPBulk(adat, groupby=["cA", "cD"], layer="missing_layer")
+        assert False
+
+    assert True
+
+
 def test_adjusted_raw():
     """
     tests whether the ADPBulk object can be run correctly
     after the original adat changes but the raw does not
     """
     adat = build_adat()
     mask = np.random.random(SIZE_M) < 0.3
@@ -111,61 +148,65 @@
         _ = ADPBulk(adat, groupby="foobar")
     with pytest.raises(ValueError):
         _ = ADPBulk(adat, groupby=["foobar", "barbaz"])
     with pytest.raises(ValueError):
         _ = ADPBulk(adat, groupby=["foobar", "cA"])
     assert True
 
+
 def test_init_missing_method():
     """
     tests whether the ADPBulk object be init incorrectly
     with missing method
     """
     adat = build_adat()
     with pytest.raises(ValueError):
         _ = ADPBulk(adat, groupby="cA", method="not_a_method")
     assert True
 
+
 def test_fit_indices():
     """
     tests whether the indices are properly fit
     """
     adat = build_adat()
     adpb = ADPBulk(adat, "cA")
     adpb.fit()
 
     assert "cA" in adpb.group_idx.keys()
     for g in adat.obs["cA"].unique():
         assert g in adpb.group_idx["cA"].keys()
-        assert len(adpb.group_idx["cA"][g]) ==\
-                np.sum(adat.obs["cA"] == g)
+        assert len(adpb.group_idx["cA"][g]) == np.sum(adat.obs["cA"] == g)
+
 
 def test_transform_singular():
     """
     tests whether the transformation can be performed
     """
     adat = build_adat()
     for condition in adat.obs.columns.values:
         for use_raw in [True, False]:
             for method in ["mean", "median", "sum"]:
                 adpb = ADPBulk(adat, condition, method=method, use_raw=use_raw)
                 matrix = adpb.fit_transform()
                 assert isinstance(matrix, pd.DataFrame)
 
+
 def test_transform_combination():
     """
     tests whether the transformation can be performed
     """
     adat = build_adat()
     for use_raw in [True, False]:
         for method in ["mean", "median", "sum"]:
             adpb = ADPBulk(adat, ["cA", "cB"], method=method, use_raw=use_raw)
             matrix = adpb.fit_transform()
             assert isinstance(matrix, pd.DataFrame)
 
+
 def test_order_of_operations():
     """
     test whether the order of observations are properly organized
     """
     adat = build_adat()
     adpb = ADPBulk(adat, "cA")
     with pytest.raises(AttributeError):
```

### Comparing `adpbulk-0.1.3/PKG-INFO` & `adpbulk-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adpbulk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pseudo-Bulking Single-Cell RNA-seq
 Author-email: Noam Teyssier <noam.teyssier@ucsf.edu>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: anndata>=0.7.4
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: pandas>=0.21
```

