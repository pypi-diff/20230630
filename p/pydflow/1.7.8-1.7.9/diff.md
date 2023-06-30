# Comparing `tmp/pydflow-1.7.8.tar.gz` & `tmp/pydflow-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydflow-1.7.8.tar", last modified: Thu Jun 29 05:36:58 2023, max compression
+gzip compressed data, was "pydflow-1.7.9.tar", last modified: Thu Jun 29 11:05:24 2023, max compression
```

## Comparing `pydflow-1.7.8.tar` & `pydflow-1.7.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:36:58.449645 pydflow-1.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-29 05:36:49.000000 pydflow-1.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 05:36:49.000000 pydflow-1.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-29 05:36:58.449645 pydflow-1.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-06-29 05:36:49.000000 pydflow-1.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 05:36:49.000000 pydflow-1.7.8/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 05:36:58.449645 pydflow-1.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-29 05:36:49.000000 pydflow-1.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:36:58.441645 pydflow-1.7.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:36:58.445645 pydflow-1.7.8/src/dflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/argo_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:36:58.445645 pydflow-1.7.8/src/dflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/client/v1alpha1_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/client/v1alpha1_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/client/v1alpha1_retry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/client/v1alpha1_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/client/v1alpha1_value_from.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/context_syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    51335 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/op_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:36:58.449645 pydflow-1.7.8/src/dflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/plugins/bohrium.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/plugins/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    23061 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/plugins/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/plugins/launching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/plugins/lebesgue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/plugins/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/plugins/oss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/plugins/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:36:58.449645 pydflow-1.7.8/src/dflow/python/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/python/op.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/python/opio.py
--rw-r--r--   0 runner    (1001) docker     (123)    31750 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/python/python_op_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/python/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)   102485 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/util_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    25540 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    45198 2023-06-29 05:36:49.000000 pydflow-1.7.8/src/dflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:36:58.449645 pydflow-1.7.8/src/pydflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-29 05:36:58.000000 pydflow-1.7.8/src/pydflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-29 05:36:58.000000 pydflow-1.7.8/src/pydflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 05:36:58.000000 pydflow-1.7.8/src/pydflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 05:36:58.000000 pydflow-1.7.8/src/pydflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-29 05:36:58.000000 pydflow-1.7.8/src/pydflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 05:36:58.000000 pydflow-1.7.8/src/pydflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:36:58.449645 pydflow-1.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-29 05:36:49.000000 pydflow-1.7.8/tests/test_big_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-29 05:36:49.000000 pydflow-1.7.8/tests/test_conditional_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-29 05:36:49.000000 pydflow-1.7.8/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-29 05:36:49.000000 pydflow-1.7.8/tests/test_group_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-06-29 05:36:49.000000 pydflow-1.7.8/tests/test_makevasp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-29 05:36:49.000000 pydflow-1.7.8/tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-29 05:36:49.000000 pydflow-1.7.8/tests/test_recurse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-29 05:36:49.000000 pydflow-1.7.8/tests/test_reuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-29 05:36:49.000000 pydflow-1.7.8/tests/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-29 05:36:49.000000 pydflow-1.7.8/tests/test_subpath_slices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:05:24.802526 pydflow-1.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-29 11:05:10.000000 pydflow-1.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 11:05:10.000000 pydflow-1.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-29 11:05:24.802526 pydflow-1.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-06-29 11:05:10.000000 pydflow-1.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 11:05:10.000000 pydflow-1.7.9/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:05:24.802526 pydflow-1.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-29 11:05:10.000000 pydflow-1.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:05:24.790525 pydflow-1.7.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:05:24.794525 pydflow-1.7.9/src/dflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/argo_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:05:24.794525 pydflow-1.7.9/src/dflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/client/v1alpha1_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/client/v1alpha1_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/client/v1alpha1_retry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/client/v1alpha1_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/client/v1alpha1_value_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/context_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51335 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/op_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:05:24.798525 pydflow-1.7.9/src/dflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/plugins/bohrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/plugins/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23061 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/plugins/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/plugins/launching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/plugins/lebesgue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/plugins/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/plugins/oss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/plugins/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:05:24.798525 pydflow-1.7.9/src/dflow/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/python/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/python/opio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31750 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/python/python_op_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/python/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103754 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/util_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25540 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45198 2023-06-29 11:05:10.000000 pydflow-1.7.9/src/dflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:05:24.798525 pydflow-1.7.9/src/pydflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-29 11:05:24.000000 pydflow-1.7.9/src/pydflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-29 11:05:24.000000 pydflow-1.7.9/src/pydflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:05:24.000000 pydflow-1.7.9/src/pydflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 11:05:24.000000 pydflow-1.7.9/src/pydflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-29 11:05:24.000000 pydflow-1.7.9/src/pydflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 11:05:24.000000 pydflow-1.7.9/src/pydflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:05:24.802526 pydflow-1.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-29 11:05:10.000000 pydflow-1.7.9/tests/test_big_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-29 11:05:10.000000 pydflow-1.7.9/tests/test_conditional_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-29 11:05:10.000000 pydflow-1.7.9/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-29 11:05:10.000000 pydflow-1.7.9/tests/test_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-06-29 11:05:10.000000 pydflow-1.7.9/tests/test_makevasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-29 11:05:10.000000 pydflow-1.7.9/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-29 11:05:10.000000 pydflow-1.7.9/tests/test_recurse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-29 11:05:10.000000 pydflow-1.7.9/tests/test_reuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-29 11:05:10.000000 pydflow-1.7.9/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-29 11:05:10.000000 pydflow-1.7.9/tests/test_subpath_slices.py
```

### Comparing `pydflow-1.7.8/LICENSE` & `pydflow-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/PKG-INFO` & `pydflow-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.7.8
+Version: 1.7.9
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
 Home-page: https://github.com/deepmodeling/dflow
 Author: Xinzijian Liu
 Author-email: liuxzj@dp.tech
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pydflow-1.7.8/README.md` & `pydflow-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/setup.py` & `pydflow-1.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/__init__.py` & `pydflow-1.7.9/src/dflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/argo_objects.py` & `pydflow-1.7.9/src/dflow/argo_objects.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/client/v1alpha1_artifact.py` & `pydflow-1.7.9/src/dflow/client/v1alpha1_artifact.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/client/v1alpha1_parameter.py` & `pydflow-1.7.9/src/dflow/client/v1alpha1_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/client/v1alpha1_retry_strategy.py` & `pydflow-1.7.9/src/dflow/client/v1alpha1_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/client/v1alpha1_sequence.py` & `pydflow-1.7.9/src/dflow/client/v1alpha1_sequence.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/client/v1alpha1_value_from.py` & `pydflow-1.7.9/src/dflow/client/v1alpha1_value_from.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/common.py` & `pydflow-1.7.9/src/dflow/common.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/config.py` & `pydflow-1.7.9/src/dflow/config.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/context_syntax.py` & `pydflow-1.7.9/src/dflow/context_syntax.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/dag.py` & `pydflow-1.7.9/src/dflow/dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/executor.py` & `pydflow-1.7.9/src/dflow/executor.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/io.py` & `pydflow-1.7.9/src/dflow/io.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/main.py` & `pydflow-1.7.9/src/dflow/main.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/op_template.py` & `pydflow-1.7.9/src/dflow/op_template.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/plugins/bohrium.py` & `pydflow-1.7.9/src/dflow/plugins/bohrium.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/plugins/datasets.py` & `pydflow-1.7.9/src/dflow/plugins/datasets.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/plugins/dispatcher.py` & `pydflow-1.7.9/src/dflow/plugins/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/plugins/launching.py` & `pydflow-1.7.9/src/dflow/plugins/launching.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/plugins/lebesgue.py` & `pydflow-1.7.9/src/dflow/plugins/lebesgue.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/plugins/metadata.py` & `pydflow-1.7.9/src/dflow/plugins/metadata.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/plugins/oss.py` & `pydflow-1.7.9/src/dflow/plugins/oss.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/plugins/ray.py` & `pydflow-1.7.9/src/dflow/plugins/ray.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/python/op.py` & `pydflow-1.7.9/src/dflow/python/op.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/python/opio.py` & `pydflow-1.7.9/src/dflow/python/opio.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/python/python_op_template.py` & `pydflow-1.7.9/src/dflow/python/python_op_template.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/python/utils.py` & `pydflow-1.7.9/src/dflow/python/utils.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/resource.py` & `pydflow-1.7.9/src/dflow/resource.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/slurm.py` & `pydflow-1.7.9/src/dflow/slurm.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/step.py` & `pydflow-1.7.9/src/dflow/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,27 +359,25 @@
         if self.key is not None:
             self.template.inputs.parameters["dflow_key"] = InputParameter(
                 value="")
             self.inputs.parameters["dflow_key"] = InputParameter(
                 value=str(self.key))
 
         if slices is not None:
-            from .dag import DAG
-            from .steps import Steps
-            assert isinstance(self.template, (DAG, Steps)), \
-                "Please specify slices in PythonOPTemplate "\
-                "if the template is a Python OP template"
             self.template = self.template.copy()
             self.template.slices = slices
+            self.template.add_slices(slices)
             for name, par in self.template.inputs.parameters.items():
                 if name not in self.inputs.parameters:
                     self.inputs.parameters[name] = deepcopy(par)
-            self.template.add_slices(slices)
-            self.inputs.parameters["dflow_slice"] = InputParameter(
-                value=slices.slices)
+            from .dag import DAG
+            from .steps import Steps
+            if isinstance(self.template, (DAG, Steps)):
+                self.inputs.parameters["dflow_slice"] = InputParameter(
+                    value=slices.slices)
 
         sum_var = None
         if isinstance(self.with_param, ArgoRange) and \
                 isinstance(self.with_param.end, ArgoSum):
             sum_var = self.with_param.end.param
 
         if self.with_sequence is not None and \
@@ -393,155 +391,46 @@
             concat_var = self.with_param.end.param.param
 
         if self.with_sequence is not None and \
                 isinstance(self.with_sequence.count, ArgoLen) and \
                 isinstance(self.with_sequence.count.param, ArgoConcat):
             concat_var = self.with_sequence.count.param.param
 
