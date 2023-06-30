# Comparing `tmp/simplex_assimilate-0.1.0.tar.gz` & `tmp/simplex_assimilate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplex_assimilate-0.1.0.tar", max compression
+gzip compressed data, was "simplex_assimilate-0.1.1.tar", max compression
```

## Comparing `simplex_assimilate-0.1.0.tar` & `simplex_assimilate-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      766 2023-06-14 17:24:55.722986 simplex_assimilate-0.1.0/README.md
--rw-r--r--   0        0        0      639 2023-06-14 17:37:54.131152 simplex_assimilate-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-14 14:47:15.034463 simplex_assimilate-0.1.0/simplex_assimilate/__init__.py
--rw-r--r--   0        0        0     9602 2023-06-14 16:28:48.062321 simplex_assimilate-0.1.0/simplex_assimilate/cdf_transport.py
--rw-r--r--   0        0        0     4196 2023-06-14 17:08:51.038465 simplex_assimilate-0.1.0/simplex_assimilate/dirichlet.py
--rw-r--r--   0        0        0     1407 2023-06-14 16:59:00.153456 simplex_assimilate-0.1.0/simplex_assimilate/quantize.py
--rw-r--r--   0        0        0     1241 1970-01-01 00:00:00.000000 simplex_assimilate-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-06-14 18:19:15.322493 simplex_assimilate-0.1.1/README.md
+-rw-r--r--   0        0        0      660 2023-06-30 07:53:44.002764 simplex_assimilate-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-06-14 19:41:47.172366 simplex_assimilate-0.1.1/simplex_assimilate/__init__.py
+-rw-r--r--   0        0        0    10063 2023-06-14 20:28:19.516095 simplex_assimilate-0.1.1/simplex_assimilate/cdf.py
+-rw-r--r--   0        0        0     4196 2023-06-14 17:08:51.038465 simplex_assimilate-0.1.1/simplex_assimilate/dirichlet.py
+-rw-r--r--   0        0        0     1407 2023-06-14 16:59:00.153456 simplex_assimilate-0.1.1/simplex_assimilate/quantize.py
+-rw-r--r--   0        0        0     1153 2023-06-14 19:49:43.938700 simplex_assimilate-0.1.1/simplex_assimilate/transport.py
+-rw-r--r--   0        0        0     1367 1970-01-01 00:00:00.000000 simplex_assimilate-0.1.1/PKG-INFO
```

### Comparing `simplex_assimilate-0.1.0/README.md` & `simplex_assimilate-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # Simplex Assimilate: Data assimilation on the simplex
 
+![Coverage](tests/coverage.svg)
+
 ## Installation 
 ```bash
 pip install simplex-assimilate
 ```
 
 ## File Structure
  - `simplex_assimilate/` source code
- - `simplex_assimilate/cdf_transport.py` Optimal transport of samples on the simplex.
+ - `simplex_assimilate/cdf.py` Conditional distribution functions for the mixed dirichlet prior.
  - `simplex_assimilate/quantize.py` Convert floating point samples to fixed point representation.
  - `simplex_assimilate/dirichlet.py` Model samples on the simplex with a mixture of Dirichlet distributions. Fit parameters by maximum likelihood.
