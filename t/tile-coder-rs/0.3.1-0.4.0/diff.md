# Comparing `tmp/tile_coder_rs-0.3.1.tar.gz` & `tmp/tile_coder_rs-0.4.0.tar.gz`

## Comparing `tile_coder_rs-0.3.1.tar` & `tile_coder_rs-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      171 1970-01-01 00:00:00.000000 tile_coder_rs-0.3.1/Cargo.toml
--rw-r--r--   0     1001      123     2789 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123       35 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/.gitignore
--rw-r--r--   0     1001      123       10 2023-06-18 04:34:50.000000 tile_coder_rs-0.3.1/dist/tile_coder_rs-0.3.1.tar.gz
--rw-r--r--   0     1001      123      235 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/pyproject.toml
--rw-r--r--   0     1001      123       56 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/requirements.txt
--rw-r--r--   0     1001      123     1760 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/src/lib.rs
--rw-r--r--   0     1001      123     3469 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/src/tc.rs
--rw-r--r--   0     1001      123      747 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/tests/perf.py
--rw-r--r--   0     1001      123     2590 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/tests/tc.py
--rw-r--r--   0     1001      123      473 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/tests/test.py
--rw-r--r--   0     1001      123       55 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/tile_coder_rs/__init__.py
--rw-r--r--   0     1001      123        0 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/tile_coder_rs/py.typed
--rw-r--r--   0     1001      123      187 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/tile_coder_rs/tile_coder_rs.pyi
--rw-r--r--   0     1001      123     9589 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/Cargo.lock
--rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 tile_coder_rs-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      171 1970-01-01 00:00:00.000000 tile_coder_rs-0.4.0/Cargo.toml
+-rw-r--r--   0     1001      123     2789 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123       35 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/.gitignore
+-rw-r--r--   0     1001      123       10 2023-06-30 16:25:04.000000 tile_coder_rs-0.4.0/dist/tile_coder_rs-0.4.0.tar.gz
+-rw-r--r--   0     1001      123      235 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/pyproject.toml
+-rw-r--r--   0     1001      123       56 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/requirements.txt
+-rw-r--r--   0     1001      123     1964 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/src/lib.rs
+-rw-r--r--   0     1001      123     4347 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/src/tc.rs
+-rw-r--r--   0     1001      123      747 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/tests/perf.py
+-rw-r--r--   0     1001      123     2590 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/tests/tc.py
+-rw-r--r--   0     1001      123      473 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/tests/test.py
+-rw-r--r--   0     1001      123       55 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/tile_coder_rs/__init__.py
+-rw-r--r--   0     1001      123        0 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/tile_coder_rs/py.typed
+-rw-r--r--   0     1001      123      240 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/tile_coder_rs/tile_coder_rs.pyi
+-rw-r--r--   0     1001      123     9589 2023-06-30 16:24:58.000000 tile_coder_rs-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 tile_coder_rs-0.4.0/PKG-INFO
```

### Comparing `tile_coder_rs-0.3.1/.github/workflows/CI.yml` & `tile_coder_rs-0.4.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `tile_coder_rs-0.3.1/src/lib.rs` & `tile_coder_rs-0.4.0/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -3,28 +3,26 @@
 use numpy::ndarray::{ArrayView1, ArrayView2, Array1, Zip};
 use numpy::{IntoPyArray, PyReadonlyArray2};
 use numpy::{PyArray1,PyReadonlyArray1};
 use pyo3::prelude::*;
 
 mod tc;
 
-enum BoundStrat {
+pub enum BoundStrat {
     Clip,
     Wrap,
-    Scale,
 }
 
 impl FromStr for BoundStrat {
     type Err = ();
 
     fn from_str(input: &str) -> Result<BoundStrat, Self::Err> {
         match input {
             "clip" => Ok(BoundStrat::Clip),
             "wrap" => Ok(BoundStrat::Wrap),
-            "scale" => Ok(BoundStrat::Scale),
             _ => Err(()),
         }
     }
 }
 
 fn minmax_scale(pos: f64, bound: ArrayView1<f64>) -> f64 {
     (pos - bound[0]) / (bound[1] - bound[0])
@@ -51,21 +49,27 @@
     fn test_py<'py>(
         py: Python<'py>,
         dims: u32,
         tiles: PyReadonlyArray1<u32>,
         tilings: u32,
         bounds: PyReadonlyArray2<f64>,
         offsets: PyReadonlyArray2<f64>,
+        bound_strats: Vec<&str>,
         pos: PyReadonlyArray1<f64>,
     ) -> &'py PyArray1<u32> {
         let offsets = offsets.as_array();
         let pos = pos.as_array();
         let bounds = bounds.as_array();
         let tiles = tiles.as_array();
+        let bound_strats: Vec<BoundStrat> =
+            bound_strats
+                .iter()
+                .map(|v| BoundStrat::from_str(&v).expect("Unknown bounding strategy!"))
+                .collect();
 
         let pos = apply_bounds(pos, bounds);
-        let res = py.allow_threads(|| tc::get_tc_indices(dims, &tiles, tilings, &offsets, &pos));
+        let res = py.allow_threads(|| tc::get_tc_indices(dims, &tiles, tilings, &offsets, &bound_strats, &pos));
         res.into_pyarray(py)
     }
 
     Ok(())
 }
```

### Comparing `tile_coder_rs-0.3.1/tests/perf.py` & `tile_coder_rs-0.4.0/tests/perf.py`

 * *Files identical despite different names*

### Comparing `tile_coder_rs-0.3.1/tests/tc.py` & `tile_coder_rs-0.4.0/tests/tc.py`

 * *Files identical despite different names*

### Comparing `tile_coder_rs-0.3.1/Cargo.lock` & `tile_coder_rs-0.4.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tile-coder-rs"
-version = "0.3.1"
+version = "0.4.0"
 dependencies = [
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "unicode-ident"
```

