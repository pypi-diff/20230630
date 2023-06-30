# Comparing `tmp/skglm-0.2.tar.gz` & `tmp/skglm-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skglm-0.2.tar", last modified: Tue Oct 18 08:57:40 2022, max compression
+gzip compressed data, was "skglm-0.3.tar", last modified: Fri Jun 30 14:20:10 2023, max compression
```

## Comparing `skglm-0.2.tar` & `skglm-0.3.tar`

### file list

```diff
@@ -1,42 +1,54 @@
-drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2022-10-18 08:57:40.402078 skglm-0.2/
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1527 2022-08-25 11:28:36.000000 skglm-0.2/LICENSE
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     3059 2022-10-18 08:57:40.402078 skglm-0.2/PKG-INFO
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     2718 2022-08-25 11:28:36.000000 skglm-0.2/README.rst
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)       38 2022-10-18 08:57:40.402078 skglm-0.2/setup.cfg
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1177 2022-08-25 11:28:36.000000 skglm-0.2/setup.py
-drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2022-10-18 08:57:40.398077 skglm-0.2/skglm/
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)      204 2022-10-18 08:57:01.000000 skglm-0.2/skglm/__init__.py
-drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2022-10-18 08:57:40.398077 skglm-0.2/skglm/datafits/
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)      357 2022-10-12 06:51:56.000000 skglm-0.2/skglm/datafits/__init__.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     7109 2022-08-25 11:28:36.000000 skglm-0.2/skglm/datafits/base.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     2132 2022-10-10 16:51:18.000000 skglm-0.2/skglm/datafits/group.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     3306 2022-10-18 08:56:26.000000 skglm-0.2/skglm/datafits/multi_task.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    12781 2022-10-12 06:51:56.000000 skglm-0.2/skglm/datafits/single_task.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    45219 2022-10-12 06:51:56.000000 skglm-0.2/skglm/estimators.py
-drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2022-10-18 08:57:40.398077 skglm-0.2/skglm/experimental/
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)       64 2022-10-12 06:51:56.000000 skglm-0.2/skglm/experimental/__init__.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1049 2022-10-18 08:56:20.000000 skglm-0.2/skglm/experimental/_plot_sqrt_lasso.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     7243 2022-10-18 08:56:26.000000 skglm-0.2/skglm/experimental/sqrt_lasso.py
-drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2022-10-18 08:57:40.398077 skglm-0.2/skglm/penalties/
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)      392 2022-10-10 16:51:18.000000 skglm-0.2/skglm/penalties/__init__.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1721 2022-08-30 14:35:40.000000 skglm-0.2/skglm/penalties/base.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    11258 2022-08-25 11:28:36.000000 skglm-0.2/skglm/penalties/block_separable.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    15400 2022-08-25 11:28:36.000000 skglm-0.2/skglm/penalties/separable.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     2230 2022-04-14 08:49:05.000000 skglm-0.2/skglm/plot_utils.py
-drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2022-10-18 08:57:40.398077 skglm-0.2/skglm/solvers/
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)      282 2022-10-10 16:51:18.000000 skglm-0.2/skglm/solvers/__init__.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    12955 2022-09-09 04:37:02.000000 skglm-0.2/skglm/solvers/accelerated_cd.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    13002 2022-10-10 16:51:18.000000 skglm-0.2/skglm/solvers/anderson_cd.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1035 2022-10-10 16:51:18.000000 skglm-0.2/skglm/solvers/base.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     2658 2022-08-25 11:28:36.000000 skglm-0.2/skglm/solvers/common.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     5472 2022-10-10 16:51:18.000000 skglm-0.2/skglm/solvers/gram_cd.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     6292 2022-10-10 16:51:18.000000 skglm-0.2/skglm/solvers/group_bcd.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    14782 2022-10-18 08:56:26.000000 skglm-0.2/skglm/solvers/multitask_bcd.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    15364 2022-10-18 08:56:26.000000 skglm-0.2/skglm/solvers/prox_newton.py
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    14092 2022-10-12 06:51:56.000000 skglm-0.2/skglm/utils.py
-drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2022-10-18 08:57:40.398077 skglm-0.2/skglm.egg-info/
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     3059 2022-10-18 08:57:40.000000 skglm-0.2/skglm.egg-info/PKG-INFO
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)      841 2022-10-18 08:57:40.000000 skglm-0.2/skglm.egg-info/SOURCES.txt
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)        1 2022-10-18 08:57:40.000000 skglm-0.2/skglm.egg-info/dependency_links.txt
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)       50 2022-10-18 08:57:40.000000 skglm-0.2/skglm.egg-info/requires.txt
--rw-rw-r--   0 mathurin  (1000) mathurin  (1000)        6 2022-10-18 08:57:40.000000 skglm-0.2/skglm.egg-info/top_level.txt
+drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2023-06-30 14:20:10.007534 skglm-0.3/
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1527 2023-05-31 13:14:00.000000 skglm-0.3/LICENSE
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     5413 2023-06-30 14:20:10.007534 skglm-0.3/PKG-INFO
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     5032 2023-06-30 13:37:13.000000 skglm-0.3/README.md
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)       38 2023-06-30 14:20:10.007534 skglm-0.3/setup.cfg
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1247 2023-03-08 12:14:18.000000 skglm-0.3/setup.py
+drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2023-06-30 14:20:09.999534 skglm-0.3/skglm/
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)      218 2023-06-30 14:19:56.000000 skglm-0.3/skglm/__init__.py
+drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2023-06-30 14:20:09.999534 skglm-0.3/skglm/datafits/
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)      411 2023-05-31 13:14:00.000000 skglm-0.3/skglm/datafits/__init__.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     7109 2022-08-25 11:28:36.000000 skglm-0.3/skglm/datafits/base.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     4015 2023-04-18 07:31:03.000000 skglm-0.3/skglm/datafits/group.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     3318 2023-04-18 07:31:03.000000 skglm-0.3/skglm/datafits/multi_task.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    25199 2023-06-30 07:46:13.000000 skglm-0.3/skglm/datafits/single_task.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    52348 2023-06-30 13:37:13.000000 skglm-0.3/skglm/estimators.py
+drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2023-06-30 14:20:10.003534 skglm-0.3/skglm/experimental/
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)      267 2023-06-30 13:37:13.000000 skglm-0.3/skglm/experimental/__init__.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1054 2022-12-07 12:44:33.000000 skglm-0.3/skglm/experimental/_plot_sqrt_lasso.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     8052 2023-04-18 07:31:03.000000 skglm-0.3/skglm/experimental/pdcd_ws.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     2242 2023-04-18 07:31:03.000000 skglm-0.3/skglm/experimental/quantile_regression.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     3214 2023-04-18 07:31:03.000000 skglm-0.3/skglm/experimental/reweighted.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     7773 2023-06-30 13:37:13.000000 skglm-0.3/skglm/experimental/sqrt_lasso.py
+drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2023-06-30 14:20:10.003534 skglm-0.3/skglm/penalties/
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)      485 2023-06-13 09:46:30.000000 skglm-0.3/skglm/penalties/__init__.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1721 2022-08-30 14:35:40.000000 skglm-0.3/skglm/penalties/base.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    11445 2023-04-18 07:31:03.000000 skglm-0.3/skglm/penalties/block_separable.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1737 2023-06-30 07:46:13.000000 skglm-0.3/skglm/penalties/non_separable.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    19846 2023-06-13 09:46:30.000000 skglm-0.3/skglm/penalties/separable.py
+drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2023-06-30 14:20:10.003534 skglm-0.3/skglm/solvers/
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)      421 2023-06-13 09:46:30.000000 skglm-0.3/skglm/solvers/__init__.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    13011 2022-12-07 12:44:33.000000 skglm-0.3/skglm/solvers/anderson_cd.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1035 2022-10-27 11:07:01.000000 skglm-0.3/skglm/solvers/base.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     2658 2022-08-25 11:28:36.000000 skglm-0.3/skglm/solvers/common.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     4169 2023-06-30 07:46:13.000000 skglm-0.3/skglm/solvers/fista.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     5536 2023-04-18 07:31:03.000000 skglm-0.3/skglm/solvers/gram_cd.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     6335 2022-12-07 12:44:33.000000 skglm-0.3/skglm/solvers/group_bcd.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    13016 2022-12-07 12:44:33.000000 skglm-0.3/skglm/solvers/group_prox_newton.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     3122 2023-06-30 07:46:13.000000 skglm-0.3/skglm/solvers/lbfgs.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    14782 2022-11-04 08:17:26.000000 skglm-0.3/skglm/solvers/multitask_bcd.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)    16014 2023-06-30 07:46:13.000000 skglm-0.3/skglm/solvers/prox_newton.py
+drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2023-06-30 14:20:10.007534 skglm-0.3/skglm/utils/
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)        0 2022-12-07 12:44:33.000000 skglm-0.3/skglm/utils/__init__.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1432 2022-12-07 12:44:33.000000 skglm-0.3/skglm/utils/anderson.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     8857 2023-06-21 14:12:21.000000 skglm-0.3/skglm/utils/data.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     2073 2022-12-07 12:44:33.000000 skglm-0.3/skglm/utils/jit_compilation.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     5255 2022-12-07 12:44:33.000000 skglm-0.3/skglm/utils/prox_funcs.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     2889 2023-06-30 07:46:13.000000 skglm-0.3/skglm/utils/sparse_ops.py
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)      714 2022-12-07 12:44:33.000000 skglm-0.3/skglm/utils/validation.py
+drwxrwxr-x   0 mathurin  (1000) mathurin  (1000)        0 2023-06-30 14:20:09.999534 skglm-0.3/skglm.egg-info/
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     5413 2023-06-30 14:20:09.000000 skglm-0.3/skglm.egg-info/PKG-INFO
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)     1169 2023-06-30 14:20:09.000000 skglm-0.3/skglm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)        1 2023-06-30 14:20:09.000000 skglm-0.3/skglm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)       50 2023-06-30 14:20:09.000000 skglm-0.3/skglm.egg-info/requires.txt
+-rw-rw-r--   0 mathurin  (1000) mathurin  (1000)        6 2023-06-30 14:20:09.000000 skglm-0.3/skglm.egg-info/top_level.txt
```

### Comparing `skglm-0.2/LICENSE` & `skglm-0.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, scikit-learn-contrib
+Copyright (c) 2023, scikit-learn-contrib
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `skglm-0.2/setup.py` & `skglm-0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,27 +9,28 @@
             version = line.split('=')[1].strip().strip('\'')
             break
 if version is None:
     raise RuntimeError('Could not determine version')
 
 DISTNAME = 'skglm'
 DESCRIPTION = 'A fast and modular scikit-learn replacement for generalized linear models'
-with open('README.rst', 'r') as f:
+with open('README.md', 'r', encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 MAINTAINER = 'Mathurin Massias'
 MAINTAINER_EMAIL = 'mathurin.massias@gmail.com'
 LICENSE = 'BSD (3-clause)'
 DOWNLOAD_URL = 'https://github.com/scikit-learn-contrib/skglm.git'
 VERSION = version
 URL = 'https://contrib.scikit-learn.org/skglm'
 
 setup(name=DISTNAME,
       version=version,
       description=DESCRIPTION,
       long_description=LONG_DESCRIPTION,
+      long_description_content_type='text/markdown',
       maintainer=MAINTAINER,
       maintainer_email=MAINTAINER_EMAIL,
       url=URL,
       download_url=DOWNLOAD_URL,
       packages=find_packages(),
       install_requires=['numpy>=1.12', 'numba',
                         'scipy>=0.18.0', 'scikit-learn>=1.0']
```

### Comparing `skglm-0.2/skglm/datafits/base.py` & `skglm-0.3/skglm/datafits/base.py`

 * *Files identical despite different names*

### Comparing `skglm-0.2/skglm/datafits/group.py` & `skglm-0.3/skglm/datafits/group.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import numpy as np
 from numpy.linalg import norm
 from numba import int32, float64
 
 from skglm.datafits.base import BaseDatafit
+from skglm.datafits.single_task import Logistic
 
 
 class QuadraticGroup(BaseDatafit):
     r"""Quadratic datafit used with group penalties.
 
-    The datafit reads::
+    The datafit reads:
 
-    (1 / (2 * n_samples)) * ||y - X w||^2_2
+    .. math:: 1 / (2 xx n_"samples") ||y - Xw||_2 ^ 2
 
     Attributes
     ----------
     grp_indices : array, shape (n_features,)
         The group indices stacked contiguously
         ([grp1_indices, grp2_indices, ...]).
 
@@ -67,7 +68,67 @@
         return grad_g
 
     def gradient_scalar(self, X, y, w, Xw, j):
         return X[:, j] @ (Xw - y) / len(y)
 
     def intercept_update_step(self, y, Xw):
         return np.mean(Xw - y)
+
+
+class LogisticGroup(Logistic):
+    r"""Logistic datafit used with group penalties.
+
+    The datafit reads:
+
+    .. math:: 1 / n_"samples" sum_(i=1)^(n_"samples") log(1 + exp(-y_i (Xw)_i))
+
+    Attributes
+    ----------
+    grp_indices : array, shape (n_features,)
+        The group indices stacked contiguously
+        ``[grp1_indices, grp2_indices, ...]``.
+
+    grp_ptr : array, shape (n_groups + 1,)
+        The group pointers such that two consecutive elements delimit
+        the indices of a group in ``grp_indices``.
+
+    lipschitz : array, shape (n_groups,)
+        The lipschitz constants for each group.
+    """
+
+    def __init__(self, grp_ptr, grp_indices):
+        self.grp_ptr, self.grp_indices = grp_ptr, grp_indices
+
+    def get_spec(self):
+        spec = (
+            ('grp_ptr', int32[:]),
+            ('grp_indices', int32[:]),
+            ('lipschitz', float64[:])
+        )
+        return spec
+
+    def params_to_dict(self):
+        return dict(grp_ptr=self.grp_ptr,
+                    grp_indices=self.grp_indices)
+
+    def initialize(self, X, y):
+        grp_ptr, grp_indices = self.grp_ptr, self.grp_indices
+        n_groups = len(grp_ptr) - 1
+
+        lipschitz = np.zeros(n_groups)
+        for g in range(n_groups):
+            grp_g_indices = grp_indices[grp_ptr[g]: grp_ptr[g+1]]
+            X_g = X[:, grp_g_indices]
+            lipschitz[g] = norm(X_g, ord=2) ** 2 / (4 * len(y))
+
+        self.lipschitz = lipschitz
+
+    def gradient_g(self, X, y, w, Xw, g):
+        grp_ptr, grp_indices = self.grp_ptr, self.grp_indices
+        grp_g_indices = grp_indices[grp_ptr[g]: grp_ptr[g+1]]
+        raw_grad_val = self.raw_grad(y, Xw)
+
+        grad_g = np.zeros(len(grp_g_indices))
+        for idx, j in enumerate(grp_g_indices):
+            grad_g[idx] = X[:, j] @ raw_grad_val
+
+        return grad_g
```

### Comparing `skglm-0.2/skglm/datafits/multi_task.py` & `skglm-0.3/skglm/datafits/multi_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 from skglm.datafits.base import BaseMultitaskDatafit
 
 
 class QuadraticMultiTask(BaseMultitaskDatafit):
     """Quadratic datafit used for multi-task regression.
 
-    The datafit reads::
+    The datafit reads:
 
-    (1 / (2 * n_samples)) * ||Y - X W||^2_F
+    .. math: 1 / (2 xx n_"samples") ||Y - XW||_F ^ 2
 
     Attributes
     ----------
     XtY : array, shape (n_features, n_tasks)
         Pre-computed quantity used during the gradient evaluation.
 
     lipschitz : array, shape (n_features,)
         The coordinatewise gradient Lipschitz constants. Equal to
-        norm(X, axis=0) ** 2 / n_samples.
+        ``norm(X, axis=0) ** 2 / n_samples``.
     """
 
     def __init__(self):
         pass
 
     def get_spec(self):
         spec = (
```

### Comparing `skglm-0.2/skglm/estimators.py` & `skglm-0.3/skglm/estimators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # License: BSD 3 clause
 
 import warnings
 import numpy as np
 from scipy.sparse import issparse
 from scipy.special import expit
-from skglm.solvers.prox_newton import ProxNewton
+from numbers import Integral, Real
+from skglm.solvers import ProxNewton, LBFGS
 
-from sklearn.utils.validation import check_is_fitted
-from sklearn.utils import check_array, check_consistent_length
+from sklearn.utils.validation import (check_is_fitted, check_array,
+                                      check_consistent_length)
 from sklearn.linear_model._base import (
     LinearModel, RegressorMixin,
     LinearClassifierMixin, SparseCoefMixin, BaseEstimator
 )
 from sklearn.utils.extmath import softmax
 from sklearn.preprocessing import LabelEncoder
+from sklearn.utils._param_validation import Interval, StrOptions
 from sklearn.multiclass import OneVsRestClassifier, check_classification_targets
 
-from skglm.utils import compiled_clone
+from skglm.utils.jit_compilation import compiled_clone
 from skglm.solvers import AndersonCD, MultiTaskBCD
-from skglm.datafits import Quadratic, Logistic, QuadraticSVC, QuadraticMultiTask
-from skglm.penalties import L1, WeightedL1, L1_plus_L2, MCPenalty, IndicatorBox, L2_1
+from skglm.datafits import Cox, Quadratic, Logistic, QuadraticSVC, QuadraticMultiTask
+from skglm.penalties import (L1, WeightedL1, L1_plus_L2, L2,
+                             MCPenalty, IndicatorBox, L2_1)
 
 
 def _glm_fit(X, y, model, datafit, penalty, solver):
     is_classif = isinstance(datafit, (Logistic, QuadraticSVC))
     fit_intercept = solver.fit_intercept
 
     if is_classif:
@@ -159,28 +162,30 @@
 
     This estimator takes a penalty and a datafit and runs a coordinate descent solver
     to solve the optimization problem. It handles classification and regression tasks.
 
     Parameters
     ----------
     datafit : instance of BaseDatafit, optional
-        Datafit. If None, `datafit` is initialized as a `Quadratic` datafit.
-        `datafit` is replaced by a JIT-compiled instance when calling fit.
+        Datafit. If ``None``, ``datafit`` is initialized as a :class:`.Quadratic`
+        datafit.  ``datafit`` is replaced by a JIT-compiled instance when calling fit.
 
     penalty : instance of BasePenalty, optional
-        Penalty. If None, `penalty` is initialized as a `L1` penalty.
-        `penalty` is replaced by a JIT-compiled instance when calling fit.
+        Penalty. If ``None``, ``penalty`` is initialized as a :class:`.L1` penalty.
+        ``penalty`` is replaced by a JIT-compiled instance when
+        calling fit.
 
     solver : instance of BaseSolver, optional
-        Solver. If None, `solver` is initialized as an `AndersonCD` solver.
+        Solver. If ``None``, ``solver`` is initialized as an :class:`.AndersonCD`
+        solver.
 
     Attributes
     ----------
     coef_ : array, shape (n_features,) or (n_features, n_tasks)
-        parameter array (w in the cost function formula)
+        parameter array (:math:`w` in the cost function formula)
 
     sparse_coef_ : scipy.sparse matrix, shape (n_features, 1) or (n_features, n_tasks)
         ``sparse_coef_`` is a readonly property derived from ``coef_``
 
     intercept_ : array, shape (n_tasks,)
         constant term in decision function.
 
@@ -228,14 +233,22 @@
 
         stop_crit : array, shape (n_alphas,)
             Value of stopping criterion at convergence along the path.
 
         n_iters : array, shape (n_alphas,), optional
             The number of iterations along the path. If return_n_iter is set to `True`.
         """
