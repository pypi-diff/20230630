# Comparing `tmp/cyc-gbm-0.0.22.tar.gz` & `tmp/cyc-gbm-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyc-gbm-0.0.22.tar", last modified: Fri Jun 30 07:02:19 2023, max compression
+gzip compressed data, was "cyc-gbm-0.0.23.tar", last modified: Fri Jun 30 08:49:36 2023, max compression
```

## Comparing `cyc-gbm-0.0.22.tar` & `cyc-gbm-0.0.23.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 07:02:19.774740 cyc-gbm-0.0.22/
--rw-r--r--   0 Henning    (501) staff       (20)     1073 2023-06-28 08:34:18.000000 cyc-gbm-0.0.22/LICENSE
--rw-r--r--   0 Henning    (501) staff       (20)       24 2023-06-28 13:08:08.000000 cyc-gbm-0.0.22/MANIFEST.in
--rw-r--r--   0 Henning    (501) staff       (20)     2898 2023-06-30 07:02:19.771444 cyc-gbm-0.0.22/PKG-INFO
--rw-r--r--   0 Henning    (501) staff       (20)     2399 2023-06-30 06:59:14.000000 cyc-gbm-0.0.22/README.md
-drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 07:02:19.756438 cyc-gbm-0.0.22/cyc_gbm/
--rw-r--r--   0 Henning    (501) staff       (20)       75 2023-06-12 14:42:41.000000 cyc-gbm-0.0.22/cyc_gbm/__init__.py
--rw-r--r--   0 Henning    (501) staff       (20)     5303 2023-06-28 11:32:48.000000 cyc-gbm-0.0.22/cyc_gbm/baseline_models.py
--rw-r--r--   0 Henning    (501) staff       (20)     7198 2023-06-28 11:32:48.000000 cyc-gbm-0.0.22/cyc_gbm/cyc_gbm.py
--rw-r--r--   0 Henning    (501) staff       (20)    25435 2023-06-12 14:42:41.000000 cyc-gbm-0.0.22/cyc_gbm/distributions.py
--rw-r--r--   0 Henning    (501) staff       (20)     4030 2023-06-28 11:01:36.000000 cyc-gbm-0.0.22/cyc_gbm/gbm_tree.py
--rw-r--r--   0 Henning    (501) staff       (20)     3054 2023-06-12 14:42:41.000000 cyc-gbm-0.0.22/cyc_gbm/logger.py
--rw-r--r--   0 Henning    (501) staff       (20)    12282 2023-06-28 11:32:48.000000 cyc-gbm-0.0.22/cyc_gbm/numerical_illustration.py
--rw-r--r--   0 Henning    (501) staff       (20)     6461 2023-06-28 11:32:48.000000 cyc-gbm-0.0.22/cyc_gbm/tune_kappa.py
-drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 07:02:19.765873 cyc-gbm-0.0.22/cyc_gbm.egg-info/
--rw-r--r--   0 Henning    (501) staff       (20)     2898 2023-06-30 07:02:19.000000 cyc-gbm-0.0.22/cyc_gbm.egg-info/PKG-INFO
--rw-r--r--   0 Henning    (501) staff       (20)      431 2023-06-30 07:02:19.000000 cyc-gbm-0.0.22/cyc_gbm.egg-info/SOURCES.txt
--rw-r--r--   0 Henning    (501) staff       (20)        1 2023-06-30 07:02:19.000000 cyc-gbm-0.0.22/cyc_gbm.egg-info/dependency_links.txt
--rw-r--r--   0 Henning    (501) staff       (20)       62 2023-06-30 07:02:19.000000 cyc-gbm-0.0.22/cyc_gbm.egg-info/requires.txt
--rw-r--r--   0 Henning    (501) staff       (20)        8 2023-06-30 07:02:19.000000 cyc-gbm-0.0.22/cyc_gbm.egg-info/top_level.txt
--rw-r--r--   0 Henning    (501) staff       (20)      475 2023-06-28 08:34:18.000000 cyc-gbm-0.0.22/pyproject.toml
--rw-r--r--   0 Henning    (501) staff       (20)       62 2023-06-28 13:39:29.000000 cyc-gbm-0.0.22/requirements.txt
--rw-r--r--   0 Henning    (501) staff       (20)       38 2023-06-30 07:02:19.775582 cyc-gbm-0.0.22/setup.cfg
--rw-r--r--   0 Henning    (501) staff       (20)      871 2023-06-30 07:01:19.000000 cyc-gbm-0.0.22/setup.py
-drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 07:02:19.768328 cyc-gbm-0.0.22/tests/
--rw-r--r--   0 Henning    (501) staff       (20)    17413 2023-06-28 11:49:31.000000 cyc-gbm-0.0.22/tests/test_cyc_gbm.py
+drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 08:49:36.170157 cyc-gbm-0.0.23/
+-rw-r--r--   0 Henning    (501) staff       (20)     1073 2023-06-28 08:34:18.000000 cyc-gbm-0.0.23/LICENSE
+-rw-r--r--   0 Henning    (501) staff       (20)       24 2023-06-30 07:06:30.000000 cyc-gbm-0.0.23/MANIFEST.in
+-rw-r--r--   0 Henning    (501) staff       (20)     2898 2023-06-30 08:49:36.169420 cyc-gbm-0.0.23/PKG-INFO
+-rw-r--r--   0 Henning    (501) staff       (20)     2399 2023-06-30 07:06:30.000000 cyc-gbm-0.0.23/README.md
+drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 08:49:36.158284 cyc-gbm-0.0.23/cyc_gbm/
+-rw-r--r--   0 Henning    (501) staff       (20)       75 2023-06-12 14:42:41.000000 cyc-gbm-0.0.23/cyc_gbm/__init__.py
+-rw-r--r--   0 Henning    (501) staff       (20)     5303 2023-06-28 11:32:48.000000 cyc-gbm-0.0.23/cyc_gbm/baseline_models.py
+-rw-r--r--   0 Henning    (501) staff       (20)     7198 2023-06-28 11:32:48.000000 cyc-gbm-0.0.23/cyc_gbm/cyc_gbm.py
+-rw-r--r--   0 Henning    (501) staff       (20)    26784 2023-06-30 08:48:10.000000 cyc-gbm-0.0.23/cyc_gbm/distributions.py
+-rw-r--r--   0 Henning    (501) staff       (20)     4030 2023-06-28 11:01:36.000000 cyc-gbm-0.0.23/cyc_gbm/gbm_tree.py
+-rw-r--r--   0 Henning    (501) staff       (20)     3054 2023-06-12 14:42:41.000000 cyc-gbm-0.0.23/cyc_gbm/logger.py
+-rw-r--r--   0 Henning    (501) staff       (20)    12282 2023-06-28 11:32:48.000000 cyc-gbm-0.0.23/cyc_gbm/numerical_illustration.py
+-rw-r--r--   0 Henning    (501) staff       (20)     6461 2023-06-28 11:32:48.000000 cyc-gbm-0.0.23/cyc_gbm/tune_kappa.py
+drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 08:49:36.166387 cyc-gbm-0.0.23/cyc_gbm.egg-info/
+-rw-r--r--   0 Henning    (501) staff       (20)     2898 2023-06-30 08:49:36.000000 cyc-gbm-0.0.23/cyc_gbm.egg-info/PKG-INFO
+-rw-r--r--   0 Henning    (501) staff       (20)      431 2023-06-30 08:49:36.000000 cyc-gbm-0.0.23/cyc_gbm.egg-info/SOURCES.txt
+-rw-r--r--   0 Henning    (501) staff       (20)        1 2023-06-30 08:49:36.000000 cyc-gbm-0.0.23/cyc_gbm.egg-info/dependency_links.txt
+-rw-r--r--   0 Henning    (501) staff       (20)       62 2023-06-30 08:49:36.000000 cyc-gbm-0.0.23/cyc_gbm.egg-info/requires.txt
+-rw-r--r--   0 Henning    (501) staff       (20)        8 2023-06-30 08:49:36.000000 cyc-gbm-0.0.23/cyc_gbm.egg-info/top_level.txt
+-rw-r--r--   0 Henning    (501) staff       (20)      475 2023-06-28 08:34:18.000000 cyc-gbm-0.0.23/pyproject.toml
+-rw-r--r--   0 Henning    (501) staff       (20)       62 2023-06-30 07:06:30.000000 cyc-gbm-0.0.23/requirements.txt
+-rw-r--r--   0 Henning    (501) staff       (20)       38 2023-06-30 08:49:36.170421 cyc-gbm-0.0.23/setup.cfg
+-rw-r--r--   0 Henning    (501) staff       (20)      871 2023-06-30 08:48:27.000000 cyc-gbm-0.0.23/setup.py
+drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 08:49:36.167394 cyc-gbm-0.0.23/tests/
+-rw-r--r--   0 Henning    (501) staff       (20)    17413 2023-06-28 11:49:31.000000 cyc-gbm-0.0.23/tests/test_cyc_gbm.py
```

### Comparing `cyc-gbm-0.0.22/LICENSE` & `cyc-gbm-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.22/PKG-INFO` & `cyc-gbm-0.0.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyc-gbm
-Version: 0.0.22
+Version: 0.0.23
 Summary: A python package for the Cyclical Gradient Boosting Machine algorithm
 Home-page: https://github.com/henningzakrisson/cyc-gbm
 Author: Henning Zakrisson
 Author-email: henning.zakrisson@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cyc-gbm-0.0.22/README.md` & `cyc-gbm-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.22/cyc_gbm/baseline_models.py` & `cyc-gbm-0.0.23/cyc_gbm/baseline_models.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.22/cyc_gbm/cyc_gbm.py` & `cyc-gbm-0.0.23/cyc_gbm/cyc_gbm.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.22/cyc_gbm/distributions.py` & `cyc-gbm-0.0.23/cyc_gbm/distributions.py`

 * *Files 3% similar despite different names*

```diff
@@ -330,14 +330,56 @@
         self, z: np.ndarray, k: int, w: Union[np.ndarray, float] = 1.0
     ) -> np.ndarray:
         if k == 1:
             return w * z[0]
         elif k == 2:
             return w * np.exp(2 * z[1])
 
