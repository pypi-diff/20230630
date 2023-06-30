# Comparing `tmp/cyc-gbm-0.0.21.tar.gz` & `tmp/cyc-gbm-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyc-gbm-0.0.21.tar", last modified: Fri Jun 30 06:36:41 2023, max compression
+gzip compressed data, was "cyc-gbm-0.0.22.tar", last modified: Fri Jun 30 07:02:19 2023, max compression
```

## Comparing `cyc-gbm-0.0.21.tar` & `cyc-gbm-0.0.22.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 06:36:41.447723 cyc-gbm-0.0.21/
--rw-r--r--   0 Henning    (501) staff       (20)     1073 2023-06-28 08:34:18.000000 cyc-gbm-0.0.21/LICENSE
--rw-r--r--   0 Henning    (501) staff       (20)       24 2023-06-28 13:08:08.000000 cyc-gbm-0.0.21/MANIFEST.in
--rw-r--r--   0 Henning    (501) staff       (20)     3000 2023-06-30 06:36:41.446454 cyc-gbm-0.0.21/PKG-INFO
--rw-r--r--   0 Henning    (501) staff       (20)     2501 2023-06-28 12:35:30.000000 cyc-gbm-0.0.21/README.md
-drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 06:36:41.437609 cyc-gbm-0.0.21/cyc_gbm/
--rw-r--r--   0 Henning    (501) staff       (20)       75 2023-06-12 14:42:41.000000 cyc-gbm-0.0.21/cyc_gbm/__init__.py
--rw-r--r--   0 Henning    (501) staff       (20)     5303 2023-06-28 11:32:48.000000 cyc-gbm-0.0.21/cyc_gbm/baseline_models.py
--rw-r--r--   0 Henning    (501) staff       (20)     7198 2023-06-28 11:32:48.000000 cyc-gbm-0.0.21/cyc_gbm/cyc_gbm.py
--rw-r--r--   0 Henning    (501) staff       (20)    25435 2023-06-12 14:42:41.000000 cyc-gbm-0.0.21/cyc_gbm/distributions.py
--rw-r--r--   0 Henning    (501) staff       (20)     4030 2023-06-28 11:01:36.000000 cyc-gbm-0.0.21/cyc_gbm/gbm_tree.py
--rw-r--r--   0 Henning    (501) staff       (20)     3054 2023-06-12 14:42:41.000000 cyc-gbm-0.0.21/cyc_gbm/logger.py
--rw-r--r--   0 Henning    (501) staff       (20)    12282 2023-06-28 11:32:48.000000 cyc-gbm-0.0.21/cyc_gbm/numerical_illustration.py
--rw-r--r--   0 Henning    (501) staff       (20)     6461 2023-06-28 11:32:48.000000 cyc-gbm-0.0.21/cyc_gbm/tune_kappa.py
-drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 06:36:41.442140 cyc-gbm-0.0.21/cyc_gbm.egg-info/
--rw-r--r--   0 Henning    (501) staff       (20)     3000 2023-06-30 06:36:41.000000 cyc-gbm-0.0.21/cyc_gbm.egg-info/PKG-INFO
--rw-r--r--   0 Henning    (501) staff       (20)      431 2023-06-30 06:36:41.000000 cyc-gbm-0.0.21/cyc_gbm.egg-info/SOURCES.txt
--rw-r--r--   0 Henning    (501) staff       (20)        1 2023-06-30 06:36:41.000000 cyc-gbm-0.0.21/cyc_gbm.egg-info/dependency_links.txt
--rw-r--r--   0 Henning    (501) staff       (20)       62 2023-06-30 06:36:41.000000 cyc-gbm-0.0.21/cyc_gbm.egg-info/requires.txt
--rw-r--r--   0 Henning    (501) staff       (20)        8 2023-06-30 06:36:41.000000 cyc-gbm-0.0.21/cyc_gbm.egg-info/top_level.txt
--rw-r--r--   0 Henning    (501) staff       (20)      475 2023-06-28 08:34:18.000000 cyc-gbm-0.0.21/pyproject.toml
--rw-r--r--   0 Henning    (501) staff       (20)       62 2023-06-28 13:39:29.000000 cyc-gbm-0.0.21/requirements.txt
--rw-r--r--   0 Henning    (501) staff       (20)       38 2023-06-30 06:36:41.447936 cyc-gbm-0.0.21/setup.cfg
--rw-r--r--   0 Henning    (501) staff       (20)      871 2023-06-28 13:39:41.000000 cyc-gbm-0.0.21/setup.py
-drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 06:36:41.443104 cyc-gbm-0.0.21/tests/
--rw-r--r--   0 Henning    (501) staff       (20)    17413 2023-06-28 11:49:31.000000 cyc-gbm-0.0.21/tests/test_cyc_gbm.py
+drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 07:02:19.774740 cyc-gbm-0.0.22/
+-rw-r--r--   0 Henning    (501) staff       (20)     1073 2023-06-28 08:34:18.000000 cyc-gbm-0.0.22/LICENSE
+-rw-r--r--   0 Henning    (501) staff       (20)       24 2023-06-28 13:08:08.000000 cyc-gbm-0.0.22/MANIFEST.in
+-rw-r--r--   0 Henning    (501) staff       (20)     2898 2023-06-30 07:02:19.771444 cyc-gbm-0.0.22/PKG-INFO
+-rw-r--r--   0 Henning    (501) staff       (20)     2399 2023-06-30 06:59:14.000000 cyc-gbm-0.0.22/README.md
+drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 07:02:19.756438 cyc-gbm-0.0.22/cyc_gbm/
+-rw-r--r--   0 Henning    (501) staff       (20)       75 2023-06-12 14:42:41.000000 cyc-gbm-0.0.22/cyc_gbm/__init__.py
+-rw-r--r--   0 Henning    (501) staff       (20)     5303 2023-06-28 11:32:48.000000 cyc-gbm-0.0.22/cyc_gbm/baseline_models.py
+-rw-r--r--   0 Henning    (501) staff       (20)     7198 2023-06-28 11:32:48.000000 cyc-gbm-0.0.22/cyc_gbm/cyc_gbm.py
+-rw-r--r--   0 Henning    (501) staff       (20)    25435 2023-06-12 14:42:41.000000 cyc-gbm-0.0.22/cyc_gbm/distributions.py
+-rw-r--r--   0 Henning    (501) staff       (20)     4030 2023-06-28 11:01:36.000000 cyc-gbm-0.0.22/cyc_gbm/gbm_tree.py
+-rw-r--r--   0 Henning    (501) staff       (20)     3054 2023-06-12 14:42:41.000000 cyc-gbm-0.0.22/cyc_gbm/logger.py
+-rw-r--r--   0 Henning    (501) staff       (20)    12282 2023-06-28 11:32:48.000000 cyc-gbm-0.0.22/cyc_gbm/numerical_illustration.py
+-rw-r--r--   0 Henning    (501) staff       (20)     6461 2023-06-28 11:32:48.000000 cyc-gbm-0.0.22/cyc_gbm/tune_kappa.py
+drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 07:02:19.765873 cyc-gbm-0.0.22/cyc_gbm.egg-info/
+-rw-r--r--   0 Henning    (501) staff       (20)     2898 2023-06-30 07:02:19.000000 cyc-gbm-0.0.22/cyc_gbm.egg-info/PKG-INFO
+-rw-r--r--   0 Henning    (501) staff       (20)      431 2023-06-30 07:02:19.000000 cyc-gbm-0.0.22/cyc_gbm.egg-info/SOURCES.txt
+-rw-r--r--   0 Henning    (501) staff       (20)        1 2023-06-30 07:02:19.000000 cyc-gbm-0.0.22/cyc_gbm.egg-info/dependency_links.txt
+-rw-r--r--   0 Henning    (501) staff       (20)       62 2023-06-30 07:02:19.000000 cyc-gbm-0.0.22/cyc_gbm.egg-info/requires.txt
+-rw-r--r--   0 Henning    (501) staff       (20)        8 2023-06-30 07:02:19.000000 cyc-gbm-0.0.22/cyc_gbm.egg-info/top_level.txt
+-rw-r--r--   0 Henning    (501) staff       (20)      475 2023-06-28 08:34:18.000000 cyc-gbm-0.0.22/pyproject.toml
+-rw-r--r--   0 Henning    (501) staff       (20)       62 2023-06-28 13:39:29.000000 cyc-gbm-0.0.22/requirements.txt
+-rw-r--r--   0 Henning    (501) staff       (20)       38 2023-06-30 07:02:19.775582 cyc-gbm-0.0.22/setup.cfg
+-rw-r--r--   0 Henning    (501) staff       (20)      871 2023-06-30 07:01:19.000000 cyc-gbm-0.0.22/setup.py
+drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 07:02:19.768328 cyc-gbm-0.0.22/tests/
+-rw-r--r--   0 Henning    (501) staff       (20)    17413 2023-06-28 11:49:31.000000 cyc-gbm-0.0.22/tests/test_cyc_gbm.py
```

### Comparing `cyc-gbm-0.0.21/LICENSE` & `cyc-gbm-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.21/PKG-INFO` & `cyc-gbm-0.0.22/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyc-gbm
-Version: 0.0.21
+Version: 0.0.22
 Summary: A python package for the Cyclical Gradient Boosting Machine algorithm
 Home-page: https://github.com/henningzakrisson/cyc-gbm
 Author: Henning Zakrisson
 Author-email: henning.zakrisson@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cyc-gbm
 A package for the Cyclical Gradient Boosting Machine algorithm. For the (pre-print) paper describing the algorithm, see [here](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4352505).
 
 ## Installation