+        # TODO: add support for Cox datafit in `_glm_fit`
+        # `_glm_fit` interpret `Cox` as a multitask datafit which breaks down solvers
+        if isinstance(self.datafit, Cox):
+            raise ValueError(
+                "`GeneralizedLinearEstimator` doesn't currently support "
+                "`Cox` datafit"
+            )
+
         self.penalty = self.penalty if self.penalty else L1(1.)
         self.datafit = self.datafit if self.datafit else Quadratic()
         self.solver = self.solver if self.solver else AndersonCD()
 
         return _glm_fit(X, y, self, self.datafit, self.penalty, self.solver)
 
     def predict(self, X):
@@ -286,17 +299,18 @@
             params[p_prefix + p_key] = p_val
         return params
 
 
 class Lasso(LinearModel, RegressorMixin):
     r"""Lasso estimator based on Celer solver and primal extrapolation.
 
-    The optimization objective for Lasso is::
+    The optimization objective for Lasso is:
 
-        (1 / (2 * n_samples)) * ||y - X w||^2_2 + alpha * \sum_j |w_j|
+    .. math::
+        1 / (2 xx n_"samples")  ||y - Xw||_2 ^ 2 + alpha ||w||_1
 
     Parameters
     ----------
     alpha : float, optional
         Penalty strength.
 
     max_iter : int, optional
@@ -310,28 +324,31 @@
 
     verbose : bool or int
         Amount of verbosity.
 
     tol : float, optional
         Stopping criterion for the optimization.
 
+    positive : bool, optional
+        When set to ``True``, forces the coefficient vector to be positive.
+
     fit_intercept : bool, optional (default=True)
         Whether or not to fit an intercept.
 
     warm_start : bool, optional (default=False)
-        When set to True, reuse the solution of the previous call to fit as
+        When set to ``True``, reuse the solution of the previous call to fit as
         initialization, otherwise, just erase the previous solution.
 
     ws_strategy : str
-        The score used to build the working set. Can be ``fixpoint`` or ``subdiff``.
+        The score used to build the working set. Can be ``"fixpoint"`` or ``"subdiff"``.
 
     Attributes
     ----------
     coef_ : array, shape (n_features,)
-        parameter vector (w in the cost function formula)
+        parameter vector (:math:`w` in the cost function formula)
 
     sparse_coef_ : scipy.sparse matrix, shape (n_features, 1)
         ``sparse_coef_`` is a readonly property derived from ``coef_``
 
     intercept_ : float
         constant term in decision function.
 
@@ -341,22 +358,24 @@
     See Also
     --------
     WeightedLasso : Weighted Lasso regularization.
     MCPRegression : Sparser regularization than L1 norm.
     """
 
     def __init__(self, alpha=1., max_iter=50, max_epochs=50_000, p0=10, verbose=0,
-                 tol=1e-4, fit_intercept=True, warm_start=False, ws_strategy="subdiff"):
+                 tol=1e-4, positive=False, fit_intercept=True, warm_start=False,
+                 ws_strategy="subdiff"):
         super().__init__()
         self.alpha = alpha
         self.tol = tol
         self.max_iter = max_iter
         self.max_epochs = max_epochs
         self.p0 = p0
         self.ws_strategy = ws_strategy
+        self.positive = positive
         self.fit_intercept = fit_intercept
         self.warm_start = warm_start
         self.verbose = verbose
 
     def fit(self, X, y):
         """Fit the model according to the given training data.
 
@@ -374,15 +393,15 @@
             Fitted estimator.
         """
         # TODO: Add Gram solver
         solver = AndersonCD(
             self.max_iter, self.max_epochs, self.p0, tol=self.tol,
             ws_strategy=self.ws_strategy, fit_intercept=self.fit_intercept,
             warm_start=self.warm_start, verbose=self.verbose)
-        return _glm_fit(X, y, self, Quadratic(), L1(self.alpha), solver)
+        return _glm_fit(X, y, self, Quadratic(), L1(self.alpha, self.positive), solver)
 
     def path(self, X, y, alphas, coef_init=None, return_n_iter=True, **params):
         """Compute Lasso path.
 
         Parameters
         ----------
         X : array, shape (n_samples, n_features)
@@ -391,15 +410,16 @@
         y : array, shape (n_samples,)
             Target vector.
 
         alphas : array, shape (n_alphas,)
             Grid of alpha.
 
         coef_init : array, shape (n_features,), optional
-            If warm_start is enabled, the optimization problem restarts from coef_init.
+            If warm_start is enabled, the optimization problem restarts from
+            ``coef_init``.
 
         return_n_iter : bool
             Returns the number of iterations along the path.
 
         **params : kwargs
             All parameters supported by path.
 
@@ -411,40 +431,42 @@
         coefs : array, shape (n_features, n_alphas)
             Coefficients along the path.
 
         stop_crit : array, shape (n_alphas,)
             Value of stopping criterion at convergence along the path.
 
         n_iters : array, shape (n_alphas,), optional
-            The number of iterations along the path. If return_n_iter is set to `True`.
+            The number of iterations along the path. If return_n_iter is set to
+            ``True``.
         """
-        penalty = compiled_clone(L1(self.alpha))
+        penalty = compiled_clone(L1(self.alpha, self.positive))
         datafit = compiled_clone(Quadratic(), to_float32=X.dtype == np.float32)
         solver = AndersonCD(
             self.max_iter, self.max_epochs, self.p0, tol=self.tol,
             ws_strategy=self.ws_strategy, fit_intercept=self.fit_intercept,
             warm_start=self.warm_start, verbose=self.verbose)
         return solver.path(X, y, datafit, penalty, alphas, coef_init, return_n_iter)
 
 
 class WeightedLasso(LinearModel, RegressorMixin):
     r"""WeightedLasso estimator based on Celer solver and primal extrapolation.
 
-    The optimization objective for WeightedLasso is::
+    The optimization objective for WeightedLasso is:
 
-        (1 / (2 * n_samples)) * ||y - X w||^2_2 + alpha * \sum_j weights_j |w_j|
+    .. math::
+        1 / (2 xx n_"samples") ||y - Xw||_2 ^ 2 + alpha ||w||_1
 
     Parameters
     ----------
     alpha : float, optional
         Penalty strength.
 
     weights : array, shape (n_features,), optional (default=None)
         Positive weights used in the L1 penalty part of the Lasso
-        objective. If None, weights equal to 1 are used.
+        objective. If ``None``, weights equal to 1 are used.
 
     max_iter : int, optional
         The maximum number of iterations (subproblem definitions).
 
     max_epochs : int
         Maximum number of CD epochs on each subproblem.
 
@@ -453,28 +475,31 @@
 
     verbose : bool or int
         Amount of verbosity.
 
     tol : float, optional
         Stopping criterion for the optimization.
 
+    positive : bool, optional
+        When set to ``True``, forces the coefficient vector to be positive.
+
     fit_intercept : bool, optional (default=True)
         Whether or not to fit an intercept.
 
     warm_start : bool, optional (default=False)
-        When set to True, reuse the solution of the previous call to fit as
+        When set to ``True``, reuse the solution of the previous call to fit as
         initialization, otherwise, just erase the previous solution.
 
     ws_strategy : str
         The score used to build the working set. Can be ``fixpoint`` or ``subdiff``.
 
     Attributes
     ----------
     coef_ : array, shape (n_features,)
-        parameter vector (w in the cost function formula)
+        parameter vector (:math:`w` in the cost function formula)
 
     sparse_coef_ : scipy.sparse matrix, shape (n_features, 1)
         ``sparse_coef_`` is a readonly property derived from ``coef_``
 
     intercept_ : float
         constant term in decision function.
 
@@ -488,24 +513,25 @@
 
     Notes
     -----
     Supports weights equal to 0, i.e. unpenalized features.
     """
 
     def __init__(self, alpha=1., weights=None, max_iter=50, max_epochs=50_000, p0=10,
-                 verbose=0, tol=1e-4, fit_intercept=True, warm_start=False,
-                 ws_strategy="subdiff"):
+                 verbose=0, tol=1e-4, positive=False, fit_intercept=True,
+                 warm_start=False, ws_strategy="subdiff"):
         super().__init__()
         self.alpha = alpha
         self.weights = weights
         self.tol = tol
         self.max_iter = max_iter
         self.max_epochs = max_epochs
         self.p0 = p0
         self.ws_strategy = ws_strategy
+        self.positive = positive
         self.fit_intercept = fit_intercept
         self.warm_start = warm_start
         self.verbose = verbose
 
     def path(self, X, y, alphas, coef_init=None, return_n_iter=True, **params):
         """Compute Weighted Lasso path.
 
@@ -544,15 +570,15 @@
             The number of iterations along the path. If return_n_iter is set to `True`.
         """
         weights = np.ones(X.shape[1]) if self.weights is None else self.weights
         if X.shape[1] != len(weights):
             raise ValueError("The number of weights must match the number of \
                               features. Got %s, expected %s." % (
                 len(weights), X.shape[1]))
-        penalty = compiled_clone(WeightedL1(self.alpha, weights))
+        penalty = compiled_clone(WeightedL1(self.alpha, weights, self.positive))
         datafit = compiled_clone(Quadratic(), to_float32=X.dtype == np.float32)
         solver = AndersonCD(
             self.max_iter, self.max_epochs, self.p0, tol=self.tol,
             ws_strategy=self.ws_strategy, fit_intercept=self.fit_intercept,
             warm_start=self.warm_start, verbose=self.verbose)
         return solver.path(X, y, datafit, penalty, alphas, coef_init, return_n_iter)
 
@@ -570,31 +596,33 @@
         Returns
         -------
         self :
             Fitted estimator.
         """
         if self.weights is None:
             warnings.warn('Weights are not provided, fitting with Lasso penalty')
-            penalty = L1(self.alpha)
+            penalty = L1(self.alpha, self.positive)
         else:
-            penalty = WeightedL1(self.alpha, self.weights)
+            penalty = WeightedL1(self.alpha, self.weights, self.positive)
         solver = AndersonCD(
             self.max_iter, self.max_epochs, self.p0, tol=self.tol,
             ws_strategy=self.ws_strategy, fit_intercept=self.fit_intercept,
             warm_start=self.warm_start, verbose=self.verbose)
         return _glm_fit(X, y, self, Quadratic(), penalty, solver)
 
 
 class ElasticNet(LinearModel, RegressorMixin):
     r"""Elastic net estimator.
 
-    The optimization objective for Elastic net is::
+    The optimization objective for Elastic net is:
 
-        (1 / (2 * n_samples)) * ||y - X w||^2_2 + l1_ratio * alpha * sum_j |w_j| \
-        + (1 - l1_ratio) * alpha / 2 sum_j w_j ** 2
+    .. math::
+        1 / (2 xx n_"samples") ||y - Xw||_2 ^ 2
+        + tt"l1_ratio" xx alpha ||w||_1
+        + (1 - tt"l1_ratio") xx alpha/2 ||w||_2 ^ 2
 
     Parameters
     ----------
     alpha : float, optional
         Penalty strength.
 
     l1_ratio : float, default=0.5
@@ -614,28 +642,31 @@
 
     verbose : bool or int
         Amount of verbosity.
 
     tol : float, optional
         Stopping criterion for the optimization.
 
+    positive : bool, optional
+        When set to ``True``, forces the coefficient vector to be positive.
+
     fit_intercept : bool, optional (default=True)
         Whether or not to fit an intercept.
 
     warm_start : bool, optional (default=False)
-        When set to True, reuse the solution of the previous call to fit as
+        When set to ``True``, reuse the solution of the previous call to fit as
         initialization, otherwise, just erase the previous solution.
 
     ws_strategy : str
         The score used to build the working set. Can be ``fixpoint`` or ``subdiff``.
 
     Attributes
     ----------
     coef_ : array, shape (n_features,)
-        parameter vector (w in the cost function formula)
+        parameter vector (:math:`w` in the cost function formula)
 
     sparse_coef_ : scipy.sparse matrix, shape (n_features, 1)
         ``sparse_coef_`` is a readonly property derived from ``coef_``
 
     intercept_ : float
         constant term in decision function.
 
@@ -644,25 +675,26 @@
 
     See Also
     --------
     Lasso : Lasso regularization.
     """
 
     def __init__(self, alpha=1., l1_ratio=0.5, max_iter=50, max_epochs=50_000, p0=10,
-                 verbose=0, tol=1e-4, fit_intercept=True, warm_start=False,
-                 ws_strategy="subdiff"):
+                 verbose=0, tol=1e-4, positive=False, fit_intercept=True,
+                 warm_start=False, ws_strategy="subdiff"):
         super().__init__()
         self.alpha = alpha
         self.l1_ratio = l1_ratio
         self.tol = tol
         self.max_iter = max_iter
         self.max_epochs = max_epochs
         self.p0 = p0
         self.ws_strategy = ws_strategy
         self.fit_intercept = fit_intercept
+        self.positive = positive
         self.warm_start = warm_start
         self.verbose = verbose
 
     def path(self, X, y, alphas, coef_init=None, return_n_iter=True, **params):
         """Compute Elastic Net path.
 
         Parameters
@@ -693,17 +725,18 @@
         coefs : array, shape (n_features, n_alphas)
             Coefficients along the path.
 
         stop_crit : array, shape (n_alphas,)
             Value of stopping criterion at convergence along the path.
 
         n_iters : array, shape (n_alphas,), optional
-            The number of iterations along the path. If return_n_iter is set to `True`.
+            The number of iterations along the path. If return_n_iter is set to
+            ``True``.
         """
-        penalty = compiled_clone(L1_plus_L2(self.alpha, self.l1_ratio))
+        penalty = compiled_clone(L1_plus_L2(self.alpha, self.l1_ratio, self.positive))
         datafit = compiled_clone(Quadratic(), to_float32=X.dtype == np.float32)
         solver = AndersonCD(
             self.max_iter, self.max_epochs, self.p0, tol=self.tol,
             ws_strategy=self.ws_strategy, fit_intercept=self.fit_intercept,
             warm_start=self.warm_start, verbose=self.verbose)
         return solver.path(X, y, datafit, penalty, alphas, coef_init, return_n_iter)
 
@@ -724,39 +757,43 @@
             Fitted estimator.
         """
         solver = AndersonCD(
             self.max_iter, self.max_epochs, self.p0, tol=self.tol,
             ws_strategy=self.ws_strategy, fit_intercept=self.fit_intercept,
             warm_start=self.warm_start, verbose=self.verbose)
         return _glm_fit(X, y, self, Quadratic(),
-                        L1_plus_L2(self.alpha, self.l1_ratio), solver)
+                        L1_plus_L2(self.alpha, self.l1_ratio, self.positive), solver)
 
 
 class MCPRegression(LinearModel, RegressorMixin):
     r"""Linear regression with MCP penalty estimator.
 
-    The optimization objective for MCPRegression is, with x >= 0::
+    The optimization objective for MCPRegression is, with :math:`x >= 0`:
 
-        pen(x) = alpha * x - x^2 / (2 * gamma) if x =< gamma * alpha
-                 gamma * alpha ** 2 / 2        if x > gamma * alpha
-
-        obj = (1 / (2 * n_samples)) * ||y - X w||^2_2 + pen(|w_j|)
+    .. math::
+        "pen"(x) = {(alpha x - x^2 / (2 gamma), if x <= alpha gamma),
+                    (gamma alpha^2 / 2        , if x > alpha gamma):}
+
+    .. math::
+        "obj" = 1 / (2 xx n_"samples") ||y - Xw||_2 ^ 2
+              + sum_(j=1)^(n_"features") "pen"(|w_j|)
 
     For more details see
-    Coordinate descent algorithms for nonconvex penalized regression,
-    with applications to biological feature selection, Breheny and Huang.
+    `Coordinate descent algorithms for nonconvex penalized regression,
+    with applications to biological feature selection, Breheny and Huang
+    <https://doi.org/10.1214/10-aoas388>`_.
 
     Parameters
     ----------
     alpha : float, optional
         Penalty strength.
 
     gamma : float, default=3
-        If gamma = 1, the prox of MCP is a hard thresholding.
-        If gamma = np.inf it is a soft thresholding.
+        If ``gamma = 1``, the prox of MCP is a hard thresholding.
+        If ``gamma = np.inf`` it is a soft thresholding.
         Should be larger than (or equal to) 1.
 
     max_iter : int, optional
         The maximum number of iterations (subproblem definitions).
 
     max_epochs : int
         Maximum number of CD epochs on each subproblem.
@@ -770,24 +807,24 @@
     tol : float, optional
         Stopping criterion for the optimization.
 
     fit_intercept : bool, optional (default=True)
         Whether or not to fit an intercept.
 
     warm_start : bool, optional (default=False)
-        When set to True, reuse the solution of the previous call to fit as
+        When set to ``True``, reuse the solution of the previous call to fit as
         initialization, otherwise, just erase the previous solution.
 
     ws_strategy : str
         The score used to build the working set. Can be ``fixpoint`` or ``subdiff``.
 
     Attributes
     ----------
     coef_ : array, shape (n_features,)
-        parameter vector (w in the cost function formula)
+        parameter vector (:math:`w` in the cost function formula)
 
     sparse_coef_ : scipy.sparse matrix, shape (n_features, 1)
         ``sparse_coef_`` is a readonly property derived from ``coef_``
 
     intercept_ : float
         constant term in decision function.
 
@@ -825,15 +862,16 @@
         y : array, shape (n_samples,)
             Target vector.
 
         alphas : array, shape (n_alphas,)
             Grid of alpha.
 
         coef_init : array, shape (n_features,), optional
-            If warm_start is enabled, the optimization problem restarts from coef_init.
+            If warm start is enabled, the optimization problem restarts from
+            ``coef_init``.
 
         return_n_iter : bool
             Returns the number of iterations along the path.
 
         **params : kwargs
             All parameters supported by path.
 
@@ -845,15 +883,16 @@
         coefs : array, shape (n_features, n_alphas)
             Coefficients along the path.
 
         stop_crit : array, shape (n_alphas,)
             Value of stopping criterion at convergence along the path.
 
         n_iters : array, shape (n_alphas,), optional
-            The number of iterations along the path. If return_n_iter is set to `True`.
+            The number of iterations along the path. If return_n_iter is set to
+            ``True``.
         """
         penalty = compiled_clone(MCPenalty(self.alpha, self.gamma))
         datafit = compiled_clone(Quadratic(), to_float32=X.dtype == np.float32)
         solver = AndersonCD(
             self.max_iter, self.max_epochs, self.p0, tol=self.tol,
             ws_strategy=self.ws_strategy, fit_intercept=self.fit_intercept,
             warm_start=self.warm_start, verbose=self.verbose)