-        if hasattr(self.template, "slices") and self.template.slices is not \
-                None and self.template.slices.group_size is not None:
-            self.template = self.template.copy()
-            group_size = self.template.slices.group_size
-            self.template.inputs.parameters["dflow_nslices"] = InputParameter()
-            if self.template.slices.shuffle:
-                self.template.pre_script += "import random\n"
-                self.template.pre_script += "random.seed(%s)\n" % \
-                    self.template.slices.random_seed
-                # pre script is formatted
-                self.template.pre_script += "shuffled = "\
-                    "list(range({{{{inputs.parameters.dflow_nslices}}}}))\n"
-                self.template.pre_script += "random.shuffle(shuffled)\n"
-                self.template.pre_script += "random.seed()\n"  # unset seed
-            if isinstance(self.with_param, ArgoRange):
-                self.template.inputs.parameters["dflow_range_end"] = \
-                    InputParameter()
-                self.inputs.parameters["dflow_range_end"] = \
-                    InputParameter(value=self.with_param.end)
-                self.template.inputs.parameters["dflow_range_start"] = \
-                    InputParameter()
-                self.inputs.parameters["dflow_range_start"] = \
-                    InputParameter(value=self.with_param.start)
-                self.template.inputs.parameters["dflow_range_step"] = \
-                    InputParameter()
-                self.inputs.parameters["dflow_range_step"] = \
-                    InputParameter(value=self.with_param.step)
-                nslices = argo_len(self.with_param)
-                old_slices = self.template.slices.slices
-                self.template.slices.slices = \
-                    "[range({{inputs.parameters.dflow_range_start}}, "\
-                    "{{inputs.parameters.dflow_range_end}}, "\
-                    "{{inputs.parameters.dflow_range_step}})"\
-                    "[%s] for i in range({{item}}*%s, min(({{item}}+1)*%s"\
-                    ", {{inputs.parameters.dflow_nslices}}))]" % (
-                        old_slices.replace("{{item}}", "shuffled[i]"
-                                           if self.template.slices.shuffle
-                                           else "i"), group_size, group_size)
-                # re-render the script
-                self.template.set_slices(self.template.slices)
-                self.with_param = argo_range(if_expression(
-                    "%s %% %s > 0" % (nslices, group_size),
-                    "%s/%s + 1" % (nslices, group_size),
-                    "%s/%s" % (nslices, group_size)))
-            elif self.with_param is not None:
-                self.template.inputs.parameters["dflow_with_param"] = \
-                    InputParameter()
-                self.inputs.parameters["dflow_with_param"] = \
-                    InputParameter(value=self.with_param)
-                if hasattr(self.with_param, "__len__"):
-                    nslices = len(self.with_param)
-                else:
-                    nslices = argo_len(self.with_param)
-                old_slices = self.template.slices.slices
-                self.template.slices.slices = \
-                    "[json.loads(r'''{{inputs.parameters.dflow_with_param}}"\
-                    "''')[%s] for i in range({{item}}*%s, min(({{item}}+1)*%s"\
-                    ", {{inputs.parameters.dflow_nslices}}))]" % (
-                        old_slices.replace("{{item}}", "shuffled[i]"
-                                           if self.template.slices.shuffle
-                                           else "i"), group_size, group_size)
-                # re-render the script
-                self.template.set_slices(self.template.slices)
-                self.with_param = argo_range(if_expression(
-                    "%s %% %s > 0" % (nslices, group_size),
-                    "%s/%s + 1" % (nslices, group_size),
-                    "%s/%s" % (nslices, group_size)))
-            if self.with_sequence is not None:
-                self.template.inputs.parameters["dflow_sequence_start"] = \
-                    InputParameter()
-                self.template.inputs.parameters["dflow_sequence_end"] = \
-                    InputParameter()
-                self.template.inputs.parameters["dflow_sequence_count"] = \
-                    InputParameter()
-                start = self.with_sequence.start
-                if start is None:
-                    start = 0
-                end = self.with_sequence.end
-                count = self.with_sequence.count
-                format = self.with_sequence.format
-                self.inputs.parameters["dflow_sequence_start"] = \
-                    InputParameter(value=start)
-                self.inputs.parameters["dflow_sequence_end"] = \
-                    InputParameter(value=end)
-                self.inputs.parameters["dflow_sequence_count"] = \
-                    InputParameter(value=count)
-                if count is not None:
-                    nslices = count
-                else:
-                    nslices = if_expression(
-                        "%s > %s" % (end, start),
-                        "%s + 1 - %s" % (end, start),
-                        "%s + 1 - %s" % (start, end))
-                old_slices = self.template.slices.slices
-                self.template.slices.slices = \
-                    "[[%s for j in (range(int('{{inputs.parameters."\
-                    "dflow_sequence_start}}'), int('{{inputs.parameters."\
-                    "dflow_sequence_start}}') + int('{{inputs.parameters."\
-                    "dflow_sequence_count}}') + 1) if '{{inputs.parameters."\
-                    "dflow_sequence_count}}' != 'null' else range(int('{{"\
-                    "inputs.parameters.dflow_sequence_start}}'), int('{{"\
-                    "inputs.parameters.dflow_sequence_end}}') + 1) if int('{{"\
-                    "inputs.parameters.dflow_sequence_end}}') > int('{{"\
-                    "inputs.parameters.dflow_sequence_start}}') else range("\
-                    "int('{{inputs.parameters.dflow_sequence_start}}'), "\
-                    "int('{{inputs.parameters.dflow_sequence_end}}') - 1, -1)"\
-                    ")][%s] for i in range(int('{{item}}')*%s, min((int('{{"\
-                    "item}}')+1)*%s, {{inputs.parameters.dflow_nslices}}))]"\
-                    % (old_slices.replace(
-                        "'{{item}}'", "('%s' %% j)" % format)
-                        if format is not None
-                        else old_slices.replace("{{item}}", "j"),
-                        "shuffled[i]" if self.template.slices.shuffle else "i",
-                        group_size, group_size)
-                # re-render the script
-                self.template.set_slices(self.template.slices)
-                self.with_sequence = argo_sequence(
-                    count=if_expression(
-                        "%s %% %s > 0" % (nslices, group_size),
-                        "%s/%s + 1" % (nslices, group_size),
-                        "%s/%s" % (nslices, group_size)), format=format)
-
-            self.inputs.parameters["dflow_nslices"] = InputParameter(
-                value=nslices)
-
         sliced_output_artifact = self.template.slices.output_artifact if \
             hasattr(self.template, "slices") and \
             self.template.slices is not None else []
 
         sliced_input_artifact = self.template.slices.input_artifact if \
             hasattr(self.template, "slices") and \
             self.template.slices is not None and \
             self.template.slices.sub_path else []
 