+You can install the package using pip:
+```bash
+pip install cyc-gbm
+```
+Alternatively, you can install the package from source by following these steps:
+
 1. Clone this repository to your local machine:
     ```bash
     git clone https://github.com/henningzakrisson/c-gbm.git
     ```
 2. Create a virtual environment in the root directory of the repository:
     ```bash
     python3 -m venv venv
@@ -35,44 +41,37 @@
     ```
 ## Usage example
 Fitting the mean and (log) sigma parameters of a normal distribution to a simulated dataset:
 
 ```python
 import numpy as np
 from cyc_gbm import CycGBM
-from cyc_gbm.distributions import initiate_distribution
+from sklearn.model_selection import train_test_split
 
 # Simulate data
-X = np.random.normal(size=(10000, 3))
+X = np.random.normal(size=(1000, 2))
 mu = X[:, 0] + 10 * (X[:, 1] > 0)
-log_sigma = 3 - 2 * (X[:, 1] > 0)
-z = np.stack([mu, log_sigma], axis=0)
-dist = initiate_distribution(distribution='normal')
-y = dist.simulate(z=z)
+sigma = np.exp(3 - 2 * (X[:, 0] > 0))
+y = np.random.normal(mu, sigma)
 
 # Split data
-idx = np.arange(X.shape[0])
-np.random.shuffle(idx)
-idx_train, idx_test = idx[:500], idx[500:]
-X_train, y_train, z_train = X[idx_train], y[idx_train], z[:, idx_train]
-X_test, y_test, z_test = X[idx_test], y[idx_test], z[:, idx_test]
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
 
 # Fit model
 model = CycGBM(
    distribution='normal',
-   kappa=[40, 20],
+   kappa=[26,34],
    eps=0.1,
    max_depth=2,
-   min_samples_leaf=10,
+   min_samples_leaf=20,
 )
 model.fit(X_train, y_train)
 
 # Evaluate
-z_hat = model.predict(X_test)
-loss = model.dist.loss(y=y_test, z=z_hat).sum()
+loss = model.dist.loss(y=y_test, z=model.predict(X_test)).sum()
 print(f'negative log likelihood: {loss}')
 ```
 
 ## Reproducing the numerical illustrations in the paper
 The numerical illustrations in the paper can be reproduced by running the ````numerical_illustration```` function in the ````src/numerical_illustration.py```` module. 
 The function takes the path to a configuration file as input. 
 The configuration file is a yaml file that specifies the parameters of the numerical illustration.