+class NormalDistributionUni(Distribution):
+    def __init__(
+        self,
+    ):
+        """Initialize a normal distribution object with only the mu parameter.
+
+        Parameterization: z[0] = mu, where E[X] = mu, Var(X) = 1
+        """
+        super().__init__(d=1)
+
+    def loss(
+        self, y: np.ndarray, z: np.ndarray, w: Union[np.ndarray, float] = 1.0
+    ) -> np.ndarray:
+        if np.any(w != 1):
+            raise NotImplementedError(
+                "Weighted loss not implemented for univariatevariate normal distribution"
+            )
+        return (y - z[0]) ** 2
+
+    def grad(
+        self, y: np.ndarray, z: np.ndarray, j: int = 0, w: Union[np.ndarray, float] = 1.0
+    ) -> np.ndarray:
+        return y - z[0]
+
+    def mme(self, y: np.ndarray, w: Union[np.ndarray, float] = 1.0) -> np.ndarray:
+        return y.mean()
+
+    def simulate(
+        self,
+        z: np.ndarray,
+        w: Union[np.ndarray, float] = 1.0,
+        random_state: Union[int, None] = None,
+        rng: Union[np.random.Generator, None] = None,
+    ) -> np.ndarray:
+        if rng is None:
+            rng = np.random.default_rng(seed=random_state)
+        return rng.normal(z[0], 1)
+
+    def moment(
+        self, z: np.ndarray, k: int = 1, w: Union[np.ndarray, float] = 1.0
+    ) -> np.ndarray:
+        return z[0]
 
 @inherit_docstrings
 class NegativeBinomialDistribution(Distribution):
     def __init__(
         self,
     ):
         """Initialize a negative binomial distribution object.
@@ -725,31 +767,34 @@
             ],
             np.ndarray,
         ],
     ] = None,
     moment: Union[
         None, Callable[[np.ndarray, int, Union[np.ndarray, float]], np.ndarray]
     ] = None,
-    d: Union[None, int] = None,
+    d: int = 2,
 ) -> Distribution:
     """
     Returns a probability distribution object based on the distribution name.
 
     :param distribution: A string representing the name of the distribution to create.
     :param loss: A function that computes the loss. Only used if dist == "custom".
     :param grad: A function that computes the gradient of the loss. Only used if dist == "custom".
     :param mme: A function that computes the method of moments estimator. Only used if dist == "custom".
     :param simulate: A function that simulates data from the distribution. Only used if dist == "custom".
     :param moment: A function that computes the kth moment of the distribution. Only used if dist == "custom".