@@ -882,17 +921,18 @@
         return _glm_fit(X, y, self, Quadratic(), MCPenalty(self.alpha, self.gamma),
                         solver)
 
 
 class SparseLogisticRegression(LinearClassifierMixin, SparseCoefMixin, BaseEstimator):
     r"""Sparse Logistic regression estimator.
 
-    The optimization objective for sparse Logistic regression is::
+    The optimization objective for sparse Logistic regression is:
 
-        mean(log(1 + exp(-y_i x_i^T w))) + alpha * ||w||_1
+    .. math:: 1 / n_"samples" sum_(i=1)^(n_"samples") log(1 + exp(-y_i x_i^T w))
+        + alpha ||w||_1
 
     Parameters
     ----------
     alpha : float, default=1.0
         Regularization strength; must be a positive float.
 
     tol : float, optional
@@ -907,26 +947,26 @@
     verbose : bool or int
         Amount of verbosity.
 
     fit_intercept : bool, optional (default=True)
         Whether or not to fit an intercept.
 
     warm_start : bool, optional (default=False)
-        When set to True, reuse the solution of the previous call to fit as
+        When set to ``True``, reuse the solution of the previous call to fit as
         initialization, otherwise, just erase the previous solution.
 
     Attributes
     ----------
     classes_ : ndarray, shape (n_classes, )
         A list of class labels known to the classifier.
 
     coef_ : ndarray, shape (1, n_features) or (n_classes, n_features)
         Coefficient of the features in the decision function.
 
-        `coef_` is of shape (1, n_features) when the given problem is binary.
+        ``coef_`` is of shape (1, n_features) when the given problem is binary.
 
     intercept_ :  ndarray, shape (1,) or (n_classes,)
         constant term in decision function. Not handled yet.
 
     n_iter_ : int
         Number of subproblems solved to reach the specified tolerance.
     """
@@ -973,15 +1013,15 @@
         For a multi_class problem, a one-vs-rest approach, i.e calculate the probability
         of each class assuming it to be positive using the logistic function.
         and normalize these values across all the classes.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
-            Vector to be scored, where `n_samples` is the number of samples and
+            Vector to be scored, where ``n_samples`` is the number of samples and
             `n_features` is the number of features.
 
         Returns
         -------
         T : array-like of shape (n_samples, n_classes)
             Returns the probability of the sample for each class in the model,
             where classes are ordered as they are in ``self.classes_``.
@@ -991,15 +1031,15 @@
             # Code taken from https://github.com/scikit-learn/scikit-learn/
             # blob/c900ad385cecf0063ddd2d78883b0ea0c99cd835/sklearn/
             # linear_model/_base.py#L458
             def _predict_proba_lr(X):
                 """Probability estimation for OvR logistic regression.
 
                 Positive class probabilities are computed as
-                1. / (1. + np.exp(-self.decision_function(X)));
+                ``1. / (1. + np.exp(-self.decision_function(X)))``;
                 multiclass is handled by normalizing that over all classes.
                 """
                 prob = self.decision_function(X)
                 expit(prob, out=prob)
                 if prob.ndim == 1:
                     return np.vstack([1 - prob, prob]).T
                 else:
@@ -1018,28 +1058,33 @@
                 decision_2d = decision
             return softmax(decision_2d, copy=False)
 
 
 class LinearSVC(LinearClassifierMixin, SparseCoefMixin, BaseEstimator):
     r"""LinearSVC estimator, with hinge loss.
 
-    The optimization objective for LinearSVC is::
+    The optimization objective for LinearSVC is:
 
-        C * \sum_i max(0, 1 - y_i beta.T X[i, :]) + 1 / 2 * ||beta||^2
+    .. math:: C xx sum_(i=1)^(n_"samples") max(0, 1 - y_i beta^T X[i, :])
+        + 1/2 ||beta||_2 ^ 2
 
     i.e. hinge datafit loss (non-smooth) + l2 regularization (smooth)
 
     To solve this, we solve the dual optimization problem to stay in our
     framework of smooth datafit and non-smooth penalty.
-    The dual optimization problem of SVC is::
+    The dual optimization problem of SVC is:
 
-        1 / 2 * ||(y X).T w||^2_2 - \sum_i w_i + \sum_i ind(0 <= w_i <= C)
+    .. math::
+        1/2 ||(yX)^T w||_2 ^ 2
+        - \sum_(i=1)^(n_"samples") w_i
+        + \sum_(i=1)^(n_"samples") [0 <= w_i <= C]
 
-    The primal-dual relation is given by::
-        w = \sum_i y_i * w_i * X[i, :]
+    The primal-dual relation is given by:
+
+    .. math:: w = \sum_(i=1)^(n_"samples") y_i w_i X[i, :]
 
     Parameters
     ----------
     C : float, optional
         Regularization parameter. The strength of the regularization is
         inversely proportional to C. Must be strictly positive.
 
@@ -1058,24 +1103,24 @@
     tol : float, optional
         Stopping criterion for the optimization.
 
     fit_intercept : bool, optional (default=True)
         Whether or not to fit an intercept.
 
     warm_start : bool, optional (default=False)
-        When set to True, reuse the solution of the previous call to fit as
+        When set to ``True``, reuse the solution of the previous call to fit as
         initialization, otherwise, just erase the previous solution.
 
     ws_strategy : str
         The score used to build the working set. Can be ``fixpoint`` or ``subdiff``.
 
     Attributes
     ----------
     coef_ : array, shape (n_features,)
-        parameter vector (w in the cost function formula)
+        parameter vector (:math:`w` in the cost function formula)
 
     sparse_coef_ : scipy.sparse matrix, shape (n_features, 1)
         ``sparse_coef_`` is a readonly property derived from ``coef_``
 
     intercept_ : float
         constant term in decision function.
 
@@ -1121,28 +1166,191 @@
             ws_strategy=self.ws_strategy, fit_intercept=False,
             warm_start=self.warm_start, verbose=self.verbose)
         return _glm_fit(X, y, self, QuadraticSVC(), IndicatorBox(self.C), solver)
 
     # TODO add predict_proba for LinearSVC
 
 
+class CoxEstimator(LinearModel):
+    r"""Elastic Cox estimator with Efron and Breslow estimate.
+
+    Refer to :ref:`Mathematics behind Cox datafit <maths_cox_datafit>`
+    for details about the datafit expression. The data convention for the estimator is
+
+    - ``X`` the design matrix with ``n_features`` predictors
+    - ``y`` a two-column array where the first ``tm`` is of event time occurrences
+      and the second ``s`` is of censoring.
+
+    For L2-regularized Cox (``l1_ratio=0.``) :ref:`LBFGS <skglm.solvers.LBFGS>`
+    is the used solver, otherwise it is :ref:`ProxNewton <skglm.solvers.ProxNewton>`.
+
+    Parameters
+    ----------
+    alpha : float, optional
+        Penalty strength. It must be strictly positive.
+
+    l1_ratio : float, default=0.5
+        The ElasticNet mixing parameter, with ``0 <= l1_ratio <= 1``. For
+        ``l1_ratio = 0`` the penalty is an L2 penalty. ``For l1_ratio = 1`` it
+        is an L1 penalty.  For ``0 < l1_ratio < 1``, the penalty is a
+        combination of L1 and L2.
+
+    method : {'efron', 'breslow'}, default='efron'
+        The estimate used for the Cox datafit. Use ``efron`` to
+        handle tied observations.
+
+    tol : float, optional
+        Stopping criterion for the optimization.
+
+    max_iter : int, optional
+        The maximum number of iterations to solve the problem.
+
+    verbose : bool or int
+        Amount of verbosity.
+
+    Attributes
+    ----------
+    coef_ : array, shape (n_features,)
+        Parameter vector of Cox regression.
+
+    stop_crit_ : float
+        The value of the stopping criterion at convergence.
+    """
+
+    _parameter_constraints: dict = {
+        "alpha": [Interval(Real, 0, None, closed="neither")],
+        "l1_ratio": [Interval(Real, 0, 1, closed="both")],
+        "method": [StrOptions({"efron", "breslow"})],
+        "tol": [Interval(Real, 0, None, closed="left")],
+        "max_iter": [Interval(Integral, 1, None, closed="left")],
+        "verbose": ["boolean", Interval(Integral, 0, 2, closed="both")],
+    }
+
+    def __init__(self, alpha=1., l1_ratio=0.7, method="efron", tol=1e-4,
+                 max_iter=50, verbose=False):
+        self.alpha = alpha
+        self.l1_ratio = l1_ratio
+        self.method = method
+        self.tol = tol
+        self.max_iter = max_iter
+        self.verbose = verbose
+
+    def fit(self, X, y):
+        """Fit Cox estimator.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, n_features)
+            Design matrix.
+
+        y : array-like, shape (n_samples, 2)
+            Two-column array where the first is of event time occurrences
+            and the second is of censoring. If it is of dimension 1, it is
+            assumed to be the times vector and there no censoring.
+
+        Returns
+        -------
+        self :
+            The fitted estimator.
+        """
+        self._validate_params()
+
+        # validate input data
+        X = check_array(
+            X,
+            accept_sparse="csc",
+            order="F",
+            dtype=[np.float64, np.float32],
+            input_name="X",
+        )
+        if y is None:
+            # Needed to pass check estimator. Message error is
+            # copy/paste from https://github.com/scikit-learn/scikit-learn/blob/ \
+            # 23ff51c07ebc03c866984e93c921a8993e96d1f9/sklearn/utils/ \
+            # estimator_checks.py#L3886
+            raise ValueError("requires y to be passed, but the target y is None")
+        y = check_array(
+            y,
+            accept_sparse=False,
+            order="F",
+            dtype=X.dtype,
+            ensure_2d=False,
+            input_name="y",
+        )
+        if y.ndim == 1:
+            warnings.warn(
+                f"{repr(self)} requires the vector of response `y` to have "
+                f"two columns. Got one column.\nAssuming that `y` "
+                "is the vector of times and there is no censoring."
+            )
+            y = np.column_stack((y, np.ones_like(y))).astype(X.dtype, order="F")
+        elif y.shape[1] > 2:
+            raise ValueError(
+                f"{repr(self)} requires the vector of response `y` to have "
+                f"two columns. Got {y.shape[1]} columns."
+            )
+
+        check_consistent_length(X, y)
+
+        # init datafit and penalty
+        datafit = Cox(self.method)
+
+        if self.l1_ratio == 1.:
+            penalty = L1(self.alpha)
+        elif 0. < self.l1_ratio < 1.:
+            penalty = L1_plus_L2(self.alpha, self.l1_ratio)
+        else:
+            penalty = L2(self.alpha)
+
+        # skglm internal: JIT compile classes
+        datafit = compiled_clone(datafit)
+        penalty = compiled_clone(penalty)
+
+        # init solver
+        if self.l1_ratio == 0.:
+            solver = LBFGS(max_iter=self.max_iter, tol=self.tol, verbose=self.verbose)
+        else:
+            solver = ProxNewton(
+                max_iter=self.max_iter, tol=self.tol, verbose=self.verbose,
+                fit_intercept=False,
+            )
+
+        # solve problem
+        if not issparse(X):
+            datafit.initialize(X, y)
+        else:
+            datafit.initialize_sparse(X.data, X.indptr, X.indices, y)
+
+        w, _, stop_crit = solver.solve(X, y, datafit, penalty)
+
+        # save to attribute
+        self.coef_ = w
+        self.stop_crit_ = stop_crit
+
+        self.intercept_ = 0.
+        self.n_features_in_ = X.shape[1]
+        self.feature_names_in_ = np.arange(X.shape[1])
+
+        return self
+
+
 class MultiTaskLasso(LinearModel, RegressorMixin):
     r"""MultiTaskLasso estimator.
 
-    The optimization objective for MultiTaskLasso is::
+    The optimization objective for MultiTaskLasso is:
 
-        (1 / (2 * n_samples)) * ||y - X W||^2_2 + alpha * ||W||_{21}
+    .. math:: 1 / (2 xx n_"samples") ||y - XW||_2 ^ 2 + alpha ||W||_(21)
 
     Parameters
     ----------
     alpha : float, optional
         Regularization strength (constant that multiplies the L21 penalty).
 
     copy_X : bool, optional (default=True)
-        If True, X will be copied; else, it may be overwritten.
+        If ``True``, X will be copied; else, it may be overwritten.
 
     max_iter : int, optional
         The maximum number of iterations (subproblem definitions).
 
     max_epochs : int
         Maximum number of CD epochs on each subproblem.
 
@@ -1155,24 +1363,24 @@
     tol : float, optional
         Stopping criterion for the optimization.
 
     fit_intercept : bool, optional (default=True)
         Whether or not to fit an intercept.
 
     warm_start : bool, optional (default=False)
-        When set to True, reuse the solution of the previous call to fit as
+        When set to ``True``, reuse the solution of the previous call to fit as
         initialization, otherwise, just erase the previous solution.
 
     ws_strategy : str
         The score used to build the working set. Can be ``fixpoint`` or ``subdiff``.
 
     Attributes
     ----------
     coef_ : array, shape (n_features,)
-        parameter vector (w in the cost function formula)
+        parameter vector (:math:`w` in the cost function formula)
 
     sparse_coef_ : scipy.sparse matrix, shape (n_features, 1)
         ``sparse_coef_`` is a readonly property derived from ``coef_``
 
     intercept_ : float
         constant term in decision function.
 
@@ -1264,15 +1472,16 @@
         Y : array, shape (n_samples, n_tasks)
             Target matrix.
 
         alphas : array, shape (n_alphas,)
             Grid of alpha.
 
         coef_init : array, shape (n_features,), optional
-            If warm_start is enabled, the optimization problem restarts from coef_init.
+            If warm start is enabled, the optimization problem restarts from
+            ``coef_init``.
 
         return_n_iter : bool
             Returns the number of iterations along the path.
 
         **params : kwargs
             All parameters supported by path.
 
@@ -1284,15 +1493,16 @@
         coefs : array, shape (n_features, n_tasks, n_alphas)
             Coefficients along the path.
 
         stop_crit : array, shape (n_alphas,)
             Value of stopping criterion at convergence along the path.
 
         n_iters : array, shape (n_alphas,), optional
-            The number of iterations along the path. If return_n_iter is set to `True`.
+            The number of iterations along the path. If return_n_iter is set to
+            ``True``.
         """
         datafit = compiled_clone(QuadraticMultiTask(), to_float32=X.dtype == np.float32)
         penalty = compiled_clone(L2_1(self.alpha))
         solver = MultiTaskBCD(
             self.max_iter, self.max_epochs, self.p0, tol=self.tol,
             ws_strategy=self.ws_strategy, fit_intercept=self.fit_intercept,
             warm_start=self.warm_start, verbose=self.verbose)
```

### Comparing `skglm-0.2/skglm/experimental/_plot_sqrt_lasso.py` & `skglm-0.3/skglm/experimental/_plot_sqrt_lasso.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import numpy as np
 from numpy.linalg import norm
 import matplotlib.pyplot as plt
-from skglm.utils import make_correlated_data
+from skglm.utils.data import make_correlated_data
 from skglm.experimental.sqrt_lasso import SqrtLasso, _chambolle_pock_sqrt
 
 X, y, _ = make_correlated_data(n_samples=200, n_features=100, random_state=24)
 
 n_samples, n_features = X.shape
 alpha_max = norm(X.T @ y, ord=np.inf) / (norm(y) * np.sqrt(n_samples))
```

### Comparing `skglm-0.2/skglm/experimental/sqrt_lasso.py` & `skglm-0.3/skglm/experimental/sqrt_lasso.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 import warnings
 import numpy as np
 from numpy.linalg import norm
 from sklearn.exceptions import ConvergenceWarning
 from sklearn.linear_model._base import LinearModel, RegressorMixin
 
 from skglm.penalties import L1
-from skglm.utils import compiled_clone, ST_vec, proj_L2ball
+from skglm.utils.prox_funcs import ST_vec, proj_L2ball, BST
+from skglm.utils.jit_compilation import compiled_clone
 from skglm.datafits.base import BaseDatafit
 from skglm.solvers.prox_newton import ProxNewton
 
 
 class SqrtQuadratic(BaseDatafit):
-    """Square root quadratic datafit.
+    r"""Unnormalized square root quadratic datafit.
 
-    The datafit reads::
-        ||y - Xw||_2 / sqrt(n_samples)
+    The datafit reads:
+
+    .. math::
+
+        ||y - Xw||_2
     """
 
     def __init__(self):
         pass
 
     def get_spec(self):
         spec = ()
         return spec
 
     def params_to_dict(self):
         return dict()
 
     def value(self, y, w, Xw):
