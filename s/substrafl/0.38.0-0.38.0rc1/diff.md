# Comparing `tmp/substrafl-0.38.0.tar.gz` & `tmp/substrafl-0.38.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrafl-0.38.0.tar", last modified: Fri Jun 30 10:06:29 2023, max compression
+gzip compressed data, was "substrafl-0.38.0rc1.tar", last modified: Tue Jun 27 09:44:58 2023, max compression
```

## Comparing `substrafl-0.38.0.tar` & `substrafl-0.38.0rc1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.638620 substrafl-0.38.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-06-30 10:06:26.000000 substrafl-0.38.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-30 10:06:29.638620 substrafl-0.38.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-30 10:06:26.000000 substrafl-0.38.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-30 10:06:26.000000 substrafl-0.38.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 10:06:29.638620 substrafl-0.38.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-30 10:06:26.000000 substrafl-0.38.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.630620 substrafl-0.38.0/substrafl/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.634620 substrafl-0.38.0/substrafl/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/algorithms/algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.634620 substrafl-0.38.0/substrafl/algorithms/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/algorithms/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/algorithms/pytorch/torch_base_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    23454 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/algorithms/pytorch/torch_scaffold_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/algorithms/pytorch/torch_single_organization_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/algorithms/pytorch/weight_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/compute_plan_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.634620 substrafl-0.38.0/substrafl/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/dependency/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/dependency/path_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/dependency/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/evaluation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.634620 substrafl-0.38.0/substrafl/index_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/index_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/index_generator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/index_generator/np_index_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18182 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/model_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.634620 substrafl-0.38.0/substrafl/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/nodes/aggregation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/nodes/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.634620 substrafl-0.38.0/substrafl/nodes/references/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/nodes/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/nodes/references/local_state.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/nodes/references/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/nodes/test_data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/nodes/train_data_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.634620 substrafl-0.38.0/substrafl/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/remote/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/remote/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.634620 substrafl-0.38.0/substrafl/remote/register/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/remote/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/remote/register/generate_wheel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/remote/register/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/remote/remote_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.634620 substrafl-0.38.0/substrafl/remote/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/remote/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/remote/serializers/pickle_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/remote/serializers/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/remote/substratools_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.638620 substrafl-0.38.0/substrafl/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/strategies/fed_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/strategies/fed_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/strategies/newton_raphson.py
--rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/strategies/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/strategies/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/strategies/single_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-30 10:06:26.000000 substrafl-0.38.0/substrafl/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:06:29.634620 substrafl-0.38.0/substrafl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-30 10:06:29.000000 substrafl-0.38.0/substrafl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-30 10:06:29.000000 substrafl-0.38.0/substrafl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:06:29.000000 substrafl-0.38.0/substrafl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-30 10:06:29.000000 substrafl-0.38.0/substrafl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 10:06:29.000000 substrafl-0.38.0/substrafl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.935521 substrafl-0.38.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-27 09:44:58.935521 substrafl-0.38.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:44:58.935521 substrafl-0.38.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.927521 substrafl-0.38.0rc1/substrafl/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.927521 substrafl-0.38.0rc1/substrafl/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23454 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/weight_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/compute_plan_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/dependency/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/dependency/path_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/dependency/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/evaluation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/index_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/index_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/index_generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/index_generator/np_index_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18182 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/model_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/aggregation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/nodes/references/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/references/local_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/references/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/test_data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/train_data_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/remote/register/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/register/generate_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/register/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/remote_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/remote/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/serializers/pickle_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/serializers/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/substratools_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.935521 substrafl-0.38.0rc1/substrafl/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/fed_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/fed_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/newton_raphson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/single_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.927521 substrafl-0.38.0rc1/substrafl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-27 09:44:58.000000 substrafl-0.38.0rc1/substrafl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-27 09:44:58.000000 substrafl-0.38.0rc1/substrafl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:44:58.000000 substrafl-0.38.0rc1/substrafl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-27 09:44:58.000000 substrafl-0.38.0rc1/substrafl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 09:44:58.000000 substrafl-0.38.0rc1/substrafl.egg-info/top_level.txt
```

### Comparing `substrafl-0.38.0/LICENSE` & `substrafl-0.38.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/PKG-INFO` & `substrafl-0.38.0rc1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.38.0
+Version: 0.38.0rc1
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.38.0/README.md` & `substrafl-0.38.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/pyproject.toml` & `substrafl-0.38.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/setup.py` & `substrafl-0.38.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/__init__.py` & `substrafl-0.38.0rc1/substrafl/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/algorithms/algo.py` & `substrafl-0.38.0rc1/substrafl/algorithms/algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/algorithms/pytorch/__init__.py` & `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/algorithms/pytorch/torch_base_algo.py` & `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/algorithms/pytorch/torch_fed_avg_algo.py` & `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/algorithms/pytorch/torch_fed_pca_algo.py` & `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py` & `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/algorithms/pytorch/torch_scaffold_algo.py` & `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/algorithms/pytorch/torch_single_organization_algo.py` & `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/algorithms/pytorch/weight_manager.py` & `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/weight_manager.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/compute_plan_builder.py` & `substrafl-0.38.0rc1/substrafl/compute_plan_builder.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/dependency/constants.py` & `substrafl-0.38.0rc1/substrafl/dependency/constants.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/dependency/path_management.py` & `substrafl-0.38.0rc1/substrafl/dependency/path_management.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/dependency/schemas.py` & `substrafl-0.38.0rc1/substrafl/dependency/schemas.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/evaluation_strategy.py` & `substrafl-0.38.0rc1/substrafl/evaluation_strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/exceptions.py` & `substrafl-0.38.0rc1/substrafl/exceptions.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/experiment.py` & `substrafl-0.38.0rc1/substrafl/experiment.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/index_generator/base.py` & `substrafl-0.38.0rc1/substrafl/index_generator/base.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/index_generator/np_index_generator.py` & `substrafl-0.38.0rc1/substrafl/index_generator/np_index_generator.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/logger.py` & `substrafl-0.38.0rc1/substrafl/logger.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/model_loading.py` & `substrafl-0.38.0rc1/substrafl/model_loading.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/nodes/__init__.py` & `substrafl-0.38.0rc1/substrafl/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/nodes/aggregation_node.py` & `substrafl-0.38.0rc1/substrafl/nodes/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/nodes/node.py` & `substrafl-0.38.0rc1/substrafl/nodes/node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/nodes/test_data_node.py` & `substrafl-0.38.0rc1/substrafl/nodes/test_data_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/nodes/train_data_node.py` & `substrafl-0.38.0rc1/substrafl/nodes/train_data_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/remote/decorators.py` & `substrafl-0.38.0rc1/substrafl/remote/decorators.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/remote/operations.py` & `substrafl-0.38.0rc1/substrafl/remote/operations.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/remote/register/generate_wheel.py` & `substrafl-0.38.0rc1/substrafl/remote/register/generate_wheel.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/remote/register/register.py` & `substrafl-0.38.0rc1/substrafl/remote/register/register.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/remote/remote_struct.py` & `substrafl-0.38.0rc1/substrafl/remote/remote_struct.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/remote/serializers/pickle_serializer.py` & `substrafl-0.38.0rc1/substrafl/remote/serializers/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/remote/substratools_methods.py` & `substrafl-0.38.0rc1/substrafl/remote/substratools_methods.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/strategies/fed_avg.py` & `substrafl-0.38.0rc1/substrafl/strategies/fed_avg.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/strategies/fed_pca.py` & `substrafl-0.38.0rc1/substrafl/strategies/fed_pca.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/strategies/newton_raphson.py` & `substrafl-0.38.0rc1/substrafl/strategies/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/strategies/scaffold.py` & `substrafl-0.38.0rc1/substrafl/strategies/scaffold.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/strategies/schemas.py` & `substrafl-0.38.0rc1/substrafl/strategies/schemas.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/strategies/single_organization.py` & `substrafl-0.38.0rc1/substrafl/strategies/single_organization.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl/strategies/strategy.py` & `substrafl-0.38.0rc1/substrafl/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0/substrafl.egg-info/PKG-INFO` & `substrafl-0.38.0rc1/substrafl.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.38.0
+Version: 0.38.0rc1
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.38.0/substrafl.egg-info/SOURCES.txt` & `substrafl-0.38.0rc1/substrafl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