-    :param d: The dimension of the distribution. Only used if dist == "custom".
+    :param d: The dimension of the distribution.
     :return: A probability distribution object based on the distribution name.
     :raises UnknownDistribution: If the input distribution name is not recognized.
     """
     if distribution == "normal":
-        return NormalDistribution()
+        if d ==1:
+            return NormalDistributionUni()
+        if d==2:
+            return NormalDistribution()
     if distribution == "gamma":
         return GammaDistribution()
     if distribution == "beta_prime":
         return BetaPrimeDistribution()
     if distribution == "inv_gauss":
         return InverseGaussianDistribution()
     if distribution == "neg_bin":
```

### Comparing `cyc-gbm-0.0.22/cyc_gbm/gbm_tree.py` & `cyc-gbm-0.0.23/cyc_gbm/gbm_tree.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.22/cyc_gbm/logger.py` & `cyc-gbm-0.0.23/cyc_gbm/logger.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.22/cyc_gbm/numerical_illustration.py` & `cyc-gbm-0.0.23/cyc_gbm/numerical_illustration.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.22/cyc_gbm/tune_kappa.py` & `cyc-gbm-0.0.23/cyc_gbm/tune_kappa.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.22/cyc_gbm.egg-info/PKG-INFO` & `cyc-gbm-0.0.23/cyc_gbm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyc-gbm
-Version: 0.0.22
+Version: 0.0.23
 Summary: A python package for the Cyclical Gradient Boosting Machine algorithm
 Home-page: https://github.com/henningzakrisson/cyc-gbm
 Author: Henning Zakrisson
 Author-email: henning.zakrisson@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cyc-gbm-0.0.22/setup.py` & `cyc-gbm-0.0.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="cyc-gbm",
-    version="0.0.22",
+    version="0.0.23",
     author="Henning Zakrisson",
     author_email="henning.zakrisson@gmail.com",
     description="A python package for the Cyclical Gradient Boosting Machine algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/henningzakrisson/cyc-gbm",
     packages=find_packages(),
```

### Comparing `cyc-gbm-0.0.22/tests/test_cyc_gbm.py` & `cyc-gbm-0.0.23/tests/test_cyc_gbm.py`

 * *Files identical despite different names*