+        auto_loop_artifacts = []
+        if hasattr(self.template, "slices") and self.template.slices is not \
+                None and not self.template.slices.sub_path and \
+                self.with_param is None and self.with_sequence is None:
+            if self.template.slices.input_parameter:
+                name = self.template.slices.input_parameter[0]
+                value = self.inputs.parameters[name].value
+                self.with_param = argo_range(argo_len(value))
+            else:
+                assert len(self.template.slices.input_artifact) > 0, "sliced "\
+                    "input parameter or artifact must not be empty to infer "\
+                    "with_param"
+                auto_loop_artifacts = self.template.slices.input_artifact
+
         if sliced_output_artifact or sliced_input_artifact or \
-                sum_var is not None or concat_var is not None:
+                sum_var is not None or concat_var is not None or \
+                auto_loop_artifacts:
             self.template = self.template.copy()
             init_template = InitArtifactForSlices(
                 self.template, self.util_image, self.util_command,
                 self.util_image_pull_policy, self.key, sliced_output_artifact,
-                sliced_input_artifact, sum_var, concat_var)
+                sliced_input_artifact, sum_var, concat_var,
+                auto_loop_artifacts)
             if self.key is not None:
                 self.template.inputs.parameters["dflow_group_key"] = \
                     InputParameter(value="")
                 self.inputs.parameters["dflow_group_key"] = InputParameter(
                     value=re.sub("{{=?item.*}}", "group", str(self.key)))
                 self.template.inputs.parameters["dflow_artifact_key"] = \
                     InputParameter(value="")
