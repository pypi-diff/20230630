# Comparing `tmp/ice_simplex_assimilate-0.1.1.tar.gz` & `tmp/ice_simplex_assimilate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ice_simplex_assimilate-0.1.1.tar", max compression
+gzip compressed data, was "ice_simplex_assimilate-0.1.2.tar", max compression
```

## Comparing `ice_simplex_assimilate-0.1.1.tar` & `ice_simplex_assimilate-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-14 19:27:28.966885 ice_simplex_assimilate-0.1.1/README.md
--rw-r--r--   0        0        0       46 2023-06-14 19:41:47.179033 ice_simplex_assimilate-0.1.1/ice_simplex_assimilate/__init__.py
--rw-r--r--   0        0        0     3430 2023-06-14 18:46:53.104387 ice_simplex_assimilate-0.1.1/ice_simplex_assimilate/deltize.py
--rw-r--r--   0        0        0      298 2023-06-14 18:30:25.741811 ice_simplex_assimilate-0.1.1/ice_simplex_assimilate/io.py
--rw-r--r--   0        0        0     7655 2023-06-10 12:08:05.805803 ice_simplex_assimilate-0.1.1/ice_simplex_assimilate/visualize.py
--rw-r--r--   0        0        0      550 2023-06-30 07:53:09.305475 ice_simplex_assimilate-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 ice_simplex_assimilate-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-14 19:27:28.966885 ice_simplex_assimilate-0.1.2/README.md
+-rw-r--r--   0        0        0       46 2023-06-14 19:41:47.179033 ice_simplex_assimilate-0.1.2/ice_simplex_assimilate/__init__.py
+-rw-r--r--   0        0        0     3632 2023-06-30 12:51:51.012910 ice_simplex_assimilate-0.1.2/ice_simplex_assimilate/deltize.py
+-rw-r--r--   0        0        0      298 2023-06-14 18:30:25.741811 ice_simplex_assimilate-0.1.2/ice_simplex_assimilate/io.py
+-rw-r--r--   0        0        0     7655 2023-06-10 12:08:05.805803 ice_simplex_assimilate-0.1.2/ice_simplex_assimilate/visualize.py
+-rw-r--r--   0        0        0      550 2023-06-30 12:55:02.808346 ice_simplex_assimilate-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 ice_simplex_assimilate-0.1.2/PKG-INFO
```

### Comparing `ice_simplex_assimilate-0.1.1/ice_simplex_assimilate/deltize.py` & `ice_simplex_assimilate-0.1.2/ice_simplex_assimilate/deltize.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,9 +79,12 @@
     v = h_bnd[:-1] * l + h_bnd[1:] * r
     return RawSample(area=np.array(a), volume=np.array(v), snow=np.zeros_like(a))
 
 
 def post_process_ensemble(ensemble: NDArray[np.float64], h_bnd: HeightBounds) -> List[RawSample]:
     raw_samples = []
     for sample in ensemble:
+        print(sample)
         raw_samples.append(post_process_sample(sample, h_bnd=h_bnd))
     return raw_samples
+def raw_ensemble_to_matrices(raw_ensemble: List[RawSample]) -> NDArray[np.float64]:
+    return np.array([s.area for s in raw_ensemble]), np.array([s.volume for s in raw_ensemble])
```

### Comparing `ice_simplex_assimilate-0.1.1/ice_simplex_assimilate/visualize.py` & `ice_simplex_assimilate-0.1.2/ice_simplex_assimilate/visualize.py`

 * *Files identical despite different names*

### Comparing `ice_simplex_assimilate-0.1.1/pyproject.toml` & `ice_simplex_assimilate-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ice-simplex-assimilate"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Oscar Laird <olaird25@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ice_simplex_assimilate"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

