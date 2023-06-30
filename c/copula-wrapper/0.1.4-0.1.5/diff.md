# Comparing `tmp/copula_wrapper-0.1.4.tar.gz` & `tmp/copula_wrapper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copula_wrapper-0.1.4.tar", max compression
+gzip compressed data, was "copula_wrapper-0.1.5.tar", max compression
```

## Comparing `copula_wrapper-0.1.4.tar` & `copula_wrapper-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     7263 2023-06-28 18:25:54.663437 copula_wrapper-0.1.4/README.md
--rw-r--r--   0        0        0      129 2023-06-28 11:21:57.906760 copula_wrapper-0.1.4/copula_wrapper/__init__.py
--rw-r--r--   0        0        0      849 2023-06-28 11:21:57.920888 copula_wrapper-0.1.4/copula_wrapper/correlation_convert.py
--rw-r--r--   0        0        0    10364 2023-06-30 19:25:33.247988 copula_wrapper-0.1.4/copula_wrapper/joint_distribution.py
--rw-r--r--   0        0        0     1012 2023-06-30 19:25:40.630600 copula_wrapper-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      527 2022-09-15 10:13:48.083787 copula_wrapper-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-28 11:21:57.952446 copula_wrapper-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0      939 2023-06-28 10:46:09.213901 copula_wrapper-0.1.4/tests/e2e/__init__.py
--rw-r--r--   0        0        0      933 2023-06-28 10:46:10.005341 copula_wrapper-0.1.4/tests/e2e/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2536 2023-06-28 10:49:58.377127 copula_wrapper-0.1.4/tests/e2e/__pycache__/test_8_dimensional.cpython-310-pytest-7.4.0.pyc
--rw-r--r--   0        0        0      512 2023-06-28 11:22:23.484423 copula_wrapper-0.1.4/tests/e2e/__pycache__/test_correlation.cpython-310-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3307 2023-06-28 18:41:22.104915 copula_wrapper-0.1.4/tests/e2e/__pycache__/test_marginals.cpython-310-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2481 2023-06-28 10:49:33.844051 copula_wrapper-0.1.4/tests/e2e/test_8_dimensional.py
--rw-r--r--   0        0        0      197 2023-06-28 11:21:57.928787 copula_wrapper-0.1.4/tests/e2e/test_correlation.py
--rw-r--r--   0        0        0     1327 2023-06-28 18:41:21.788761 copula_wrapper-0.1.4/tests/e2e/test_marginals.py
--rw-r--r--   0        0        0    12139 2022-09-15 10:13:48.084054 copula_wrapper-0.1.4/tests/seeds.py
--rw-r--r--   0        0        0      649 2022-09-15 10:13:48.084155 copula_wrapper-0.1.4/tests/shared.py
--rw-r--r--   0        0        0      679 2023-06-28 11:21:57.941382 copula_wrapper-0.1.4/tests/test_copula_param.py
--rw-r--r--   0        0        0      262 2023-06-30 17:51:46.472174 copula_wrapper-0.1.4/tests/test_readme_does_not_raise.py
--rw-r--r--   0        0        0     1821 2023-06-28 18:55:39.953583 copula_wrapper-0.1.4/tests/test_validate_rank_corr.py
--rw-r--r--   0        0        0     7966 1970-01-01 00:00:00.000000 copula_wrapper-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     7263 2023-06-28 18:25:54.663437 copula_wrapper-0.1.5/README.md
+-rw-r--r--   0        0        0      129 2023-06-28 11:21:57.906760 copula_wrapper-0.1.5/copula_wrapper/__init__.py
+-rw-r--r--   0        0        0      849 2023-06-28 11:21:57.920888 copula_wrapper-0.1.5/copula_wrapper/correlation_convert.py
+-rw-r--r--   0        0        0    10380 2023-06-30 19:52:13.110156 copula_wrapper-0.1.5/copula_wrapper/joint_distribution.py
+-rw-r--r--   0        0        0     1012 2023-06-30 19:52:17.093286 copula_wrapper-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      527 2022-09-15 10:13:48.083787 copula_wrapper-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-28 11:21:57.952446 copula_wrapper-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0      939 2023-06-28 10:46:09.213901 copula_wrapper-0.1.5/tests/e2e/__init__.py
+-rw-r--r--   0        0        0      933 2023-06-28 10:46:10.005341 copula_wrapper-0.1.5/tests/e2e/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2536 2023-06-28 10:49:58.377127 copula_wrapper-0.1.5/tests/e2e/__pycache__/test_8_dimensional.cpython-310-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0      512 2023-06-28 11:22:23.484423 copula_wrapper-0.1.5/tests/e2e/__pycache__/test_correlation.cpython-310-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3307 2023-06-28 18:41:22.104915 copula_wrapper-0.1.5/tests/e2e/__pycache__/test_marginals.cpython-310-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2481 2023-06-28 10:49:33.844051 copula_wrapper-0.1.5/tests/e2e/test_8_dimensional.py
+-rw-r--r--   0        0        0      197 2023-06-28 11:21:57.928787 copula_wrapper-0.1.5/tests/e2e/test_correlation.py
+-rw-r--r--   0        0        0     1327 2023-06-28 18:41:21.788761 copula_wrapper-0.1.5/tests/e2e/test_marginals.py
+-rw-r--r--   0        0        0    12139 2022-09-15 10:13:48.084054 copula_wrapper-0.1.5/tests/seeds.py
+-rw-r--r--   0        0        0      649 2022-09-15 10:13:48.084155 copula_wrapper-0.1.5/tests/shared.py
+-rw-r--r--   0        0        0      679 2023-06-28 11:21:57.941382 copula_wrapper-0.1.5/tests/test_copula_param.py
+-rw-r--r--   0        0        0      262 2023-06-30 17:51:46.472174 copula_wrapper-0.1.5/tests/test_readme_does_not_raise.py
+-rw-r--r--   0        0        0     1821 2023-06-28 18:55:39.953583 copula_wrapper-0.1.5/tests/test_validate_rank_corr.py
+-rw-r--r--   0        0        0     7966 1970-01-01 00:00:00.000000 copula_wrapper-0.1.5/PKG-INFO
```

### Comparing `copula_wrapper-0.1.4/README.md` & `copula_wrapper-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/copula_wrapper/correlation_convert.py` & `copula_wrapper-0.1.5/copula_wrapper/correlation_convert.py`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/copula_wrapper/joint_distribution.py` & `copula_wrapper-0.1.5/copula_wrapper/joint_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 import statsmodels
 import statsmodels.distributions.copula.api
 from scipy.stats.distributions import rv_frozen
 from statsmodels.distributions.copula.copulas import CopulaDistribution
 
 from copula_wrapper.correlation_convert import to_pearsons_rho
 
-# TODO: add example with list/matrix input
+
 class CopulaJoint:
     """
-    Wrapper for ``CopulaDistribution`` from ``statsmodels``.
+    Wrapper for ``CopulaDistribution`` from ``statsmodels``. At the moment, only the Gaussian
+    copula is supported.
 
     The rank correlations that the joint distribution will satisfy must be specified as either
     Spearman's rho or Kendall's tau.
 
     Dimensions may be named by giving ``marginals`` and the rank correlations as dictionaries.
     In this case, the PDF and CDF are queried by passing a dictionary of values.
```