+ - `simplex_assimilate/transport.py` Optimal transport of samples on the simplex.
  - `tests/` unit tests
  - `coverage_report/` coverage reports
 
 ## See Also
   - [Ice Simplex Assimilate Repository](https://github.com/oscarlaird/ice_simplex_assimilate)
     - Represent an ice thickness distribution as a point on the simplex and perform transport.
```

### Comparing `simplex_assimilate-0.1.0/pyproject.toml` & `simplex_assimilate-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simplex-assimilate"
-version = "0.1.0"
+version = "0.1.1"
 description = "Perform Data Assimilation on the Simplex. Models an ensemble as a mixture of Dirichlet distributions."
 authors = ["Oscar Laird <olaird25@gmail.com>"]
 readme = "README.md"
 packages = [{include = "simplex_assimilate"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
@@ -15,11 +15,12 @@
 hypothesis = "^6.75.6"
 matplotlib = "^3.7.1"
 fire = "^0.5.0"
 jupyter = "^1.0.0"
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 mypy = "^1.3.0"
+anybadge = "^1.14.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `simplex_assimilate-0.1.0/simplex_assimilate/cdf_transport.py` & `simplex_assimilate-0.1.1/simplex_assimilate/cdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     assert j < J, 'pre_samples must have fewer components than alpha'
     # calculate likelihood for each sample against each class
     out = np.zeros((N, K))
     for i in range(N):
         for k in range(K):
             out[i, k] = likelihood(alpha[k], pre_samples[i])
     # check outputs
-    assert out.any(axis=1).all(), 'every sample must have at least one compatible class'
-    assert out.shape == (N, K)
+    # assert out.any(axis=1).all(), 'every sample must have at least one compatible class'
+    # assert out.shape == (N, K)
     return out
 
 
 def cdf(x_j, prior: dirichlet.MixedDirichlet, pre_samples: NDArray[np.uint32]) -> NDArray[np.float64]:
     #   There are three kinds of classes:
     #     lower_classes: x_j = 0    (delta distribution)
     #     middle_classes: 0 < x_j < (1 - Σx_(<j))   (beta distribution)
@@ -64,22 +64,25 @@
     upper_classes = (prior.full_alpha[:, j] > 0) & (~ prior.full_alpha[:, j + 1:].any(axis=1))
     middle_classes = ~ (lower_classes | upper_classes)
     # every compatible class must belong to exactly one of the three categories
     assert np.all(lower_classes + upper_classes + middle_classes == 1)
     # CALCULATE THE CDFs of the MIXTURE MIDDLE CLASSES
     # x_j/(1-Σx_(<j)) | x_(<j) ~ Beta(alpha_j, sum(alpha_(j+1:)))
     upper = ONE - pre_samples.sum(axis=1)
-    mixture_cdfs = np.empty((N, prior.K), dtype=np.float64)
+    mixture_cdfs = np.zeros((N, prior.K), dtype=np.float64)
     mixture_cdfs[:, lower_classes] = 1.
     mixture_cdfs[:, upper_classes] = (x_j >= upper)[:, None]
     if middle_classes.any():
         middle_alphas = prior.full_alpha[middle_classes]
         betas = np.column_stack((middle_alphas[:, j], middle_alphas[:, j + 1:].sum(axis=1)))
         # BUILD THE CDF from the LOWER, MIDDLE, and UPPER CLASSES
-        mixture_cdfs[:, middle_classes] = np.column_stack(tuple(stats.beta(*beta).cdf(x_j / upper) for beta in betas))
+        assert not posterior_pi[upper==0][:, middle_classes].any(), 'When sample\'s upper==0, middle_classes should be impossible'
+        frac = np.ones_like(x_j, dtype=np.float64)  # fraction of the remaining area covered by x_j
+        frac[upper > 0] = x_j[upper > 0] / upper[upper > 0]  # we need to be safe in case upper=0
+        mixture_cdfs[:, middle_classes] = np.column_stack(tuple(stats.beta(*beta).cdf(frac) for beta in betas))
     out = (posterior_pi * mixture_cdfs).sum(axis=1)
     # check output
     assert (out < 1 + 1e-10).all(), 'cdf must be less than 1'
     out = np.minimum(out,
                      1)  # clip to 1 (numerical error in posterior_weights can cause it to be slightly greater than 1
     assert (out <= 1).all(), 'cdf must be less than 1'
     assert (0 <= out).all(), 'cdf must be greater than 0'
@@ -138,29 +141,31 @@
         ).rvs()
         cdf_before_upper_delta = cdf(upper[upper_samples] - DELTA, prior, pre_samples[upper_samples])
         U[upper_samples, j] = stats.uniform(
             cdf_before_upper_delta,
             1 - cdf_before_upper_delta
         ).rvs()
         U[middle_samples, j] = cdf(x_j[middle_samples], prior, pre_samples[middle_samples])
+        assert np.all((0 < U[:, j]) & (U[:, j] < 1)), 'uniform samples must be in the interval (0, 1)'
     # check output
     assert np.all((0 < U) & (U < 1))
     return U
 
 
 def deuniformize(U: NDArray[np.float64], prior: dirichlet.MixedDirichlet, x_0 = None) -> NDArray[np.uint32]:
     # check inputs
     assert U.shape[1] == prior.full_alpha.shape[1], 'uniform samples must have the same number of components as prior'
     assert (0 < U).all() and (U < 1).all(), 'uniform samples must be in the interval (0, 1)'
     # build the samples
     X = np.zeros_like(U, dtype=np.uint32)
     if x_0 is not None:
         X[:, 0] = x_0
     I, J = U.shape
-    for j in range((1 if x_0 else 0), J):
+    j_start = 1 if x_0 is not None else 0
+    for j in range(j_start, J):
         pre_samples = X[:, :j]
         u_j = U[:, j]
         X[:, j] = inv_cdf(u_j, prior, pre_samples)
     # check output
     assert (X >= 0).all() and (X <= ONE).all(), 'samples must be in the interval [0, 1]'
     assert X.dtype == np.uint32, 'samples must use uint32 representation of components'
     assert X.shape == U.shape, 'samples must have the same shape as U'
```

### Comparing `simplex_assimilate-0.1.0/simplex_assimilate/dirichlet.py` & `simplex_assimilate-0.1.1/simplex_assimilate/dirichlet.py`

 * *Files identical despite different names*

### Comparing `simplex_assimilate-0.1.0/simplex_assimilate/quantize.py` & `simplex_assimilate-0.1.1/simplex_assimilate/quantize.py`

 * *Files identical despite different names*

### Comparing `simplex_assimilate-0.1.0/PKG-INFO` & `simplex_assimilate-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: simplex-assimilate
-Version: 0.1.0
+Version: 0.1.1
 Summary: Perform Data Assimilation on the Simplex. Models an ensemble as a mixture of Dirichlet distributions.
 Author: Oscar Laird
 Author-email: olaird25@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Simplex Assimilate: Data assimilation on the simplex
 
+![Coverage](tests/coverage.svg)
+
 ## Installation 
 ```bash
 pip install simplex-assimilate
 ```
 
 ## File Structure
  - `simplex_assimilate/` source code
- - `simplex_assimilate/cdf_transport.py` Optimal transport of samples on the simplex.
+ - `simplex_assimilate/cdf.py` Conditional distribution functions for the mixed dirichlet prior.
  - `simplex_assimilate/quantize.py` Convert floating point samples to fixed point representation.
  - `simplex_assimilate/dirichlet.py` Model samples on the simplex with a mixture of Dirichlet distributions. Fit parameters by maximum likelihood.
+ - `simplex_assimilate/transport.py` Optimal transport of samples on the simplex.
  - `tests/` unit tests
  - `coverage_report/` coverage reports
 
 ## See Also
   - [Ice Simplex Assimilate Repository](https://github.com/oscarlaird/ice_simplex_assimilate)
     - Represent an ice thickness distribution as a point on the simplex and perform transport.
```