@@ -694,14 +583,149 @@
                     value=str(concat_var))
                 self.with_sequence = argo_sequence(
                     argo_len(self.prepare_step.outputs.parameters[
                         "concat_%s" % name]),
                     self.with_sequence.start, self.with_sequence.end,
                     self.with_sequence.format)
 
+            if auto_loop_artifacts:
+                for name in self.inputs.artifacts:
+                    if name in auto_loop_artifacts or (name.startswith(
+                            "dflow_") and name[6:name.rfind("_")] in
+                            auto_loop_artifacts):
+                        self.prepare_step.inputs.artifacts[name].source = \
+                            self.inputs.artifacts[name].source
+                self.with_param = argo_range(
+                    self.prepare_step.outputs.parameters["dflow_nslices"])
+
+        if hasattr(self.template, "slices") and self.template.slices is not \
+                None and self.template.slices.group_size is not None:
+            self.template = self.template.copy()
+            group_size = self.template.slices.group_size
+            self.template.inputs.parameters["dflow_nslices"] = InputParameter()
+            if self.template.slices.shuffle:
+                self.template.pre_script += "import random\n"
+                self.template.pre_script += "random.seed(%s)\n" % \
+                    self.template.slices.random_seed
+                # pre script is formatted
+                self.template.pre_script += "shuffled = "\
+                    "list(range({{{{inputs.parameters.dflow_nslices}}}}))\n"
+                self.template.pre_script += "random.shuffle(shuffled)\n"
+                self.template.pre_script += "random.seed()\n"  # unset seed
+            if isinstance(self.with_param, ArgoRange):
+                self.template.inputs.parameters["dflow_range_end"] = \
+                    InputParameter()
+                self.inputs.parameters["dflow_range_end"] = \
+                    InputParameter(value=self.with_param.end)
+                self.template.inputs.parameters["dflow_range_start"] = \
+                    InputParameter()
+                self.inputs.parameters["dflow_range_start"] = \
+                    InputParameter(value=self.with_param.start)
+                self.template.inputs.parameters["dflow_range_step"] = \
+                    InputParameter()
+                self.inputs.parameters["dflow_range_step"] = \
+                    InputParameter(value=self.with_param.step)
+                nslices = argo_len(self.with_param)
+                old_slices = self.template.slices.slices
+                self.template.slices.slices = \
+                    "[range({{inputs.parameters.dflow_range_start}}, "\
+                    "{{inputs.parameters.dflow_range_end}}, "\
+                    "{{inputs.parameters.dflow_range_step}})"\
+                    "[%s] for i in range({{item}}*%s, min(({{item}}+1)*%s"\
+                    ", {{inputs.parameters.dflow_nslices}}))]" % (
+                        old_slices.replace("{{item}}", "shuffled[i]"
+                                           if self.template.slices.shuffle
+                                           else "i"), group_size, group_size)
+                # re-render the script
+                self.template.set_slices(self.template.slices)
+                self.with_param = argo_range(if_expression(
+                    "%s %% %s > 0" % (nslices, group_size),
+                    "%s/%s + 1" % (nslices, group_size),
+                    "%s/%s" % (nslices, group_size)))
+            elif self.with_param is not None:
+                self.template.inputs.parameters["dflow_with_param"] = \
+                    InputParameter()
+                self.inputs.parameters["dflow_with_param"] = \
+                    InputParameter(value=self.with_param)
+                if hasattr(self.with_param, "__len__"):
+                    nslices = len(self.with_param)
+                else:
+                    nslices = argo_len(self.with_param)
+                old_slices = self.template.slices.slices
+                self.template.slices.slices = \
+                    "[json.loads(r'''{{inputs.parameters.dflow_with_param}}"\
+                    "''')[%s] for i in range({{item}}*%s, min(({{item}}+1)*%s"\
+                    ", {{inputs.parameters.dflow_nslices}}))]" % (
+                        old_slices.replace("{{item}}", "shuffled[i]"
+                                           if self.template.slices.shuffle
+                                           else "i"), group_size, group_size)
+                # re-render the script
+                self.template.set_slices(self.template.slices)
+                self.with_param = argo_range(if_expression(
+                    "%s %% %s > 0" % (nslices, group_size),
+                    "%s/%s + 1" % (nslices, group_size),
+                    "%s/%s" % (nslices, group_size)))
+            if self.with_sequence is not None:
+                self.template.inputs.parameters["dflow_sequence_start"] = \
+                    InputParameter()
+                self.template.inputs.parameters["dflow_sequence_end"] = \
+                    InputParameter()
+                self.template.inputs.parameters["dflow_sequence_count"] = \
+                    InputParameter()
+                start = self.with_sequence.start
+                if start is None:
+                    start = 0
+                end = self.with_sequence.end
+                count = self.with_sequence.count
+                format = self.with_sequence.format
+                self.inputs.parameters["dflow_sequence_start"] = \
+                    InputParameter(value=start)
+                self.inputs.parameters["dflow_sequence_end"] = \
+                    InputParameter(value=end)
+                self.inputs.parameters["dflow_sequence_count"] = \
+                    InputParameter(value=count)
+                if count is not None:
+                    nslices = count
+                else:
+                    nslices = if_expression(
+                        "%s > %s" % (end, start),
+                        "%s + 1 - %s" % (end, start),
+                        "%s + 1 - %s" % (start, end))
+                old_slices = self.template.slices.slices
+                self.template.slices.slices = \
+                    "[[%s for j in (range(int('{{inputs.parameters."\
+                    "dflow_sequence_start}}'), int('{{inputs.parameters."\
+                    "dflow_sequence_start}}') + int('{{inputs.parameters."\
+                    "dflow_sequence_count}}') + 1) if '{{inputs.parameters."\
+                    "dflow_sequence_count}}' != 'null' else range(int('{{"\
+                    "inputs.parameters.dflow_sequence_start}}'), int('{{"\
+                    "inputs.parameters.dflow_sequence_end}}') + 1) if int('{{"\
+                    "inputs.parameters.dflow_sequence_end}}') > int('{{"\
+                    "inputs.parameters.dflow_sequence_start}}') else range("\
+                    "int('{{inputs.parameters.dflow_sequence_start}}'), "\
+                    "int('{{inputs.parameters.dflow_sequence_end}}') - 1, -1)"\
+                    ")][%s] for i in range(int('{{item}}')*%s, min((int('{{"\
+                    "item}}')+1)*%s, {{inputs.parameters.dflow_nslices}}))]"\
+                    % (old_slices.replace(
+                        "'{{item}}'", "('%s' %% j)" % format)
+                        if format is not None
+                        else old_slices.replace("{{item}}", "j"),
+                        "shuffled[i]" if self.template.slices.shuffle else "i",
+                        group_size, group_size)
+                # re-render the script
+                self.template.set_slices(self.template.slices)
+                self.with_sequence = argo_sequence(
+                    count=if_expression(
+                        "%s %% %s > 0" % (nslices, group_size),
+                        "%s/%s + 1" % (nslices, group_size),
+                        "%s/%s" % (nslices, group_size)), format=format)
+
+            self.inputs.parameters["dflow_nslices"] = InputParameter(
+                value=nslices)
+
         if config["register_tasks"] and hasattr(self.template, "slices") and \
                 self.template.slices and \
                 self.template.slices.register_first_only:
             self.template = self.template.copy()
             if self.with_param is not None:
                 if isinstance(self.with_param, ArgoVar):
                     par = self.with_param.expr