```

### Comparing `cyc-gbm-0.0.21/README.md` & `cyc-gbm-0.0.22/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # cyc-gbm
 A package for the Cyclical Gradient Boosting Machine algorithm. For the (pre-print) paper describing the algorithm, see [here](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4352505).
 
 ## Installation
+You can install the package using pip:
+```bash
+pip install cyc-gbm
+```
+Alternatively, you can install the package from source by following these steps:
+
 1. Clone this repository to your local machine:
     ```bash
     git clone https://github.com/henningzakrisson/c-gbm.git
     ```
 2. Create a virtual environment in the root directory of the repository:
     ```bash
     python3 -m venv venv
@@ -20,44 +26,37 @@
     ```
 ## Usage example
 Fitting the mean and (log) sigma parameters of a normal distribution to a simulated dataset:
 
 ```python
 import numpy as np
 from cyc_gbm import CycGBM
-from cyc_gbm.distributions import initiate_distribution
+from sklearn.model_selection import train_test_split
 
 # Simulate data
-X = np.random.normal(size=(10000, 3))
+X = np.random.normal(size=(1000, 2))
 mu = X[:, 0] + 10 * (X[:, 1] > 0)
-log_sigma = 3 - 2 * (X[:, 1] > 0)
-z = np.stack([mu, log_sigma], axis=0)
-dist = initiate_distribution(distribution='normal')
-y = dist.simulate(z=z)
+sigma = np.exp(3 - 2 * (X[:, 0] > 0))
+y = np.random.normal(mu, sigma)
 
 # Split data
-idx = np.arange(X.shape[0])
-np.random.shuffle(idx)
-idx_train, idx_test = idx[:500], idx[500:]
-X_train, y_train, z_train = X[idx_train], y[idx_train], z[:, idx_train]
-X_test, y_test, z_test = X[idx_test], y[idx_test], z[:, idx_test]
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
 
 # Fit model
 model = CycGBM(
    distribution='normal',
-   kappa=[40, 20],
+   kappa=[26,34],
    eps=0.1,
    max_depth=2,
-   min_samples_leaf=10,
+   min_samples_leaf=20,
 )
 model.fit(X_train, y_train)
 
 # Evaluate
-z_hat = model.predict(X_test)
-loss = model.dist.loss(y=y_test, z=z_hat).sum()
+loss = model.dist.loss(y=y_test, z=model.predict(X_test)).sum()
 print(f'negative log likelihood: {loss}')
 ```
 
 ## Reproducing the numerical illustrations in the paper
 The numerical illustrations in the paper can be reproduced by running the ````numerical_illustration```` function in the ````src/numerical_illustration.py```` module. 
 The function takes the path to a configuration file as input. 
 The configuration file is a yaml file that specifies the parameters of the numerical illustration.
