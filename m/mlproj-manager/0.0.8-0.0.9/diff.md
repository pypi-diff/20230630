# Comparing `tmp/mlproj_manager-0.0.8.tar.gz` & `tmp/mlproj_manager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlproj_manager-0.0.8.tar", last modified: Mon Jun 12 17:03:28 2023, max compression
+gzip compressed data, was "mlproj_manager-0.0.9.tar", last modified: Thu Jun 15 17:16:50 2023, max compression
```

## Comparing `mlproj_manager-0.0.8.tar` & `mlproj_manager-0.0.9.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.522817 mlproj_manager-0.0.8/
--rw-r--r--   0 rlai       (501) staff       (20)     1068 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/LICENSE
--rw-r--r--   0 rlai       (501) staff       (20)     2266 2023-06-12 17:03:28.523012 mlproj_manager-0.0.8/PKG-INFO
--rw-r--r--   0 rlai       (501) staff       (20)     1777 2023-06-05 20:14:53.000000 mlproj_manager-0.0.8/README.md
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.490764 mlproj_manager-0.0.8/mlproj_manager/
--rw-r--r--   0 rlai       (501) staff       (20)       62 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)      301 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/definitions.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.496502 mlproj_manager-0.0.8/mlproj_manager/experiments/
--rw-r--r--   0 rlai       (501) staff       (20)      102 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/experiments/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     1699 2023-06-12 17:02:12.000000 mlproj_manager-0.0.8/mlproj_manager/experiments/abstract_experiment.py
--rw-r--r--   0 rlai       (501) staff       (20)     3184 2023-02-09 17:13:35.000000 mlproj_manager-0.0.8/mlproj_manager/experiments/experiment_runner.py
--rw-r--r--   0 rlai       (501) staff       (20)     2724 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/experiments/register_experiment.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.499060 mlproj_manager-0.0.8/mlproj_manager/file_management/
--rw-r--r--   0 rlai       (501) staff       (20)      760 2023-02-17 21:24:26.000000 mlproj_manager-0.0.8/mlproj_manager/file_management/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     5286 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/file_management/experiment_management.py
--rw-r--r--   0 rlai       (501) staff       (20)    13624 2023-03-01 03:25:29.000000 mlproj_manager-0.0.8/mlproj_manager/file_management/file_and_directory_management.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.499896 mlproj_manager-0.0.8/mlproj_manager/function_approximators/
--rw-r--r--   0 rlai       (501) staff       (20)       30 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/function_approximators/__init__.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.502743 mlproj_manager-0.0.8/mlproj_manager/function_approximators/neural_networks/
--rw-r--r--   0 rlai       (501) staff       (20)       92 2023-06-06 15:46:12.000000 mlproj_manager-0.0.8/mlproj_manager/function_approximators/neural_networks/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     9821 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/function_approximators/neural_networks/convolutional_network.py
--rw-r--r--   0 rlai       (501) staff       (20)     6295 2023-06-06 15:46:12.000000 mlproj_manager-0.0.8/mlproj_manager/function_approximators/neural_networks/general_deep_network.py
--rw-r--r--   0 rlai       (501) staff       (20)     8422 2023-03-01 03:30:11.000000 mlproj_manager-0.0.8/mlproj_manager/main.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.506453 mlproj_manager-0.0.8/mlproj_manager/plots_and_summaries/
--rw-r--r--   0 rlai       (501) staff       (20)        0 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/plots_and_summaries/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)    12903 2023-02-21 20:11:42.000000 mlproj_manager-0.0.8/mlproj_manager/plots_and_summaries/plot_results.py
--rw-r--r--   0 rlai       (501) staff       (20)     3960 2023-02-21 19:55:11.000000 mlproj_manager-0.0.8/mlproj_manager/plots_and_summaries/plotting_functions.py
--rw-r--r--   0 rlai       (501) staff       (20)      659 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/plots_and_summaries/summaries.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.507330 mlproj_manager-0.0.8/mlproj_manager/problems/
--rw-r--r--   0 rlai       (501) staff       (20)       35 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/problems/__init__.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.510492 mlproj_manager-0.0.8/mlproj_manager/problems/reinforcement_learning/
--rw-r--r--   0 rlai       (501) staff       (20)       89 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/problems/reinforcement_learning/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     1574 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py
--rw-r--r--   0 rlai       (501) staff       (20)     6238 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/problems/reinforcement_learning/mountain_car.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.512097 mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/
--rw-r--r--   0 rlai       (501) staff       (20)      243 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     1301 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/abstract_dataset.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.513378 mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/cifar/
--rw-r--r--   0 rlai       (501) staff       (20)     9890 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/cifar/cifar_data_loader.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.514183 mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/mnist/
--rw-r--r--   0 rlai       (501) staff       (20)     7610 2023-02-09 19:08:17.000000 mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/mnist/mnist_data_loader.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.515024 mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/target_generating_network/
--rw-r--r--   0 rlai       (501) staff       (20)     4336 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/target_generating_network/taget_generating_network.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.516452 mlproj_manager-0.0.8/mlproj_manager/util/
--rw-r--r--   0 rlai       (501) staff       (20)      145 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/util/__init__.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.518707 mlproj_manager-0.0.8/mlproj_manager/util/data_preprocessing_and_transformations/
--rw-r--r--   0 rlai       (501) staff       (20)      163 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/util/data_preprocessing_and_transformations/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     7164 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/util/data_preprocessing_and_transformations/image_transformations.py
--rw-r--r--   0 rlai       (501) staff       (20)     3928 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/util/data_preprocessing_and_transformations/normalization_and_preprocessing.py
--rw-r--r--   0 rlai       (501) staff       (20)     1750 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/util/experiments_util.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.522046 mlproj_manager-0.0.8/mlproj_manager/util/neural_networks/
--rw-r--r--   0 rlai       (501) staff       (20)      449 2023-06-05 20:01:39.000000 mlproj_manager-0.0.8/mlproj_manager/util/neural_networks/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     1986 2023-06-05 20:07:28.000000 mlproj_manager-0.0.8/mlproj_manager/util/neural_networks/network_architecture.py
--rw-r--r--   0 rlai       (501) staff       (20)      287 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/util/neural_networks/other_torch_utilities.py
--rw-r--r--   0 rlai       (501) staff       (20)     6328 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/mlproj_manager/util/neural_networks/weights_initialization_and_manipulation.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-12 17:03:28.494073 mlproj_manager-0.0.8/mlproj_manager.egg-info/
--rw-r--r--   0 rlai       (501) staff       (20)     2266 2023-06-12 17:03:28.000000 mlproj_manager-0.0.8/mlproj_manager.egg-info/PKG-INFO
--rw-r--r--   0 rlai       (501) staff       (20)     2298 2023-06-12 17:03:28.000000 mlproj_manager-0.0.8/mlproj_manager.egg-info/SOURCES.txt
--rw-r--r--   0 rlai       (501) staff       (20)        1 2023-06-12 17:03:28.000000 mlproj_manager-0.0.8/mlproj_manager.egg-info/dependency_links.txt
--rw-r--r--   0 rlai       (501) staff       (20)       69 2023-06-12 17:03:28.000000 mlproj_manager-0.0.8/mlproj_manager.egg-info/requires.txt
--rw-r--r--   0 rlai       (501) staff       (20)       15 2023-06-12 17:03:28.000000 mlproj_manager-0.0.8/mlproj_manager.egg-info/top_level.txt
--rw-r--r--   0 rlai       (501) staff       (20)       87 2023-02-07 20:44:06.000000 mlproj_manager-0.0.8/pyproject.toml
--rw-r--r--   0 rlai       (501) staff       (20)      657 2023-06-12 17:03:28.523918 mlproj_manager-0.0.8/setup.cfg
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.203348 mlproj_manager-0.0.9/
+-rw-r--r--   0 rlai       (501) staff       (20)     1068 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/LICENSE
+-rw-r--r--   0 rlai       (501) staff       (20)     2266 2023-06-15 17:16:50.203540 mlproj_manager-0.0.9/PKG-INFO
+-rw-r--r--   0 rlai       (501) staff       (20)     1777 2023-06-05 20:14:53.000000 mlproj_manager-0.0.9/README.md
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.162581 mlproj_manager-0.0.9/mlproj_manager/
+-rw-r--r--   0 rlai       (501) staff       (20)       62 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)      301 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/definitions.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.169800 mlproj_manager-0.0.9/mlproj_manager/experiments/
+-rw-r--r--   0 rlai       (501) staff       (20)      102 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/experiments/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1699 2023-06-12 17:02:12.000000 mlproj_manager-0.0.9/mlproj_manager/experiments/abstract_experiment.py
+-rw-r--r--   0 rlai       (501) staff       (20)     3362 2023-06-15 17:15:18.000000 mlproj_manager-0.0.9/mlproj_manager/experiments/experiment_runner.py
+-rw-r--r--   0 rlai       (501) staff       (20)     2724 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/experiments/register_experiment.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.173103 mlproj_manager-0.0.9/mlproj_manager/file_management/
+-rw-r--r--   0 rlai       (501) staff       (20)      832 2023-06-14 20:46:43.000000 mlproj_manager-0.0.9/mlproj_manager/file_management/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     3318 2023-06-14 20:57:49.000000 mlproj_manager-0.0.9/mlproj_manager/file_management/concatenate_experiment_results.py
+-rw-r--r--   0 rlai       (501) staff       (20)     5286 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/file_management/experiment_management.py
+-rw-r--r--   0 rlai       (501) staff       (20)    16342 2023-06-14 20:46:43.000000 mlproj_manager-0.0.9/mlproj_manager/file_management/file_and_directory_management.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.174145 mlproj_manager-0.0.9/mlproj_manager/function_approximators/
+-rw-r--r--   0 rlai       (501) staff       (20)       30 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/function_approximators/__init__.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.179315 mlproj_manager-0.0.9/mlproj_manager/function_approximators/neural_networks/
+-rw-r--r--   0 rlai       (501) staff       (20)       92 2023-06-06 15:46:12.000000 mlproj_manager-0.0.9/mlproj_manager/function_approximators/neural_networks/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     9821 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/function_approximators/neural_networks/convolutional_network.py
+-rw-r--r--   0 rlai       (501) staff       (20)     6295 2023-06-06 15:46:12.000000 mlproj_manager-0.0.9/mlproj_manager/function_approximators/neural_networks/general_deep_network.py
+-rw-r--r--   0 rlai       (501) staff       (20)     8422 2023-03-01 03:30:11.000000 mlproj_manager-0.0.9/mlproj_manager/main.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.182927 mlproj_manager-0.0.9/mlproj_manager/plots_and_summaries/
+-rw-r--r--   0 rlai       (501) staff       (20)        0 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/plots_and_summaries/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)    12903 2023-02-21 20:11:42.000000 mlproj_manager-0.0.9/mlproj_manager/plots_and_summaries/plot_results.py
+-rw-r--r--   0 rlai       (501) staff       (20)     3960 2023-02-21 19:55:11.000000 mlproj_manager-0.0.9/mlproj_manager/plots_and_summaries/plotting_functions.py
+-rw-r--r--   0 rlai       (501) staff       (20)      659 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/plots_and_summaries/summaries.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.184337 mlproj_manager-0.0.9/mlproj_manager/problems/
+-rw-r--r--   0 rlai       (501) staff       (20)       35 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/problems/__init__.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.188651 mlproj_manager-0.0.9/mlproj_manager/problems/reinforcement_learning/
+-rw-r--r--   0 rlai       (501) staff       (20)       89 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/problems/reinforcement_learning/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1574 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py
+-rw-r--r--   0 rlai       (501) staff       (20)     6238 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/problems/reinforcement_learning/mountain_car.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.190573 mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/
+-rw-r--r--   0 rlai       (501) staff       (20)      243 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1301 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/abstract_dataset.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.191658 mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/cifar/
+-rw-r--r--   0 rlai       (501) staff       (20)     9890 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/cifar/cifar_data_loader.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.192828 mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/mnist/
+-rw-r--r--   0 rlai       (501) staff       (20)     7610 2023-02-09 19:08:17.000000 mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/mnist/mnist_data_loader.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.193872 mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/target_generating_network/
+-rw-r--r--   0 rlai       (501) staff       (20)     4336 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/target_generating_network/taget_generating_network.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.195487 mlproj_manager-0.0.9/mlproj_manager/util/
+-rw-r--r--   0 rlai       (501) staff       (20)      145 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/util/__init__.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.198645 mlproj_manager-0.0.9/mlproj_manager/util/data_preprocessing_and_transformations/
+-rw-r--r--   0 rlai       (501) staff       (20)      163 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/util/data_preprocessing_and_transformations/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     7164 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/util/data_preprocessing_and_transformations/image_transformations.py
+-rw-r--r--   0 rlai       (501) staff       (20)     3928 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/util/data_preprocessing_and_transformations/normalization_and_preprocessing.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1750 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/util/experiments_util.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.202397 mlproj_manager-0.0.9/mlproj_manager/util/neural_networks/
+-rw-r--r--   0 rlai       (501) staff       (20)      449 2023-06-05 20:01:39.000000 mlproj_manager-0.0.9/mlproj_manager/util/neural_networks/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1986 2023-06-05 20:07:28.000000 mlproj_manager-0.0.9/mlproj_manager/util/neural_networks/network_architecture.py
+-rw-r--r--   0 rlai       (501) staff       (20)      287 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/util/neural_networks/other_torch_utilities.py
+-rw-r--r--   0 rlai       (501) staff       (20)     6328 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/mlproj_manager/util/neural_networks/weights_initialization_and_manipulation.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-15 17:16:50.166907 mlproj_manager-0.0.9/mlproj_manager.egg-info/
+-rw-r--r--   0 rlai       (501) staff       (20)     2266 2023-06-15 17:16:50.000000 mlproj_manager-0.0.9/mlproj_manager.egg-info/PKG-INFO
+-rw-r--r--   0 rlai       (501) staff       (20)     2363 2023-06-15 17:16:50.000000 mlproj_manager-0.0.9/mlproj_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 rlai       (501) staff       (20)        1 2023-06-15 17:16:50.000000 mlproj_manager-0.0.9/mlproj_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 rlai       (501) staff       (20)       69 2023-06-15 17:16:50.000000 mlproj_manager-0.0.9/mlproj_manager.egg-info/requires.txt
+-rw-r--r--   0 rlai       (501) staff       (20)       15 2023-06-15 17:16:50.000000 mlproj_manager-0.0.9/mlproj_manager.egg-info/top_level.txt
+-rw-r--r--   0 rlai       (501) staff       (20)       87 2023-02-07 20:44:06.000000 mlproj_manager-0.0.9/pyproject.toml
+-rw-r--r--   0 rlai       (501) staff       (20)      657 2023-06-15 17:16:50.204579 mlproj_manager-0.0.9/setup.cfg
```

### Comparing `mlproj_manager-0.0.8/LICENSE` & `mlproj_manager-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/PKG-INFO` & `mlproj_manager-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlproj_manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package with utilities for managing and running machine learning projects
 Home-page: https://github.com/JFernando4/Research_Project_Manager
 Author: J. Fernando Hernandez-Garcia
 Author-email: jfhernan@ualberta.ca
 Keywords: ml,rl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mlproj_manager-0.0.8/README.md` & `mlproj_manager-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/experiments/abstract_experiment.py` & `mlproj_manager-0.0.9/mlproj_manager/experiments/abstract_experiment.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/experiments/experiment_runner.py` & `mlproj_manager-0.0.9/mlproj_manager/experiments/experiment_runner.py`

 * *Files 17% similar despite different names*

```diff
@@ -53,16 +53,19 @@
         assert hasattr(parsed_args, "exp_file_path") and hasattr(parsed_args, "exp_class_name"), \
             "Cannot register experiment without exp_file_path and exp_class_name"
         exp_file_path = parsed_args.exp_file_path
         exp_class_name = parsed_args.exp_class_name
         register_experiment(exp_name, exp_file_path, exp_class_name)
 
     # load experiment module