-        return np.linalg.norm(y - Xw) / np.sqrt(len(y))
+        return np.linalg.norm(y - Xw)
 
     def raw_grad(self, y, Xw):
         """Compute gradient of datafit w.r.t ``Xw``.
 
         Raises
         ------
             Exception
@@ -40,29 +44,47 @@
         """
         minus_residual = Xw - y
         norm_residuals = norm(minus_residual)
 
         if norm_residuals < 1e-2 * norm(y):
             raise ValueError("SmallResidualException")
 
-        return minus_residual / (norm_residuals * np.sqrt(len(y)))
+        return minus_residual / norm_residuals
 
     def raw_hessian(self, y, Xw):
         """Diagonal matrix upper bounding the Hessian."""
         n_samples = len(y)
-        fill_value = 1 / (np.sqrt(n_samples) * norm(y - Xw))
+        fill_value = 1 / norm(y - Xw)
         return np.full(n_samples, fill_value)
 
+    def prox(self, w, step, y):
+        """Prox of ``step * ||y - . ||``."""
+        return y - BST(y - w, step)
+
+    def prox_conjugate(self, z, step, y):
+        """Prox of ``step * ||y - . ||^*``."""
+        return proj_L2ball(z - step * y)
+
+    def subdiff_distance(self, Xw, z, y):
+        """Distance of ``z`` to subdiff of ||y - . || at ``Xw``."""
+        # computation note: \partial ||y - . ||(Xw) = - \partial || . ||(y - Xw)
+        y_minus_Xw = y - Xw
+
+        if np.any(y_minus_Xw):
+            return norm(z + y_minus_Xw / norm(y_minus_Xw))
+
+        return norm(z - proj_L2ball(z))
+
 
 class SqrtLasso(LinearModel, RegressorMixin):
     """Square root Lasso estimator based on Prox Newton solver.
 
-    The optimization objective for square root Lasso is::
+    The optimization objective for square root Lasso is:
 
-        |y - X w||_2 / sqrt(n_samples) + alpha * ||w||_1
+    .. math:: ||y - Xw||_2 + alpha ||w||_1
 
     Parameters
     ----------
     alpha : float, default 1
         Penalty strength.
 
     max_iter : int, default 20
@@ -200,15 +222,16 @@
         return alphas, coefs
 
 
 def _chambolle_pock_sqrt(X, y, alpha, max_iter=1000, obj_freq=10, verbose=False):
     """Apply Chambolle-Pock algorithm to solve square-root Lasso.
 
     The objective function is:
-        min_w ||Xw - y||_2/sqrt(n_samples) + alpha * ||w||_1.
+
+        min_w ||Xw - y||_2 + alpha * ||w||_1.
     """
     n_samples, n_features = X.shape
     # dual variable is z, primal is w
     z_old = np.zeros(n_samples)
     z = z_old.copy()
     w = np.zeros(n_features)
 
@@ -216,17 +239,17 @@
 
     L = norm(X, ord=2)
     # take primal and dual stepsizes equal
     tau = 0.99 / L
     sigma = 0.99 / L
 
     for t in range(max_iter):
-        w = ST_vec(w - tau * X.T @ (2 * z - z_old), alpha * np.sqrt(n_samples) * tau)
+        w = ST_vec(w - tau * X.T @ (2 * z - z_old), alpha * tau)
         z_old = z.copy()
         z[:] = proj_L2ball(z + sigma * (X @ w - y))
 
         if t % obj_freq == 0:
-            objs.append(norm(X @ w - y) / np.sqrt(n_samples) + alpha * norm(w, ord=1))
+            objs.append(norm(X @ w - y) + alpha * norm(w, ord=1))
             if verbose:
                 print(f"Iter {t}, obj {objs[-1]: .10f}")
 
     return w, z, objs
```

### Comparing `skglm-0.2/skglm/penalties/base.py` & `skglm-0.3/skglm/penalties/base.py`

 * *Files identical despite different names*

### Comparing `skglm-0.2/skglm/penalties/block_separable.py` & `skglm-0.3/skglm/penalties/block_separable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from numpy.linalg import norm
 
 from numba import float64, int32
 
 from skglm.penalties.base import BasePenalty
-from skglm.utils import (
+from skglm.utils.prox_funcs import (
     BST, prox_block_2_05, prox_SCAD, value_SCAD, prox_MCP, value_MCP)
 
 
 class L2_1(BasePenalty):
     """L2/1 row-wise penalty: sum of L2 norms of rows."""
 
     def __init__(self, alpha):
@@ -154,24 +154,30 @@
 
     def is_penalized(self, n_features):
         """Return a binary mask with the penalized features."""
         return np.ones(n_features, dtype=np.bool_)
 
 
 class BlockSCAD(BasePenalty):
-    """Block Smoothly Clipped Absolute Deviation.
+    r"""Block Smoothly Clipped Absolute Deviation.
 
     Notes
     -----
-    With W_j the j-th row of W, the penalty is:
-        pen(||W_j||) = alpha * ||W_j||               if ||W_j|| =< alpha
-                       (2 * gamma * alpha * ||W_j|| - ||W_j|| ** 2 - alpha ** 2) \
-                           / (2 * (gamma - 1))       if alpha < ||W_j|| < alpha * gamma
-                       (alpha **2 * (gamma + 1)) / 2 if ||W_j|| > gamma * alpha
-        value = sum_{j=1}^{n_features} pen(||W_j||)
+    With :math:`W_j` the j-th row of math:`W`, the penalty is:
+
+    .. math::
+        "pen"(||W_j||) = {
+            (alpha ||W_j||            , if \ \ \ \ \ \ \ \ \ \ ||W_j|| <= alpha),
+            ((2 alpha gamma ||W_j|| - ||W_j||^2 - alpha^2) / (2 (gamma - 1))
+                                      , if       alpha  \ \  < ||W_j|| <= alpha gamma),
+            ((alpha^2 (gamma + 1)) / 2, if       alpha gamma < ||W_j||)
+        :}
+
+    .. math::
+        "value" = sum_(j=1)^(n_"features") "pen"(||W_j||)
     """
 
     def __init__(self, alpha, gamma):
         self.alpha = alpha
         self.gamma = gamma
 
     def get_spec(self):
@@ -222,17 +228,20 @@
         """Return a binary mask with the penalized features."""
         return np.ones(n_features, dtype=np.bool_)
 
 
 class WeightedGroupL2(BasePenalty):
     r"""Weighted Group L2 penalty.
 
-    The penalty reads::
+    The penalty reads
+
+    .. math::
+        sum_{g=1}^{n_"groups"} "weights"_g xx ||w_{[g]}||
 
-        \sum_{g} weights[g] * ||w_g||_2
+    with :math:`w_{[g]}` being the coefficients of the g-th group.
 
     Attributes
     ----------
     alpha : float
         The regularization parameter.
 
     weights : array, shape (n_groups,)
@@ -282,16 +291,16 @@
     def prox_1group(self, value, stepsize, g):
         """Compute the proximal operator of group ``g``."""
         return BST(value, self.alpha * stepsize * self.weights[g])
 
     def subdiff_distance(self, w, grad_ws, ws):
         """Compute distance to the subdifferential at ``w`` of negative gradient.
 
-        Note: ``grad_ws`` is a stacked array of ``-``gradients.
-        ([-grad_ws_1, -grad_ws_2, ...])
+        Note: ``grad_ws`` is a stacked array of gradients.
+        ([grad_ws_1, grad_ws_2, ...])
         """
         alpha, weights = self.alpha, self.weights
         grp_ptr, grp_indices = self.grp_ptr, self.grp_indices
 
         scores = np.zeros(len(ws))
         grad_ptr = 0
         for idx, g in enumerate(ws):
@@ -303,15 +312,15 @@
             w_g = w[grp_g_indices]
             norm_w_g = norm(w_g)
 
             if norm_w_g == 0:
                 scores[idx] = max(0, norm(grad_g) - alpha * weights[g])
             else:
                 subdiff = alpha * weights[g] * w_g / norm_w_g
-                scores[idx] = norm(grad_g - subdiff)
+                scores[idx] = norm(grad_g + subdiff)
 
         return scores
 
     def is_penalized(self, n_groups):
         return np.ones(n_groups, dtype=np.bool_)
 
     def generalized_support(self, w):
```

### Comparing `skglm-0.2/skglm/penalties/separable.py` & `skglm-0.3/skglm/penalties/separable.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,61 @@
 import numpy as np
 from numba import float64
 from numba.types import bool_
 
 from skglm.penalties.base import BasePenalty
-from skglm.utils import (
+from skglm.utils.prox_funcs import (
     ST, box_proj, prox_05, prox_2_3, prox_SCAD, value_SCAD, prox_MCP, value_MCP)
 
 
 class L1(BasePenalty):
-    """L1 penalty."""
+    """:math:`ell_1` penalty."""
 
-    def __init__(self, alpha):
+    def __init__(self, alpha, positive=False):
         self.alpha = alpha
+        self.positive = positive
 
     def get_spec(self):
         spec = (
             ('alpha', float64),
+            ('positive', bool_),
         )
         return spec
 
     def params_to_dict(self):
-        return dict(alpha=self.alpha)
+        return dict(alpha=self.alpha, positive=self.positive)
 
     def value(self, w):
         """Compute L1 penalty value."""
         return self.alpha * np.sum(np.abs(w))
 
     def prox_1d(self, value, stepsize, j):
         """Compute proximal operator of the L1 penalty (soft-thresholding operator)."""
-        return ST(value, self.alpha * stepsize)
+        return ST(value, self.alpha * stepsize, self.positive)
 
     def subdiff_distance(self, w, grad, ws):
         """Compute distance of negative gradient to the subdifferential at w."""
         subdiff_dist = np.zeros_like(grad)
         for idx, j in enumerate(ws):
-            if w[j] == 0:
-                # distance of - grad_j to  [-alpha, alpha]
-                subdiff_dist[idx] = max(0, np.abs(grad[idx]) - self.alpha)
+            if self.positive:
+                if w[j] < 0:
+                    subdiff_dist[idx] = np.inf
+                elif w[j] == 0:
+                    # distance of -grad_j to (-infty, alpha]
+                    subdiff_dist[idx] = max(0, -grad[idx] - self.alpha)
+                else:
+                    # distance of -grad_j to {alpha}
+                    subdiff_dist[idx] = np.abs(grad[idx] + self.alpha)
             else:
-                # distance of - grad_j to alpha * sign(w[j])
-                subdiff_dist[idx] = np.abs(
-                    - grad[idx] - np.sign(w[j]) * self.alpha)
+                if w[j] == 0:
+                    # distance of -grad_j to  [-alpha, alpha]
+                    subdiff_dist[idx] = max(0, np.abs(grad[idx]) - self.alpha)
+                else:
+                    # distance of -grad_j to {alpha * sign(w[j])}
+                    subdiff_dist[idx] = np.abs(grad[idx] + np.sign(w[j]) * self.alpha)
         return subdiff_dist
 
     def is_penalized(self, n_features):
         """Return a binary mask with the penalized features."""
         return np.ones(n_features, dtype=np.bool_)
 
     def generalized_support(self, w):
@@ -53,58 +64,72 @@
 
     def alpha_max(self, gradient0):
         """Return penalization value for which 0 is solution."""
         return np.max(np.abs(gradient0))
 
 
 class L1_plus_L2(BasePenalty):
-    """L1 + L2 penalty (aka ElasticNet penalty)."""
+    """:math:`ell_1 + ell_2` penalty (aka ElasticNet penalty)."""
 
-    def __init__(self, alpha, l1_ratio):
+    def __init__(self, alpha, l1_ratio, positive=False):
         self.alpha = alpha
         self.l1_ratio = l1_ratio
+        self.positive = positive
 
     def get_spec(self):
         spec = (
             ('alpha', float64),
             ('l1_ratio', float64),
+            ('positive', bool_),
         )
         return spec
 
     def params_to_dict(self):
-        return dict(alpha=self.alpha,
-                    l1_ratio=self.l1_ratio)
+        return dict(alpha=self.alpha, l1_ratio=self.l1_ratio, positive=self.positive)
 
     def value(self, w):
         """Compute the L1 + L2 penalty value."""
         value = self.l1_ratio * self.alpha * np.sum(np.abs(w))
         value += (1 - self.l1_ratio) * self.alpha / 2 * np.sum(w ** 2)
         return value
 
     def prox_1d(self, value, stepsize, j):
         """Compute the proximal operator (scaled soft-thresholding)."""
-        prox = ST(value, self.l1_ratio * self.alpha * stepsize)
+        prox = ST(value, self.l1_ratio * self.alpha * stepsize, self.positive)
         prox /= (1 + stepsize * (1 - self.l1_ratio) * self.alpha)
         return prox
 
     def subdiff_distance(self, w, grad, ws):
         """Compute distance of negative gradient to the subdifferential at w."""
         subdiff_dist = np.zeros_like(grad)
+        alpha = self.alpha
+        l1_ratio = self.l1_ratio
+
         for idx, j in enumerate(ws):
-            if w[j] == 0:
-                # distance of - grad_j to alpha * l1_ratio * [-1, 1]
-                subdiff_dist[idx] = max(
-                    0, np.abs(grad[idx]) - self.alpha * self.l1_ratio)
+            if self.positive:
+                if w[j] < 0:
+                    subdiff_dist[idx] = np.inf
+                elif w[j] == 0:
+                    # distance of -grad_j to (-infty, alpha * l1_ratio]
+                    subdiff_dist[idx] = max(0, -grad[idx] - alpha * l1_ratio)
+                else:
+                    # distance of -grad_j to alpha * {l1_ratio + (1 - l1_ratio) * w[j]}
+                    subdiff_dist[idx] = np.abs(
+                        grad[idx] + alpha * (l1_ratio
+                                             + (1 - l1_ratio) * w[j]))
             else:
-                # distance of - grad_j to alpha * l_1 ratio * sign(w[j]) +
-                # alpha * (1 - l1_ratio) * w[j]
-                subdiff_dist[idx] = np.abs(
-                    - grad[idx] -
-                    self.alpha * (self.l1_ratio *
-                                  np.sign(w[j]) + (1 - self.l1_ratio) * w[j]))
+                if w[j] == 0:
+                    # distance of -grad_j to alpha * l1_ratio * [-1, 1]
+                    subdiff_dist[idx] = max(0, np.abs(grad[idx]) - alpha * l1_ratio)
+                else:
+                    # distance of -grad_j to
+                    # {alpha * (l1 ratio * sign(w[j]) + (1 - l1_ratio) * w[j])}
+                    subdiff_dist[idx] = np.abs(
+                        grad[idx] + alpha * (l1_ratio * np.sign(w[j])
+                                             + (1 - l1_ratio) * w[j]))
         return subdiff_dist
 
     def is_penalized(self, n_features):
         """Return a binary mask with the penalized features."""
         return np.ones(n_features).astype(bool_)
 
     def generalized_support(self, w):
@@ -115,49 +140,62 @@
         """Return penalization value for which 0 is solution."""
         return np.max(np.abs(gradient0))
 
 
 class WeightedL1(BasePenalty):
     """Weighted L1 penalty."""
 
-    def __init__(self, alpha, weights):
+    def __init__(self, alpha, weights, positive=False):
         self.alpha = alpha
         self.weights = weights.astype(np.float64)
+        self.positive = positive
 
     def get_spec(self):
         spec = (
             ('alpha', float64),
             ('weights', float64[:]),
+            ('positive', bool_),
         )
         return spec
 
     def params_to_dict(self):
-        return dict(alpha=self.alpha,
-                    weights=self.weights)
+        return dict(alpha=self.alpha, weights=self.weights, positive=self.positive)
 
     def value(self, w):
         """Compute the weighted L1 penalty."""
         return self.alpha * np.sum(np.abs(w) * self.weights)
 
     def prox_1d(self, value, stepsize, j):
         """Compute the proximal operator of weighted L1 (weighted soft-thresholding)."""
-        return ST(value, self.alpha * stepsize * self.weights[j])
+        return ST(value, self.alpha * stepsize * self.weights[j], self.positive)
 
     def subdiff_distance(self, w, grad, ws):
         """Compute distance of negative gradient to the subdifferential at w."""
         subdiff_dist = np.zeros_like(grad)
+        alpha = self.alpha
+        weights = self.weights
+
         for idx, j in enumerate(ws):
-            if w[j] == 0:
-                # distance of - grad_j to alpha * weights[j] * [-1, 1]
-                subdiff_dist[idx] = max(
-                    0, np.abs(grad[idx]) - self.alpha * self.weights[j])
+            if self.positive:
+                if w[j] < 0:
+                    subdiff_dist[idx] = np.inf
+                elif w[j] == 0:
+                    # distance of -grad_j to (-infty, alpha * weights[j]]
+                    subdiff_dist[idx] = max(0, -grad[idx] - alpha * weights[j])
+                else:
+                    # distance of -grad_j to {alpha * weights[j]}
+                    subdiff_dist[idx] = np.abs(grad[idx] + alpha * weights[j])
             else:
-                # distance of - grad_j to alpha * weights[j] * sign(w[j])
-                subdiff_dist[idx] = np.abs(
-                    - grad[idx] - self.alpha * self.weights[j] * np.sign(w[j]))
+                if w[j] == 0:
+                    # distance of -grad_j to alpha * weights[j] * [-1, 1]
+                    subdiff_dist[idx] = max(0, np.abs(grad[idx]) - alpha * weights[j])
+                else:
+                    # distance of -grad_j to {alpha * weights[j] * sign(w[j])}
+                    subdiff_dist[idx] = np.abs(
+                        grad[idx] + alpha * weights[j] * np.sign(w[j]))
         return subdiff_dist
 
     def is_penalized(self, n_features):
         """Return a binary mask with the penalized features."""
         return self.weights != 0
 
     def generalized_support(self, w):
@@ -171,19 +209,21 @@
 
 
 class MCPenalty(BasePenalty):
     """Minimax Concave Penalty (MCP), a non-convex sparse penalty.
 
     Notes
     -----
