# Comparing `tmp/cca_zoo-2.0.7.tar.gz` & `tmp/cca_zoo-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cca_zoo-2.0.7.tar", last modified: Mon Jun 26 12:13:07 2023, max compression
+gzip compressed data, was "cca_zoo-2.0.8.tar", max compression
```

## Comparing `cca_zoo-2.0.7.tar` & `cca_zoo-2.0.8.tar`

### file list

```diff
@@ -1,114 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo/classical/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_gcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_grcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_altmaxvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_deflation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13837 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_elasticnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_ey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_gradkcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_incrementalpls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_pls_als.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_pmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_scca_admm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_scca_hsic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_scca_parkhomenko.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_scca_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_stochasticpls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_iterative/_swcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_kcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_mcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_ncca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_partialcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_pcacca.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_pls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_prcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/classical/_tcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/data/deep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/data/simulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo/deep/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo/deep/_discriminative/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_discriminative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca_ey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca_noi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca_sdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dgcca.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dtcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo/deep/_generative/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_generative/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_generative/_dccae.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_generative/_dvcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/_generative/_splitae.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/deep/objectives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/model_selection/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/model_selection/_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo/probabilistic/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/probabilistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/probabilistic/_probabilisticcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/test/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/test/test_deepmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/test/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/test/test_probabilistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/test/test_regularised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/test/test_stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/test/test_unregularized.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/utils/check_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/cca_zoo/visualisation/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/cca_zoo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/examples/plot_dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/examples/plot_dcca_custom_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/examples/plot_dcca_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/examples/plot_dvcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/examples/plot_hyperparameter_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/examples/plot_kernel_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/examples/plot_many_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/examples/plot_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/examples/plot_sparse_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-26 12:12:54.000000 cca_zoo-2.0.7/examples/plot_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:13:06.000000 cca_zoo-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-26 12:13:05.000000 cca_zoo-2.0.7/setup.py
+-rw-r--r--   0        0        0     1069 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/LICENSE
+-rw-r--r--   0        0        0     3999 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/README.md
+-rw-r--r--   0        0        0      323 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/__init__.py
+-rw-r--r--   0        0        0      127 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/data/__init__.py
+-rw-r--r--   0        0        0     3176 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/data/deep.py
+-rw-r--r--   0        0        0     7074 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/data/simulated.py
+-rw-r--r--   0        0        0      598 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/__init__.py
+-rw-r--r--   0        0        0     5356 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_base.py
+-rw-r--r--   0        0        0      276 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/__init__.py
+-rw-r--r--   0        0        0     1831 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca.py
+-rw-r--r--   0        0        0     2342 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
+-rw-r--r--   0        0        0     2401 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_ey.py
+-rw-r--r--   0        0        0     1275 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_gh.py
+-rw-r--r--   0        0        0     2240 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_noi.py
+-rw-r--r--   0        0        0     2539 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_sdl.py
+-rw-r--r--   0        0        0     1681 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_svd.py
+-rw-r--r--   0        0        0      676 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dgcca.py
+-rw-r--r--   0        0        0      784 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dtcca.py
+-rw-r--r--   0        0        0       82 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_generative/__init__.py
+-rw-r--r--   0        0        0     1449 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_generative/_base.py
+-rw-r--r--   0        0        0     2481 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_generative/_dccae.py
+-rw-r--r--   0        0        0     5339 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_generative/_dvcca.py
+-rw-r--r--   0        0        0     2051 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_generative/_splitae.py
+-rw-r--r--   0        0        0     9528 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/architectures.py
+-rw-r--r--   0        0        0      337 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/callbacks.py
+-rw-r--r--   0        0        0     1931 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/metrics.py
+-rw-r--r--   0        0        0     8808 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/objectives.py
+-rw-r--r--   0        0        0     1385 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/__init__.py
+-rw-r--r--   0        0        0     7492 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_base.py
+-rw-r--r--   0        0        0     1584 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_dummy.py
+-rw-r--r--   0        0        0     3332 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gcca.py
+-rw-r--r--   0        0        0      133 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gradient/__init__.py
+-rw-r--r--   0        0        0     8646 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gradient/_ey.py
+-rw-r--r--   0        0        0     2223 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gradient/_gh.py
+-rw-r--r--   0        0        0     1757 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gradient/_gradient.py
+-rw-r--r--   0        0        0     1713 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gradient/_stochasticpls.py
+-rw-r--r--   0        0        0     1738 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gradient/_svd.py
+-rw-r--r--   0        0        0     6599 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_grcca.py
+-rw-r--r--   0        0        0      451 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/__init__.py
+-rw-r--r--   0        0        0     7048 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_altmaxvar.py
+-rw-r--r--   0        0        0    10968 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_base.py
+-rw-r--r--   0        0        0     2459 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_deflation.py
+-rw-r--r--   0        0        0    13982 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_elasticnet.py
+-rw-r--r--   0        0        0     3789 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_incrementalpls.py
+-rw-r--r--   0        0        0     3246 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_pls_als.py
+-rw-r--r--   0        0        0     6728 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_admm.py
+-rw-r--r--   0        0        0     4089 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_parkhomenko.py
+-rw-r--r--   0        0        0     7166 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_pmd.py
+-rw-r--r--   0        0        0     4460 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_span.py
+-rw-r--r--   0        0        0     3813 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_swcca.py
+-rw-r--r--   0        0        0    10289 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_mcca.py
+-rw-r--r--   0        0        0     3087 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_partialcca.py
+-rw-r--r--   0        0        0     1621 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_pcacca.py
+-rw-r--r--   0        0        0    11203 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_pls.py
+-rw-r--r--   0        0        0     4214 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_prcca.py
+-rw-r--r--   0        0        0     2341 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_search.py
+-rw-r--r--   0        0        0     4710 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_tcca.py
+-rw-r--r--   0        0        0      330 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/model_selection/__init__.py
+-rw-r--r--   0        0        0    11669 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/model_selection/_search.py
+-rw-r--r--   0        0        0    18413 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/model_selection/_validation.py
+-rw-r--r--   0        0        0       62 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/nonparametric/__init__.py
+-rw-r--r--   0        0        0     5066 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/nonparametric/_gradkcca.py
+-rw-r--r--   0        0        0    12589 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/nonparametric/_kcca.py
+-rw-r--r--   0        0        0     6385 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/nonparametric/_ncca.py
+-rw-r--r--   0        0        0     6280 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/nonparametric/_scca_hsic.py
+-rw-r--r--   0        0        0       80 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/probabilistic/__init__.py
+-rw-r--r--   0        0        0     4502 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/probabilistic/_probabilisticcca.py
+-rw-r--r--   0        0        0      129 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/utils/__init__.py
+-rw-r--r--   0        0        0     1581 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/utils/check_values.py
+-rw-r--r--   0        0        0      163 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/visualisation/__init__.py
+-rw-r--r--   0        0        0     2292 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/visualisation/plotting.py
+-rw-r--r--   0        0        0     1158 2023-06-30 02:09:48.110476 cca_zoo-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5233 1970-01-01 00:00:00.000000 cca_zoo-2.0.8/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cca_zoo-2.0.7/README.md` & `cca_zoo-2.0.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -10,36 +10,42 @@
 
 `cca-zoo` is a collection of linear, kernel, and deep methods for canonical correlation analysis of multiview data.
 Where possible it follows the `scikit-learn`/`mvlearn` APIs and models therefore have `fit`/`transform`/`fit_transform`
 methods as standard.
 
 ## Installation
 
