# Comparing `tmp/hgdl-2.1.0.tar.gz` & `tmp/hgdl-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgdl-2.1.0.tar", last modified: Fri May 19 22:24:01 2023, max compression
+gzip compressed data, was "hgdl-2.1.1.tar", last modified: Fri Jun 30 20:55:13 2023, max compression
```

## Comparing `hgdl-2.1.0.tar` & `hgdl-2.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:24:01.255931 hgdl-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-19 22:23:52.000000 hgdl-2.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-19 22:23:52.000000 hgdl-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-19 22:23:52.000000 hgdl-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-19 22:24:01.255931 hgdl-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-19 22:23:52.000000 hgdl-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:24:01.255931 hgdl-2.1.0/hgdl/
--rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-19 22:24:01.255931 hgdl-2.1.0/hgdl/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:24:01.255931 hgdl-2.1.0/hgdl/global_methods/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/global_methods/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2611 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/global_methods/global_optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16288 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/hgdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:24:01.255931 hgdl-2.1.0/hgdl/local_methods/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/local_methods/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2545 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/local_methods/bump_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1290 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/local_methods/dNewton.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4466 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/local_methods/local_optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/meta_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/misc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4107 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/optima.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/support_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:24:01.255931 hgdl-2.1.0/hgdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-19 22:24:01.000000 hgdl-2.1.0/hgdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-19 22:24:01.000000 hgdl-2.1.0/hgdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:24:01.000000 hgdl-2.1.0/hgdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 22:24:01.000000 hgdl-2.1.0/hgdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 22:24:01.000000 hgdl-2.1.0/hgdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-19 22:24:01.255931 hgdl-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2363 2023-05-19 22:23:52.000000 hgdl-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:24:01.255931 hgdl-2.1.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-05-19 22:23:52.000000 hgdl-2.1.0/tests/test_non_diff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1659 2023-05-19 22:23:52.000000 hgdl-2.1.0/tests/test_rosenbrock.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-05-19 22:23:52.000000 hgdl-2.1.0/tests/test_schwefel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1146 2023-05-19 22:23:52.000000 hgdl-2.1.0/tests/test_schwefel_BFGS.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1117 2023-05-19 22:23:52.000000 hgdl-2.1.0/tests/test_schwefel_CG.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-19 22:23:52.000000 hgdl-2.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:55:13.987814 hgdl-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-30 20:55:03.000000 hgdl-2.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-30 20:55:03.000000 hgdl-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 20:55:03.000000 hgdl-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-30 20:55:13.987814 hgdl-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-30 20:55:03.000000 hgdl-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:55:13.987814 hgdl-2.1.1/hgdl/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-06-30 20:55:03.000000 hgdl-2.1.1/hgdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-30 20:55:13.987814 hgdl-2.1.1/hgdl/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:55:13.983814 hgdl-2.1.1/hgdl/global_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:55:03.000000 hgdl-2.1.1/hgdl/global_methods/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2611 2023-06-30 20:55:03.000000 hgdl-2.1.1/hgdl/global_methods/global_optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16297 2023-06-30 20:55:03.000000 hgdl-2.1.1/hgdl/hgdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:55:13.983814 hgdl-2.1.1/hgdl/local_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:55:03.000000 hgdl-2.1.1/hgdl/local_methods/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2545 2023-06-30 20:55:03.000000 hgdl-2.1.1/hgdl/local_methods/bump_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1289 2023-06-30 20:55:03.000000 hgdl-2.1.1/hgdl/local_methods/dNewton.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4528 2023-06-30 20:55:03.000000 hgdl-2.1.1/hgdl/local_methods/local_optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-06-30 20:55:03.000000 hgdl-2.1.1/hgdl/meta_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-06-30 20:55:03.000000 hgdl-2.1.1/hgdl/misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4095 2023-06-30 20:55:03.000000 hgdl-2.1.1/hgdl/optima.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-06-30 20:55:03.000000 hgdl-2.1.1/hgdl/support_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:55:13.983814 hgdl-2.1.1/hgdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-30 20:55:13.000000 hgdl-2.1.1/hgdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-30 20:55:13.000000 hgdl-2.1.1/hgdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:55:13.000000 hgdl-2.1.1/hgdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-30 20:55:13.000000 hgdl-2.1.1/hgdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 20:55:13.000000 hgdl-2.1.1/hgdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-30 20:55:13.987814 hgdl-2.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2363 2023-06-30 20:55:03.000000 hgdl-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:55:13.987814 hgdl-2.1.1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-06-30 20:55:03.000000 hgdl-2.1.1/tests/test_non_diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1659 2023-06-30 20:55:03.000000 hgdl-2.1.1/tests/test_rosenbrock.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-06-30 20:55:03.000000 hgdl-2.1.1/tests/test_schwefel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1146 2023-06-30 20:55:03.000000 hgdl-2.1.1/tests/test_schwefel_BFGS.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1117 2023-06-30 20:55:03.000000 hgdl-2.1.1/tests/test_schwefel_CG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-06-30 20:55:03.000000 hgdl-2.1.1/versioneer.py
```

### Comparing `hgdl-2.1.0/LICENSE` & `hgdl-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/PKG-INFO` & `hgdl-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgdl
-Version: 2.1.0
+Version: 2.1.1
 Summary: HGDL Optimization
 Home-page: https://github.com//hgdl
 Author: David Perryman, Marcus Noack
 Author-email: MarcusNoack@lbl.gov
 License: BSD3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `hgdl-2.1.0/README.md` & `hgdl-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/hgdl/global_methods/global_optimizer.py` & `hgdl-2.1.1/hgdl/global_methods/global_optimizer.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/hgdl/hgdl.py` & `hgdl-2.1.1/hgdl/hgdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         optimization takes place.
     bounds : np.ndarray
         The bounds of the domain; an np.ndarray of shape (D x 2), where D is the
         dimensionality of the space in which the
         optimization takes place. Here D is the dimension of the input domain.
     hess : Callable, optional
         The Hessian of the function to be MINIMIZED. A callable that accepts an 
-    np.ndarray and optional arguments, and returns a
+        np.ndarray and optional arguments, and returns a
         np.ndarray of shape (D x D). The default value is no-op.
     num_epochs : int, optional
         The number of epochs the algorithm runs through before being terminated.
         One epoch is the convergence of all local walkers,
         the deflation of the identified optima, and the global replacement of the 
         walkers. Note, the algorithm is running asynchronously, so a high number
         of epochs can be chosen without concerns, it will not affect the run time 
@@ -95,15 +95,15 @@
         The number of iterations before local optimizations are terminated. 
         The default is 1000.
         It can be lowered when second-order local optimizers are used.
     args : tuple, optional
         A tuple of arguments that will be communicated to the function, 
         the gradient, and the Hessian callables.
         Default = ().
-    constr : object, optional
+    constraints : object, optional
         An optional n-tuple of constraint objects.
         The default is no constraints (). Constraints are defined following 
         scipy.optimize.NonlinearConstraint.
 
     Attributes
     ----------
     optima : object
@@ -149,15 +149,15 @@
 
     ###########################################################################
     ###########################################################################
     ############USER FUNCTIONS#################################################
     ###########################################################################
     ###########################################################################
     ###########################################################################
-    def optimize(self, dask_client=None, x0=None, tolerance=1e-6):
+    def optimize(self, dask_client=None, x0=None, tolerance=1e-8):
         """
         Function to start the optimization. Note, this function will not 
         return anything. Use the method hgdl.HGDL.get_latest() 
         (non-blocking) or hgdl.HGDL.get_final() (blocking)
         to query results.
 
         Parameters
```