-    With x >= 0
-    pen(x) =
-    alpha * x - x^2 / (2 * gamma) if x =< gamma * alpha
-    gamma * alpha^2 / 2           if x > gamma * alpha
-    value = sum_{j=1}^{n_features} pen(abs(w_j))
+    With :math:`x >= 0`:
+
+    .. math::
+        "pen"(x) = {(alpha x - x^2 / (2 gamma), if x =< alpha gamma),
+                    (gamma alpha^2 / 2        , if x > alpha gamma):}
+    .. math::
+        "value" = sum_(j=1)^(n_"features") "pen"(abs(w_j))
     """
 
     def __init__(self, alpha, gamma):
         self.alpha = alpha
         self.gamma = gamma
 
     def get_spec(self):
@@ -230,25 +270,30 @@
 
     def alpha_max(self, gradient0):
         """Return penalization value for which 0 is solution."""
         return np.max(np.abs(gradient0))
 
 
 class SCAD(BasePenalty):
-    """Smoothly Clipped Absolute Deviation.
+    r"""Smoothly Clipped Absolute Deviation.
 
     Notes
     -----
-    With x >= 0
-    pen(x) =
-    alpha * x                         if x =< alpha
-    2 * gamma * alpha * x - x^2 - alpha^2 \
-        / 2 * (gamma - 1))            if alpha < x < alpha * gamma
-    alpha^2 * (gamma + 1) / 2      if x > gamma * alpha
-    value = sum_{j=1}^{n_features} pen(abs(w_j))
+    With :math:`x >= 0`:
+
+    .. math::
+        "pen"(x) = {
+            (alpha x                  , if \ \ \ \ \ \ \ \ \ \ x <= alpha),
+            (2 alpha gamma x - x^2 - alpha^2 / 2 (gamma - 1)
+                                      , if       alpha \ \   < x <= alpha gamma),
+            (alpha^2 (gamma + 1) / 2  , if       alpha gamma < x  )
+        :}
+
+    .. math::
+        "value" = sum_(j=1)^(n_"features") "pen"(abs(w_j))
     """
 
     def __init__(self, alpha, gamma):
         self.alpha = alpha
         self.gamma = gamma
 
     def get_spec(self):