-Dependency of some implemented algorithms are heavy, such as `pytorch` and `numpyro`.
-We provide several options to accomodate the user's needs.
-For full details of algorithms included, please refer to section [Implemented Methods](#implemented-methods)
+You can install cca-zoo with pip or poetry. cca-zoo has an optional probabilistic feature that you can enable with the [probabilistic] suffix.
 
-Standard installation:
+To install cca-zoo with pip, run one of the following commands in your terminal:
 
-```
+```bash
 pip install cca-zoo
 ```
 
-For deep learning elements use:
+To install cca-zoo with poetry, run one of the following commands in your terminal:
 
-```
-pip install cca-zoo[deep]
+```bash
+pip install cca-zoo[probabilistic]
 ```
 
-For probabilistic elements use:
+Can also use poetry to install:
 
+```bash
+poetry add cca-zoo
 ```
-pip install cca-zoo[probabilistic]
+
+or
+
+```bash
+poetry add cca-zoo[probabilistic]
 ```
 
+
+
 ## Documentation
 
 Available at https://cca-zoo.readthedocs.io/en/latest/
 
 ## Citation:
 
 CCA-Zoo is intended as research software. Citations and use of our software help us justify the effort which has gone
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/__init__.py` & `cca_zoo-2.0.8/cca_zoo/linear/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 from ._mcca import MCCA, CCA, rCCA
 from ._pls import PLS, MPLS
 from ._gcca import GCCA
 from ._grcca import GRCCA
-from ._ncca import NCCA
 from ._partialcca import PartialCCA
 from ._prcca import PRCCA
 from ._tcca import TCCA
 from ._pcacca import PCACCA
-from ._kcca import KCCA, KGCCA, KTCCA
 
 
 __all__ = [
     "CCA",
     "GCCA",
     "GRCCA",
-    "KCCA",
     "MCCA",
-    "NCCA",
     "PLS",
     "PRCCA",
-    "KTCCA",
     "TCCA",
     "PartialCCA",
     "rCCA",
     "PCACCA",
-    "KGCCA",
     "MPLS",
 ]
 
 # if pytorch-lightning is installed then import ._iterative
 
 try:
     from ._iterative import (
-        CCAEY,
-        CCAGH,
-        CCASVD,
-        PLS_ALS,  # SCCA_ADMM,; SWCCA,
-        PLSEY,
-        PLSSVD,
+        PLS_ALS,
         SCCA_IPLS,
         SCCA_PMD,
         AltMaxVar,
         ElasticCCA,
-        PLSStochasticPower,
         SCCA_Parkhomenko,
         SCCA_Span,
     )
 
     __all__ += [
         "ElasticCCA",
         "SCCA_IPLS",
         "PLS_ALS",
         "SCCA_PMD",
         "SCCA_Parkhomenko",
         "SCCA_Span",
         "AltMaxVar",
+    ]
+except:
+    # let user know that if they want to use iterative methods they need to install pytorch-lightning from version 2.0.0
+    print("To use iterative methods please install pytorch-lightning")
+try:
+    from ._gradient import (
+        CCAEY,
+        CCAGH,
+        CCASVD,
+        PLSEY,
+        PLSSVD,
+        PLSStochasticPower,
+    )
+
+    __all__ += [
         "CCAEY",
         "PLSEY",
         "CCAGH",
         "CCASVD",
         "PLSSVD",
+        "PLSStochasticPower",
     ]
+
 except:
-    # let user know that if they want to use iterative methods they need to install pytorch-lightning from version 2.0.0
-    print(
-        "To use iterative methods please install pytorch-lightning from version 2.0.0"
-    )
+    print("To use gradient methods please install pytorch-lightning")
+
 
 classes = __all__
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_base.py` & `cca_zoo-2.0.8/cca_zoo/linear/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import numpy as np
 from sklearn.base import BaseEstimator, MultiOutputMixin, RegressorMixin
 from sklearn.utils.validation import FLOAT_DTYPES, check_is_fitted, check_random_state
 
 
 class BaseModel(BaseEstimator, MultiOutputMixin, RegressorMixin):
     """
-    A base class for multivariate latent variable classical.
+    A base class for multivariate latent variable linear.
 
     This class implements common methods and attributes for fitting and transforming
-    multiple views of data using latent variable classical. It inherits from scikit-learn's
+    multiple views of data using latent variable linear. It inherits from scikit-learn's
     BaseEstimator, MultiOutputMixin and RegressorMixin classes.
 
     Parameters
     ----------
     latent_dimensions : int, optional
         Number of latent dimensions to fit. Default is 1.
     copy_data : bool, optional
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_dummy.py` & `cca_zoo-2.0.8/cca_zoo/linear/_dummy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable
 
 import numpy as np
 
-from cca_zoo.classical._base import BaseModel
+from cca_zoo.linear._base import BaseModel
 
 
 class DummyCCA(BaseModel):
     def __init__(
         self,
         latent_dimensions: int = 1,
         copy_data=True,
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_gcca.py` & `cca_zoo-2.0.8/cca_zoo/linear/_gcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Union
 
 import numpy as np
 
-from cca_zoo.classical._mcca import MCCA
+from cca_zoo.linear._mcca import MCCA
 from cca_zoo.utils.check_values import _process_parameter
 
 
 class GCCA(MCCA):
     r"""
     A class used to fit GCCA model. This model extends CCA to more than two views by optimizing the sum of correlations with a shared auxiliary vector.
 
@@ -25,15 +25,15 @@
 
     References
     ----------
     Tenenhaus, Arthur, and Michel Tenenhaus. "Regularized generalized canonical correlation analysis." Psychometrika 76.2 (2011): 257.
 
     Examples
     --------
-    >>> from cca_zoo.classical import GCCA
+    >>> from cca_zoo.linear import GCCA
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> X3 = rng.random((10,5))
     >>> model = GCCA()
     >>> model.fit((X1,X2,X3)).score((X1,X2,X3))
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_grcca.py` & `cca_zoo-2.0.8/cca_zoo/linear/_grcca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import warnings
 from typing import Iterable
 
 import numpy as np
 
-from cca_zoo.classical._mcca import MCCA
+from cca_zoo.linear._mcca import MCCA
 from cca_zoo.utils import _process_parameter
 
 
 class GRCCA(MCCA):
     """
     Grouped Regularized Canonical Correlation Analysis
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_altmaxvar.py` & `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_altmaxvar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Iterable, Union
 
 import numpy as np
 import torch
-from skprox.proximal_operators import _proximal_operators
 
-from cca_zoo.classical._iterative._base import BaseIterative, BaseLoop
+from cca_zoo.linear._iterative._base import BaseIterative, BaseLoop
 from cca_zoo.utils import _process_parameter
 
 
 class AltMaxVar(BaseIterative):
     def __init__(
         self,
         latent_dimensions=1,
@@ -19,36 +18,39 @@
         proximal="L1",
         positive=False,
         tau: Union[Iterable[float], float] = None,
         proximal_params: Iterable[dict] = None,
         gamma=0.1,
         learning_rate=0.1,
         T=100,
+        trainer_kwargs=None,
         convergence_checking=None,
         track=None,
         verbose=False,
     ):
         super().__init__(
             latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             random_state=random_state,
             tol=tol,
             epochs=epochs,
             convergence_checking=convergence_checking,
             track=track,
             verbose=verbose,
-            trainer_kwargs={"accelerator": "cpu"},
+            trainer_kwargs=trainer_kwargs,
         )
         self.tau = tau
         self.proximal = proximal
         self.proximal_params = proximal_params
         self.gamma = gamma
         self.learning_rate = learning_rate
         self.T = T
         self.positive = positive
+        # set trainer kwargs accelerator to 'cpu'
+        self.trainer_kwargs["accelerator"] = "cpu"
 
     def _get_module(self, weights=None, k=None):
         return AltMaxVarLoop(
             weights=weights,
             k=k,
             gamma=self.gamma,
             T=self.T,
@@ -161,7 +163,67 @@
                 t += 1
 
         # if track or convergence_checking is enabled, compute the objective function
         if self.tracking or self.convergence_checking:
             objective = self.objective(batch["views"])
 
             return {"loss": torch.tensor(objective)}
+
+
+from pyproximal import (
+    L0,
+    L0Ball,
+    L1,
+    L1Ball,
+    L2,
+    L21,
+    L21_plus_L1,
+    Nuclear,
+    NuclearBall,
+    Log,
+    Log1,
+    Euclidean,
+    EuclideanBall,
+)
+
+PROXIMAL_OPERATORS = {
+    "L0": L0,
+    "L0Ball": L0Ball,
+    "L1": L1,
+    "L1Ball": L1Ball,
+    "L2": L2,
+    "L21": L21,
+    "L21_plus_L1": L21_plus_L1,
+    "Nuclear": Nuclear,
+    "NuclearBall": NuclearBall,
+    "Log": Log,
+    "Log1": Log1,
+    "Euclidean": Euclidean,
+    "EuclideanBall": EuclideanBall,
+}
+
+PROXIMAL_PARAMS = {
+    "Dummy": (),
+    "L0": frozenset(["sigma"]),
+    "L0Ball": frozenset(["radius"]),
+    "L1": frozenset(["sigma"]),
+    "L1Ball": frozenset(["n", "radius"]),
+    "L2": frozenset(["sigma"]),
+    "L21": frozenset(["ndim", "sigma"]),
+    "L21_plus_L1": frozenset(["sigma", "rho"]),
+    "TV": frozenset(["sigma", "isotropic", "dims"]),
+    "Nuclear": frozenset(["dim", "sigma"]),
+    "NuclearBall": frozenset(["dims", "radius"]),
+    "Log": frozenset(["sigma", "gamma"]),
+    "Log1": frozenset(["sigma", "delta"]),
+    "Euclidean": frozenset(["sigma"]),
+    "TVL1": frozenset(["sigma", "shape", "l1_ratio"]),
+}
+
+
+def _proximal_operators(proximal, filter_params=True, **params):
+    if proximal in PROXIMAL_OPERATORS:
+        if filter_params:
+            params = {k: params[k] for k in params if k in PROXIMAL_PARAMS[proximal]}
+        return PROXIMAL_OPERATORS[proximal](**params)
+    elif callable(proximal):
+        return proximal(**params)
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_base.py` & `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 import numpy as np
 import pytorch_lightning as pl
 from pytorch_lightning.callbacks import Callback, EarlyStopping
 from torch.utils import data
 from torch.utils.data import DataLoader
 
 from cca_zoo.data.deep import NumpyDataset
-from cca_zoo.classical import MCCA, rCCA
-from cca_zoo.classical._base import BaseModel
-from cca_zoo.classical._dummy import DummyCCA
+from cca_zoo.linear import MCCA, rCCA
+from cca_zoo.linear._base import BaseModel
+from cca_zoo.linear._dummy import DummyCCA
 import torch
 
 # Default Trainer kwargs
 DEFAULT_TRAINER_KWARGS = dict(
     enable_checkpointing=False,
     logger=False,
     enable_model_summary=False,
-    enable_progress_bar=False,
+    enable_progress_bar=True,
 )
 
 DEFAULT_LOADER_KWARGS = dict(
     num_workers=0, pin_memory=True, drop_last=False, shuffle=False
 )
 
 
@@ -42,15 +42,15 @@
         learning_rate=1,
         initialization: Union[str, callable] = "random",
         callbacks: Optional[Union[List[Callback], Callback]] = None,
         trainer_kwargs=None,
         convergence_checking=None,
         patience=10,
         track=None,
-        verbose=False,
+        verbose=None,
     ):
         super().__init__(
             latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             random_state=random_state,
             accept_sparse=accept_sparse,
         )
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_deflation.py` & `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_deflation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from abc import ABC
 from typing import Iterable
+
+import numpy as np
 import pytorch_lightning as pl
 from tqdm import tqdm
-import numpy as np
-from cca_zoo.classical._iterative._base import BaseIterative
 
 
-class BaseDeflation(BaseIterative, ABC):
+class DeflationMixin:
     def _fit(self, views: Iterable[np.ndarray]):
         # if views is a tuple then convert to a list
         if isinstance(views, tuple):
             views = list(views)
         # tqdm for each latent dimension
         for k in tqdm(
             range(self.latent_dimensions), desc="Latent Dimension", leave=False
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_elasticnet.py` & `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_elasticnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import warnings
 from typing import Iterable, Union
 
 import numpy as np
 import torch
 from sklearn.linear_model import ElasticNet, Lasso, Ridge, SGDRegressor
 
-from cca_zoo.classical._iterative._base import BaseLoop
-from cca_zoo.classical._iterative._deflation import BaseDeflation
+from cca_zoo.linear._iterative._base import BaseLoop, BaseIterative
+from cca_zoo.linear._iterative._deflation import DeflationMixin
 from cca_zoo.utils import _process_parameter
 
 
-class ElasticCCA(BaseDeflation):
+class ElasticCCA(DeflationMixin, BaseIterative):
     r"""
     A class used to fit an elastic CCA model for two or more views of data.
 
     This model finds the linear projections of multiple views that maximize their pairwise correlations while enforcing L1 and L2 penalties on the projection vectors.
 
     ElasticCCA uses CCA with an auxiliary variable target i.e. MAXVAR configuration
 
@@ -49,15 +49,15 @@
     stochastic : bool, default=False
         Whether to use stochastic gradient descent
     positive : bool or list of bools, default=None
         Whether to use non-negative constraints
 
     Examples
     --------
-    >>> from cca_zoo.classical import ElasticCCA
+    >>> from cca_zoo.linear import ElasticCCA
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = ElasticCCA(c=[1e-1,1e-1],l1_ratio=[0.5,0.5], random_state=0)
     >>> model.fit((X1,X2)).score((X1,X2))
     array([0.9316638])
@@ -72,14 +72,15 @@
         deflation="cca",
         initialization: Union[str, callable] = "pls",
         tol: float = 1e-3,
         alpha: Union[Iterable[float], float] = None,
         l1_ratio: Union[Iterable[float], float] = None,
         stochastic=False,
         positive: Union[Iterable[bool], bool] = None,
+        trainer_kwargs=None,
         convergence_checking=None,
         track=None,
         verbose=False,
     ):
         self.alpha = alpha
         self.l1_ratio = l1_ratio
         self.stochastic = stochastic