+    initial_time = time.perf_counter()
     experiment_module = SourceFileLoader(exp_class_name, exp_file_path).load_module()
     exp_class = getattr(experiment_module, exp_class_name)
+    final_time = time.perf_counter()
+    print("Time it took to load module in minutes: {0:.2f}".format((final_time - initial_time) / 60))
     assert issubclass(exp_class, Experiment)
     
     # initialize experiment
     initial_time = time.perf_counter()
     exp = exp_class(exp_params=exp_dict,
                     results_dir=exp_dir,
                     run_index=exp_dict["index"],
```

### Comparing `mlproj_manager-0.0.8/mlproj_manager/experiments/register_experiment.py` & `mlproj_manager-0.0.9/mlproj_manager/experiments/register_experiment.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/file_management/__init__.py` & `mlproj_manager-0.0.9/mlproj_manager/file_management/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # for directory management
-from .file_and_directory_management import get_experiment_dir
+from .file_and_directory_management import get_experiment_dir, get_file_paths_that_contain_keywords, get_indices
 # for saving and writing files
 from .file_and_directory_management import save_experiment_results, save_results_dict, save_index, write_slurm_file, \
     save_experiment_config_file
 # for loading files
 from .file_and_directory_management import read_json_file, load_experiment_results, get_names_for_parameter_sweep
 # for aggregating files
 from .file_and_directory_management import bin_1d_array, bin_results, aggregate_results, aggregate_large_results, \
-    get_first_of_each_epoch
+    get_first_of_each_epoch, concatenate_results
 # for experiment management
 from .experiment_management import get_missing_indices, get_dims_and_dtype_of_npy_file, \
     get_param_values, create_parameter_values, override_slurm_config
```

### Comparing `mlproj_manager-0.0.8/mlproj_manager/file_management/experiment_management.py` & `mlproj_manager-0.0.9/mlproj_manager/file_management/experiment_management.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/file_management/file_and_directory_management.py` & `mlproj_manager-0.0.9/mlproj_manager/file_management/file_and_directory_management.py`

 * *Files 14% similar despite different names*

```diff
@@ -131,14 +131,82 @@
     temp_path = os.path.join(results_dir, "config_files")
     os.makedirs(temp_path, exist_ok=True)
     with open(os.path.join(temp_path, "index-" + str(run_index) + ".json"), mode="w") as json_file:
         json.dump(obj=exp_params, fp=json_file, indent=1)
     print("Config file successfully stored!")
 
 
+def concatenate_results(results_dir: str, store_concatenated_results: bool = True, indices: list = None):
+    """
+    Given a directory containing results from different runs of an experiment where each file is named
+    "index-$RUN_NUMBER.py", it reads all the files and creates a list with all the results ordered based on the
+    $RUN_NUMBER in ascending order. If specified, it stores the list into a file named
+    "indices-$MIN_RUN_NUMBER-$MAX_RUN_NUMBER.py"
+
+    param results_dir: directory containing np files, each file corresponding to a different index
+    param store_concatenated_results: bool indicating whether to store the list in memory
+    param indices: list of int corresponding to the $RUN_NUMBER of each index
+    return: np array with results
+    """
+
+    if indices is None:
+        indices = get_indices(results_dir)
+    concatenated_results_file_name = "indices-{0}-{1}.npy".format(indices[0], indices[-1])
+    concatenated_results_file_path = os.path.join(results_dir, concatenated_results_file_name)
+    if os.path.isfile(concatenated_results_file_path):
+        return np.load(concatenated_results_file_path)
+
+    results = []
+    for index in indices:
+        temp_file_path = os.path.join(results_dir, "index-{0}.npy".format(index))
+        results.append(np.load(temp_file_path))
+
+    if store_concatenated_results:
+        np.save(concatenated_results_file_path, results)
+        print("Results successfully saved at: {0}".format(concatenated_results_file_path))
+
+    return np.array(results)
+
+
+def get_indices(results_dir: str):
+    """
+    Given a directory containing files named "index-$RUN_NUMBER.py", the function returns a list of indices ordered in
+    ascending order
+
+    param results_dir: path to some directory
+    return: list of int corresponding to the indices of the files in ascending order
+    """
+    indices = []
+    for file_name in os.listdir(results_dir):
+        if "index" not in file_name: continue
+        striped_file_name = file_name.split(".")[0]     # removes file format from file name
+        run_number = striped_file_name.split("-")[1]
+        indices.append(run_number)
+    indices.sort(reverse=False)
+    return indices
+
+
+def get_file_paths_that_contain_keywords(dir_path: str, keyword_tuple: tuple):
+
+    if not os.path.isdir(dir_path):
+        raise ValueError("The path does not correspond to a directory.\n\tPath: {0}".format(dir_path))
+
+    file_paths = []
+
+    for file_name in os.listdir(dir_path):
+        file_path = os.path.join(dir_path, file_name)
+
+        if not os.path.isfile(file_path): continue
+
+        if all(keyword in file_name for keyword in keyword_tuple):
+            file_paths.append(file_path)
+
+    return file_paths
+
+
 # ---*---*---*---*---*---*--- For loading files ---*---*---*---*---*---*--- #
 def read_json_file(filepath: str):
     """
     Read a json file and returns its data as a dictionary
     :param filepath: (str) path to the file
     :return: a dictionary with the data in the json file
     """
```

### Comparing `mlproj_manager-0.0.8/mlproj_manager/function_approximators/neural_networks/convolutional_network.py` & `mlproj_manager-0.0.9/mlproj_manager/function_approximators/neural_networks/convolutional_network.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/function_approximators/neural_networks/general_deep_network.py` & `mlproj_manager-0.0.9/mlproj_manager/function_approximators/neural_networks/general_deep_network.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/main.py` & `mlproj_manager-0.0.9/mlproj_manager/main.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/plots_and_summaries/plot_results.py` & `mlproj_manager-0.0.9/mlproj_manager/plots_and_summaries/plot_results.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/plots_and_summaries/plotting_functions.py` & `mlproj_manager-0.0.9/mlproj_manager/plots_and_summaries/plotting_functions.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/plots_and_summaries/summaries.py` & `mlproj_manager-0.0.9/mlproj_manager/plots_and_summaries/summaries.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py` & `mlproj_manager-0.0.9/mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/problems/reinforcement_learning/mountain_car.py` & `mlproj_manager-0.0.9/mlproj_manager/problems/reinforcement_learning/mountain_car.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/abstract_dataset.py` & `mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/abstract_dataset.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/cifar/cifar_data_loader.py` & `mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/cifar/cifar_data_loader.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/mnist/mnist_data_loader.py` & `mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/mnist/mnist_data_loader.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/problems/supervised_learning/target_generating_network/taget_generating_network.py` & `mlproj_manager-0.0.9/mlproj_manager/problems/supervised_learning/target_generating_network/taget_generating_network.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/util/data_preprocessing_and_transformations/image_transformations.py` & `mlproj_manager-0.0.9/mlproj_manager/util/data_preprocessing_and_transformations/image_transformations.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/util/data_preprocessing_and_transformations/normalization_and_preprocessing.py` & `mlproj_manager-0.0.9/mlproj_manager/util/data_preprocessing_and_transformations/normalization_and_preprocessing.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/util/experiments_util.py` & `mlproj_manager-0.0.9/mlproj_manager/util/experiments_util.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/util/neural_networks/network_architecture.py` & `mlproj_manager-0.0.9/mlproj_manager/util/neural_networks/network_architecture.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager/util/neural_networks/weights_initialization_and_manipulation.py` & `mlproj_manager-0.0.9/mlproj_manager/util/neural_networks/weights_initialization_and_manipulation.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.8/mlproj_manager.egg-info/PKG-INFO` & `mlproj_manager-0.0.9/mlproj_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlproj-manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package with utilities for managing and running machine learning projects
 Home-page: https://github.com/JFernando4/Research_Project_Manager
 Author: J. Fernando Hernandez-Garcia
 Author-email: jfhernan@ualberta.ca
 Keywords: ml,rl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mlproj_manager-0.0.8/mlproj_manager.egg-info/SOURCES.txt` & `mlproj_manager-0.0.9/mlproj_manager.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 mlproj_manager.egg-info/requires.txt
 mlproj_manager.egg-info/top_level.txt
 mlproj_manager/experiments/__init__.py
 mlproj_manager/experiments/abstract_experiment.py
 mlproj_manager/experiments/experiment_runner.py
 mlproj_manager/experiments/register_experiment.py
 mlproj_manager/file_management/__init__.py
+mlproj_manager/file_management/concatenate_experiment_results.py
 mlproj_manager/file_management/experiment_management.py
 mlproj_manager/file_management/file_and_directory_management.py
 mlproj_manager/function_approximators/__init__.py
 mlproj_manager/function_approximators/neural_networks/__init__.py
 mlproj_manager/function_approximators/neural_networks/convolutional_network.py
 mlproj_manager/function_approximators/neural_networks/general_deep_network.py
 mlproj_manager/plots_and_summaries/__init__.py
```

### Comparing `mlproj_manager-0.0.8/setup.cfg` & `mlproj_manager-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlproj_manager
-version = 0.0.8
+version = 0.0.9
 author = J. Fernando Hernandez-Garcia
 author_email = jfhernan@ualberta.ca
 description = A package with utilities for managing and running machine learning projects
 long_description = file: README.md
 url = https://github.com/JFernando4/Research_Project_Manager
 license_files = LICENSE
 keywords = ml, rl
```