### Comparing `hgdl-2.1.0/hgdl/local_methods/bump_function.py` & `hgdl-2.1.1/hgdl/local_methods/bump_function.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/hgdl/local_methods/dNewton.py` & `hgdl-2.1.1/hgdl/local_methods/dNewton.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 from loguru import logger
-
 from .. import misc
 
 
 def DNewton(func, grad, hess, bounds, x0, max_iter, tol, *args):
     e = np.inf
     gradient = np.ones((len(x0))) * np.inf
     counter = 0
```

### Comparing `hgdl-2.1.0/hgdl/local_methods/local_optimizer.py` & `hgdl-2.1.1/hgdl/local_methods/local_optimizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from distributed import get_client
 from loguru import logger
 from scipy.optimize import minimize
 
 from . import bump_function as defl
 from .. import misc
-from . import dNewton as DNewton
+from .dNewton import DNewton as DNewton
 
 
 def run_local(d, optima, x0):
     x_defl, f_defl, radii = optima.get_deflation_points(len(optima.list))
     return run_local_optimizer(d, x0, x_defl, radii)
 
 
@@ -64,15 +64,15 @@
 
 
 def local_method(data, method="dNewton"):
     from functools import partial
     d = data["d"]
     x0 = np.array(data["x0"])
     e = np.inf
-    local_success = True
+    local_success = False
     tol = d.tolerance
     x_defl = data["x_defl"]
     r_defl = data["radius"]
     bounds = d.bounds
     max_iter = d.local_max_iter
     args = d.args
     method = d.local_optimizer