@@ -93,20 +94,22 @@
             latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             epochs=epochs,
             deflation=deflation,
             initialization=initialization,
             tol=tol,
             random_state=random_state,
+            trainer_kwargs=trainer_kwargs,
             convergence_checking=convergence_checking,
             patience=0,
             track=track,
             verbose=verbose,
-            trainer_kwargs={"accelerator": "cpu"},
         )
+        # set trainer kwargs accelerator to 'cpu'
+        self.trainer_kwargs["accelerator"] = "cpu"
 
     def _check_params(self):
         self.alpha = _process_parameter("alpha", self.alpha, 0, self.n_views_)
         self.l1_ratio = _process_parameter("l1_ratio", self.l1_ratio, 0, self.n_views_)
         self.positive = _process_parameter(
             "positive", self.positive, False, self.n_views_
         )
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_ey.py` & `cca_zoo-2.0.8/cca_zoo/linear/_gradient/_ey.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union
 
 import numpy as np
 import torch
 
-from cca_zoo.classical._iterative._base import BaseIterative
-from cca_zoo.classical._iterative._gradient import GradientLoop
-from cca_zoo.classical._pls import PLSMixin
+from cca_zoo.linear._iterative._base import BaseIterative
+from cca_zoo.linear._gradient._gradient import GradientLoop
+from cca_zoo.linear._pls import PLSMixin
 
 
 class CCAEY(BaseIterative):
     """
     A class used to fit Regularized CCA by Delta-EigenGame
 
     Parameters
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_gh.py` & `cca_zoo-2.0.8/cca_zoo/linear/_gradient/_gh.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from cca_zoo.classical._iterative._ey import CCAEY, EYLoop
+from cca_zoo.linear._gradient._ey import CCAEY, EYLoop
 
 
 class CCAGH(CCAEY):
     def _get_module(self, weights=None, k=None):
         return GHALoop(
             weights=weights,
             k=k,
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_gradient.py` & `cca_zoo-2.0.8/cca_zoo/linear/_gradient/_gradient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from cca_zoo.classical._iterative._base import BaseLoop
+from cca_zoo.linear._iterative._base import BaseLoop
 
 
 class GradientLoop(BaseLoop):
     def __init__(
         self,
         weights=None,
         k=None,
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_gradkcca.py` & `cca_zoo-2.0.8/cca_zoo/nonparametric/_gradkcca.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 import numpy as np
 import numpy.linalg as la
 from sklearn.kernel_approximation import Nystroem
 from sklearn.metrics import pairwise_kernels
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.classical._iterative._base import BaseIterative
+from cca_zoo.linear._iterative._base import BaseIterative
+from cca_zoo.nonparametric._kcca import KernelMixin
 from cca_zoo.utils import _process_parameter
 
 
-class GradKCCA(BaseIterative):
+class GradKCCA(BaseIterative, KernelMixin):
     """
     References
     ----------
     [1] Viivi Uurtio, Sahely Bhadra, and Juho Rousu. Large-scale sparse kernel canonical correlation analysis. In Kamalika Chaudhuri and Ruslan Salakhutdinov, editors, Proceedings of the 36th International Conference on Machine Learning, volume 97 of Proceedings of Machine Learning Research, pages 6383–6391, Long Beach, California, USA, 09–15 Jun 2019. PMLR.
 
     """
 
@@ -60,38 +61,14 @@
         self.gamma = _process_parameter("gamma", self.gamma, None, self.n_views)
         self.coef0 = _process_parameter("coef0", self.coef0, 1, self.n_views)
         self.degree = _process_parameter("degree", self.degree, 1, self.n_views)
         self.nystrom_components = _process_parameter(
             "nystrom components", self.nystrom_components, 100, self.n_views
         )
 
-    def _get_kernel(self, view_index, X, Y=None):
-        if callable(self.kernel[view_index]):
-            params = self.kernel_params[view_index] or {}
-        else:
-            params = {
-                "gamma": self.gamma[view_index],
-                "degree": self.degree[view_index],
-                "coef0": self.coef0[view_index],
-            }
-        if self.nystrom:
-            nystroem = Nystroem(
-                kernel=self.kernel[view_index],
-                n_components=self.nystrom_components[view_index],
-                **params,
-            )
-            if Y is None:
-                Y = X
-            K = nystroem.fit_transform(X) @ nystroem.transform(Y).T
-            return K
-        else:
-            return pairwise_kernels(
-                X, Y, metric=self.kernel[view_index], filter_params=True, **params
-            )
-
     def backracking_line_search(self, w, gw, stp, X, K, obj_old, view_index):
         while True:
             w_new = w + gw * stp
             w_new = w_new / la.norm(w_new)
             Kw_new = self._get_kernel(view_index, X, w_new[None, :])
             obj_new = self._objective(None, (Kw_new, K), None)
             if obj_new > obj_old + 1e-4 * np.abs(obj_old):
@@ -157,14 +134,7 @@
                     weights[view_index], self.c[view_index]
                 )
             else:
                 raise ValueError(
                     "projection {self.proj[view_index]} not supported. Pass a generator implementing this method"
                 )
         return scores, weights
-
-    def transform(self, views: Iterable[np.ndarray], **kwargs):
-        check_is_fitted(self, attributes=["weights"])
-        scores = [
-            self._get_kernel(i, view, self.weights[i].T) for i, view in enumerate(views)
-        ]
-        return scores
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_incrementalpls.py` & `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_incrementalpls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union
 
 import numpy as np
 
-from cca_zoo.classical._iterative._base import BaseIterative
+from cca_zoo.linear._iterative._base import BaseIterative
 
 
 class IncrementalPLS(BaseIterative):
     r"""
     A class used to fit Incremental PLS
 
     Parameters
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_pls_als.py` & `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_pls_als.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Union
 
 import numpy as np
 
 