```

### Comparing `pydflow-1.7.8/src/dflow/steps.py` & `pydflow-1.7.9/src/dflow/steps.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/task.py` & `pydflow-1.7.9/src/dflow/task.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/util_ops.py` & `pydflow-1.7.9/src/dflow/util_ops.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+import jsonpickle
+import typeguard
+
+from . import __path__
 from .common import S3Artifact
 from .config import config
 from .io import (InputArtifact, InputParameter, Inputs, OutputArtifact,
                  OutputParameter)
 from .op_template import PythonScriptOPTemplate, ShellOPTemplate
 
 
 class InitArtifactForSlices(PythonScriptOPTemplate):
     def __init__(self, template, image, command, image_pull_policy, key,
                  sliced_output_artifact, sliced_input_artifact, sum_var,
-                 concat_var, tmp_root="/tmp"):
+                 concat_var, auto_loop_artifacts, tmp_root="/tmp"):
         name = template.name
         super().__init__(name="%s-init-artifact" % name, image=image,
                          command=command, image_pull_policy=image_pull_policy)
         self.origin = template
         self.key = key
         self.sliced_output_artifact = sliced_output_artifact
         self.sliced_input_artifact = sliced_input_artifact
         self.sum_var = sum_var
         self.concat_var = concat_var
+        self.auto_loop_artifacts = auto_loop_artifacts
         self.tmp_root = tmp_root
 
         if self.key is not None:
             self.inputs.parameters["dflow_group_key"] = InputParameter()
             # For the case of reusing sliced steps, ensure that the output
             # artifacts are reused
             for name in self.sliced_output_artifact:
@@ -68,14 +73,34 @@
         if self.concat_var is not None:
             name = self.concat_var.name
             self.inputs.parameters[name] = InputParameter()
             self.outputs.parameters["concat_%s" % name] = OutputParameter(
                 value_from_path="%s/outputs/parameters/concat_%s" %
                 (self.tmp_root, name), type=list)
 
+        if self.auto_loop_artifacts:
+            python_packages = []
+            python_packages += __path__
+            python_packages += jsonpickle.__path__
+            python_packages += typeguard.__path__
+            self.python_packages = set(python_packages)
+            self.inputs.artifacts["dflow_python_packages"] = InputArtifact(
+                path="%s/inputs/artifacts/dflow_python_packages"
+                % self.tmp_root)
+            for name in self.origin.inputs.artifacts:
+                if name in self.auto_loop_artifacts or (name.startswith(
+                        "dflow_") and name[6:name.rfind("_")] in
+                        self.auto_loop_artifacts):
+                    self.inputs.artifacts[name] = InputArtifact(
+                        path="%s/inputs/artifacts/%s" % (self.tmp_root, name),
+                        optional=True)
+            self.outputs.parameters["dflow_nslices"] = OutputParameter(
+                value_from_path="%s/outputs/parameters/dflow_nslices" %
+                self.tmp_root, type=int)
+
         self.render_script()
 
     def render_script(self):
         script = "import os, json\n"
         for name in self.sliced_output_artifact:
             script += "os.makedirs(r'%s/outputs/artifacts/%s/%s', "\
                 "exist_ok=True)\n" % (self.tmp_root, name,
@@ -151,14 +176,45 @@
         else:
             var += item
 os.makedirs(r'%s/outputs/parameters', exist_ok=True)
 with open(r'%s/outputs/parameters/concat_%s', 'w') as f:
     f.write(json.dumps(var))\n""" % (
                 name, self.tmp_root, self.tmp_root, name)
 
+        if self.auto_loop_artifacts:
+            from .python.python_op_template import handle_packages_script
+            script += handle_packages_script(
+                "%s/inputs/artifacts/dflow_python_packages" % self.tmp_root)
+            script += "from dflow.python import Artifact\n"
+            script += "from dflow.python.utils import handle_input_artifact\n"
+            script += "from pathlib import Path\n"
+            script += "from typing import List\n"
+            script += "input = {}\n"
+            required = []
+            for name in self.auto_loop_artifacts:
+                script += "input['%s'] = handle_input_artifact('%s', "\
+                    "Artifact(List[Path]), None, r'%s', None, n_parts=%s, "\
+                    "keys_of_parts=%s, prefix=%s)\n" % (
+                        name, name, self.tmp_root,
+                        self.origin.n_parts.get(name, None),
+                        self.origin.keys_of_parts.get(name, None),
+                        self.origin.input_artifact_prefix.get(name, None))
+                if not self.origin.input_sign[name].optional:
+                    required.append(name)
+
+            if len(required) > 1:
+                script += "assert " + " == ".join(
+                    ["len(input['%s'])" % name for name in required]) + "\n"
+
+            script += "os.makedirs(r'%s/outputs/parameters', "\
+                "exist_ok=True)\n" % self.tmp_root
+            script += "with open(r'%s/outputs/parameters/dflow_nslices', 'w')"\
+                " as f:\n" % self.tmp_root
+            script += "    f.write(str(len(input['%s'])))\n" % required[0]
+
         self.script = script
 
 
 class CheckNumSuccess(ShellOPTemplate):
     def __init__(self, name="check-num-success", image=None,
                  image_pull_policy=None):
         super().__init__(name=name, image=image,
```

### Comparing `pydflow-1.7.8/src/dflow/utils.py` & `pydflow-1.7.9/src/dflow/utils.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/dflow/workflow.py` & `pydflow-1.7.9/src/dflow/workflow.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/src/pydflow.egg-info/PKG-INFO` & `pydflow-1.7.9/src/pydflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.7.8
+Version: 1.7.9
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
 Home-page: https://github.com/deepmodeling/dflow
 Author: Xinzijian Liu
 Author-email: liuxzj@dp.tech
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pydflow-1.7.8/src/pydflow.egg-info/SOURCES.txt` & `pydflow-1.7.9/src/pydflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/tests/test_big_parameter.py` & `pydflow-1.7.9/tests/test_big_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/tests/test_conditional_outputs.py` & `pydflow-1.7.9/tests/test_conditional_outputs.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/tests/test_dag.py` & `pydflow-1.7.9/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/tests/test_group_size.py` & `pydflow-1.7.9/tests/test_group_size.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/tests/test_makevasp.py` & `pydflow-1.7.9/tests/test_makevasp.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/tests/test_python.py` & `pydflow-1.7.9/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/tests/test_recurse.py` & `pydflow-1.7.9/tests/test_recurse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/tests/test_reuse.py` & `pydflow-1.7.9/tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/tests/test_slices.py` & `pydflow-1.7.9/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.8/tests/test_subpath_slices.py` & `pydflow-1.7.9/tests/test_subpath_slices.py`

 * *Files identical despite different names*