@@ -302,17 +347,18 @@
 
 
 class IndicatorBox(BasePenalty):
     """Box constraint penalty.
 
     Notes
     -----
-    ind_[0, alpha]^n_samples
-    where ind is the indicator function of the convex set
-    [0, alpha]^n_samples
+    .. math:: bb"1"_([0, alpha]^(n_"samples"))
+
+    where :math:`bb"1"` is the indicator function of the convex set
+    :math:`[0, alpha]^(n_"samples")`
     """
 
     def __init__(self, alpha):
         self.alpha = alpha
 
     def get_spec(self):
         spec = (
@@ -358,15 +404,15 @@
         """Return a mask with coefficients that are neither 0 nor alpha."""
         # w is the output of the projection unto [0, C] so checking strict equality
         # should be ok and we can avoid np.isclose
         return np.logical_and(w != 0, w != self.alpha)
 
 
 class L0_5(BasePenalty):
-    """L_{0.5} non-convex quasi-norm penalty."""
+    """:math:`ell_(0.5)` non-convex quasi-norm penalty."""
 
     def __init__(self, alpha):
         self.alpha = alpha
 
     def get_spec(self):
         spec = (
             ('alpha', float64),
@@ -376,14 +422,18 @@
     def params_to_dict(self):
         return dict(alpha=self.alpha)
 
     def value(self, w):
         """Compute the value of L0_5 at w."""
         return self.alpha * np.sum(np.abs(w) ** 0.5)
 
+    def derivative(self, w):
+        """Compute the element-wise derivative."""
+        return 1. / (2. * np.sqrt(np.abs(w)) + 1e-12)
+
     def prox_1d(self, value, stepsize, j):
         """Compute the proximal operator of L0_5."""
         return prox_05(value, self.alpha * stepsize)
 
     def subdiff_distance(self, w, grad, ws):
         """Compute distance of negative gradient to the subdifferential at w."""
         subdiff_dist = np.zeros_like(grad)
@@ -407,15 +457,15 @@
 
     def generalized_support(self, w):
         """Return a mask with non-zero coefficients."""
         return w != 0
 
 
 class L2_3(BasePenalty):
-    """L_{2/3} quasi-norm non-convex penalty."""
+    """:math:`ell_(2/3)` quasi-norm non-convex penalty."""
 
     def __init__(self, alpha):
         self.alpha = alpha
 
     def get_spec(self):
         spec = (
             ('alpha', float64),
@@ -425,14 +475,18 @@
     def params_to_dict(self):
         return dict(alpha=self.alpha)
 
     def value(self, w):
         """Compute the value of the L2_3 norm at w."""
         return self.alpha * np.sum(np.abs(w) ** (2/3))
 
+    def derivative(self, w):
+        """Compute the element-wise derivative."""
+        return 2 / (3 * np.abs(w) ** (1/3) + 1e-12)
+
     def prox_1d(self, value, stepsize, j):
         """Compute the proximal operator of the L2_3 norm."""
         return prox_2_3(value, self.alpha * stepsize)
 
     def subdiff_distance(self, w, grad, ws):
         """Compute distance of negative gradient to the subdifferential at w."""
         subdiff_dist = np.zeros_like(grad)
@@ -454,7 +508,83 @@
     def is_penalized(self, n_features):
         """Return a binary mask with the penalized features."""
         return np.ones(n_features, bool_)
 
     def generalized_support(self, w):
         """Return a mask with non-zero coefficients."""
         return w != 0
+
+
+class PositiveConstraint(BasePenalty):
+    """Positivity constraint penalty."""
+
+    def __init__(self):
+        pass
+
+    def get_spec(self):
+        return ()
+
+    def params_to_dict(self):
+        return dict()
+
+    def value(self, w):
+        """Compute the value of the PositiveConstraint penalty at w."""
+        return np.inf if (w < 0).any() else 0.
+
+    def prox_1d(self, value, stepsize, j):
+        """Compute the proximal operator of the PositiveConstraint."""
+        return max(0., value)
+
+    def subdiff_distance(self, w, grad, ws):
+        """Compute distance of negative gradient to the subdifferential at w."""
+        subdiff_dist = np.zeros_like(grad)
+        for idx, j in enumerate(ws):
+            if w[j] == 0:
+                # distance of - grad_j to  ]-infty, 0]
+                subdiff_dist[idx] = max(0, -grad[idx])
+            elif w[j] > 0:
+                # distance of - grad_j to 0
+                subdiff_dist[idx] = abs(-grad[idx])
+            else:
+                # subdiff is empty, distance is infinite
+                subdiff_dist[idx] = np.inf
+
+        return subdiff_dist
+
+    def is_penalized(self, n_features):
+        """Return a binary mask with the penalized features."""
+        return np.ones(n_features, bool_)
+
+    def generalized_support(self, w):
+        """Return a mask with non-zero coefficients."""
+        return w != 0
+
+
+class L2(BasePenalty):
+    r""":math:`ell_2` penalty.
+
+    The penalty reads
+
+    .. math::
+
+        \alpha / 2  ||w||_2^2
+    """
+
+    def __init__(self, alpha):
+        self.alpha = alpha
+
+    def get_spec(self):
+        spec = (
+            ('alpha', float64),
+        )
+        return spec
+
+    def params_to_dict(self):
+        return dict(alpha=self.alpha)
+
+    def value(self, w):
+        """Compute the value of the L2 penalty."""
+        return self.alpha * (w ** 2).sum() / 2
+
+    def gradient(self, w):
+        """Compute the gradient of the L2 penalty."""
+        return self.alpha * w
```

### Comparing `skglm-0.2/skglm/solvers/accelerated_cd.py` & `skglm-0.3/skglm/solvers/anderson_cd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from numba import njit
 from scipy import sparse
 from sklearn.utils import check_array
 from skglm.solvers.common import construct_grad, construct_grad_sparse, dist_fix_point
 from skglm.solvers.base import BaseSolver
-from skglm.utils import AndersonAcceleration
+from skglm.utils.anderson import AndersonAcceleration
 
 
 class AndersonCD(BaseSolver):
     """Coordinate descent solver with working sets and Anderson acceleration.
 
     fit_intercept : bool
         Whether or not to fit an intercept.
@@ -19,14 +19,15 @@
 
     max_epochs : int, optional
         Maximum number of (block) CD epochs on each subproblem.
 
     p0 : int, optional
         First working set size.
 
+    tol : float, optional
         The tolerance for the optimization.
 
     ws_strategy : ('subdiff'|'fixpoint'), optional
         The score used to build the working set.
 
     verbose : bool or int, optional
         Amount of verbosity. 0/False is silent.
@@ -57,15 +58,15 @@
         self.verbose = verbose
 
     def solve(self, X, y, datafit, penalty, w_init=None, Xw_init=None):
         if self.ws_strategy not in ("subdiff", "fixpoint"):
             raise ValueError(
                 'Unsupported value for self.ws_strategy:', self.ws_strategy)
         n_samples, n_features = X.shape
-        w = np.zeros(n_features) if w_init is None else w_init
+        w = np.zeros(n_features + self.fit_intercept) if w_init is None else w_init
         Xw = np.zeros(n_samples) if Xw_init is None else Xw_init
         pen = penalty.is_penalized(n_features)
         unpen = ~pen
         n_unpen = unpen.sum()
         obj_out = []
         all_feats = np.arange(n_features)
         stop_crit = np.inf  # initialize for case n_iter=0
```

### Comparing `skglm-0.2/skglm/solvers/anderson_cd.py` & `skglm-0.3/skglm/solvers/multitask_bcd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,345 +1,428 @@
 import numpy as np
-from numba import njit
 from scipy import sparse
+from numba import njit
+from numpy.linalg import norm
 from sklearn.utils import check_array
-from skglm.solvers.common import construct_grad, construct_grad_sparse, dist_fix_point
 from skglm.solvers.base import BaseSolver
-from skglm.utils import AndersonAcceleration
-
-
-class AndersonCD(BaseSolver):
-    """Coordinate descent solver with working sets and Anderson acceleration.
-
-    fit_intercept : bool
-        Whether or not to fit an intercept.
-
-    max_iter : int, optional
-        The maximum number of iterations (definition of working set and
-        resolution of problem restricted to features in working set).
 
-    max_epochs : int, optional
-        Maximum number of (block) CD epochs on each subproblem.
 
-    p0 : int, optional
-        First working set size.
-
-    tol : float, optional
-        The tolerance for the optimization.
-
-    ws_strategy : ('subdiff'|'fixpoint'), optional
-        The score used to build the working set.
-
-    verbose : bool or int, optional
-        Amount of verbosity. 0/False is silent.
-
-    References
-    ----------
-    .. [1] Bertrand, Q. and Klopfenstein, Q. and Bannier, P.-A. and Gidel, G.
-           and Massias, M.
-           "Beyond L1: Faster and Better Sparse Models with skglm", 2022
-           https://arxiv.org/abs/2204.07826
-
-    .. [2] Bertrand, Q. and Massias, M.
-           "Anderson acceleration of coordinate descent", AISTATS, 2021
-           https://proceedings.mlr.press/v130/bertrand21a.html
-           code: https://github.com/mathurinm/andersoncd
-    """
+class MultiTaskBCD(BaseSolver):
+    """Block coordinate descent solver for multi-task problems."""
 
-    def __init__(self, max_iter=50, max_epochs=50_000, p0=10,
-                 tol=1e-4, ws_strategy="subdiff", fit_intercept=True,
+    def __init__(self, max_iter=100, max_epochs=50_000, p0=10, tol=1e-6,
+                 use_acc=True, ws_strategy="subdiff", fit_intercept=True,
                  warm_start=False, verbose=0):
         self.max_iter = max_iter
         self.max_epochs = max_epochs
         self.p0 = p0
         self.tol = tol
+        self.use_acc = use_acc
         self.ws_strategy = ws_strategy
         self.fit_intercept = fit_intercept
         self.warm_start = warm_start
         self.verbose = verbose
 
-    def solve(self, X, y, datafit, penalty, w_init=None, Xw_init=None):
-        if self.ws_strategy not in ("subdiff", "fixpoint"):
-            raise ValueError(
-                'Unsupported value for self.ws_strategy:', self.ws_strategy)
+    def solve(self, X, Y, datafit, penalty, W_init=None, XW_init=None):
         n_samples, n_features = X.shape
-        w = np.zeros(n_features + self.fit_intercept) if w_init is None else w_init
-        Xw = np.zeros(n_samples) if Xw_init is None else Xw_init
+        n_tasks = Y.shape[1]
         pen = penalty.is_penalized(n_features)
         unpen = ~pen
         n_unpen = unpen.sum()
         obj_out = []
         all_feats = np.arange(n_features)
         stop_crit = np.inf  # initialize for case n_iter=0
-        w_acc, Xw_acc = np.zeros(n_features + self.fit_intercept), np.zeros(n_samples)
+        K = 5
 
-        is_sparse = sparse.issparse(X)
-        if is_sparse:
-            datafit.initialize_sparse(X.data, X.indptr, X.indices, y)
-        else:
-            datafit.initialize(X, y)
+        W = (np.zeros((n_features + self.fit_intercept, n_tasks)) if W_init is None
+             else W_init)
+        XW = np.zeros((n_samples, n_tasks)) if XW_init is None else XW_init
 
-        if len(w) != n_features + self.fit_intercept:
+        if W.shape[0] != n_features + self.fit_intercept:
             if self.fit_intercept:
                 val_error_message = (
-                    "w should be of size n_features + 1 when using fit_intercept=True: "
-                    f"expected {n_features + 1}, got {len(w)}.")
+                    "W.shape[0] should be n_features + 1 when using fit_intercept=True:"
+                    f" expected {n_features + 1}, got {W.shape[0]}.")
             else:
                 val_error_message = (
-                    "w should be of size n_features: "
-                    f"expected {n_features}, got {len(w)}.")
+                    "W.shape[0] should be of size n_features: "
+                    f"expected {n_features}, got {W.shape[0]}.")
             raise ValueError(val_error_message)
 
+        is_sparse = sparse.issparse(X)
+        if is_sparse:
+            datafit.initialize_sparse(X.data, X.indptr, X.indices, Y)
+        else:
+            datafit.initialize(X, Y)
+
         for t in range(self.max_iter):
             if is_sparse:
                 grad = datafit.full_grad_sparse(
-                    X.data, X.indptr, X.indices, y, Xw)
+                    X.data, X.indptr, X.indices, Y, XW)
             else:
-                grad = construct_grad(X, y, w[:n_features], Xw, datafit, all_feats)
+                grad = construct_grad(X, Y, W, XW, datafit, all_feats)
 
-            # The intercept is not taken into account in the optimality conditions since
-            # the derivative w.r.t. to the intercept may be very large. It is not likely
-            # to change significantly the optimality conditions.
             if self.ws_strategy == "subdiff":
-                opt = penalty.subdiff_distance(w[:n_features], grad, all_feats)
+                opt = penalty.subdiff_distance(W, grad, all_feats)
             elif self.ws_strategy == "fixpoint":
-                opt = dist_fix_point(w[:n_features], grad, datafit, penalty, all_feats)
-
-            if self.fit_intercept:
-                intercept_opt = np.abs(datafit.intercept_update_step(y, Xw))
-            else:
-                intercept_opt = 0.
-
-            stop_crit = max(np.max(opt), intercept_opt)
-
+                opt = dist_fix_point(W, grad, datafit, penalty, all_feats)
+            stop_crit = np.max(opt)
             if self.verbose:
                 print(f"Stopping criterion max violation: {stop_crit:.2e}")
             if stop_crit <= self.tol:
                 break
             # 1) select features : all unpenalized, + 2 * (nnz and penalized)
-            ws_size = max(min(self.p0 + n_unpen, n_features),
-                          min(2 * penalty.generalized_support(w[:n_features]).sum() -
-                              n_unpen, n_features))
-
+            # TODO fix p0 takes the intercept into account
+            ws_size = min(n_features, max(2 * (norm(W, axis=1) != 0).sum() - n_unpen,
+                                          self.p0 + n_unpen))
             opt[unpen] = np.inf  # always include unpenalized features
-            opt[penalty.generalized_support(w[:n_features])] = np.inf
-
-            # here use topk instead of np.argsort(opt)[-ws_size:]
+            opt[norm(W[:n_features], axis=1) != 0] = np.inf  # TODO check
             ws = np.argpartition(opt, -ws_size)[-ws_size:]
+            # is equivalent to ws = np.argsort(kkt)[-ws_size:]
 
-            # re init AA at every iter to consider ws
-            accelerator = AndersonAcceleration(K=5)
-            w_acc[:] = 0.
-            # ws to be used in AndersonAcceleration
-            ws_intercept = np.append(ws, -1) if self.fit_intercept else ws
+            if self.use_acc:
+                last_K_w = np.zeros([K + 1,
+                                     (ws_size + self.fit_intercept) * n_tasks])
+                U = np.zeros([K, (ws_size + self.fit_intercept) * n_tasks])
 
             if self.verbose:
                 print(f'Iteration {t + 1}, {ws_size} feats in subpb.')
 
             # 2) do iterations on smaller problem
             is_sparse = sparse.issparse(X)
             for epoch in range(self.max_epochs):
                 if is_sparse:
-                    _cd_epoch_sparse(
-                        X.data, X.indptr, X.indices, y, w[:n_features], Xw,
-                        datafit, penalty, ws)
+                    _bcd_epoch_sparse(
+                        X.data, X.indptr, X.indices, Y, W, XW, datafit, penalty,
+                        ws)
                 else:
-                    _cd_epoch(X, y, w[:n_features], Xw, datafit, penalty, ws)
-
+                    _bcd_epoch(X, Y, W, XW, datafit, penalty, ws)
                 # update intercept
                 if self.fit_intercept:
-                    intercept_old = w[-1]
-                    w[-1] -= datafit.intercept_update_step(y, Xw)
-                    Xw += (w[-1] - intercept_old)
-
-                # 3) do Anderson acceleration on smaller problem
-                w_acc[ws_intercept], Xw_acc[:], is_extrap = accelerator.extrapolate(
-                    w[ws_intercept], Xw)
-
-                if is_extrap:  # avoid computing p_obj for un-extrapolated w, Xw
-                    # TODO : manage penalty.value(w, ws) for weighted Lasso
-                    p_obj = (datafit.value(y, w[:n_features], Xw) +
-                             penalty.value(w[:n_features]))
-                    p_obj_acc = (datafit.value(y, w_acc[:n_features], Xw_acc) +
-                                 penalty.value(w_acc[:n_features]))
-
-                    if p_obj_acc < p_obj:
-                        w[:], Xw[:] = w_acc, Xw_acc
-                        p_obj = p_obj_acc
+                    intercept_old = W[-1, :].copy()
+                    W[-1, :] -= datafit.intercept_update_step(Y, XW)
+                    XW += (W[-1, :] - intercept_old)
+
+                if self.use_acc:
+                    if self.fit_intercept:
+                        ws_ = np.append(ws, -1)
+                    else:
+                        ws_ = ws.copy()
+                    last_K_w[epoch % (K + 1)] = W[ws_, :].ravel()
+
+                    # 3) do Anderson acceleration on smaller problem
+                    if epoch % (K + 1) == K:
+                        for k in range(K):
+                            U[k] = last_K_w[k + 1] - last_K_w[k]
+                        C = np.dot(U, U.T)
+
+                        try:
+                            z = np.linalg.solve(C, np.ones(K))
+                            c = z / z.sum()
+                            W_acc = np.zeros((n_features + self.fit_intercept, n_tasks))
+                            W_acc[ws_, :] = np.sum(
+                                last_K_w[:-1] * c[:, None], axis=0).reshape(
+                                    (ws_size + self.fit_intercept, n_tasks))
+                            p_obj = datafit.value(Y, W, XW) + penalty.value(W)
+                            Xw_acc = (X[:, ws] @ W_acc[ws]
+                                      + self.fit_intercept * W_acc[-1])
+                            p_obj_acc = datafit.value(
+                                Y, W_acc, Xw_acc) + penalty.value(W_acc)
+                            if p_obj_acc < p_obj:
+                                W[:] = W_acc
+                                XW[:] = Xw_acc
+                        except np.linalg.LinAlgError:
+                            if max(self.verbose - 1, 0):
+                                print("----------Linalg error")
+
+                if epoch > 0 and epoch % 10 == 0:
+                    p_obj = datafit.value(Y, W[ws, :], XW) + penalty.value(W)
 
-                if epoch % 10 == 0:
                     if is_sparse:
                         grad_ws = construct_grad_sparse(
-                            X.data, X.indptr, X.indices, y, w, Xw, datafit, ws)
+                            X.data, X.indptr, X.indices, Y, XW, datafit, ws)
                     else:
-                        grad_ws = construct_grad(X, y, w, Xw, datafit, ws)
+                        grad_ws = construct_grad(X, Y, W, XW, datafit, ws)
+
                     if self.ws_strategy == "subdiff":
-                        opt_ws = penalty.subdiff_distance(w[:n_features], grad_ws, ws)
+                        opt_ws = penalty.subdiff_distance(W, grad_ws, ws)
                     elif self.ws_strategy == "fixpoint":
-                        opt_ws = dist_fix_point(
-                            w[:n_features], grad_ws, datafit, penalty, ws)
+                        opt_ws = dist_fix_point(W, grad_ws, datafit, penalty, ws)
 
                     stop_crit_in = np.max(opt_ws)
                     if max(self.verbose - 1, 0):
-                        p_obj = (datafit.value(y, w[:n_features], Xw) +
-                                 penalty.value(w[:n_features]))
                         print(f"Epoch {epoch + 1}, objective {p_obj:.10f}, "
                               f"stopping crit {stop_crit_in:.2e}")
                     if ws_size == n_features:
                         if stop_crit_in <= self.tol:
                             break
                     else:
                         if stop_crit_in < 0.3 * stop_crit:
                             if max(self.verbose - 1, 0):
                                 print("Early exit")
                             break
-            p_obj = datafit.value(y, w[:n_features], Xw) + penalty.value(w[:n_features])
             obj_out.append(p_obj)
-        return w, np.array(obj_out), stop_crit
+        return W, np.array(obj_out), stop_crit
 
-    def path(self, X, y, datafit, penalty, alphas=None, w_init=None,
-             return_n_iter=False):
-        X = check_array(X, 'csc', dtype=[np.float64, np.float32],
-                        order='F', copy=False, accept_large_sparse=False)
-        y = check_array(y, 'csc', dtype=X.dtype.type, order='F', copy=False,
-                        ensure_2d=False)
+    def path(self, X, Y, datafit, penalty, alphas, W_init=None, return_n_iter=False):
+        X = check_array(X, "csc", dtype=[
+            np.float64, np.float32], order="F", copy=False)
+        Y = check_array(Y, "csc", dtype=[
+            np.float64, np.float32], order="F", copy=False)
         if sparse.issparse(X):
-            datafit.initialize_sparse(X.data, X.indptr, X.indices, y)
+            datafit.initialize_sparse(X.data, X.indptr, X.indices, Y)
         else:
-            datafit.initialize(X, y)
+            datafit.initialize(X, Y)
         n_features = X.shape[1]
+        n_tasks = Y.shape[1]
         if alphas is None:
-            raise ValueError('alphas should be passed explicitly')
-
+            raise ValueError("alphas should be provided.")
         n_alphas = len(alphas)
-        coefs = np.zeros((n_features + self.fit_intercept, n_alphas), order='F',
-                         dtype=X.dtype)
+
+        coefs = np.zeros((n_features + self.fit_intercept, n_tasks, n_alphas),
+                         order="C", dtype=X.dtype)
         stop_crits = np.zeros(n_alphas)
         p0 = self.p0
 
         if return_n_iter:
             n_iters = np.zeros(n_alphas, dtype=int)
 
+        Y = np.asfortranarray(Y)
+        XW = np.zeros(Y.shape, order='F')
         for t in range(n_alphas):
             alpha = alphas[t]
-            penalty.alpha = alpha
+            penalty.alpha = alpha  # TODO this feels it will break sklearn compat
             if self.verbose:
-                to_print = "##### Computing alpha %d/%d" % (t + 1, n_alphas)
-                print("#" * len(to_print))
-                print(to_print)
-                print("#" * len(to_print))
+                msg = "##### Computing alpha %d/%d" % (t + 1, n_alphas)
+                print("#" * len(msg))
+                print(msg)
+                print("#" * len(msg))
             if t > 0:
-                w = coefs[:, t - 1].copy()
-                # TODO tmp fix debug for L05:  p0 > replace by 1 (?)
-                p0 = max(np.sum(penalty.generalized_support(w)), p0)
+                W = coefs[:, :, t - 1].copy()
+                p0 = max(len(np.where(W[:, 0] != 0)[0]), p0)
             else:
-                if w_init is not None:
-                    w = w_init.copy()
-                    supp_size = penalty.generalized_support(w[:n_features]).sum()
-                    p0 = max(supp_size, p0)
-                    if supp_size:
-                        Xw = X @ w[:n_features] + self.fit_intercept * w[-1]
-                    # TODO explain/clean this hack
-                    else:
-                        Xw = np.zeros_like(y)
+                if W_init is not None:
+                    W = W_init.T
+                    XW = np.asfortranarray(X @ W)
+                    p0 = max(len(np.where(W[:, 0] != 0)[0]), p0)
                 else:
-                    w = np.zeros(n_features + self.fit_intercept, dtype=X.dtype)
-                    Xw = np.zeros(X.shape[0], dtype=X.dtype)
-
-            sol = self.solve(X, y, datafit, penalty, w, Xw)
-
-            coefs[:, t] = sol[0]
-            stop_crits[t] = sol[-1]
+                    W = np.zeros(
+                        (n_features + self.fit_intercept, n_tasks), dtype=X.dtype,
+                        order='C')
+                    p0 = 10
+            sol = self.solve(X, Y, datafit, penalty, W, XW)
+            coefs[:, :, t], stop_crits[t] = sol[0], sol[2]
 
             if return_n_iter:
                 n_iters[t] = len(sol[1])
 
+        coefs = np.swapaxes(coefs, 0, 1).copy('F')
+
         results = alphas, coefs, stop_crits
         if return_n_iter:
             results += (n_iters,)
+
         return results
 
 
 @njit
-def _cd_epoch(X, y, w, Xw, datafit, penalty, ws):
-    """Run an epoch of coordinate descent in place.
+def dist_fix_point(W, grad_ws, datafit, penalty, ws):
+    """Compute the violation of the fixed point iterate schema.
+
+    Parameters
+    ----------
+    W : array, shape (n_features, n_tasks)
+        Coefficient matrix.
+
+    grad_ws : array, shape (ws_size, n_tasks)
+        Gradient restricted to the working set.
+
+    datafit: instance of BaseMultiTaskDatafit
+        Datafit.
+
+    penalty: instance of BasePenalty
+        Penalty.
+
+    ws : array, shape (ws_size,)
+        The working set.
+
+    Returns
+    -------
+    dist_fix_point : array, shape (ws_size,)
+        Contain the violation score for every feature.
+    """
+    dist_fix_point = np.zeros(ws.shape[0])
+    for idx, j in enumerate(ws):
+        lcj = datafit.lipschitz[j]
+        if lcj:
+            dist_fix_point[idx] = norm(
+                W[j] - penalty.prox_1feat(W[j] - grad_ws[idx] / lcj, 1. / lcj, j))
+    return dist_fix_point
+
+
+@njit
+def construct_grad(X, Y, W, XW, datafit, ws):
+    """Compute the gradient of the datafit restricted to the working set.
 
     Parameters
     ----------
     X : array, shape (n_samples, n_features)
         Design matrix.
 
-    y : array, shape (n_samples,)
-        Target vector.
+    Y : array, shape (n_samples, n_tasks)
+        Target matrix.
 
-    w : array, shape (n_features,)
-        Coefficient vector.
+    W : array, shape (n_features, n_tasks)
+        Coefficient matrix.
 
-    Xw : array, shape (n_samples,)
+    XW : array, shape (n_samples, n_tasks)
         Model fit.
 
-    datafit : Datafit
+    datafit : instance of BaseMultiTaskDatafit
         Datafit.
 
-    penalty : Penalty
+    ws : array, shape (ws_size,)
+        The working set.
+
+    Returns
+    -------
+    grad : array, shape (ws_size, n_tasks)
+        The gradient restricted to the working set.
+    """
+    n_tasks = XW.shape[1]
+    grad = np.zeros((ws.shape[0], n_tasks))
+    for idx, j in enumerate(ws):
+        grad[idx, :] = datafit.gradient_j(X, Y, W, XW, j)
+    return grad
+
+
+@njit
+def construct_grad_sparse(data, indptr, indices, Y, XW, datafit, ws):
+    """Compute the gradient of the datafit restricted to the working set.
+
+    Parameters
+    ----------
+    data : array-like
+        Data array of the matrix in CSC format.
+
+    indptr : array-like
+        CSC format index point array.
+
+    indices : array-like
+        CSC format index array.
+
+    Y : array, shape (n_samples, n_tasks)
+        Target matrix.
+
+    XW : array, shape (n_samples, n_tasks)
+        Model fit.
+
+    datafit : instance of BaseMultiTaskDatafit
+        Datafit.
+
+    ws : array, shape (ws_size,)
+        The working set.
+
+    Returns
+    -------
+    grad : array, shape (ws_size, n_tasks)
+        The gradient restricted to the working set.
+    """
+    n_tasks = XW.shape[1]
+    grad = np.zeros((ws.shape[0], n_tasks))
+    for idx, j in enumerate(ws):
+        grad[idx, :] = datafit.gradient_j_sparse(
+            data, indptr, indices, Y, XW, j)
+    return grad
+
+
+@njit
+def _bcd_epoch(X, Y, W, XW, datafit, penalty, ws):
+    """Run an epoch of block coordinate descent in place.
+
+    Parameters
+    ----------
+    X : array, shape (n_samples, n_features)
+        Design matrix.
+
+    Y : array, shape (n_samples, n_tasks)
+        Target matrix.
+
+    W : array, shape (n_features, n_tasks)
+        Coefficient matrix.
+
+    XW : array, shape (n_samples, n_tasks)
+        Model fit.
+
+    datafit : instance of BaseMultiTaskDatafit
+        Datafit.
+
+    penalty : instance of BasePenalty
         Penalty.
 
     ws : array, shape (ws_size,)
-        The range of features.
+        The working set.
     """
     lc = datafit.lipschitz
+    n_tasks = Y.shape[1]
     for j in ws:
-        stepsize = 1/lc[j] if lc[j] != 0 else 1000
+        if lc[j] == 0.:
+            continue
         Xj = X[:, j]
-        old_w_j = w[j]
-        w[j] = penalty.prox_1d(
-            old_w_j - datafit.gradient_scalar(X, y, w, Xw, j) * stepsize,
-            stepsize, j)
-        if w[j] != old_w_j:
-            Xw += (w[j] - old_w_j) * Xj
+        old_W_j = W[j, :].copy()  # copy is very important here
+        W[j, :] = penalty.prox_1feat(
+            W[j, :] - datafit.gradient_j(X, Y, W, XW, j) / lc[j],
+            1 / lc[j], j)
+        if not np.all(W[j, :] == old_W_j):
+            for k in range(n_tasks):
+                tmp = W[j, k] - old_W_j[k]
+                if tmp != 0:
+                    XW[:, k] += tmp * Xj
 
 
 @njit
-def _cd_epoch_sparse(X_data, X_indptr, X_indices, y, w, Xw, datafit, penalty, ws):
-    """Run an epoch of coordinate descent in place for a sparse CSC array.
+def _bcd_epoch_sparse(X_data, X_indptr, X_indices, Y, W, XW, datafit, penalty, ws):
+    """Run an epoch of block coordinate descent in place for a sparse CSC array.
 
     Parameters
     ----------
     X_data : array, shape (n_elements,)
         `data` attribute of the sparse CSC matrix X.
 
     X_indptr : array, shape (n_features + 1,)
         `indptr` attribute of the sparse CSC matrix X.
 
     X_indices : array, shape (n_elements,)
         `indices` attribute of the sparse CSC matrix X.
 
-    y : array, shape (n_samples,)
-        Target vector.
+    Y : array, shape (n_samples, n_tasks)
+        Target matrix.
 
-    w : array, shape (n_features,)
-        Coefficient vector.
+    W : array, shape (n_features, n_tasks)
+        Coefficient matrix.
 
-    Xw : array, shape (n_samples,)
+    XW : array, shape (n_samples, n_tasks)
         Model fit.
 
-    datafit : Datafit
+    datafit : instance of BaseMultiTaskDatafit
         Datafit.
 
-    penalty : Penalty
+    penalty : instance of BasePenalty
         Penalty.
 
     ws : array, shape (ws_size,)
-        The working set.
+        Features to be updated.
     """
     lc = datafit.lipschitz
     for j in ws:
-        stepsize = 1/lc[j] if lc[j] != 0 else 1000
-
-        old_w_j = w[j]
-        gradj = datafit.gradient_scalar_sparse(X_data, X_indptr, X_indices, y, Xw, j)
-        w[j] = penalty.prox_1d(
-            old_w_j - gradj * stepsize, stepsize, j)
-        diff = w[j] - old_w_j
-        if diff != 0:
+        if lc[j] == 0.:
+            continue
+        old_W_j = W[j, :].copy()
+        grad_j = datafit.gradient_j_sparse(X_data, X_indptr, X_indices, Y, XW, j)
+        W[j] = penalty.prox_1feat(
+            old_W_j - grad_j / lc[j], 1 / lc[j], j)
+        # TODO: could be enhanced?
+        diff = W[j, :] - old_W_j
+        if not np.all(diff == 0):
             for i in range(X_indptr[j], X_indptr[j + 1]):
-                Xw[X_indices[i]] += diff * X_data[i]
+                for t in range(Y.shape[1]):
+                    XW[X_indices[i], t] += diff[t] * X_data[i]
```

### Comparing `skglm-0.2/skglm/solvers/base.py` & `skglm-0.3/skglm/solvers/base.py`

 * *Files identical despite different names*

### Comparing `skglm-0.2/skglm/solvers/common.py` & `skglm-0.3/skglm/solvers/common.py`

 * *Files identical despite different names*

### Comparing `skglm-0.2/skglm/solvers/gram_cd.py` & `skglm-0.3/skglm/solvers/gram_cd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 import warnings
 import numpy as np
 from numba import njit
 from scipy.sparse import issparse
 from skglm.solvers.base import BaseSolver
-from skglm.utils import AndersonAcceleration
+from skglm.utils.anderson import AndersonAcceleration
 
 
 class GramCD(BaseSolver):
     r"""Coordinate descent solver keeping the gradients up-to-date with Gram updates.
 
-    This solver should be used when n_features < n_samples, and computes the
-    (n_features, n_features) Gram matrix which comes with an overhead. It is  only
-    suited to Quadratic datafits.
+    This solver should be used when ``n_features`` < ``n_samples``, and computes the
+    (``n_features``, ``n_features``) Gram matrix which comes with an overhead. It is
+    only suited to Quadratic datafits.
 
-    It minimizes::
-        1 / (2*n_samples) * norm(y - Xw)**2 + penalty(w)
+    It minimizes:
 
-    which can be rewritten as::
-        w.T @ Q @ w / (2*n_samples) - q.T @ w / n_samples + penalty(w)
+    .. math:: 1 / (2 xx n_"samples") ||y - Xw||^2 + "penalty"(w)
 
-    where::
-        Q = X.T @ X (gram matrix), and q = X.T @ y
+    which can be rewritten as:
+
+    .. math:: 1 / (2 xx n_"samples") w^T Q w - 1 / n_"samples" q^T w + "penalty"(w)
+
+    where:
+
+    .. math:: Q = X^T X " (gram matrix),  and " q = X^T y
 
     Attributes
     ----------
     max_iter : int, default 100
         Maximum number of iterations.
 
     w_init : array, shape (n_features,), default None
         Initial value of coefficients.
-        If set to None, a zero vector is used instead.
+        If set to ``None``, a zero vector is used instead.
 
     use_acc : bool, default True
-        Extrapolate the iterates based on the past 5 iterates if set to True.
+        Extrapolate the iterates based on the past 5 iterates if set to ``True``.
 
     greedy_cd : bool, default True
         Use a greedy strategy to select features to update in coordinate descent epochs
-        if set to True. A cyclic strategy is used otherwise.
+        if set to ``True``. A cyclic strategy is used otherwise.
 
     tol : float, default 1e-4
         Tolerance for convergence.
 
     verbose : bool, default False
         Amount of verbosity. 0/False is silent.
     """
```

### Comparing `skglm-0.2/skglm/solvers/group_bcd.py` & `skglm-0.3/skglm/solvers/group_bcd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
 from numba import njit
+
 from skglm.solvers.base import BaseSolver
-from skglm.utils import AndersonAcceleration, check_group_compatible
+from skglm.utils.anderson import AndersonAcceleration
+from skglm.utils.validation import check_group_compatible
 
 
 class GroupBCD(BaseSolver):
     """Block coordinate descent solver for group problems.
 
     Attributes
     ----------
@@ -166,10 +168,10 @@
     grp_ptr = datafit.grp_ptr
     n_features_ws = sum([grp_ptr[g+1] - grp_ptr[g] for g in ws])
 
     grads = np.zeros(n_features_ws)
     grad_ptr = 0
     for g in ws:
         grad_g = datafit.gradient_g(X, y, w, Xw, g)
-        grads[grad_ptr: grad_ptr+len(grad_g)] = -grad_g
+        grads[grad_ptr: grad_ptr+len(grad_g)] = grad_g
         grad_ptr += len(grad_g)
     return grads
```

### Comparing `skglm-0.2/skglm/solvers/multitask_bcd.py` & `skglm-0.3/skglm/solvers/prox_newton.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,428 +1,438 @@
+import warnings
+
 import numpy as np
-from scipy import sparse
 from numba import njit
-from numpy.linalg import norm
-from sklearn.utils import check_array
+from scipy.sparse import issparse
 from skglm.solvers.base import BaseSolver
 
+from sklearn.exceptions import ConvergenceWarning
+from skglm.utils.sparse_ops import _sparse_xj_dot
 
-class MultiTaskBCD(BaseSolver):
-    """Block coordinate descent solver for multi-task problems."""
+EPS_TOL = 0.3
+MAX_CD_ITER = 20
+MAX_BACKTRACK_ITER = 20
 
-    def __init__(self, max_iter=100, max_epochs=50_000, p0=10, tol=1e-6,
-                 use_acc=True, ws_strategy="subdiff", fit_intercept=True,
-                 warm_start=False, verbose=0):
-        self.max_iter = max_iter
-        self.max_epochs = max_epochs
+
+class ProxNewton(BaseSolver):
+    """Prox Newton solver combined with working sets.
+
+    p0 : int, default 10
+        Minimum number of features to be included in the working set.
+
+    max_iter : int, default 20
+        Maximum number of outer iterations.
+
+    max_pn_iter : int, default 1000
+        Maximum number of prox Newton iterations on each subproblem.
+
+    tol : float, default 1e-4
+        Tolerance for convergence.
+
+    fit_intercept : bool, default True
+        If ``True``, fits an unpenalized intercept.
+
+    verbose : bool, default False
+        Amount of verbosity. 0/False is silent.
+
+    References
+    ----------
+    .. [1] Massias, M. and Vaiter, S. and Gramfort, A. and Salmon, J.
+        "Dual Extrapolation for Sparse Generalized Linear Models", JMLR, 2020,
+        https://arxiv.org/abs/1907.05830
+        code: https://github.com/mathurinm/celer
+
+    .. [2] Johnson, T. B. and Guestrin, C.
+        "Blitz: A principled meta-algorithm for scaling sparse optimization",
+        ICML, 2015.
+        https://proceedings.mlr.press/v37/johnson15.html
+        code: https://github.com/tbjohns/BlitzL1
+    """
+
+    def __init__(self, p0=10, max_iter=20, max_pn_iter=1000, tol=1e-4,
+                 fit_intercept=True, warm_start=False, verbose=0):
         self.p0 = p0
+        self.max_iter = max_iter
+        self.max_pn_iter = max_pn_iter
         self.tol = tol
-        self.use_acc = use_acc
-        self.ws_strategy = ws_strategy
         self.fit_intercept = fit_intercept
         self.warm_start = warm_start
         self.verbose = verbose
 
-    def solve(self, X, Y, datafit, penalty, W_init=None, XW_init=None):
+    def solve(self, X, y, datafit, penalty, w_init=None, Xw_init=None):
+        dtype = X.dtype
         n_samples, n_features = X.shape
-        n_tasks = Y.shape[1]
-        pen = penalty.is_penalized(n_features)
-        unpen = ~pen
-        n_unpen = unpen.sum()
-        obj_out = []
-        all_feats = np.arange(n_features)
-        stop_crit = np.inf  # initialize for case n_iter=0
-        K = 5
-
-        W = (np.zeros((n_features + self.fit_intercept, n_tasks)) if W_init is None
-             else W_init)
-        XW = np.zeros((n_samples, n_tasks)) if XW_init is None else XW_init
+        fit_intercept = self.fit_intercept
+
+        w = np.zeros(n_features + fit_intercept, dtype) if w_init is None else w_init
+        Xw = np.zeros(n_samples, dtype) if Xw_init is None else Xw_init
+        all_features = np.arange(n_features)
+        stop_crit = 0.
+        p_objs_out = []
 
-        if W.shape[0] != n_features + self.fit_intercept:
+        is_sparse = issparse(X)
+        if is_sparse:
+            X_bundles = (X.data, X.indptr, X.indices)
+
+        if len(w) != n_features + self.fit_intercept:
             if self.fit_intercept:
                 val_error_message = (
-                    "W.shape[0] should be n_features + 1 when using fit_intercept=True:"
-                    f" expected {n_features + 1}, got {W.shape[0]}.")
+                    "w should be of size n_features + 1 when using fit_intercept=True: "
+                    f"expected {n_features + 1}, got {len(w)}.")
             else:
                 val_error_message = (
-                    "W.shape[0] should be of size n_features: "
-                    f"expected {n_features}, got {W.shape[0]}.")
+                    "w should be of size n_features: "
+                    f"expected {n_features}, got {len(w)}.")
             raise ValueError(val_error_message)
 
-        is_sparse = sparse.issparse(X)
-        if is_sparse:
-            datafit.initialize_sparse(X.data, X.indptr, X.indices, Y)
-        else:
-            datafit.initialize(X, Y)
-
         for t in range(self.max_iter):
+            # compute scores
             if is_sparse:
-                grad = datafit.full_grad_sparse(
-                    X.data, X.indptr, X.indices, Y, XW)
+                grad = _construct_grad_sparse(
+                    *X_bundles, y, w[:n_features], Xw, datafit, all_features)
             else:
-                grad = construct_grad(X, Y, W, XW, datafit, all_feats)
+                grad = _construct_grad(X, y, w[:n_features], Xw, datafit, all_features)
 
-            if self.ws_strategy == "subdiff":
-                opt = penalty.subdiff_distance(W, grad, all_feats)
-            elif self.ws_strategy == "fixpoint":
-                opt = dist_fix_point(W, grad, datafit, penalty, all_feats)
-            stop_crit = np.max(opt)
+            opt = penalty.subdiff_distance(w[:n_features], grad, all_features)
+
+            # optimality of intercept
+            if fit_intercept:
+                # gradient w.r.t. intercept (constant features of ones)
+                intercept_opt = np.abs(np.sum(datafit.raw_grad(y, Xw)))
+            else:
+                intercept_opt = 0.
+
+            # check convergences
+            stop_crit = max(np.max(opt), intercept_opt)
             if self.verbose:
-                print(f"Stopping criterion max violation: {stop_crit:.2e}")
+                p_obj = datafit.value(y, w, Xw) + penalty.value(w[:n_features])
+                print(
+                    "Iteration {}: {:.10f}, ".format(t+1, p_obj) +
+                    "stopping crit: {:.2e}".format(stop_crit)
+                )
+
             if stop_crit <= self.tol:
+                if self.verbose:
+                    print("Stopping criterion max violation: {:.2e}".format(stop_crit))
                 break
-            # 1) select features : all unpenalized, + 2 * (nnz and penalized)
-            # TODO fix p0 takes the intercept into account
-            ws_size = min(n_features, max(2 * (norm(W, axis=1) != 0).sum() - n_unpen,
-                                          self.p0 + n_unpen))
-            opt[unpen] = np.inf  # always include unpenalized features
-            opt[norm(W[:n_features], axis=1) != 0] = np.inf  # TODO check
-            ws = np.argpartition(opt, -ws_size)[-ws_size:]
-            # is equivalent to ws = np.argsort(kkt)[-ws_size:]
 
-            if self.use_acc:
-                last_K_w = np.zeros([K + 1,
-                                     (ws_size + self.fit_intercept) * n_tasks])
-                U = np.zeros([K, (ws_size + self.fit_intercept) * n_tasks])
+            # build working set
+            gsupp_size = penalty.generalized_support(w).sum()
+            ws_size = max(min(self.p0, n_features),
+                          min(n_features, 2 * gsupp_size))
+            # similar to np.argsort()[-ws_size:] but without sorting
+            ws = np.argpartition(opt, -ws_size)[-ws_size:]
 
-            if self.verbose:
-                print(f'Iteration {t + 1}, {ws_size} feats in subpb.')
+            grad_ws = grad[ws]
+            tol_in = EPS_TOL * stop_crit
 
-            # 2) do iterations on smaller problem
-            is_sparse = sparse.issparse(X)
-            for epoch in range(self.max_epochs):
+            for pn_iter in range(self.max_pn_iter):
+                # find descent direction
                 if is_sparse:
-                    _bcd_epoch_sparse(
-                        X.data, X.indptr, X.indices, Y, W, XW, datafit, penalty,
-                        ws)
+                    delta_w_ws, X_delta_w_ws = _descent_direction_s(
+                        *X_bundles, y, w, Xw, fit_intercept, grad_ws, datafit,
+                        penalty, ws, tol=EPS_TOL*tol_in)
                 else:
-                    _bcd_epoch(X, Y, W, XW, datafit, penalty, ws)
-                # update intercept
-                if self.fit_intercept:
-                    intercept_old = W[-1, :].copy()
-                    W[-1, :] -= datafit.intercept_update_step(Y, XW)
-                    XW += (W[-1, :] - intercept_old)
-
-                if self.use_acc:
-                    if self.fit_intercept:
-                        ws_ = np.append(ws, -1)
-                    else:
-                        ws_ = ws.copy()
-                    last_K_w[epoch % (K + 1)] = W[ws_, :].ravel()
-
-                    # 3) do Anderson acceleration on smaller problem
-                    if epoch % (K + 1) == K:
-                        for k in range(K):
-                            U[k] = last_K_w[k + 1] - last_K_w[k]
-                        C = np.dot(U, U.T)
-
-                        try:
-                            z = np.linalg.solve(C, np.ones(K))
-                            c = z / z.sum()
-                            W_acc = np.zeros((n_features + self.fit_intercept, n_tasks))
-                            W_acc[ws_, :] = np.sum(
-                                last_K_w[:-1] * c[:, None], axis=0).reshape(
-                                    (ws_size + self.fit_intercept, n_tasks))
-                            p_obj = datafit.value(Y, W, XW) + penalty.value(W)
-                            Xw_acc = (X[:, ws] @ W_acc[ws]
-                                      + self.fit_intercept * W_acc[-1])
-                            p_obj_acc = datafit.value(
-                                Y, W_acc, Xw_acc) + penalty.value(W_acc)
-                            if p_obj_acc < p_obj:
-                                W[:] = W_acc
-                                XW[:] = Xw_acc
-                        except np.linalg.LinAlgError:
-                            if max(self.verbose - 1, 0):
-                                print("----------Linalg error")
-
-                if epoch > 0 and epoch % 10 == 0:
-                    p_obj = datafit.value(Y, W[ws, :], XW) + penalty.value(W)
-
-                    if is_sparse:
-                        grad_ws = construct_grad_sparse(
-                            X.data, X.indptr, X.indices, Y, XW, datafit, ws)
-                    else:
-                        grad_ws = construct_grad(X, Y, W, XW, datafit, ws)
-
-                    if self.ws_strategy == "subdiff":
-                        opt_ws = penalty.subdiff_distance(W, grad_ws, ws)
-                    elif self.ws_strategy == "fixpoint":
-                        opt_ws = dist_fix_point(W, grad_ws, datafit, penalty, ws)
-
-                    stop_crit_in = np.max(opt_ws)
-                    if max(self.verbose - 1, 0):
-                        print(f"Epoch {epoch + 1}, objective {p_obj:.10f}, "
-                              f"stopping crit {stop_crit_in:.2e}")
-                    if ws_size == n_features:
-                        if stop_crit_in <= self.tol:
-                            break
-                    else:
-                        if stop_crit_in < 0.3 * stop_crit:
-                            if max(self.verbose - 1, 0):
-                                print("Early exit")
-                            break
-            obj_out.append(p_obj)
-        return W, np.array(obj_out), stop_crit
-
-    def path(self, X, Y, datafit, penalty, alphas, W_init=None, return_n_iter=False):
-        X = check_array(X, "csc", dtype=[
-            np.float64, np.float32], order="F", copy=False)
-        Y = check_array(Y, "csc", dtype=[
-            np.float64, np.float32], order="F", copy=False)
-        if sparse.issparse(X):
-            datafit.initialize_sparse(X.data, X.indptr, X.indices, Y)
-        else:
-            datafit.initialize(X, Y)
-        n_features = X.shape[1]
-        n_tasks = Y.shape[1]
-        if alphas is None:
-            raise ValueError("alphas should be provided.")
-        n_alphas = len(alphas)
-
-        coefs = np.zeros((n_features + self.fit_intercept, n_tasks, n_alphas),
-                         order="C", dtype=X.dtype)
-        stop_crits = np.zeros(n_alphas)
-        p0 = self.p0
-
-        if return_n_iter:
-            n_iters = np.zeros(n_alphas, dtype=int)
-
-        Y = np.asfortranarray(Y)
-        XW = np.zeros(Y.shape, order='F')
-        for t in range(n_alphas):
-            alpha = alphas[t]
-            penalty.alpha = alpha  # TODO this feels it will break sklearn compat
-            if self.verbose:
-                msg = "##### Computing alpha %d/%d" % (t + 1, n_alphas)
-                print("#" * len(msg))
-                print(msg)
-                print("#" * len(msg))
-            if t > 0:
-                W = coefs[:, :, t - 1].copy()
-                p0 = max(len(np.where(W[:, 0] != 0)[0]), p0)
-            else:
-                if W_init is not None:
-                    W = W_init.T
-                    XW = np.asfortranarray(X @ W)
-                    p0 = max(len(np.where(W[:, 0] != 0)[0]), p0)
+                    delta_w_ws, X_delta_w_ws = _descent_direction(
+                        X, y, w, Xw, fit_intercept, grad_ws, datafit,
+                        penalty, ws, tol=EPS_TOL*tol_in)
+
+                # backtracking line search with inplace update of w, Xw
+                if is_sparse:
+                    grad_ws[:] = _backtrack_line_search_s(
+                        *X_bundles, y, w, Xw, fit_intercept, datafit, penalty,
+                        delta_w_ws, X_delta_w_ws, ws)
                 else:
-                    W = np.zeros(
-                        (n_features + self.fit_intercept, n_tasks), dtype=X.dtype,
-                        order='C')
-                    p0 = 10
-            sol = self.solve(X, Y, datafit, penalty, W, XW)
-            coefs[:, :, t], stop_crits[t] = sol[0], sol[2]
-
-            if return_n_iter:
-                n_iters[t] = len(sol[1])
-
-        coefs = np.swapaxes(coefs, 0, 1).copy('F')
-
-        results = alphas, coefs, stop_crits
-        if return_n_iter:
-            results += (n_iters,)
+                    grad_ws[:] = _backtrack_line_search(
+                        X, y, w, Xw, fit_intercept, datafit, penalty,
+                        delta_w_ws, X_delta_w_ws, ws)
+
+                # check convergence
+                opt_in = penalty.subdiff_distance(w, grad_ws, ws)
+                stop_crit_in = np.max(opt_in)
+
+                if max(self.verbose-1, 0):
+                    p_obj = datafit.value(y, w, Xw) + penalty.value(w)
+                    print(
+                        "PN iteration {}: {:.10f}, ".format(pn_iter+1, p_obj) +
+                        "stopping crit in: {:.2e}".format(stop_crit_in)
+                    )
+
+                if stop_crit_in <= tol_in:
+                    if max(self.verbose-1, 0):
+                        print("Early exit")
+                    break
 
-        return results
+            p_obj = datafit.value(y, w, Xw) + penalty.value(w)
+            p_objs_out.append(p_obj)
+        else:
+            warnings.warn(
+                f"`ProxNewton` did not converge for tol={self.tol:.3e} "
+                f"and max_iter={self.max_iter}.\n"
+                "Consider increasing `max_iter` and/or `tol`.",
+                category=ConvergenceWarning
+            )
+        return w, np.asarray(p_objs_out), stop_crit
 
 
 @njit
-def dist_fix_point(W, grad_ws, datafit, penalty, ws):
-    """Compute the violation of the fixed point iterate schema.
-
-    Parameters
-    ----------
-    W : array, shape (n_features, n_tasks)
-        Coefficient matrix.
-
-    grad_ws : array, shape (ws_size, n_tasks)
-        Gradient restricted to the working set.
-
-    datafit: instance of BaseMultiTaskDatafit
-        Datafit.
-
-    penalty: instance of BasePenalty
-        Penalty.
-
-    ws : array, shape (ws_size,)
-        The working set.
+def _descent_direction(X, y, w_epoch, Xw_epoch, fit_intercept, grad_ws, datafit,
+                       penalty, ws, tol):
+    # Given:
+    #   1) b = \nabla F(X w_epoch)
+    #   2) D = \nabla^2 F(X w_epoch)  <------>  raw_hess
+    # Minimize quadratic approximation for delta_w = w - w_epoch:
+    #  b.T @ X @ delta_w + \
+    #  1/2 * delta_w.T @ (X.T @ D @ X) @ delta_w + penalty(w)
+    dtype = X.dtype
+    raw_hess = datafit.raw_hessian(y, Xw_epoch)
 
-    Returns
-    -------
-    dist_fix_point : array, shape (ws_size,)
-        Contain the violation score for every feature.
-    """
-    dist_fix_point = np.zeros(ws.shape[0])
+    lipschitz = np.zeros(len(ws), dtype)
     for idx, j in enumerate(ws):
-        lcj = datafit.lipschitz[j]
-        if lcj:
-            dist_fix_point[idx] = norm(
-                W[j] - penalty.prox_1feat(W[j] - grad_ws[idx] / lcj, 1. / lcj, j))
-    return dist_fix_point
-
-
-@njit
-def construct_grad(X, Y, W, XW, datafit, ws):
-    """Compute the gradient of the datafit restricted to the working set.
-
-    Parameters
-    ----------
-    X : array, shape (n_samples, n_features)
-        Design matrix.
-
-    Y : array, shape (n_samples, n_tasks)
-        Target matrix.
-
-    W : array, shape (n_features, n_tasks)
-        Coefficient matrix.
+        lipschitz[idx] = raw_hess @ X[:, j] ** 2
 
-    XW : array, shape (n_samples, n_tasks)
-        Model fit.
+    # for a less costly stopping criterion, we do not compute the exact gradient,
+    # but store each coordinate-wise gradient every time we update one coordinate
+    past_grads = np.zeros(len(ws), dtype)
+    X_delta_w_ws = np.zeros(X.shape[0], dtype)
+    ws_intercept = np.append(ws, -1) if fit_intercept else ws
+    w_ws = w_epoch[ws_intercept]
+
+    if fit_intercept:
+        lipschitz_intercept = np.sum(raw_hess)
+        grad_intercept = np.sum(datafit.raw_grad(y, Xw_epoch))
+
+    for cd_iter in range(MAX_CD_ITER):
+        for idx, j in enumerate(ws):
+            # skip when X[:, j] == 0
+            if lipschitz[idx] == 0:
+                continue
+
+            past_grads[idx] = grad_ws[idx] + X[:, j] @ (raw_hess * X_delta_w_ws)
+            old_w_idx = w_ws[idx]
+            stepsize = 1 / lipschitz[idx]
+
+            w_ws[idx] = penalty.prox_1d(
+                old_w_idx - stepsize * past_grads[idx], stepsize, j)
+
+            if w_ws[idx] != old_w_idx:
+                X_delta_w_ws += (w_ws[idx] - old_w_idx) * X[:, j]
+
+        if fit_intercept:
+            past_grads_intercept = grad_intercept + raw_hess @ X_delta_w_ws
+            old_intercept = w_ws[-1]
+            w_ws[-1] -= past_grads_intercept / lipschitz_intercept
+
+            if w_ws[-1] != old_intercept:
+                X_delta_w_ws += w_ws[-1] - old_intercept
+
+        if cd_iter % 5 == 0:
+            # TODO: can be improved by passing in w_ws but breaks for WeightedL1
+            current_w = w_epoch.copy()
+            current_w[ws_intercept] = w_ws
+            opt = penalty.subdiff_distance(current_w, past_grads, ws)
+            stop_crit = np.max(opt)
 
-    datafit : instance of BaseMultiTaskDatafit
-        Datafit.
+            if fit_intercept:
+                stop_crit = max(stop_crit, np.abs(past_grads_intercept))
 
-    ws : array, shape (ws_size,)
-        The working set.
+            if stop_crit <= tol:
+                break
 
-    Returns
-    -------
-    grad : array, shape (ws_size, n_tasks)
-        The gradient restricted to the working set.
-    """
-    n_tasks = XW.shape[1]
-    grad = np.zeros((ws.shape[0], n_tasks))
-    for idx, j in enumerate(ws):
-        grad[idx, :] = datafit.gradient_j(X, Y, W, XW, j)
-    return grad
+    # descent direction
+    return w_ws - w_epoch[ws_intercept], X_delta_w_ws
 
 
+# sparse version of _descent_direction
 @njit
-def construct_grad_sparse(data, indptr, indices, Y, XW, datafit, ws):
-    """Compute the gradient of the datafit restricted to the working set.
-
-    Parameters
-    ----------
-    data : array-like
-        Data array of the matrix in CSC format.
-
-    indptr : array-like
-        CSC format index point array.
-
-    indices : array-like
-        CSC format index array.
-
-    Y : array, shape (n_samples, n_tasks)
-        Target matrix.
-
-    XW : array, shape (n_samples, n_tasks)
-        Model fit.
-
-    datafit : instance of BaseMultiTaskDatafit
-        Datafit.
+def _descent_direction_s(X_data, X_indptr, X_indices, y, w_epoch,
+                         Xw_epoch, fit_intercept, grad_ws, datafit, penalty, ws, tol):
+    dtype = X_data.dtype
+    raw_hess = datafit.raw_hessian(y, Xw_epoch)
 
-    ws : array, shape (ws_size,)
-        The working set.
-
-    Returns
-    -------
-    grad : array, shape (ws_size, n_tasks)
-        The gradient restricted to the working set.
-    """
-    n_tasks = XW.shape[1]
-    grad = np.zeros((ws.shape[0], n_tasks))
+    lipschitz = np.zeros(len(ws), dtype)
     for idx, j in enumerate(ws):
-        grad[idx, :] = datafit.gradient_j_sparse(
-            data, indptr, indices, Y, XW, j)
-    return grad
-
+        # equivalent to: lipschitz[idx] += raw_hess * X[:, j] ** 2
+        lipschitz[idx] = _sparse_squared_weighted_norm(
+            X_data, X_indptr, X_indices, j, raw_hess)
+
+    # see _descent_direction() comment
+    past_grads = np.zeros(len(ws), dtype)
+    X_delta_w_ws = np.zeros(Xw_epoch.shape[0], dtype)
+    ws_intercept = np.append(ws, -1) if fit_intercept else ws
+    w_ws = w_epoch[ws_intercept]
+
+    if fit_intercept:
+        lipschitz_intercept = np.sum(raw_hess)
+        grad_intercept = np.sum(datafit.raw_grad(y, Xw_epoch))
+
+    for cd_iter in range(MAX_CD_ITER):
+        for idx, j in enumerate(ws):
+            # skip when X[:, j] == 0
+            if lipschitz[idx] == 0:
+                continue
+
+            past_grads[idx] = grad_ws[idx]
+            # equivalent to cached_grads[idx] += X[:, j] @ (raw_hess * X_delta_w_ws)
+            past_grads[idx] += _sparse_weighted_dot(
+                X_data, X_indptr, X_indices, j, X_delta_w_ws, raw_hess)
+
+            old_w_idx = w_ws[idx]
+            stepsize = 1 / lipschitz[idx]
+
+            w_ws[idx] = penalty.prox_1d(
+                old_w_idx - stepsize * past_grads[idx], stepsize, j)
+
+            if w_ws[idx] != old_w_idx:
+                _update_X_delta_w(X_data, X_indptr, X_indices, X_delta_w_ws,
+                                  w_ws[idx] - old_w_idx, j)
+
+        if fit_intercept:
+            past_grads_intercept = grad_intercept + raw_hess @ X_delta_w_ws
+            old_intercept = w_ws[-1]
+            w_ws[-1] -= past_grads_intercept / lipschitz_intercept
+
+            if w_ws[-1] != old_intercept:
+                X_delta_w_ws += w_ws[-1] - old_intercept
+
+        if cd_iter % 5 == 0:
+            # TODO: could be improved by passing in w_ws
+            current_w = w_epoch.copy()
+            current_w[ws_intercept] = w_ws
+            opt = penalty.subdiff_distance(current_w, past_grads, ws)
+            stop_crit = np.max(opt)
 
-@njit
-def _bcd_epoch(X, Y, W, XW, datafit, penalty, ws):
-    """Run an epoch of block coordinate descent in place.
+            if fit_intercept:
+                stop_crit = max(stop_crit, np.abs(past_grads_intercept))
 
-    Parameters
-    ----------
-    X : array, shape (n_samples, n_features)
-        Design matrix.
+            if stop_crit <= tol:
+                break
 
-    Y : array, shape (n_samples, n_tasks)
-        Target matrix.
+    # descent direction
+    return w_ws - w_epoch[ws_intercept], X_delta_w_ws
 
-    W : array, shape (n_features, n_tasks)
-        Coefficient matrix.
 
-    XW : array, shape (n_samples, n_tasks)
-        Model fit.
+@njit
+def _backtrack_line_search(X, y, w, Xw, fit_intercept, datafit, penalty, delta_w_ws,
+                           X_delta_w_ws, ws):
+    # 1) find step in [0, 1] such that:
+    #   penalty(w + step * delta_w) - penalty(w) +
+    #   step * \nabla datafit(w + step * delta_w) @ delta_w < 0
+    # ref: https://www.di.ens.fr/~aspremon/PDF/ENSAE/Newton.pdf
+    # 2) inplace update of w and Xw and return grad_ws of the last w and Xw
+    step, prev_step = 1., 0.
+    n_features = X.shape[1]
+    ws_intercept = np.append(ws, -1) if fit_intercept else ws
+    # TODO: could be improved by passing in w[ws]
+    old_penalty_val = penalty.value(w[:n_features])
+
+    # try step = 1, 1/2, 1/4, ...
+    for _ in range(MAX_BACKTRACK_ITER):
+        w[ws_intercept] += (step - prev_step) * delta_w_ws
+        Xw += (step - prev_step) * X_delta_w_ws
+
+        grad_ws = _construct_grad(X, y, w[:n_features], Xw, datafit, ws)
+        # TODO: could be improved by passing in w[ws]
+        stop_crit = penalty.value(w[:n_features]) - old_penalty_val
+
+        # it is mandatory to split the two operations, otherwise numba raises an error
+        # cf. https://github.com/numba/numba/issues/9025
+        dot = grad_ws @ delta_w_ws[:len(ws)]
+        stop_crit += step * dot
 
-    datafit : instance of BaseMultiTaskDatafit
-        Datafit.
+        if fit_intercept:
+            stop_crit += step * delta_w_ws[-1] * np.sum(datafit.raw_grad(y, Xw))
 
-    penalty : instance of BasePenalty
-        Penalty.
+        if stop_crit < 0:
+            break
+        else:
+            prev_step = step
+            step /= 2
+    else:
+        pass
+        # TODO this case is not handled yet
 
-    ws : array, shape (ws_size,)
-        The working set.
-    """
-    lc = datafit.lipschitz
-    n_tasks = Y.shape[1]
-    for j in ws:
-        if lc[j] == 0.:
-            continue
-        Xj = X[:, j]
-        old_W_j = W[j, :].copy()  # copy is very important here
-        W[j, :] = penalty.prox_1feat(
-            W[j, :] - datafit.gradient_j(X, Y, W, XW, j) / lc[j],
-            1 / lc[j], j)
-        if not np.all(W[j, :] == old_W_j):
-            for k in range(n_tasks):
-                tmp = W[j, k] - old_W_j[k]
-                if tmp != 0:
-                    XW[:, k] += tmp * Xj
+    return grad_ws
 
 
+# sparse version of _backtrack_line_search
 @njit
-def _bcd_epoch_sparse(X_data, X_indptr, X_indices, Y, W, XW, datafit, penalty, ws):
-    """Run an epoch of block coordinate descent in place for a sparse CSC array.
+def _backtrack_line_search_s(X_data, X_indptr, X_indices, y, w, Xw, fit_intercept,
+                             datafit, penalty, delta_w_ws, X_delta_w_ws, ws):
+    step, prev_step = 1., 0.
+    n_features = len(X_indptr) - 1
+    ws_intercept = np.append(ws, -1) if fit_intercept else ws
+    # TODO: could be improved by passing in w[ws]
+    old_penalty_val = penalty.value(w[:n_features])
+
+    for _ in range(MAX_BACKTRACK_ITER):
+        w[ws_intercept] += (step - prev_step) * delta_w_ws
+        Xw += (step - prev_step) * X_delta_w_ws
+
+        grad_ws = _construct_grad_sparse(X_data, X_indptr, X_indices,
+                                         y, w[:n_features], Xw, datafit, ws)
+        # TODO: could be improved by passing in w[ws]
+        stop_crit = penalty.value(w[:n_features]) - old_penalty_val
+
+        # it is mandatory to split the two operations, otherwise numba raises an error
+        # cf. https://github.com/numba/numba/issues/9025
+        dot = grad_ws.T @ delta_w_ws[:len(ws)]
+        stop_crit += step * dot
 
-    Parameters
-    ----------
-    X_data : array, shape (n_elements,)
-        `data` attribute of the sparse CSC matrix X.
+        if fit_intercept:
+            stop_crit += step * delta_w_ws[-1] * np.sum(datafit.raw_grad(y, Xw))
 
-    X_indptr : array, shape (n_features + 1,)
-        `indptr` attribute of the sparse CSC matrix X.
+        if stop_crit < 0:
+            break
+        else:
+            prev_step = step
+            step /= 2
+    else:
+        pass  # TODO
 
-    X_indices : array, shape (n_elements,)
-        `indices` attribute of the sparse CSC matrix X.
+    return grad_ws
 
-    Y : array, shape (n_samples, n_tasks)
-        Target matrix.
 
-    W : array, shape (n_features, n_tasks)
-        Coefficient matrix.
+@njit
+def _construct_grad(X, y, w, Xw, datafit, ws):
+    # Compute grad of datafit restricted to ws. This function avoids
+    # recomputing raw_grad for every j, which is costly for logreg
+    raw_grad = datafit.raw_grad(y, Xw)
+    grad = np.zeros(len(ws), dtype=X.dtype)
+    for idx, j in enumerate(ws):
+        grad[idx] = X[:, j] @ raw_grad
+    return grad
 
-    XW : array, shape (n_samples, n_tasks)
-        Model fit.
 
-    datafit : instance of BaseMultiTaskDatafit
-        Datafit.
+@njit
+def _construct_grad_sparse(X_data, X_indptr, X_indices, y, w, Xw, datafit, ws):
+    # Compute grad of datafit restricted to ws in case X sparse
+    raw_grad = datafit.raw_grad(y, Xw)
+    grad = np.zeros(len(ws), dtype=X_data.dtype)
+    for idx, j in enumerate(ws):
+        grad[idx] = _sparse_xj_dot(X_data, X_indptr, X_indices, j, raw_grad)
+    return grad
 
-    penalty : instance of BasePenalty
-        Penalty.
 
-    ws : array, shape (ws_size,)
-        Features to be updated.
-    """
-    lc = datafit.lipschitz
-    for j in ws:
-        if lc[j] == 0.:
-            continue
-        old_W_j = W[j, :].copy()
-        grad_j = datafit.gradient_j_sparse(X_data, X_indptr, X_indices, Y, XW, j)
-        W[j] = penalty.prox_1feat(
-            old_W_j - grad_j / lc[j], 1 / lc[j], j)
-        # TODO: could be enhanced?
-        diff = W[j, :] - old_W_j
-        if not np.all(diff == 0):
-            for i in range(X_indptr[j], X_indptr[j + 1]):
-                for t in range(Y.shape[1]):
-                    XW[X_indices[i], t] += diff[t] * X_data[i]
+@njit(fastmath=True)
+def _sparse_weighted_dot(X_data, X_indptr, X_indices, j, other, weights):
+    # Compute X[:, j] @ (weights * other) in case X sparse
+    res = 0.
+    for i in range(X_indptr[j], X_indptr[j+1]):
+        res += X_data[i] * other[X_indices[i]] * weights[X_indices[i]]
+    return res
+
+
+@njit(fastmath=True)
+def _sparse_squared_weighted_norm(X_data, X_indptr, X_indices, j, weights):
+    # Compute weights @ X[:, j]**2 in case X sparse
+    res = 0.
+    for i in range(X_indptr[j], X_indptr[j+1]):
+        res += weights[X_indices[i]] * X_data[i]**2
+    return res
+
+
+@njit(fastmath=True)
+def _update_X_delta_w(X_data, X_indptr, X_indices, X_delta_w, diff, j):
+    # Compute X_delta_w += diff * X[:, j] in case of X sparse
+    for i in range(X_indptr[j], X_indptr[j+1]):
+        X_delta_w[X_indices[i]] += diff * X_data[i]
```

### Comparing `skglm-0.2/skglm.egg-info/SOURCES.txt` & `skglm-0.3/skglm.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 LICENSE
-README.rst
+README.md
 setup.py
 skglm/__init__.py
 skglm/estimators.py
-skglm/plot_utils.py
-skglm/utils.py
 skglm.egg-info/PKG-INFO
 skglm.egg-info/SOURCES.txt
 skglm.egg-info/dependency_links.txt
 skglm.egg-info/requires.txt
 skglm.egg-info/top_level.txt
 skglm/datafits/__init__.py
 skglm/datafits/base.py
 skglm/datafits/group.py
 skglm/datafits/multi_task.py
 skglm/datafits/single_task.py
 skglm/experimental/__init__.py
 skglm/experimental/_plot_sqrt_lasso.py
+skglm/experimental/pdcd_ws.py
+skglm/experimental/quantile_regression.py
+skglm/experimental/reweighted.py
 skglm/experimental/sqrt_lasso.py
 skglm/penalties/__init__.py
 skglm/penalties/base.py
 skglm/penalties/block_separable.py
+skglm/penalties/non_separable.py
 skglm/penalties/separable.py
 skglm/solvers/__init__.py
-skglm/solvers/accelerated_cd.py
 skglm/solvers/anderson_cd.py
 skglm/solvers/base.py
 skglm/solvers/common.py
+skglm/solvers/fista.py
 skglm/solvers/gram_cd.py
 skglm/solvers/group_bcd.py
+skglm/solvers/group_prox_newton.py
+skglm/solvers/lbfgs.py
 skglm/solvers/multitask_bcd.py
-skglm/solvers/prox_newton.py
+skglm/solvers/prox_newton.py
+skglm/utils/__init__.py
+skglm/utils/anderson.py
+skglm/utils/data.py
+skglm/utils/jit_compilation.py
+skglm/utils/prox_funcs.py
+skglm/utils/sparse_ops.py
+skglm/utils/validation.py
```

