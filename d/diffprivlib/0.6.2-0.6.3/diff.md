# Comparing `tmp/diffprivlib-0.6.2.tar.gz` & `tmp/diffprivlib-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffprivlib-0.6.2.tar", last modified: Fri Dec  9 15:13:39 2022, max compression
+gzip compressed data, was "diffprivlib-0.6.3.tar", last modified: Fri Jun 30 15:35:56 2023, max compression
```

## Comparing `diffprivlib-0.6.2.tar` & `diffprivlib-0.6.3.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:39.224836 diffprivlib-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2022-12-09 15:13:39.224836 diffprivlib-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:39.192835 diffprivlib-0.6.2/diffprivlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/accountant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:39.200836 diffprivlib-0.6.2/diffprivlib/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/bingham.py
--rw-r--r--   0 runner    (1001) docker     (123)    21267 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/exponential.py
--rw-r--r--   0 runner    (1001) docker     (123)    12872 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)    17897 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/laplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/snapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/staircase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:39.200836 diffprivlib-0.6.2/diffprivlib/mechanisms/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/transforms/inttostring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/transforms/roundedinteger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/transforms/stringtoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/mechanisms/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:39.204836 diffprivlib-0.6.2/diffprivlib/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25986 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/models/forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/models/k_means.py
--rw-r--r--   0 runner    (1001) docker     (123)    13742 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/models/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    19229 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/models/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    13018 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/models/naive_bayes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14252 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/models/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    12973 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/models/standard_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:39.204836 diffprivlib-0.6.2/diffprivlib/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16598 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/tools/histograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/tools/quantiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    32660 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/diffprivlib/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:39.196835 diffprivlib-0.6.2/diffprivlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2022-12-09 15:13:39.000000 diffprivlib-0.6.2/diffprivlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2022-12-09 15:13:39.000000 diffprivlib-0.6.2/diffprivlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 15:13:39.000000 diffprivlib-0.6.2/diffprivlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-09 15:13:39.000000 diffprivlib-0.6.2/diffprivlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-09 15:13:39.000000 diffprivlib-0.6.2/diffprivlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-09 15:13:39.224836 diffprivlib-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:39.204836 diffprivlib-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:39.212836 diffprivlib-0.6.2/tests/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_BernoulliNegExp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_Binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_Bingham.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_DPMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_DPMechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_Exponential.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_ExponentialCategorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_ExponentialHierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_Gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_GaussianAnalytic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_GaussianDiscrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_Geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_GeometricFolded.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_GeometricTruncated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_Laplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_LaplaceBoundedDomain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_LaplaceBoundedNoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_LaplaceFolded.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_LaplaceTruncated.py
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_PermuteAndFlip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_Snapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_Staircase.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_TruncationAndFoldingMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_Uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/test_Vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:39.216836 diffprivlib-0.6.2/tests/mechanisms/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/transforms/test_DPTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/transforms/test_IntToString.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/transforms/test_RoundedInteger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/mechanisms/transforms/test_StringToInt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:39.220836 diffprivlib-0.6.2/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/test_DecisionTreeClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/test_FittingTree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/test_GaussianNB.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/test_KMeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/test_LinearRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7999 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/test_LogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/test_PCA.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/test_RandomForestClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/test_StandardScaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/test_covariance_eig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/test_incremental_mean_and_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/models/test_logistic_regression_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/test_Budget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13811 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/test_BudgetAccountant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/test_check_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/test_check_epsilon_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/test_check_random_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/test_clip_to_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/test_clip_to_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:39.224836 diffprivlib-0.6.2/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_count_nonzero.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_histogram2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_histogramdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_nanmean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_nanstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_nansum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_nanvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_percentile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_quantile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2022-12-09 15:13:29.000000 diffprivlib-0.6.2/tests/tools/test_var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:56.467315 diffprivlib-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-06-30 15:35:56.467315 diffprivlib-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:56.447315 diffprivlib-0.6.3/diffprivlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/accountant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:56.447315 diffprivlib-0.6.3/diffprivlib/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/bingham.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21267 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/snapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/staircase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:56.451315 diffprivlib-0.6.3/diffprivlib/mechanisms/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/transforms/inttostring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/transforms/roundedinteger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/transforms/stringtoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/mechanisms/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:56.451315 diffprivlib-0.6.3/diffprivlib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26109 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/models/forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/models/k_means.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/models/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19229 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/models/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/models/naive_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/models/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/models/standard_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:56.451315 diffprivlib-0.6.3/diffprivlib/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16598 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/tools/histograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/tools/quantiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32660 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/diffprivlib/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:56.447315 diffprivlib-0.6.3/diffprivlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-06-30 15:35:56.000000 diffprivlib-0.6.3/diffprivlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-30 15:35:56.000000 diffprivlib-0.6.3/diffprivlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:35:56.000000 diffprivlib-0.6.3/diffprivlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 15:35:56.000000 diffprivlib-0.6.3/diffprivlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 15:35:56.000000 diffprivlib-0.6.3/diffprivlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-30 15:35:56.467315 diffprivlib-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:56.455315 diffprivlib-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:56.459315 diffprivlib-0.6.3/tests/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_BernoulliNegExp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_Binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_Bingham.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_DPMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_DPMechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_Exponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_ExponentialCategorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_ExponentialHierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_Gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_GaussianAnalytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_GaussianDiscrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_Geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_GeometricFolded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_GeometricTruncated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_Laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_LaplaceBoundedDomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_LaplaceBoundedNoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_LaplaceFolded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_LaplaceTruncated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_PermuteAndFlip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_Snapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_Staircase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_TruncationAndFoldingMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_Uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/test_Vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:56.459315 diffprivlib-0.6.3/tests/mechanisms/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/transforms/test_DPTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/transforms/test_IntToString.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/transforms/test_RoundedInteger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/mechanisms/transforms/test_StringToInt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:56.463315 diffprivlib-0.6.3/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/test_DecisionTreeClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/test_FittingTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/test_GaussianNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/test_KMeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/test_LinearRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/test_LogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/test_PCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/test_RandomForestClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/test_StandardScaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/test_covariance_eig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/test_incremental_mean_and_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/models/test_logistic_regression_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/test_Budget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13811 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/test_BudgetAccountant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/test_check_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/test_check_epsilon_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/test_check_random_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/test_clip_to_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/test_clip_to_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:56.467315 diffprivlib-0.6.3/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_count_nonzero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_histogram2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_histogramdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_nanmean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_nanstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_nansum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_nanvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_percentile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-30 15:35:36.000000 diffprivlib-0.6.3/tests/tools/test_var.py
```

### Comparing `diffprivlib-0.6.2/LICENSE.md` & `diffprivlib-0.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/PKG-INFO` & `diffprivlib-0.6.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffprivlib
-Version: 0.6.2
+Version: 0.6.3
 Summary: IBM Differential Privacy Library
 Home-page: https://github.com/IBM/differential-privacy-library
 Author: Naoise Holohan
 Author-email: naoise.holohan@ibm.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -160,7 +160,14 @@
   journal = {ArXiv e-prints},
   archivePrefix = "arXiv",
   volume = {1907.02444 [cs.CR]},
   primaryClass = "cs.CR",
   month = jul
 }
 ```
+
+## References
+
+* Holohan, N., Antonatos, S., Braghin, S. and Mac Aonghusa, P., 2018. The Bounded Laplace Mechanism in Differential privacy. arXiv preprint arXiv:1808.10410.
+* Holohan, N., Braghin, S., Mac Aonghusa, P. and Levacher, K., 2019. Diffprivlib: the IBM Differential Privacy Library. arXiv preprint arXiv:1907.02444.
+* Ludwig, H., Baracaldo, N., Thomas, G., Zhou, Y., Anwar, A., Rajamoni, S., Ong, Y., Radhakrishnan, J., Verma, A., Sinn, M. and Purcell, M., 2020. IBM Federated Learning: an Enterprise Framework White Paper v0. 1. arXiv preprint arXiv:2007.10987.
+* Holohan, N. and Braghin, S., 2021. Secure Random Sampling in Differential Privacy. In Computer Security–ESORICS 2021: 26th European Symposium on Research in Computer Security, Darmstadt, Germany, October 4–8, 2021, Proceedings, Part II 26 (pp. 523-542). Springer International Publishing.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `diffprivlib-0.6.2/README.md` & `diffprivlib-0.6.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -129,7 +129,14 @@
   journal = {ArXiv e-prints},
   archivePrefix = "arXiv",
   volume = {1907.02444 [cs.CR]},
   primaryClass = "cs.CR",
   month = jul
 }
 ```
+
+## References
+
+* Holohan, N., Antonatos, S., Braghin, S. and Mac Aonghusa, P., 2018. The Bounded Laplace Mechanism in Differential privacy. arXiv preprint arXiv:1808.10410.
+* Holohan, N., Braghin, S., Mac Aonghusa, P. and Levacher, K., 2019. Diffprivlib: the IBM Differential Privacy Library. arXiv preprint arXiv:1907.02444.
+* Ludwig, H., Baracaldo, N., Thomas, G., Zhou, Y., Anwar, A., Rajamoni, S., Ong, Y., Radhakrishnan, J., Verma, A., Sinn, M. and Purcell, M., 2020. IBM Federated Learning: an Enterprise Framework White Paper v0. 1. arXiv preprint arXiv:2007.10987.
+* Holohan, N. and Braghin, S., 2021. Secure Random Sampling in Differential Privacy. In Computer Security–ESORICS 2021: 26th European Symposium on Research in Computer Security, Darmstadt, Germany, October 4–8, 2021, Proceedings, Part II 26 (pp. 523-542). Springer International Publishing.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `diffprivlib-0.6.2/diffprivlib/__init__.py` & `diffprivlib-0.6.3/diffprivlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 
 """
 from diffprivlib import mechanisms
 from diffprivlib import models
 from diffprivlib import tools
 from diffprivlib.accountant import BudgetAccountant
 
-__version__ = '0.6.2'
+__version__ = '0.6.3'
```

### Comparing `diffprivlib-0.6.2/diffprivlib/accountant.py` & `diffprivlib-0.6.3/diffprivlib/accountant.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/__init__.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/__init__.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/base.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/base.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/binary.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/binary.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/bingham.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/bingham.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/exponential.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/exponential.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/gaussian.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/gaussian.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/geometric.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/geometric.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/laplace.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/laplace.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/snapping.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/snapping.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/staircase.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/staircase.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/transforms/__init__.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/transforms/base.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/transforms/base.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/transforms/inttostring.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/transforms/inttostring.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/transforms/roundedinteger.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/transforms/roundedinteger.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/transforms/stringtoint.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/transforms/stringtoint.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/uniform.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/uniform.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/mechanisms/vector.py` & `diffprivlib-0.6.3/diffprivlib/mechanisms/vector.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/models/__init__.py` & `diffprivlib-0.6.3/diffprivlib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/models/forest.py` & `diffprivlib-0.6.3/diffprivlib/models/forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -627,7 +627,11 @@
         yield self.left_child
         yield self.right_child
         yield self.feature
         yield self.threshold
         yield 0.0  # Impurity
         yield 0  # n_node_samples
         yield 0.0  # weighted_n_node_samples
+
+        # remove branch when scikit-learn v1.3 is min requirement
+        if len(NODE_DTYPE) > 7:
+            yield False
```

### Comparing `diffprivlib-0.6.2/diffprivlib/models/k_means.py` & `diffprivlib-0.6.3/diffprivlib/models/k_means.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/models/linear_regression.py` & `diffprivlib-0.6.3/diffprivlib/models/linear_regression.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/models/logistic_regression.py` & `diffprivlib-0.6.3/diffprivlib/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/models/naive_bayes.py` & `diffprivlib-0.6.3/diffprivlib/models/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/models/pca.py` & `diffprivlib-0.6.3/diffprivlib/models/pca.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/models/standard_scaler.py` & `diffprivlib-0.6.3/diffprivlib/models/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/models/utils.py` & `diffprivlib-0.6.3/diffprivlib/models/utils.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/tools/__init__.py` & `diffprivlib-0.6.3/diffprivlib/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/tools/histograms.py` & `diffprivlib-0.6.3/diffprivlib/tools/histograms.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/tools/quantiles.py` & `diffprivlib-0.6.3/diffprivlib/tools/quantiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     quant = np.ravel(quant)
 
     if np.any(quant < 0) or np.any(quant > 1):
         raise ValueError("Quantiles must be in the unit interval [0, 1].")
 
     if len(quant) > 1:
         return np.array([quantile(array, q_i, epsilon=epsilon / len(quant), bounds=bounds, axis=axis, keepdims=keepdims,
-                                  accountant=accountant) for q_i in quant])
+                                  accountant=accountant, random_state=random_state) for q_i in quant])
 
     # Dealing with a single quant from now on
     quant = quant.item()
 
     if axis is not None or keepdims:
         return _wrap_axis(quantile, array, quant=quant, epsilon=epsilon, bounds=bounds, axis=axis, keepdims=keepdims,
                           random_state=random_state, accountant=accountant)
@@ -127,15 +127,15 @@
 
     k = array.size
     array = np.append(array, list(bounds))
     array.sort()
 
     interval_sizes = np.diff(array)
 
-    # Todo: Need to find a way to do this in a differentially private way
+    # Todo: Need to find a way to do this in a differentially private way, see GH 80
     if np.isnan(interval_sizes).any():
         return np.nan
 
     mech = Exponential(epsilon=epsilon, sensitivity=1, utility=list(-np.abs(np.arange(0, k + 1) - quant * k)),
                        measure=list(interval_sizes), random_state=random_state)
     idx = mech.randomise()
     output = random_state.random() * (array[idx+1] - array[idx]) + array[idx]
```

### Comparing `diffprivlib-0.6.2/diffprivlib/tools/utils.py` & `diffprivlib-0.6.3/diffprivlib/tools/utils.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/utils.py` & `diffprivlib-0.6.3/diffprivlib/utils.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib/validation.py` & `diffprivlib-0.6.3/diffprivlib/validation.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/diffprivlib.egg-info/PKG-INFO` & `diffprivlib-0.6.3/diffprivlib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffprivlib
-Version: 0.6.2
+Version: 0.6.3
 Summary: IBM Differential Privacy Library
 Home-page: https://github.com/IBM/differential-privacy-library
 Author: Naoise Holohan
 Author-email: naoise.holohan@ibm.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -160,7 +160,14 @@
   journal = {ArXiv e-prints},
   archivePrefix = "arXiv",
   volume = {1907.02444 [cs.CR]},
   primaryClass = "cs.CR",
   month = jul
 }
 ```
+
+## References
+
+* Holohan, N., Antonatos, S., Braghin, S. and Mac Aonghusa, P., 2018. The Bounded Laplace Mechanism in Differential privacy. arXiv preprint arXiv:1808.10410.
+* Holohan, N., Braghin, S., Mac Aonghusa, P. and Levacher, K., 2019. Diffprivlib: the IBM Differential Privacy Library. arXiv preprint arXiv:1907.02444.
+* Ludwig, H., Baracaldo, N., Thomas, G., Zhou, Y., Anwar, A., Rajamoni, S., Ong, Y., Radhakrishnan, J., Verma, A., Sinn, M. and Purcell, M., 2020. IBM Federated Learning: an Enterprise Framework White Paper v0. 1. arXiv preprint arXiv:2007.10987.
+* Holohan, N. and Braghin, S., 2021. Secure Random Sampling in Differential Privacy. In Computer Security–ESORICS 2021: 26th European Symposium on Research in Computer Security, Darmstadt, Germany, October 4–8, 2021, Proceedings, Part II 26 (pp. 523-542). Springer International Publishing.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `diffprivlib-0.6.2/diffprivlib.egg-info/SOURCES.txt` & `diffprivlib-0.6.3/diffprivlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/setup.py` & `diffprivlib-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_BernoulliNegExp.py` & `diffprivlib-0.6.3/tests/mechanisms/test_BernoulliNegExp.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_Binary.py` & `diffprivlib-0.6.3/tests/mechanisms/test_Binary.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_Bingham.py` & `diffprivlib-0.6.3/tests/mechanisms/test_Bingham.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_DPMachine.py` & `diffprivlib-0.6.3/tests/mechanisms/test_DPMachine.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_DPMechanism.py` & `diffprivlib-0.6.3/tests/mechanisms/test_DPMechanism.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_Exponential.py` & `diffprivlib-0.6.3/tests/mechanisms/test_Exponential.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_ExponentialCategorical.py` & `diffprivlib-0.6.3/tests/mechanisms/test_ExponentialCategorical.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_ExponentialHierarchical.py` & `diffprivlib-0.6.3/tests/mechanisms/test_ExponentialHierarchical.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_Gaussian.py` & `diffprivlib-0.6.3/tests/mechanisms/test_Gaussian.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_GaussianAnalytic.py` & `diffprivlib-0.6.3/tests/mechanisms/test_GaussianAnalytic.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_GaussianDiscrete.py` & `diffprivlib-0.6.3/tests/mechanisms/test_GaussianDiscrete.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_Geometric.py` & `diffprivlib-0.6.3/tests/mechanisms/test_Geometric.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_GeometricFolded.py` & `diffprivlib-0.6.3/tests/mechanisms/test_GeometricFolded.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_GeometricTruncated.py` & `diffprivlib-0.6.3/tests/mechanisms/test_GeometricTruncated.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_Laplace.py` & `diffprivlib-0.6.3/tests/mechanisms/test_Laplace.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_LaplaceBoundedDomain.py` & `diffprivlib-0.6.3/tests/mechanisms/test_LaplaceBoundedDomain.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_LaplaceBoundedNoise.py` & `diffprivlib-0.6.3/tests/mechanisms/test_LaplaceBoundedNoise.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_LaplaceFolded.py` & `diffprivlib-0.6.3/tests/mechanisms/test_LaplaceFolded.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_LaplaceTruncated.py` & `diffprivlib-0.6.3/tests/mechanisms/test_LaplaceTruncated.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_PermuteAndFlip.py` & `diffprivlib-0.6.3/tests/mechanisms/test_PermuteAndFlip.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_Snapping.py` & `diffprivlib-0.6.3/tests/mechanisms/test_Snapping.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_Staircase.py` & `diffprivlib-0.6.3/tests/mechanisms/test_Staircase.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_TruncationAndFoldingMixin.py` & `diffprivlib-0.6.3/tests/mechanisms/test_TruncationAndFoldingMixin.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_Uniform.py` & `diffprivlib-0.6.3/tests/mechanisms/test_Uniform.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/test_Vector.py` & `diffprivlib-0.6.3/tests/mechanisms/test_Vector.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/transforms/test_DPTransformer.py` & `diffprivlib-0.6.3/tests/mechanisms/transforms/test_DPTransformer.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/transforms/test_IntToString.py` & `diffprivlib-0.6.3/tests/mechanisms/transforms/test_IntToString.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/transforms/test_RoundedInteger.py` & `diffprivlib-0.6.3/tests/mechanisms/transforms/test_RoundedInteger.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/mechanisms/transforms/test_StringToInt.py` & `diffprivlib-0.6.3/tests/mechanisms/transforms/test_StringToInt.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/models/test_DecisionTreeClassifier.py` & `diffprivlib-0.6.3/tests/models/test_DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/models/test_FittingTree.py` & `diffprivlib-0.6.3/tests/models/test_FittingTree.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/models/test_GaussianNB.py` & `diffprivlib-0.6.3/tests/models/test_GaussianNB.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/models/test_KMeans.py` & `diffprivlib-0.6.3/tests/models/test_KMeans.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/models/test_LinearRegression.py` & `diffprivlib-0.6.3/tests/models/test_LinearRegression.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/models/test_LogisticRegression.py` & `diffprivlib-0.6.3/tests/models/test_LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/models/test_PCA.py` & `diffprivlib-0.6.3/tests/models/test_PCA.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/models/test_RandomForestClassifier.py` & `diffprivlib-0.6.3/tests/models/test_RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/models/test_StandardScaler.py` & `diffprivlib-0.6.3/tests/models/test_StandardScaler.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/models/test_covariance_eig.py` & `diffprivlib-0.6.3/tests/models/test_covariance_eig.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/models/test_incremental_mean_and_var.py` & `diffprivlib-0.6.3/tests/models/test_incremental_mean_and_var.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/models/test_logistic_regression_path.py` & `diffprivlib-0.6.3/tests/models/test_logistic_regression_path.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/test_Budget.py` & `diffprivlib-0.6.3/tests/test_Budget.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/test_BudgetAccountant.py` & `diffprivlib-0.6.3/tests/test_BudgetAccountant.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/test_check_bounds.py` & `diffprivlib-0.6.3/tests/test_check_bounds.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/test_check_epsilon_delta.py` & `diffprivlib-0.6.3/tests/test_check_epsilon_delta.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/test_check_random_state.py` & `diffprivlib-0.6.3/tests/test_check_random_state.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/test_clip_to_bounds.py` & `diffprivlib-0.6.3/tests/test_clip_to_bounds.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/test_clip_to_norm.py` & `diffprivlib-0.6.3/tests/test_clip_to_norm.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_count_nonzero.py` & `diffprivlib-0.6.3/tests/tools/test_count_nonzero.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_histogram.py` & `diffprivlib-0.6.3/tests/tools/test_histogram.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_histogram2d.py` & `diffprivlib-0.6.3/tests/tools/test_histogram2d.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_histogramdd.py` & `diffprivlib-0.6.3/tests/tools/test_histogramdd.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_mean.py` & `diffprivlib-0.6.3/tests/tools/test_mean.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_median.py` & `diffprivlib-0.6.3/tests/tools/test_median.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_nanmean.py` & `diffprivlib-0.6.3/tests/tools/test_nanmean.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_nanstd.py` & `diffprivlib-0.6.3/tests/tools/test_nanstd.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_nansum.py` & `diffprivlib-0.6.3/tests/tools/test_nansum.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_nanvar.py` & `diffprivlib-0.6.3/tests/tools/test_nanvar.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_quantile.py` & `diffprivlib-0.6.3/tests/tools/test_quantile.py`

 * *Files 9% similar despite different names*

```diff
@@ -119,14 +119,24 @@
     def test_nan(self):
         a = np.random.random((5, 5))
         a[2, 2] = np.nan
 
         res = quantile(a, 0.5, bounds=(0, 1))
         self.assertTrue(np.isnan(res))
 
+    def test_random_state(self):
+        rng = check_random_state(0)
+        quantiles_1 = quantile([0, 1, 2, 3, 4], quant=[0.33, 0.66], bounds=(0, 4), random_state=rng)
+        quantiles_2 = quantile([0, 1, 2, 3, 4], quant=[0.33, 0.66], bounds=(0, 4), random_state=rng)
+        assert not np.all(quantiles_1 == quantiles_2)
+
+        quantiles_1 = quantile([0, 1, 2, 3, 4], quant=[0.33, 0.66], bounds=(0, 4), random_state=0)
+        quantiles_2 = quantile([0, 1, 2, 3, 4], quant=[0.33, 0.66], bounds=(0, 4), random_state=0)
+        assert np.all(quantiles_1 == quantiles_2)
+
     def test_accountant(self):
         from diffprivlib.accountant import BudgetAccountant
         acc = BudgetAccountant(1.5, 0)
 
         a = np.random.random((1000, 5))
         quantile(a, 0.5, epsilon=1, bounds=(0, 1), accountant=acc)
         self.assertEqual((1.0, 0), acc.total())
```

### Comparing `diffprivlib-0.6.2/tests/tools/test_std.py` & `diffprivlib-0.6.3/tests/tools/test_std.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_sum.py` & `diffprivlib-0.6.3/tests/tools/test_sum.py`

 * *Files identical despite different names*

### Comparing `diffprivlib-0.6.2/tests/tools/test_var.py` & `diffprivlib-0.6.3/tests/tools/test_var.py`

 * *Files identical despite different names*

