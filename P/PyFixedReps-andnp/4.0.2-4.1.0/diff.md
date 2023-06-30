# Comparing `tmp/PyFixedReps-andnp-4.0.2.tar.gz` & `tmp/PyFixedReps-andnp-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFixedReps-andnp-4.0.2.tar", last modified: Sun Jun 18 04:47:36 2023, max compression
+gzip compressed data, was "PyFixedReps-andnp-4.1.0.tar", last modified: Fri Jun 30 16:38:21 2023, max compression
```

## Comparing `PyFixedReps-andnp-4.0.2.tar` & `PyFixedReps-andnp-4.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      181 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/PyFixedReps/BaseRepresentation.py
--rw-r--r--   0        0        0      751 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/PyFixedReps/RBF.py
--rw-r--r--   0        0        0     2869 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/PyFixedReps/TileCoder.py
--rw-r--r--   0        0        0      220 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/PyFixedReps/__init__.py
--rw-r--r--   0        0        0      477 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/PyFixedReps/_jit.py
--rw-r--r--   0        0        0     2931 2023-06-18 04:47:35.073283 PyFixedReps-andnp-4.0.2/README.md
--rw-r--r--   0        0        0      945 2023-06-18 04:47:35.081283 PyFixedReps-andnp-4.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/tests/__init__.py
--rw-r--r--   0        0        0      437 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/tests/test_RBF.py
--rw-r--r--   0        0        0     3907 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/tests/test_TileCoder.py
--rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 PyFixedReps-andnp-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0      181 2023-06-30 16:37:39.968398 PyFixedReps-andnp-4.1.0/PyFixedReps/BaseRepresentation.py
+-rw-r--r--   0        0        0      751 2023-06-30 16:37:39.968398 PyFixedReps-andnp-4.1.0/PyFixedReps/RBF.py
+-rw-r--r--   0        0        0     3154 2023-06-30 16:37:39.968398 PyFixedReps-andnp-4.1.0/PyFixedReps/TileCoder.py
+-rw-r--r--   0        0        0      220 2023-06-30 16:37:39.968398 PyFixedReps-andnp-4.1.0/PyFixedReps/__init__.py
+-rw-r--r--   0        0        0      477 2023-06-30 16:37:39.968398 PyFixedReps-andnp-4.1.0/PyFixedReps/_jit.py
+-rw-r--r--   0        0        0     2931 2023-06-30 16:38:18.770405 PyFixedReps-andnp-4.1.0/README.md
+-rw-r--r--   0        0        0      945 2023-06-30 16:38:18.782406 PyFixedReps-andnp-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 16:37:39.968398 PyFixedReps-andnp-4.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      437 2023-06-30 16:37:39.968398 PyFixedReps-andnp-4.1.0/tests/test_RBF.py
+-rw-r--r--   0        0        0     3907 2023-06-30 16:37:39.968398 PyFixedReps-andnp-4.1.0/tests/test_TileCoder.py
+-rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 PyFixedReps-andnp-4.1.0/PKG-INFO
```

### Comparing `PyFixedReps-andnp-4.0.2/PyFixedReps/RBF.py` & `PyFixedReps-andnp-4.1.0/PyFixedReps/RBF.py`

 * *Files identical despite different names*

### Comparing `PyFixedReps-andnp-4.0.2/PyFixedReps/TileCoder.py` & `PyFixedReps-andnp-4.1.0/PyFixedReps/TileCoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,28 +13,29 @@
     tiles: int | Sequence[int]
     tilings: int
     dims: int
 
     offset: str = 'cascade'
     scale_output: bool = True
     input_ranges: Optional[Sequence[Range | None]] = None
-    bound: str = 'wrap'
+    bound: str | Sequence[str] = 'clip'
 
 class TileCoder(BaseRepresentation):
     def __init__(self, config: TileCoderConfig, rng: Optional[RandomState] = None):
         self.rng = rng
         self._c = c = config
 
         ranges: Sequence[Range | None] = [None] * c.dims
         if c.input_ranges is not None:
             assert len(c.input_ranges) == c.dims
             ranges = c.input_ranges
 
         self._tiles: Any = _normalize_tiles(c.tiles, c.dims)
         self._input_ranges = _normalize_scalars(ranges)