### Comparing `copula_wrapper-0.1.4/pyproject.toml` & `copula_wrapper-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "copula_wrapper"
-version = "0.1.4"
+version = "0.1.5"
 homepage = "https://github.com/tadamcz/copula-wrapper"
 description = "Top-level package for statsmodels copula wrapper."
 authors = ["Tom Adamczewski <tadamczewskipublic@gmail.com>"]
 readme = "README.md"
 classifiers=[
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
```

### Comparing `copula_wrapper-0.1.4/tests/__init__.py` & `copula_wrapper-0.1.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/tests/conftest.py` & `copula_wrapper-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/tests/e2e/__init__.py` & `copula_wrapper-0.1.5/tests/e2e/__init__.py`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/tests/e2e/__pycache__/__init__.cpython-310.pyc` & `copula_wrapper-0.1.5/tests/e2e/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/tests/e2e/__pycache__/test_8_dimensional.cpython-310-pytest-7.4.0.pyc` & `copula_wrapper-0.1.5/tests/e2e/__pycache__/test_8_dimensional.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/tests/e2e/__pycache__/test_correlation.cpython-310-pytest-7.4.0.pyc` & `copula_wrapper-0.1.5/tests/e2e/__pycache__/test_correlation.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/tests/e2e/__pycache__/test_marginals.cpython-310-pytest-7.4.0.pyc` & `copula_wrapper-0.1.5/tests/e2e/__pycache__/test_marginals.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/tests/e2e/test_8_dimensional.py` & `copula_wrapper-0.1.5/tests/e2e/test_8_dimensional.py`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/tests/e2e/test_marginals.py` & `copula_wrapper-0.1.5/tests/e2e/test_marginals.py`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/tests/seeds.py` & `copula_wrapper-0.1.5/tests/seeds.py`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/tests/shared.py` & `copula_wrapper-0.1.5/tests/shared.py`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/tests/test_copula_param.py` & `copula_wrapper-0.1.5/tests/test_copula_param.py`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/tests/test_validate_rank_corr.py` & `copula_wrapper-0.1.5/tests/test_validate_rank_corr.py`

 * *Files identical despite different names*

### Comparing `copula_wrapper-0.1.4/PKG-INFO` & `copula_wrapper-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copula-wrapper
-Version: 0.1.4
+Version: 0.1.5
 Summary: Top-level package for statsmodels copula wrapper.
 Home-page: https://github.com/tadamcz/copula-wrapper
 Author: Tom Adamczewski
 Author-email: tadamczewskipublic@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