-from cca_zoo.classical._iterative._base import BaseLoop
-from cca_zoo.classical._iterative._deflation import BaseDeflation
-from cca_zoo.classical._pls import PLSMixin
+from cca_zoo.linear._iterative._base import BaseLoop, BaseIterative
+from cca_zoo.linear._iterative._deflation import DeflationMixin
+from cca_zoo.linear._pls import PLSMixin
 
 
-class PLS_ALS(BaseDeflation, PLSMixin):
+class PLS_ALS(PLSMixin, DeflationMixin, BaseIterative):
     r"""
     A class used to fit a PLS model by alternating least squares (ALS).
 
     This model finds the linear projections of two views that maximize their covariance while minimizing their residual variance.
 
     The objective function of PLS-ALS is:
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_pmd.py` & `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_pmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import itertools
 import warnings
 
 import numpy as np
 import torch
 
-from cca_zoo.classical._iterative._base import BaseLoop
-from cca_zoo.classical._iterative._deflation import BaseDeflation
-from cca_zoo.classical._pls import PLSMixin
-from cca_zoo.classical._search import _delta_search
+from cca_zoo.linear._iterative._base import BaseLoop, BaseIterative
+from cca_zoo.linear._iterative._deflation import DeflationMixin
+from cca_zoo.linear._pls import PLSMixin
+from cca_zoo.linear._search import _delta_search
 from cca_zoo.utils import _process_parameter
 
 
-class SCCA_PMD(BaseDeflation, PLSMixin):
+class SCCA_PMD(DeflationMixin, PLSMixin, BaseIterative):
     r"""
     A class used to fit a sparse CCA model by penalized matrix decomposition (PMD).
 
     This model finds the linear projections of two views that maximize their correlation while enforcing sparsity constraints on the projection vectors.
 
     The objective function of SCCA-PMD is:
 