```

### Comparing `cyc-gbm-0.0.21/cyc_gbm/baseline_models.py` & `cyc-gbm-0.0.22/cyc_gbm/baseline_models.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.21/cyc_gbm/cyc_gbm.py` & `cyc-gbm-0.0.22/cyc_gbm/cyc_gbm.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.21/cyc_gbm/distributions.py` & `cyc-gbm-0.0.22/cyc_gbm/distributions.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.21/cyc_gbm/gbm_tree.py` & `cyc-gbm-0.0.22/cyc_gbm/gbm_tree.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.21/cyc_gbm/logger.py` & `cyc-gbm-0.0.22/cyc_gbm/logger.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.21/cyc_gbm/numerical_illustration.py` & `cyc-gbm-0.0.22/cyc_gbm/numerical_illustration.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.21/cyc_gbm/tune_kappa.py` & `cyc-gbm-0.0.22/cyc_gbm/tune_kappa.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.21/cyc_gbm.egg-info/PKG-INFO` & `cyc-gbm-0.0.22/cyc_gbm.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyc-gbm
-Version: 0.0.21
+Version: 0.0.22
 Summary: A python package for the Cyclical Gradient Boosting Machine algorithm
 Home-page: https://github.com/henningzakrisson/cyc-gbm
 Author: Henning Zakrisson
 Author-email: henning.zakrisson@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cyc-gbm
 A package for the Cyclical Gradient Boosting Machine algorithm. For the (pre-print) paper describing the algorithm, see [here](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4352505).
 
 ## Installation