@@ -80,41 +80,43 @@
     # augment grad, hess
     grad = partial(defl.deflated_grad, grad_func=d.grad, x_defl=x_defl, radius=r_defl)
     hess = partial(defl.deflated_hess, grad_func=d.grad, hess_func=d.hess, x_defl=x_defl, radius=r_defl)
 
     # call local methods
     if method == "dNewton":
         x, f, g, eig, local_success = DNewton(d.func, grad, hess, bounds, x0, max_iter, tol, *args)
-        # f = d.func(x,*args)
-        r = 1. / np.min(eig)
+        if np.linalg.norm(g) < 1e-3:
+            local_success = True
+            r = 1. / np.min(eig)
+        else:
+            eig = np.array([0.0])
+            r = 0.0
 
     elif type(method) == str:
-        res = minimize(d.func, x0, args=args, method=method, jac=grad, hess=hess, bounds=bounds, constraints=constr,
-                       options={"disp": False})
+        res = minimize(d.func, x0, args=args, method=method, jac=grad, hess=hess,
+              bounds=bounds, constraints=constr, tol = tol, options={"disp": False})
         x = res["x"]
         f = res["fun"]
         g = res["jac"]
 
-        local_success = False
-        if np.linalg.norm(g) < 1e-5:
+        if np.linalg.norm(g) < 1e-3:
             local_success = True
             eig = np.linalg.eig(hess(x, *args))[0]
             r = 1. / np.min(eig)
         else:
             eig = np.array([0.0])
             r = 0.0
 
 
     elif callable(method):
         res = method(d.func, grad, hess, bounds, x0, *args)
         x = res["x"]
         f = res["fun"]
         g = res["jac"]
-        local_success = False
-        if np.linalg.norm(g) < 1e-5:
+        if np.linalg.norm(g) < 1e-3:
             local_success = True
             eig = np.linalg.eig(hess(x, *args))[0]
             r = 1. / np.min(eig)
         else:
             eig = np.array([0.0])
             r = 0.0
```

### Comparing `hgdl-2.1.0/hgdl/meta_data.py` & `hgdl-2.1.1/hgdl/meta_data.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/hgdl/misc.py` & `hgdl-2.1.1/hgdl/misc.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/hgdl/optima.py` & `hgdl-2.1.1/hgdl/optima.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         clean_f = f[clean_indices]
         clean_g = g[clean_indices]
         clean_eig = eig[clean_indices]
         clean_radii = r[clean_indices]
         classifier = []
         ##making the classifier
         for i in range(len(clean_x)):
-            if any(clean_g[i] > 1e-5):
+            if any(clean_g[i] > 1e-3):
                 classifier.append("degenerate")
             elif any(abs(clean_eig[i]) < 10e-6):
                 classifier.append("zero curvature")
             elif all(clean_eig[i] > 0.0):
                 classifier.append("minimum")
             elif all(clean_eig[i] < 0.0):
                 classifier.append("maximum")
@@ -63,16 +63,15 @@
         new_optima_list = []
         for i in range(len(clean_x)):
             new_optima_list.append(
                 self.make_optima_list_entry(clean_x[i], clean_f[i], classifier[i], clean_eig[i], clean_g[i],
                                             np.linalg.norm(clean_g[i]), clean_radii[i]))
         optima_list = self.list + new_optima_list
 
-        def find_f(d):
-            return d["f(x)"]
+        def find_f(d): return d["f(x)"]
 
         optima_list.sort(key=find_f)
         self.list = optima_list[0:self.max_optima]
         return self.list
 
     def get_minima(self, n):
         try:
```

### Comparing `hgdl-2.1.0/hgdl/support_functions.py` & `hgdl-2.1.1/hgdl/support_functions.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/hgdl.egg-info/PKG-INFO` & `hgdl-2.1.1/hgdl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgdl
-Version: 2.1.0
+Version: 2.1.1
 Summary: HGDL Optimization
 Home-page: https://github.com//hgdl
 Author: David Perryman, Marcus Noack
 Author-email: MarcusNoack@lbl.gov
 License: BSD3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `hgdl-2.1.0/hgdl.egg-info/SOURCES.txt` & `hgdl-2.1.1/hgdl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/setup.py` & `hgdl-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/tests/test_non_diff.py` & `hgdl-2.1.1/tests/test_non_diff.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/tests/test_rosenbrock.py` & `hgdl-2.1.1/tests/test_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/tests/test_schwefel.py` & `hgdl-2.1.1/tests/test_schwefel.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/tests/test_schwefel_BFGS.py` & `hgdl-2.1.1/tests/test_schwefel_BFGS.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/tests/test_schwefel_CG.py` & `hgdl-2.1.1/tests/test_schwefel_CG.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.1.0/versioneer.py` & `hgdl-2.1.1/versioneer.py`

 * *Files identical despite different names*