@@ -68,32 +68,35 @@
         random_state=None,
         epochs=100,
         deflation="cca",
         initialization="pls",
         tol=1e-3,
         positive=False,
         tau=None,
+        trainer_kwargs=None,
         convergence_checking=None,
         track=None,
-        verbose=False,
+        verbose=None,
     ):
         super().__init__(
             latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             random_state=random_state,
             epochs=epochs,
             deflation=deflation,
             initialization=initialization,
             tol=tol,
+            trainer_kwargs=trainer_kwargs,
             convergence_checking=convergence_checking,
             patience=0,
             track=track,
             verbose=verbose,
-            trainer_kwargs={"accelerator": "cpu"},
         )
+        # set trainer kwargs accelerator to 'cpu'
+        self.trainer_kwargs["accelerator"] = "cpu"
         self.tau = tau
         self.positive = positive
 
     def _check_params(self):
         if self.tau is None:
             warnings.warn(
                 "tau parameter not set. Setting to tau=1 i.e. maximum regularisation of l1 norm"
@@ -153,15 +156,14 @@
             mask = np.arange(scores.shape[0]) != view_index
             # apply the mask to scores and sum along dim k
             target = np.sum(scores[mask], axis=0)
             self.weights[view_index] = view.T @ target
             self.weights[view_index] = _delta_search(
                 self.weights[view_index],
                 self.t[view_index],
-                tol=self.tol,
             )
             if np.linalg.norm(self.weights[view_index]) <= 0:
                 warnings.warn(
                     f"All result weights are zero in view {view_index}. "
                     "Try less regularisation or another initialisation"
                 )
         # if tracking or convergence_checking is enabled, compute the objective function
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_scca_admm.py` & `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_admm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Iterable, Union
 
 import numpy as np
 
 from cca_zoo.utils import _process_parameter
 from ._base import BaseIterative, BaseLoop
+from ._deflation import DeflationMixin
 
 
-class SCCA_ADMM(BaseIterative):
+class SCCA_ADMM(BaseIterative, DeflationMixin):
     r"""
     Fits a sparse CCA model by alternating ADMM for two or more views.
 
     .. math::
 
         w_{opt}=\underset{w}{\mathrm{argmax}}\{\sum_i\sum_{j\neq i} \|X_iw_i-X_jw_j\|^2 + \|w_i\|_1\}\\
 
@@ -45,15 +46,15 @@
 
     References
     ----------
     Suo, Xiaotong, et al. "Sparse canonical correlation analysis." arXiv preprint arXiv:1705.10865 (2017).
 
     Examples
     --------
-    >>> from cca_zoo.classical import SCCA_ADMM
+    >>> from cca_zoo.linear import SCCA_ADMM
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = SCCA_ADMM(random_state=0,tau=[1e-1,1e-1])
     >>> model.fit((X1,X2)).score((X1,X2))
     array([0.84348183])
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_scca_hsic.py` & `cca_zoo-2.0.8/cca_zoo/nonparametric/_scca_hsic.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import numpy.linalg as la
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import KernelCenterer
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.classical._iterative._gradkcca import GradKCCA
+from cca_zoo.nonparametric._gradkcca import GradKCCA
 from cca_zoo.utils import _process_parameter
 
 
 class SCCA_HSIC(GradKCCA):
     """
     References
     ----------
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_scca_parkhomenko.py` & `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_parkhomenko.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from typing import Iterable, Union
-
 import numpy as np
-import pytorch_lightning as pl
-
-from cca_zoo.classical._iterative._base import BaseLoop
-from cca_zoo.classical._iterative._deflation import BaseDeflation
-from cca_zoo.classical._search import _softthreshold
+from cca_zoo.linear._iterative._base import BaseLoop, BaseIterative
+from cca_zoo.linear._iterative._deflation import DeflationMixin
+from cca_zoo.linear._pls import PLSMixin
 from cca_zoo.utils import _process_parameter
 
 
-class SCCA_Parkhomenko(BaseDeflation):
+class SCCA_Parkhomenko(DeflationMixin, PLSMixin, BaseIterative):
     r"""
     A class used to fit a sparse CCA (penalized CCA) model for two or more views.
 
     This model finds the linear projections of multiple views that maximize their pairwise correlations while enforcing sparsity constraints on the projection vectors.
 
     The objective function of sparse CCA is:
 
@@ -29,15 +26,15 @@
 
     References
     ----------
     Parkhomenko, Elena, David Tritchler, and Joseph Beyene. "Sparse canonical correlation analysis with application to genomic data integration." Statistical applications in genetics and molecular biology 8.1 (2009).
 
     Examples
     --------
-    >>> from cca_zoo.classical import SCCA_Parkhomenko
+    >>> from cca_zoo.linear import SCCA_Parkhomenko
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = SCCA_Parkhomenko(tau=[0.001,0.001],random_state=0)
     >>> model.fit((X1,X2)).score((X1,X2))
     array([0.81803527])
@@ -105,11 +102,12 @@
             mask = np.arange(scores.shape[0]) != view_index
             # apply the mask to scores and sum along dim k
             target = np.sum(scores[mask], axis=0)
             self.weights[view_index] = np.cov(
                 np.hstack((batch["views"][view_index], target[:, np.newaxis])).T
             )[:-1, -1]
             self.weights[view_index] /= np.linalg.norm(self.weights[view_index])
-            self.weights[view_index] = _softthreshold(
-                self.weights[view_index], self.tau[view_index] / 2
-            )
+            # Apply soft thresholding to the weights with optimal delta
+            self.weights[view_index] = np.clip(
+                self.weights[view_index] - self.tau[view_index] / 2, 0, None
+            ) - np.clip(-self.weights[view_index] - self.tau[view_index] / 2, 0, None)
             self.weights[view_index] /= np.linalg.norm(self.weights[view_index])
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_scca_span.py` & `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_span.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Iterable, Union
 
 import numpy as np
-import torch
 
-from cca_zoo.classical._iterative._base import BaseIterative, BaseLoop
-from cca_zoo.classical._search import _delta_search, support_threshold
+from cca_zoo.linear._iterative._base import BaseIterative, BaseLoop
+from cca_zoo.linear._iterative._deflation import DeflationMixin
+from cca_zoo.linear._search import _delta_search, support_threshold
 from cca_zoo.utils import _process_parameter
 
 
-class SCCA_Span(BaseIterative):
+class SCCA_Span(DeflationMixin, BaseIterative):
     r"""
     Fits a Sparse CCA model using SpanCCA.
 
     .. math::
 
         w_{opt}=\underset{w}{\mathrm{argmax}}\{\sum_i\sum_{j\neq i} \|X_iw_i-X_jw_j\|^2 + \text{l1_ratio}\|w_i\|_1\}\\
 
@@ -23,15 +23,15 @@
     References
     ----------
     Asteris, Megasthenis, et al. "A simple and provable algorithm for sparse diagonal CCA." International Conference on Machine Learning. PMLR, 2016.
 
 
     Examples
     --------
-    >>> from cca_zoo.classical import SCCA_Span
+    >>> from cca_zoo.linear import SCCA_Span
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = SCCA_Span(regularisation="l0", tau=[2, 2])
     >>> model.fit((X1,X2)).score((X1,X2))
     array([0.84556666])
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_svd.py` & `cca_zoo-2.0.8/cca_zoo/linear/_gradient/_svd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Union
 
 import torch
 
-from cca_zoo.classical._iterative._ey import CCAEY, EYLoop
-from cca_zoo.classical._pls import PLSMixin
+
+from cca_zoo.linear._gradient._ey import EYLoop, CCAEY
+from cca_zoo.linear._pls import PLSMixin
 
 
 class CCASVD(CCAEY):
     def _get_module(self, weights=None, k=None):
         return SVDLoop(
             weights=weights,
             k=k,
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_iterative/_swcca.py` & `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_swcca.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from itertools import combinations
 from typing import Iterable, Union
 
 import numpy as np
 
-from cca_zoo.classical._base import _BaseIterative
-from cca_zoo.classical._search import _delta_search, support_threshold
+from cca_zoo.linear._iterative._base import BaseIterative
+from cca_zoo.linear._iterative._deflation import DeflationMixin
+from cca_zoo.linear._search import _delta_search, support_threshold
 from cca_zoo.utils import _process_parameter
 
 
-class SWCCA(_BaseIterative):
+class SWCCA(BaseIterative, DeflationMixin):
     r"""
     A class used to fit SWCCA model
 
     References
     ----------
     .. Wenwen, M. I. N., L. I. U. Juan, and Shihua Zhang. "Sparse Weighted Canonical Correlation Analysis." Chinese Journal of Electronics 27.3 (2018): 459-466.
 
     Examples
     --------
-    >>> from cca_zoo.classical import SWCCA
+    >>> from cca_zoo.linear import SWCCA
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = SWCCA(regularisation='l0',tau=[2, 2], sample_support=5, random_state=0)
     >>> model.fit((X1,X2)).score((X1,X2))
     array([0.61620969])
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_kcca.py` & `cca_zoo-2.0.8/cca_zoo/nonparametric/_kcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import numpy as np
 from scipy.linalg import block_diag
 from sklearn.metrics import pairwise_kernels
 from sklearn.utils.validation import check_is_fitted
 
 from cca_zoo.utils import _process_parameter
-from ._gcca import GCCA
-from ._mcca import MCCA
-from ._tcca import TCCA
+from cca_zoo.linear._gcca import GCCA
+from cca_zoo.linear._mcca import MCCA
+from cca_zoo.linear._tcca import TCCA
 
 
 class KernelMixin:
     def _check_params(self):
         self.kernel = _process_parameter("kernel", self.kernel, "linear", self.n_views_)
         self.gamma = _process_parameter("gamma", self.gamma, None, self.n_views_)
         self.coef0 = _process_parameter("coef0", self.coef0, 1, self.n_views_)
@@ -101,15 +101,15 @@
     coef0: Iterable[float], optional
         Coef0 parameter or list of parameters for the polynomial or sigmoid kernel for each view, by default None. Ignored if kernel is not polynomial or sigmoid.
     kernel_params: Iterable[dict], optional
         Additional parameters or list of parameters for the kernel function for each view, by default None.
 
     Examples
     --------
-    >>> from cca_zoo.classical import KCCA
+    >>> from cca_zoo.linear import KCCA
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> X3 = rng.random((10,5))
     >>> model = KCCA()
     >>> model.fit((X1,X2,X3)).score((X1,X2,X3))
@@ -202,15 +202,15 @@
 
     References
     ----------
     Tenenhaus, Arthur, Cathy Philippe, and Vincent Frouin. "Kernel generalized canonical correlation analysis." Computational Statistics & Data Analysis 90 (2015): 114-131.
 
     Examples
     --------
-    >>> from cca_zoo.classical import KGCCA
+    >>> from cca_zoo.linear import KGCCA
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> X3 = rng.random((10,5))
     >>> model = KGCCA()
     >>> model.fit((X1,X2,X3)).score((X1,X2,X3))
@@ -286,15 +286,15 @@
 
     References
     ----------
     Kim, Tae-Kyun, Shu-Fai Wong, and Roberto Cipolla. "Tensor canonical correlation analysis for action classification." 2007 IEEE Conference on Computer Vision and Pattern Recognition. IEEE, 2007
 
     Examples
     --------
-    >>> from cca_zoo.classical import KTCCA
+    >>> from cca_zoo.linear import KTCCA
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> X3 = rng.random((10,5))
     >>> model = KTCCA()
     >>> model.fit((X1,X2,X3)).score((X1,X2,X3))
     array([1.69896269])
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_mcca.py` & `cca_zoo-2.0.8/cca_zoo/linear/_mcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterable, Union
 
 import numpy as np
 from scipy.linalg import block_diag
 from scipy.linalg import eigh
 from sklearn.decomposition import PCA
 
-from cca_zoo.classical._base import BaseModel
+from cca_zoo.linear._base import BaseModel
 from cca_zoo.utils import _process_parameter
 
 
 class MCCA(BaseModel):
     r"""
     A class used to fit Regularised CCA (canonical ridge) model. This model adds a regularization term to the CCA objective function to avoid overfitting and improve stability. It uses PCA to perform the optimization efficiently for high dimensional data.
 
@@ -274,15 +274,15 @@
     References
     --------
 
     Hotelling, Harold. "Relations between two sets of variates." Breakthroughs in statistics. Springer, New York, NY, 1992. 162-190.
 
     Example
     -------
-    >>> from cca_zoo.classical import CCA
+    >>> from cca_zoo.linear import CCA
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = CCA()
     >>> model.fit((X1,X2)).score((X1,X2))
     array([1.])
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_ncca.py` & `cca_zoo-2.0.8/cca_zoo/nonparametric/_ncca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Iterable, Union
 
 import numpy as np
 from sklearn.metrics import pairwise_kernels
 from sklearn.neighbors import NearestNeighbors
 
-from cca_zoo.classical._base import BaseModel
+from cca_zoo.linear._base import BaseModel
 from cca_zoo.utils.check_values import _process_parameter
 
 
 class NCCA(BaseModel):
     """
     A class used to fit nonparametric (NCCA) model. This model extends CCA to nonlinear relationships by using local linear projections based on nearest neighbors.
 
@@ -30,15 +30,15 @@
 
     References
     ----------
     Michaeli, Tomer, Weiran Wang, and Karen Livescu. "Nonparametric canonical correlation analysis." International conference on machine learning. PMLR, 2016.
 
     Example
     -------
-    >>> from cca_zoo.classical import NCCA
+    >>> from cca_zoo.linear import NCCA
     >>> X1 = np.random.rand(10,5)
     >>> X2 = np.random.rand(10,5)
     >>> model = NCCA()
     >>> model.fit((X1,X2)).score((X1,X2))
     array([1.])
     """
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_partialcca.py` & `cca_zoo-2.0.8/cca_zoo/linear/_partialcca.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterable, Union
 
 import numpy as np
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.classical import MCCA
+from cca_zoo.linear import MCCA
 
 
 class PartialCCA(MCCA):
     r"""
     A class used to fit a partial CCA model. This model extends CCA to account for confounding variables that may affect the correlation between views.
 
     .. math::
@@ -23,15 +23,15 @@
 
     References
     ----------
     Rao, B. Raja. "Partial canonical correlations." Trabajos de estadistica y de investigación operativa 20.2-3 (1969): 211-219.
 
     Example
     -------
-    >>> from cca_zoo.classical import PartialCCA
+    >>> from cca_zoo.linear import PartialCCA
     >>> X1 = np.random.rand(10,5)
     >>> X2 = np.random.rand(10,5)
     >>> partials = np.random.rand(10,3)
     >>> model = PartialCCA()
     >>> model.fit((X1,X2),partials=partials).score((X1,X2))
     array([0.99993046])
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_pcacca.py` & `cca_zoo-2.0.8/cca_zoo/linear/_pcacca.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Union
 
 import numpy as np
 
-from cca_zoo.classical._mcca import MCCA
+from cca_zoo.linear._mcca import MCCA
 
 
 class PCACCA(MCCA):
     """
     Principal Component Analysis CCA
 
     Data driven PCA on each view followed by CCA on the PCA components. Keep percentage of variance
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_pls.py` & `cca_zoo-2.0.8/cca_zoo/linear/_pls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cca_zoo.classical import rCCA, MCCA
+from cca_zoo.linear import rCCA, MCCA
 from typing import Iterable
 
 import numpy as np
 
 
 def reduce_dims(x):
     U, S, _ = np.linalg.svd(x, full_matrices=False)
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_prcca.py` & `cca_zoo-2.0.8/cca_zoo/linear/_prcca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import warnings
 from typing import Iterable
 
 import numpy as np
 from scipy.linalg import block_diag
 
-from cca_zoo.classical._mcca import MCCA
+from cca_zoo.linear._mcca import MCCA
 
 
 class PRCCA(MCCA):
     """
     Partially Regularized Canonical Correlation Analysis
```

### Comparing `cca_zoo-2.0.7/cca_zoo/classical/_tcca.py` & `cca_zoo-2.0.8/cca_zoo/linear/_tcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterable
 
 import numpy as np
 import tensorly as tl
 from scipy.linalg import sqrtm
 from tensorly.decomposition import parafac
 
-from cca_zoo.classical import MCCA
+from cca_zoo.linear import MCCA
 
 
 class TCCA(MCCA):
     r"""
     A class used to fit TCCA model. This model extends MCCA to higher order correlations by using tensor products of the views.
 
     The objective function of TCCA is:
@@ -26,15 +26,15 @@
 
     References
     ----------
     Kim, Tae-Kyun, Shu-Fai Wong, and Roberto Cipolla. "Tensor canonical correlation analysis for action classification." 2007 IEEE Conference on Computer Vision and Pattern Recognition. IEEE, 2007
 
     Examples
     --------
-    >>> from cca_zoo.classical import TCCA
+    >>> from cca_zoo.linear import TCCA
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> X3 = rng.random((10,5))
     >>> model = TCCA()
     >>> model.fit((X1,X2,X3)).score((X1,X2,X3))
     array([1.14595755])
```

### Comparing `cca_zoo-2.0.7/cca_zoo/data/deep.py` & `cca_zoo-2.0.8/cca_zoo/data/deep.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/data/simulated.py` & `cca_zoo-2.0.8/cca_zoo/data/simulated.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sklearn.datasets import make_spd_matrix
 from sklearn.utils.validation import check_random_state
 
 from cca_zoo.utils import _process_parameter
 
 
 class LinearSimulatedData:
-    # This class generates simulated data for linear classical with multiple views
+    # This class generates simulated data for linear linear with multiple views
     def __init__(
         self,
         view_features: List[int],
         latent_dims: int = 1,
         view_sparsity: Union[List[float], float] = None,
         correlation: Union[List[float], float] = 0.99,
         structure: str = "random",
@@ -34,14 +34,15 @@
         )
         self.structure = _process_parameter(
             "structure", structure, "random", len(view_features)
         )
         self.positive = _process_parameter(
             "positive", positive, False, len(view_features)
         )
+        self.rng = check_random_state(self.random_state)
         # Generate the covariance matrices and the true features for each view
         covs, self.true_features = self._generate_covariance_matrices()
         # Generate the joint covariance matrix by combining the view covariances and the cross-covariances
         joint_cov = self._generate_joint_covariance(covs)
         # Compute the Cholesky decomposition of the joint covariance matrix
         self.chol = np.linalg.cholesky(joint_cov)
 
@@ -139,24 +140,19 @@
         return weights * mask
 
     def _make_weights_positive(self, weights):
         # set all negative elements to zero
         return np.abs(weights)
 
     def sample(self, n: int):
-        X = np.zeros((n, self.chol.shape[0]))
-        for i in range(n):
-            X[i, :] = self._chol_sample(self.chol)
+        # Sample from the model by multiplying the Cholesky decomposition of the joint covariance matrix by a random vector
+        X = (self.chol @ self.rng.randn(self.chol.shape[0], n)).T
         views = np.split(X, np.cumsum(self.view_features)[:-1], axis=1)
         return views
 
-    def _chol_sample(self, chol):
-        rng = check_random_state(self.random_state)
-        return chol @ rng.randn(chol.shape[0])
-
 
 def _decorrelate_dims(up, cov):
     A = up.T @ cov @ up
     for k in range(1, A.shape[0]):
         up[:, k:] -= np.outer(up[:, k - 1], A[k - 1, k:] / A[k - 1, k - 1])
         A = up.T @ cov @ up
     return up
```

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/__init__.py` & `cca_zoo-2.0.8/cca_zoo/deep/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_base.py` & `cca_zoo-2.0.8/cca_zoo/deep/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import pytorch_lightning as pl
 import torch
 from torch.optim.lr_scheduler import CosineAnnealingLR, MultiStepLR
 
 
 class BaseDeep(pl.LightningModule):
-    """A base class for deep learning classical using PyTorch Lightning."""
+    """A base class for deep learning linear using PyTorch Lightning."""
 
     def __init__(
         self,
         latent_dimensions: int,
         optimizer: str = "adam",
         scheduler: Optional[str] = None,
         lr: float = 1e-2,
```

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca.py` & `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 
 from cca_zoo.deep import objectives
 from cca_zoo.deep._base import BaseDeep
 from cca_zoo.deep.metrics import MCCA
-from cca_zoo.classical._base import BaseModel
+from cca_zoo.linear._base import BaseModel
 
 
 class DCCA(BaseDeep, BaseModel):
     """
     A class used to fit a DCCA model.
 
     References
```

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py` & `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca_ey.py` & `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_ey.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca_gh.py` & `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_gh.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca_noi.py` & `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_noi.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca_sdl.py` & `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_sdl.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dcca_svd.py` & `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_svd.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dgcca.py` & `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dgcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_discriminative/_dtcca.py` & `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dtcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_generative/_base.py` & `cca_zoo-2.0.8/cca_zoo/deep/_generative/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_generative/_dccae.py` & `cca_zoo-2.0.8/cca_zoo/deep/_generative/_dccae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_generative/_dvcca.py` & `cca_zoo-2.0.8/cca_zoo/deep/_generative/_dvcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/_generative/_splitae.py` & `cca_zoo-2.0.8/cca_zoo/deep/_generative/_splitae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/architectures.py` & `cca_zoo-2.0.8/cca_zoo/deep/architectures.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/metrics.py` & `cca_zoo-2.0.8/cca_zoo/deep/metrics.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/deep/objectives.py` & `cca_zoo-2.0.8/cca_zoo/deep/objectives.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/model_selection/_search.py` & `cca_zoo-2.0.8/cca_zoo/model_selection/_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
 
 class GridSearchCV(BaseSearchCV):
     """
 
     :Example:
     >>> from cca_zoo.model_selection import GridSearchCV
-    >>> from cca_zoo.classical import MCCA
+    >>> from cca_zoo.linear import MCCA
     >>> X1 = [[0, 0, 1], [1, 0, 0], [2, 2, 2], [3, 5, 4]]
     >>> X2 = [[0.1, -0.2], [0.9, 1.1], [6.2, 5.9], [11.9, 12.3]]
     >>> X3 = [[0, 1, 0], [1, 9, 0], [4, 3, 3,], [12, 8, 10]]
     >>> model = MCCA()
     >>> params = {'c': [[0.1, 0.2], [0.3, 0.4], 0.1]}
     >>> GridSearchCV(model,param_grid=params, cv=3).fit([X1,X2,X3]).best_estimator_.c
     [0.1, 0.3, 0.1]
@@ -214,15 +214,15 @@
 
 
 class RandomizedSearchCV(BaseSearchCV):
     """
 
     :Example:
     >>> from cca_zoo.model_selection import RandomizedSearchCV
-    >>> from cca_zoo.classical import MCCA
+    >>> from cca_zoo.linear import MCCA
     >>> from sklearn._utils.fixes import loguniform
     >>> X1 = [[0, 0, 1], [1, 0, 0], [2, 2, 2], [3, 5, 4]]
     >>> X2 = [[0.1, -0.2], [0.9, 1.1], [6.2, 5.9], [11.9, 12.3]]
     >>> X3 = [[0, 1, 0], [1, 9, 0], [4, 3, 3,], [12, 8, 10]]
     >>> model = MCCA()
     >>> params = {'c': [loguniform(1e-4, 1e0), loguniform(1e-4, 1e0), [0.1]]}
     >>> def scorer(estimator, views):
```

### Comparing `cca_zoo-2.0.7/cca_zoo/model_selection/_validation.py` & `cca_zoo-2.0.8/cca_zoo/model_selection/_validation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/probabilistic/_probabilisticcca.py` & `cca_zoo-2.0.8/cca_zoo/probabilistic/_probabilisticcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import numpyro
 import numpyro.distributions as dist
 from jax.random import PRNGKey
 from numpyro.infer import MCMC, NUTS, Predictive
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.classical._base import BaseModel
+from cca_zoo.linear._base import BaseModel
 
 
 class ProbabilisticCCA(BaseModel):
     """
     A class used to fit a Probabilistic CCA. Not quite the same due to using VI methods rather than EM
 
     Parameters
```

### Comparing `cca_zoo-2.0.7/cca_zoo/utils/check_values.py` & `cca_zoo-2.0.8/cca_zoo/utils/check_values.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.7/cca_zoo/visualisation/plotting.py` & `cca_zoo-2.0.8/cca_zoo/visualisation/plotting.py`

 * *Files identical despite different names*

