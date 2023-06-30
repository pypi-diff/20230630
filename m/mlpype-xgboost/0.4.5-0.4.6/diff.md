# Comparing `tmp/mlpype-xgboost-0.4.5.tar.gz` & `tmp/mlpype-xgboost-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-xgboost-0.4.5.tar", last modified: Mon Jun 26 20:43:25 2023, max compression
+gzip compressed data, was "mlpype-xgboost-0.4.6.tar", last modified: Fri Jun 30 14:22:55 2023, max compression
```

## Comparing `mlpype-xgboost-0.4.5.tar` & `mlpype-xgboost-0.4.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:43:25.325697 mlpype-xgboost-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 20:43:25.325697 mlpype-xgboost-0.4.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:43:25.325697 mlpype-xgboost-0.4.5/mlpype_xgboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 20:43:25.000000 mlpype-xgboost-0.4.5/mlpype_xgboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-26 20:43:25.000000 mlpype-xgboost-0.4.5/mlpype_xgboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:43:25.000000 mlpype-xgboost-0.4.5/mlpype_xgboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-26 20:43:25.000000 mlpype-xgboost-0.4.5/mlpype_xgboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:43:25.000000 mlpype-xgboost-0.4.5/mlpype_xgboost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:43:25.325697 mlpype-xgboost-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-26 20:39:45.000000 mlpype-xgboost-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:55.699551 mlpype-xgboost-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 14:22:55.699551 mlpype-xgboost-0.4.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:55.699551 mlpype-xgboost-0.4.6/mlpype_xgboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 14:22:55.000000 mlpype-xgboost-0.4.6/mlpype_xgboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-30 14:22:55.000000 mlpype-xgboost-0.4.6/mlpype_xgboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:22:55.000000 mlpype-xgboost-0.4.6/mlpype_xgboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-30 14:22:55.000000 mlpype-xgboost-0.4.6/mlpype_xgboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:22:55.000000 mlpype-xgboost-0.4.6/mlpype_xgboost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:22:55.699551 mlpype-xgboost-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-30 14:18:44.000000 mlpype-xgboost-0.4.6/setup.py
```

