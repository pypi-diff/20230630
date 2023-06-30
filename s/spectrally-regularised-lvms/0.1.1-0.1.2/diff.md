# Comparing `tmp/spectrally_regularised_lvms-0.1.1.tar.gz` & `tmp/spectrally_regularised_lvms-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrally_regularised_lvms-0.1.1.tar", max compression
+gzip compressed data, was "spectrally_regularised_lvms-0.1.2.tar", max compression
```

## Comparing `spectrally_regularised_lvms-0.1.1.tar` & `spectrally_regularised_lvms-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1090 2023-04-28 07:39:34.154025 spectrally_regularised_lvms-0.1.1/LICENSE
--rw-r--r--   0        0        0     1732 2023-06-09 10:28:34.571440 spectrally_regularised_lvms-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6972 2023-06-09 10:17:44.865209 spectrally_regularised_lvms-0.1.1/README.md
--rw-r--r--   0        0        0     1201 2023-06-09 10:21:40.319411 spectrally_regularised_lvms-0.1.1/spectrally_regularised_LVMs/__init__.py
--rw-r--r--   0        0        0    32459 2023-05-29 12:05:32.601314 spectrally_regularised_lvms-0.1.1/spectrally_regularised_LVMs/cost_functions.py
--rw-r--r--   0        0        0    21405 2023-05-26 12:13:55.515128 spectrally_regularised_lvms-0.1.1/spectrally_regularised_LVMs/helper_methods.py
--rw-r--r--   0        0        0    13584 2023-05-26 12:13:55.515631 spectrally_regularised_lvms-0.1.1/spectrally_regularised_LVMs/negen_approx.py
--rw-r--r--   0        0        0    16767 2023-06-09 10:22:09.397167 spectrally_regularised_lvms-0.1.1/spectrally_regularised_LVMs/spectral_regulariser.py
--rw-r--r--   0        0        0    52590 2023-06-09 10:22:40.773825 spectrally_regularised_lvms-0.1.1/spectrally_regularised_LVMs/spectrally_regularised_model.py
--rw-r--r--   0        0        0     8183 1970-01-01 00:00:00.000000 spectrally_regularised_lvms-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-28 07:39:34.154025 spectrally_regularised_lvms-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1778 2023-06-30 09:54:42.114178 spectrally_regularised_lvms-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3762 2023-06-18 11:04:30.198907 spectrally_regularised_lvms-0.1.2/README.md
+-rw-r--r--   0        0        0     1201 2023-06-30 09:54:42.125360 spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/__init__.py
+-rw-r--r--   0        0        0    32459 2023-05-29 12:05:32.601314 spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/cost_functions.py
+-rw-r--r--   0        0        0    21405 2023-05-26 12:13:55.515128 spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/helper_methods.py
+-rw-r--r--   0        0        0    13584 2023-05-26 12:13:55.515631 spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/negen_approx.py
+-rw-r--r--   0        0        0    16767 2023-06-09 10:22:09.397167 spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/spectral_regulariser.py
+-rw-r--r--   0        0        0    52758 2023-06-30 09:53:06.824340 spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/spectrally_regularised_model.py
+-rw-r--r--   0        0        0     5077 1970-01-01 00:00:00.000000 spectrally_regularised_lvms-0.1.2/PKG-INFO
```

### Comparing `spectrally_regularised_lvms-0.1.1/LICENSE` & `spectrally_regularised_lvms-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrally_regularised_lvms-0.1.1/pyproject.toml` & `spectrally_regularised_lvms-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrally-regularised-LVMs"
-version = "0.1.1"
+version = "0.1.2"
 description = "An implementation of linear LVMs with a spectral regulariser."
 authors = ["Ryan Balshaw <ryanbalshaw81@gmail.com>"]
 maintainers = ["Ryan Balshaw <ryanbalshaw81@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/RyanBalshaw/spectrally-regularised-LVMs"
 repository = "https://github.com/RyanBalshaw/spectrally-regularised-LVMs"
@@ -43,14 +43,16 @@
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
 sphinx-autobuild = ">=2021.0"
 sphinx-rtd-theme = ">=1.0"
+numpydoc = "^1.5.0"
+autodocsumm = "^0.2.11"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "Bug tracker" = "https://github.com/RyanBalshaw/spectrally-regularised-LVMs/issues"
```

### Comparing `spectrally_regularised_lvms-0.1.1/spectrally_regularised_LVMs/__init__.py` & `spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     hankel_matrix,
 )
 from .negen_approx import CubeObject, ExpObject, LogcoshObject, QuadObject
 from .spectral_regulariser import SpectralObjective
 from .spectrally_regularised_model import LinearModel
 
 __author__ = "Ryan Balshaw"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __email__ = "ryanbalshaw81@gmail.com"
 __description__ = (
     "Train linear LVMs with the addition "
     "of a spectral regularisation term with minimal effort."
 )
 __uri__ = "http://spectrally-regularised-lvms.readthedocs.io/"
 __all__ = [
```

### Comparing `spectrally_regularised_lvms-0.1.1/spectrally_regularised_LVMs/cost_functions.py` & `spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/cost_functions.py`

 * *Files identical despite different names*

### Comparing `spectrally_regularised_lvms-0.1.1/spectrally_regularised_LVMs/helper_methods.py` & `spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/helper_methods.py`

 * *Files identical despite different names*

### Comparing `spectrally_regularised_lvms-0.1.1/spectrally_regularised_LVMs/negen_approx.py` & `spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/negen_approx.py`

 * *Files identical despite different names*

### Comparing `spectrally_regularised_lvms-0.1.1/spectrally_regularised_LVMs/spectral_regulariser.py` & `spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/spectral_regulariser.py`

 * *Files identical despite different names*

### Comparing `spectrally_regularised_lvms-0.1.1/spectrally_regularised_LVMs/spectrally_regularised_model.py` & `spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/spectrally_regularised_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,21 +273,14 @@
             hessian_update_type.lower()
         )  # Type of jacobian update
         self.use_ls = use_ls
         self.use_hessian = use_hessian
         self.save_dir = save_dir
         self.verbose = verbose
 