+You can install the package using pip:
+```bash
+pip install cyc-gbm
+```
+Alternatively, you can install the package from source by following these steps:
+
 1. Clone this repository to your local machine:
     ```bash
     git clone https://github.com/henningzakrisson/c-gbm.git
     ```
 2. Create a virtual environment in the root directory of the repository:
     ```bash
     python3 -m venv venv
@@ -35,44 +41,37 @@
     ```
 ## Usage example
 Fitting the mean and (log) sigma parameters of a normal distribution to a simulated dataset:
 
 ```python
 import numpy as np
 from cyc_gbm import CycGBM
-from cyc_gbm.distributions import initiate_distribution
+from sklearn.model_selection import train_test_split
 
 # Simulate data
-X = np.random.normal(size=(10000, 3))
+X = np.random.normal(size=(1000, 2))
 mu = X[:, 0] + 10 * (X[:, 1] > 0)
-log_sigma = 3 - 2 * (X[:, 1] > 0)
-z = np.stack([mu, log_sigma], axis=0)
-dist = initiate_distribution(distribution='normal')
-y = dist.simulate(z=z)
+sigma = np.exp(3 - 2 * (X[:, 0] > 0))
+y = np.random.normal(mu, sigma)
 
 # Split data
-idx = np.arange(X.shape[0])
-np.random.shuffle(idx)
-idx_train, idx_test = idx[:500], idx[500:]
-X_train, y_train, z_train = X[idx_train], y[idx_train], z[:, idx_train]
-X_test, y_test, z_test = X[idx_test], y[idx_test], z[:, idx_test]
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
 
 # Fit model
 model = CycGBM(
    distribution='normal',
-   kappa=[40, 20],
+   kappa=[26,34],
    eps=0.1,
    max_depth=2,
-   min_samples_leaf=10,
+   min_samples_leaf=20,
 )
 model.fit(X_train, y_train)
 
 # Evaluate
-z_hat = model.predict(X_test)
-loss = model.dist.loss(y=y_test, z=z_hat).sum()
+loss = model.dist.loss(y=y_test, z=model.predict(X_test)).sum()
 print(f'negative log likelihood: {loss}')
 ```
 
 ## Reproducing the numerical illustrations in the paper
 The numerical illustrations in the paper can be reproduced by running the ````numerical_illustration```` function in the ````src/numerical_illustration.py```` module. 
 The function takes the path to a configuration file as input. 
 The configuration file is a yaml file that specifies the parameters of the numerical illustration.
```

### Comparing `cyc-gbm-0.0.21/setup.py` & `cyc-gbm-0.0.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="cyc-gbm",
-    version="0.0.21",
+    version="0.0.22",
     author="Henning Zakrisson",
     author_email="henning.zakrisson@gmail.com",
     description="A python package for the Cyclical Gradient Boosting Machine algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/henningzakrisson/cyc-gbm",
     packages=find_packages(),
```

### Comparing `cyc-gbm-0.0.21/tests/test_cyc_gbm.py` & `cyc-gbm-0.0.22/tests/test_cyc_gbm.py`

 * *Files identical despite different names*