+        self._bound_strats = _normalize_bounds(c.bound, c.dims)
         self._tiling_offsets: Array = np.array([ self._build_offset(ntl) for ntl in range(c.tilings) ])
         self._total_tiles = int(c.tilings * self._tiles.prod())
 
     # construct tiling offsets
     # defaults to evenly spaced tilings
     def _build_offset(self, n: int):
         if self._c.offset == 'random':
@@ -50,15 +51,15 @@
             i = n - (self._c.tilings / 2)
             return np.ones(self._c.dims) * i * (tile_length / self._c.tilings)
 
         raise Exception('Unknown offset type')
 
     def get_indices(self, pos: npt.ArrayLike):
         pos_ = np.asarray(pos, dtype=np.float64)
-        return get_tc_indices(self._c.dims, self._tiles, self._c.tilings, self._input_ranges, self._tiling_offsets, pos_)
+        return get_tc_indices(self._c.dims, self._tiles, self._c.tilings, self._input_ranges, self._tiling_offsets, self._bound_strats, pos_)
 
     def features(self):
         return self._total_tiles
 
     def encode(self, s: npt.ArrayLike):
         indices = self.get_indices(s)
         vec = np.zeros(self.features())
@@ -73,14 +74,20 @@
 
 def _normalize_tiles(tiles: int | Iterable[int], dims: int) -> np.ndarray:
     if isinstance(tiles, int):
         tiles = [tiles for _ in range(dims)]
 
     return np.fromiter(tiles, dtype=np.uint32, count=dims)
 
+def _normalize_bounds(bound_strat: str | Sequence[str], dims: int) -> List[str]:
+    if isinstance(bound_strat, str):
+        return [bound_strat] * dims
+
+    return list(bound_strat)
+
 def _normalize_scalars(sc: Sequence[Tuple[float, float] | None]):
     out: List[Tuple[float, float]] = []
     for r in sc:
         if r is None:
             out.append((0., 1.))
 
         else:
```

### Comparing `PyFixedReps-andnp-4.0.2/README.md` & `PyFixedReps-andnp-4.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # PyFixedReps
 Short for: Python Fixed Representations.
 This is a collection of unit tested implementations of common fixed representations commonly used with linear (in features) RL systems.
 
 ## Installing
 Can be installed using `pip` by including this in your `requirements.txt`:
 ```
-pip install PyFixedReps-andnp==4.0.2
+pip install PyFixedReps-andnp==4.1.0
 ```
 I highly recommend specifying the version number when installing in order to ensure reproducibility of experiments.
 This library is fairly stable, so does not change often and there is little risk of missing an important change.
 
 ## Tile-coder
 ```python
 from PyFixedReps import TileCoder
```

### Comparing `PyFixedReps-andnp-4.0.2/pyproject.toml` & `PyFixedReps-andnp-4.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "4.0.2"
+version = "4.1.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
     "README.md",
 ]
 
 [tool.pdm]
@@ -16,31 +16,31 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "mypy>=0.991",
     "flake8>=6.0.0",
     "commitizen>=2.39.1",
     "pre-commit>=2.21.0",
     "build>=0.10.0",
-    "twine>=4.0.2",
+    "twine>=4.1.0",
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "PyFixedReps-andnp"
-version = "4.0.2"
+version = "4.1.0"
 description = ""
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numpy>=1.23.5",
     "numba>=0.56.4",
-    "tile-coder-rs==0.3.1",
+    "tile-coder-rs>=0.4.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `PyFixedReps-andnp-4.0.2/tests/test_TileCoder.py` & `PyFixedReps-andnp-4.1.0/tests/test_TileCoder.py`

 * *Files identical despite different names*

### Comparing `PyFixedReps-andnp-4.0.2/PKG-INFO` & `PyFixedReps-andnp-4.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: PyFixedReps-andnp
-Version: 4.0.2
+Version: 4.1.0
 License: MIT
 Author-email: Andy Patterson <andnpatterson@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # PyFixedReps
 Short for: Python Fixed Representations.
 This is a collection of unit tested implementations of common fixed representations commonly used with linear (in features) RL systems.
 
 ## Installing
 Can be installed using `pip` by including this in your `requirements.txt`:
 ```
-pip install PyFixedReps-andnp==4.0.2
+pip install PyFixedReps-andnp==4.1.0
 ```
 I highly recommend specifying the version number when installing in order to ensure reproducibility of experiments.
 This library is fairly stable, so does not change often and there is little risk of missing an important change.
 
 ## Tile-coder
 ```python
 from PyFixedReps import TileCoder
```