-        # Initialise the processor instance  (could be in base class except for var_PCA)
-        self.processor_inst = DataProcessor(self.whiten, self.var_PCA)
-
-        if self.perform_gso:
-            # Initialise the orthogonalisation instance (could be in base class)
-            self.gs_inst = DeflationOrthogonalisation()
-
         # Sequential unconstrained minimisation technique parameters
         if self.sumt_flag:
             if self.sumt_parameters is None:  # Initialise
                 self.sumt_parameters = {
                     "alpha_init": 0.1,
                     "alpha_end": 100,
                     "alpha_multiplier": 10,
@@ -316,15 +309,28 @@
             )
 
         if type(self.n_sources) != int:
             print("Please enter in a valid number of sources.")
             raise SystemExit
 
         if not self.whiten:
-            print("Non-whitened version is chosen.")
+            if self.cost_instance.__class__.__name__ == "NegentropyCost":
+                print("As negentropy loss is used, whitening is automatically applied.")
+                # For future implementation, this could be adapted.
+                self.whiten = True
+
+            else:
+                print("Non-whitened version is chosen.")
+
+        # Initialise the processor instance  (could be in base class except for var_PCA)
+        self.processor_inst = DataProcessor(self.whiten, self.var_PCA)
+
+        if self.perform_gso:
+            # Initialise the orthogonalisation instance (could be in base class)
+            self.gs_inst = DeflationOrthogonalisation()
 
     def kurtosis(self, y):
         """
 
         Parameters
         ----------
         y : ndarray
@@ -1229,18 +1235,14 @@
     ):
         """
         This method follows the scikit-learn API call and estimates the model parameters
         based off the users initialisation choices.
 
         Parameters
         ----------
-        This method estimates the model parameters for some given X, W, and Lambda.
-
-        Parameters
-        ----------
         X : ndarray
             The data matrix X.
 
         n_iters : int
                         The max number of iterations that are to be performed for each
                         source.
```

